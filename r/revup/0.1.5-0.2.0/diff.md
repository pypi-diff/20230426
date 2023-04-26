# Comparing `tmp/revup-0.1.5.tar.gz` & `tmp/revup-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revup-0.1.5.tar", last modified: Wed Jan 11 23:14:38 2023, max compression
+gzip compressed data, was "revup-0.2.0.tar", last modified: Tue Apr 25 18:54:51 2023, max compression
```

## Comparing `revup-0.1.5.tar` & `revup-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:14:38.822288 revup-0.1.5/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1069 2023-01-11 23:02:09.000000 revup-0.1.5/LICENSE
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    12901 2023-01-11 23:14:38.822288 revup-0.1.5/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    11281 2023-01-11 23:02:09.000000 revup-0.1.5/README.md
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:02:09.000000 revup-0.1.5/pyproject.toml
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:14:38.818288 revup-0.1.5/revup/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      147 2023-01-11 23:13:47.000000 revup-0.1.5/revup/__init__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1170 2023-01-11 23:02:09.000000 revup-0.1.5/revup/__main__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     8930 2023-01-11 23:02:09.000000 revup-0.1.5/revup/amend.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2632 2023-01-11 23:02:09.000000 revup-0.1.5/revup/cherry_pick.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2161 2023-01-11 23:12:37.000000 revup-0.1.5/revup/config.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    27155 2023-01-11 23:02:09.000000 revup-0.1.5/revup/git.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      394 2023-01-11 23:02:09.000000 revup-0.1.5/revup/github.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2817 2023-01-11 23:02:09.000000 revup-0.1.5/revup/github_real.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    21667 2023-01-11 23:02:09.000000 revup-0.1.5/revup/github_utils.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2244 2023-01-11 23:02:09.000000 revup-0.1.5/revup/logs.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:14:38.822288 revup-0.1.5/revup/man1/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1338 2023-01-11 23:14:32.000000 revup-0.1.5/revup/man1/amend.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      693 2023-01-11 23:14:32.000000 revup-0.1.5/revup/man1/cherry-pick.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      932 2023-01-11 23:14:32.000000 revup-0.1.5/revup/man1/restack.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2513 2023-01-11 23:14:33.000000 revup-0.1.5/revup/man1/revup.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3385 2023-01-11 23:14:33.000000 revup-0.1.5/revup/man1/upload.1.gz
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      574 2023-01-11 23:02:09.000000 revup-0.1.5/revup/restack.py
--rwxrwxr-x   0 jerry     (1000) jerry     (1000)    15107 2023-01-11 23:12:37.000000 revup-0.1.5/revup/revup.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     9819 2023-01-11 23:02:09.000000 revup-0.1.5/revup/shell.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2390 2023-01-11 23:02:09.000000 revup-0.1.5/revup/toolkit.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    61002 2023-01-11 23:02:09.000000 revup-0.1.5/revup/topic_stack.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1074 2023-01-11 23:02:09.000000 revup-0.1.5/revup/types.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3790 2023-01-11 23:02:09.000000 revup-0.1.5/revup/upload.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:14:38.822288 revup-0.1.5/revup.egg-info/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    12901 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      680 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/SOURCES.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/dependency_links.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       47 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/entry_points.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       75 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/requires.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        6 2023-01-11 23:14:38.000000 revup-0.1.5/revup.egg-info/top_level.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1806 2023-01-11 23:14:38.822288 revup-0.1.5/setup.cfg
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      861 2023-01-11 23:02:09.000000 revup-0.1.5/setup.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.117042 revup-0.2.0/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1069 2023-01-11 23:02:09.000000 revup-0.2.0/LICENSE
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    12928 2023-04-25 18:54:51.117042 revup-0.2.0/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    11281 2023-01-11 23:02:09.000000 revup-0.2.0/README.md
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2023-01-11 23:02:09.000000 revup-0.2.0/pyproject.toml
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      147 2023-04-25 18:52:57.000000 revup-0.2.0/revup/__init__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      976 2023-04-15 00:51:58.000000 revup-0.2.0/revup/__main__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9280 2023-04-13 20:59:39.000000 revup-0.2.0/revup/amend.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2653 2023-04-13 20:59:39.000000 revup-0.2.0/revup/cherry_pick.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3568 2023-04-13 17:46:12.000000 revup-0.2.0/revup/config.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    29863 2023-04-14 21:18:39.000000 revup-0.2.0/revup/git.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      394 2023-01-11 23:02:09.000000 revup-0.2.0/revup/github.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2817 2023-01-11 23:02:09.000000 revup-0.2.0/revup/github_real.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    21678 2023-04-15 00:51:58.000000 revup-0.2.0/revup/github_utils.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2302 2023-04-13 20:59:39.000000 revup-0.2.0/revup/logs.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup/man1/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1336 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/amend.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      692 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/cherry-pick.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1019 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/config.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      931 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/restack.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2194 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/revup.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3492 2023-04-25 18:54:10.000000 revup-0.2.0/revup/man1/upload.1.gz
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      412 2023-04-13 20:59:39.000000 revup-0.2.0/revup/restack.py
+-rwxrwxr-x   0 jerry     (1000) jerry     (1000)    16057 2023-04-13 17:46:12.000000 revup-0.2.0/revup/revup.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9819 2023-01-11 23:02:09.000000 revup-0.2.0/revup/shell.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2402 2023-03-06 21:56:06.000000 revup-0.2.0/revup/toolkit.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    63501 2023-04-14 01:18:56.000000 revup-0.2.0/revup/topic_stack.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2490 2023-04-19 02:22:49.000000 revup-0.2.0/revup/types.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3652 2023-04-13 23:09:23.000000 revup-0.2.0/revup/upload.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.113042 revup-0.2.0/revup.egg-info/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    12928 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      725 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       47 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/entry_points.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       85 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/requires.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        6 2023-04-25 18:54:51.000000 revup-0.2.0/revup.egg-info/top_level.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1817 2023-04-25 18:54:51.117042 revup-0.2.0/setup.cfg
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      861 2023-01-11 23:02:09.000000 revup-0.2.0/setup.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2023-04-25 18:54:51.117042 revup-0.2.0/tests/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1569 2023-01-11 23:02:09.000000 revup-0.2.0/tests/test_tools.py
```

### Comparing `revup-0.1.5/LICENSE` & `revup-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revup-0.1.5/PKG-INFO` & `revup-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revup
-Version: 0.1.5
+Version: 0.2.0
 Summary: Revolutionary github tools. Effortlessly create multiple branches and pull requests.
 Home-page: https://github.com/skydio/revup
 Author: Jerry Zhang
 Author-email: jerry@skydio.com
 License: MIT
 Project-URL: Source, https://github.com/skydio/revup
 Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
@@ -28,30 +28,30 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
 
-  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/revup_light.svg"/>
+  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/revup_light.svg"/>
 
 </p>
 
 <p align="center">
 <a href="https://github.com/Skydio/revup"><img alt="Source Code" src="https://img.shields.io/badge/source-code-blue"/></a>
 <a href="https://github.com/Skydio/revup/issues"><img alt="Issues" src="https://img.shields.io/badge/issue-tracker-blue"/></a>
 <img alt="Python 3.8 | 3.9 | 3.10" src="https://img.shields.io/pypi/pyversions/revup"/>
 <a href="https://pypi.org/project/revup/"><img alt="PyPI" src="https://img.shields.io/pypi/v/revup"/></a>
 <a href="https://github.com/Skydio/revup/tree/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/pypi/l/revup"/></a>
 </p>
 
 Revup provides command-line tools that allow developers to iterate faster on parallel changes and reduce the overhead of creating and maintaining code reviews.
 
 <p align="center">
-<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_1.gif"/>
+<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif"/>
 </p>
 
 # Features
 
 - Revup creates multiple independent chains of branches for you in the background and without touching your working tree. It then creates and manages github pull requests for all those branches.
 - Pull requests target the actual base branch and can be merged manually or by continuous integration
 - Rebase detection saves time and continuous integration cost by not re-pushing if the patch hasn't changed
@@ -116,34 +116,34 @@
 git commit -m "My first revup foo" -m "Topic: foo"
 echo peh > bar; git add bar
 git commit -m "My first revup bar" -m "Topic: bar"
 
 revup upload
 ```
 
-![tutorial_1](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_1.gif)
+![tutorial_1](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif)
 
 You've uploaded your first revup changes! Notice how in github, both branches target 'main'. This allows them to be merged independently.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/bar_github.png" width="50%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/bar_github.png" width="50%">
 
 Under the hood, revup creates and pushes these branches for you, tracking and managing the dependencies as needed.
 
 ## Create relative pull requests
 
 Now we'll make a new review that's relative to "foo". The "Relative" tag will ensure the new review targets the correct branch.
 
 ```sh
 echo deh >> foo; git add foo
 git commit -m "My second revup foo" -m "Topic: foo2" -m "Relative: foo"
 
 revup upload
 ```
 
-![tutorial_2](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_2.gif)
+![tutorial_2](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif)
 
 With this simple but powerful model, you can upload independent and dependent changes all at once.
 
 - Multiple commits can be in one topic, in which case they will all be in a single pull request.
 - Commits in the same topic do not need to be adjacent in history.
 - Topics relative to each other do not need to be adjacent in history, but the second topic must come after the first.
 
@@ -157,15 +157,15 @@
 revup amend HEAD~ --no-edit  # Specify a commit to amend
 # or
 revup amend bar --no-edit  # Specify a topic name to amend
 
 revup upload
 ```
 
-![tutorial_3](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_3.gif)
+![tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_3.gif)
 
 `revup amend` makes it easy to modify commits in your history. You also have other options for modifying reviews:
 
 - Adding new commits with the same topic
 - Using `git rebase --interactive` along with `git commit --amend`
 
 ## Pulling in upstream changes
@@ -238,19 +238,19 @@
 revup upload --base-branch custom-branch-name
 ```
 
 ## Review graph and patchsets
 
 Revup will add 2 comments in every pull request to provide helpful features for users and reviewers. These are enabled by default and automatically updated as the pull request changes.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/review_graph.png" width="40%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/review_graph.png" width="40%">
 
 The review graph provides links and titles to all local pull requests that have a relative relationship with the current pull request, including any that it depends on, or that depend on it. This allows you to quickly browse between pull requests in a chain.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/patchsets.png" width="80%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png" width="80%">
 
 The patchsets table provides a history of uploads for a given pull request as well as links and summaries of the diff between each upload. Notably, revup specially handles
 the case where you rebase then upload and will show you a diff with upstream files excluded.
 
 # Configuring revup
 
 Revup is highly configurable using a standard config file format. Every flag is also a config option, so users can get the exact behavior they need.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revup Version: 0.1.5 Summary: Revolutionary github
+Metadata-Version: 2.1 Name: revup Version: 0.2.0 Summary: Revolutionary github
 tools. Effortlessly create multiple branches and pull requests. Home-page:
 https://github.com/skydio/revup Author: Jerry Zhang Author-email:
 jerry@skydio.com License: MIT Project-URL: Source, https://github.com/skydio/
 revup Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
 Keywords: github python git workflow version-control python3 developer-tools
 code-review pull-requests developers developer-productivity stacked-diffs
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -51,41 +51,41 @@
 permissions". Revup needs this in order to create and modify pull requests. ##
 Create independent pull requests Make your first two commits that will become
 two separate pull requests. Note the "Topic:" tag in the commit message - this
 is what causes revup to recognize and act on a commit. Each separately named
 topic will become a new pull request. ```sh echo meh > foo; git add foo git
 commit -m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git
 commit -m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1]
