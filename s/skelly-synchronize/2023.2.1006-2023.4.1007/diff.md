# Comparing `tmp/skelly_synchronize-2023.2.1006.tar.gz` & `tmp/skelly_synchronize-2023.4.1007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.2.1006.tar", last modified: Tue Feb 28 23:01:49 2023, max compression
+gzip compressed data, was "skelly_synchronize-2023.4.1007.tar", last modified: Wed Apr 26 15:56:17 2023, max compression
```

## Comparing `skelly_synchronize-2023.2.1006.tar` & `skelly_synchronize-2023.4.1007.tar`

### file list

```diff
@@ -1,21 +1,26 @@
--rw-r--r--   0        0        0       65 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/.gitattributes
--rw-r--r--   0        0        0      146 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0      924 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/.gitignore
--rw-r--r--   0        0        0    34523 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/LICENSE
--rw-r--r--   0        0        0     2072 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/README.md
--rw-r--r--   0        0        0     1571 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/pyproject.toml
--rw-r--r--   0        0        0       90 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/requirements.txt
--rw-r--r--   0        0        0       50 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/setup.py
--rw-r--r--   0        0        0      976 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     1799 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0    13771 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0     1018 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/tests/unit_tests.py
--rw-r--r--   0        0        0     1340 2023-02-28 23:01:42.185000 skelly_synchronize-2023.2.1006/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     2886 1970-01-01 00:00:00.000000 skelly_synchronize-2023.2.1006/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/.gitattributes
+-rw-r--r--   0        0        0      146 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0      924 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/.gitignore
+-rw-r--r--   0        0        0    34523 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/LICENSE
+-rw-r--r--   0        0        0     2571 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/README.md
+-rw-r--r--   0        0        0     1600 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/requirements.txt
+-rw-r--r--   0        0        0       50 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/setup.py
+-rw-r--r--   0        0        0      976 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     1799 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0    18027 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0     1449 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0     1018 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/tests/unit_tests.py
+-rw-r--r--   0        0        0      577 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1340 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1871 2023-04-26 15:56:06.646586 skelly_synchronize-2023.4.1007/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3438 1970-01-01 00:00:00.000000 skelly_synchronize-2023.4.1007/PKG-INFO
```

### Comparing `skelly_synchronize-2023.2.1006/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.4.1007/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.4.1007/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/.gitignore` & `skelly_synchronize-2023.4.1007/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/LICENSE` & `skelly_synchronize-2023.4.1007/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/README.md` & `skelly_synchronize-2023.4.1007/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 
 This package synchronizes a set of videos of the same event by cross-correlating their audio files. The videos will be synchronized so that they all start at the earliest shared time, and end at the latest shared time. 
 
 # Install and Run
 
 Skelly_synchronize can be installed through pip by running `pip install skelly_synchronize` in your terminal. Once it has installed, it can be run with the command `python -m skelly_synchronize`. While running, the GUI window may appear frozen, but the terminal should show the progress. Large videos may take a significant amount of time. 
 
+Skelly_synchronize currently depends on FFmpeg, a command line tool that handles the video files. If you do not have FFmpeg downloaded, you will need to install it separately. You can download FFmpeg here: https://ffmpeg.org/download.html
+
 <img width="593" alt="Skelly_synchronize_gui_window" src="https://user-images.githubusercontent.com/24758117/221995127-340899d7-4f04-4f87-a2d7-ba1d49cd00e2.png">
 
 # Video Requirements
 
 The following requirements must be met for the script to function:
 
 1. Videos must have audio
 2. Videos must be in the same file format (default is ".mp4")
+3. Videos must have the exact same framerate (frames per second). There are often slight differences between brands/models of camera that lead to one camera's "60 fps" being different from another's. If your frame rates do not match, an error will be thrown.
 3. All videos in folder must have overlapping audio from the same real world event
 
 
 # How to run from source
 
 First clone this repository and pip install the `requirements.txt` file.
