# Comparing `tmp/yark-1.2.7.tar.gz` & `tmp/yark-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yark-1.2.7.tar", max compression
+gzip compressed data, was "yark-1.2.8.tar", max compression
```

## Comparing `yark-1.2.7.tar` & `yark-1.2.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1081 2023-02-12 12:50:30.923409 yark-1.2.7/LICENSE
--rw-r--r--   0        0        0     3357 2023-02-19 09:43:06.601218 yark-1.2.7/README.md
--rw-r--r--   0        0        0      952 2023-02-19 09:46:51.383392 yark-1.2.7/pyproject.toml
--rw-r--r--   0        0        0      653 2023-02-19 09:43:06.620847 yark-1.2.7/yark/__init__.py
--rw-r--r--   0        0        0      135 2023-02-19 09:43:06.620918 yark-1.2.7/yark/__main__.py
--rw-r--r--   0        0        0    26418 2023-02-19 09:43:06.621241 yark-1.2.7/yark/channel.py
--rw-r--r--   0        0        0     7831 2023-02-19 09:43:06.621367 yark-1.2.7/yark/cli.py
--rw-r--r--   0        0        0     1178 2023-02-19 09:43:06.621427 yark-1.2.7/yark/errors.py
--rw-r--r--   0        0        0     5451 2023-02-19 09:43:06.621547 yark-1.2.7/yark/reporter.py
--rw-r--r--   0        0        0     5071 2023-02-19 09:43:06.621648 yark-1.2.7/yark/templates/base.html
--rw-r--r--   0        0        0     3527 2023-02-19 09:43:06.621755 yark-1.2.7/yark/templates/channel.html
--rw-r--r--   0        0        0      887 2023-02-19 09:43:06.621830 yark-1.2.7/yark/templates/index.html
--rw-r--r--   0        0        0    16296 2023-02-19 09:43:06.621934 yark-1.2.7/yark/templates/video.html
--rw-r--r--   0        0        0      279 2023-02-19 09:43:06.621993 yark-1.2.7/yark/utils.py
--rw-r--r--   0        0        0    11750 2023-02-19 09:43:06.622111 yark-1.2.7/yark/video.py
--rw-r--r--   0        0        0     8031 2023-02-19 09:43:06.622198 yark-1.2.7/yark/viewer.py
--rw-r--r--   0        0        0     4310 1970-01-01 00:00:00.000000 yark-1.2.7/setup.py
--rw-r--r--   0        0        0     4267 1970-01-01 00:00:00.000000 yark-1.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-26 08:39:14.067110 yark-1.2.8/LICENSE
+-rw-r--r--   0        0        0     3357 2023-04-26 08:45:47.515449 yark-1.2.8/README.md
+-rw-r--r--   0        0        0      952 2023-04-26 08:52:44.030608 yark-1.2.8/pyproject.toml
+-rw-r--r--   0        0        0      653 2023-04-26 08:45:47.519735 yark-1.2.8/yark/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-26 08:39:14.086460 yark-1.2.8/yark/__main__.py
+-rw-r--r--   0        0        0    19511 2023-04-26 08:45:48.376450 yark-1.2.8/yark/archiver/archive.py
+-rw-r--r--   0        0        0    26389 2023-04-26 08:52:25.113627 yark-1.2.8/yark/channel.py
+-rw-r--r--   0        0        0     7831 2023-04-26 08:45:47.520682 yark-1.2.8/yark/cli.py
+-rw-r--r--   0        0        0     1178 2023-04-26 08:45:47.520832 yark-1.2.8/yark/errors.py
+-rw-r--r--   0        0        0     5451 2023-04-26 08:45:47.520960 yark-1.2.8/yark/reporter.py
+-rw-r--r--   0        0        0     5071 2023-04-26 08:45:47.521149 yark-1.2.8/yark/templates/base.html
+-rw-r--r--   0        0        0     3527 2023-04-26 08:45:47.521252 yark-1.2.8/yark/templates/channel.html
+-rw-r--r--   0        0        0      887 2023-04-26 08:45:47.521402 yark-1.2.8/yark/templates/index.html
+-rw-r--r--   0        0        0    16296 2023-04-26 08:45:47.521628 yark-1.2.8/yark/templates/video.html
+-rw-r--r--   0        0        0      279 2023-04-26 08:45:47.521763 yark-1.2.8/yark/utils.py
+-rw-r--r--   0        0        0    11750 2023-04-26 08:45:47.521916 yark-1.2.8/yark/video.py
+-rw-r--r--   0        0        0     8031 2023-04-26 08:45:47.522087 yark-1.2.8/yark/viewer.py
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 yark-1.2.8/setup.py
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 yark-1.2.8/PKG-INFO
```

### Comparing `yark-1.2.7/LICENSE` & `yark-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/README.md` & `yark-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/pyproject.toml` & `yark-1.2.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "yark"
-version = "1.2.7"
+version = "1.2.8"
 description = "YouTube archiving made simple."
 authors = ["Owen Griffiths <root@ogriffiths.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/owez/yark"
 classifiers = [
     "Topic :: System :: Archiving",
     "Topic :: System :: Archiving :: Backup",
     "Topic :: Multimedia :: Video",
 ]
 include = [{ path = "templates/*" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Flask = "^2.2.2"
+Flask = "^2.3.1"
 requests = "^2.28.2"
 colorama = "^0.4.6"
-yt-dlp = "^2023.2.17"
+yt-dlp = "^2023.3.4"
 progress = "^1.6"
 
 [tool.poetry.scripts]
 yark = "yark.cli:_cli"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.991"
 poethepoet = "^0.18.1"
-types-colorama = "^0.4.15.7"
-types-requests = "^2.28.11.13"
+types-colorama = "^0.4.15.11"
+types-requests = "^2.28.11.17"
 black = "^22.12.0"
 
 [tool.poe.tasks]
 lint = { shell = "set -e && mypy yark examples/madness.py" }
 fmt = "black yark examples/madness.py"
 
 [build-system]
```

### Comparing `yark-1.2.7/yark/__init__.py` & `yark-1.2.8/yark/__init__.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/channel.py` & `yark-1.2.8/yark/channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """Channel and overall archive management with downloader"""
 
 from __future__ import annotations
 from datetime import datetime
 import json
-import os
 from pathlib import Path
 import time
 from yt_dlp import YoutubeDL, DownloadError  # type: ignore
 from colorama import Style, Fore
 import sys
 from .reporter import Reporter
 from .errors import ArchiveNotFoundException, _err_msg, VideoNotFoundException
 from .video import Video, Element
 from typing import Any
 import time
 from progress.spinner import PieSpinner
 from concurrent.futures import ThreadPoolExecutor
 import time
-import concurrent.futures.thread
 
 ARCHIVE_COMPAT = 3
 """
 Version of Yark archives which this script is capable of properly parsing
 
 - Version 1 was the initial format and had all the basic information you can see in the viewer now
 - Version 2 introduced livestreams and shorts into the mix, as well as making the channel id into a simple url
@@ -199,19 +197,19 @@
                     bar.next()
                     time.sleep(0.075)
 
             # Get result from thread now that it's finished
             res = future.result()
 
         # Uncomment for saving big dumps for testing
-        # with open("demo/dump.json", "w+") as file:
+        # with open(self.path / "dump.json", "w+") as file:
         #     json.dump(res, file)
 
         # Uncomment for loading big dumps for testing
-        # res = json.load(open("demo/dump.json", "r"))
+        # res = json.load(open(self.path / "dump.json", "r"))
 
         # Parse downloaded metadata
         self._parse_metadata(res)
 
     def _download_metadata(self) -> dict[str, Any]:
         """Downloads metadata dict and returns for further parsing"""
         # Construct downloader
```

### Comparing `yark-1.2.7/yark/cli.py` & `yark-1.2.8/yark/cli.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/errors.py` & `yark-1.2.8/yark/errors.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/reporter.py` & `yark-1.2.8/yark/reporter.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/templates/base.html` & `yark-1.2.8/yark/templates/base.html`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/templates/channel.html` & `yark-1.2.8/yark/templates/channel.html`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/templates/index.html` & `yark-1.2.8/yark/templates/index.html`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/templates/video.html` & `yark-1.2.8/yark/templates/video.html`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/video.py` & `yark-1.2.8/yark/video.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/yark/viewer.py` & `yark-1.2.8/yark/viewer.py`

 * *Files identical despite different names*

### Comparing `yark-1.2.7/setup.py` & `yark-1.2.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['yark']
+['yark', 'yark.archiver']
 
 package_data = \
 {'': ['*'], 'yark': ['templates/*']}
 
 install_requires = \
-['Flask>=2.2.2,<3.0.0',
+['Flask>=2.3.1,<3.0.0',
  'colorama>=0.4.6,<0.5.0',
  'progress>=1.6,<2.0',
  'requests>=2.28.2,<3.0.0',
- 'yt-dlp>=2023.2.17,<2024.0.0']
+ 'yt-dlp>=2023.3.4,<2024.0.0']
 
 entry_points = \
 {'console_scripts': ['yark = yark.cli:_cli']}
 
 setup_kwargs = {
     'name': 'yark',
-    'version': '1.2.7',
+    'version': '1.2.8',
     'description': 'YouTube archiving made simple.',
     'long_description': '# Yark\n\nYouTube archiving made simple.\n\n<!-- TODO: uncomment when new gui is out -->\n<!-- If you\'re reading this, you\'re probably trying to download/use Yark via PyPI which has been removed in newer versions. You can download a modern version of Yark [here](https://github.com/Owez/yark).\n\n<p><img src="https://raw.githubusercontent.com/Owez/yark/1.2-support/examples/images/transition.png" alt="Version release transition" title="Version release transition" width="450" /></p> -->\n\n## Installation\n\nTo install Yark, simply download [Python 3.9+](https://www.python.org/downloads/) and [FFmpeg](https://ffmpeg.org/) (optional), then run the following:\n\n```shell\n$ pip3 install yark\n```\n\n## Managing your Archive\n\nOnce you\'ve installed Yark, think of a name for your archive (e.g., "foobar") and copy the target\'s url:\n\n```shell\n$ yark new foobar https://www.youtube.com/channel/UCSMdm6bUYIBN0KfS2CVuEPA\n```\n\nNow that you\'ve created the archive, you can tell Yark to download all videos and metadata using the refresh command:\n\n```shell\n$ yark refresh foobar\n```\n\nOnce everything has been downloaded, Yark will automatically give you a status report of what\'s changed since the last refresh:\n\n<p><img src="https://raw.githubusercontent.com/Owez/yark/1.2-support/examples/images/cli_dark.png" alt="Report Demo" title="Report Demo" width="600" /></p>\n\n## Viewing your Archive\n\nViewing you archive is easy, just type `view` with your archives name:\n\n```shell\n$ yark view foobar\n```\n\nThis will pop up an offline website in your browser letting you watch all videos 🚀\n\n<p><img src="https://raw.githubusercontent.com/Owez/yark/1.2-support/examples/images/viewer_light.png" alt="Viewer Demo" title="Viewer Demo" width=650 /></p>\n\nUnder each video is a rich history report filled with timelines and graphs, as well as a noting feature which lets you add timestamped and permalinked comments 👐\n\n<p><img src="https://raw.githubusercontent.com/Owez/yark/1.2-support/examples/images/viewer_stats_light.png" alt="Viewer Demo – Stats" title="Viewer Demo – Stats" width=650 /></p>\n\nLight and dark modes are both available and automatically apply based on the system\'s theme.\n\n## Details\n\nHere are some things to keep in mind when using Yark; the good and the bad:\n\n- Don\'t create a new archive again if you just want to update it, Yark accumulates all new metadata for you via timestamps\n- Feel free to suggest new features via the issues tab on this repository\n- Scheduling isn\'t a feature just yet, please use [`cron`](https://en.wikipedia.org/wiki/Cron) or something similar!\n\n## Archive Format\n\nThe archive format itself is simple and consists of a directory-based structure with a core metadata file and all thumbnail/video data in their own directories as typical files:\n\n- `[name]/` – Your self-contained archive\n  - `yark.json` – Archive file with all metadata\n  - `yark.bak` – Backup archive file to protect against data damage\n  - `videos/` – Directory containing all known videos\n    - `[id].*` – Files containing video data for YouTube videos\n  - `thumbnails/` – Directory containing all known thumbnails\n    - `[hash].png` – Files containing thumbnails with its BLAKE2 hash\n\nIt\'s best to take a few minutes to familiarize yourself with your archive by looking at files which look interesting to you in it, everything is quite readable.\n',
     'author': 'Owen Griffiths',
     'author_email': 'root@ogriffiths.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/owez/yark',
```

### Comparing `yark-1.2.7/PKG-INFO` & `yark-1.2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: yark
-Version: 1.2.7
+Version: 1.2.8
 Summary: YouTube archiving made simple.
 Home-page: https://github.com/owez/yark
 License: MIT
 Author: Owen Griffiths
 Author-email: root@ogriffiths.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
-Requires-Dist: Flask (>=2.2.2,<3.0.0)
+Requires-Dist: Flask (>=2.3.1,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: progress (>=1.6,<2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: yt-dlp (>=2023.2.17,<2024.0.0)
+Requires-Dist: yt-dlp (>=2023.3.4,<2024.0.0)
 Project-URL: Repository, https://github.com/owez/yark
 Description-Content-Type: text/markdown
 
 # Yark
 
 YouTube archiving made simple.
```

