# Comparing `tmp/sandwine-1.3.3.tar.gz` & `tmp/sandwine-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sandwine-1.3.3.tar", last modified: Wed Apr 26 10:45:26 2023, max compression
+gzip compressed data, was "sandwine-2.0.0.tar", last modified: Wed Apr 26 11:14:55 2023, max compression
```

## Comparing `sandwine-1.3.3.tar` & `sandwine-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 10:45:26.874486 sandwine-1.3.3/
--rw-r--r--   0 sping     (1000) sping     (1000)    35149 2023-02-25 17:36:47.000000 sandwine-1.3.3/COPYING
--rw-r--r--   0 sping     (1000) sping     (1000)     8446 2023-04-26 10:45:26.874486 sandwine-1.3.3/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     7317 2023-03-27 02:07:33.000000 sandwine-1.3.3/README.md
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 10:45:26.873486 sandwine-1.3.3/sandwine/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2023-02-25 17:36:47.000000 sandwine-1.3.3/sandwine/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      766 2023-02-25 17:36:47.000000 sandwine-1.3.3/sandwine/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)    16899 2023-04-26 10:43:41.000000 sandwine-1.3.3/sandwine/_main.py
--rw-r--r--   0 sping     (1000) sping     (1000)      847 2023-04-26 10:44:49.000000 sandwine-1.3.3/sandwine/_metadata.py
--rw-r--r--   0 sping     (1000) sping     (1000)     6061 2023-03-27 02:07:33.000000 sandwine-1.3.3/sandwine/_x11.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 10:45:26.874486 sandwine-1.3.3/sandwine.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)     8446 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)      319 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       49 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       20 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/requires.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        9 2023-04-26 10:45:26.000000 sandwine-1.3.3/sandwine.egg-info/top_level.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-04-26 10:45:26.875486 sandwine-1.3.3/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     2309 2023-04-26 10:43:41.000000 sandwine-1.3.3/setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 11:14:55.794837 sandwine-2.0.0/
+-rw-r--r--   0 sping     (1000) sping     (1000)    35149 2023-02-25 17:36:47.000000 sandwine-2.0.0/COPYING
+-rw-r--r--   0 sping     (1000) sping     (1000)     8473 2023-04-26 11:14:55.794837 sandwine-2.0.0/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     7317 2023-03-27 02:07:33.000000 sandwine-2.0.0/README.md
+-rw-r--r--   0 sping     (1000) sping     (1000)     2047 2023-04-26 11:13:46.000000 sandwine-2.0.0/pyproject.toml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 11:14:55.792837 sandwine-2.0.0/sandwine/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2023-02-25 17:36:47.000000 sandwine-2.0.0/sandwine/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      766 2023-02-25 17:36:47.000000 sandwine-2.0.0/sandwine/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    17691 2023-04-26 11:13:35.000000 sandwine-2.0.0/sandwine/_main.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     6061 2023-03-27 02:07:33.000000 sandwine-2.0.0/sandwine/_x11.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-04-26 11:14:55.793837 sandwine-2.0.0/sandwine.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)     8473 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)      303 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       49 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       20 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/requires.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        9 2023-04-26 11:14:55.000000 sandwine-2.0.0/sandwine.egg-info/top_level.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-04-26 11:14:55.794837 sandwine-2.0.0/setup.cfg
```

### Comparing `sandwine-1.3.3/COPYING` & `sandwine-2.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `sandwine-1.3.3/PKG-INFO` & `sandwine-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: sandwine
-Version: 1.3.3
+Version: 2.0.0
 Summary: Command-line tool to run Windows apps with Wine and bwrap/bubblewrap isolation
-Home-page: https://github.com/hartwork/sandwine
-Author: Sebastian Pipping
-Author-email: sebastian@pipping.org
+Author-email: Sebastian Pipping <sebastian@pipping.org>
 License: GPLv3+
+Project-URL: Homepage, https://github.com/hartwork/sandwine
+Project-URL: Bug Tracker, https://github.com/hartwork/sandwine/issues
+Keywords: Wine,sandbox,sandboxing,bubblewrap,bwrap
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Unix
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Emulators
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run the test suite](https://github.com/hartwork/sandwine/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/sandwine/actions/workflows/run-tests.yml)
 [![Run pre-commit](https://github.com/hartwork/sandwine/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/hartwork/sandwine/actions/workflows/pre-commit.yml)
```

### Comparing `sandwine-1.3.3/README.md` & `sandwine-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sandwine-1.3.3/sandwine/__main__.py` & `sandwine-2.0.0/sandwine/__main__.py`

 * *Files identical despite different names*

