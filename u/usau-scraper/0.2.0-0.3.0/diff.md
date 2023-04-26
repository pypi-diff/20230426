# Comparing `tmp/usau-scraper-0.2.0.tar.gz` & `tmp/usau-scraper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usau-scraper-0.2.0.tar", last modified: Tue Apr  4 20:15:50 2023, max compression
+gzip compressed data, was "usau-scraper-0.3.0.tar", last modified: Tue Apr 25 16:33:50 2023, max compression
```

## Comparing `usau-scraper-0.2.0.tar` & `usau-scraper-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.163378 usau-scraper-0.2.0/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      301 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/.bumpversion.cfg
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      551 2023-03-21 23:52:01.000000 usau-scraper-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    11357 2023-02-07 19:30:12.000000 usau-scraper-0.2.0/LICENSE
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      536 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/MANIFEST.in
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2630 2023-04-04 18:50:42.000000 usau-scraper-0.2.0/Makefile
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    18887 2023-04-04 20:15:50.162786 usau-scraper-0.2.0/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     4960 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/README.md
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.128623 usau-scraper-0.2.0/docs/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      638 2023-04-03 14:59:19.000000 usau-scraper-0.2.0/docs/Makefile
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      799 2023-04-03 14:59:19.000000 usau-scraper-0.2.0/docs/make.bat
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.133305 usau-scraper-0.2.0/docs/source/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2029 2023-04-04 18:50:42.000000 usau-scraper-0.2.0/docs/source/conf.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      878 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/docs/source/index.rst
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.134928 usau-scraper-0.2.0/examples/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     6624 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/examples/USAU_Scraper_Example.ipynb
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2329 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/pyproject.toml
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       38 2023-04-04 20:15:50.163555 usau-scraper-0.2.0/setup.cfg
--rw-rw-r--   0 theodoremcnulty   (501) staff       (20)       39 2023-02-27 18:37:36.000000 usau-scraper-0.2.0/setup.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.137191 usau-scraper-0.2.0/usau_scraper/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      249 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/usau_scraper/__init__.py
--rw-rw-r--   0 theodoremcnulty   (501) staff       (20)      118 2023-03-08 19:58:10.000000 usau-scraper-0.2.0/usau_scraper/__main__.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    10108 2023-04-04 20:12:02.000000 usau-scraper-0.2.0/usau_scraper/teamScraper.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.139919 usau-scraper-0.2.0/usau_scraper/tests/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     5567 2023-04-03 14:59:19.000000 usau-scraper-0.2.0/usau_scraper/tests/test_all.py
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1233 2023-03-08 16:58:23.000000 usau-scraper-0.2.0/usau_scraper/tournamentScraper.py
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.161862 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    15801 2023-03-02 18:55:12.000000 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      383 2023-03-02 18:55:12.000000 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-03-02 18:55:12.000000 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-03-02 18:55:12.000000 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/requires.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       55 2023-03-02 18:55:12.000000 usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/top_level.txt
-drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-04 20:15:50.139516 usau-scraper-0.2.0/usau_scraper.egg-info/
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)    18887 2023-04-04 20:15:49.000000 usau-scraper-0.2.0/usau_scraper.egg-info/PKG-INFO
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      767 2023-04-04 20:15:50.000000 usau-scraper-0.2.0/usau_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-04-04 20:15:49.000000 usau-scraper-0.2.0/usau_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-04-04 20:15:49.000000 usau-scraper-0.2.0/usau_scraper.egg-info/requires.txt
--rw-r--r--   0 theodoremcnulty   (501) staff       (20)       13 2023-04-04 20:15:50.000000 usau-scraper-0.2.0/usau_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.166925 usau-scraper-0.3.0/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      301 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      551 2023-04-24 21:18:45.000000 usau-scraper-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    11357 2023-02-07 19:30:12.000000 usau-scraper-0.3.0/LICENSE
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      536 2023-04-04 20:12:02.000000 usau-scraper-0.3.0/MANIFEST.in
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2630 2023-04-25 15:43:37.000000 usau-scraper-0.3.0/Makefile
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    19732 2023-04-25 16:33:50.166563 usau-scraper-0.3.0/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     5805 2023-04-25 16:22:47.000000 usau-scraper-0.3.0/README.md
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.156752 usau-scraper-0.3.0/docs/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      638 2023-04-03 14:59:19.000000 usau-scraper-0.3.0/docs/Makefile
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      799 2023-04-03 14:59:19.000000 usau-scraper-0.3.0/docs/make.bat
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.158780 usau-scraper-0.3.0/docs/source/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2029 2023-04-04 18:50:42.000000 usau-scraper-0.3.0/docs/source/conf.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1722 2023-04-25 16:04:54.000000 usau-scraper-0.3.0/docs/source/index.rst
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      191 2023-04-25 16:06:05.000000 usau-scraper-0.3.0/docs/source/modules.rst
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.159939 usau-scraper-0.3.0/examples/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    33908 2023-04-05 15:20:17.000000 usau-scraper-0.3.0/examples/usau_scraper_example.ipynb
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     2329 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/pyproject.toml
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       38 2023-04-25 16:33:50.167009 usau-scraper-0.3.0/setup.cfg
+-rw-rw-r--   0 theodoremcnulty   (501) staff       (20)       39 2023-02-27 18:37:36.000000 usau-scraper-0.3.0/setup.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.162509 usau-scraper-0.3.0/usau_scraper/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      249 2023-04-25 16:26:11.000000 usau-scraper-0.3.0/usau_scraper/__init__.py
+-rw-rw-r--   0 theodoremcnulty   (501) staff       (20)      118 2023-03-08 19:58:10.000000 usau-scraper-0.3.0/usau_scraper/__main__.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    13589 2023-04-25 16:22:26.000000 usau-scraper-0.3.0/usau_scraper/teamScraper.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.164765 usau-scraper-0.3.0/usau_scraper/tests/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     5630 2023-04-25 16:17:46.000000 usau-scraper-0.3.0/usau_scraper/tests/test_all.py
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)     1233 2023-03-08 16:58:23.000000 usau-scraper-0.3.0/usau_scraper/tournamentScraper.py
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.165996 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    15801 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      383 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/requires.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       55 2023-03-02 18:55:12.000000 usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 theodoremcnulty   (501) staff       (20)        0 2023-04-25 16:33:50.164519 usau-scraper-0.3.0/usau_scraper.egg-info/
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)    19732 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      791 2023-04-25 16:33:50.000000 usau-scraper-0.3.0/usau_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)        1 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)      181 2023-04-25 16:33:49.000000 usau-scraper-0.3.0/usau_scraper.egg-info/requires.txt
+-rw-r--r--   0 theodoremcnulty   (501) staff       (20)       13 2023-04-25 16:33:50.000000 usau-scraper-0.3.0/usau_scraper.egg-info/top_level.txt
```

### Comparing `usau-scraper-0.2.0/CONTRIBUTING.md` & `usau-scraper-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/LICENSE` & `usau-scraper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/MANIFEST.in` & `usau-scraper-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/Makefile` & `usau-scraper-0.3.0/Makefile`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/PKG-INFO` & `usau-scraper-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usau-scraper
-Version: 0.2.0
+Version: 0.3.0
 Summary: The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website.
 Author-email: Erin McNulty <eem2188@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,17 +226,17 @@
 The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the [USAU website](https://play.usaultimate.org/events/tournament/?ViewAll=false&IsLeagueType=false&IsClinic=false&FilterByCategory=AE).
 
 ![Apache Liscence](https://img.shields.io/github/license/erin2722/usau-scraper?color=f72d2d)
 
 [![PyPI](https://img.shields.io/pypi/v/usau-scraper?color=2d2df7)](https://pypi.org/project/usau-scraper/)
 
 [![Docs](https://img.shields.io/badge/documentation-gh%20pages-%23fffb03)](https://erin2722.github.io/usau-scraper/)
-[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/docs/examples/USAU_Scraper_Example.ipynb)
+[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb)
 
-[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/ColumbiaOSS/example-project-python/actions?query=workflow%3A%22Build+Status%22)
+[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/erin2722/usau-scraper/actions?query=workflow%3A%22Build+Status%22)
 ![Open Issues](https://img.shields.io/github/issues/erin2722/usau-scraper?color=f79502)
 [![codecov](https://codecov.io/gh/erin2722/usau-scraper/branch/main/graph/badge.svg)](https://codecov.io/gh/erin2722/usau-scraper)
 
 ## Overview
 
 USAU (USA Ultimate) is the governing body of ultimate frisbee, and its website (which is notoriously hard to navigate) contains all of the information about high school, college, and club ultimate frisbee teams. Right now, there is no easy way to access this data. USAU scraper solves this problem by scraping the USAU website for data and therefore allowing other developers to easily use the data on the USAU site. This project will open the door to more data analytic projects concerning ultimate frisbee.
 
@@ -248,15 +248,15 @@
 
 After installing the library, there are currently 3 functions available for use: getTeamInfo, getTeamSchedule, and getTeamRoster.
 
 Simply `import * from usau_scraper`, and then call any of the following functions:
 
 ### getTeamInfo()
 
-`getTeamInfo()` returns all information about the first 10 teams matching the query
+`getTeamInfo()` returns all information about the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -276,15 +276,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamSchedule
 
-`getTeamSchedule()` returns the season schedule and record of the first 10 teams matching the query
+`getTeamSchedule()` returns the season schedule and record of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -315,15 +315,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamRoster
 
-`getTeamRoster()` returns the roster of the first 10 teams matching the query
+`getTeamRoster()` returns the roster of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -347,25 +347,51 @@
             ]
         },
         ...
     ]
 }
 ```
 
