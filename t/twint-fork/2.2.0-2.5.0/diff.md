# Comparing `tmp/twint_fork-2.2.0.tar.gz` & `tmp/twint_fork-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twint_fork-2.2.0.tar", last modified: Tue Mar 28 11:11:59 2023, max compression
+gzip compressed data, was "twint_fork-2.5.0.tar", last modified: Wed Apr 26 06:40:36 2023, max compression
```

## Comparing `twint_fork-2.2.0.tar` & `twint_fork-2.5.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-28 11:11:59.796464 twint_fork-2.2.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.2.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.2.0/MANIFEST.in
--rw-r--r--   0 hyi        (502) staff       (20)     9106 2023-03-28 11:11:59.795791 twint_fork-2.2.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     8428 2023-03-28 11:11:31.000000 twint_fork-2.2.0/README.md
--rw-r--r--   0 hyi        (502) staff       (20)       38 2023-03-28 11:11:59.796514 twint_fork-2.2.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1644 2023-03-28 11:11:47.000000 twint_fork-2.2.0/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-28 11:11:59.788579 twint_fork-2.2.0/twint/
--rw-r--r--   0 hyi        (502) staff       (20)      818 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       64 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/__version__.py
--rw-r--r--   0 hyi        (502) staff       (20)    14812 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/cli.py
--rw-r--r--   0 hyi        (502) staff       (20)     2512 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/config.py
--rw-r--r--   0 hyi        (502) staff       (20)     1034 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/datelock.py
--rw-r--r--   0 hyi        (502) staff       (20)     4780 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/feed.py
--rw-r--r--   0 hyi        (502) staff       (20)     4454 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/format.py
--rw-r--r--   0 hyi        (502) staff       (20)    11714 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/get.py
--rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/output.py
--rw-r--r--   0 hyi        (502) staff       (20)    17709 2023-03-28 11:11:31.000000 twint_fork-2.2.0/twint/run.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-28 11:11:59.793781 twint_fork-2.2.0/twint/storage/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/storage/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)    10876 2023-03-28 11:11:31.000000 twint_fork-2.2.0/twint/storage/db.py
--rw-r--r--   0 hyi        (502) staff       (20)    14035 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/storage/elasticsearch.py
--rw-r--r--   0 hyi        (502) staff       (20)     6258 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/storage/panda.py
--rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/storage/write.py
--rw-r--r--   0 hyi        (502) staff       (20)     3939 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/storage/write_meta.py
--rw-r--r--   0 hyi        (502) staff       (20)     3820 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/token.py
--rw-r--r--   0 hyi        (502) staff       (20)     5419 2023-03-28 11:11:31.000000 twint_fork-2.2.0/twint/tweet.py
--rw-r--r--   0 hyi        (502) staff       (20)     6382 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/url.py
--rw-r--r--   0 hyi        (502) staff       (20)     1974 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/user.py
--rw-r--r--   0 hyi        (502) staff       (20)      621 2023-03-22 13:37:09.000000 twint_fork-2.2.0/twint/verbose.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-03-28 11:11:59.795474 twint_fork-2.2.0/twint_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)     9106 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      627 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)       62 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       51 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      137 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)        6 2023-03-28 11:11:59.000000 twint_fork-2.2.0/twint_fork.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.090996 twint_fork-2.5.0/
+-rw-r--r--   0 hyi        (502) staff       (20)     1071 2023-03-22 13:37:09.000000 twint_fork-2.5.0/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)       26 2023-03-22 13:37:09.000000 twint_fork-2.5.0/MANIFEST.in
+-rw-r--r--   0 hyi        (502) staff       (20)     7620 2023-04-26 06:40:36.089236 twint_fork-2.5.0/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     6808 2023-04-26 03:16:17.000000 twint_fork-2.5.0/README.md
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2023-04-26 06:40:36.091074 twint_fork-2.5.0/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1803 2023-04-26 06:34:18.000000 twint_fork-2.5.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.076925 twint_fork-2.5.0/twint/
+-rw-r--r--   0 hyi        (502) staff       (20)      808 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       61 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       64 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/__version__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    15324 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/cli.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2513 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/config.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1080 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/datelock.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4131 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/feed.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4464 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/format.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11838 2023-04-26 00:44:20.000000 twint_fork-2.5.0/twint/get.py
+-rw-r--r--   0 hyi        (502) staff       (20)     8168 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/output.py
+-rw-r--r--   0 hyi        (502) staff       (20)    19339 2023-04-26 06:33:01.000000 twint_fork-2.5.0/twint/run.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.080912 twint_fork-2.5.0/twint/storage/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-22 13:37:09.000000 twint_fork-2.5.0/twint/storage/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    11197 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/db.py
+-rw-r--r--   0 hyi        (502) staff       (20)    13379 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/elasticsearch.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6307 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/panda.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2161 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/write.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3493 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/storage/write_meta.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3937 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/token.py
+-rw-r--r--   0 hyi        (502) staff       (20)     5533 2023-04-25 13:25:39.000000 twint_fork-2.5.0/twint/tweet.py
+-rw-r--r--   0 hyi        (502) staff       (20)     6026 2023-04-26 02:31:23.000000 twint_fork-2.5.0/twint/url.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1285 2023-04-26 00:44:03.000000 twint_fork-2.5.0/twint/user.py
+-rw-r--r--   0 hyi        (502) staff       (20)      622 2023-04-20 09:29:26.000000 twint_fork-2.5.0/twint/verbose.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2023-04-26 06:40:36.085332 twint_fork-2.5.0/twint_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)     7620 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      645 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       62 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       51 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      137 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        6 2023-04-26 06:40:36.000000 twint_fork-2.5.0/twint_fork.egg-info/top_level.txt
```

### Comparing `twint_fork-2.2.0/LICENSE` & `twint_fork-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twint_fork-2.2.0/PKG-INFO` & `twint_fork-2.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: twint_fork
-Version: 2.2.0
+Version: 2.5.0
 Summary: An advanced Twitter scraping & OSINT tool.
-Home-page: https://github.com/twintproject/twint
-Author: Cody Zacharias
-Author-email: codyzacharias@pm.me
+Home-page: https://github.com/yihong0618/twint
+Author: Cody Zacharias, yihong0618
+Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6.0
+Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
+# This is a fork from twint maintain by yihong0618
+
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social) 
 
 >No authentication. No API. No limits.