### Comparing `sandwine-1.3.3/sandwine/_main.py` & `sandwine-2.0.0/sandwine/_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,31 @@
 # more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with sandwine. If not, see <https://www.gnu.org/licenses/>.
 
 import logging
 import os
+import pty
 import random
 import shlex
 import signal
 import subprocess
 import sys
 from argparse import ArgumentParser, RawTextHelpFormatter
 from contextlib import nullcontext
 from dataclasses import dataclass
 from enum import Enum, auto
+from importlib.metadata import metadata
 from operator import attrgetter, itemgetter
 from textwrap import dedent
 from typing import Optional
 
 import coloredlogs
 
-from sandwine._metadata import DESCRIPTION, VERSION
 from sandwine._x11 import X11Display, X11Mode, create_x11_context, detect_and_require_nested_x11
 
 _logger = logging.getLogger(__name__)
 
 
 class AccessMode(Enum):
     READ_ONLY = 'ro'
@@ -49,35 +50,37 @@
     BIND_RW = auto()
     BIND_DEV = auto()
     TMPFS = auto()
     PROC = auto()
 
 
 def parse_command_line(args):
+    distribution = metadata('sandwine')
+
     usage = dedent('''\
         usage: sandwine [OPTIONS] [--] PROGRAM [ARG ..]
            or: sandwine [OPTIONS] --configure
            or: sandwine --help
            or: sandwine --version
     ''')[len('usage: '):]
 
     parser = ArgumentParser(
         prog='sandwine',
         usage=usage,
-        description=DESCRIPTION,
+        description=distribution['Summary'],
         formatter_class=RawTextHelpFormatter,
         epilog=dedent("""\
         Software libre licensed under GPL v3 or later.
         Brought to you by Sebastian Pipping <sebastian@pipping.org>.
 
         Please report bugs at https://github.com/hartwork/sandwine — thank you!
     """),
     )
 
-    parser.add_argument('--version', action='version', version=VERSION)
+    parser.add_argument('--version', action='version', version=distribution['Version'])
 
     program = parser.add_argument_group('positional arguments')
     program.add_argument('argv_0', metavar='PROGRAM', nargs='?', help='command to run')
     program.add_argument('argv_1_plus',
                          metavar='ARG',
                          nargs='*',
                          help='arguments to pass to PROGRAM')
@@ -139,14 +142,21 @@
                        help='bind mount host PATH on PATH (CAREFUL!)')
 
     general = parser.add_argument_group('general operation arguments')
     general.add_argument('--configure',
                          action='store_true',
                          help='enforce running winecfg before start of PROGRAM'
                          ' (default: run winecfg as needed)')