-(https://raw.githubusercontent.com/skydio/revup/main/docs/images/
+(https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
 tutorial_1.gif) You've uploaded your first revup changes! Notice how in github,
 both branches target 'main'. This allows them to be merged independently.
-[https://raw.githubusercontent.com/skydio/revup/main/docs/images/
-foo_github.png][https://raw.githubusercontent.com/skydio/revup/main/docs/
+[https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
+foo_github.png][https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
 images/bar_github.png] Under the hood, revup creates and pushes these branches
 for you, tracking and managing the dependencies as needed. ## Create relative
 pull requests Now we'll make a new review that's relative to "foo". The
 "Relative" tag will ensure the new review targets the correct branch. ```sh
 echo deh >> foo; git add foo git commit -m "My second revup foo" -m "Topic:
 foo2" -m "Relative: foo" revup upload ``` ![tutorial_2](https://
-raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_2.gif) With
+raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif) With
 this simple but powerful model, you can upload independent and dependent
 changes all at once. - Multiple commits can be in one topic, in which case they
 will all be in a single pull request. - Commits in the same topic do not need
 to be adjacent in history. - Topics relative to each other do not need to be
 adjacent in history, but the second topic must come after the first. ## Modify
 pull requests Now let's update a pull request. ```sh echo heh >> bar; git add
 bar # Either revup amend HEAD~ --no-edit # Specify a commit to amend # or revup
 amend bar --no-edit # Specify a topic name to amend revup upload ``` !
-[tutorial_3](https://raw.githubusercontent.com/skydio/revup/main/docs/images/
-tutorial_3.gif) `revup amend` makes it easy to modify commits in your history.
-You also have other options for modifying reviews: - Adding new commits with
-the same topic - Using `git rebase --interactive` along with `git commit --
-amend` ## Pulling in upstream changes Use `git pull --rebase` to pull in
-changes. Don't use `git merge` or `git pull` without rebase as this creates a
-merge commit. By default revup will not upload if you pull but haven't made
+[tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
+images/tutorial_3.gif) `revup amend` makes it easy to modify commits in your
+history. You also have other options for modifying reviews: - Adding new
+commits with the same topic - Using `git rebase --interactive` along with `git
+commit --amend` ## Pulling in upstream changes Use `git pull --rebase` to pull
+in changes. Don't use `git merge` or `git pull` without rebase as this creates
+a merge commit. By default revup will not upload if you pull but haven't made
 changes to a commit. To override this and upload always, run `revup upload --
 rebase`. ``` [pull] rebase = true [rebase] autoStash = true ``` We recommend
 adding the above to `.gitconfig` to make pulling and rebasing easier. # More
 features This is a non-exhaustive intro to some more handy revup features. For
 a full description of features, see the [docs](https://github.com/Skydio/revup/
 tree/main/docs) or run `revup -h` or `revup upload -h` to view docs in `man`
 format. ## Work with forks For contributing to projects that you may not have
@@ -110,20 +110,20 @@
 latter case). ``` A fix for multiple branches Topic: fix Branches: main, rel1.1
 ``` You can specify base branch on the command line as well, although this is
 usually not necessary unless you're working on a branch that the autodetector
 doesn't know about (see Repo config below). ``` revup upload --base-branch
 custom-branch-name ``` ## Review graph and patchsets Revup will add 2 comments
 in every pull request to provide helpful features for users and reviewers.
 These are enabled by default and automatically updated as the pull request
-changes. [https://raw.githubusercontent.com/skydio/revup/main/docs/images/
+changes. [https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
 review_graph.png] The review graph provides links and titles to all local pull
 requests that have a relative relationship with the current pull request,
 including any that it depends on, or that depend on it. This allows you to
 quickly browse between pull requests in a chain. [https://
-raw.githubusercontent.com/skydio/revup/main/docs/images/patchsets.png] The
+raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png] The
 patchsets table provides a history of uploads for a given pull request as well
 as links and summaries of the diff between each upload. Notably, revup
 specially handles the case where you rebase then upload and will show you a
 diff with upstream files excluded. # Configuring revup Revup is highly
 configurable using a standard config file format. Every flag is also a config
 option, so users can get the exact behavior they need. Flags specified on the
 command line take precedence, followed by config in `~/.revupconfig`, followed
```

### Comparing `revup-0.1.5/README.md` & `revup-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `revup-0.1.5/revup/amend.py` & `revup-0.2.0/revup/amend.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import asyncio
 import logging
 import re
 import subprocess
 
 from revup import git, topic_stack
 from revup.types import (
+    CommitHeader,
     GitConflictException,
     GitTreeHash,
     RevupConflictException,
     RevupUsageException,
 )
 
 RE_TOPIC_WITH_MODIFIERS = re.compile(r"(?P<topic>[a-zA-Z\-_0-9]+)(?P<modifiers>[\^~]+[0-9]*)?")
@@ -165,73 +166,83 @@
 
     if not args.no_edit and not args.drop:
         new_msg = invoke_editor_for_commit_msg(
             git_ctx,
             git_ctx.editor,
             await get_topic_summary(topics) if args.parse_topics else "",
             stack[0].commit_msg,
-            await git_ctx.git_stdout("--no-pager", "diff", "--cached", "--stat", "--no-color")
-            if has_diff
-            else "",
-            ""
-            if args.insert
-            else await git_ctx.git_stdout(
-                "--no-pager", "diff", commit + "~", commit, "--stat", "--no-color"
+            (
+                await git_ctx.git_stdout("--no-pager", "diff", "--cached", "--stat", "--no-color")
+                if has_diff
+                else ""
+            ),
+            (
+                ""
+                if args.insert
+                else await git_ctx.git_stdout(
+                    "--no-pager", "diff", commit + "~", commit, "--stat", "--no-color"
+                )
             ),
         )
         if len(new_msg.strip()) == 0:
             logging.info("Exited due to empty commit message.")
             return 1
 
         if stack[0].commit_msg == new_msg and not has_diff:
             return 0
 
         stack[0].commit_msg = new_msg
 
     if has_diff:
-        if not args.drop:
-            stack[-1].tree = GitTreeHash(await git_ctx.git_stdout("write-tree"))
         new_commit = stack[0].parents[0]
 
         for i, commit_obj in enumerate(stack):
             if i == 0 and args.drop:
                 # Drop the target commit
                 continue
             elif i == 0 and len(stack) > 1:
                 # Perform an amend for the first commit, unless there's only one
                 # in which case we can use the tree shortcut.
+                temp_commit = CommitHeader(
+                    GitTreeHash(await git_ctx.git_stdout("write-tree")), [git.HEAD_COMMIT]
+                )
+                temp_commit.title = temp_commit.commit_msg = "cached changes"
+                temp_commit.commit_id = await git_ctx.commit_tree(temp_commit)
+                stack[-1].tree = temp_commit.tree
                 try:
-                    new_commit = await git_ctx.synthetic_amend(commit_obj)
+                    new_commit = await git_ctx.synthetic_amend(commit_obj, temp_commit)
                 except GitConflictException as exc:
+                    await git_ctx.dump_conflict(exc)
                     raise RevupConflictException(
-                        "Couldn't apply cached changes to\n"
-                        f'"{commit_obj.title}" ({commit_obj.commit_id[:8]})\n'
-                        "You may need to `git rebase -i` to resolve these conflicts!"
+                        temp_commit,
+                        commit_obj.commit_id,
+                        "You may need to `git rebase -i` to resolve these conflicts!",
                     ) from exc
             else:
                 if i == len(stack) - 1 and not args.drop:
                     # For the final commit (if drop isn't used) we can assume that
                     # the state is the exact same as the original cache, so we
                     # don't actually have to apply a patch.
                     new_commit = await git_ctx.cherry_pick_from_tree(commit_obj, new_commit)
                 else:
                     try:
                         new_commit = await git_ctx.synthetic_cherry_pick_from_commit(
                             commit_obj, new_commit
                         )
                     except GitConflictException as exc:
+                        await git_ctx.dump_conflict(exc)
                         raise RevupConflictException(
-                            f'Couldn\'t re-apply commit "{commit_obj.title}"'
-                            f" ({commit_obj.commit_id[:8]})\nYou may need to `git rebase -i` to"
-                            " resolve these conflicts!"
+                            commit_obj,
+                            new_commit,
+                            "You may need to `git rebase -i` to resolve these conflicts!",
                         ) from exc
     else:
         # If there's no diff (only text changed), its much faster to use the same trees
         new_commit = stack[0].parents[0]
         for stack_entry in stack:
             new_commit = await git_ctx.cherry_pick_from_tree(stack_entry, new_commit)
 
     git_env = {
         "GIT_REFLOG_ACTION": "reset --soft (revup amend)",
     }
-    await git_ctx.git("reset", "--soft", new_commit, env=git_env)
+    await git_ctx.soft_reset(new_commit, git_env)
     return 0
```

### Comparing `revup-0.1.5/revup/cherry_pick.py` & `revup-0.2.0/revup/cherry_pick.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     """
     Squash the given branch's changes into a single commit, and cherry-pick
     that commit onto the local branch.
     """
     branch_to_pick = args.branch[0]
     remote_branch_to_pick = git_ctx.ensure_branch_prefix(branch_to_pick)
     branch_exists, remote_branch_exists = await asyncio.gather(
-        git_ctx.commit_exists(branch_to_pick), git_ctx.commit_exists(remote_branch_to_pick)
+        git_ctx.is_branch_or_commit(branch_to_pick),
+        git_ctx.is_branch_or_commit(remote_branch_to_pick),
     )
     if remote_branch_exists and not branch_exists:
         logging.warning(
             f"Couldn't find '{branch_to_pick}', assuming you meant '{remote_branch_to_pick}'"
         )
         branch_to_pick = remote_branch_to_pick
     elif not branch_exists:
```

### Comparing `revup-0.1.5/revup/git.py` & `revup-0.2.0/revup/git.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import asyncio
 import copy
 import logging
 import os
 import re
 import shutil
 import tempfile
-from dataclasses import dataclass
 from typing import Any, Dict, List, NamedTuple, Optional, Pattern, Tuple
 
+from async_lru import alru_cache as lru_cache
+
 from revup import shell
 from revup.types import (
+    CommitHeader,
     GitCommitHash,
+    GitConflict,
     GitConflictException,
     GitTreeHash,
     RevupUsageException,
 )
 
 RE_RAW_COMMIT_ID = re.compile(r"^(?P<commit>[a-f0-9]+)$", re.MULTILINE)
 RE_RAW_AUTHOR = re.compile(
@@ -36,14 +39,16 @@
     r"^:(?P<old_mode>[0-9]+) (?P<new_mode>[0-9]+) (?P<old_hash>[0-9a-f]+) (?P<new_hash>[0-9a-f]+)"
     r" (?P<type>[a-zA-Z]+)\t(?P<path>.*)$",
     re.MULTILINE,
 )
 
 RE_COMMIT_HASH = re.compile(r"^[0-9a-f]{8,}")
 
+HEAD_COMMIT = GitCommitHash("HEAD")
+
 GIT_DIFF_ARGS = [
     "--no-pager",
     "diff",
     "--full-index",
     "--no-color",
     "--no-textconv",
     "-U1",
@@ -54,33 +59,14 @@
 
 GitHubRepoInfo = NamedTuple(
     "GitHubRepoInfo",
     [("name", str), ("owner", str)],
 )
 
 
-@dataclass
-class CommitHeader:
-    """
-    Represents the information extracted from `git rev-list --header`
-    """
-
-    tree: GitTreeHash
-    parents: List[GitCommitHash]
-    author_name: str = ""
-    author_email: str = ""
-    author_date: str = ""
-    committer_name: str = ""
-    committer_email: str = ""
-    committer_date: str = ""
-    commit_msg: str = ""
-    title: str = ""
-    commit_id: GitCommitHash = GitCommitHash("")
-
-
 def parse_commit_header(raw_header: str) -> CommitHeader:
     def _search_group(raw_header: str, regex: Pattern[str], group: str) -> str:
         m = regex.search(raw_header)
         assert m
         return m.group(group)
 
     tree = GitTreeHash(_search_group(raw_header, RE_RAW_TREE, "tree"))
@@ -177,15 +163,15 @@
 
     repo_root, git_dir, actual_version, email, editor, main_exists = await asyncio.gather(
         git_ctx.git_stdout("rev-parse", "--show-toplevel"),
         git_ctx.git_stdout("rev-parse", "--path-format=absolute", "--git-dir"),
         git_ctx.git_stdout("--version"),
         get_email(),
         get_editor(),
-        git_ctx.commit_exists(main_branch),
+        git_ctx.is_branch_or_commit(f"{remote_name}/{main_branch}"),
     )
 
     if git_version:
         version_arr = [int(v) for v in git_version.split(".")]
         actual_version_arr = [int(v) for v in actual_version.split()[2].split(".")[:3]]
         for v, a in zip(version_arr, actual_version_arr):
             if a > v:
@@ -259,14 +245,26 @@
         self.base_branch_globs = base_branch_globs.strip().splitlines()
         self.temp_dir = tempfile.TemporaryDirectory(  # pylint: disable=consider-using-with
             prefix="revup_"
         )
         if self.keep_temp:
             os.makedirs(self.get_scratch_dir(), exist_ok=True)
 
+    def clear_cache(self) -> None:
+        """
+        Clear caches for all functions that are decorated with lru_cache(). This is generally
+        overdoing it since its usually sufficient to only clear certain entries, however most usages
+        currently happen at the end of the program so it isn't worth optimizing now.
+        """
+        self.is_branch_or_commit.cache_clear()  # pylint: disable=no-member
+        self.to_commit_hash.cache_clear()  # pylint: disable=no-member
+        self.fork_point.cache_clear()  # pylint: disable=no-member
+        self.distance_to_fork_point.cache_clear()  # pylint: disable=no-member
+        self.have_identical_trees.cache_clear()  # pylint: disable=no-member
+
     def get_scratch_dir(self) -> str:
         """
         Get the name of the current scratch directory. Any contents will be deleted
         when the program exits.
         """
         return f"{self.repo_root}/.revup" if self.keep_temp else self.temp_dir.name
 
@@ -318,15 +316,15 @@
 
         info = GitHubRepoInfo(owner=owner, name=name)
         return info
 
     async def rev_list(
         self,
         include: str,
-        exclude: str = None,
+        exclude: Optional[str] = None,
         first_parent: bool = False,
         exclude_first_parent: bool = False,
         header: bool = False,
         max_revs: int = 0,
     ) -> str:
         """
         Wrapper for git rev-list
@@ -340,31 +338,33 @@
             rev_list_args.append("--exclude-first-parent-only")
         if header:
             rev_list_args.append("--header")
         if exclude is not None:
             rev_list_args.extend(["--not", exclude])
         return await self.git_stdout(*rev_list_args)
 
+    @lru_cache(maxsize=None)
     async def is_branch_or_commit(self, obj: str) -> bool:
         return await self.git_return_code("rev-parse", "--verify", "--quiet", obj) == 0
 
     async def verify_branch_or_commit(self, obj: str) -> None:
         if not await self.is_branch_or_commit(obj):
             raise RevupUsageException(f"{obj} is not a commit or branch name!")
 
-    async def commit_exists(self, obj: str) -> bool:
-        return (
-            await self.git_return_code("rev-parse", "--verify", "--quiet", obj + "^{commit}") == 0
-        )
-
+    @lru_cache(maxsize=None)
     async def to_commit_hash(self, ref: str) -> GitCommitHash:
-        return GitCommitHash(
-            await self.git_stdout("rev-parse", "--verify", "--quiet", ref + "^{commit}")
+        ret, stdout = await self.git(
+            "rev-parse", "--verify", "--quiet", ref + "^{commit}", raiseonerror=False
         )
+        if ret != 0:
+            raise RevupUsageException(f"{ref} is not a branch name!")
+
+        return GitCommitHash(stdout)
 
+    @lru_cache(maxsize=None)
     async def fork_point(self, ref: str, baseRef: str) -> GitCommitHash:
         """
         Define the fork-point of your branch and a base branch as the commit at
         which the two branches first diverged in history.
         To find this, get the list of commits reachable from your branch,
         but not reachable from the base branch. The fork point is the parent of
         the last commit in that list, and the length of that commit list is
@@ -386,14 +386,15 @@
             )
         )[1].split("\n")[0]
 
         if not commit:
             return GitCommitHash(ref)
         return GitCommitHash(f"{commit}~")
 