@@ -89,48 +93,31 @@
 
 Noticed a lot of people are having issues installing (including me). Please use the Dockerfile temporarily while I look into them. 
 
 ## CLI Basic Examples and Combos
 A few simple examples to help you understand the basics:
 
 - `twint -u username` - Scrape all the Tweets of a *user* (doesn't include **retweets** but includes **replies**).
-- `twint -u username -s pineapple` - Scrape all Tweets from the *user*'s timeline containing _pineapple_.
-- `twint -s pineapple` - Collect every Tweet containing *pineapple* from everyone's Tweets.
-- `twint -u username --year 2014` - Collect Tweets that were tweeted **before** 2014.
-- `twint -u username --since "2015-12-20 20:30:15"` - Collect Tweets that were tweeted since 2015-12-20 20:30:15.
-- `twint -u username --since 2015-12-20` - Collect Tweets that were tweeted since 2015-12-20 00:00:00.
-- `twint -u username -o file.txt` - Scrape Tweets and save to file.txt.
-- `twint -u username -o file.csv --csv` - Scrape Tweets and save as a csv file.
-- `twint -u username --email --phone` - Show Tweets that might have phone numbers or email addresses.
-- `twint -s "Donald Trump" --verified` - Display Tweets by verified users that Tweeted about Donald Trump.
-- `twint -g="48.880048,2.385939,1km" -o file.csv --csv` - Scrape Tweets from a radius of 1km around a place in Paris and export them to a csv file.
-- `twint -u username -es localhost:9200` - Output Tweets to Elasticsearch
-- `twint -u username -o file.json --json` - Scrape Tweets and save as a json file.
-- `twint -u username --database tweets.db` - Save Tweets to a SQLite database.
 - `twint -u username --followers` - Scrape a Twitter user's followers.
 - `twint -u username --following` - Scrape who a Twitter user follows.
-- `twint -u username --favorites` - Collect all the Tweets a user has favorited (gathers ~3200 tweet).
-- `twint -u username --following --user-full` - Collect full user information a person follows
-- `twint -u username --timeline` - Use an effective method to gather Tweets from a user's profile (Gathers ~3200 Tweets, including **retweets** & **replies**).
-- `twint -u username --retweets` - Use a quick method to gather the last 900 Tweets (that includes retweets) from a user's profile.
+- `twint -u username --following` - Collect full user information a person follows
 - `twint -u username --resume resume_file.txt` - Resume a search starting from the last saved scroll-id.
 
 More detail about the commands and options are located in the [wiki](https://github.com/twintproject/twint/wiki/Commands)
 
 ## Module Example
 
 Twint can now be used as a module and supports custom formatting. **More details are located in the [wiki](https://github.com/twintproject/twint/wiki/Module)**
 
 ```python
 import twint
 
 # Configure
 c = twint.Config()
 c.Username = "realDonaldTrump"
-c.Search = "great"
 
 # Run
 twint.run.Search(c)
 ```
 > Output
 
 `955511208597184512 2018-01-22 18:43:19 GMT <now> pineapples are the best fruit`
```

### Comparing `twint_fork-2.2.0/README.md` & `twint_fork-2.5.0/twint_fork.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: twint-fork
+Version: 2.5.0
+Summary: An advanced Twitter scraping & OSINT tool.
+Home-page: https://github.com/yihong0618/twint
+Author: Cody Zacharias, yihong0618
+Author-email: codyzacharias@pm.me, zouzou0208@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# This is a fork from twint maintain by yihong0618
+
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social) 
 
 >No authentication. No API. No limits.
@@ -69,48 +93,31 @@
 
 Noticed a lot of people are having issues installing (including me). Please use the Dockerfile temporarily while I look into them. 
 
 ## CLI Basic Examples and Combos
 A few simple examples to help you understand the basics:
 
 - `twint -u username` - Scrape all the Tweets of a *user* (doesn't include **retweets** but includes **replies**).
-- `twint -u username -s pineapple` - Scrape all Tweets from the *user*'s timeline containing _pineapple_.
-- `twint -s pineapple` - Collect every Tweet containing *pineapple* from everyone's Tweets.
-- `twint -u username --year 2014` - Collect Tweets that were tweeted **before** 2014.
-- `twint -u username --since "2015-12-20 20:30:15"` - Collect Tweets that were tweeted since 2015-12-20 20:30:15.
-- `twint -u username --since 2015-12-20` - Collect Tweets that were tweeted since 2015-12-20 00:00:00.
-- `twint -u username -o file.txt` - Scrape Tweets and save to file.txt.
-- `twint -u username -o file.csv --csv` - Scrape Tweets and save as a csv file.
-- `twint -u username --email --phone` - Show Tweets that might have phone numbers or email addresses.
-- `twint -s "Donald Trump" --verified` - Display Tweets by verified users that Tweeted about Donald Trump.
-- `twint -g="48.880048,2.385939,1km" -o file.csv --csv` - Scrape Tweets from a radius of 1km around a place in Paris and export them to a csv file.
-- `twint -u username -es localhost:9200` - Output Tweets to Elasticsearch
-- `twint -u username -o file.json --json` - Scrape Tweets and save as a json file.
-- `twint -u username --database tweets.db` - Save Tweets to a SQLite database.
 - `twint -u username --followers` - Scrape a Twitter user's followers.
 - `twint -u username --following` - Scrape who a Twitter user follows.
-- `twint -u username --favorites` - Collect all the Tweets a user has favorited (gathers ~3200 tweet).
-- `twint -u username --following --user-full` - Collect full user information a person follows
-- `twint -u username --timeline` - Use an effective method to gather Tweets from a user's profile (Gathers ~3200 Tweets, including **retweets** & **replies**).
-- `twint -u username --retweets` - Use a quick method to gather the last 900 Tweets (that includes retweets) from a user's profile.
+- `twint -u username --following` - Collect full user information a person follows
 - `twint -u username --resume resume_file.txt` - Resume a search starting from the last saved scroll-id.
 
 More detail about the commands and options are located in the [wiki](https://github.com/twintproject/twint/wiki/Commands)
 
 ## Module Example
 
 Twint can now be used as a module and supports custom formatting. **More details are located in the [wiki](https://github.com/twintproject/twint/wiki/Module)**
 
 ```python
 import twint
 
 # Configure
 c = twint.Config()
 c.Username = "realDonaldTrump"
-c.Search = "great"
 
 # Run
 twint.run.Search(c)
 ```
 > Output
 
 `955511208597184512 2018-01-22 18:43:19 GMT <now> pineapples are the best fruit`
```

### Comparing `twint_fork-2.2.0/twint/__init__.py` & `twint_fork-2.5.0/twint/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-'''
+"""
 TWINT - Twitter Intelligence Tool (formerly known as Tweep).
 
 See wiki on Github for in-depth details.
 https://github.com/twintproject/twint/wiki
 
 Licensed under MIT License
 Copyright (c) 2018 Cody Zacharias
-'''
+"""
 import logging, os
 
 from .config import Config
 from .__version__ import __version__
 from . import run
 
-_levels = {
-    'info': logging.INFO,
-    'debug': logging.DEBUG
-}
+_levels = {"info": logging.INFO, "debug": logging.DEBUG}
 
-_level = os.getenv('TWINT_DEBUG', 'info')
+_level = os.getenv("TWINT_DEBUG", "info")
 _logLevel = _levels[_level]
 
 if _level == "debug":
     logger = logging.getLogger()
-    _output_fn = 'twint.log'
+    _output_fn = "twint.log"
     logger.setLevel(_logLevel)
-    formatter = logging.Formatter('%(levelname)s:%(asctime)s:%(name)s:%(message)s')
+    formatter = logging.Formatter("%(levelname)s:%(asctime)s:%(name)s:%(message)s")
     fileHandler = logging.FileHandler(_output_fn)
     fileHandler.setLevel(_logLevel)
     fileHandler.setFormatter(formatter)
     logger.addHandler(fileHandler)
```

### Comparing `twint_fork-2.2.0/twint/cli.py` & `twint_fork-2.5.0/twint/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,88 +1,79 @@
 #!/usr/bin/env python3
-'''
+"""
 Twint.py - Twitter Intelligence Tool (formerly known as Tweep).
 
 See wiki on Github for in-depth details.
 https://github.com/twintproject/twint/wiki
 
 Licensed under MIT License
 Copyright (c) 2018 The Twint Project  
-'''
+"""
 import sys
 import os
 import argparse
 
 from . import run
 from . import config
 from . import storage
 
 
 def error(_error, message):
-    """ Print errors to stdout
-    """
+    """Print errors to stdout"""
     print("[-] {}: {}".format(_error, message))
     sys.exit(0)
 
 
 def check(args):
-    """ Error checking
-    """
+    """Error checking"""
     if args.username is not None or args.userlist or args.members_list:
         if args.verified:
-            error("Contradicting Args",
-                  "Please use --verified in combination with -s.")
+            error("Contradicting Args", "Please use --verified in combination with -s.")
         if args.userid:
-            error("Contradicting Args",
-                  "--userid and -u cannot be used together.")
+            error("Contradicting Args", "--userid and -u cannot be used together.")
         if args.all:
-            error("Contradicting Args",
-                  "--all and -u cannot be used together.")
+            error("Contradicting Args", "--all and -u cannot be used together.")
     elif args.search and args.timeline:
-        error("Contradicting Args",
-              "--s and --tl cannot be used together.")
+        error("Contradicting Args", "--s and --tl cannot be used together.")
     elif args.timeline and not args.username:
         error("Error", "-tl cannot be used without -u.")
     elif args.search is None:
         if args.custom_query is not None:
             pass
         elif (args.geo or args.near) is None and not (args.all or args.userid):
             error("Error", "Please use at least -u, -s, -g or --near.")
     elif args.all and args.userid:
-        error("Contradicting Args",
-              "--all and --userid cannot be used together")
+        error("Contradicting Args", "--all and --userid cannot be used together")
     if args.output is None:
         if args.csv:
             error("Error", "Please specify an output file (Example: -o file.csv).")
         elif args.json:
             error("Error", "Please specify an output file (Example: -o file.json).")
     if args.backoff_exponent <= 0:
         error("Error", "Please specifiy a positive value for backoff_exponent")
     if args.min_wait_time < 0:
         error("Error", "Please specifiy a non negative value for min_wait_time")
 
 
 def loadUserList(ul, _type):
-    """ Concatenate users
-    """
+    """Concatenate users"""
     if os.path.exists(os.path.abspath(ul)):
         userlist = open(os.path.abspath(ul), "r").read().splitlines()
     else:
         userlist = ul.split(",")
     if _type == "search":
         un = ""
         for user in userlist:
             un += "%20OR%20from%3A" + user
         return un[15:]
     return userlist
 
 
 def initialize(args):
-    """ Set default values for config from args
-    """
+    """Set default values for config from args"""
     c = config.Config()
     c.Username = args.username
     c.User_id = args.userid
     c.Search = args.search
     c.Geo = args.geo
     c.Location = args.location
     c.Near = args.near
@@ -143,146 +134,278 @@
     c.TranslateDest = args.translate_dest
     c.Backoff_exponent = args.backoff_exponent
     c.Min_wait_time = args.min_wait_time
     return c
 
 
 def options():
-    """ Parse arguments
-    """
-    ap = argparse.ArgumentParser(prog="twint",
-                                 usage="python3 %(prog)s [options]",
-                                 description="TWINT - An Advanced Twitter Scraping Tool.")
+    """Parse arguments"""
+    ap = argparse.ArgumentParser(
+        prog="twint",
+        usage="python3 %(prog)s [options]",
+        description="TWINT - An Advanced Twitter Scraping Tool.",
+    )
     ap.add_argument("-u", "--username", help="User's Tweets you want to scrape.")
-    ap.add_argument("-s", "--search", help="Search for Tweets containing this word or phrase.")
+    ap.add_argument(
+        "-s", "--search", help="Search for Tweets containing this word or phrase."
+    )
     ap.add_argument("-g", "--geo", help="Search for geocoded Tweets.")
     ap.add_argument("--near", help="Near a specified city.")
-    ap.add_argument("--location", help="Show user's location (Experimental).", action="store_true")
+    ap.add_argument(
+        "--location", help="Show user's location (Experimental).", action="store_true"
+    )
     ap.add_argument("-l", "--lang", help="Search for Tweets in a specific language.")
     ap.add_argument("-o", "--output", help="Save output to a file.")
     ap.add_argument("-es", "--elasticsearch", help="Index to Elasticsearch.")
     ap.add_argument("--year", help="Filter Tweets before specified year.")
-    ap.add_argument("--since", help="Filter Tweets sent since date (Example: \"2017-12-27 20:30:15\" or 2017-12-27).",
-                    metavar="DATE")
-    ap.add_argument("--until", help="Filter Tweets sent until date (Example: \"2017-12-27 20:30:15\" or 2017-12-27).",
-                    metavar="DATE")
-    ap.add_argument("--email", help="Filter Tweets that might have email addresses", action="store_true")
-    ap.add_argument("--phone", help="Filter Tweets that might have phone numbers", action="store_true")
-    ap.add_argument("--verified", help="Display Tweets only from verified users (Use with -s).",
-                    action="store_true")
+    ap.add_argument(
+        "--since",
+        help='Filter Tweets sent since date (Example: "2017-12-27 20:30:15" or 2017-12-27).',
+        metavar="DATE",
+    )
+    ap.add_argument(
+        "--until",
+        help='Filter Tweets sent until date (Example: "2017-12-27 20:30:15" or 2017-12-27).',
+        metavar="DATE",
+    )
+    ap.add_argument(
+        "--email",
+        help="Filter Tweets that might have email addresses",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--phone",
+        help="Filter Tweets that might have phone numbers",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--verified",
+        help="Display Tweets only from verified users (Use with -s).",
+        action="store_true",
+    )
     ap.add_argument("--csv", help="Write as .csv file.", action="store_true")
-    ap.add_argument("--tabs", help="Separate CSV fields with tab characters, not commas.", action="store_true")
+    ap.add_argument(
+        "--tabs",
+        help="Separate CSV fields with tab characters, not commas.",
+        action="store_true",
+    )
     ap.add_argument("--json", help="Write as .json file", action="store_true")
-    ap.add_argument("--hashtags", help="Output hashtags in seperate column.", action="store_true")
-    ap.add_argument("--cashtags", help="Output cashtags in seperate column.", action="store_true")
+    ap.add_argument(
+        "--hashtags", help="Output hashtags in seperate column.", action="store_true"
+    )
+    ap.add_argument(
+        "--cashtags", help="Output cashtags in seperate column.", action="store_true"
+    )
     ap.add_argument("--userid", help="Twitter user id.")
     ap.add_argument("--limit", help="Number of Tweets to pull (Increments of 20).")
-    ap.add_argument("--count", help="Display number of Tweets scraped at the end of session.",
-                    action="store_true")
-    ap.add_argument("--stats", help="Show number of replies, retweets, and likes.",
-                    action="store_true")
+    ap.add_argument(
+        "--count",
+        help="Display number of Tweets scraped at the end of session.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--stats",
+        help="Show number of replies, retweets, and likes.",
+        action="store_true",
+    )
     ap.add_argument("-db", "--database", help="Store Tweets in a sqlite3 database.")
     ap.add_argument("--to", help="Search Tweets to a user.", metavar="USERNAME")
-    ap.add_argument("--all", help="Search all Tweets associated with a user.", metavar="USERNAME")
-    ap.add_argument("--followers", help="Scrape a person's followers.", action="store_true")
-    ap.add_argument("--following", help="Scrape a person's follows", action="store_true")
-    ap.add_argument("--favorites", help="Scrape Tweets a user has liked.", action="store_true")
+    ap.add_argument(
+        "--all", help="Search all Tweets associated with a user.", metavar="USERNAME"
+    )
+    ap.add_argument(
+        "--followers", help="Scrape a person's followers.", action="store_true"
+    )
+    ap.add_argument(
+        "--following", help="Scrape a person's follows", action="store_true"
+    )
+    ap.add_argument(
+        "--favorites", help="Scrape Tweets a user has liked.", action="store_true"
+    )
     ap.add_argument("--proxy-type", help="Socks5, HTTP, etc.")
     ap.add_argument("--proxy-host", help="Proxy hostname or IP.")
     ap.add_argument("--proxy-port", help="The port of the proxy server.")
-    ap.add_argument("--tor-control-port", help="If proxy-host is set to tor, this is the control port", default=9051)
-    ap.add_argument("--tor-control-password",
-                    help="If proxy-host is set to tor, this is the password for the control port",
-                    default="my_password")
-    ap.add_argument("--essid",
-                    help="Elasticsearch Session ID, use this to differentiate scraping sessions.",
-                    nargs="?", default="")
+    ap.add_argument(
+        "--tor-control-port",
+        help="If proxy-host is set to tor, this is the control port",
+        default=9051,
+    )
+    ap.add_argument(
+        "--tor-control-password",
+        help="If proxy-host is set to tor, this is the password for the control port",
+        default="my_password",
+    )
+    ap.add_argument(
+        "--essid",
+        help="Elasticsearch Session ID, use this to differentiate scraping sessions.",
+        nargs="?",
+        default="",
+    )
     ap.add_argument("--userlist", help="Userlist from list or file.")
-    ap.add_argument("--retweets",
-                    help="Include user's Retweets (Warning: limited).",
-                    action="store_true")
+    ap.add_argument(
+        "--retweets",
+        help="Include user's Retweets (Warning: limited).",
+        action="store_true",
+    )
     ap.add_argument("--format", help="Custom output format (See wiki for details).")
-    ap.add_argument("--user-full",
-                    help="Collect all user information (Use with followers or following only).",
-                    action="store_true")
+    ap.add_argument(
+        "--user-full",
+        help="Collect all user information (Use with followers or following only).",
+        action="store_true",
+    )
     # I am removing this this feature for the time being, because it is no longer required, default method will do this
     # ap.add_argument("--profile-full",
     #                 help="Slow, but effective method of collecting a user's Tweets and RT.",
     #                 action="store_true")
     ap.add_argument(
         "-tl",
         "--timeline",
         help="Collects every tweet from a User's Timeline. (Tweets, RTs & Replies)",
         action="store_true",
     )
-    ap.add_argument("--translate",
-                    help="Get tweets translated by Google Translate.",
-                    action="store_true")
-    ap.add_argument("--translate-dest", help="Translate tweet to language (ISO2).",
-                    default="en")
+    ap.add_argument(
+        "--translate",
+        help="Get tweets translated by Google Translate.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--translate-dest", help="Translate tweet to language (ISO2).", default="en"
+    )
     ap.add_argument("--store-pandas", help="Save Tweets in a DataFrame (Pandas) file.")
-    ap.add_argument("--pandas-type",
-                    help="Specify HDF5 or Pickle (HDF5 as default)", nargs="?", default="HDF5")
-    ap.add_argument("-it", "--index-tweets",
-                    help="Custom Elasticsearch Index name for Tweets.", nargs="?", default="twinttweets")
-    ap.add_argument("-if", "--index-follow",
-                    help="Custom Elasticsearch Index name for Follows.",
-                    nargs="?", default="twintgraph")
-    ap.add_argument("-iu", "--index-users", help="Custom Elasticsearch Index name for Users.",
-                    nargs="?", default="twintuser")
-    ap.add_argument("--debug",
-                    help="Store information in debug logs", action="store_true")
+    ap.add_argument(
+        "--pandas-type",
+        help="Specify HDF5 or Pickle (HDF5 as default)",
+        nargs="?",
+        default="HDF5",
+    )
+    ap.add_argument(
+        "-it",
+        "--index-tweets",
+        help="Custom Elasticsearch Index name for Tweets.",
+        nargs="?",
+        default="twinttweets",
+    )
+    ap.add_argument(
+        "-if",
+        "--index-follow",
+        help="Custom Elasticsearch Index name for Follows.",
+        nargs="?",
+        default="twintgraph",
+    )
+    ap.add_argument(
+        "-iu",
+        "--index-users",
+        help="Custom Elasticsearch Index name for Users.",
+        nargs="?",
+        default="twintuser",
+    )
+    ap.add_argument(
+        "--debug", help="Store information in debug logs", action="store_true"
+    )
     ap.add_argument("--resume", help="Resume from Tweet ID.", metavar="TWEET_ID")
-    ap.add_argument("--videos", help="Display only Tweets with videos.", action="store_true")
-    ap.add_argument("--images", help="Display only Tweets with images.", action="store_true")
-    ap.add_argument("--media",
-                    help="Display Tweets with only images or videos.", action="store_true")
-    ap.add_argument("--replies", help="Display replies to a subject.", action="store_true")
-    ap.add_argument("-pc", "--pandas-clean",
-                    help="Automatically clean Pandas dataframe at every scrape.")
+    ap.add_argument(
+        "--videos", help="Display only Tweets with videos.", action="store_true"
+    )
+    ap.add_argument(
+        "--images", help="Display only Tweets with images.", action="store_true"
+    )
+    ap.add_argument(
+        "--media",
+        help="Display Tweets with only images or videos.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--replies", help="Display replies to a subject.", action="store_true"
+    )
+    ap.add_argument(
+        "-pc",
+        "--pandas-clean",
+        help="Automatically clean Pandas dataframe at every scrape.",
+    )
     ap.add_argument("-cq", "--custom-query", help="Custom search query.")
-    ap.add_argument("-pt", "--popular-tweets", help="Scrape popular tweets instead of recent ones.",
-                    action="store_true")
-    ap.add_argument("-sc", "--skip-certs", help="Skip certs verification, useful for SSC.", action="store_false")
-    ap.add_argument("-ho", "--hide-output", help="Hide output, no tweets will be displayed.", action="store_true")
-    ap.add_argument("-nr", "--native-retweets", help="Filter the results for retweets only.", action="store_true")
+    ap.add_argument(
+        "-pt",
+        "--popular-tweets",
+        help="Scrape popular tweets instead of recent ones.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "-sc",
+        "--skip-certs",
+        help="Skip certs verification, useful for SSC.",
+        action="store_false",
+    )
+    ap.add_argument(
+        "-ho",
+        "--hide-output",
+        help="Hide output, no tweets will be displayed.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "-nr",
+        "--native-retweets",
+        help="Filter the results for retweets only.",
+        action="store_true",
+    )
     ap.add_argument("--min-likes", help="Filter the tweets by minimum number of likes.")
-    ap.add_argument("--min-retweets", help="Filter the tweets by minimum number of retweets.")
-    ap.add_argument("--min-replies", help="Filter the tweets by minimum number of replies.")
-    ap.add_argument("--links", help="Include or exclude tweets containing one o more links. If not specified" +
-                                    " you will get both tweets that might contain links or not.")
+    ap.add_argument(
+        "--min-retweets", help="Filter the tweets by minimum number of retweets."
+    )
+    ap.add_argument(
+        "--min-replies", help="Filter the tweets by minimum number of replies."
+    )
+    ap.add_argument(
+        "--links",
+        help="Include or exclude tweets containing one o more links. If not specified"
+        + " you will get both tweets that might contain links or not.",
+    )
     ap.add_argument("--source", help="Filter the tweets for specific source client.")
-    ap.add_argument("--members-list", help="Filter the tweets sent by users in a given list.")
-    ap.add_argument("-fr", "--filter-retweets", help="Exclude retweets from the results.", action="store_true")
-    ap.add_argument("--backoff-exponent", help="Specify a exponent for the polynomial backoff in case of errors.",
-                    type=float, default=3.0)
-    ap.add_argument("--min-wait-time", type=float, default=15,
-                    help="specifiy a minimum wait time in case of scraping limit error. This value will be adjusted by twint if the value provided does not satisfy the limits constraints")
+    ap.add_argument(
+        "--members-list", help="Filter the tweets sent by users in a given list."
+    )
+    ap.add_argument(
+        "-fr",
+        "--filter-retweets",
+        help="Exclude retweets from the results.",
+        action="store_true",
+    )
+    ap.add_argument(
+        "--backoff-exponent",
+        help="Specify a exponent for the polynomial backoff in case of errors.",
+        type=float,
+        default=3.0,
+    )
+    ap.add_argument(
+        "--min-wait-time",
+        type=float,
+        default=15,
+        help="specifiy a minimum wait time in case of scraping limit error. This value will be adjusted by twint if the value provided does not satisfy the limits constraints",
+    )
     args = ap.parse_args()
 
     return args
 
 
 def main():
-    """ Main
-    """
+    """Main"""
     args = options()
     check(args)
 
     if args.pandas_clean:
         storage.panda.clean()
 
     c = initialize(args)
 
     if args.userlist:
         c.Query = loadUserList(args.userlist, "search")
 
     if args.pandas_clean:
         storage.panda.clean()
 
+    # for now it had been broken
     if args.favorites:
         if args.userlist:
             _userlist = loadUserList(args.userlist, "favorites")
             for _user in _userlist:
                 args.username = _user
                 c = initialize(args)
                 run.Favorites(c)
@@ -334,9 +457,9 @@
     if sys.version_info < (3, 6):
         print("[-] TWINT requires Python version 3.6+.")
         sys.exit(0)
 
     main()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `twint_fork-2.2.0/twint/config.py` & `twint_fork-2.5.0/twint/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from dataclasses import dataclass
 from typing import Optional
 
+
 @dataclass
 class Config:
     Username: Optional[str] = None
     User_id: Optional[str] = None
     Search: Optional[str] = None
     Lookup: bool = False
     Geo: str = ""
```

### Comparing `twint_fork-2.2.0/twint/datelock.py` & `twint_fork-2.5.0/twint/datelock.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,29 @@
     if ListLength == 1:
         return string + " 00:00:00"
     else:
         return ""
 
 
 def Set(Until, Since):
-    logme.debug(__name__+':Set')
+    logme.debug(__name__ + ":Set")
     d = Datelock()
 
     if Until:
-        d.until = datetime.datetime.strptime(convertToDateTime(Until), "%Y-%m-%d %H:%M:%S")
+        d.until = datetime.datetime.strptime(
+            convertToDateTime(Until), "%Y-%m-%d %H:%M:%S"
+        )
         d.until = utc_to_local(d.until)
     else:
         d.until = datetime.datetime.today()
 
     if Since:
-        d.since = datetime.datetime.strptime(convertToDateTime(Since), "%Y-%m-%d %H:%M:%S")
+        d.since = datetime.datetime.strptime(
+            convertToDateTime(Since), "%Y-%m-%d %H:%M:%S"
+        )
         d.since = utc_to_local(d.since)
         d._since_def_user = True
     else:
         d.since = datetime.datetime.strptime("2006-03-21 00:00:00", "%Y-%m-%d %H:%M:%S")
         d.since = utc_to_local(d.since)
         d._since_def_user = False
```

### Comparing `twint_fork-2.2.0/twint/format.py` & `twint_fork-2.5.0/twint/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging as logme
 
+
 def Tweet(config, t):
     if config.Format:
-        logme.debug(__name__+':Tweet:Format')
+        logme.debug(__name__ + ":Tweet:Format")
         output = config.Format.replace("{id}", t.id_str)
         output = output.replace("{conversation_id}", t.conversation_id)
         output = output.replace("{date}", t.datestamp)
         output = output.replace("{time}", t.timestamp)
         output = output.replace("{user_id}", t.user_id_str)
         output = output.replace("{username}", t.username)
         output = output.replace("{name}", t.name)
@@ -30,15 +31,15 @@
         output = output.replace("{near}", t.near)
         output = output.replace("{geo}", t.geo)
         output = output.replace("{mentions}", ",".join(t.mentions))
         output = output.replace("{translate}", t.translate)
         output = output.replace("{trans_src}", t.trans_src)
         output = output.replace("{trans_dest}", t.trans_dest)
     else:
-        logme.debug(__name__+':Tweet:notFormat')
+        logme.debug(__name__ + ":Tweet:notFormat")
         output = f"{t.id_str} {t.datestamp} {t.timestamp} {t.timezone} "
 
         # TODO: someone who is familiar with this code, needs to take a look at what this is <also see tweet.py>
         # if t.retweet:
         #    output += "RT "
 
         output += f"<{t.username}> {t.tweet}"
@@ -51,17 +52,18 @@
             output += f" {cashtags}"
         if config.Stats:
             output += f" | {t.replies_count} replies {t.retweets_count} retweets {t.likes_count} likes"
         if config.Translate:
             output += f" {t.translate} {t.trans_src} {t.trans_dest}"
     return output
 
+
 def User(_format, u):
     if _format:
-        logme.debug(__name__+':User:Format')
+        logme.debug(__name__ + ":User:Format")
         output = _format.replace("{id}", str(u.id))
         output = output.replace("{name}", u.name)
         output = output.replace("{username}", u.username)
         output = output.replace("{bio}", u.bio)
         output = output.replace("{location}", u.location)
         output = output.replace("{url}", u.url)
         output = output.replace("{join_date}", u.join_date)
@@ -75,15 +77,15 @@
         output = output.replace("{verified}", str(u.is_verified))
         output = output.replace("{avatar}", u.avatar)
         if u.background_image:
             output = output.replace("{background_image}", u.background_image)
         else:
             output = output.replace("{background_image}", "")
     else:
-        logme.debug(__name__+':User:notFormat')
+        logme.debug(__name__ + ":User:notFormat")
         output = f"{u.id} | {u.name} | @{u.username} | Private: "
         output += f"{u.is_private} | Verified: {u.is_verified} |"
         output += f" Bio: {u.bio} | Location: {u.location} | Url: "
         output += f"{u.url} | Joined: {u.join_date} {u.join_time} "
         output += f"| Tweets: {u.tweets} | Following: {u.following}"
         output += f" | Followers: {u.followers} | Likes: {u.likes} "
         output += f"| Media: {u.media_count} | Avatar: {u.avatar}"
```

### Comparing `twint_fork-2.2.0/twint/get.py` & `twint_fork-2.5.0/twint/get.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,243 +37,264 @@
     # ' Chrome/57.0.2987.133 Safari/537.36',
     # 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)'
     # ' Chrome/57.0.2987.133 Safari/537.36',
     # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)'
     # ' Chrome/55.0.2883.87 Safari/537.36',
     # 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko)'
     # ' Chrome/55.0.2883.87 Safari/537.36',
-
-    'Mozilla/4.0 (compatible; MSIE 9.0; Windows NT 6.1)',
-    'Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0)',
-    'Mozilla/5.0 (Windows NT 6.1; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (Windows NT 6.2; WOW64; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0)',
-    'Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0)',
-    'Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko',
-    'Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)',
-    'Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)',
-    'Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 2.0.50727; .NET CLR 3.0.4506.2152; .NET '
-    'CLR 3.5.30729)',
+    "Mozilla/4.0 (compatible; MSIE 9.0; Windows NT 6.1)",
+    "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.1; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (Windows NT 6.2; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)",
+    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)",
+    "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 2.0.50727; .NET CLR 3.0.4506.2152; .NET "
+    "CLR 3.5.30729)",
 ]
 
 
 # function to convert python `dict` to json and then encode it to be passed in the url as a parameter
 # some urls require this format
 def dict_to_url(dct):
     return quote(dumps(dct))
 
 
 def get_connector(config):
-    logme.debug(__name__ + ':get_connector')
+    logme.debug(__name__ + ":get_connector")
     _connector = None
     if config.Proxy_host:
         if config.Proxy_host.lower() == "tor":
-            _connector = ProxyConnector(
-                host='127.0.0.1',
-                port=9050,
-                rdns=True)
+            _connector = ProxyConnector(host="127.0.0.1", port=9050, rdns=True)
         elif config.Proxy_port and config.Proxy_type:
             if config.Proxy_type.lower() == "socks5":
                 _type = ProxyType.SOCKS5
             elif config.Proxy_type.lower() == "socks4":
                 _type = ProxyType.SOCKS4
             elif config.Proxy_type.lower() == "http":
                 global httpproxy
                 httpproxy = "http://" + config.Proxy_host + ":" + str(config.Proxy_port)
                 return _connector
             else:
                 logme.critical("get_connector:proxy-type-error")
-                print("Error: Proxy types allowed are: http, socks5 and socks4. No https.")
+                print(
+                    "Error: Proxy types allowed are: http, socks5 and socks4. No https."
+                )
                 sys.exit(1)
             _connector = ProxyConnector(
                 proxy_type=_type,
                 host=config.Proxy_host,
                 port=config.Proxy_port,
-                rdns=True)
+                rdns=True,
+            )
         else:
-            logme.critical(__name__ + ':get_connector:proxy-port-type-error')
+            logme.critical(__name__ + ":get_connector:proxy-port-type-error")
             print("Error: Please specify --proxy-host, --proxy-port, and --proxy-type")
             sys.exit(1)
     else:
         if config.Proxy_port or config.Proxy_type:
-            logme.critical(__name__ + ':get_connector:proxy-host-arg-error')
+            logme.critical(__name__ + ":get_connector:proxy-host-arg-error")
             print("Error: Please specify --proxy-host, --proxy-port, and --proxy-type")
             sys.exit(1)
 
     return _connector
 
 
 async def RequestUrl(config, init):
-    logme.debug(__name__ + ':RequestUrl')
+    logme.debug(__name__ + ":RequestUrl")
     _connector = get_connector(config)
     _serialQuery = ""
     params = []
     _url = ""
-    _headers = [("authorization", config.Bearer_token), ("x-guest-token", config.Guest_token)]
+    _headers = [
+        ("authorization", config.Bearer_token),
+        ("x-guest-token", config.Guest_token),
+    ]
 
     # TODO : do this later
     if config.Profile:
-        logme.debug(__name__ + ':RequestUrl:Profile')
+        logme.debug(__name__ + ":RequestUrl:Profile")
         _url, params, _serialQuery = url.SearchProfile(config, init)
     elif config.TwitterSearch:
-        logme.debug(__name__ + ':RequestUrl:TwitterSearch')
+        logme.debug(__name__ + ":RequestUrl:TwitterSearch")
         _url, params, _serialQuery = await url.Search(config, init)
     else:
         if config.Following:
-            logme.debug(__name__ + ':RequestUrl:Following')
+            logme.debug(__name__ + ":RequestUrl:Following")
             _url = await url.Following(config.Username, init)
         elif config.Followers:
-            logme.debug(__name__ + ':RequestUrl:Followers')
+            logme.debug(__name__ + ":RequestUrl:Followers")
             _url = await url.Followers(config.Username, init)
         else:
-            logme.debug(__name__ + ':RequestUrl:Favorites')
+            logme.debug(__name__ + ":RequestUrl:Favorites")
             _url = await url.Favorites(config.Username, init)
         _serialQuery = _url
 
-    response = await Request(_url, params=params, connector=_connector, headers=_headers)
+    response = await Request(
+        _url, params=params, connector=_connector, headers=_headers
+    )
 
     if config.Debug:
         print(_serialQuery, file=open("twint-request_urls.log", "a", encoding="utf-8"))
 
     return response
 
 
 def ForceNewTorIdentity(config):
-    logme.debug(__name__ + ':ForceNewTorIdentity')
+    logme.debug(__name__ + ":ForceNewTorIdentity")
     try:
-        tor_c = socket.create_connection(('127.0.0.1', config.Tor_control_port))
-        tor_c.send('AUTHENTICATE "{}"\r\nSIGNAL NEWNYM\r\n'.format(config.Tor_control_password).encode())
+        tor_c = socket.create_connection(("127.0.0.1", config.Tor_control_port))
+        tor_c.send(
+            'AUTHENTICATE "{}"\r\nSIGNAL NEWNYM\r\n'.format(
+                config.Tor_control_password
+            ).encode()
+        )
         response = tor_c.recv(1024)
-        if response != b'250 OK\r\n250 OK\r\n':
-            sys.stderr.write('Unexpected response from Tor control port: {}\n'.format(response))
-            logme.critical(__name__ + ':ForceNewTorIdentity:unexpectedResponse')
+        if response != b"250 OK\r\n250 OK\r\n":
+            sys.stderr.write(
+                "Unexpected response from Tor control port: {}\n".format(response)
+            )
+            logme.critical(__name__ + ":ForceNewTorIdentity:unexpectedResponse")
     except Exception as e:
-        logme.debug(__name__ + ':ForceNewTorIdentity:errorConnectingTor')
-        sys.stderr.write('Error connecting to Tor control port: {}\n'.format(repr(e)))
-        sys.stderr.write('If you want to rotate Tor ports automatically - enable Tor control port\n')
+        logme.debug(__name__ + ":ForceNewTorIdentity:errorConnectingTor")
+        sys.stderr.write("Error connecting to Tor control port: {}\n".format(repr(e)))
+        sys.stderr.write(
+            "If you want to rotate Tor ports automatically - enable Tor control port\n"
+        )
 
 
 async def Request(_url, connector=None, params=None, headers=None):
-    logme.debug(__name__ + ':Request:Connector')
+    logme.debug(__name__ + ":Request:Connector")
     async with aiohttp.ClientSession(
         connector=connector, headers=headers, trust_env=True
     ) as session:
         return await Response(session, _url, params)
 
 
 async def Response(session, _url, params=None):
-    logme.debug(__name__ + ':Response')
+    logme.debug(__name__ + ":Response")
     with timeout(120):
-        async with session.get(_url, ssl=True, params=params, proxy=httpproxy) as response:
+        async with session.get(
+            _url, ssl=True, params=params, proxy=httpproxy
+        ) as response:
             resp = await response.text()
-            if response.status == 429:  # 429 implies Too many requests i.e. Rate Limit Exceeded
-                raise TokenExpiryException(loads(resp)['errors'][0]['message'])
+            if (
+                response.status == 429
+            ):  # 429 implies Too many requests i.e. Rate Limit Exceeded
+                raise TokenExpiryException(loads(resp)["errors"][0]["message"])
             return resp
 
 
 async def RandomUserAgent(wa=None):
-    logme.debug(__name__ + ':RandomUserAgent')
+    logme.debug(__name__ + ":RandomUserAgent")
     try:
         if wa:
             return "Mozilla/5.0 (Windows NT 6.4; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/41.0.2225.0 Safari/537.36"
         return UserAgent(verify_ssl=False, use_cache_server=False).random
     except:
         return random.choice(user_agent_list)
 
 
 async def Username(_id, bearer_token, guest_token):
-    logme.debug(__name__ + ':Username')
-    _dct = {'userId': _id, 'withHighlightedLabel': False}
-    _url = "https://api.twitter.com/graphql/B9FuNQVmyx32rdbIPEZKag/UserByRestId?variables={}".format(dict_to_url(_dct))
+    logme.debug(__name__ + ":Username")
+    _dct = {"userId": _id, "withHighlightedLabel": False}
+    _url = "https://api.twitter.com/graphql/B9FuNQVmyx32rdbIPEZKag/UserByRestId?variables={}".format(
+        dict_to_url(_dct)
+    )
     _headers = {
-        'authorization': bearer_token,
-        'x-guest-token': guest_token,
+        "authorization": bearer_token,
+        "x-guest-token": guest_token,
     }
     r = await Request(_url, headers=_headers)
     j_r = loads(r)
-    username = j_r['data']['user']['legacy']['screen_name']
+    username = j_r["data"]["user"]["legacy"]["screen_name"]
     return username
 
 
 async def Tweet(url, config, conn):
-    logme.debug(__name__ + ':Tweet')
+    logme.debug(__name__ + ":Tweet")
     try:
         response = await Request(url)
         soup = BeautifulSoup(response, "html.parser")
         tweets = soup.find_all("div", "tweet")
         await Tweets(tweets, config, conn, url)
     except Exception as e:
-        logme.critical(__name__ + ':Tweet:' + str(e))
+        logme.critical(__name__ + ":Tweet:" + str(e))
 
 
 async def User(username, config, conn, user_id=False):
-    logme.debug(__name__ + ':User')
-    _dct = {'screen_name': username, 'withHighlightedLabel': False}
-    _url = 'https://api.twitter.com/graphql/jMaTS-_Ea8vh9rpKggJbCQ/UserByScreenName?variables={}'\
-        .format(dict_to_url(_dct))
+    logme.debug(__name__ + ":User")
+    _dct = {"screen_name": username, "withHighlightedLabel": False}
+    _url = f"https://api.twitter.com/1.1/users/show.json?screen_name={username}"
     _headers = {
-        'authorization': config.Bearer_token,
-        'x-guest-token': config.Guest_token,
+        "authorization": config.Bearer_token,
+        "x-guest-token": config.Guest_token,
     }
     try:
         response = await Request(_url, headers=_headers)
         j_r = loads(response)
         if user_id:
             try:
-                _id = j_r['data']['user']['rest_id']
+                _id = j_r["id_str"]
                 return _id
             except KeyError as e:
-                logme.critical(__name__ + ':User:' + str(e))
+                logme.critical(__name__ + ":User:" + str(e))
                 return
         await Users(j_r, config, conn)
     except Exception as e:
-        logme.critical(__name__ + ':User:' + str(e))
+        logme.critical(__name__ + ":User:" + str(e))
         raise
 
 
 def Limit(Limit, count):
-    logme.debug(__name__ + ':Limit')
+    logme.debug(__name__ + ":Limit")
     if Limit is not None and count >= int(Limit):
         return True
 
 
 async def Multi(feed, config, conn):
-    logme.debug(__name__ + ':Multi')
+    logme.debug(__name__ + ":Multi")
     count = 0
     try:
         with concurrent.futures.ThreadPoolExecutor(max_workers=20) as executor:
             loop = asyncio.get_event_loop()
             futures = []
             for tweet in feed:
                 count += 1
                 if config.Favorites or config.Profile_full:
-                    logme.debug(__name__ + ':Multi:Favorites-profileFull')
+                    logme.debug(__name__ + ":Multi:Favorites-profileFull")
                     link = tweet.find("a")["href"]
                     url = f"https://twitter.com{link}&lang=en"
                 elif config.User_full:
-                    logme.debug(__name__ + ':Multi:userFull')
+                    logme.debug(__name__ + ":Multi:userFull")
                     username = tweet.find("a")["name"]
                     url = f"http://twitter.com/{username}?lang=en"
                 else:
-                    logme.debug(__name__ + ':Multi:else-url')
-                    link = tweet.find("a", "tweet-timestamp js-permalink js-nav js-tooltip")["href"]
+                    logme.debug(__name__ + ":Multi:else-url")
+                    link = tweet.find(
+                        "a", "tweet-timestamp js-permalink js-nav js-tooltip"
+                    )["href"]
                     url = f"https://twitter.com{link}?lang=en"
 
                 if config.User_full:
-                    logme.debug(__name__ + ':Multi:user-full-Run')
-                    futures.append(loop.run_in_executor(executor, await User(url,
-                                                                             config, conn)))
+                    logme.debug(__name__ + ":Multi:user-full-Run")
+                    futures.append(
+                        loop.run_in_executor(executor, await User(url, config, conn))
+                    )
                 else:
-                    logme.debug(__name__ + ':Multi:notUser-full-Run')
-                    futures.append(loop.run_in_executor(executor, await Tweet(url,
-                                                                              config, conn)))
-            logme.debug(__name__ + ':Multi:asyncioGather')
+                    logme.debug(__name__ + ":Multi:notUser-full-Run")
+                    futures.append(
+                        loop.run_in_executor(executor, await Tweet(url, config, conn))
+                    )
+            logme.debug(__name__ + ":Multi:asyncioGather")
             await asyncio.gather(*futures)
     except Exception as e:
         # TODO: fix error not error
         # print(str(e) + " [x] get.Multi")
         # will return "'NoneType' object is not callable"
         # but still works
         # logme.critical(__name__+':Multi:' + str(e))
```

### Comparing `twint_fork-2.2.0/twint/output.py` & `twint_fork-2.5.0/twint/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,235 +7,235 @@
 
 import logging as logme
 
 follows_list = []
 tweets_list = []
 users_list = []
 
-author_list = {''}
+author_list = {""}
 author_list.pop()
 
 # used by Pandas
 _follows_object = {}
 
 
 def _formatDateTime(datetimestamp):
     try:
         return int(datetime.strptime(datetimestamp, "%Y-%m-%d %H:%M:%S").timestamp())
     except ValueError:
         return int(datetime.strptime(datetimestamp, "%Y-%m-%d").timestamp())
 
 
 def _clean_follow_list():
-    logme.debug(__name__ + ':clean_follow_list')
+    logme.debug(__name__ + ":clean_follow_list")
     global _follows_object
     _follows_object = {}
 
 
 def clean_lists():
-    logme.debug(__name__ + ':clean_lists')
+    logme.debug(__name__ + ":clean_lists")
     global follows_list
     global tweets_list
     global users_list
     follows_list = []
     tweets_list = []
     users_list = []
 
 
 def datecheck(datetimestamp, config):
-    logme.debug(__name__ + ':datecheck')
+    logme.debug(__name__ + ":datecheck")
     if config.Since:
-        logme.debug(__name__ + ':datecheck:SinceTrue')
+        logme.debug(__name__ + ":datecheck:SinceTrue")
 
         d = _formatDateTime(datetimestamp)
         s = _formatDateTime(config.Since)
 
         if d < s:
             return False
     if config.Until:
-        logme.debug(__name__ + ':datecheck:UntilTrue')
+        logme.debug(__name__ + ":datecheck:UntilTrue")
 
         d = _formatDateTime(datetimestamp)
         s = _formatDateTime(config.Until)
 
         if d > s:
             return False
-    logme.debug(__name__ + ':datecheck:dateRangeFalse')
+    logme.debug(__name__ + ":datecheck:dateRangeFalse")
     return True
 
 
 # TODO In this method we need to delete the quoted tweets, because twitter also sends the quoted tweets in the
 #  `tweets` list along with the other tweets
 def is_tweet(tw):
     try:
         tw["data-item-id"]
-        logme.debug(__name__ + ':is_tweet:True')
+        logme.debug(__name__ + ":is_tweet:True")
         return True
     except:
-        logme.critical(__name__ + ':is_tweet:False')
+        logme.critical(__name__ + ":is_tweet:False")
         return False
 
 
 def _output(obj, output, config, **extra):
-    logme.debug(__name__ + ':_output')
+    logme.debug(__name__ + ":_output")
     if config.Lowercase:
         if isinstance(obj, str):
-            logme.debug(__name__ + ':_output:Lowercase:username')
+            logme.debug(__name__ + ":_output:Lowercase:username")
             obj = obj.lower()
         elif obj.__class__.__name__ == "user":
-            logme.debug(__name__ + ':_output:Lowercase:user')
+            logme.debug(__name__ + ":_output:Lowercase:user")
             pass
         elif obj.__class__.__name__ == "tweet":
-            logme.debug(__name__ + ':_output:Lowercase:tweet')
+            logme.debug(__name__ + ":_output:Lowercase:tweet")
             obj.username = obj.username.lower()
             author_list.update({obj.username})
             for dct in obj.mentions:
                 for key, val in dct.items():
                     dct[key] = val.lower()
             for i in range(len(obj.hashtags)):
                 obj.hashtags[i] = obj.hashtags[i].lower()
             for i in range(len(obj.cashtags)):
                 obj.cashtags[i] = obj.cashtags[i].lower()
         else:
-            logme.info('_output:Lowercase:hiddenTweetFound')
+            logme.info("_output:Lowercase:hiddenTweetFound")
             print("[x] Hidden tweet found, account suspended due to violation of TOS")
             return
     if config.Output != None:
         if config.Store_csv:
             try:
                 write.Csv(obj, config)
-                logme.debug(__name__ + ':_output:CSV')
+                logme.debug(__name__ + ":_output:CSV")
             except Exception as e:
-                logme.critical(__name__ + ':_output:CSV:Error:' + str(e))
+                logme.critical(__name__ + ":_output:CSV:Error:" + str(e))
                 print(str(e) + " [x] output._output")
         elif config.Store_json:
             write.Json(obj, config)
-            logme.debug(__name__ + ':_output:JSON')
+            logme.debug(__name__ + ":_output:JSON")
         else:
             write.Text(output, config.Output)
-            logme.debug(__name__ + ':_output:Text')
+            logme.debug(__name__ + ":_output:Text")
 
     if config.Elasticsearch:
-        logme.debug(__name__ + ':_output:Elasticsearch')
+        logme.debug(__name__ + ":_output:Elasticsearch")
         print("", end=".", flush=True)
     else:
         if not config.Hide_output:
             try:
-                print(output.replace('\n', ' '))
+                print(output.replace("\n", " "))
             except UnicodeEncodeError:
-                logme.critical(__name__ + ':_output:UnicodeEncodeError')
+                logme.critical(__name__ + ":_output:UnicodeEncodeError")
                 print("unicode error [x] output._output")
 
 
 async def checkData(tweet, config, conn):
-    logme.debug(__name__ + ':checkData')
+    logme.debug(__name__ + ":checkData")
     tweet = Tweet(tweet, config)
     if not tweet.datestamp:
-        logme.critical(__name__ + ':checkData:hiddenTweetFound')
+        logme.critical(__name__ + ":checkData:hiddenTweetFound")
         print("[x] Hidden tweet found, account suspended due to violation of TOS")
         return
     if datecheck(tweet.datestamp + " " + tweet.timestamp, config):
         output = format.Tweet(config, tweet)
         if config.Database:
-            logme.debug(__name__ + ':checkData:Database')
+            logme.debug(__name__ + ":checkData:Database")
             db.tweets(conn, tweet, config)
         if config.Pandas:
-            logme.debug(__name__ + ':checkData:Pandas')
+            logme.debug(__name__ + ":checkData:Pandas")
             panda.update(tweet, config)
         if config.Store_object:
-            logme.debug(__name__ + ':checkData:Store_object')
-            if hasattr(config.Store_object_tweets_list, 'append'):
+            logme.debug(__name__ + ":checkData:Store_object")
+            if hasattr(config.Store_object_tweets_list, "append"):
                 config.Store_object_tweets_list.append(tweet)
             else:
                 tweets_list.append(tweet)
         if config.Elasticsearch:
-            logme.debug(__name__ + ':checkData:Elasticsearch')
+            logme.debug(__name__ + ":checkData:Elasticsearch")
             elasticsearch.Tweet(tweet, config)
         _output(tweet, output, config)
     # else:
     #     logme.critical(__name__+':checkData:copyrightedTweet')
 
 
 async def Tweets(tweets, config, conn):
-    logme.debug(__name__ + ':Tweets')
+    logme.debug(__name__ + ":Tweets")
     if config.Favorites or config.Location:
-        logme.debug(__name__ + ':Tweets:fav+full+loc')
+        logme.debug(__name__ + ":Tweets:fav+full+loc")
         for tw in tweets:
             await checkData(tw, config, conn)
     elif config.TwitterSearch or config.Profile:
-        logme.debug(__name__ + ':Tweets:TwitterSearch')
+        logme.debug(__name__ + ":Tweets:TwitterSearch")
         await checkData(tweets, config, conn)
     else:
-        logme.debug(__name__ + ':Tweets:else')
+        logme.debug(__name__ + ":Tweets:else")
         if int(tweets["data-user-id"]) == config.User_id or config.Retweets:
             await checkData(tweets, config, conn)
 
 
 async def Users(u, config, conn):
-    logme.debug(__name__ + ':User')
+    logme.debug(__name__ + ":User")
     global users_list
 
     user = User(u)
     output = format.User(config.Format, user)
 
     if config.Database:
-        logme.debug(__name__ + ':User:Database')
+        logme.debug(__name__ + ":User:Database")
         db.user(conn, config, user)
 
     if config.Elasticsearch:
-        logme.debug(__name__ + ':User:Elasticsearch')
+        logme.debug(__name__ + ":User:Elasticsearch")
         _save_date = user.join_date
         _save_time = user.join_time
         user.join_date = str(datetime.strptime(user.join_date, "%d %b %Y")).split()[0]
         user.join_time = str(datetime.strptime(user.join_time, "%I:%M %p")).split()[1]
         elasticsearch.UserProfile(user, config)
         user.join_date = _save_date
         user.join_time = _save_time
 
     if config.Store_object:
-        logme.debug(__name__ + ':User:Store_object')
+        logme.debug(__name__ + ":User:Store_object")
 
-        if hasattr(config.Store_object_follow_list, 'append'):
+        if hasattr(config.Store_object_follow_list, "append"):
             config.Store_object_follow_list.append(user)
-        elif hasattr(config.Store_object_users_list, 'append'):
+        elif hasattr(config.Store_object_users_list, "append"):
             config.Store_object_users_list.append(user)
         else:
             users_list.append(user)  # twint.user.user
 
     if config.Pandas:
-        logme.debug(__name__ + ':User:Pandas+user')
+        logme.debug(__name__ + ":User:Pandas+user")
         panda.update(user, config)
 
     _output(user, output, config)
 
 
 async def Username(username, config, conn):
-    logme.debug(__name__ + ':Username')
+    logme.debug(__name__ + ":Username")
     global _follows_object
     global follows_list
     follow_var = config.Following * "following" + config.Followers * "followers"
 
     if config.Database:
-        logme.debug(__name__ + ':Username:Database')
+        logme.debug(__name__ + ":Username:Database")
         db.follow(conn, config.Username, config.Followers, username)
 
     if config.Elasticsearch:
-        logme.debug(__name__ + ':Username:Elasticsearch')
+        logme.debug(__name__ + ":Username:Elasticsearch")
         elasticsearch.Follow(username, config)
 
     if config.Store_object:
-        if hasattr(config.Store_object_follow_list, 'append'):
+        if hasattr(config.Store_object_follow_list, "append"):
             config.Store_object_follow_list.append(username)
         else:
             follows_list.append(username)  # twint.user.user
 
     if config.Pandas:
-        logme.debug(__name__ + ':Username:object+pandas')
+        logme.debug(__name__ + ":Username:object+pandas")
         try:
             _ = _follows_object[config.Username][follow_var]
         except KeyError:
             _follows_object.update({config.Username: {follow_var: []}})
         _follows_object[config.Username][follow_var].append(username)
         if config.Pandas_au:
-            logme.debug(__name__ + ':Username:object+pandas+au')
+            logme.debug(__name__ + ":Username:object+pandas+au")
             panda.update(_follows_object[config.Username], config)
     _output(username, username, config)
```

### Comparing `twint_fork-2.2.0/twint/run.py` & `twint_fork-2.5.0/twint/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import sys, os, datetime
-from asyncio import get_event_loop, TimeoutError, ensure_future, new_event_loop, set_event_loop
+from asyncio import (
+    get_event_loop,
+    TimeoutError,
+    ensure_future,
+    new_event_loop,
+    set_event_loop,
+)
 
 from . import datelock, feed, get, output, verbose, storage
 from .token import TokenExpiryException
 from . import token
 from .storage import db
 from .feed import NoMoreTweetsException
 
 import logging as logme
 
 import time
 
-bearer = 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs' \
-         '%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA'
+bearer = (
+    "Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs"
+    "%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA"
+)
 
 
 class Twint:
     def __init__(self, config):
-        logme.debug(__name__ + ':Twint:__init__')
-        if config.Resume is not None and (config.TwitterSearch or config.Followers or config.Following):
-            logme.debug(__name__ + ':Twint:__init__:Resume')
+        logme.debug(__name__ + ":Twint:__init__")
+        if config.Resume is not None and (
+            config.TwitterSearch or config.Followers or config.Following
+        ):
+            logme.debug(__name__ + ":Twint:__init__:Resume")
             self.init = self.get_resume(config.Resume)
         else:
             self.init = -1
 
         config.deleted = []
         self.feed: list = [-1]
         self.count = 0
@@ -32,205 +42,251 @@
         self.config.Bearer_token = bearer
         # TODO might have to make some adjustments for it to work with multi-treading
         # USAGE : to get a new guest token simply do `self.token.refresh()`
         self.token = token.Token(config)
         self.token.refresh()
         self.conn = db.Conn(config.Database)
         self.d = datelock.Set(self.config.Until, self.config.Since)
+        self.is_feed_done = False
         verbose.Elastic(config.Elasticsearch)
 
         if self.config.Store_object:
-            logme.debug(__name__ + ':Twint:__init__:clean_follow_list')
+            logme.debug(__name__ + ":Twint:__init__:clean_follow_list")
             output._clean_follow_list()
 
         if self.config.Pandas_clean:
-            logme.debug(__name__ + ':Twint:__init__:pandas_clean')
+            logme.debug(__name__ + ":Twint:__init__:pandas_clean")
             storage.panda.clean()
 
     def get_resume(self, resumeFile):
         if not os.path.exists(resumeFile):
-            return '-1'
-        with open(resumeFile, 'r') as rFile:
-            _init = rFile.readlines()[-1].strip('\n')
+            return "-1"
+        with open(resumeFile, "r") as rFile:
+            _init = rFile.readlines()[-1].strip("\n")
             return _init
 
     async def Feed(self):
-        logme.debug(__name__ + ':Twint:Feed')
+        logme.debug(__name__ + ":Twint:Feed")
         consecutive_errors_count = 0
         while True:
             # this will receive a JSON string, parse it into a `dict` and do the required stuff
             try:
                 response = await get.RequestUrl(self.config, self.init)
             except TokenExpiryException as e:
-                logme.debug(__name__ + 'Twint:Feed:' + str(e))
+                logme.debug(__name__ + "Twint:Feed:" + str(e))
                 self.token.refresh()
                 response = await get.RequestUrl(self.config, self.init)
 
             if self.config.Debug:
-                print(response, file=open("twint-last-request.log", "w", encoding="utf-8"))
+                print(
+                    response, file=open("twint-last-request.log", "w", encoding="utf-8")
+                )
 
             self.feed = []
             try:
                 if self.config.Favorites:
                     self.feed, self.init = feed.MobileFav(response)
                     favorite_err_cnt = 0
                     if len(self.feed) == 0 and len(self.init) == 0:
-                        while (len(self.feed) == 0 or len(self.init) == 0) and favorite_err_cnt < 5:
+                        while (
+                            len(self.feed) == 0 or len(self.init) == 0
+                        ) and favorite_err_cnt < 5:
                             self.user_agent = await get.RandomUserAgent(wa=False)
-                            response = await get.RequestUrl(self.config, self.init,
-                                                            headers=[("User-Agent", self.user_agent)])
+                            response = await get.RequestUrl(
+                                self.config,
+                                self.init,
+                                headers=[("User-Agent", self.user_agent)],
+                            )
                             self.feed, self.init = feed.MobileFav(response)
                             favorite_err_cnt += 1
                             time.sleep(1)
                         if favorite_err_cnt == 5:
                             print("Favorite page could not be fetched")
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Followers or self.config.Following:
                     self.feed, self.init = feed.Follow(response)
                     if not self.count % 40:
                         time.sleep(5)
                 elif self.config.Profile or self.config.TwitterSearch:
                     try:
-                        self.feed, self.init = feed.parse_tweets(self.config, response)
+                        # track the max_id if we need to continue
+                        # ticky to make slef.feed to empty
+                        # TODO
+                        self.feed, init = feed.parse_tweets(
+                            self.config, response, self.init
+                        )
+                        if self.init != init or init == -1:
+                            self.init = init
+                        else:
+                            self.is_feed_done = True
+                            break
                     except NoMoreTweetsException as e:
-                        logme.debug(__name__ + ':Twint:Feed:' + str(e))
-                        print('[!] ' + str(e) + ' Scraping will stop now.')
-                        print('found {} deleted tweets in this search.'.format(len(self.config.deleted)))
+                        logme.debug(__name__ + ":Twint:Feed:" + str(e))
+                        print("[!] " + str(e) + " Scraping will stop now.")
+                        print(
+                            "found {} deleted tweets in this search.".format(
+                                len(self.config.deleted)
+                            )
+                        )
                         break
                 break
             except TimeoutError as e:
                 if self.config.Proxy_host.lower() == "tor":
                     print("[?] Timed out, changing Tor identity...")
                     if self.config.Tor_control_password is None:
-                        logme.critical(__name__ + ':Twint:Feed:tor-password')
-                        sys.stderr.write("Error: config.Tor_control_password must be set for proxy auto-rotation!\r\n")
+                        logme.critical(__name__ + ":Twint:Feed:tor-password")
+                        sys.stderr.write(
+                            "Error: config.Tor_control_password must be set for proxy auto-rotation!\r\n"
+                        )
                         sys.stderr.write(
                             "Info: What is it? See https://stem.torproject.org/faq.html#can-i-interact-with-tors"
-                            "-controller-interface-directly\r\n")
+                            "-controller-interface-directly\r\n"
+                        )
                         break
                     else:
                         get.ForceNewTorIdentity(self.config)
                         continue
                 else:
-                    logme.critical(__name__ + ':Twint:Feed:' + str(e))
+                    logme.critical(__name__ + ":Twint:Feed:" + str(e))
                     print(str(e))
                     break
             except Exception as e:
                 if self.config.Profile or self.config.Favorites:
                     print("[!] Twitter does not return more data, scrape stops here.")
                     break
 
-                logme.critical(__name__ + ':Twint:Feed:noData' + str(e))
+                logme.critical(__name__ + ":Twint:Feed:noData" + str(e))
                 # Sometimes Twitter says there is no data. But it's a lie.
                 # raise
                 consecutive_errors_count += 1
                 if consecutive_errors_count < self.config.Retries_count:
                     # skip to the next iteration if wait time does not satisfy limit constraints
-                    delay = round(consecutive_errors_count ** self.config.Backoff_exponent, 1)
+                    delay = round(
+                        consecutive_errors_count**self.config.Backoff_exponent, 1
+                    )
 
                     # if the delay is less than users set min wait time then replace delay
                     if self.config.Min_wait_time > delay:
                         delay = self.config.Min_wait_time
 
-                    sys.stderr.write('sleeping for {} secs\n'.format(delay))
+                    sys.stderr.write("sleeping for {} secs\n".format(delay))
                     time.sleep(delay)
                     self.user_agent = await get.RandomUserAgent(wa=True)
                     continue
-                logme.critical(__name__ + ':Twint:Feed:Tweets_known_error:' + str(e))
+                logme.critical(__name__ + ":Twint:Feed:Tweets_known_error:" + str(e))
                 sys.stderr.write(str(e) + " [x] run.Feed")
                 sys.stderr.write(
                     "[!] if you get this error but you know for sure that more tweets exist, please open an issue and "
-                    "we will investigate it!")
+                    "we will investigate it!"
+                )
                 break
         if self.config.Resume:
             print(self.init, file=open(self.config.Resume, "a", encoding="utf-8"))
 
     async def follow(self):
         await self.Feed()
         if self.config.User_full:
-            logme.debug(__name__ + ':Twint:follow:userFull')
+            logme.debug(__name__ + ":Twint:follow:userFull")
             self.count += await get.Multi(self.feed, self.config, self.conn)
         else:
-            logme.debug(__name__ + ':Twint:follow:notUserFull')
+            logme.debug(__name__ + ":Twint:follow:notUserFull")
             for user in self.feed:
                 self.count += 1
-                username = user.find("a")["name"]
+                username = user["screen_name"]
                 await output.Username(username, self.config, self.conn)
 
     async def favorite(self):
-        logme.debug(__name__ + ':Twint:favorite')
+        logme.debug(__name__ + ":Twint:favorite")
         await self.Feed()
         favorited_tweets_list = []
         for tweet in self.feed:
             tweet_dict = {}
             self.count += 1
             try:
-                tweet_dict['data-item-id'] = tweet.find("div", {"class": "tweet-text"})['data-id']
+                tweet_dict["data-item-id"] = tweet.find("div", {"class": "tweet-text"})[
+                    "data-id"
+                ]
                 t_url = tweet.find("span", {"class": "metadata"}).find("a")["href"]
-                tweet_dict['data-conversation-id'] = t_url.split('?')[0].split('/')[-1]
-                tweet_dict['username'] = tweet.find("div", {"class": "username"}).text.replace('\n', '').replace(' ',
-                                                                                                                 '')
-                tweet_dict['tweet'] = tweet.find("div", {"class": "tweet-text"}).find("div", {"class": "dir-ltr"}).text
+                tweet_dict["data-conversation-id"] = t_url.split("?")[0].split("/")[-1]
+                tweet_dict["username"] = (
+                    tweet.find("div", {"class": "username"})
+                    .text.replace("\n", "")
+                    .replace(" ", "")
+                )
+                tweet_dict["tweet"] = (
+                    tweet.find("div", {"class": "tweet-text"})
+                    .find("div", {"class": "dir-ltr"})
+                    .text
+                )
                 date_str = tweet.find("td", {"class": "timestamp"}).find("a").text
                 # test_dates = ["1m", "2h", "Jun 21, 2019", "Mar 12", "28 Jun 19"]
                 # date_str = test_dates[3]
-                if len(date_str) <= 3 and (date_str[-1] == "m" or date_str[-1] == "h"):  # 25m 1h
+                if len(date_str) <= 3 and (
+                    date_str[-1] == "m" or date_str[-1] == "h"
+                ):  # 25m 1h
                     dateu = str(datetime.date.today())
-                    tweet_dict['date'] = dateu
-                elif ',' in date_str:  # Aug 21, 2019
-                    sp = date_str.replace(',', '').split(' ')
-                    date_str_formatted = sp[1] + ' ' + sp[0] + ' ' + sp[2]
-                    dateu = datetime.datetime.strptime(date_str_formatted, "%d %b %Y").strftime("%Y-%m-%d")
-                    tweet_dict['date'] = dateu
-                elif len(date_str.split(' ')) == 3:  # 28 Jun 19
-                    sp = date_str.split(' ')
+                    tweet_dict["date"] = dateu
+                elif "," in date_str:  # Aug 21, 2019
+                    sp = date_str.replace(",", "").split(" ")
+                    date_str_formatted = sp[1] + " " + sp[0] + " " + sp[2]
+                    dateu = datetime.datetime.strptime(
+                        date_str_formatted, "%d %b %Y"
+                    ).strftime("%Y-%m-%d")
+                    tweet_dict["date"] = dateu
+                elif len(date_str.split(" ")) == 3:  # 28 Jun 19
+                    sp = date_str.split(" ")
                     if len(sp[2]) == 2:
-                        sp[2] = '20' + sp[2]
-                    date_str_formatted = sp[0] + ' ' + sp[1] + ' ' + sp[2]
-                    dateu = datetime.datetime.strptime(date_str_formatted, "%d %b %Y").strftime("%Y-%m-%d")
-                    tweet_dict['date'] = dateu
+                        sp[2] = "20" + sp[2]
+                    date_str_formatted = sp[0] + " " + sp[1] + " " + sp[2]
+                    dateu = datetime.datetime.strptime(
+                        date_str_formatted, "%d %b %Y"
+                    ).strftime("%Y-%m-%d")
+                    tweet_dict["date"] = dateu
                 else:  # Aug 21
-                    sp = date_str.split(' ')
-                    date_str_formatted = sp[1] + ' ' + sp[0] + ' ' + str(datetime.date.today().year)
-                    dateu = datetime.datetime.strptime(date_str_formatted, "%d %b %Y").strftime("%Y-%m-%d")
-                    tweet_dict['date'] = dateu
+                    sp = date_str.split(" ")
+                    date_str_formatted = (
+                        sp[1] + " " + sp[0] + " " + str(datetime.date.today().year)
+                    )
+                    dateu = datetime.datetime.strptime(
+                        date_str_formatted, "%d %b %Y"
+                    ).strftime("%Y-%m-%d")
+                    tweet_dict["date"] = dateu
 
                 favorited_tweets_list.append(tweet_dict)
 
             except Exception as e:
-                logme.critical(__name__ + ':Twint:favorite:favorite_field_lack')
+                logme.critical(__name__ + ":Twint:favorite:favorite_field_lack")
                 print("shit: ", date_str, " ", str(e))
 
         try:
             self.config.favorited_tweets_list += favorited_tweets_list
         except AttributeError:
             self.config.favorited_tweets_list = favorited_tweets_list
 
     async def profile(self):
         await self.Feed()
-        logme.debug(__name__ + ':Twint:profile')
+        logme.debug(__name__ + ":Twint:profile")
         for tweet in self.feed:
             self.count += 1
             await output.Tweets(tweet, self.config, self.conn)
 
     async def tweets(self):
         await self.Feed()
         # TODO : need to take care of this later
         if self.config.Location:
-            logme.debug(__name__ + ':Twint:tweets:location')
+            logme.debug(__name__ + ":Twint:tweets:location")
             self.count += await get.Multi(self.feed, self.config, self.conn)
         else:
-            logme.debug(__name__ + ':Twint:tweets:notLocation')
+            logme.debug(__name__ + ":Twint:tweets:notLocation")
             for tweet in self.feed:
                 self.count += 1
                 await output.Tweets(tweet, self.config, self.conn)
 
     async def main(self, callback=None):
-
         task = ensure_future(self.run())  # Might be changed to create_task in 3.7+.
 
         if callback:
             task.add_done_callback(callback)
 
         await task
 
@@ -241,116 +297,137 @@
     async def run(self):
         if self.config.TwitterSearch:
             self.user_agent = await get.RandomUserAgent(wa=True)
         else:
             self.user_agent = await get.RandomUserAgent()
 
         if self.config.User_id is not None and self.config.Username is None:
-            logme.debug(__name__ + ':Twint:main:user_id')
-            self.config.Username = await get.Username(self.config.User_id, self.config.Bearer_token,
-                                                      self.config.Guest_token)
+            logme.debug(__name__ + ":Twint:main:user_id")
+            self.config.Username = await get.Username(
+                self.config.User_id, self.config.Bearer_token, self.config.Guest_token
+            )
 
         if self.config.Username is not None and self.config.User_id is None:
-            logme.debug(__name__ + ':Twint:main:username')
-
-            self.config.User_id = await get.User(self.config.Username, self.config, self.conn, True)
+            logme.debug(__name__ + ":Twint:main:username")
+            self.config.User_id = await get.User(
+                self.config.Username, self.config, self.conn, True
+            )
             if self.config.User_id is None:
-                raise ValueError("Cannot find twitter account with name = " + self.config.Username)
+                raise ValueError(
+                    "Cannot find twitter account with name = " + self.config.Username
+                )
 
         # TODO : will need to modify it to work with the new endpoints
         if self.config.TwitterSearch and self.config.Since and self.config.Until:
-            logme.debug(__name__ + ':Twint:main:search+since+until')
+            logme.debug(__name__ + ":Twint:main:search+since+until")
             while self.d.since < self.d.until:
-                self.config.Since = datetime.datetime.strftime(self.d.since, "%Y-%m-%d %H:%M:%S")
-                self.config.Until = datetime.datetime.strftime(self.d.until, "%Y-%m-%d %H:%M:%S")
+                self.config.Since = datetime.datetime.strftime(
+                    self.d.since, "%Y-%m-%d %H:%M:%S"
+                )
+                self.config.Until = datetime.datetime.strftime(
+                    self.d.until, "%Y-%m-%d %H:%M:%S"
+                )
                 if len(self.feed) > 0:
                     await self.tweets()
                 else:
-                    logme.debug(__name__ + ':Twint:main:gettingNewTweets')
+                    logme.debug(__name__ + ":Twint:main:gettingNewTweets")
                     break
 
                 if get.Limit(self.config.Limit, self.count):
                     break
         elif self.config.Lookup:
             await self.Lookup()
         else:
-            logme.debug(__name__ + ':Twint:main:not-search+since+until')
+            logme.debug(__name__ + ":Twint:main:not-search+since+until")
             while True:
                 if len(self.feed) > 0:
                     if self.config.Followers or self.config.Following:
-                        logme.debug(__name__ + ':Twint:main:follow')
+                        logme.debug(__name__ + ":Twint:main:follow")
                         await self.follow()
                     elif self.config.Favorites:
-                        logme.debug(__name__ + ':Twint:main:favorites')
+                        logme.debug(__name__ + ":Twint:main:favorites")
                         await self.favorite()
                     elif self.config.Profile:
-                        logme.debug(__name__ + ':Twint:main:profile')
+                        logme.debug(__name__ + ":Twint:main:profile")
                         await self.profile()
                     elif self.config.TwitterSearch:
-                        logme.debug(__name__ + ':Twint:main:twitter-search')
+                        logme.debug(__name__ + ":Twint:main:twitter-search")
                         await self.tweets()
+                        # this code is a mess, tricky to get it done
+                        if self.is_feed_done:
+                            break
                 else:
-                    logme.debug(__name__ + ':Twint:main:no-more-tweets')
+                    logme.debug(__name__ + ":Twint:main:no-more-tweets")
                     break
 
                 # logging.info("[<] " + str(datetime.now()) + ':: run+Twint+main+CallingGetLimit2')
                 if get.Limit(self.config.Limit, self.count):
-                    logme.debug(__name__ + ':Twint:main:reachedLimit')
+                    logme.debug(__name__ + ":Twint:main:reachedLimit")
                     break
 
         if self.config.Count:
             verbose.Count(self.count, self.config)
 
     async def Lookup(self):
-        logme.debug(__name__ + ':Twint:Lookup')
+        logme.debug(__name__ + ":Twint:Lookup")
 
         try:
             if self.config.User_id is not None and self.config.Username is None:
-                logme.debug(__name__ + ':Twint:Lookup:user_id')
-                self.config.Username = await get.Username(self.config.User_id, self.config.Bearer_token,
-                                                          self.config.Guest_token)
-            await get.User(self.config.Username, self.config, db.Conn(self.config.Database))
+                logme.debug(__name__ + ":Twint:Lookup:user_id")
+                self.config.Username = await get.Username(
+                    self.config.User_id,
+                    self.config.Bearer_token,
+                    self.config.Guest_token,
+                )
+            await get.User(
+                self.config.Username, self.config, db.Conn(self.config.Database)
+            )
 
         except Exception as e:
-            logme.exception(__name__ + ':Twint:Lookup:Unexpected exception occurred.')
+            logme.exception(__name__ + ":Twint:Lookup:Unexpected exception occurred.")
             raise
 
 
 def run(config, callback=None):
-    logme.debug(__name__ + ':run')
+    logme.debug(__name__ + ":run")
     try:
         get_event_loop()
     except RuntimeError as e:
         if "no current event loop" in str(e):
             set_event_loop(new_event_loop())
         else:
-            logme.exception(__name__ + ':run:Unexpected exception while handling an expected RuntimeError.')
+            logme.exception(
+                __name__
+                + ":run:Unexpected exception while handling an expected RuntimeError."
+            )
             raise
     except Exception as e:
         logme.exception(
-            __name__ + ':run:Unexpected exception occurred while attempting to get or create a new event loop.')
+            __name__
+            + ":run:Unexpected exception occurred while attempting to get or create a new event loop."
+        )
         raise
 
     get_event_loop().run_until_complete(Twint(config).main(callback))
 
 
 def Favorites(config):
-    logme.debug(__name__ + ':Favorites')
+    logme.debug(__name__ + ":Favorites")
     config.Favorites = True
     config.Following = False
     config.Followers = False
     config.Profile = False
     config.TwitterSearch = False
     run(config)
     if config.Pandas_au:
         storage.panda._autoget("tweet")
 
 
 def Followers(config):
-    logme.debug(__name__ + ':Followers')
+    logme.debug(__name__ + ":Followers")
     config.Followers = True
     config.Following = False
     config.Profile = False
     config.Favorites = False
     config.TwitterSearch = False
     run(config)
     if config.Pandas_au:
@@ -359,15 +436,15 @@
             storage.panda._autoget("user")
     if config.Pandas_clean and not config.Store_object:
         # storage.panda.clean()
         output._clean_follow_list()
 
 
 def Following(config):
-    logme.debug(__name__ + ':Following')
+    logme.debug(__name__ + ":Following")
     config.Following = True
     config.Followers = False
     config.Profile = False
     config.Favorites = False
     config.TwitterSearch = False
     run(config)
     if config.Pandas_au:
@@ -376,40 +453,40 @@
             storage.panda._autoget("user")
     if config.Pandas_clean and not config.Store_object:
         # storage.panda.clean()
         output._clean_follow_list()
 
 
 def Lookup(config):
-    logme.debug(__name__ + ':Lookup')
+    logme.debug(__name__ + ":Lookup")
     config.Profile = False
     config.Lookup = True
     config.Favorites = False
     config.FOllowing = False
     config.Followers = False
     config.TwitterSearch = False
     run(config)
     if config.Pandas_au:
         storage.panda._autoget("user")
 
 
 def Profile(config):
-    logme.debug(__name__ + ':Profile')
+    logme.debug(__name__ + ":Profile")
     config.Profile = True
     config.Favorites = False
     config.Following = False
     config.Followers = False
     config.TwitterSearch = False
     run(config)
     if config.Pandas_au:
         storage.panda._autoget("tweet")
 
 
 def Search(config, callback=None):
-    logme.debug(__name__ + ':Search')
+    logme.debug(__name__ + ":Search")
     config.TwitterSearch = True
     config.Favorites = False
     config.Following = False
     config.Followers = False
     config.Profile = False
     run(config, callback)
     if config.Pandas_au:
```

### Comparing `twint_fork-2.2.0/twint/storage/db.py` & `twint_fork-2.5.0/twint/storage/db.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import sys
 import time
 import hashlib
 import json
 
 from datetime import datetime
 
+
 def Conn(database):
     if database:
         print("[+] Inserting into Database: " + str(database))
         conn = init(database)
-        if isinstance(conn, str): # error
+        if isinstance(conn, str):  # error
             print(conn)
             sys.exit(1)
     else:
         conn = ""
 
     return conn
 
+
 def init(db):
     try:
         conn = sqlite3.connect(db)
         cursor = conn.cursor()
 
         table_users = """
             CREATE TABLE IF NOT EXISTS
@@ -116,15 +118,15 @@
                     reply_to_tweet_id integer,
                     CONSTRAINT replies_pk PRIMARY KEY (user_id, tweet_id),
                     CONSTRAINT tweet_id_fk FOREIGN KEY (tweet_id) REFERENCES tweets(id)
                 );
         """
         cursor.execute(table_reply_to)
 
-        table_favorites =  """
+        table_favorites = """
             CREATE TABLE IF NOT EXISTS
                 favorites(
                     user_id integer not null,
                     tweet_id integer not null,
                     CONSTRAINT favorites_pk PRIMARY KEY (user_id, tweet_id),
                     CONSTRAINT user_id_fk FOREIGN KEY (user_id) REFERENCES users(id),
                     CONSTRAINT tweet_id_fk FOREIGN KEY (tweet_id) REFERENCES tweets(id)
@@ -178,56 +180,87 @@
         """
         cursor.execute(table_following_names)
 
         return conn
     except Exception as e:
         return str(e)
 
+
 def fTable(Followers):
     if Followers:
         table = "followers_names"
     else:
         table = "following_names"
 
     return table
 
+
 def uTable(Followers):
     if Followers:
         table = "followers"
     else:
         table = "following"
 
     return table
 
+
 def follow(conn, Username, Followers, User):
     try:
-        time_ms = round(time.time()*1000)
+        time_ms = round(time.time() * 1000)
         cursor = conn.cursor()
-        entry = (User, time_ms, Username,)
+        entry = (
+            User,
+            time_ms,
+            Username,
+        )
         table = fTable(Followers)
         query = f"INSERT INTO {table} VALUES(?,?,?)"
         cursor.execute(query, entry)
         conn.commit()
     except sqlite3.IntegrityError:
         pass
 
+
 def get_hash_id(conn, id):
     cursor = conn.cursor()
-    cursor.execute('SELECT hex_dig FROM users WHERE id = ? LIMIT 1', (id,))
+    cursor.execute("SELECT hex_dig FROM users WHERE id = ? LIMIT 1", (id,))
     resultset = cursor.fetchall()
     return resultset[0][0] if resultset else -1
 
+
 def user(conn, config, User):
     try:
-        time_ms = round(time.time()*1000)
+        time_ms = round(time.time() * 1000)
         cursor = conn.cursor()
-        user = [int(User.id), User.id, User.name, User.username, User.bio, User.location, User.url,User.join_date, User.join_time, User.tweets, User.following, User.followers, User.likes, User.media_count, User.is_private, User.is_verified, User.avatar, User.background_image]
-
-        hex_dig = hashlib.sha256(','.join(str(v) for v in user).encode()).hexdigest()
-        entry = tuple(user) + (hex_dig,time_ms,)
+        user = [
+            int(User.id),
+            User.id,
+            User.name,
+            User.username,
+            User.bio,
+            User.location,
+            User.url,
+            User.join_date,
+            User.join_time,
+            User.tweets,
+            User.following,
+            User.followers,
+            User.likes,
+            User.media_count,
+            User.is_private,
+            User.is_verified,
+            User.avatar,
+            User.background_image,
+        ]
+
+        hex_dig = hashlib.sha256(",".join(str(v) for v in user).encode()).hexdigest()
+        entry = tuple(user) + (
+            hex_dig,
+            time_ms,
+        )
         old_hash = get_hash_id(conn, User.id)
 
         if old_hash == -1 or old_hash != hex_dig:
             query = f"INSERT INTO users VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)"
             cursor.execute(query, entry)
         else:
             pass
@@ -237,71 +270,88 @@
             query = f"INSERT INTO {table} VALUES(?,?)"
             cursor.execute(query, (config.User_id, int(User.id)))
 
         conn.commit()
     except sqlite3.IntegrityError:
         pass
 
+
 def tweets(conn, Tweet, config):
     try:
-        time_ms = round(time.time()*1000)
+        time_ms = round(time.time() * 1000)
         cursor = conn.cursor()
-        entry = (Tweet.id,
-                    Tweet.id_str,
-                    Tweet.tweet,
-                    Tweet.lang,
-                    Tweet.conversation_id,
-                    Tweet.datetime,
-                    Tweet.datestamp,
-                    Tweet.timestamp,
-                    Tweet.timezone,
-                    json.dumps(Tweet.place) if Tweet.place else None,
-                    Tweet.replies_count,
-                    Tweet.likes_count,
-                    Tweet.retweets_count,
-                    Tweet.user_id,
-                    Tweet.user_id_str,
-                    Tweet.username,
-                    Tweet.name,
-                    Tweet.link,
-                    json.dumps(Tweet.mentions) if Tweet.mentions else None,
-                    ",".join(Tweet.hashtags),
-                    ",".join(Tweet.cashtags),
-                    ",".join(Tweet.urls),
-                    ",".join(Tweet.photos),
-                    Tweet.thumbnail,
-                    Tweet.quote_url,
-                    Tweet.video,
-                    Tweet.geo,
-                    Tweet.near,
-                    Tweet.source,
-                    time_ms,
-                    Tweet.translate,
-                    Tweet.trans_src,
-                    Tweet.trans_dest)
-        cursor.execute('INSERT INTO tweets VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)', entry)
+        entry = (
+            Tweet.id,
+            Tweet.id_str,
+            Tweet.tweet,
+            Tweet.lang,
+            Tweet.conversation_id,
+            Tweet.datetime,
+            Tweet.datestamp,
+            Tweet.timestamp,
+            Tweet.timezone,
+            json.dumps(Tweet.place) if Tweet.place else None,
+            Tweet.replies_count,
+            Tweet.likes_count,
+            Tweet.retweets_count,
+            Tweet.user_id,
+            Tweet.user_id_str,
+            Tweet.username,
+            Tweet.name,
+            Tweet.link,
+            json.dumps(Tweet.mentions) if Tweet.mentions else None,
+            ",".join(Tweet.hashtags),
+            ",".join(Tweet.cashtags),
+            ",".join(Tweet.urls),
+            ",".join(Tweet.photos),
+            Tweet.thumbnail,
+            Tweet.quote_url,
+            Tweet.video,
+            Tweet.geo,
+            Tweet.near,
+            Tweet.source,
+            time_ms,
+            Tweet.translate,
+            Tweet.trans_src,
+            Tweet.trans_dest,
+        )
+        cursor.execute(
+            "INSERT INTO tweets VALUES(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)",
+            entry,
+        )
 
         if config.Favorites:
-            query = 'INSERT INTO favorites VALUES(?,?)'
+            query = "INSERT INTO favorites VALUES(?,?)"
             cursor.execute(query, (config.User_id, Tweet.id))
 
         if Tweet.retweet:
-            query = 'INSERT INTO retweets VALUES(?,?,?,?,?)'
-            _d = datetime.timestamp(datetime.strptime(Tweet.retweet_date, "%Y-%m-%d %H:%M:%S"))
-            cursor.execute(query, (int(Tweet.user_rt_id), Tweet.user_rt, Tweet.id, int(Tweet.retweet_id), _d))
+            query = "INSERT INTO retweets VALUES(?,?,?,?,?)"
+            _d = datetime.timestamp(
+                datetime.strptime(Tweet.retweet_date, "%Y-%m-%d %H:%M:%S")
+            )
+            cursor.execute(
+                query,
+                (
+                    int(Tweet.user_rt_id),
+                    Tweet.user_rt,
+                    Tweet.id,
+                    int(Tweet.retweet_id),
+                    _d,
+                ),
+            )
 
         if Tweet.reply_to:
             for reply in Tweet.reply_to:
-                query = 'INSERT INTO replies VALUES(?,?,?,?)'
+                query = "INSERT INTO replies VALUES(?,?,?,?)"
                 cursor.execute(
                     query,
                     (
                         Tweet.id,
-                        int(reply['id']),
-                        reply['screen_name'],
-                        reply['tweet_id'],
+                        int(reply["id"]),
+                        reply["screen_name"],
+                        reply["tweet_id"],
                     ),
                 )
 
         conn.commit()
     except sqlite3.IntegrityError:
         pass
```

### Comparing `twint_fork-2.2.0/twint/storage/elasticsearch.py` & `twint_fork-2.5.0/twint/storage/elasticsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,192 +11,208 @@
 _is_near_def = False
 _is_location_def = False
 _near = {}
 _location = {}
 
 geolocator = Nominatim(user_agent="twint-1.2")
 
+
 class RecycleObject(object):
-    def write(self, junk): pass
-    def flush(self): pass
+    def write(self, junk):
+        pass
+
+    def flush(self):
+        pass
+
 
 def getLocation(place, **options):
-    location = geolocator.geocode(place,timeout=1000)
+    location = geolocator.geocode(place, timeout=1000)
     if location:
         if options.get("near"):
             global _near
             _near = {"lat": location.latitude, "lon": location.longitude}
             return True
         elif options.get("location"):
             global _location
             _location = {"lat": location.latitude, "lon": location.longitude}
             return True
         return {"lat": location.latitude, "lon": location.longitude}
     else:
         return {}
 
+
 def handleIndexResponse(response):
     try:
         if response["status"] == 400:
             return True
     except KeyError:
         pass
     if response["acknowledged"]:
-        print("[+] Index \"" + response["index"] + "\" created!")
+        print('[+] Index "' + response["index"] + '" created!')
     else:
         print("[x] error index creation :: storage.elasticsearch.handleIndexCreation")
     if response["shards_acknowledged"]:
         print("[+] Shards acknowledged, everything is ready to be used!")
         return True
     else:
         print("[x] error with shards :: storage.elasticsearch.HandleIndexCreation")
         return False
 
+
 def createIndex(config, instance, **scope):
     if scope.get("scope") == "tweet":
         tweets_body = {
-                "mappings": {
-                    "properties": {
-                        "id": {"type": "long"},
-                        "conversation_id": {"type": "long"},
-                        "created_at": {"type": "text"},
-                        "date": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss"},
-                        "timezone": {"type": "keyword"},
-                        "place": {"type": "keyword"},
-                        "location": {"type": "keyword"},
-                        "tweet": {"type": "text"},
-                        "lang": {"type": "keyword"},
-                        "hashtags": {"type": "keyword", "normalizer": "hashtag_normalizer"},
-                        "cashtags": {"type": "keyword", "normalizer": "hashtag_normalizer"},
-                        "user_id_str": {"type": "keyword"},
-                        "username": {"type": "keyword", "normalizer": "hashtag_normalizer"},
-                        "name": {"type": "text"},
-                        "profile_image_url": {"type": "text"},
-                        "day": {"type": "integer"},
-                        "hour": {"type": "integer"},
-                        "link": {"type": "text"},
-                        "retweet": {"type": "text"},
-                        "essid": {"type": "keyword"},
-                        "nlikes": {"type": "integer"},
-                        "nreplies": {"type": "integer"},
-                        "nretweets": {"type": "integer"},
-                        "quote_url": {"type": "text"},
-                        "video": {"type":"integer"},
-                        "thumbnail": {"type":"text"},
-                        "search": {"type": "text"},
-                        "near": {"type": "text"},
-                        "geo_near": {"type": "geo_point"},
-                        "geo_tweet": {"type": "geo_point"},
-                        "photos": {"type": "text"},
-                        "user_rt_id": {"type": "keyword"},
-                        "mentions": {"type": "keyword", "normalizer": "hashtag_normalizer"},
-                        "source": {"type": "keyword"},
-                        "user_rt": {"type": "keyword"},
-                        "retweet_id": {"type": "keyword"},
-                        "reply_to": {
-                            "type": "nested",
-                            "properties": {
-                                "user_id": {"type": "keyword"},
-                                "username": {"type": "keyword"}
-                            }
+            "mappings": {
+                "properties": {
+                    "id": {"type": "long"},
+                    "conversation_id": {"type": "long"},
+                    "created_at": {"type": "text"},
+                    "date": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss"},
+                    "timezone": {"type": "keyword"},
+                    "place": {"type": "keyword"},
+                    "location": {"type": "keyword"},
+                    "tweet": {"type": "text"},
+                    "lang": {"type": "keyword"},
+                    "hashtags": {"type": "keyword", "normalizer": "hashtag_normalizer"},
+                    "cashtags": {"type": "keyword", "normalizer": "hashtag_normalizer"},
+                    "user_id_str": {"type": "keyword"},
+                    "username": {"type": "keyword", "normalizer": "hashtag_normalizer"},
+                    "name": {"type": "text"},
+                    "profile_image_url": {"type": "text"},
+                    "day": {"type": "integer"},
+                    "hour": {"type": "integer"},
+                    "link": {"type": "text"},
+                    "retweet": {"type": "text"},
+                    "essid": {"type": "keyword"},
+                    "nlikes": {"type": "integer"},
+                    "nreplies": {"type": "integer"},
+                    "nretweets": {"type": "integer"},
+                    "quote_url": {"type": "text"},
+                    "video": {"type": "integer"},
+                    "thumbnail": {"type": "text"},
+                    "search": {"type": "text"},
+                    "near": {"type": "text"},
+                    "geo_near": {"type": "geo_point"},
+                    "geo_tweet": {"type": "geo_point"},
+                    "photos": {"type": "text"},
+                    "user_rt_id": {"type": "keyword"},
+                    "mentions": {"type": "keyword", "normalizer": "hashtag_normalizer"},
+                    "source": {"type": "keyword"},
+                    "user_rt": {"type": "keyword"},
+                    "retweet_id": {"type": "keyword"},
+                    "reply_to": {
+                        "type": "nested",
+                        "properties": {
+                            "user_id": {"type": "keyword"},
+                            "username": {"type": "keyword"},
                         },
-                        "retweet_date": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss", "ignore_malformed": True},
-                        "urls": {"type": "keyword"},
-                        "translate": {"type": "text"},
-                        "trans_src": {"type": "keyword"},
-                        "trans_dest": {"type": "keyword"},
-                        }
                     },
-                    "settings": {
-                        "number_of_shards": 1,
-                        "analysis": {
-                            "normalizer": {
-                                "hashtag_normalizer": {
-                                    "type": "custom",
-                                    "char_filter": [],
-                                    "filter": ["lowercase", "asciifolding"]
-                                }
-                            }
+                    "retweet_date": {
+                        "type": "date",
+                        "format": "yyyy-MM-dd HH:mm:ss",
+                        "ignore_malformed": True,
+                    },
+                    "urls": {"type": "keyword"},
+                    "translate": {"type": "text"},
+                    "trans_src": {"type": "keyword"},
+                    "trans_dest": {"type": "keyword"},
+                }
+            },
+            "settings": {
+                "number_of_shards": 1,
+                "analysis": {
+                    "normalizer": {
+                        "hashtag_normalizer": {
+                            "type": "custom",
+                            "char_filter": [],
+                            "filter": ["lowercase", "asciifolding"],
                         }
                     }
-                }
+                },
+            },
+        }
         with nostdout():
-            resp = instance.indices.create(index=config.Index_tweets, body=tweets_body, ignore=400)
+            resp = instance.indices.create(
+                index=config.Index_tweets, body=tweets_body, ignore=400
+            )
         return handleIndexResponse(resp)
     elif scope.get("scope") == "follow":
         follow_body = {
-                "mappings": {
-                    "properties": {
-                        "user": {"type": "keyword"},
-                        "follow": {"type": "keyword"},
-                        "essid": {"type": "keyword"}
-                        }
-                    },
-                    "settings": {
-                        "number_of_shards": 1
-                    }
+            "mappings": {
+                "properties": {
+                    "user": {"type": "keyword"},
+                    "follow": {"type": "keyword"},
+                    "essid": {"type": "keyword"},
                 }
+            },
+            "settings": {"number_of_shards": 1},
+        }
         with nostdout():
-            resp = instance.indices.create(index=config.Index_follow, body=follow_body, ignore=400)
+            resp = instance.indices.create(
+                index=config.Index_follow, body=follow_body, ignore=400
+            )
         return handleIndexResponse(resp)
     elif scope.get("scope") == "user":
         user_body = {
-                "mappings": {
-                    "properties": {
-                        "id": {"type": "keyword"},
-                        "name": {"type": "keyword"},
-                        "username": {"type": "keyword"},
-                        "bio": {"type": "text"},
-                        "location": {"type": "keyword"},
-                        "url": {"type": "text"},
-                        "join_datetime": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss"},
-                        "tweets": {"type": "integer"},
-                        "following": {"type": "integer"},
-                        "followers": {"type": "integer"},
-                        "likes": {"type": "integer"},
-                        "media": {"type": "integer"},
-                        "private": {"type": "integer"},
-                        "verified": {"type": "integer"},
-                        "avatar": {"type": "text"},
-                        "background_image": {"type": "text"},
-                        "session": {"type": "keyword"},
-                        "geo_user": {"type": "geo_point"}
-                        }
-                    },
-                    "settings": {
-                        "number_of_shards": 1
-                    }
+            "mappings": {
+                "properties": {
+                    "id": {"type": "keyword"},
+                    "name": {"type": "keyword"},
+                    "username": {"type": "keyword"},
+                    "bio": {"type": "text"},
+                    "location": {"type": "keyword"},
+                    "url": {"type": "text"},
+                    "join_datetime": {"type": "date", "format": "yyyy-MM-dd HH:mm:ss"},
+                    "tweets": {"type": "integer"},
+                    "following": {"type": "integer"},
+                    "followers": {"type": "integer"},
+                    "likes": {"type": "integer"},
+                    "media": {"type": "integer"},
+                    "private": {"type": "integer"},
+                    "verified": {"type": "integer"},
+                    "avatar": {"type": "text"},
+                    "background_image": {"type": "text"},
+                    "session": {"type": "keyword"},
+                    "geo_user": {"type": "geo_point"},
                 }
+            },
+            "settings": {"number_of_shards": 1},
+        }
         with nostdout():
-            resp = instance.indices.create(index=config.Index_users, body=user_body, ignore=400)
+            resp = instance.indices.create(
+                index=config.Index_users, body=user_body, ignore=400
+            )
         return handleIndexResponse(resp)
     else:
         print("[x] error index pre-creation :: storage.elasticsearch.createIndex")
         return False
 
+
 @contextlib.contextmanager
 def nostdout():
     savestdout = sys.stdout
     sys.stdout = RecycleObject()
     yield
     sys.stdout = savestdout
 
+
 def weekday(day):
     weekdays = {
-            "Monday": 1,
-            "Tuesday": 2,
-            "Wednesday": 3,
-            "Thursday": 4,
-            "Friday": 5,
-            "Saturday": 6,
-            "Sunday": 7,
-            }
+        "Monday": 1,
+        "Tuesday": 2,
+        "Wednesday": 3,
+        "Thursday": 4,
+        "Friday": 5,
+        "Saturday": 6,
+        "Sunday": 7,
+    }
 
     return weekdays[day]
 
+
 def Tweet(Tweet, config):
     global _index_tweet_status
     global _is_near_def
     date_obj = datetime.strptime(Tweet.datetime, "%Y-%m-%d %H:%M:%S %Z")
 
     actions = []
 
@@ -204,44 +220,44 @@
         retweet = Tweet.retweet
     except AttributeError:
         retweet = None
 
     dt = f"{Tweet.datestamp} {Tweet.timestamp}"
 
     j_data = {
-            "_index": config.Index_tweets,
-            "_id": str(Tweet.id) + "_raw_" + config.Essid,
-            "_source": {
-                "id": str(Tweet.id),
-                "conversation_id": Tweet.conversation_id,
-                "created_at": Tweet.datetime,
-                "date": dt,
-                "timezone": Tweet.timezone,
-                "place": Tweet.place,
-                "tweet": Tweet.tweet,
-                "language": Tweet.lang,
-                "hashtags": Tweet.hashtags,
-                "cashtags": Tweet.cashtags,
-                "user_id_str": Tweet.user_id_str,
-                "username": Tweet.username,
-                "name": Tweet.name,
-                "day": date_obj.weekday(),
-                "hour": date_obj.hour,
-                "link": Tweet.link,
-                "retweet": retweet,
-                "essid": config.Essid,
-                "nlikes": int(Tweet.likes_count),
-                "nreplies": int(Tweet.replies_count),
-                "nretweets": int(Tweet.retweets_count),
-                "quote_url": Tweet.quote_url,
-                "video": Tweet.video,
-                "search": str(config.Search),
-                "near": config.Near
-                }
-            }
+        "_index": config.Index_tweets,
+        "_id": str(Tweet.id) + "_raw_" + config.Essid,
+        "_source": {
+            "id": str(Tweet.id),
+            "conversation_id": Tweet.conversation_id,
+            "created_at": Tweet.datetime,
+            "date": dt,
+            "timezone": Tweet.timezone,
+            "place": Tweet.place,
+            "tweet": Tweet.tweet,
+            "language": Tweet.lang,
+            "hashtags": Tweet.hashtags,
+            "cashtags": Tweet.cashtags,
+            "user_id_str": Tweet.user_id_str,
+            "username": Tweet.username,
+            "name": Tweet.name,
+            "day": date_obj.weekday(),
+            "hour": date_obj.hour,
+            "link": Tweet.link,
+            "retweet": retweet,
+            "essid": config.Essid,
+            "nlikes": int(Tweet.likes_count),
+            "nreplies": int(Tweet.replies_count),
+            "nretweets": int(Tweet.retweets_count),
+            "quote_url": Tweet.quote_url,
+            "video": Tweet.video,
+            "search": str(config.Search),
+            "near": config.Near,
+        },
+    }
     if retweet is not None:
         j_data["_source"].update({"user_rt_id": Tweet.user_rt_id})
         j_data["_source"].update({"user_rt": Tweet.user_rt})
         j_data["_source"].update({"retweet_id": Tweet.retweet_id})
         j_data["_source"].update({"retweet_date": Tweet.retweet_date})
     if Tweet.reply_to:
         j_data["_source"].update({"reply_to": Tweet.reply_to})
@@ -276,83 +292,87 @@
     if Tweet.place:
         _t_place = getLocation(Tweet.place)
         if _t_place:
             j_data["_source"].update({"geo_tweet": getLocation(Tweet.place)})
     if Tweet.source:
         j_data["_source"].update({"source": Tweet.Source})
     if config.Translate:
-        j_data["_source"].update({"translate": Tweet.translate})        
+        j_data["_source"].update({"translate": Tweet.translate})
         j_data["_source"].update({"trans_src": Tweet.trans_src})
         j_data["_source"].update({"trans_dest": Tweet.trans_dest})
 
     actions.append(j_data)
 
     es = Elasticsearch(config.Elasticsearch, verify_certs=config.Skip_certs)
     if not _index_tweet_status:
         _index_tweet_status = createIndex(config, es, scope="tweet")
     with nostdout():
         helpers.bulk(es, actions, chunk_size=2000, request_timeout=200)
     actions = []
 
+
 def Follow(user, config):
     global _index_follow_status
     actions = []
 
     if config.Following:
         _user = config.Username
         _follow = user
     else:
         _user = user
         _follow = config.Username
     j_data = {
-            "_index": config.Index_follow,
-            "_id": _user + "_" + _follow + "_" + config.Essid,
-            "_source": {
-                "user": _user,
-                "follow": _follow,
-                "essid": config.Essid
-                }
-            }
+        "_index": config.Index_follow,
+        "_id": _user + "_" + _follow + "_" + config.Essid,
+        "_source": {"user": _user, "follow": _follow, "essid": config.Essid},
+    }
     actions.append(j_data)
 
     es = Elasticsearch(config.Elasticsearch, verify_certs=config.Skip_certs)
     if not _index_follow_status:
         _index_follow_status = createIndex(config, es, scope="follow")
     with nostdout():
         helpers.bulk(es, actions, chunk_size=2000, request_timeout=200)
     actions = []
 
+
 def UserProfile(user, config):
     global _index_user_status
     global _is_location_def
     actions = []
 
     j_data = {
-            "_index": config.Index_users,
-            "_id": user.id + "_" + user.join_date + "_" + user.join_time + "_" + config.Essid,
-            "_source": {
-                "id": user.id,
-                "name": user.name,
-                "username": user.username,
-                "bio": user.bio,
-                "location": user.location,
-                "url": user.url,
-                "join_datetime": user.join_date + " " + user.join_time,
-                "tweets": user.tweets,
-                "following": user.following,
-                "followers": user.followers,
-                "likes": user.likes,
-                "media": user.media_count,
-                "private": user.is_private,
-                "verified": user.is_verified,
-                "avatar": user.avatar,
-                "background_image": user.background_image,
-                "session": config.Essid
-                }
-            }
+        "_index": config.Index_users,
+        "_id": user.id
+        + "_"
+        + user.join_date
+        + "_"
+        + user.join_time
+        + "_"
+        + config.Essid,
+        "_source": {
+            "id": user.id,
+            "name": user.name,
+            "username": user.username,
+            "bio": user.bio,
+            "location": user.location,
+            "url": user.url,
+            "join_datetime": user.join_date + " " + user.join_time,
+            "tweets": user.tweets,
+            "following": user.following,
+            "followers": user.followers,
+            "likes": user.likes,
+            "media": user.media_count,
+            "private": user.is_private,
+            "verified": user.is_verified,
+            "avatar": user.avatar,
+            "background_image": user.background_image,
+            "session": config.Essid,
+        },
+    }
     if config.Location:
         if not _is_location_def:
             _is_location_def = getLocation(user.location, location=True)
         if _location:
             j_data["_source"].update({"geo_user": _location})
     actions.append(j_data)
```

### Comparing `twint_fork-2.2.0/twint/storage/panda.py` & `twint_fork-2.5.0/twint/storage/panda.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 from time import strftime, localtime
 from twint.tweet import Tweet_formats
 
 Tweets_df = None
 Follow_df = None
 User_df = None
 
-_object_blocks = {
-    "tweet": [],
-    "user": [],
-    "following": [],
-    "followers": []
-}
+_object_blocks = {"tweet": [], "user": [], "following": [], "followers": []}
 
 weekdays = {
-        "Monday": 1,
-        "Tuesday": 2,
-        "Wednesday": 3,
-        "Thursday": 4,
-        "Friday": 5,
-        "Saturday": 6,
-        "Sunday": 7,
-        }
+    "Monday": 1,
+    "Tuesday": 2,
+    "Wednesday": 3,
+    "Thursday": 4,
+    "Friday": 5,
+    "Saturday": 6,
+    "Sunday": 7,
+}
 
 _type = ""
 
+
 def _concat(df, _type):
     if df is None:
         df = pd.DataFrame(_object_blocks[_type])
     else:
         _df = pd.DataFrame(_object_blocks[_type])
         df = pd.concat([df, _df], sort=True)
     return df
 
+
 def _autoget(_type):
     global Tweets_df
     global Follow_df
     global User_df
 
     if _type == "tweet":
         Tweets_df = _concat(Tweets_df, _type)
@@ -47,30 +44,35 @@
     else:
         error("[x] Wrong type of object passed")
 
 
 def update(object, config):
     global _type
 
-    #try:
+    # try:
     #    _type = ((object.__class__.__name__ == "tweet")*"tweet" +
     #             (object.__class__.__name__ == "user")*"user")
-    #except AttributeError:
+    # except AttributeError:
     #    _type = config.Following*"following" + config.Followers*"followers"
     if object.__class__.__name__ == "tweet":
         _type = "tweet"
     elif object.__class__.__name__ == "user":
         _type = "user"
     elif object.__class__.__name__ == "dict":
-        _type = config.Following*"following" + config.Followers*"followers"
+        _type = config.Following * "following" + config.Followers * "followers"
 
     if _type == "tweet":
         Tweet = object
-        datetime_ms = datetime.datetime.strptime(Tweet.datetime, Tweet_formats['datetime']).timestamp() * 1000
-        day = weekdays[strftime("%A", localtime(datetime_ms/1000))]
+        datetime_ms = (
+            datetime.datetime.strptime(
+                Tweet.datetime, Tweet_formats["datetime"]
+            ).timestamp()
+            * 1000
+        )
+        day = weekdays[strftime("%A", localtime(datetime_ms / 1000))]
         dt = f"{object.datestamp} {object.timestamp}"
         _data = {
             "id": str(Tweet.id),
             "conversation_id": Tweet.conversation_id,
             "created_at": datetime_ms,
             "date": dt,
             "timezone": Tweet.timezone,
@@ -80,15 +82,15 @@
             "hashtags": Tweet.hashtags,
             "cashtags": Tweet.cashtags,
             "user_id": Tweet.user_id,
             "user_id_str": Tweet.user_id_str,
             "username": Tweet.username,
             "name": Tweet.name,
             "day": day,
-            "hour": strftime("%H", localtime(datetime_ms/1000)),
+            "hour": strftime("%H", localtime(datetime_ms / 1000)),
             "link": Tweet.link,
             "urls": Tweet.urls,
             "photos": Tweet.photos,
             "video": Tweet.video,
             "thumbnail": Tweet.thumbnail,
             "retweet": Tweet.retweet,
             "nlikes": int(Tweet.likes_count),
@@ -102,16 +104,16 @@
             "user_rt_id": Tweet.user_rt_id,
             "user_rt": Tweet.user_rt,
             "retweet_id": Tweet.retweet_id,
             "reply_to": Tweet.reply_to,
             "retweet_date": Tweet.retweet_date,
             "translate": Tweet.translate,
             "trans_src": Tweet.trans_src,
-            "trans_dest": Tweet.trans_dest
-            }
+            "trans_dest": Tweet.trans_dest,
+        }
         _object_blocks[_type].append(_data)
     elif _type == "user":
         user = object
         try:
             background_image = user.background_image
         except:
             background_image = ""
@@ -130,20 +132,20 @@
             "followers": user.followers,
             "likes": user.likes,
             "media": user.media_count,
             "private": user.is_private,
             "verified": user.is_verified,
             "avatar": user.avatar,
             "background_image": background_image,
-            }
+        }
         _object_blocks[_type].append(_data)
     elif _type == "followers" or _type == "following":
         _data = {
-            config.Following*"following" + config.Followers*"followers" :
-                             {config.Username: object[_type]}
+            config.Following * "following"
+            + config.Followers * "followers": {config.Username: object[_type]}
         }
         _object_blocks[_type] = _data
     else:
         print("Wrong type of object passed!")
 
 
 def clean():
@@ -154,14 +156,15 @@
     _object_blocks["following"].clear()
     _object_blocks["followers"].clear()
     _object_blocks["user"].clear()
     Tweets_df = None
     Follow_df = None
     User_df = None
 
+
 def save(_filename, _dataframe, **options):
     if options.get("dataname"):
         _dataname = options.get("dataname")
     else:
         _dataname = "twint"
 
     if not options.get("type"):
@@ -171,16 +174,19 @@
             _store[_dataname] = _dataframe
             _store.close()
     elif options.get("type") == "Pickle":
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             _dataframe.to_pickle(_filename + ".pkl")
     else:
-        print("""Please specify: filename, DataFrame, DataFrame name and type
-              (HDF5, default, or Pickle)""")
+        print(
+            """Please specify: filename, DataFrame, DataFrame name and type
+              (HDF5, default, or Pickle)"""
+        )
+
 
 def read(_filename, **options):
     if not options.get("dataname"):
         _dataname = "twint"
     else:
         _dataname = options.get("dataname")
 
@@ -188,9 +194,11 @@
         _store = pd.HDFStore(_filename + ".h5")
         _df = _store[_dataname]
         return _df
     elif options.get("type") == "Pickle":
         _df = pd.read_pickle(_filename + ".pkl")
         return _df
     else:
-        print("""Please specify: DataFrame, DataFrame name (twint as default),
-              filename and type (HDF5, default, or Pickle""")
+        print(
+            """Please specify: DataFrame, DataFrame name (twint as default),
+              filename and type (HDF5, default, or Pickle"""
+        )
```

### Comparing `twint_fork-2.2.0/twint/storage/write.py` & `twint_fork-2.5.0/twint/storage/write.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,85 @@
 from . import write_meta as meta
 import csv
 import json
 import os
 
+
 def outputExt(objType, fType):
     if objType == "str":
         objType = "username"
     outExt = f"/{objType}s.{fType}"
 
     return outExt
 
+
 def addExt(base, objType, fType):
-    if len(base.split('.')) == 1:
+    if len(base.split(".")) == 1:
         createDirIfMissing(base)
         base += outputExt(objType, fType)
 
     return base
 
+
 def Text(entry, f):
-    print(entry.replace('\n', ' '), file=open(f, "a", encoding="utf-8"))
+    print(entry.replace("\n", " "), file=open(f, "a", encoding="utf-8"))
+
 
 def Type(config):
     if config.User_full:
         _type = "user"
     elif config.Followers or config.Following:
         _type = "username"
     else:
         _type = "tweet"
 
     return _type
 
+
 def struct(obj, custom, _type):
     if custom:
         fieldnames = custom
         row = {}
         for f in fieldnames:
             row[f] = meta.Data(obj, _type)[f]
     else:
         fieldnames = meta.Fieldnames(_type)
         row = meta.Data(obj, _type)
 
     return fieldnames, row
 
+
 def createDirIfMissing(dirname):
     if not os.path.exists(dirname):
         os.makedirs(dirname)
 
+
 def Csv(obj, config):
     _obj_type = obj.__class__.__name__
     if _obj_type == "str":
         _obj_type = "username"
     fieldnames, row = struct(obj, config.Custom[_obj_type], _obj_type)
-    
+
     base = addExt(config.Output, _obj_type, "csv")
-    dialect = 'excel-tab' if 'Tabs' in config.__dict__ else 'excel'
-    
+    dialect = "excel-tab" if "Tabs" in config.__dict__ else "excel"
+
     if not (os.path.exists(base)):
-        with open(base, "w", newline='', encoding="utf-8") as csv_file:
+        with open(base, "w", newline="", encoding="utf-8") as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=fieldnames, dialect=dialect)
             writer.writeheader()
 
-    with open(base, "a", newline='', encoding="utf-8") as csv_file:
+    with open(base, "a", newline="", encoding="utf-8") as csv_file:
         writer = csv.DictWriter(csv_file, fieldnames=fieldnames, dialect=dialect)
         writer.writerow(row)
 
+
 def Json(obj, config):
     _obj_type = obj.__class__.__name__
     if _obj_type == "str":
         _obj_type = "username"
     null, data = struct(obj, config.Custom[_obj_type], _obj_type)
 
     base = addExt(config.Output, _obj_type, "json")
 
-    with open(base, "a", newline='', encoding="utf-8") as json_file:
+    with open(base, "a", newline="", encoding="utf-8") as json_file:
         json.dump(data, json_file, ensure_ascii=False)
         json_file.write("\n")
```

### Comparing `twint_fork-2.2.0/twint/storage/write_meta.py` & `twint_fork-2.5.0/twint/storage/write_meta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,149 +1,156 @@
 def tweetData(t):
     data = {
-            "id": int(t.id),
-            "conversation_id": t.conversation_id,
-            "created_at": t.datetime,
-            "date": t.datestamp,
-            "time": t.timestamp,
-            "timezone": t.timezone,
-            "user_id": t.user_id,
-            "username": t.username,
-            "name": t.name,
-            "place": t.place,
-            "tweet": t.tweet,
-            "language": t.lang,
-            "mentions": t.mentions,
-            "urls": t.urls,
-            "photos": t.photos,
-            "replies_count": int(t.replies_count),
-            "retweets_count": int(t.retweets_count),
-            "likes_count": int(t.likes_count),
-            "hashtags": t.hashtags,
-            "cashtags": t.cashtags,
-            "link": t.link,
-            "retweet": t.retweet,
-            "quote_url": t.quote_url,
-            "video": t.video,
-            "thumbnail": t.thumbnail,
-            "near": t.near,
-            "geo": t.geo,
-            "source": t.source,
-            "user_rt_id": t.user_rt_id,
-            "user_rt": t.user_rt,
-            "retweet_id": t.retweet_id,
-            "reply_to": t.reply_to,
-            "retweet_date": t.retweet_date,
-            "translate": t.translate,
-            "trans_src": t.trans_src,
-            "trans_dest": t.trans_dest,
-            }
+        "id": int(t.id),
+        "conversation_id": t.conversation_id,
+        "created_at": t.datetime,
+        "date": t.datestamp,
+        "time": t.timestamp,
+        "timezone": t.timezone,
+        "user_id": t.user_id,
+        "username": t.username,
+        "name": t.name,
+        "place": t.place,
+        "tweet": t.tweet,
+        "language": t.lang,
+        "mentions": t.mentions,
+        "urls": t.urls,
+        "photos": t.photos,
+        "replies_count": int(t.replies_count),
+        "retweets_count": int(t.retweets_count),
+        "likes_count": int(t.likes_count),
+        "hashtags": t.hashtags,
+        "cashtags": t.cashtags,
+        "link": t.link,
+        "retweet": t.retweet,
+        "quote_url": t.quote_url,
+        "video": t.video,
+        "thumbnail": t.thumbnail,
+        "near": t.near,
+        "geo": t.geo,
+        "source": t.source,
+        "user_rt_id": t.user_rt_id,
+        "user_rt": t.user_rt,
+        "retweet_id": t.retweet_id,
+        "reply_to": t.reply_to,
+        "retweet_date": t.retweet_date,
+        "translate": t.translate,
+        "trans_src": t.trans_src,
+        "trans_dest": t.trans_dest,
+    }
     return data
 
+
 def tweetFieldnames():
     fieldnames = [
-            "id",
-            "conversation_id",
-            "created_at",
-            "date",
-            "time",
-            "timezone",
-            "user_id",
-            "username",
-            "name",
-            "place",
-            "tweet",
-            "language",
-            "mentions",
-            "urls",
-            "photos",
-            "replies_count",
-            "retweets_count",
-            "likes_count",
-            "hashtags",
-            "cashtags",
-            "link",
-            "retweet",
-            "quote_url",
-            "video",
-            "thumbnail",
-            "near",
-            "geo",
-            "source",
-            "user_rt_id",
-            "user_rt",
-            "retweet_id",
-            "reply_to",
-            "retweet_date",
-            "translate",
-            "trans_src",
-            "trans_dest"
-            ]
+        "id",
+        "conversation_id",
+        "created_at",
+        "date",
+        "time",
+        "timezone",
+        "user_id",
+        "username",
+        "name",
+        "place",
+        "tweet",
+        "language",
+        "mentions",
+        "urls",
+        "photos",
+        "replies_count",
+        "retweets_count",
+        "likes_count",
+        "hashtags",
+        "cashtags",
+        "link",
+        "retweet",
+        "quote_url",
+        "video",
+        "thumbnail",
+        "near",
+        "geo",
+        "source",
+        "user_rt_id",
+        "user_rt",
+        "retweet_id",
+        "reply_to",
+        "retweet_date",
+        "translate",
+        "trans_src",
+        "trans_dest",
+    ]
     return fieldnames
 
+
 def userData(u):
     data = {
-            "id": int(u.id),
-            "name": u.name,
-            "username": u.username,
-            "bio": u.bio,
-            "location": u.location,
-            "url": u.url,
-            "join_date": u.join_date,
-            "join_time": u.join_time,
-            "tweets": int(u.tweets),
-            "following": int(u.following),
-            "followers": int(u.followers),
-            "likes": int(u.likes),
-            "media": int(u.media_count),
-            "private": u.is_private,
-            "verified": u.is_verified,
-            "profile_image_url": u.avatar,
-            "background_image": u.background_image
-            }
+        "id": int(u.id),
+        "name": u.name,
+        "username": u.username,
+        "bio": u.bio,
+        "location": u.location,
+        "url": u.url,
+        "join_date": u.join_date,
+        "join_time": u.join_time,
+        "tweets": int(u.tweets),
+        "following": int(u.following),
+        "followers": int(u.followers),
+        "likes": int(u.likes),
+        "media": int(u.media_count),
+        "private": u.is_private,
+        "verified": u.is_verified,
+        "profile_image_url": u.avatar,
+        "background_image": u.background_image,
+    }
     return data
 
+
 def userFieldnames():
     fieldnames = [
-            "id",
-            "name",
-            "username",
-            "bio",
-            "location",
-            "url",
-            "join_date",
-            "join_time",
-            "tweets",
-            "following",
-            "followers",
-            "likes",
-            "media",
-            "private",
-            "verified",
-            "profile_image_url",
-            "background_image"
-            ]
+        "id",
+        "name",
+        "username",
+        "bio",
+        "location",
+        "url",
+        "join_date",
+        "join_time",
+        "tweets",
+        "following",
+        "followers",
+        "likes",
+        "media",
+        "private",
+        "verified",
+        "profile_image_url",
+        "background_image",
+    ]
     return fieldnames
 
+
 def usernameData(u):
     return {"username": u}
 
+
 def usernameFieldnames():
     return ["username"]
 
+
 def Data(obj, _type):
     if _type == "user":
         ret = userData(obj)
     elif _type == "username":
         ret = usernameData(obj)
     else:
         ret = tweetData(obj)
 
     return ret
 
+
 def Fieldnames(_type):
     if _type == "user":
         ret = userFieldnames()
     elif _type == "username":
         ret = usernameFieldnames()
     else:
         ret = tweetFieldnames()
```

### Comparing `twint_fork-2.2.0/twint/token.py` & `twint_fork-2.5.0/twint/token.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,82 +14,89 @@
     def __init__(self, msg):
         super().__init__(msg)
 
 
 class Token:
     def __init__(self, config):
         self._session = requests.Session()
-        self._session.headers.update({'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0'})
+        self._session.headers.update(
+            {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0"
+            }
+        )
         self.config = config
         self._retries = 5
         self._timeout = 10
-        self.url = 'https://twitter.com'
+        self.url = "https://twitter.com"
 
     def _request(self):
         for attempt in range(self._retries + 1):
             # The request is newly prepared on each retry because of potential cookie updates.
-            req = self._session.prepare_request(requests.Request('GET', self.url))
-            logme.debug(f'Retrieving {req.url}')
+            req = self._session.prepare_request(requests.Request("GET", self.url))
+            logme.debug(f"Retrieving {req.url}")
             try:
                 r = self._session.send(req, allow_redirects=True, timeout=self._timeout)
             except requests.exceptions.RequestException as exc:
                 if attempt < self._retries:
-                    retrying = ', retrying'
+                    retrying = ", retrying"
                     level = logme.WARNING
                 else:
-                    retrying = ''
+                    retrying = ""
                     level = logme.ERROR
-                logme.log(level, f'Error retrieving {req.url}: {exc!r}{retrying}')
+                logme.log(level, f"Error retrieving {req.url}: {exc!r}{retrying}")
             else:
                 success, msg = (True, None)
-                msg = f': {msg}' if msg else ''
+                msg = f": {msg}" if msg else ""
 
                 if success:
-                    logme.debug(f'{req.url} retrieved successfully{msg}')
+                    logme.debug(f"{req.url} retrieved successfully{msg}")
                     return r
             if attempt < self._retries:
                 # TODO : might wanna tweak this back-off timer
-                sleep_time = 2.0 * 2 ** attempt
-                logme.info(f'Waiting {sleep_time:.0f} seconds')
+                sleep_time = 2.0 * 2**attempt
+                logme.info(f"Waiting {sleep_time:.0f} seconds")
                 time.sleep(sleep_time)
         else:
-            msg = f'{self._retries + 1} requests to {self.url} failed, giving up.'
+            msg = f"{self._retries + 1} requests to {self.url} failed, giving up."
             logme.fatal(msg)
             self.config.Guest_token = None
             raise RefreshTokenException(msg)
 
     def refresh(self):
-        logme.debug('Retrieving guest token')
+        logme.debug("Retrieving guest token")
         res = self._request()
         match = re.search(r'\("gt=(\d+);', res.text)
         if match:
-            logme.debug('Found guest token in HTML')
+            logme.debug("Found guest token in HTML")
             self.config.Guest_token = str(match.group(1))
         else:
             headers = {
-                'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0',
-                'authority': 'api.twitter.com',
-                'content-length': '0',
-                'authorization': self.config.Bearer_token,
-                'x-twitter-client-language': 'en',
-                'x-csrf-token': res.cookies.get("ct0"),
-                'x-twitter-active-user': 'yes',
-                'content-type': 'application/x-www-form-urlencoded',
-                'accept': '*/*',
-                'sec-gpc': '1',
-                'origin': 'https://twitter.com',
-                'sec-fetch-site': 'same-site',
-                'sec-fetch-mode': 'cors',
-                'sec-fetch-dest': 'empty',
-                'referer': 'https://twitter.com/',
-                'accept-language': 'en-US',
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:78.0) Gecko/20100101 Firefox/78.0",
+                "authority": "api.twitter.com",
+                "content-length": "0",
+                "authorization": self.config.Bearer_token,
+                "x-twitter-client-language": "en",
+                "x-csrf-token": res.cookies.get("ct0"),
+                "x-twitter-active-user": "yes",
+                "content-type": "application/x-www-form-urlencoded",
+                "accept": "*/*",
+                "sec-gpc": "1",
+                "origin": "https://twitter.com",
+                "sec-fetch-site": "same-site",
+                "sec-fetch-mode": "cors",
+                "sec-fetch-dest": "empty",
+                "referer": "https://twitter.com/",
+                "accept-language": "en-US",
             }
             self._session.headers.update(headers)
-            req = self._session.prepare_request(requests.Request('POST', 'https://api.twitter.com/1.1/guest/activate.json'))
+            req = self._session.prepare_request(
+                requests.Request(
+                    "POST", "https://api.twitter.com/1.1/guest/activate.json"
+                )
+            )
             res = self._session.send(req, allow_redirects=True, timeout=self._timeout)
             match = re.search(r'{"guest_token":"(\d+)"}', res.text)
             if match:
                 self.config.Guest_token = str(match.group(1))
             else:
                 self.config.Guest_token = None
-                raise RefreshTokenException('Could not find the Guest token in')
-
+                raise RefreshTokenException("Could not find the Guest token in")
```

### Comparing `twint_fork-2.2.0/twint/tweet.py` & `twint_fork-2.5.0/twint/tweet.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,171 +1,181 @@
 from time import strftime, localtime
 from datetime import datetime, timezone
 
 import logging as logme
 from googletransx import Translator
-# ref. 
+
+# ref.
 # - https://github.com/x0rzkov/py-googletrans#basic-usage
 translator = Translator()
 
 
 class tweet:
-    """Define Tweet class
-    """
+    """Define Tweet class"""
+
     type = "tweet"
 
     def __init__(self):
         pass
 
 
 def utc_to_local(utc_dt):
     return utc_dt.replace(tzinfo=timezone.utc).astimezone(tz=None)
 
 
 Tweet_formats = {
-    'datetime': '%Y-%m-%d %H:%M:%S %Z',
-    'datestamp': '%Y-%m-%d',
-    'timestamp': '%H:%M:%S'
+    "datetime": "%Y-%m-%d %H:%M:%S %Z",
+    "datestamp": "%Y-%m-%d",
+    "timestamp": "%H:%M:%S",
 }
 
 
 def _get_mentions(tw):
-    """Extract mentions from tweet
-    """
-    logme.debug(__name__ + ':get_mentions')
+    """Extract mentions from tweet"""
+    logme.debug(__name__ + ":get_mentions")
     try:
         mentions = [
             {
-                'screen_name': _mention['screen_name'],
-                'name': _mention['name'],
-                'id': _mention['id_str'],
-            } for _mention in tw['entities']['user_mentions']
-            if tw['display_text_range'][0] < _mention['indices'][0]
+                "screen_name": _mention["screen_name"],
+                "name": _mention["name"],
+                "id": _mention["id_str"],
+            }
+            for _mention in tw["entities"]["user_mentions"]
+            if tw["display_text_range"][0] < _mention["indices"][0]
         ]
     except KeyError:
         mentions = []
     return mentions
 
 
 def _get_reply_to(tw):
     try:
         reply_to = [
             {
-                'screen_name': _mention['screen_name'],
-                'name': _mention['name'],
-                'id': _mention['id_str'],
-                'tweet_id': (
-                    tw.get('in_reply_to_status_id')
-                    if _mention['id'] == tw.get('in_reply_to_user_id')
+                "screen_name": _mention["screen_name"],
+                "name": _mention["name"],
+                "id": _mention["id_str"],
+                "tweet_id": (
+                    tw.get("in_reply_to_status_id")
+                    if _mention["id"] == tw.get("in_reply_to_user_id")
                     else None
                 ),
-            } for _mention in tw['entities']['user_mentions']
-            if tw['display_text_range'][0] > _mention['indices'][1]
+            }
+            for _mention in tw["entities"]["user_mentions"]
+            if tw["display_text_range"][0] > _mention["indices"][1]
         ]
     except KeyError:
         reply_to = []
     return reply_to
 
 
 def getText(tw):
-    """Replace some text
-    """
-    logme.debug(__name__ + ':getText')
-    text = tw['full_text']
+    """Replace some text"""
+    logme.debug(__name__ + ":getText")
+    text = tw["full_text"]
     text = text.replace("http", " http")
     text = text.replace("pic.twitter", " pic.twitter")
     text = text.replace("\n", " ")
 
     return text
 
 
 def Tweet(tw, config):
-    """Create Tweet object
-    """
-    logme.debug(__name__ + ':Tweet')
+    """Create Tweet object"""
+    logme.debug(__name__ + ":Tweet")
     t = tweet()
-    t.id = int(tw['id_str'])
+    t.id = int(tw["id_str"])
     t.id_str = tw["id_str"]
     t.conversation_id = tw["conversation_id_str"]
+    user = tw["user"]
 
     # parsing date to user-friendly format
-    _dt = tw['created_at']
-    _dt = datetime.strptime(_dt, '%a %b %d %H:%M:%S %z %Y')
+    _dt = tw["created_at"]
+    _dt = datetime.strptime(_dt, "%a %b %d %H:%M:%S %z %Y")
     _dt = utc_to_local(_dt)
-    t.datetime = str(_dt.strftime(Tweet_formats['datetime']))
+    t.datetime = str(_dt.strftime(Tweet_formats["datetime"]))
     # date is of the format year,
-    t.datestamp = _dt.strftime(Tweet_formats['datestamp'])
-    t.timestamp = _dt.strftime(Tweet_formats['timestamp'])
-    t.user_id = int(tw["user_id_str"])
-    t.user_id_str = tw["user_id_str"]
-    t.username = tw["user_data"]['screen_name']
-    t.name = tw["user_data"]['name']
-    t.place = tw['geo'] if 'geo' in tw and tw['geo'] else ""
+    t.datestamp = _dt.strftime(Tweet_formats["datestamp"])
+    t.timestamp = _dt.strftime(Tweet_formats["timestamp"])
+    t.user_id = int(user["id"])
+    t.user_id_str = user["id_str"]
+    t.username = user["screen_name"]
+    t.name = user["name"]
+    t.place = tw["geo"] if "geo" in tw and tw["geo"] else ""
     t.timezone = strftime("%z", localtime())
     t.mentions = _get_mentions(tw)
     t.reply_to = _get_reply_to(tw)
     try:
-        t.urls = [_url['expanded_url'] for _url in tw['entities']['urls']]
+        t.urls = [_url["expanded_url"] for _url in tw["entities"]["urls"]]
     except KeyError:
         t.urls = []
     try:
-        t.photos = [_img['media_url_https'] for _img in tw['entities']['media'] if _img['type'] == 'photo' and
-                    _img['expanded_url'].find('/photo/') != -1]
+        t.photos = [
+            _img["media_url_https"]
+            for _img in tw["entities"]["media"]
+            if _img["type"] == "photo" and _img["expanded_url"].find("/photo/") != -1
+        ]
     except KeyError:
         t.photos = []
     try:
-        t.video = 1 if len(tw['extended_entities']['media']) else 0
+        t.video = 1 if len(tw["extended_entities"]["media"]) else 0
     except KeyError:
         t.video = 0
     try:
-        t.thumbnail = tw['extended_entities']['media'][0]['media_url_https']
+        t.thumbnail = tw["extended_entities"]["media"][0]["media_url_https"]
     except KeyError:
-        t.thumbnail = ''
+        t.thumbnail = ""
     t.tweet = getText(tw)
-    t.lang = tw['lang']
+    t.lang = tw["lang"]
     try:
-        t.hashtags = [hashtag['text'] for hashtag in tw['entities']['hashtags']]
+        t.hashtags = [hashtag["text"] for hashtag in tw["entities"]["hashtags"]]
     except KeyError:
         t.hashtags = []
     try:
-        t.cashtags = [cashtag['text'] for cashtag in tw['entities']['symbols']]
+        t.cashtags = [cashtag["text"] for cashtag in tw["entities"]["symbols"]]
     except KeyError:
         t.cashtags = []
-    t.replies_count = tw['reply_count']
-    t.retweets_count = tw['retweet_count']
-    t.likes_count = tw['favorite_count']
+    t.replies_count = tw["reply_count"]
+    t.retweets_count = tw["retweet_count"]
+    t.likes_count = tw["favorite_count"]
     t.link = f"https://twitter.com/{t.username}/status/{t.id}"
     try:
-        if 'user_rt_id' in tw['retweet_data']:
+        if "user_rt_id" in tw["retweet_data"]:
             t.retweet = True
-            t.retweet_id = tw['retweet_data']['retweet_id']
-            t.retweet_date = tw['retweet_data']['retweet_date']
-            t.user_rt = tw['retweet_data']['user_rt']
-            t.user_rt_id = tw['retweet_data']['user_rt_id']
+            t.retweet_id = tw["retweet_data"]["retweet_id"]
+            t.retweet_date = tw["retweet_data"]["retweet_date"]
+            t.user_rt = tw["retweet_data"]["user_rt"]
+            t.user_rt_id = tw["retweet_data"]["user_rt_id"]
     except KeyError:
         t.retweet = False
-        t.retweet_id = ''
-        t.retweet_date = ''
-        t.user_rt = ''
-        t.user_rt_id = ''
-    try:
-        t.quote_url = tw['quoted_status_permalink']['expanded'] if tw['is_quote_status'] else ''
+        t.retweet_id = ""
+        t.retweet_date = ""
+        t.user_rt = ""
+        t.user_rt_id = ""
+    try:
+        t.quote_url = (
+            tw["quoted_status_permalink"]["expanded"] if tw["is_quote_status"] else ""
+        )
     except KeyError:
         # means that the quoted tweet have been deleted
         t.quote_url = 0
     t.near = config.Near if config.Near else ""
     t.geo = config.Geo if config.Geo else ""
     t.source = config.Source if config.Source else ""
-    t.translate = ''
-    t.trans_src = ''
-    t.trans_dest = ''
+    t.translate = ""
+    t.trans_src = ""
+    t.trans_dest = ""
     if config.Translate:
         try:
             ts = translator.translate(text=t.tweet, dest=config.TranslateDest)
             t.translate = ts.text
             t.trans_src = ts.src
             t.trans_dest = ts.dest
         # ref. https://github.com/SuniTheFish/ChainTranslator/blob/master/ChainTranslator/__main__.py#L31
         except ValueError as e:
-            logme.debug(__name__ + ':Tweet:translator.translate:' + str(e))
-            raise Exception("Invalid destination language: {} / Tweet: {}".format(config.TranslateDest, t.tweet))
+            logme.debug(__name__ + ":Tweet:translator.translate:" + str(e))
+            raise Exception(
+                "Invalid destination language: {} / Tweet: {}".format(
+                    config.TranslateDest, t.tweet
+                )
+            )
     return t
```

### Comparing `twint_fork-2.2.0/twint/url.py` & `twint_fork-2.5.0/twint/url.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,134 +2,123 @@
 from sys import platform
 import logging as logme
 from urllib.parse import urlencode
 from urllib.parse import quote
 
 mobile = "https://mobile.twitter.com"
 base = "https://api.twitter.com/2/search/adaptive.json"
+base = "https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name"
 
 
 def _sanitizeQuery(_url, params):
     _serialQuery = ""
     _serialQuery = urlencode(params, quote_via=quote)
     _serialQuery = _url + "?" + _serialQuery
     return _serialQuery
 
 
 def _formatDate(date):
     if "win" in platform:
-        return f'\"{date.split()[0]}\"'
+        return f'"{date.split()[0]}"'
     try:
         return int(datetime.datetime.strptime(date, "%Y-%m-%d %H:%M:%S").timestamp())
     except ValueError:
         return int(datetime.datetime.strptime(date, "%Y-%m-%d").timestamp())
 
 
 async def Favorites(username, init):
-    logme.debug(__name__ + ':Favorites')
+    logme.debug(__name__ + ":Favorites")
     url = f"{mobile}/{username}/favorites?lang=en"
 
-    if init != '-1':
+    url = f"https://api.twitter.com/1.1/favorites/list.json?screen_name={username}"
+    print(url)
+    if init != "-1":
         url += f"&max_id={init}"
 
     return url
 
 
 async def Followers(username, init):
-    logme.debug(__name__ + ':Followers')
+    logme.debug(__name__ + ":Followers")
     url = f"{mobile}/{username}/followers?lang=en"
+    url = f"https://api.twitter.com/1.1/followers/list.json?screen_name={username}&count=100"
 
-    if init != '-1':
+    if init != "-1":
         url += f"&cursor={init}"
 
     return url
 
 
 async def Following(username, init):
-    logme.debug(__name__ + ':Following')
-    url = f"{mobile}/{username}/following?lang=en"
+    logme.debug(__name__ + ":Following")
+    url = f"https://api.twitter.com/1.1/friends/list.json?screen_name={username}&count=100"
 
-    if init != '-1':
+    if init != "-1":
         url += f"&cursor={init}"
 
     return url
 
 
 async def MobileProfile(username, init):
-    logme.debug(__name__ + ':MobileProfile')
+    logme.debug(__name__ + ":MobileProfile")
     url = f"{mobile}/{username}?lang=en"
 
-    if init != '-1':
+    if init != "-1":
         url += f"&max_id={init}"
 
     return url
 
 
 async def Search(config, init):
-    logme.debug(__name__ + ':Search')
+    logme.debug(__name__ + ":Search")
     url = base
     tweet_count = 100 if not config.Limit else config.Limit
     q = ""
     params = [
         # ('include_blocking', '1'),
         # ('include_blocked_by', '1'),
         # ('include_followed_by', '1'),
         # ('include_want_retweets', '1'),
         # ('include_mute_edge', '1'),
         # ('include_can_dm', '1'),
-        ('include_can_media_tag', '1'),
+        ("include_can_media_tag", "1"),
         # ('skip_status', '1'),
         # ('include_cards', '1'),
-        ('include_ext_alt_text', 'true'),
-        ('include_quote_count', 'true'),
-        ('include_reply_count', '1'),
-        ('tweet_mode', 'extended'),
-        ('include_entities', 'true'),
-        ('include_user_entities', 'true'),
-        ('include_ext_media_availability', 'true'),
-        ('send_error_codes', 'true'),
-        ('simple_quoted_tweet', 'true'),
-        ('count', tweet_count),
-        ('query_source', 'typed_query'),
+        ("include_ext_alt_text", "true"),
+        ("include_quote_count", "true"),
+        ("include_reply_count", "1"),
+        ("tweet_mode", "extended"),
+        ("include_entities", "true"),
+        ("include_user_entities", "true"),
+        ("include_ext_media_availability", "true"),
+        ("send_error_codes", "true"),
+        ("simple_quoted_tweet", "true"),
+        ("count", tweet_count),
+        ("query_source", "typed_query"),
         # ('pc', '1'),
-        ('cursor', str(init)),
-        ('spelling_corrections', '1'),
-        ('ext', 'mediaStats%2ChighlightedLabel'),
-        ('tweet_search_mode', 'live'),  # this can be handled better, maybe take an argument and set it then
+        ("cursor", str(init)),
+        ("spelling_corrections", "1"),
+        ("ext", "mediaStats%2ChighlightedLabel"),
+        (
+            "tweet_search_mode",
+            "live",
+        ),  # this can be handled better, maybe take an argument and set it then
     ]
     if not config.Popular_tweets:
-        params.append(('f', 'tweets'))
+        params.append(("f", "tweets"))
     if config.Lang:
         params.append(("l", config.Lang))
         params.append(("lang", "en"))
     if config.Query:
         q += f" from:{config.Query}"
     if config.Username:
         q += f" from:{config.Username}"
     if config.Geo:
         config.Geo = config.Geo.replace(" ", "")
         q += f" geocode:{config.Geo}"
-    if config.Search:
-
-        q += f" {config.Search}"
-    if config.Year:
-        q += f" until:{config.Year}-1-1"
-    if config.Since:
-        q += f" since:{_formatDate(config.Since)}"
-    if config.Until:
-        q += f" until:{_formatDate(config.Until)}"
-    if config.Email:
-        q += ' "mail" OR "email" OR'
-        q += ' "gmail" OR "e-mail"'
-    if config.Phone:
-        q += ' "phone" OR "call me" OR "text me"'
-    if config.Verified:
-        q += " filter:verified"
-    if config.To:
-        q += f" to:{config.To}"
     if config.All:
         q += f" to:{config.All} OR from:{config.All} OR @{config.All}"
     if config.Near:
         q += f' near:"{config.Near}"'
     if config.Images:
         q += " filter:images"
     if config.Videos:
@@ -137,68 +126,61 @@
     if config.Media:
         q += " filter:media"
     if config.Replies:
         q += " filter:replies"
     # although this filter can still be used, but I found it broken in my preliminary testing, needs more testing
     if config.Native_retweets:
         q += " filter:nativeretweets"
-    if config.Min_likes:
-        q += f" min_faves:{config.Min_likes}"
-    if config.Min_retweets:
-        q += f" min_retweets:{config.Min_retweets}"
-    if config.Min_replies:
-        q += f" min_replies:{config.Min_replies}"
     if config.Links == "include":
         q += " filter:links"
     elif config.Links == "exclude":
         q += " exclude:links"
     if config.Source:
-        q += f" source:\"{config.Source}\""
-    if config.Members_list:
-        q += f" list:{config.Members_list}"
-    if config.Filter_retweets:
-        q += f" exclude:nativeretweets exclude:retweets"
-    if config.Custom_query:
-        q = config.Custom_query
-
+        q += f' source:"{config.Source}"'
     q = q.strip()
     params.append(("q", q))
     _serialQuery = _sanitizeQuery(url, params)
+    if init != -1:
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=100&max_id={init}"
+    else:
+        url = f"https://api.twitter.com/1.1/statuses/user_timeline.json?screen_name={config.Username}&count=100"
     return url, params, _serialQuery
 
 
 def SearchProfile(config, init=None):
-    logme.debug(__name__ + ':SearchProfile')
-    _url = 'https://api.twitter.com/2/timeline/profile/{user_id}.json'.format(user_id=config.User_id)
+    logme.debug(__name__ + ":SearchProfile")
+    _url = "https://api.twitter.com/2/timeline/profile/{user_id}.json".format(
+        user_id=config.User_id
+    )
     tweet_count = 100
     params = [
         # some of the fields are not required, need to test which ones aren't required
-        ('include_profile_interstitial_type', '1'),
-        ('include_blocking', '1'),
-        ('include_blocked_by', '1'),
-        ('include_followed_by', '1'),
-        ('include_want_retweets', '1'),
-        ('include_mute_edge', '1'),
-        ('include_can_dm', '1'),
-        ('include_can_media_tag', '1'),
-        ('skip_status', '1'),
-        ('cards_platform', 'Web - 12'),
-        ('include_cards', '1'),
-        ('include_ext_alt_text', 'true'),
-        ('include_quote_count', 'true'),
-        ('include_reply_count', '1'),
-        ('tweet_mode', 'extended'),
-        ('include_entities', 'true'),
-        ('include_user_entities', 'true'),
-        ('include_ext_media_color', 'true'),
-        ('include_ext_media_availability', 'true'),
-        ('send_error_codes', 'true'),
-        ('simple_quoted_tweet', 'true'),
-        ('include_tweet_replies', 'true'),
-        ('count', tweet_count),
-        ('ext', 'mediaStats%2ChighlightedLabel'),
+        ("include_profile_interstitial_type", "1"),
+        ("include_blocking", "1"),
+        ("include_blocked_by", "1"),
+        ("include_followed_by", "1"),
+        ("include_want_retweets", "1"),
+        ("include_mute_edge", "1"),
+        ("include_can_dm", "1"),
+        ("include_can_media_tag", "1"),
+        ("skip_status", "1"),
+        ("cards_platform", "Web - 12"),
+        ("include_cards", "1"),
+        ("include_ext_alt_text", "true"),
+        ("include_quote_count", "true"),
+        ("include_reply_count", "1"),
+        ("tweet_mode", "extended"),
+        ("include_entities", "true"),
+        ("include_user_entities", "true"),
+        ("include_ext_media_color", "true"),
+        ("include_ext_media_availability", "true"),
+        ("send_error_codes", "true"),
+        ("simple_quoted_tweet", "true"),
+        ("include_tweet_replies", "true"),
+        ("count", tweet_count),
+        ("ext", "mediaStats%2ChighlightedLabel"),
     ]
 
     if type(init) == str:
-        params.append(('cursor', str(init)))
+        params.append(("cursor", str(init)))
     _serialQuery = _sanitizeQuery(_url, params)
     return _url, params, _serialQuery
```

### Comparing `twint_fork-2.2.0/twint/verbose.py` & `twint_fork-2.5.0/twint/verbose.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,10 +9,11 @@
     else:
         msg += f"{count} Tweets"
         if config.Username:
             msg += f" from @{config.Username}"
     msg += "."
     print(msg)
 
+
 def Elastic(elasticsearch):
     if elasticsearch:
         print("[+] Indexing to Elasticsearch @ " + str(elasticsearch))
```

### Comparing `twint_fork-2.2.0/twint_fork.egg-info/PKG-INFO` & `twint_fork-2.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,8 @@
-Metadata-Version: 2.1
-Name: twint-fork
-Version: 2.2.0
-Summary: An advanced Twitter scraping & OSINT tool.
-Home-page: https://github.com/twintproject/twint
-Author: Cody Zacharias
-Author-email: codyzacharias@pm.me
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+# This is a fork from twint maintain by yihong0618
 
 # TWINT - Twitter Intelligence Tool
 ![2](https://i.imgur.com/iaH3s7z.png)
 ![3](https://i.imgur.com/hVeCrqL.png)
 
 [![PyPI](https://img.shields.io/pypi/v/twint.svg)](https://pypi.org/project/twint/) [![Build Status](https://travis-ci.org/twintproject/twint.svg?branch=master)](https://travis-ci.org/twintproject/twint) [![Python 3.6|3.7|3.8](https://img.shields.io/badge/Python-3.6%2F3.7%2F3.8-blue.svg)](https://www.python.org/download/releases/3.0/) [![GitHub license](https://img.shields.io/github/license/haccer/tweep.svg)](https://github.com/haccer/tweep/blob/master/LICENSE) [![Downloads](https://pepy.tech/badge/twint)](https://pepy.tech/project/twint) [![Downloads](https://pepy.tech/badge/twint/week)](https://pepy.tech/project/twint/week) [![Patreon](https://img.shields.io/endpoint.svg?url=https:%2F%2Fshieldsio-patreon.herokuapp.com%2Ftwintproject)](https://www.patreon.com/twintproject) ![](https://img.shields.io/twitter/follow/noneprivacy.svg?label=Follow&style=social) 
 
@@ -89,48 +71,31 @@
 
 Noticed a lot of people are having issues installing (including me). Please use the Dockerfile temporarily while I look into them. 
 
 ## CLI Basic Examples and Combos
 A few simple examples to help you understand the basics:
 
 - `twint -u username` - Scrape all the Tweets of a *user* (doesn't include **retweets** but includes **replies**).
-- `twint -u username -s pineapple` - Scrape all Tweets from the *user*'s timeline containing _pineapple_.
-- `twint -s pineapple` - Collect every Tweet containing *pineapple* from everyone's Tweets.
-- `twint -u username --year 2014` - Collect Tweets that were tweeted **before** 2014.
-- `twint -u username --since "2015-12-20 20:30:15"` - Collect Tweets that were tweeted since 2015-12-20 20:30:15.
-- `twint -u username --since 2015-12-20` - Collect Tweets that were tweeted since 2015-12-20 00:00:00.
-- `twint -u username -o file.txt` - Scrape Tweets and save to file.txt.
-- `twint -u username -o file.csv --csv` - Scrape Tweets and save as a csv file.
-- `twint -u username --email --phone` - Show Tweets that might have phone numbers or email addresses.
-- `twint -s "Donald Trump" --verified` - Display Tweets by verified users that Tweeted about Donald Trump.
-- `twint -g="48.880048,2.385939,1km" -o file.csv --csv` - Scrape Tweets from a radius of 1km around a place in Paris and export them to a csv file.
-- `twint -u username -es localhost:9200` - Output Tweets to Elasticsearch
-- `twint -u username -o file.json --json` - Scrape Tweets and save as a json file.
-- `twint -u username --database tweets.db` - Save Tweets to a SQLite database.
 - `twint -u username --followers` - Scrape a Twitter user's followers.
 - `twint -u username --following` - Scrape who a Twitter user follows.
-- `twint -u username --favorites` - Collect all the Tweets a user has favorited (gathers ~3200 tweet).
-- `twint -u username --following --user-full` - Collect full user information a person follows
-- `twint -u username --timeline` - Use an effective method to gather Tweets from a user's profile (Gathers ~3200 Tweets, including **retweets** & **replies**).
-- `twint -u username --retweets` - Use a quick method to gather the last 900 Tweets (that includes retweets) from a user's profile.
+- `twint -u username --following` - Collect full user information a person follows
 - `twint -u username --resume resume_file.txt` - Resume a search starting from the last saved scroll-id.
 
 More detail about the commands and options are located in the [wiki](https://github.com/twintproject/twint/wiki/Commands)
 
 ## Module Example
 
 Twint can now be used as a module and supports custom formatting. **More details are located in the [wiki](https://github.com/twintproject/twint/wiki/Module)**
 
 ```python
 import twint
 
 # Configure
 c = twint.Config()
 c.Username = "realDonaldTrump"
-c.Search = "great"
 
 # Run
 twint.run.Search(c)
 ```
 > Output
 
 `955511208597184512 2018-01-22 18:43:19 GMT <now> pineapples are the best fruit`
```

### Comparing `twint_fork-2.2.0/twint_fork.egg-info/SOURCES.txt` & `twint_fork-2.5.0/twint_fork.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 twint/__init__.py
+twint/__main__.py
 twint/__version__.py
 twint/cli.py
 twint/config.py
 twint/datelock.py
 twint/feed.py
 twint/format.py
 twint/get.py
```