+    general.add_argument('--no-pty',
+                         dest='with_pty',
+                         default=True,
+                         action='store_false',
+                         help='refrain from creating a pseudo-terminal'
+                         ', stop protecting against TIOCSTI/TIOCLINUX hijacking (CAREFUL!)'
+                         ' (default: create a pseudo-terminal)')
     general.add_argument('--no-wine',
                          dest='with_wine',
                          default=True,
                          action='store_false',
                          help='run PROGRAM without use of Wine'
                          ' (default: run command "wine PROGRAM [ARG ..]")')
     general.add_argument('--retry',
@@ -234,15 +244,14 @@
     env_tasks = {var: None for var in ['HOME', 'TERM', 'USER', 'WINEDEBUG']}
     env_tasks['container'] = 'sandwine'
     unshare_args = ['--unshare-user', '--unshare-all']
 
     argv = ArgvBuilder()
 
     argv.add('bwrap')
-    argv.add('--new-session')
     argv.add('--disable-userns')
     argv.add('--die-with-parent')
 
     # Hostname
     hostname = random_hostname()
     env_tasks['HOSTNAME'] = hostname
     argv.add('--hostname', hostname)
@@ -412,14 +421,27 @@
     argv = ['bwrap', '--disable-userns', '--help']
     if subprocess.call(argv, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL) != 0:
         _logger.error('sandwine requires bubblewrap >=0.8.0'
                       ', aborting.')
         sys.exit(1)
 
 
+def spawn_argv(argv: list[str], with_pty: bool) -> int:
+    if not with_pty:
+        return subprocess.call(argv)
+
+    wait_status = pty.spawn(argv)
+
+    exit_code = os.waitstatus_to_exitcode(wait_status)
+    if exit_code < 0:  # e.g. -2 for "killed by SIGINT"
+        exit_code = 128 - exit_code  # e.g. -2 -> 130
+
+    return exit_code
+
+
 def main():
     exit_code = 0
     try:
         config = parse_command_line(sys.argv[1:])
 
         coloredlogs.install(level=logging.DEBUG)
 
@@ -443,15 +465,15 @@
         argv_builder = create_bwrap_argv(config)
         argv_builder.announce_to(sys.stderr)
 
         argv = list(argv_builder.iter_flat())
 
         with x11context:
             try:
-                exit_code = subprocess.call(argv)
+                exit_code = spawn_argv(argv, with_pty=config.with_pty)
             except FileNotFoundError:
                 _logger.error(f'Command {argv[0]!r} is not available, aborting.')
                 exit_code = 127
 
     except KeyboardInterrupt:
         exit_code = 128 + signal.SIGINT
```

### Comparing `sandwine-1.3.3/sandwine/_x11.py` & `sandwine-2.0.0/sandwine/_x11.py`

 * *Files identical despite different names*

### Comparing `sandwine-1.3.3/sandwine.egg-info/PKG-INFO` & `sandwine-2.0.0/sandwine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: sandwine
-Version: 1.3.3
+Version: 2.0.0
 Summary: Command-line tool to run Windows apps with Wine and bwrap/bubblewrap isolation
-Home-page: https://github.com/hartwork/sandwine
-Author: Sebastian Pipping
-Author-email: sebastian@pipping.org
+Author-email: Sebastian Pipping <sebastian@pipping.org>
 License: GPLv3+
+Project-URL: Homepage, https://github.com/hartwork/sandwine
+Project-URL: Bug Tracker, https://github.com/hartwork/sandwine/issues
+Keywords: Wine,sandbox,sandboxing,bubblewrap,bwrap
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Unix
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Emulators
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run the test suite](https://github.com/hartwork/sandwine/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/sandwine/actions/workflows/run-tests.yml)
 [![Run pre-commit](https://github.com/hartwork/sandwine/actions/workflows/pre-commit.yml/badge.svg)](https://github.com/hartwork/sandwine/actions/workflows/pre-commit.yml)
```

### Comparing `sandwine-1.3.3/setup.py` & `sandwine-2.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#! /usr/bin/env python3
 # This file is part of the sandwine project.
 #
 # Copyright (c) 2023 Sebastian Pipping <sebastian@pipping.org>
 #
 # sandwine is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free
 # Software Foundation, either version 3 of the License, or (at your option)
@@ -12,53 +11,48 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or
 # FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for
 # more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with sandwine. If not, see <https://www.gnu.org/licenses/>.
 
-from setuptools import find_packages, setup
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
 
-from sandwine._metadata import DESCRIPTION, VERSION
+[project]
+name = "sandwine"
+version = "2.0.0"
+license = {text = "GPLv3+"}
+description = "Command-line tool to run Windows apps with Wine and bwrap/bubblewrap isolation"
+readme = {file = "README.md", content-type = "text/markdown"}
+authors = [
+  { name="Sebastian Pipping", email="sebastian@pipping.org" },
+]
+requires-python = ">=3.9"
+dependencies = [
+  "coloredlogs>=15.0.1",
+]
+keywords = ["Wine", "sandbox", "sandboxing", "bubblewrap", "bwrap"]
+classifiers = [
+  "Development Status :: 3 - Alpha",
+  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+  "Intended Audience :: Developers",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Intended Audience :: Developers",
+  "Intended Audience :: End Users/Desktop",
+  "Operating System :: Unix",
+  "Topic :: Security",
+  "Topic :: System :: Emulators",
+]
 
-setup(
-    name='sandwine',
-    version=VERSION,
-    license='GPLv3+',
-    description=DESCRIPTION,
-    long_description=open('README.md', encoding='utf-8').read(),
-    long_description_content_type='text/markdown',
-    author='Sebastian Pipping',
-    author_email='sebastian@pipping.org',
-    url='https://github.com/hartwork/sandwine',
-    python_requires='>=3.7',
-    setup_requires=[
-        'setuptools>=38.6.0',  # for long_description_content_type
-    ],
-    install_requires=[
-        'coloredlogs>=15.0.1',
-    ],
-    packages=find_packages(),
-    entry_points={
-        'console_scripts': [
-            'sandwine = sandwine._main:main',
-        ],
-    },
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Intended Audience :: Developers',
-        'Intended Audience :: End Users/Desktop',
-        'Operating System :: Unix',
-        'Topic :: Security',
-        'Topic :: System :: Emulators',
-    ],
-)
+[project.urls]
+"Homepage" = "https://github.com/hartwork/sandwine"
+"Bug Tracker" = "https://github.com/hartwork/sandwine/issues"
+
+[project.scripts]
+sandwine = "sandwine._main:main"
```