+    @lru_cache(maxsize=None)
     async def distance_to_fork_point(self, ref: str, baseRef: str, max_n: int = 0) -> int:
         """
         Return number of commits between ref and its fork point with baseRef, up to the given max.
         """
         max_args = ["-n", f"{max_n + 1}"] if max_n else []
         ret = await self.git_stdout(
             "rev-list",
@@ -409,16 +410,19 @@
     async def is_ancestor(self, ref: str, ancestor: str) -> bool:
         """
         Return whether ref is a first parent ancestor of the given ancestor.
 
         This is different from merge-base --is-ancestor since that checks all
         parents, not just the first.
         """
+        if ref == ancestor:
+            return True
         return await self.distance_to_fork_point(ref, ancestor, 1) == 0
 
+    @lru_cache(maxsize=None)
     async def have_identical_trees(self, ref1: GitCommitHash, ref2: GitCommitHash) -> bool:
         """
         Return whether two commit-ish have the same trees, which indicate that
         they have no diff.
         """
         tree1 = await self.git_stdout("rev-parse", f"{ref1}^{{tree}}")
         tree2 = await self.git_stdout("rev-parse", f"{ref2}^{{tree}}")
@@ -480,16 +484,16 @@
                 ret.append(result.group("branch"))
         return ret
 
     async def get_best_base_branch_candidates(
         self, commit: str, limit_to_base_branches: bool = True, allow_self: bool = True
     ) -> List[str]:
         """
-        Find the best base branch for the current HEAD by listing candidate remote branches
-        Return the branch(es) with the shortest distance from HEAD to fork-point
+        Find the best base branch for the given commit by listing candidate remote branches
+        Return the branch(es) with the shortest distance from the commit to fork-point
         """
         branches = await self.find_remote_branches(commit, limit_to_base_branches, True)
         candidates: List[Tuple[int, str]] = []
 
         if len(branches) == 1:
             return branches
 
@@ -586,15 +590,15 @@
                 commit + "~",
                 commit,
             ]
         )
         ret = (
             await self.sh.piped_sh(
                 patch_source,
-                [self.git_path, "patch-id", "--stable"],
+                [self.git_path, "patch-id", "--verbatim"],
             )
         )[1].split()
         # If the diff is empty, patch id will return nothing. We just use that as the patch-id since
         # it fulfills the requirement of matching other empty diffs.
         return ret[0] if ret else ""
 
     async def get_diff_summary(
@@ -603,92 +607,129 @@
         commit: GitCommitHash,
     ) -> str:
         """
         Return the summary of the diff (files and lines changed)
         """
         return (await self.git_stdout("diff", "--shortstat", parent, commit)).rstrip()
 