```

### Comparing `skelly_synchronize-2023.2.1006/pyproject.toml` & `skelly_synchronize-2023.4.1007/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 dependencies = [
 "pytest",
 "librosa",
 "PyQt6",
 "numpy",
 "scipy",
 "setuptools",
+"opencv-python",
+"deffcode",
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.02.1006"
+current_version = "v2023.04.1007"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.02.1006"
+__version__ = "v2023.04.1007"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/skelly_synchronize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,236 @@
 import librosa
 import time
 import logging
 import subprocess
+import cv2
 import numpy as np
+import json
 from scipy import signal
 from pathlib import Path
 from typing import Dict
+from deffcode import FFdecoder
 
 logging.basicConfig(level=logging.INFO)
 
-from utils.get_video_files import get_video_file_list
+from skelly_synchronize.utils.get_video_files import get_video_file_list
+from skelly_synchronize.utils.path_handling_utilities import (
+    get_parent_directory,
+    get_file_name,
+    create_directory,
+)
+from skelly_synchronize.tests.utilities.check_list_values_are_equal import (
+    check_list_values_are_equal,
+)
+from skelly_synchronize.tests.utilities.get_number_of_frames_of_videos_in_a_folder import (
+    get_number_of_frames_of_videos_in_a_folder,
+)
 
 
 class VideoSynchronize:
     """Class of functions for time synchronizing and trimming video files based on cross correlation of their audio."""
 
     def __init__(self) -> None:
         """Initialize VideoSynchronize class"""
         logging.debug("VideoSynchronize class initialized")
 
-    def synchronize(self, session_folder_path: Path, video_file_list: list) -> list:
+    def synchronize(
+        self,
+        session_folder_path: Path,
+        video_file_list: list,
+        video_handler: str = "deffcode",
+    ) -> list:
         """Run the functions from the VideoSynchronize class to synchronize all videos with the given file type in the base path folder.
-        Uses FFmpeg to handle the video files.
+        Uses deffcode and to handle the video files as default, set "video_handler" to "ffmpeg" to use ffmpeg methods instead.
+        ffmpeg is used to get audio from the video files with either method.
         """
 
-        synchronized_video_folder_name = "SyncedVideos"
-        self.synchronized_folder_path = (
-            session_folder_path / synchronized_video_folder_name
-        )
-        audio_folder_name = "AudioFiles"
-        self.audio_folder_path = session_folder_path / audio_folder_name
-
-        # create synchronized video and audio file folders
-        self.synchronized_folder_path.mkdir(parents=False, exist_ok=True)
-        self.audio_folder_path.mkdir(parents=False, exist_ok=True)
+        self.synchronized_folder_path = create_directory(
+            parent_directory=session_folder_path, directory_name="synchronized_videos"
+        )
+        self.audio_folder_path = create_directory(
+            parent_directory=session_folder_path, directory_name="audio_files"
+        )
 
         # create dictionaries with video and audio information
-        video_info_dict = self._get_video_info_dict(video_file_list)
+        video_info_dict = self._get_video_info_dict(
+            video_filepath_list=video_file_list, video_handler="ffmpeg"
+        )
         audio_signal_dict = self._get_audio_files(
-            video_info_dict, audio_extension="wav"
+            video_info_dict=video_info_dict, audio_extension="wav"
         )
 
         # get video fps and audio sample rate
-        fps_list = self._get_fps_list(video_info_dict)
-        audio_sample_rates = self.get_audio_sample_rates(audio_signal_dict)
+        fps_list = self._get_fps_list(video_info_dict=video_info_dict)
+        audio_sample_rates = self._get_audio_sample_rates(
+            audio_signal_dict=audio_signal_dict
+        )
 
         # frame rates and audio sample rates must be the same duration for the trimming process to work correctly
-        self._check_rates(fps_list)
-        self._check_rates(audio_sample_rates)
+        fps = check_list_values_are_equal(input_list=fps_list)
+        audio_sample_rate = check_list_values_are_equal(input_list=audio_sample_rates)
 
         # find the lags between starting times
-        lag_dict = self._find_lags(audio_signal_dict, audio_sample_rates[0])
+        lag_dict = self._find_lags(
+            audio_signal_dict=audio_signal_dict, sample_rate=audio_sample_rate
+        )
 
-        synched_video_names = self._trim_videos(video_info_dict, lag_dict)
-        return synched_video_names
+        self._trim_videos(
+            video_info_dict=video_info_dict,
+            lag_dict=lag_dict,
+            fps=fps,
+            video_handler=video_handler,
+        )
+
+        synchronized_video_framecounts = get_number_of_frames_of_videos_in_a_folder(
+            folder_path=self.synchronized_folder_path
+        )
+        logging.info(
+            f"All videos are {check_list_values_are_equal(synchronized_video_framecounts)} frames long"
+        )
 
-    def _get_video_info_dict(self, video_filepath_list: list) -> Dict[str, dict]:
+    def _get_video_info_dict(
+        self, video_filepath_list: list, video_handler: str = "ffmpeg"
+    ) -> Dict[str, dict]:
+        """Get a dictionary with video information from the given video file paths."""
         video_info_dict = dict()
         for video_filepath in video_filepath_list:
             video_dict = dict()
             video_dict["video filepath"] = video_filepath
             video_dict["video pathstring"] = str(video_filepath)
-            video_name = str(video_filepath).split("/")[-1]
-            video_dict["camera name"] = video_name.split(".")[0]
+            video_name = get_file_name(video_filepath)
+            video_dict["camera name"] = video_name
+
+            if video_handler == "ffmpeg":
+                video_dict["video duration"] = self._extract_video_duration_ffmpeg(
+                    file_pathstring=str(video_filepath)
+                )
+                video_dict["video fps"] = self._extract_video_fps_ffmpeg(
+                    file_pathstring=str(video_filepath)
+                )
 
-            video_dict["video duration"] = self._extract_video_duration_ffmpeg(
-                str(video_filepath)
-            )
-            video_dict["video fps"] = self._extract_video_fps_ffmpeg(
-                str(video_filepath)
-            )
             video_info_dict[video_name] = video_dict
 
         return video_info_dict
 
     def _get_audio_files(
         self, video_info_dict: Dict[str, dict], audio_extension: str
     ) -> dict:
+        """Get a dictionary with audio files and information from the given video file paths."""
         audio_signal_dict = dict()
         for video_dict in video_info_dict.values():
             self._extract_audio_from_video_ffmpeg(
                 file_pathstring=video_dict["video pathstring"],
                 file_name=video_dict["camera name"],
                 output_folder_path=self.audio_folder_path,
                 output_extension=audio_extension,
             )
 
             audio_name = video_dict["camera name"] + "." + audio_extension
 
-            audio_signal, audio_rate = librosa.load(
-                self.audio_folder_path / audio_name, sr=None
+            audio_signal, sample_rate = librosa.load(
+                path=self.audio_folder_path / audio_name, sr=None
             )
+
+            audio_duration = librosa.get_duration(y=audio_signal, sr=sample_rate)
+            logging.info(f"audio file {audio_name} is {audio_duration} seconds long")
             audio_signal_dict[audio_name] = {
                 "audio file": audio_signal,
-                "sample rate": audio_rate,
+                "sample rate": sample_rate,
                 "camera name": video_dict["camera name"],
+                "audio duration": audio_duration,
             }
 
         return audio_signal_dict
 
     def _get_fps_list(self, video_info_dict: Dict[str, dict]):
+        """Get list of the frames per second in earch video"""
         return [video_dict["video fps"] for video_dict in video_info_dict.values()]
 
-    def _check_rates(self, rate_list: list):
-        """Check if audio sample rates or video frame rates are equal, throw an exception if not (or if no rates are given)."""
-        if len(rate_list) == 0:
-            raise Exception("no rates given")
-
-        if rate_list.count(rate_list[0]) == len(rate_list):
-            logging.debug(f"all rates are equal to {rate_list[0]}")
-            return rate_list[0]
-        else:
-            raise Exception(f"rates are not equal, rates are {rate_list}")
-
     def _find_lags(self, audio_signal_dict: dict, sample_rate: int) -> Dict[str, float]:
         """Take a file list containing video and audio files, as well as the sample rate of the audio, cross correlate the audio files, and output a lag list.
         The lag list is normalized so that the lag of the latest video to start in time is 0, and all other lags are positive.
         """
         comparison_file_key = next(iter(audio_signal_dict))
+        logging.info(
+            f"comparison file is: {comparison_file_key}, sample rate is: {sample_rate}"
+        )
+
         lag_dict = {
             single_audio_dict["camera name"]: self._cross_correlate(
-                audio_signal_dict[comparison_file_key]["audio file"],
-                single_audio_dict["audio file"],
+                audio1=audio_signal_dict[comparison_file_key]["audio file"],
+                audio2=single_audio_dict["audio file"],
             )
             / sample_rate
             for single_audio_dict in audio_signal_dict.values()
-        }  # cross correlates all audio to the first audio file in the list, and divides by the audio sample rate in order to get the lag in seconds
+        }  # cross correlates all audio to the first audio file in the dict, and divides by the audio sample rate in order to get the lag in seconds
 
-        normalized_lag_dict = self._normalize_lag_dictionary(lag_dict)
+        normalized_lag_dict = self._normalize_lag_dictionary(lag_dictionary=lag_dict)
 
-        logging.debug(
-            f"original lag list: {lag_dict} normalized lag list: {normalized_lag_dict}"
+        logging.info(
+            f"original lag dict: {lag_dict} normalized lag dict: {normalized_lag_dict}"
         )
 
         return normalized_lag_dict
 
     def _trim_videos(
-        self, video_info_dict: Dict[str, dict], lag_dict: Dict[str, float]
+        self,
+        video_info_dict: Dict[str, dict],
+        lag_dict: Dict[str, float],
+        fps: float,
+        video_handler: str = "deffcode",
     ) -> list:
         """Take a list of video files and a list of lags, and make all videos start and end at the same time."""
 
-        min_duration = self._find_minimum_video_duration(video_info_dict, lag_dict)
-        trimmed_video_filenames = []  # can be used for plotting
+        minimum_duration = self._find_minimum_video_duration(
+            video_info_dict=video_info_dict, lag_dict=lag_dict
+        )
+        minimum_frames = int(minimum_duration * fps)
 
         for video_dict in video_info_dict.values():
             logging.debug(f"trimming video file {video_dict['camera name']}")
-            if video_dict["camera name"].split("_")[0] == "raw":
-                synced_video_name = "synced_" + video_dict["camera name"][4:] + ".mp4"
-            else:
-                synced_video_name = "synced_" + video_dict["camera name"] + ".mp4"
-            trimmed_video_filenames.append(
-                synced_video_name
-            )  # add new name to list to reference for plotting
-            logging.info(f"Saving video - Cam name: {video_dict['camera name']}")
-            self._trim_single_video_ffmpeg(
-                input_video_pathstring=video_dict["video pathstring"],
-                start_time=lag_dict[video_dict["camera name"]],
-                desired_duration=min_duration,
-                output_video_pathstring=str(
-                    self.synchronized_folder_path / synced_video_name
-                ),
+            synced_video_name = self._name_synced_video(
+                raw_video_filename=video_dict["camera name"]
             )
-            logging.info(
-                f"Video Saved - Cam name: {video_dict['camera name']}, Video Duration: {min_duration}"
+
+            start_time = lag_dict[video_dict["camera name"]]
+            start_frame = int(start_time * fps)
+            frame_list = self._get_frame_list(
+                start_frame=start_frame, duration_frames=minimum_frames
             )
 
-        return trimmed_video_filenames
+            if video_handler == "ffmpeg":
+                logging.info(f"Saving video - Cam name: {video_dict['camera name']}")
+                logging.info(f"desired saving duration is: {minimum_duration} seconds")
+                self._trim_single_video_ffmpeg(
+                    input_video_pathstring=video_dict["video pathstring"],
+                    start_time=start_time,
+                    desired_duration=minimum_duration,
+                    output_video_pathstring=str(
+                        self.synchronized_folder_path / synced_video_name
+                    ),
+                )
+                logging.info(
+                    f"Video Saved - Cam name: {video_dict['camera name']}, Video Duration in Seconds: {minimum_duration}"
+                )
+            if video_handler == "deffcode":
+                logging.info(f"Saving video - Cam name: {video_dict['camera name']}")
+                logging.info(
+                    f"start frame is: {start_frame} desired saving duration is: {minimum_frames} frames"
+                )
+                self._trim_single_video_deffcode(
+                    input_video_pathstring=video_dict["video pathstring"],
+                    frame_list=frame_list,
+                    output_video_pathstring=str(
+                        self.synchronized_folder_path / synced_video_name
+                    ),
+                )
+                logging.info(
+                    f"Video Saved - Cam name: {video_dict['camera name']}, Video Duration in Frames: {minimum_frames}"
+                )
 
     def _extract_audio_from_video_ffmpeg(
         self,
         file_pathstring: str,
         file_name: str,
         output_folder_path: Path,
         output_extension="wav",
@@ -232,14 +293,54 @@
         cleaned_stdout = str(extract_fps_subprocess.stdout).split("'")[1].split("\\")[0]
         # separate out numerator and denominator to calculate the fraction
         numerator, denominator = cleaned_stdout.split("/")
         video_fps = float(int(numerator) / int(denominator))
 
         return video_fps
 
+    def _trim_single_video_deffcode(
+        self,
+        input_video_pathstring: str,
+        frame_list: list,
+        output_video_pathstring: str,
+    ):
+        decoder = FFdecoder(
+            input_video_pathstring,
+            frame_format="bgr24",
+        ).formulate()
+
+        metadata_dictionary = json.loads(decoder.metadata)
+
+        fourcc = cv2.VideoWriter_fourcc(*"mp4v")
+        framerate = metadata_dictionary["output_framerate"]
+        framesize = tuple(metadata_dictionary["output_frames_resolution"])
+
+        video_writer_object = cv2.VideoWriter(
+            output_video_pathstring, fourcc, framerate, framesize
+        )
+
+        current_frame = 0
+        written_frames = 0
+
+        for frame in decoder.generateFrame():
+            if frame is None:
+                break
+
+            if current_frame in frame_list:
+                video_writer_object.write(frame)
+                written_frames += 1
+
+            if written_frames == len(frame_list):
+                break
+
+            current_frame += 1
+
+        decoder.terminate()
+        video_writer_object.release()
+
     def _trim_single_video_ffmpeg(
         self,
         input_video_pathstring: str,
         start_time: float,
         desired_duration: float,
         output_video_pathstring: str,
     ):
@@ -257,15 +358,19 @@
                 "-y",
                 f"{output_video_pathstring}",
             ],
             stdout=subprocess.PIPE,
             stderr=subprocess.STDOUT,
         )
 
-    def get_audio_sample_rates(self, audio_signal_dict: Dict[str, float]) -> list:
+    def _get_frame_list(self, start_frame: int, duration_frames: int) -> list:
+        """Get a list of frame numbers for video to be trimmed to"""
+        return [start_frame + frame for frame in range(duration_frames)]
+
+    def _get_audio_sample_rates(self, audio_signal_dict: Dict[str, float]) -> list:
         """Get the sample rates of each audio file and return them in a list"""
         audio_sample_rate_list = [
             single_audio_dict["sample rate"]
             for single_audio_dict in audio_signal_dict.values()
         ]
 
         return audio_sample_rate_list
@@ -274,35 +379,35 @@
         """Perform z-score normalization on an audio file and return the normalized audio file - this is best practice for correlating."""
         return (audio_file - np.mean(audio_file)) / np.std(
             audio_file - np.mean(audio_file)
         )
 
     def _cross_correlate(self, audio1, audio2):
         """Take two audio files, synchronize them using cross correlation, and trim them to the same length.
-        Inputs are two WAV files to be synchronizeded. Return the lag expressed in terms of the audio sample rate of the clips.
+        Inputs are two WAV files to be synchronized. Return the lag expressed in terms of the audio sample rate of the clips.
         """
 
         # compute cross correlation with scipy correlate function, which gives the correlation of every different lag value
         # mode='full' makes sure every lag value possible between the two signals is used, and method='fft' uses the fast fourier transform to speed the process up
         correlation = signal.correlate(audio1, audio2, mode="full", method="fft")
         # lags gives the amount of time shift used at each index, corresponding to the index of the correlate output list
         lags = signal.correlation_lags(audio1.size, audio2.size, mode="full")
         # lag is the time shift used at the point of maximum correlation - this is the key value used for shifting our audio/video
         lag = lags[np.argmax(correlation)]
 
         return lag
 
     def _find_minimum_video_duration(
-        self, video_info_dict: Dict[str, dict], lag_list: list
+        self, video_info_dict: Dict[str, dict], lag_dict: dict
     ) -> float:
         """Take a list of video files and a list of lags, and find what the shortest video is starting from each videos lag offset"""
 
         min_duration = min(
             [
-                video_dict["video duration"] - lag_list[video_dict["camera name"]]
+                video_dict["video duration"] - lag_dict[video_dict["camera name"]]
                 for video_dict in video_info_dict.values()
             ]
         )
 
         return min_duration
 
     def _normalize_lag_dictionary(
@@ -315,30 +420,44 @@
         normalized_lag_dictionary = {
             camera_name: (max(lag_dictionary.values()) - value)
             for camera_name, value in lag_dictionary.items()
         }
 
         return normalized_lag_dictionary
 
+    def _name_synced_video(self, raw_video_filename: str) -> str:
+        """Take a raw video filename, remove the raw prefix if its there, and return the synced video filename"""
+        if raw_video_filename.split("_")[0] == "raw":
+            synced_video_name = "synced_" + raw_video_filename[4:] + ".mp4"
+        else:
+            synced_video_name = "synced_" + raw_video_filename + ".mp4"
+
+        return synced_video_name
+
 
-def synchronize_videos(raw_video_folder_path: Path, file_type=".mp4"):
+def synchronize_videos(raw_video_folder_path: Path, file_type: str = ".mp4"):
     # start timer to measure performance
     start_timer = time.time()
 
-    session_folder_path = raw_video_folder_path.parent.absolute()
-    video_file_list = get_video_file_list(raw_video_folder_path, ".mp4")
+    session_folder_path = get_parent_directory(raw_video_folder_path)
+    video_file_list = get_video_file_list(
+        folder_path=raw_video_folder_path, file_type=file_type
+    )
 
     synchronize = VideoSynchronize()
-    synchronize.synchronize(session_folder_path, video_file_list)
+    synchronize.synchronize(
+        session_folder_path=session_folder_path,
+        video_file_list=video_file_list,
+    )
 
     # end performance timer
     end_timer = time.time()
 
     # calculate and display elapsed processing time
     elapsed_time = end_timer - start_timer
     logging.info(f"Elapsed processing time in seconds: {elapsed_time}")
 
 
 if __name__ == "__main__":
     raw_video_folder_path = Path("path/to/your/folder/of/raw/videos")
     file_type = "MP4"
-    synchronize_videos(raw_video_folder_path, file_type)
+    synchronize_videos(raw_video_folder_path=raw_video_folder_path, file_type=file_type)
```

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/tests/unit_tests.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.4.1007/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.2.1006/PKG-INFO` & `skelly_synchronize-2023.4.1007/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.2.1006
+Version: 2023.4.1007
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pytest
 Requires-Dist: librosa
 Requires-Dist: PyQt6
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: setuptools
+Requires-Dist: opencv-python
+Requires-Dist: deffcode
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Provides-Extra: dev
 
@@ -26,22 +28,25 @@
 
 This package synchronizes a set of videos of the same event by cross-correlating their audio files. The videos will be synchronized so that they all start at the earliest shared time, and end at the latest shared time. 
 
 # Install and Run
 
 Skelly_synchronize can be installed through pip by running `pip install skelly_synchronize` in your terminal. Once it has installed, it can be run with the command `python -m skelly_synchronize`. While running, the GUI window may appear frozen, but the terminal should show the progress. Large videos may take a significant amount of time. 
 
+Skelly_synchronize currently depends on FFmpeg, a command line tool that handles the video files. If you do not have FFmpeg downloaded, you will need to install it separately. You can download FFmpeg here: https://ffmpeg.org/download.html
+
 <img width="593" alt="Skelly_synchronize_gui_window" src="https://user-images.githubusercontent.com/24758117/221995127-340899d7-4f04-4f87-a2d7-ba1d49cd00e2.png">
 
 # Video Requirements
 
 The following requirements must be met for the script to function:
 
 1. Videos must have audio
 2. Videos must be in the same file format (default is ".mp4")
+3. Videos must have the exact same framerate (frames per second). There are often slight differences between brands/models of camera that lead to one camera's "60 fps" being different from another's. If your frame rates do not match, an error will be thrown.
 3. All videos in folder must have overlapping audio from the same real world event
 
 
 # How to run from source
 
 First clone this repository and pip install the `requirements.txt` file.
```

