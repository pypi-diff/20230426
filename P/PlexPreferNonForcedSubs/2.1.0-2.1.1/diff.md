# Comparing `tmp/PlexPreferNonForcedSubs-2.1.0.tar.gz` & `tmp/PlexPreferNonForcedSubs-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlexPreferNonForcedSubs-2.1.0.tar", last modified: Wed Apr 26 19:42:45 2023, max compression
+gzip compressed data, was "PlexPreferNonForcedSubs-2.1.1.tar", last modified: Wed Apr 26 20:07:56 2023, max compression
```

## Comparing `PlexPreferNonForcedSubs-2.1.0.tar` & `PlexPreferNonForcedSubs-2.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 19:42:45.961427 PlexPreferNonForcedSubs-2.1.0/
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     4331 2023-04-26 19:42:45.960429 PlexPreferNonForcedSubs-2.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 19:42:45.940279 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs/
--rw-rw-rw-   0        0        0     5856 2023-04-26 16:45:01.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 19:42:45.958941 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/
--rw-rw-rw-   0        0        0     4331 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-26 19:42:45.000000 PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3707 2023-04-26 05:41:36.000000 PlexPreferNonForcedSubs-2.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-26 19:42:45.961427 PlexPreferNonForcedSubs-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1516 2023-04-26 19:42:12.000000 PlexPreferNonForcedSubs-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:07:56.553610 PlexPreferNonForcedSubs-2.1.1/
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 PlexPreferNonForcedSubs-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4581 2023-04-26 20:07:56.553110 PlexPreferNonForcedSubs-2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 20:07:56.534137 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs/
+-rw-rw-rw-   0        0        0     5968 2023-04-26 20:05:46.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:07:56.551115 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/
+-rw-rw-rw-   0        0        0     4581 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-26 20:07:56.000000 PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3945 2023-04-26 20:00:36.000000 PlexPreferNonForcedSubs-2.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:07:56.554110 PlexPreferNonForcedSubs-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1516 2023-04-26 20:07:41.000000 PlexPreferNonForcedSubs-2.1.1/setup.py
```

### Comparing `PlexPreferNonForcedSubs-2.1.0/LICENSE` & `PlexPreferNonForcedSubs-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexPreferNonForcedSubs-2.1.0/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.0
+Version: 2.1.1
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -26,23 +26,31 @@
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
 
