# Comparing `tmp/aa_rss_to_discord-1.5.0.tar.gz` & `tmp/aa_rss_to_discord-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_rss_to_discord-1.5.0.tar", last modified: Sun Apr 16 17:42:07 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aa_rss_to_discord-1.5.0.tar` & `aa_rss_to_discord-1.6.0.tar`

### file list

```diff
@@ -1,59 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.787154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.795154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.795154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-16 17:42:07.803154 aa_rss_to_discord-1.5.0/setup.cfg
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/admin.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/apps.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/auth_hooks.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/constants.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/managers.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/models.py
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/discordbot/cogs/__init__.py
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/discordbot/cogs/rss.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/django.pot
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/migrations/0001_initial.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/aa_rss_to_discord/migrations/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/LICENSE
+-rw-r--r--   0        0        0     6016 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/README.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 aa_rss_to_discord-1.6.0/PKG-INFO
```

### Comparing `aa_rss_to_discord-1.5.0/LICENSE` & `aa_rss_to_discord-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/PKG-INFO` & `aa_rss_to_discord-1.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: aa_rss_to_discord
-Version: 1.5.0
+Name: aa-rss-to-discord
+Version: 1.6.0
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
-Home-page: https://github.com/ppfeufer/aa-rss-to-discord
-Author: Peter Pfeufer
-Author-email: develop@ppfeufer.de
-Maintainer: Peter Pfeufer
-Maintainer-email: develop@ppfeufer.de
-License: GPL-3.0
-Project-URL: Issue / Bug Reports, https://github.com/ppfeufer/aa-rss-to-discord/issues
+Project-URL: Homepage, https://github.com/ppfeufer/aa-rss-to-discord
+Project-URL: Documentation, https://github.com/ppfeufer/aa-rss-to-discord/blob/master/README.md
+Project-URL: Source, https://github.com/ppfeufer/aa-rss-to-discord.git
 Project-URL: Changelog, https://github.com/ppfeufer/aa-rss-to-discord/blob/master/CHANGELOG.md
-Keywords: allianceauth,eveonline,discord,rss
+Project-URL: Tracker, https://github.com/ppfeufer/aa-rss-to-discord/issues
+Author-email: Peter Pfeufer <develop@ppfeufer.de>
+License-Expression: GPL-3.0
+License-File: LICENSE
+Keywords: allianceauth,discord,eveonline,rss
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -22,16 +22,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: ~=3.8
+Requires-Dist: allianceauth-app-utils>=1.14.2
+Requires-Dist: allianceauth-discordbot>=3.0.5
+Requires-Dist: allianceauth>=3.0.0
+Requires-Dist: feedparser
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Alliance Auth RSS to Discord
 
 [![Version](https://img.shields.io/pypi/v/aa-rss-to-discord?label=release)](https://pypi.org/project/aa-rss-to-discord/)
 [![License](https://img.shields.io/github/license/ppfeufer/aa-rss-to-discord)](https://github.com/ppfeufer/aa-rss-to-discord/blob/master/LICENSE)
 [![Python](https://img.shields.io/pypi/pyversions/aa-rss-to-discord)](https://pypi.org/project/aa-rss-to-discord/)
 [![Django](https://img.shields.io/pypi/djversions/aa-rss-to-discord?label=django)](https://pypi.org/project/aa-rss-to-discord/)
```

### Comparing `aa_rss_to_discord-1.5.0/README.md` & `aa_rss_to_discord-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/rss.py` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/discordbot/cogs/rss.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 "Last-Translator: Nikolay <nick.postnikov@gmail.com>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-rss-to-discord/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=4; plural= n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "X-Generator: Weblate 4.16.4\n"
 
 #: models.py:41
 msgid "RSS Feed"
 msgstr "RSS лента"
 
 #: models.py:42
```

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0001_initial.py` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/models.py` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/models.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.5.0/aa_rss_to_discord/tasks.py` & `aa_rss_to_discord-1.6.0/aa_rss_to_discord/tasks.py`

 * *Files identical despite different names*