+## Example Usage
+
+After `pip install --upgrade usau-scraper` in your python env:
+
+```python
+from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+
+# Get a team's basic information
+print(getTeamInfo(
+    schoolName = 'Columbia', 
+    teamName = 'Baewatch', 
+    genderDivision=2, 
+    state='NY', 
+    competitionLevel='College', 
+    competitionDivision=1, 
+    teamDesignation=1))
+
+# Get a team's schedule for the current season
+print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
+
+# Get a team's roster for the current season
+print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
+```
+
+Additional usage examples are [in this notebook](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=20Fjgtxr35ES).
+
 ## Features (MVP)
 
 - [x] A function that, given a team name, returns basic information about them.
 - [x] A function that, given a team name, returns their schedule and record.
 - [x] A function that, given a team name, returns its roster.
 - [ ] A function that, given a tournament name, returns the results of the tournament.
 
 ## Additional features
 
 - [ ] A function that, given a college division, returns the current standings of that division.
-- [ ] An additional plugin to ultiworld to show current top 25 teams.
+- [ ] An additional plugin to [frisbee-rankings.com](http://www.frisbee-rankings.com/) to show current top 25 teams.
 - [ ] An additional plugin to ultiworld to show recent articles given a team name or college division.
 - [ ] More features tbd!
 
 ## Possible Applications
 
 - A seeding helper that, given a list of team names, returns their records for the season and their record against top 25 teams.
```

### Comparing `usau-scraper-0.2.0/README.md` & `usau-scraper-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the [USAU website](https://play.usaultimate.org/events/tournament/?ViewAll=false&IsLeagueType=false&IsClinic=false&FilterByCategory=AE).
 
 ![Apache Liscence](https://img.shields.io/github/license/erin2722/usau-scraper?color=f72d2d)
 
 [![PyPI](https://img.shields.io/pypi/v/usau-scraper?color=2d2df7)](https://pypi.org/project/usau-scraper/)
 
 [![Docs](https://img.shields.io/badge/documentation-gh%20pages-%23fffb03)](https://erin2722.github.io/usau-scraper/)
-[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/docs/examples/USAU_Scraper_Example.ipynb)
+[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb)
 
-[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/ColumbiaOSS/example-project-python/actions?query=workflow%3A%22Build+Status%22)
+[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/erin2722/usau-scraper/actions?query=workflow%3A%22Build+Status%22)
 ![Open Issues](https://img.shields.io/github/issues/erin2722/usau-scraper?color=f79502)
 [![codecov](https://codecov.io/gh/erin2722/usau-scraper/branch/main/graph/badge.svg)](https://codecov.io/gh/erin2722/usau-scraper)
 
 ## Overview
 
 USAU (USA Ultimate) is the governing body of ultimate frisbee, and its website (which is notoriously hard to navigate) contains all of the information about high school, college, and club ultimate frisbee teams. Right now, there is no easy way to access this data. USAU scraper solves this problem by scraping the USAU website for data and therefore allowing other developers to easily use the data on the USAU site. This project will open the door to more data analytic projects concerning ultimate frisbee.
 
@@ -25,15 +25,15 @@
 
 After installing the library, there are currently 3 functions available for use: getTeamInfo, getTeamSchedule, and getTeamRoster.
 
 Simply `import * from usau_scraper`, and then call any of the following functions:
 
 ### getTeamInfo()
 
-`getTeamInfo()` returns all information about the first 10 teams matching the query
+`getTeamInfo()` returns all information about the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -53,15 +53,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamSchedule
 
-`getTeamSchedule()` returns the season schedule and record of the first 10 teams matching the query
+`getTeamSchedule()` returns the season schedule and record of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -92,15 +92,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamRoster
 
-`getTeamRoster()` returns the roster of the first 10 teams matching the query
+`getTeamRoster()` returns the roster of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -124,24 +124,50 @@
             ]
         },
         ...
     ]
 }
 ```
 
+## Example Usage
+
+After `pip install --upgrade usau-scraper` in your python env:
+
+```python
+from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+
+# Get a team's basic information
+print(getTeamInfo(
+    schoolName = 'Columbia', 
+    teamName = 'Baewatch', 
+    genderDivision=2, 
+    state='NY', 
+    competitionLevel='College', 
+    competitionDivision=1, 
+    teamDesignation=1))
+
+# Get a team's schedule for the current season
+print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
+
+# Get a team's roster for the current season
+print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
+```
+
+Additional usage examples are [in this notebook](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=20Fjgtxr35ES).
+
 ## Features (MVP)
 
 - [x] A function that, given a team name, returns basic information about them.
 - [x] A function that, given a team name, returns their schedule and record.
 - [x] A function that, given a team name, returns its roster.
 - [ ] A function that, given a tournament name, returns the results of the tournament.
 
 ## Additional features
 
 - [ ] A function that, given a college division, returns the current standings of that division.
-- [ ] An additional plugin to ultiworld to show current top 25 teams.
+- [ ] An additional plugin to [frisbee-rankings.com](http://www.frisbee-rankings.com/) to show current top 25 teams.
 - [ ] An additional plugin to ultiworld to show recent articles given a team name or college division.
 - [ ] More features tbd!
 
 ## Possible Applications
 
 - A seeding helper that, given a list of team names, returns their records for the season and their record against top 25 teams.
```

### Comparing `usau-scraper-0.2.0/docs/Makefile` & `usau-scraper-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/docs/make.bat` & `usau-scraper-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/docs/source/conf.py` & `usau-scraper-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/pyproject.toml` & `usau-scraper-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "usau-scraper"
 authors = [{name = "Erin McNulty", email = "eem2188@columbia.edu"}]
 description="The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website."
 readme = "README.md"
-version = "0.2.0"
+version = "0.3.0"
 requires-python = ">=3.7"
 
 dependencies = ["bs4", "requests", "pandas", "lxml"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `usau-scraper-0.2.0/usau_scraper/teamScraper.py` & `usau-scraper-0.3.0/usau_scraper/teamScraper.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,24 +9,36 @@
 from bs4 import BeautifulSoup
 import re
 
 BASE_URL = "https://play.usaultimate.org"
 
 
 def getTeamInfo(**kwargs):
-    '''getTeamInfo() returns all information about the first 10 teams matching the query
+    '''getTeamInfo() returns all information about the first 20 teams matching the query
 
     Args:
-        schoolName
-        teamName
-        genderDivision
-        state
-        competitionLevel
-        competitionDivision
-        teamDesignation
+        ``schoolName`` (string): The school that the team is affiliated with (ex. Columbia).
+
+        ``teamName`` (string): The name of the team (ex. Pleiades).
+
+        ``genderDivision`` (string): The gender division that the team competes in.
+        Must be one of: Women, Men, Mixed, Boys, Girls.
+
+        ``state`` (string): Postal abbreviation of the state the team is in.
+
+        ``competitionLevel`` (string): The competition level that the team plays at.
+        Must be one of: Club, College, High School, or Middle School.
+
+        ``competitionDivision`` (string): The competition division that the team plays in.
+        Must be one of: Classic, Developmental, Division 1, or Division 3.
+
+        ``teamDesignation`` (string): If the team is a B or a C team. Must be B or C.
+
+        ``teamURI`` (string): If querying based on team URI, will simply return the results of the team with
+        this URI andignore other parameters.
 
     Returns:
         results:
             ::
 
                 {
                     res: OK, NOTFOUND
@@ -79,57 +91,68 @@
 
             res["teams"].append(team)
 
         return res
 
 
 def getTeamSchedule(**kwargs):
-    '''getTeamSchedule() returns the season schedule and record of the first 10 teams matching the query
+    '''getTeamSchedule() returns the season schedule and record of the first 20 teams matching the query
 
     Args:
-        schoolName,
-        teamName,
-        genderDivision,
-        state,
-        competitionLevel,
-        competitionDivision,
-        teamDesignation
+        ``schoolName`` (string): The school that the team is affiliated with (ex. Columbia).
+
+        ``teamName`` (string): The name of the team (ex. Pleiades).
+
+        ``genderDivision`` (string): The gender division that the team competes in.
+        Must be one of: Women, Men, Mixed, Boys, Girls.
+
+        ``state`` (string): Postal abbreviation of the state the team is in.
+
+        ``competitionLevel`` (string): The competition level that the team plays at.
+        Must be one of: Club, College, High School, or Middle School.
+
+        ``competitionDivision`` (string): The competition division that the team plays in.
+        Must be one of: Classic, Developmental, Division 1, or Division 3.
+
+        ``teamDesignation`` (string): If the team is a B or a C team. Must be B or C.
+
+        ``teamURI`` (string): If querying based on team URI, will simply return the results of the team with
+        this URI and ignore other parameters.
 
     Returns:
-        results:
-            ::
+        ::
 
-                {
-                    res: OK, NOTFOUND
-                    teams: [
-                        {
-                            schoolName,
-                            teamName,
-                            competitionLevel,
-                            genderDivision,
-                            wins,
-                            losses,
-                            tournaments: {
-                                name: {
-                                    games: [
-                                        {
-                                            date,
-                                            score,
-                                            opponentCollege,
-                                            opponentTeamPage
-                                        },
-                                        ...
-                                    ]
-                                },
-                                ...
+            {
+                res: OK, NOTFOUND
+                teams: [
+                    {
+                        schoolName,
+                        teamName,
+                        competitionLevel,
+                        genderDivision,
+                        wins,
+                        losses,
+                        tournaments: {
+                            name: {
+                                games: [
+                                    {
+                                        date,
+                                        score,
+                                        opponentCollege,
+                                        opponentTeamPage
+                                    },
+                                    ...
+                                ]
                             },
+                            ...
                         },
-                        ...
-                    ]
-                }'''
+                    },
+                    ...
+                ]
+            }'''
     teams = queryTeam(kwargs)
 
     if len(teams) == 0:
         return {"res": "NOTFOUND"}
 
     with requests.Session() as req:
         res = {"res": "OK", "teams": []}
@@ -176,24 +199,36 @@
 
             res["teams"].append(team)
 
         return res
 
 
 def getTeamRoster(**kwargs):
-    '''getTeamRoster() returns the roster of the first 10 teams matching the query
+    '''getTeamRoster() returns the roster of the first 20 teams matching the query
 
     Args:
-        schoolName,
-        teamName,
-        genderDivision,
-        state,
-        competitionLevel,
-        competitionDivision,
-        teamDesignation
+        ``schoolName`` (string): The school that the team is affiliated with (ex. Columbia).
+
+        ``teamName`` (string): The name of the team (ex. Pleiades).
+
+        ``genderDivision`` (string): The gender division that the team competes in.
+        Must be one of: Women, Men, Mixed, Boys, Girls.
+
+        ``state`` (string): Postal abbreviation of the state the team is in.
+
+        ``competitionLevel`` (string): The competition level that the team plays at.
+        Must be one of: Club, College, High School, or Middle School.
+
+        ``competitionDivision`` (string): The competition division that the team plays in.
+        Must be one of: Classic, Developmental, Division 1, or Division 3.
+
+        ``teamDesignation`` (string): If the team is a B or a C team. Must be B or C.
+
+        ``teamURI`` (string): If querying based on team URI, will simply return the results of the team with
+        this URI and ignore other parameters.
 
     Returns:
         results:
             ::
 
                 {
                     res: OK, NOTFOUND
@@ -268,21 +303,23 @@
     team["genderDivision"] = soup.find(id="CT_Main_0_ucTeamDetails_dlGenderDivision").find("dd").getText()
     team["location"] = soup.find(id="CT_Main_0_ucTeamDetails_dlCity").getText().strip()
 
     return team
 
 
 def queryTeam(args):
+    if "teamURI" in args:
+        return {"singleTeam": args["teamURI"]}
+
     with requests.Session() as req:
         endpoint = "/teams/events/rankings/"
         teamDict = {}
         r = req.get(BASE_URL + endpoint)
         soup = BeautifulSoup(r.content, 'html.parser')
 
-        # TODO: alternatively, if a teamID is passed in, skip this step
         data = setArgs(args)
         data['__VIEWSTATE'] = soup.find("input", id="__VIEWSTATE").get("value")
         data['__VIEWSTATEGENERATOR'] = soup.find("input", id="__VIEWSTATEGENERATOR").get("value")
         data['__EVENTVALIDATION'] = soup.find("input", id="__EVENTVALIDATION").get("value")
         r = req.post(BASE_URL + endpoint, data=data)
         soup = BeautifulSoup(r.content, 'html.parser')
 
@@ -291,23 +328,52 @@
         for link in links:
             teamDict[link.getText()] = link.get("href")
 
         return teamDict
 
 
 def setArgs(args):
-    # TODO: add input validation
-    # TODO: document the mappings from text options => ids and add them in here
+    designation_mappings = {
+        "Gender": {"Boys": 20, "Girls": 19, "Men": 17, "Mixed": 1, "Women": 2},
+        "Division": {"Classic": 10, "Developmental": 4, "Division 1": 1, "Division 3": 3},
+        "Designation": {"B": 1, "C": 2},
+    }
+
+    checkArgs(designation_mappings, args)
 
     data = {
         "__EVENTTARGET": "CT_Main_0$gvList$ctl23$ctl00$ctl00",
         "CT_Main_0$F_Status": "Published",
         "CT_Main_0$F_SchoolName": args["schoolName"] if "schoolName" in args else "",
         "CT_Main_0$F_TeamName": args["teamName"] if "teamName" in args else "",
-        "CT_Main_0$F_GenderDivisionId": args["genderDivision"] if "genderDivision" in args else "",
+        "CT_Main_0$F_GenderDivisionId": designation_mappings["Gender"][args["genderDivision"]]
+        if "genderDivision" in args
+        else "",
         "CT_Main_0$F_StateId": args["state"] if "state" in args else "",
         "CT_Main_0$F_CompetitionLevelId": args["competitionLevel"] if "competitionLevel" in args else "",
-        "CT_Main_0$F_CompetitionDivisionId": args["competitionDivision"] if "competitionDivision" in args else "",
-        "CT_Main_0$F_Designation": args["teamDesignation"] if "teamDesignation" in args else "",
+        "CT_Main_0$F_CompetitionDivisionId": designation_mappings["Division"][args["competitionDivision"]]
+        if "competitionDivision" in args
+        else "",
+        "CT_Main_0$F_Designation": designation_mappings["Designation"][args["teamDesignation"]]
+        if "teamDesignation" in args
+        else "",
     }
 
     return data
+
+
+def checkArgs(designation_mappings, args):
+    if "genderDivision" in args:
+        if args["genderDivision"] not in designation_mappings["Gender"]:
+            raise ValueError("Gender Division must be one of: Boys, Girls, Men, Mixed, Women")
+
+    if "competitionDivision" in args:
+        if args["competitionDivision"] not in designation_mappings["Division"]:
+            raise ValueError("Competition Division must be one of: Classic, Developmental, Division 1, Division 3")
+
+    if "teamDesignation" in args:
+        if args["teamDesignation"] not in designation_mappings["Designation"]:
+            raise ValueError("Competition Designation must be B or C")
+
+    if "competitionLevel" in args:
+        if args["competitionLevel"] not in ["Club", "College", "High School", "Middle School"]:
+            raise ValueError("Competition Level must be one of: Club, College, High School, Middle School")
```

### Comparing `usau-scraper-0.2.0/usau_scraper/tests/test_all.py` & `usau-scraper-0.3.0/usau_scraper/tests/test_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from usau_scraper import queryTeam, getTeamRoster, getTeamInfo, getTeamSchedule, setArgs, fillInBasicInfo
 
 # ------------------------------- UNIT TESTS -------------------------------
 
 
 # ------------------ queryTeam Tests ------------------
 def test_query_team_multiple_teams():
-    team_results = queryTeam({"schoolName": "Columbia", "competitionLevel": "College", "genderDivision": 2})
+    team_results = queryTeam({"schoolName": "Columbia", "competitionLevel": "College", "genderDivision": "Women"})
 
     expected_res_keys = ["British Columbia (Thunderbirds)", "Columbia (Curbside)", "Columbia-B (Baewatch)"]
 
     assert list(team_results.keys()) == expected_res_keys
 
 
 def test_query_team_no_teams():
@@ -23,26 +23,31 @@
 
 def test_query_team_more_than_twenty():
     team_results = queryTeam({"competitionLevel": "College"})
 
     assert len(team_results) == 20
 
 
+def test_query_team_uri_passed_in():
+    teams = queryTeam({"teamURI": "TEST_URI"})
+
+    assert len(teams) == 1
+    assert teams["singleTeam"] == "TEST_URI"
+
+
 # ------------------ setArgs Tests ------------------
 def test_set_args():
-    # TODO: change genderDivision, competitionDivision, teamDesignation to map
-    # to the non-id values, and test that
     args = {
         "schoolName": "Columbia",
         "teamName": "Baewatch",
-        "genderDivision": 2,
+        "genderDivision": "Women",
         "state": "NY",
         "competitionLevel": "College",
-        "competitionDivision": 1,
-        "teamDesignation": 1,
+        "competitionDivision": "Division 1",
+        "teamDesignation": "B",
     }
 
     expectedData = {
         "__EVENTTARGET": "CT_Main_0$gvList$ctl23$ctl00$ctl00",
         "CT_Main_0$F_Status": "Published",
         "CT_Main_0$F_SchoolName": "Columbia",
         "CT_Main_0$F_TeamName": "Baewatch",
```

### Comparing `usau-scraper-0.2.0/usau_scraper/tournamentScraper.py` & `usau-scraper-0.3.0/usau_scraper/tournamentScraper.py`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/usau_scraper/usau_scraper.egg-info/PKG-INFO` & `usau-scraper-0.3.0/usau_scraper/usau_scraper.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `usau-scraper-0.2.0/usau_scraper.egg-info/PKG-INFO` & `usau-scraper-0.3.0/usau_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usau-scraper
-Version: 0.2.0
+Version: 0.3.0
 Summary: The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the USAU website.
 Author-email: Erin McNulty <eem2188@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -226,17 +226,17 @@
 The USAU scraper is a data collector that allows developers to easily aggregate and use team results, rosters, and schedule data from the [USAU website](https://play.usaultimate.org/events/tournament/?ViewAll=false&IsLeagueType=false&IsClinic=false&FilterByCategory=AE).
 
 ![Apache Liscence](https://img.shields.io/github/license/erin2722/usau-scraper?color=f72d2d)
 
 [![PyPI](https://img.shields.io/pypi/v/usau-scraper?color=2d2df7)](https://pypi.org/project/usau-scraper/)
 
 [![Docs](https://img.shields.io/badge/documentation-gh%20pages-%23fffb03)](https://erin2722.github.io/usau-scraper/)
-[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/docs/examples/USAU_Scraper_Example.ipynb)
+[![Collab Example](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb)
 
-[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/ColumbiaOSS/example-project-python/actions?query=workflow%3A%22Build+Status%22)
+[![Build Status](https://github.com/erin2722/usau-scraper/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/erin2722/usau-scraper/actions?query=workflow%3A%22Build+Status%22)
 ![Open Issues](https://img.shields.io/github/issues/erin2722/usau-scraper?color=f79502)
 [![codecov](https://codecov.io/gh/erin2722/usau-scraper/branch/main/graph/badge.svg)](https://codecov.io/gh/erin2722/usau-scraper)
 
 ## Overview
 
 USAU (USA Ultimate) is the governing body of ultimate frisbee, and its website (which is notoriously hard to navigate) contains all of the information about high school, college, and club ultimate frisbee teams. Right now, there is no easy way to access this data. USAU scraper solves this problem by scraping the USAU website for data and therefore allowing other developers to easily use the data on the USAU site. This project will open the door to more data analytic projects concerning ultimate frisbee.
 
@@ -248,15 +248,15 @@
 
 After installing the library, there are currently 3 functions available for use: getTeamInfo, getTeamSchedule, and getTeamRoster.
 
 Simply `import * from usau_scraper`, and then call any of the following functions:
 
 ### getTeamInfo()
 
-`getTeamInfo()` returns all information about the first 10 teams matching the query
+`getTeamInfo()` returns all information about the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -276,15 +276,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamSchedule
 
-`getTeamSchedule()` returns the season schedule and record of the first 10 teams matching the query
+`getTeamSchedule()` returns the season schedule and record of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -315,15 +315,15 @@
         ...
     ]
 }
 ```
 
 ### getTeamRoster
 
-`getTeamRoster()` returns the roster of the first 10 teams matching the query
+`getTeamRoster()` returns the roster of the first 20 teams matching the query
 
 **Input:** schoolName, teamName, genderDivision, state, competitionLevel, competitionDivision, and teamDesignation as named arguments
 
 **Output:**
 
 ```
 {
@@ -347,25 +347,51 @@
             ]
         },
         ...
     ]
 }
 ```
 
+## Example Usage
+
+After `pip install --upgrade usau-scraper` in your python env:
+
+```python
+from usau_scraper import getTeamInfo, getTeamSchedule, getTeamRoster
+
+# Get a team's basic information
+print(getTeamInfo(
+    schoolName = 'Columbia', 
+    teamName = 'Baewatch', 
+    genderDivision=2, 
+    state='NY', 
+    competitionLevel='College', 
+    competitionDivision=1, 
+    teamDesignation=1))
+
+# Get a team's schedule for the current season
+print(getTeamSchedule(schoolName='Columbia', teamName='Curbside'))
+
+# Get a team's roster for the current season
+print(getTeamRoster(schoolName='Columbia', teamName='Curbside'))
+```
+
+Additional usage examples are [in this notebook](https://colab.research.google.com/github/erin2722/usau-scraper/blob/main/examples/usau_scraper_example.ipynb#scrollTo=20Fjgtxr35ES).
+
 ## Features (MVP)
 
 - [x] A function that, given a team name, returns basic information about them.
 - [x] A function that, given a team name, returns their schedule and record.
 - [x] A function that, given a team name, returns its roster.
 - [ ] A function that, given a tournament name, returns the results of the tournament.
 
 ## Additional features
 
 - [ ] A function that, given a college division, returns the current standings of that division.
-- [ ] An additional plugin to ultiworld to show current top 25 teams.
+- [ ] An additional plugin to [frisbee-rankings.com](http://www.frisbee-rankings.com/) to show current top 25 teams.
 - [ ] An additional plugin to ultiworld to show recent articles given a team name or college division.
 - [ ] More features tbd!
 
 ## Possible Applications
 
 - A seeding helper that, given a list of team names, returns their records for the season and their record against top 25 teams.
```

### Comparing `usau-scraper-0.2.0/usau_scraper.egg-info/SOURCES.txt` & `usau-scraper-0.3.0/usau_scraper.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 README.md
 pyproject.toml
 setup.py
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
-examples/USAU_Scraper_Example.ipynb
+docs/source/modules.rst
+examples/usau_scraper_example.ipynb
 usau_scraper/__init__.py
 usau_scraper/__main__.py
 usau_scraper/teamScraper.py
 usau_scraper/tournamentScraper.py
 usau_scraper.egg-info/PKG-INFO
 usau_scraper.egg-info/SOURCES.txt
 usau_scraper.egg-info/dependency_links.txt
```