-    async def synthetic_cherry_pick(
+    async def merge_tree_commit(
         self,
-        commit_info: CommitHeader,
-        parent_tree: GitTreeHash,
-        new_parent: GitCommitHash,
-        patch_source: List[str],
+        branch1: GitCommitHash,
+        branch2: GitCommitHash,
+        new_commit_info: CommitHeader,
+        merge_base: Optional[GitCommitHash] = None,
     ) -> GitCommitHash:
         """
-        Given a patch source command and a target tree, attempt to use the "synthetic" cherry-pick
-        scheme to create a commit with the given info and a first parent of new_parent. Any
-        other parents will be kept from commit_info. Returns the commit hash of the new commit.
+        Perform a combined git merge-tree and commit-tree, returning a git commit hash. Raises
+        GitConflictException if there are conflicts while merging the trees.
         """
-        temp_index_path = self.get_scratch_dir() + "/index.temp"
-        git_env = {
-            "GIT_INDEX_FILE": temp_index_path,
-        }
-        shutil.copy(f"{self.git_dir}/index", temp_index_path)
-        await self.git("reset", "-q", "--no-refresh", parent_tree, "--", ":/", env=git_env)
-        success = not (
-            await self.sh.piped_sh(
-                patch_source,
-                [self.git_path, "apply", "--cached", "--3way", "--quiet", "--allow-empty", "-"],
-                env2=git_env,
-                raiseonerror=False,
-            )
-        )[0]
-        if success:
-            new_commit_info = copy.deepcopy(commit_info)
-            new_commit_info.tree = GitTreeHash(await self.git_stdout("write-tree", env=git_env))
-            new_commit_info.parents[0] = new_parent
+        args = ["merge-tree", "--write-tree", "--messages", "-z"]
+        if merge_base:
+            args.extend(["--merge-base", merge_base])
+        args.extend([branch1, branch2])
+
+        ret, stdout = await self.git(*args, raiseonerror=False)
+
+        # See man page for git merge-tree for a complete breakdown of the output format
+        sections = stdout.split("\0\0")
+        subsections = [s.split("\0") for s in sections]
+        tree_hash = GitTreeHash(subsections[0][0])
+
+        if ret == 0:
+            new_commit_info.tree = tree_hash
             return await self.commit_tree(new_commit_info)
+        elif ret == 1:
+            # conflicted_files would be subsections[0][1:] but we don't currently use this info
+            # (it corresponds to higher order files in cache).
+            informational = subsections[1]
+            # Information section is formatted as a list of conflicts:
+            # <num paths> <paths> <type> <message>
+            # We parse num paths first and loop through to extract the other fields.
+            e = GitConflictException(tree_hash)
+            i = 0
+            while i < len(informational) - 1:
+                num_paths = int(informational[i])
+                e.conflicts.append(
+                    GitConflict(
+                        informational[i + 1 + num_paths],
+                        informational[i + 2 + num_paths].strip(),
+                        informational[i + 1 : i + 1 + num_paths],
+                    )
+                )
+                i += num_paths + 3
+            raise e
         else:
-            conflicts = await self.ls_files(show_conflicts=True, env=git_env)
-            if not conflicts:
-                logging.info("Add / delete conflicts found!")
-                logging.info("Listing conflicting paths isn't implemented for these yet.")
-            for _, stage, path in conflicts:
-                if stage == 1:
-                    logging.info("Conflict in path {}".format(path))
-            raise GitConflictException
+            raise RuntimeError(f"Unexpected / unknown error in git merge-tree {ret}")
 
-    async def synthetic_amend(self, commit_info: CommitHeader) -> GitCommitHash:
+    async def dump_conflict(self, e: GitConflictException) -> None:
         """
-        Return a commit that contains the contents of the given commit plus the current
-        contents of the cache.
+        Dump conflict to log for informational purposes. For conflicts that have content markers,
+        Look up those sections in the result tree and dump those as well.
         """
-        patch_source = (
-            [
-                self.git_path,
-            ]
-            + GIT_DIFF_ARGS
-            + [
-                "--cached",
-            ]
-        )
-        return await self.synthetic_cherry_pick(
-            commit_info, commit_info.tree, commit_info.parents[0], patch_source
+        for conflict in e.conflicts:
+            if conflict.type == "Auto-merging":
+                # A purely informational message, doesn't indicate a conflict
+                continue
+
+            logging.error(conflict.message)
+
+            if conflict.type == "CONFLICT (contents)":
+                # Look up conflict markers in tree
+                await self.dump_conflict_markers(e.tree, conflict.paths[0])
+
+    async def dump_conflict_markers(self, tree: GitTreeHash, path: str) -> None:
+        """
+        Given a tree and file within the tree, print out all groups of conflict markers,
+        prefixed with the starting and ending line numbers.
+        """
+        groups: List[List[int]] = []
+        conflict_depth = 0
+        lines = (await self.git_stdout("show", f"{tree}:{path}")).split("\n")
+        for lineno, line in enumerate(lines):
+            if line.startswith("<" * 7):
+                if conflict_depth == 0:
+                    groups.append([lineno])
+                conflict_depth += 1
+            if line.startswith(">" * 7) and conflict_depth > 0:
+                conflict_depth -= 1
+                if conflict_depth == 0:
+                    groups[-1].append(lineno + 1)
+
+        ret = []
+        for group in groups:
+            if len(group) != 2:
+                continue
+            ret.append(f"@@ {group[0]}, {group[1]}")
+            for i in range(group[0], group[1]):
+                ret.append(lines[i])
+
+        logging.info("\n".join(ret))
+
+    async def synthetic_amend(
+        self, commit_to_amend: CommitHeader, new_commit: CommitHeader
+    ) -> GitCommitHash:
+        """
+        Return a commit that contains the contents of both commit_to_amend and new_commit
+        """
+        commit_info = copy.deepcopy(commit_to_amend)
+        return await self.merge_tree_commit(
+            new_commit.commit_id, commit_info.commit_id, commit_info, new_commit.parents[0]
         )
 
     async def synthetic_cherry_pick_from_commit(
         self, commit_info: CommitHeader, new_parent: GitCommitHash
     ) -> GitCommitHash:
         """
         Return a commit that contains the contents of the given commit on top of a new parent.
         """
-        patch_source = (
-            [
-                self.git_path,
-            ]
-            + GIT_DIFF_ARGS
-            + [
-                commit_info.commit_id + "~",
-                commit_info.commit_id,
-            ]
-        )
-
-        return await self.synthetic_cherry_pick(
-            commit_info, GitTreeHash(new_parent), new_parent, patch_source
+        commit_info = copy.deepcopy(commit_info)
+        old_parent = commit_info.parents[0]
+        commit_info.parents[0] = new_parent
+        return await self.merge_tree_commit(
+            commit_info.commit_id, new_parent, commit_info, old_parent
         )
 
     async def cherry_pick_from_tree(
         self, commit_info: CommitHeader, new_parent: GitCommitHash
     ) -> GitCommitHash:
         """
         Return a commit that uses the same tree as the given commit, but is on a new parent.
@@ -731,14 +772,18 @@
 
         # Transform diff-tree raw output to ls-files style output, taking only the new version
         for m in RE_RAW_DIFF_TREE_LINE.finditer(
             await self.git_stdout("diff-tree", "-r", "--no-commit-id", "--raw", old_base, old_head)
         ):
             new_index.append(f"{m.group('new_mode')} {m.group('new_hash')} 0\t{m.group('path')}")
 
+        if not new_index:
+            # No files were actually changed, so no diff needs to be applied to new_base
+            return new_base
+
         temp_index_path = self.get_scratch_dir() + "/index.temp"
         git_env = {
             "GIT_INDEX_FILE": temp_index_path,
         }
         shutil.copy(f"{self.git_dir}/index", temp_index_path)
         await self.git("reset", "-q", "--no-refresh", new_base, "--", ":/", env=git_env)
         await self.git(
@@ -751,7 +796,13 @@
         tree = GitTreeHash(await self.git_stdout("write-tree", env=git_env))
         new_commit_info = CommitHeader(tree, [parent] if parent else [])
         new_commit_info.commit_msg = (
             f"revup virtual diff target\n\n{old_base}\n{old_head}\n{new_base}\n{new_head}"
         )
 
         return await self.commit_tree(new_commit_info)
+
+    async def soft_reset(self, new_commit: GitCommitHash, env: Dict) -> None:
+        await self.git("reset", "--soft", new_commit, env=env)
+
+        # TODO: only strictly needs to drop entries for HEAD
+        self.clear_cache()
```

### Comparing `revup-0.1.5/revup/github_real.py` & `revup-0.2.0/revup/github_real.py`

 * *Files identical despite different names*

### Comparing `revup-0.1.5/revup/github_utils.py` & `revup-0.2.0/revup/github_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 from dataclasses import dataclass, field
 from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Set, Tuple
 
 from revup import github
 from revup.git import GitHubRepoInfo
-from revup.types import GitCommitHash
+from revup.types import GitCommitHash, RevupGithubException
 
 MAX_COMMENTS_TO_QUERY = 3
 
 
 @dataclass
 class PrComment:
     text: str = ""
@@ -378,26 +378,21 @@
             }
         )
     inputs_args = get_args_dict(inputs, "pr")
     prs_out = get_result_args(len(inputs), "pr_out")
 
     arg_str = ", ".join(get_args_declaration(inputs_args, "CreatePullRequestInput!"))
 
-    request_str = "".join(
-        len(inputs)
-        * [
-            """
+    request_str = "".join(len(inputs) * ["""
             {}: createPullRequest(input: ${}) {{
                 pullRequest {{
                     id
                     url
                 }}
-            }},"""
-        ]
-    )
+            }},"""])
     request_str = request_str.format(*zip_and_flatten(prs_out, inputs_args.keys()))
 
     mutation_str = f"""
         mutation ({arg_str}) {{
             {request_str}
         }}"""
 
@@ -527,122 +522,91 @@
         + get_args_declaration(assignees_args, "AddAssigneesToAssignableInput!")
         + get_args_declaration(to_draft_args, "ConvertPullRequestToDraftInput!")
         + get_args_declaration(from_draft_args, "MarkPullRequestReadyForReviewInput!")
         + get_args_declaration(comments_args, "AddCommentInput!")
         + get_args_declaration(edit_comments_args, "UpdateIssueCommentInput!")
     )
 
-    update_str = "".join(
-        len(inputs)
-        * [
-            """
+    update_str = "".join(len(inputs) * ["""
             {}: updatePullRequest(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     update_str = update_str.format(*zip_and_flatten(prs_out, inputs_args.keys()))
 
-    request_reviewers_str = "".join(
-        len(reviewers_args)
-        * [
-            """
+    request_reviewers_str = "".join(len(reviewers_args) * ["""
             {}: requestReviews(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     request_reviewers_str = request_reviewers_str.format(
         *zip_and_flatten(reviewers_out, reviewers_args.keys())
     )
-    assignees_str = "".join(
-        len(assignees_args)
-        * [
-            """
+    assignees_str = "".join(len(assignees_args) * ["""
             {}: addAssigneesToAssignable(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     assignees_str = assignees_str.format(*zip_and_flatten(assignees_out, assignees_args.keys()))
 
-    add_labels_str = "".join(
-        len(labels_args)
-        * [
-            """
+    add_labels_str = "".join(len(labels_args) * ["""
             {}: addLabelsToLabelable(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     add_labels_str = add_labels_str.format(*zip_and_flatten(labels_out, labels_args.keys()))
 
-    to_draft_str = "".join(
-        len(convert_to_draft)
-        * [
-            """
+    to_draft_str = "".join(len(convert_to_draft) * ["""
             {}: convertPullRequestToDraft(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     to_draft_str = to_draft_str.format(*zip_and_flatten(to_draft_out, to_draft_args.keys()))
 
-    from_draft_str = "".join(
-        len(convert_from_draft)
-        * [
-            """
+    from_draft_str = "".join(len(convert_from_draft) * ["""
             {}: markPullRequestReadyForReview(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     from_draft_str = from_draft_str.format(*zip_and_flatten(from_draft_out, from_draft_args.keys()))
 
-    add_comments_str = "".join(
-        len(comments_args)
-        * [
-            """
+    add_comments_str = "".join(len(comments_args) * ["""
             {}: addComment(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     add_comments_str = add_comments_str.format(*zip_and_flatten(comments_out, comments_args.keys()))
 
-    edit_comments_str = "".join(
-        len(edit_comments_args)
-        * [
-            """
+    edit_comments_str = "".join(len(edit_comments_args) * ["""
             {}: updateIssueComment(input: ${}) {{
                 clientMutationId
-            }},"""
-        ]
-    )
+            }},"""])
     edit_comments_str = edit_comments_str.format(
         *zip_and_flatten(edit_comments_out, edit_comments_args.keys())
     )
 
     # Have any add comment mutations first in order to ensure that comments are at the top of the PR
     mutation_str = f"""
         mutation ({arg_str}) {{
             {add_comments_str}{update_str}{request_reviewers_str}{assignees_str}{add_labels_str}{to_draft_str}{from_draft_str}{edit_comments_str}
         }}"""
 
-    await github_ep.graphql(
-        mutation_str,
-        **comments_args,
-        **inputs_args,
-        **reviewers_args,
-        **assignees_args,
-        **labels_args,
-        **to_draft_args,
-        **from_draft_args,
-        **edit_comments_args,
-    )
+    try:
+        await github_ep.graphql(
+            mutation_str,
+            **comments_args,
+            **inputs_args,
+            **reviewers_args,
+            **assignees_args,
+            **labels_args,
+            **to_draft_args,
+            **from_draft_args,
+            **edit_comments_args,
+        )
+    except RevupGithubException as e:
+        if "timeout" in e.message:
+            logging.warning(
+                "Github update request timed out! Most likely this is a false alarm and changes"
+                " actually succeeded. You may want to rerun this command to verify."
+            )
+        else:
+            raise e
 
 
 RE_PR_URL = re.compile(
     r"^https://(?P<github_url>[^/]+)/(?P<owner>[^/]+)/(?P<name>[^/]+)/pull/(?P<number>[0-9]+)/?$"
 )
```

### Comparing `revup-0.1.5/revup/logs.py` & `revup-0.2.0/revup/logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,22 @@
         self._log_render = log_render
 
 
 def configure_logger(debug: bool, redactions: Dict[str, str]) -> None:
     log_filter = RedactingFilter()
     for k, v in redactions.items():
         log_filter.redact(k, v)
-    handler = RevupRichHandler()
+    handler = RevupRichHandler(keywords=[])
     handler.addFilter(log_filter)
     handler.set_render(
         LogRender(
             show_time=False,
             show_level=True,
             show_path=False,
             level_width=1,
         )
     )
+    handler.highlighter = None  # type: ignore
 
     root_logger = logging.getLogger()
     root_logger.addHandler(handler)
     root_logger.setLevel(logging.DEBUG if debug else logging.INFO)
```

### Comparing `revup-0.1.5/revup/revup.py` & `revup-0.2.0/revup/revup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from typing import Any, AsyncGenerator, Tuple
 
 import revup
 from revup import config, git, logs, shell
 from revup.types import RevupUsageException
 
 REVUP_CONFIG_ENV_VAR = "REVUP_CONFIG_PATH"
+CONFIG_FILE_NAME = ".revupconfig"
 
 
 class HelpAction(argparse.Action):
     """
     A help action that displays a manpage formatted from the markdown documentation if available.
     """
 
@@ -69,21 +70,21 @@
         cmds = self.prog.split()
         cmd = cmds[0] if len(cmds) == 1 else cmds[1]
         for action in self._actions:
             if len(action.option_strings) > 0 and action.option_strings[0].startswith("--"):
                 option = action.option_strings[0][2:].replace("-", "_")
                 if isinstance(action, _StoreTrueAction):
                     if conf.has_option(cmd, option):
-                        override = conf.get(cmd, option)
-                        if override in ("True", "False"):
-                            action.default = override == "True"
+                        override = conf.get(cmd, option).lower()
+                        if override in ("true", "false"):
+                            action.default = override == "true"
                         else:
                             raise ValueError(
                                 f'"{override}" not a valid override for boolean flag {option}, must'
-                                ' be "True" or "False"'
+                                ' be "true" or "false"'
                             )
                 elif isinstance(action, _StoreAction):
                     if conf.has_option(cmd, option):
                         action.default = conf.get(cmd, option)
 
 
 def make_toplevel_parser() -> RevupArgParser:
@@ -100,39 +101,41 @@
     revup_parser.add_argument("--fork-name", default="")
     revup_parser.add_argument("--editor")
     revup_parser.add_argument("--verbose", "-v", action="store_true")
     revup_parser.add_argument("--keep-temp", "-k", action="store_true")
     revup_parser.add_argument("--git-path", default="")
     revup_parser.add_argument("--main-branch", default="main")
     revup_parser.add_argument("--base-branch-globs", default="")
-    revup_parser.add_argument("--git-version", default="2.36.0")
+    revup_parser.add_argument("--git-version", default="2.39.0")
     return revup_parser
 
 
-async def get_config() -> config.Config:
+def get_config_path() -> str:
     home_path = os.path.expanduser("~")
-    config_file_name = ".revupconfig"
-    config_path = os.environ.get(
-        os.path.expanduser(REVUP_CONFIG_ENV_VAR), os.path.join(home_path, config_file_name)
+    return os.environ.get(
+        os.path.expanduser(REVUP_CONFIG_ENV_VAR), os.path.join(home_path, CONFIG_FILE_NAME)
     )
 
+
+async def get_config() -> config.Config:
+    config_path = get_config_path()
     if os.path.isfile(config_path) and hasattr(os, "getuid"):
         config_stat = os.stat(config_path)
         if config_stat.st_uid != os.getuid():
             raise RevupUsageException("Config file is not owned by the current user!")
         if stat.S_IMODE(config_stat.st_mode) != 0o600:
             raise RevupUsageException(
                 f"Permissions too loose on config file!\nTry `chmod 0600 {config_path}`"
             )
 
     # There's a chicken/egg problem in getting git path from config when we need git
     # to find the path of the config file. Just this once, we use the default.
     sh = shell.Shell()
     repo_root = (await sh.sh(git.get_default_git(), "rev-parse", "--show-toplevel"))[1].rstrip()
-    conf = config.Config(config_path, os.path.join(repo_root, config_file_name))
+    conf = config.Config(config_path, os.path.join(repo_root, CONFIG_FILE_NAME))
     conf.read()
     return conf
 
 
 async def get_git(args: argparse.Namespace) -> git.Git:
     sh = shell.Shell(not args.verbose)
     git_ctx = await git.make_git(
@@ -163,41 +166,49 @@
     from revup import github_real
 
     repo_info = await git_ctx.get_github_repo_info(
         github_url=args.github_url, remote_name=args.remote_name
     )
 
     if not repo_info.owner or not repo_info.name:
-        raise RuntimeError(
-            f'Configured remote "{args.remote_name}" does not\n'
-            "point to the a github repository!\n"
-            "You can set it manually by running\n"
-            f"git remote set-url {args.remote_name} git@github.com:{{OWNER}}/{{PROJECT}}\n"
-            f"or change the configured remote in {conf.config_path}\n"
+        raise RevupUsageException(
+            f'Configured remote "{args.remote_name}" does not '
+            "point to the a github repository! "
+            "You can set it manually by running "
+            f"`git remote set-url {args.remote_name} git@github.com:{{OWNER}}/{{PROJECT}}` "
+            f"or change the configured remote in {conf.config_path}/"
         )
 
     fork_info = repo_info
     if args.fork_name and args.fork_name != args.remote_name:
         fork_info = await git_ctx.get_github_repo_info(
             github_url=args.github_url, remote_name=args.fork_name
         )
 
     if not fork_info.owner or not fork_info.name:
-        raise RuntimeError(
-            f'Configured remote fork "{args.fork_info}" does not\n'
-            "point to the a github repository!\n"
-            "You can set it manually by running\n"
-            f"git remote set-url {args.fork_info} git@github.com:{{OWNER}}/{{PROJECT}}\n"
-            f"or change the configured remote in {conf.config_path}\n"
+        raise RevupUsageException(
+            f'Configured remote fork "{args.fork_info}" does not '
+            "point to the a github repository! "
+            "You can set it manually by running "
+            f"`git remote set-url {args.fork_info} git@github.com:{{OWNER}}/{{PROJECT}}` "
+            f"or change the configured remote in {conf.config_path}."
         )
 
     if repo_info.name != fork_info.name:
-        raise RuntimeError(
-            f'Configured remote fork "{args.fork_info}" is not\n'
-            f"the same repo as the remote {args.remote_info}\n"
+        raise RevupUsageException(
+            f'Configured remote fork "{args.fork_info}" is not '
+            f"the same repo as the remote {args.remote_info}."
+        )
+
+    if not args.github_oauth:
+        raise RevupUsageException(
+            "No Github OAuth token configured! "
+            "Make one at https://github.com/settings/tokens/new "
+            "(revup needs full repo permissions) "
+            "then set it with `revup config github_oauth`."
         )
 
     github_ep = github_real.RealGitHubEndpoint(
         oauth_token=args.github_oauth, proxy=args.proxy, github_url=args.github_url
     )
     try:
         yield github_ep, repo_info, fork_info
@@ -217,21 +228,26 @@
         add_help=False,
     )
     cherry_pick_parser = subparsers.add_parser(
         "cherry-pick",
         add_help=False,
     )
     amend_parser = subparsers.add_parser("amend", aliases=["commit"], add_help=False)
+    config_parser = subparsers.add_parser(
+        "config",
+        add_help=False,
+    )
 
     for p in [upload_parser, restack_parser, amend_parser]:
         # Some args are used by both upload and restack
         p.add_argument("--help", "-h", action=HelpAction, nargs=0)
         p.add_argument("--base-branch", "-b")
         p.add_argument("--relative-branch", "-e")
 
+    upload_parser.add_argument("topics", nargs="*")
     upload_parser.add_argument("--rebase", "-r", action="store_true")
     upload_parser.add_argument("--skip-confirm", "-s", action="store_true")
     upload_parser.add_argument("--dry-run", "-d", action="store_true")
     upload_parser.add_argument("--status", "-t", action="store_true")
     upload_parser.add_argument("--update-pr-body", action="store_true", default=True)
     upload_parser.add_argument("--create-local-branches", action="store_true")
     upload_parser.add_argument("--review-graph", action="store_true", default=True)
@@ -245,14 +261,15 @@
     upload_parser.add_argument(
         "--user-aliases",
     )
     upload_parser.add_argument("--uploader")
     upload_parser.add_argument("--pre-upload", "-p")
     upload_parser.add_argument("--relative-chain", "-c", action="store_true")
     upload_parser.add_argument("--auto-topic", "-a", action="store_true")
+    upload_parser.add_argument("--head", default="HEAD")
 
     restack_parser.add_argument("--topicless-last", "-t", action="store_true")
 
     amend_parser.add_argument("ref_or_topic", nargs="?")
     amend_parser.add_argument("--no-edit", "--skip-reword", "-s", action="store_true")
     amend_parser.add_argument("--insert", "-i", action="store_true")
     amend_parser.add_argument("--drop", "-d", action="store_true")
@@ -261,14 +278,19 @@
     amend_parser.add_argument("--parse-topics", default=True, action="store_true")
     amend_parser.add_argument("--parse-refs", default=True, action="store_true")
 
     cherry_pick_parser.add_argument("--help", "-h", action=HelpAction, nargs=0)
     cherry_pick_parser.add_argument("branch", nargs=1)
     cherry_pick_parser.add_argument("--base-branch", "-b")
 
+    config_parser.add_argument("--help", "-h", action=HelpAction, nargs=0)
+    config_parser.add_argument("flag", nargs=1)
+    config_parser.add_argument("value", nargs="?")
+    config_parser.add_argument("--repo", "-r", action="store_true")
+
     toolkit_parser = subparsers.add_parser(
         "toolkit", description="Test various subfunctionalities."
     )
     toolkit_subparsers = toolkit_parser.add_subparsers(dest="toolkit_cmd", required=True)
     detect_branch = toolkit_subparsers.add_parser(
         "detect-branch", description="Detect the base branch of the current branch."
     )
@@ -314,17 +336,23 @@
 
     for p in [revup_parser, amend_parser, cherry_pick_parser, restack_parser, upload_parser]:
         assert isinstance(p, RevupArgParser)
         p.set_defaults_from_config(conf.get_config())
     args = revup_parser.parse_args()
 
     # So users don't accidentally leak their oauth when sharing logs
-    logs.configure_logger(debug=args.verbose, redactions={args.github_oauth: "<GITHUB_OAUTH>"})
+    logs.configure_logger(
+        debug=args.verbose,
+        redactions={args.github_oauth: "<GITHUB_OAUTH>"} if args.github_oauth else {},
+    )
     dump_args(args)
 
+    if args.cmd == "config":
+        return config.config_main(conf, args)
+
     git_ctx = await get_git(args)
 
     if args.cmd == "toolkit":
         from revup import toolkit
 
         return await toolkit.main(args=args, git_ctx=git_ctx)
```

### Comparing `revup-0.1.5/revup/shell.py` & `revup-0.2.0/revup/shell.py`

 * *Files identical despite different names*

### Comparing `revup-0.1.5/revup/toolkit.py` & `revup-0.2.0/revup/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     elif args.toolkit_cmd == "diff-target":
         await asyncio.gather(
             git_ctx.verify_branch_or_commit(args.old_head),
             git_ctx.verify_branch_or_commit(args.new_head),
         )
 
         if not args.old_base:
-            args.old_base = git_ctx.to_commit_hash(args.old_head + "~")
+            args.old_base = await git_ctx.to_commit_hash(args.old_head + "~")
         if not args.new_base:
-            args.new_base = git_ctx.to_commit_hash(args.new_head + "~")
+            args.new_base = await git_ctx.to_commit_hash(args.new_head + "~")
         logging.info(
             await git_ctx.make_virtual_diff_target(
                 args.old_base, args.old_head, args.new_base, args.new_head, args.parent
             )
         )
     elif args.toolkit_cmd == "fork-point":
         await asyncio.gather(
```

### Comparing `revup-0.1.5/revup/topic_stack.py` & `revup-0.2.0/revup/topic_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 import logging
 import re
 import subprocess
 from collections import defaultdict
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
@@ -17,14 +18,20 @@
 from revup.types import (
     GitCommitHash,
     GitConflictException,
     RevupConflictException,
     RevupUsageException,
 )
 
+# Since topic name is incorporated into the branch name, we must ensure that it matches
+# the character set that github supports. It's possible to have other characters if they're
+# properly escaped but we don't want to deal with that for now.
+# https://docs.github.com/en/get-started/using-git/dealing-with-special-characters-in-branch-and-tag-names
+RE_BRANCH_ALLOWED = re.compile(r"^[\w\d_\.\/-]+$")
+
 
 def format_remote_branch(uploader: str, base_branch: str, topic: str) -> str:
     """
     Branches are named so that it is clear that they are made by revup
     and can be force pushed at any time, and to minimize collision with
     manually created branches.
     """
@@ -189,14 +196,17 @@
     relative_branch: str
 
     # Github access info
     github_ep: Optional[github.GitHubEndpoint] = None
     repo_info: Optional[github_utils.GitHubRepoInfo] = None
     fork_info: Optional[github_utils.GitHubRepoInfo] = None
 
+    # Commit at the head of the branch to be uploaded
+    head: str = "HEAD"
+
     # Original list of relevant commits given to the submitter
     commits: List[git.CommitHeader] = field(default_factory=list)
 
     # Topic names to topic info
     topics: Dict[str, Topic] = field(default_factory=dict)
 
     # Github node id of the repo
@@ -338,50 +348,55 @@
         )
         return PrComment(ret, orig.id if orig else None)
 
     async def populate_topics(
         self,
         auto_topic: bool = False,
         trim_tags: bool = False,
+        raise_on_invalid: bool = False,
     ) -> None:
         """
         Parse all commits and sort them into individual topics.
         """
         if self.populated:
             return
+        if self.head != "HEAD":
+            await self.git_ctx.verify_branch_or_commit(self.head)
         if self.base_branch:
             self.base_branch = self.git_ctx.ensure_branch_prefix(self.base_branch)
             await self.git_ctx.verify_branch_or_commit(self.base_branch)
         else:
             # Base branch can be autodetected if not specified
-            self.base_branch = await self.git_ctx.get_best_base_branch("HEAD", True)
+            self.base_branch = await self.git_ctx.get_best_base_branch(self.head, True)
 
         if self.relative_branch:
             self.relative_branch = self.git_ctx.ensure_branch_prefix(self.relative_branch)
             await self.git_ctx.verify_branch_or_commit(self.relative_branch)
         else:
             # If relative branch is not specified, its just the base branch
             self.relative_branch = self.base_branch
 
-        branch_point = await self.git_ctx.fork_point("HEAD", self.relative_branch)
+        branch_point = await self.git_ctx.fork_point(self.head, self.relative_branch)
         if self.base_branch != self.relative_branch:
-            base_branch_point = await self.git_ctx.fork_point("HEAD", self.base_branch)
-            if not await self.git_ctx.is_ancestor(base_branch_point, branch_point):
-                # Our model expects relative branch to be forked off base branch, and HEAD
+            base_branch_point = await self.git_ctx.fork_point(self.head, self.base_branch)
+            if raise_on_invalid and not await self.git_ctx.is_ancestor(
+                base_branch_point, branch_point
+            ):
+                # Our model expects relative branch to be forked off base branch, and head
                 # to be forked off relative branch.
                 raise RevupUsageException(
-                    "Relative branch structure is invalid: HEAD is closer to"
+                    f"Relative branch structure is invalid: {self.head} is closer to"
                     f" {self.base_branch} than {self.relative_branch}."
                     f"Specifically we expect the fork point with {self.base_branch} "
                     f"({base_branch_point}) to be an ancestor of the fork point with "
                     f"{self.relative_branch} ({branch_point})."
                 )
 
         self.commits = git.parse_rev_list(
-            await self.git_ctx.rev_list("HEAD", branch_point, header=True, first_parent=True)
+            await self.git_ctx.rev_list(self.head, branch_point, header=True, first_parent=True)
         )
 
         # Parse tags and add each commit to appropriate topics
         for c in self.commits:
             parsed_tags, trimmed_msg = self.parse_commit_tags(c.commit_msg)
             if not parsed_tags[TAG_TOPIC]:
                 if auto_topic:
@@ -391,43 +406,53 @@
                         ).translate({ord(":"): None, ord("["): None, ord("]"): None})
                     )
                 else:
                     # No topic tags, not a revup commit
                     continue
 
             if len(parsed_tags[TAG_TOPIC]) > 1:
-                raise RevupUsageException(
-                    f"Can't specify more than one topic for a commit!\n\n{c.commit_msg}"
-                )
+                if raise_on_invalid:
+                    raise RevupUsageException(
+                        f"Can't specify more than one topic for a commit!\n\n{c.commit_msg}"
+                    )
             else:
                 if trim_tags:
                     c.commit_msg = trimmed_msg
                 name = min(parsed_tags[TAG_TOPIC])
+                if raise_on_invalid and not RE_BRANCH_ALLOWED.match(name):
+                    raise RevupUsageException(f"Invalid characters in topic name '{name}'")
                 if name not in self.topics:
                     self.topics[name] = Topic(name)
                 self.topics[name].original_commits.append(c)
                 add_tags(self.topics[name].tags, parsed_tags)
         self.populated = True
 
     async def populate_reviews(
         self,
         uploader: str,
         force_relative_chain: bool = False,
-        labels: str = None,
+        labels: Optional[str] = None,
         user_aliases: str = "",
         auto_add_users: str = "",
         self_authored_only: bool = False,
+        limit_topics: Optional[List[str]] = None,
     ) -> None:
         """
         Populate reviews for already-parsed topics. Verify base branch and relative topic info to
         ensure it is valid.
         """
         seen_topics: Dict[str, Topic] = {}
         for name, topic in list(self.topics.items()):
-            relative_topic = ""
+            if limit_topics:
+                if name not in limit_topics:
+                    # If an explicit list was specified, don't upload other topics
+                    del self.topics[name]
+                    continue
+                # Disable the self authored check if this topic was explicitly given
+                self_authored_only = False
 
             if self_authored_only:
                 # Don't upload if this topic doesn't have commits authored by the current user
                 # Do this early so we don't throw errors for changes that won't be uploaded
                 has_self_authored = False
                 for c in topic.original_commits:
                     if c.author_email.lower() == self.git_ctx.email:
@@ -439,14 +464,15 @@
                     )
                     del self.topics[name]
                     continue
 
             if len(topic.tags[TAG_UPLOADER]) > 1:
                 raise RevupUsageException(f"Can't specify more than one uploader for topic {name}!")
 
+            relative_topic = ""
             if force_relative_chain and seen_topics:
                 relative_topic = list(seen_topics)[-1]
             elif len(topic.tags[TAG_RELATIVE]) > 1:
                 raise RevupUsageException(
                     "Can't specify more than 1 relative topic per topic! Got"
                     f" {topic.tags[TAG_RELATIVE]} for topic {name}"
                 )
@@ -605,14 +631,19 @@
             if auto_add_users in ("r2a", "both"):
                 topic.tags[TAG_ASSIGNEE].update(topic.tags[TAG_REVIEWER])
             if auto_add_users in ("a2r", "both"):
                 topic.tags[TAG_REVIEWER].update(topic.tags[TAG_ASSIGNEE])
 
             seen_topics[name] = topic
 
+        if limit_topics:
+            for name in limit_topics:
+                if name not in self.topics:
+                    logging.warning(f"Couldn't find any topic named {name}")
+
     async def mark_rebases(self, skip_rebase: bool) -> None:
         """
         Scan all topics and compare patch-ids to remote patch-ids. Appropriately mark any
         changes that are already merged, or where push can be skipped due to being rebases or
         being identical.
         """
         for _, topic, base_branch, review in self.all_reviews_iter():
@@ -662,32 +693,30 @@
 
             if review.pr_info is None:
                 # This is a new pr, no need to check patch ids
                 review.is_pure_rebase = False
             else:
                 if not topic.patch_ids:
                     # Lazily load patch ids for the topic.
-                    # TODO async gather to generate patch ids in parallel
-                    topic.patch_ids = [
-                        await self.git_ctx.get_patch_id(c.commit_id) for c in topic.original_commits
-                    ]
+                    topic.patch_ids = await asyncio.gather(
+                        *(self.git_ctx.get_patch_id(c.commit_id) for c in topic.original_commits)
+                    )
 
                 review.remote_commits = git.parse_rev_list(
                     await self.git_ctx.rev_list(
                         review.pr_info.headRefOid,
                         review.pr_info.baseRefOid,
                         header=True,
                         first_parent=True,
                     )
                 )
 
-                # TODO async gather to generate patch ids in parallel
-                review.remote_patch_ids = [
-                    await self.git_ctx.get_patch_id(c.commit_id) for c in review.remote_commits
-                ]
+                review.remote_patch_ids = await asyncio.gather(
+                    *(self.git_ctx.get_patch_id(c.commit_id) for c in review.remote_commits)
+                )
 
                 # This review is a rebase iff all commit diffs match
                 is_rebase = len(review.remote_commits) == len(topic.original_commits) and all(
                     local_id == remote_id
                     for local_id, remote_id in zip(topic.patch_ids, review.remote_patch_ids)
                 )
                 # This review is a "complete rebase" iff all commit diffs and metadata match
@@ -715,41 +744,58 @@
                     else:
                         # TODO: We can do more optimization by reusing the remote trees.
                         # We wouldn't benefit as much from skipping the push, but we'd save time
                         # on creating commits.
                         pass
 
             if review.is_pure_rebase and review.pr_info is not None:
-                # For a relative series of reviews, revup will only ever upload them directly
-                # on top of each other. If this relationship is ever broken, we always reupload
-                # This ensures predictable and consistent CI behavior between the branches.
-                is_on_top_of_relative = (
-                    topic.relative_topic is None
-                    or topic.relative_topic.reviews[base_branch].pr_info is None
-                    or review.remote_commits[0].parents[0]
-                    == topic.relative_topic.reviews[base_branch].remote_commits[-1].commit_id
-                )
+                if topic.relative_topic is None:
+                    if not review.base_ref:
+                        raise RuntimeError("Review doesn't have a base ref!")
+                    # For non-relative reviews, the base is correct if the remote base commit is a
+                    # first-parent ancestor of the local remote base.
+                    is_on_correct_base = await self.git_ctx.is_ancestor(
+                        review.remote_commits[0].parents[0], review.base_ref
+                    )
+                else:
+                    # For a relative series of reviews, revup will only ever upload them directly
+                    # on top of each other. If this relationship is ever broken, we always reupload
+                    # This ensures predictable and consistent CI behavior between the branches.
+                    is_on_correct_base = (
+                        topic.relative_topic.reviews[base_branch].pr_info is None
+                        or review.remote_commits[0].parents[0]
+                        == topic.relative_topic.reviews[base_branch].remote_commits[-1].commit_id
+                    )
 
                 relative_topic_is_nochange = (
                     topic.relative_topic is not None
                     and topic.relative_topic.reviews[base_branch].push_status == PushStatus.NOCHANGE
                 )
                 relative_topic_is_skippable = (
                     topic.relative_topic is None
                     or topic.relative_topic.reviews[base_branch].push_status != PushStatus.PUSHED
                 )
+                logging.debug(
+                    "Review {}/{} is correct base {} relative nochange {} skippable {}".format(
+                        base_branch,
+                        topic.name,
+                        is_on_correct_base,
+                        relative_topic_is_nochange,
+                        relative_topic_is_skippable,
+                    )
+                )
 
                 if review.base_ref == review.remote_commits[0].parents[0] or (
-                    relative_topic_is_nochange and is_on_top_of_relative
+                    relative_topic_is_nochange and is_on_correct_base
                 ):
                     # This is a rebase and the parent is the same, so there must be no change.
                     # Alternatively, it is relative to a topic with no change.
                     review.push_status = PushStatus.NOCHANGE
                 elif review.status == PrStatus.MERGED or (
-                    skip_rebase and is_on_top_of_relative and relative_topic_is_skippable
+                    skip_rebase and is_on_correct_base and relative_topic_is_skippable
                 ):
                     # Never push merged changes.
                     # Also don't push if the user asked to skip pushing rebases, but only if the
                     # relative base is correct and relative topic won't be pushed.
                     review.push_status = PushStatus.REBASE
 
                 if review.push_status == PushStatus.NOCHANGE:
@@ -826,23 +872,27 @@
                         next_parent = await self.git_ctx.synthetic_cherry_pick_from_commit(
                             commit, next_parent
                         )
                     except GitConflictException as exc:
                         parent_info = (
                             "the same topic"
                             if next_parent != review.base_ref
-                            else f'relative topic "{topic.relative_topic.name}"'
-                            if topic.relative_topic
-                            else f'base branch "{base_branch}"'
+                            else (
+                                f'relative topic "{topic.relative_topic.name}"'
+                                if topic.relative_topic
+                                else f'base branch "{base_branch}"'
+                            )
                         )
+                        await self.git_ctx.dump_conflict(exc)
                         raise RevupConflictException(
-                            "Failed to cherry-pick commit:\n"
-                            f'"{commit.title}" ({commit.commit_id[:8]}) in topic "{name}"\n'
-                            f"to new parent ({next_parent[:8]}) in {parent_info}\n\n"
-                            "You must specify relative branches to prevent this conflict!"
+                            commit,
+                            next_parent,
+                            "You must specify relative branches to prevent this conflict!",
+                            f' in topic "{name}"',
+                            f" in {parent_info}",
                         ) from exc
                     review.new_commits.append(next_parent)
 
             if review.pr_info is not None and review.pr_info.headRefOid == review.new_commits[-1]:
                 # There are a few cases where we might not know a review is no change until after
                 # creating commits:
                 # 1. The relative PR was closed without merging after being uploaded. We don't look
@@ -868,15 +918,15 @@
         switching to a different machine.
         """
         if not self.github_ep or not self.repo_info:
             raise RuntimeError("Can't fetch without github info")
 
         to_fetch = set()
         for _, _, _, review in self.all_reviews_iter():
-            if review.pr_info is not None and not await self.git_ctx.commit_exists(
+            if review.pr_info is not None and not await self.git_ctx.is_branch_or_commit(
                 review.pr_info.headRefOid
             ):
                 to_fetch.add(review.pr_info.headRefOid)
 
         if to_fetch:
             fetch_args = [
                 "fetch",
@@ -928,14 +978,16 @@
             ]
             await self.git_ctx.git(*push_args, stderr=subprocess.PIPE)
 
     async def query_github(self) -> None:
         """
         Query pr and reviewer/label info from github
         """
+        if not self.topics:
+            return
         if not self.github_ep or not self.repo_info:
             raise RuntimeError("Can't query without github info")
 
         pr_targets = []
         user_ids = set()
         labels = set()
         for _, topic, base_branch, review in self.all_reviews_iter():
@@ -982,20 +1034,17 @@
     def populate_update_info(
         self,
         update_pr_body: bool,
     ) -> None:
         """
         Populate information necessary to do PR creation / update in github.
         """
-        if (
-            not self.repo_id
-            or self.names_to_ids is None
-            or self.names_to_logins is None
-            or self.labels_to_ids is None
-        ):
+        if not self.topics:
+            return
+        if self.names_to_ids is None or self.names_to_logins is None or self.labels_to_ids is None:
             raise RuntimeError("Need to query before updating")
 
         for topic in self.topics.values():
             commit_msg_lines = topic.original_commits[0].commit_msg.split("\n")
             body = "\n".join(commit_msg_lines[1:]).strip()
             title = commit_msg_lines[0]
             for branch, review in topic.reviews.items():
@@ -1138,25 +1187,29 @@
                 review.patchsets_index is None
                 or not review.pr_info
                 or review.status == PrStatus.MERGED
             ):
                 continue
             patchsets_comment = await self.create_patchsets_comment(
                 review,
-                review.pr_info.comments[review.patchsets_index]
-                if len(review.pr_info.comments) > review.patchsets_index
-                else None,
+                (
+                    review.pr_info.comments[review.patchsets_index]
+                    if len(review.pr_info.comments) > review.patchsets_index
+                    else None
+                ),
             )
             if patchsets_comment:
                 review.pr_update.comments.append(patchsets_comment)
 
     async def create_prs(self) -> None:
         """
         Actually perform the github graphql PR creation
         """
+        if not self.topics:
+            return
         if not self.github_ep or not self.repo_info or not self.fork_info or not self.repo_id:
             raise RuntimeError("Can't update without github info")
 
         prs_to_create = []
         for _, _, _, review in self.all_reviews_iter():
             if review.status == PrStatus.NEW and review.pr_info is not None:
                 prs_to_create.append(review.pr_info)
@@ -1168,14 +1221,16 @@
                 self.github_ep, self.repo_id, self.repo_info, self.fork_info, prs_to_create
             )
 
     async def update_prs(self) -> None:
         """
         Actually perform the github graphql PR updates
         """
+        if not self.topics:
+            return
         if not self.github_ep or not self.repo_info or not self.fork_info or not self.repo_id:
             raise RuntimeError("Can't update without github info")
 
         prs_to_update = []
         for _, _, _, review in self.all_reviews_iter():
             if not review.pr_info:
                 continue
@@ -1228,24 +1283,24 @@
             to_restack = no_topic + to_pick
         for commit in to_restack:
             try:
                 new_parent = await self.git_ctx.synthetic_cherry_pick_from_commit(
                     commit, new_parent
                 )
             except GitConflictException as exc:
+                await self.git_ctx.dump_conflict(exc)
                 raise RevupConflictException(
-                    "Failed to cherry-pick commit:\n"
-                    f'"{commit.title}" ({commit.commit_id[:8]})\n'
-                    f"to new parent ({new_parent[:8]})\n\n"
-                    f"You may need to `git rebase -i {new_parent[:8]}` to resolve these conflicts!"
+                    commit,
+                    new_parent,
+                    "You may need to `git rebase -i` to resolve these conflicts!",
                 ) from exc
         git_env = {
             "GIT_REFLOG_ACTION": "reset --soft (revup restack)",
         }
-        await self.git_ctx.git("reset", "--soft", new_parent, env=git_env)
+        await self.git_ctx.soft_reset(new_parent, git_env)
         return new_parent
 
     def num_reviews_changed(self) -> int:
         """
         Return the number of reviews that require some action (push / create / update).
         This is similar to the logic that hides reviews in print() but different in some cases,
         for example we take no action for merged prs but still print them out.
@@ -1290,16 +1345,17 @@
                     )
                 maybe_relative_branch = ""
                 if review.relative_branch:
                     maybe_relative_branch = f"[bold magenta]{review.relative_branch}[/] → "
                 maybe_draft = " (draft)" if review.is_draft else ""
 
                 get_console().print(
-                    f"[green]Topic:[/] [bold cyan]{name}[/]{maybe_draft} → "
-                    f"{maybe_relative_topic}{maybe_relative_branch}[bold red]{base}[/]"
+                    f"[green]Topic:[/] [bold cyan]{name}[/]{maybe_draft} →"
+                    f" {maybe_relative_topic}{maybe_relative_branch}[bold"
+                    f" red]{self.git_ctx.remove_branch_prefix(base)}[/]"
                 )
                 logging.debug(f"Base rev: {review.base_ref}")
                 if review.new_commits:
                     logging.debug(f"New head: {review.new_commits[-1]}")
 
                 reviewers = topic.tags[TAG_REVIEWER]
                 assignees = topic.tags[TAG_ASSIGNEE]
```

### Comparing `revup-0.1.5/revup/upload.py` & `revup-0.2.0/revup/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import argparse
-import logging
 import subprocess
 from typing import Optional
 
 from rich import get_console
 
 from revup import git, github, github_utils, topic_stack
-from revup.types import GitConflictException, RevupShellException
+from revup.types import RevupShellException
 
 
 async def main(
     args: argparse.Namespace,
     git_ctx: git.Git,
     github_ep: Optional[github.GitHubEndpoint] = None,
     repo_info: Optional[github_utils.GitHubRepoInfo] = None,
@@ -22,27 +21,30 @@
     topics = topic_stack.TopicStack(
         git_ctx,
         args.base_branch,
         args.relative_branch,
         github_ep,
         repo_info,
         fork_info,
+        args.head,
     )
     with get_console().status("Finding topics…"):
         await topics.populate_topics(
             auto_topic=args.auto_topic,
             trim_tags=args.trim_tags,
+            raise_on_invalid=True,
         )
         await topics.populate_reviews(
             args.uploader if args.uploader else git_ctx.author,
             force_relative_chain=args.relative_chain,
             labels=args.labels,
             user_aliases=args.user_aliases,
             auto_add_users=args.auto_add_users,
             self_authored_only=args.self_authored_only,
+            limit_topics=args.topics,
         )
 
     if not args.dry_run:
         with get_console().status("Querying github…"):
             await topics.query_github()
             # Fetch uses the oid results from the query
             await topics.fetch_git_refs()
@@ -52,22 +54,17 @@
 
     if args.status or args.verbose:
         topics.print(skip_empty=False)
 
     if args.status:
         return 0
 
-    try:
-        with get_console().status("Creating commits…"):
-            # Need to know rebase information before creating commits
-            await topics.create_commits(args.trim_tags)
-    except GitConflictException as e:
-        logging.error(str(e))
-        logging.error("You need to specify relative topics to prevent this conflict.")
-        return 1
+    with get_console().status("Creating commits…"):
+        # Need to know rebase information before creating commits
+        await topics.create_commits(args.trim_tags)
 
     if args.dry_run:
         topics.print(not args.verbose)
         return 0
 
     topics.populate_update_info(args.update_pr_body)
     if not args.skip_confirm and topics.num_reviews_changed() > 0:
```

### Comparing `revup-0.1.5/revup.egg-info/PKG-INFO` & `revup-0.2.0/revup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revup
-Version: 0.1.5
+Version: 0.2.0
 Summary: Revolutionary github tools. Effortlessly create multiple branches and pull requests.
 Home-page: https://github.com/skydio/revup
 Author: Jerry Zhang
 Author-email: jerry@skydio.com
 License: MIT
 Project-URL: Source, https://github.com/skydio/revup
 Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
@@ -28,30 +28,30 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <p align="center">
 
-  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/revup_light.svg"/>
+  <img alt="Revup" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/revup_light.svg"/>
 
 </p>
 
 <p align="center">
 <a href="https://github.com/Skydio/revup"><img alt="Source Code" src="https://img.shields.io/badge/source-code-blue"/></a>
 <a href="https://github.com/Skydio/revup/issues"><img alt="Issues" src="https://img.shields.io/badge/issue-tracker-blue"/></a>
 <img alt="Python 3.8 | 3.9 | 3.10" src="https://img.shields.io/pypi/pyversions/revup"/>
 <a href="https://pypi.org/project/revup/"><img alt="PyPI" src="https://img.shields.io/pypi/v/revup"/></a>
 <a href="https://github.com/Skydio/revup/tree/main/LICENSE"><img alt="MIT License" src="https://img.shields.io/pypi/l/revup"/></a>
 </p>
 
 Revup provides command-line tools that allow developers to iterate faster on parallel changes and reduce the overhead of creating and maintaining code reviews.
 
 <p align="center">
-<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_1.gif"/>
+<img alt="intro_gif" src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif"/>
 </p>
 
 # Features
 
 - Revup creates multiple independent chains of branches for you in the background and without touching your working tree. It then creates and manages github pull requests for all those branches.
 - Pull requests target the actual base branch and can be merged manually or by continuous integration
 - Rebase detection saves time and continuous integration cost by not re-pushing if the patch hasn't changed
@@ -116,34 +116,34 @@
 git commit -m "My first revup foo" -m "Topic: foo"
 echo peh > bar; git add bar
 git commit -m "My first revup bar" -m "Topic: bar"
 
 revup upload
 ```
 
-![tutorial_1](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_1.gif)
+![tutorial_1](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_1.gif)
 
 You've uploaded your first revup changes! Notice how in github, both branches target 'main'. This allows them to be merged independently.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/bar_github.png" width="50%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/foo_github.png" width="50%"><img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/bar_github.png" width="50%">
 
 Under the hood, revup creates and pushes these branches for you, tracking and managing the dependencies as needed.
 
 ## Create relative pull requests
 
 Now we'll make a new review that's relative to "foo". The "Relative" tag will ensure the new review targets the correct branch.
 
 ```sh
 echo deh >> foo; git add foo
 git commit -m "My second revup foo" -m "Topic: foo2" -m "Relative: foo"
 
 revup upload
 ```
 
-![tutorial_2](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_2.gif)
+![tutorial_2](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif)
 
 With this simple but powerful model, you can upload independent and dependent changes all at once.
 
 - Multiple commits can be in one topic, in which case they will all be in a single pull request.
 - Commits in the same topic do not need to be adjacent in history.
 - Topics relative to each other do not need to be adjacent in history, but the second topic must come after the first.
 
@@ -157,15 +157,15 @@
 revup amend HEAD~ --no-edit  # Specify a commit to amend
 # or
 revup amend bar --no-edit  # Specify a topic name to amend
 
 revup upload
 ```
 
-![tutorial_3](https://raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_3.gif)
+![tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_3.gif)
 
 `revup amend` makes it easy to modify commits in your history. You also have other options for modifying reviews:
 
 - Adding new commits with the same topic
 - Using `git rebase --interactive` along with `git commit --amend`
 
 ## Pulling in upstream changes
@@ -238,19 +238,19 @@
 revup upload --base-branch custom-branch-name
 ```
 
 ## Review graph and patchsets
 
 Revup will add 2 comments in every pull request to provide helpful features for users and reviewers. These are enabled by default and automatically updated as the pull request changes.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/review_graph.png" width="40%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/review_graph.png" width="40%">
 
 The review graph provides links and titles to all local pull requests that have a relative relationship with the current pull request, including any that it depends on, or that depend on it. This allows you to quickly browse between pull requests in a chain.
 
-<img src="https://raw.githubusercontent.com/skydio/revup/main/docs/images/patchsets.png" width="80%">
+<img src="https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png" width="80%">
 
 The patchsets table provides a history of uploads for a given pull request as well as links and summaries of the diff between each upload. Notably, revup specially handles
 the case where you rebase then upload and will show you a diff with upstream files excluded.
 
 # Configuring revup
 
 Revup is highly configurable using a standard config file format. Every flag is also a config option, so users can get the exact behavior they need.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: revup Version: 0.1.5 Summary: Revolutionary github
+Metadata-Version: 2.1 Name: revup Version: 0.2.0 Summary: Revolutionary github
 tools. Effortlessly create multiple branches and pull requests. Home-page:
 https://github.com/skydio/revup Author: Jerry Zhang Author-email:
 jerry@skydio.com License: MIT Project-URL: Source, https://github.com/skydio/
 revup Project-URL: Bug Tracker, https://github.com/skydio/revup/issues
 Keywords: github python git workflow version-control python3 developer-tools
 code-review pull-requests developers developer-productivity stacked-diffs
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -51,41 +51,41 @@
 permissions". Revup needs this in order to create and modify pull requests. ##
 Create independent pull requests Make your first two commits that will become
 two separate pull requests. Note the "Topic:" tag in the commit message - this
 is what causes revup to recognize and act on a commit. Each separately named
 topic will become a new pull request. ```sh echo meh > foo; git add foo git
 commit -m "My first revup foo" -m "Topic: foo" echo peh > bar; git add bar git
 commit -m "My first revup bar" -m "Topic: bar" revup upload ``` ![tutorial_1]
-(https://raw.githubusercontent.com/skydio/revup/main/docs/images/
+(https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
 tutorial_1.gif) You've uploaded your first revup changes! Notice how in github,
 both branches target 'main'. This allows them to be merged independently.
-[https://raw.githubusercontent.com/skydio/revup/main/docs/images/
-foo_github.png][https://raw.githubusercontent.com/skydio/revup/main/docs/
+[https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
+foo_github.png][https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
 images/bar_github.png] Under the hood, revup creates and pushes these branches
 for you, tracking and managing the dependencies as needed. ## Create relative
 pull requests Now we'll make a new review that's relative to "foo". The
 "Relative" tag will ensure the new review targets the correct branch. ```sh
 echo deh >> foo; git add foo git commit -m "My second revup foo" -m "Topic:
 foo2" -m "Relative: foo" revup upload ``` ![tutorial_2](https://
-raw.githubusercontent.com/skydio/revup/main/docs/images/tutorial_2.gif) With
+raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/tutorial_2.gif) With
 this simple but powerful model, you can upload independent and dependent
 changes all at once. - Multiple commits can be in one topic, in which case they
 will all be in a single pull request. - Commits in the same topic do not need
 to be adjacent in history. - Topics relative to each other do not need to be
 adjacent in history, but the second topic must come after the first. ## Modify
 pull requests Now let's update a pull request. ```sh echo heh >> bar; git add
 bar # Either revup amend HEAD~ --no-edit # Specify a commit to amend # or revup
 amend bar --no-edit # Specify a topic name to amend revup upload ``` !
-[tutorial_3](https://raw.githubusercontent.com/skydio/revup/main/docs/images/
-tutorial_3.gif) `revup amend` makes it easy to modify commits in your history.
-You also have other options for modifying reviews: - Adding new commits with
-the same topic - Using `git rebase --interactive` along with `git commit --
-amend` ## Pulling in upstream changes Use `git pull --rebase` to pull in
-changes. Don't use `git merge` or `git pull` without rebase as this creates a
-merge commit. By default revup will not upload if you pull but haven't made
+[tutorial_3](https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/
+images/tutorial_3.gif) `revup amend` makes it easy to modify commits in your
+history. You also have other options for modifying reviews: - Adding new
+commits with the same topic - Using `git rebase --interactive` along with `git
+commit --amend` ## Pulling in upstream changes Use `git pull --rebase` to pull
+in changes. Don't use `git merge` or `git pull` without rebase as this creates
+a merge commit. By default revup will not upload if you pull but haven't made
 changes to a commit. To override this and upload always, run `revup upload --
 rebase`. ``` [pull] rebase = true [rebase] autoStash = true ``` We recommend
 adding the above to `.gitconfig` to make pulling and rebasing easier. # More
 features This is a non-exhaustive intro to some more handy revup features. For
 a full description of features, see the [docs](https://github.com/Skydio/revup/
 tree/main/docs) or run `revup -h` or `revup upload -h` to view docs in `man`
 format. ## Work with forks For contributing to projects that you may not have
@@ -110,20 +110,20 @@
 latter case). ``` A fix for multiple branches Topic: fix Branches: main, rel1.1
 ``` You can specify base branch on the command line as well, although this is
 usually not necessary unless you're working on a branch that the autodetector
 doesn't know about (see Repo config below). ``` revup upload --base-branch
 custom-branch-name ``` ## Review graph and patchsets Revup will add 2 comments
 in every pull request to provide helpful features for users and reviewers.
 These are enabled by default and automatically updated as the pull request
-changes. [https://raw.githubusercontent.com/skydio/revup/main/docs/images/
+changes. [https://raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/
 review_graph.png] The review graph provides links and titles to all local pull
 requests that have a relative relationship with the current pull request,
 including any that it depends on, or that depend on it. This allows you to
 quickly browse between pull requests in a chain. [https://
-raw.githubusercontent.com/skydio/revup/main/docs/images/patchsets.png] The
+raw.githubusercontent.com/skydio/revup/d50fc1f/docs/images/patchsets.png] The
 patchsets table provides a history of uploads for a given pull request as well
 as links and summaries of the diff between each upload. Notably, revup
 specially handles the case where you rebase then upload and will show you a
 diff with upstream files excluded. # Configuring revup Revup is highly
 configurable using a standard config file format. Every flag is also a config
 option, so users can get the exact behavior they need. Flags specified on the
 command line take precedence, followed by config in `~/.revupconfig`, followed
```

### Comparing `revup-0.1.5/revup.egg-info/SOURCES.txt` & `revup-0.2.0/revup.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,18 @@
 ./revup/shell.py
 ./revup/toolkit.py
 ./revup/topic_stack.py
 ./revup/types.py
 ./revup/upload.py
 ./revup/man1/amend.1.gz
 ./revup/man1/cherry-pick.1.gz
+./revup/man1/config.1.gz
 ./revup/man1/restack.1.gz
 ./revup/man1/revup.1.gz
 ./revup/man1/upload.1.gz
 revup.egg-info/PKG-INFO
 revup.egg-info/SOURCES.txt
 revup.egg-info/dependency_links.txt
 revup.egg-info/entry_points.txt
 revup.egg-info/requires.txt
-revup.egg-info/top_level.txt
+revup.egg-info/top_level.txt
+tests/test_tools.py
```

### Comparing `revup-0.1.5/setup.cfg` & `revup-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 package_dir = 
 	= .
 packages = 
 	revup
 python_requires = >=3.8
 install_requires = 
 	aiohttp
+	async_lru
 	rich
 setup_requires = 
 	setuptools
 	wheel
 	pip
 include_package_data = True
```

### Comparing `revup-0.1.5/setup.py` & `revup-0.2.0/setup.py`

 * *Files identical despite different names*