-## Instructions:
+## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .py script from the [releases](https://github.com/RileyXX/PlexDefaultSubtitleChanger/releases) page. 
-3. Replace `xxxxxxx` in the script with your [plex api token](https://www.plexopedia.com/plex-media-server/general/plex-token/).
-4. Install python dependency [plexapi](https://github.com/pkkid/python-plexapi). To do this, run `python -m pip install plexapi` in command prompt.
-5. Make sure Plex media server is running locally then run the script and watch it work its magic.
+2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
+3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+5. Done
 
 _Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
 
+### Run:
+`PlexPreferNonForcedSubs` in command line.
+
+### Update:
+`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
+### Uninstall:
+`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
@@ -58,7 +66,11 @@
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py` & `PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs/PlexPreferNonForcedSubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from plexapi.server import PlexServer
 from plexapi.media import SubtitleStream
 
-# Connect to Plex Media Server. Replace xxxxxxxx below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
+# Connect to Plex Media Server. Replace PLEX_TOKEN below with your Plex token. How to get token: https://www.plexopedia.com/plex-media-server/general/plex-token/
 baseurl = 'http://localhost:32400'
 token = 'PLEX_TOKEN'
 try:
     with open('token.txt', 'r') as f:
         token = f.read().strip()
 except FileNotFoundError:
     pass
 
 if token == 'PLEX_TOKEN':
     # Prompt user to enter Plex token
+    print(f'How to get your Plex token: https://www.plexopedia.com/plex-media-server/general/plex-token/\n')
     token = input("Enter your Plex token: ")
     # Save token to token.txt in the same folder as the script
     with open('token.txt', 'w') as f:
         f.write(token)
 
 plex = PlexServer(baseurl, token)
```

### Comparing `PlexPreferNonForcedSubs-2.1.0/PlexPreferNonForcedSubs.egg-info/PKG-INFO` & `PlexPreferNonForcedSubs-2.1.1/PlexPreferNonForcedSubs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexPreferNonForcedSubs
-Version: 2.1.0
+Version: 2.1.1
 Summary: This script will set all movies and shows in your local Plex library to English non forced subtitles by default.
 Home-page: https://github.com/RileyXX/PlexPreferNonForcedSubs
 Keywords: python,video,plex,subtitles,subs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -26,23 +26,31 @@
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
 
-## Instructions:
+## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .py script from the [releases](https://github.com/RileyXX/PlexDefaultSubtitleChanger/releases) page. 
-3. Replace `xxxxxxx` in the script with your [plex api token](https://www.plexopedia.com/plex-media-server/general/plex-token/).
-4. Install python dependency [plexapi](https://github.com/pkkid/python-plexapi). To do this, run `python -m pip install plexapi` in command prompt.
-5. Make sure Plex media server is running locally then run the script and watch it work its magic.
+2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
+3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+5. Done
 
 _Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
 
+### Run:
+`PlexPreferNonForcedSubs` in command line.
+
+### Update:
+`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
+### Uninstall:
+`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
@@ -58,7 +66,11 @@
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `PlexPreferNonForcedSubs-2.1.0/README.md` & `PlexPreferNonForcedSubs-2.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,31 @@
 ## What are "non-forced" subtitles?
 Non-forced subtitles provide subtitles everytime a characters speaks.
 
 ## What are "forced" subtitles?
 Forced subtitles only provide subtitles when the characters speak a foreign or alien language.
 
 
-## Instructions:
+## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/).
-2. Download the latest .py script from the [releases](https://github.com/RileyXX/PlexDefaultSubtitleChanger/releases) page. 
-3. Replace `xxxxxxx` in the script with your [plex api token](https://www.plexopedia.com/plex-media-server/general/plex-token/).
-4. Install python dependency [plexapi](https://github.com/pkkid/python-plexapi). To do this, run `python -m pip install plexapi` in command prompt.
-5. Make sure Plex media server is running locally then run the script and watch it work its magic.
+2. Run `python -m pip install PlexPreferNonForcedSubs` in command line.
+3. Make sure Plex media server is running then run the script using `PlexPreferNonForcedSubs` in command line.
+4. On first run the script will ask you to fill in your [Plex token](https://www.plexopedia.com/plex-media-server/general/plex-token/). Your token will be saved locally in the same folder as token.txt.
+5. Done
 
 _Note: This script should work on any OS where Python is installed (Windows, MacOS and Linux etc)._
 
+### Run:
+`PlexPreferNonForcedSubs` in command line.
+
+### Update:
+`python -m pip install PlexPreferNonForcedSubs --upgrade` in command line.
+### Uninstall:
+`python -m pip uninstall PlexPreferNonForcedSubs` in command line.
+
 ## Known issues/future outlook:
 * Several lines of redundant code can be shortened and/or removed
 
 ## Also posted on:
 * [Stackoverflow](https://stackoverflow.com/q/75027919/9196825)
 * [Reddit](https://www.reddit.com/r/PleX/comments/105gdh7/python_code_to_set_all_movies_and_shows_in_plex/)
 * [Plex Forums](https://forums.plex.tv/t/python-script-to-set-all-movies-and-shows-in-plex-to-use-english-non-forced-subtitles/825871)
@@ -44,7 +52,11 @@
 
 #### More donation options:
 - Cashapp: `$rileyxx`
 - Venmo: `@rileyxx`
 - Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
 - Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
 
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
```

### Comparing `PlexPreferNonForcedSubs-2.1.0/setup.py` & `PlexPreferNonForcedSubs-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '2.1.0'
+VERSION = '2.1.1'
 DESCRIPTION = 'This script will set all movies and shows in your local Plex library to English non forced subtitles by default.'
 LONG_DESCRIPTION = 'This python script will set all movies and shows in your local Plex library to English non forced subtitles by default. The subtitle selections will apply to your Plex profile and be remembered on other devices.'
 
 # Setting up
 setup(
     name="PlexPreferNonForcedSubs",
     version=VERSION,
```

