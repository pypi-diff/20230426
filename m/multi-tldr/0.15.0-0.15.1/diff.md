# Comparing `tmp/multi-tldr-0.15.0.tar.gz` & `tmp/multi-tldr-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi-tldr-0.15.0.tar", last modified: Sun Apr 16 16:14:46 2023, max compression
+gzip compressed data, was "multi-tldr-0.15.1.tar", last modified: Tue Apr 25 16:31:58 2023, max compression
```

## Comparing `multi-tldr-0.15.0.tar` & `multi-tldr-0.15.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/
--rw-r--r--   0 root         (0) root         (0)     1099 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      127 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/Readme.PyPI.md
--rw-r--r--   0 root         (0) root         (0)     9636 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/multi_tldr.egg-info/
--rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-16 16:14:46.000000 multi-tldr-0.15.0/multi_tldr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-16 16:14:46.649850 multi-tldr-0.15.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1083 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/setup.py
--rwxr-xr-x   0 root         (0) root         (0)    18575 2023-04-16 16:14:41.000000 multi-tldr-0.15.0/tldr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:31:58.931629 multi-tldr-0.15.1/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-25 16:31:58.931629 multi-tldr-0.15.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      127 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)    14473 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:31:58.931629 multi-tldr-0.15.1/multi_tldr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-25 16:31:58.000000 multi-tldr-0.15.1/multi_tldr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-25 16:31:58.931629 multi-tldr-0.15.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1083 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)    20460 2023-04-25 16:31:53.000000 multi-tldr-0.15.1/tldr.py
```

### Comparing `multi-tldr-0.15.0/LICENSE` & `multi-tldr-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multi-tldr-0.15.0/PKG-INFO` & `multi-tldr-0.15.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-tldr
-Version: 0.15.0
+Version: 0.15.1
 Summary: Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 Home-page: https://github.com/Phuker/multi-tldr
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: MIT
 Keywords: tldr cli man command usage
 Classifier: Environment :: Console
```

### Comparing `multi-tldr-0.15.0/Readme.md` & `multi-tldr-0.15.1/Readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -132,82 +132,252 @@
 
 ## Usage
 
 This tldr client is designed based on the [tldr-pages client specification 1.4](https://github.com/tldr-pages/tldr/blob/master/CLIENT-SPECIFICATION.md), so it is very similar to other clients. But the specification is not 100% implemented, there is some differences.
 
 ### Show help message
 
-```bash
-tldr --help
+```console
+$ tldr --help
+usage: tldr [-h] [-i | -l | -u] [-p platform] [-V] [-v] [command ...]
+
+multi-tldr 0.15.1
+Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
+This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.
+https://github.com/Phuker/multi-tldr
+
+positional arguments:
+  command               Command to query
+
+options:
+  -h, --help            show this help message and exit
+  -i, --init            Interactively gererate config file
+  -l, --list            Print all tldr page files path (of a command if specified) in all repo on all/specified platform
+  -u, --update          Pull all git repo
+  -p platform, --platform platform
+                        Specify platform, choices: common, linux, osx, sunos, windows, android, all, default
+  -V, --version         Show version and exit
+  -v, --verbose         Increase verbosity level (use -vv or more for greater effect)
 ```
 
 ### Show version info
 
 ```console
 $ tldr --version
-multi-tldr, by Phuker, version 0.15.0
-Homepage: https://github.com/Phuker/multi-tldr
+multi-tldr 0.15.1
+Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.
+https://github.com/Phuker/multi-tldr
 ```
 
 ### Look up a command usage
 
-```bash
-tldr tar
-tldr git pull    # same as `tldr git-pull`
+```console
+$ tldr tar
+tar - /home/user/code/tldr/pages/common/tar.md
+
+Archiving utility.
+Often combined with a compression method, such as gzip or bzip2.
+More information: <https://www.gnu.org/software/tar>.
+
+[c]reate an archive and write it to a [f]ile:
+
+    tar cf path/to/target.tar path/to/file1 path/to/file2 ...
+
+[c]reate a g[z]ipped archive and write it to a [f]ile:
+
+    tar czf path/to/target.tar.gz path/to/file1 path/to/file2 ...
+
+[c]reate a g[z]ipped archive from a directory using relative paths:
+
+    tar czf path/to/target.tar.gz --directory=path/to/directory .
+
+E[x]tract a (compressed) archive [f]ile into the current directory [v]erbosely:
+
+    tar xvf path/to/source.tar[.gz|.bz2|.xz]
+
+E[x]tract a (compressed) archive [f]ile into the target directory:
+
+    tar xf path/to/source.tar[.gz|.bz2|.xz] --directory=path/to/directory
+
+[c]reate a compressed archive and write it to a [f]ile, using [a]rchive suffix to determine the compression program:
+
+    tar caf path/to/target.tar.xz path/to/file1 path/to/file2 ...
+
+Lis[t] the contents of a tar [f]ile [v]erbosely:
+
+    tar tvf path/to/source.tar
+
+E[x]tract files matching a pattern from an archive [f]ile:
+
+    tar xf path/to/source.tar --wildcards "*.html"
+
 ```
 
-By default, only pages on default platforms in `platform_list` are output.
+`tldr git pull` is same as `tldr git-pull`:
+
+```console
+$ tldr git pull
+git-pull - /home/user/code/tldr/pages/common/git-pull.md
+
+Fetch branch from a remote repository and merge it to local repository.
+More information: <https://git-scm.com/docs/git-pull>.
+
+Download changes from default remote repository and merge it:
+
+    git pull
+
+Download changes from default remote repository and use fast-forward:
+
+    git pull --rebase
+
+Download changes from given remote repository and branch, then merge them into HEAD:
 
-You can specify platform using `-p` argument:
+    git pull remote_name branch
+
+```
+
+By default, only pages on default platforms in `platform_list` are output. You can specify platform using `-p` argument.
+
+Only macOS `osx` platform:
+
+```console
+$ tldr -p osx airport
+airport - /home/user/code/tldr/pages/osx/airport.md
+
+Wireless network configuration utility.
+More information: <https://ss64.com/osx/airport.html>.
+
+Show current wireless status information:
+
+    airport --getinfo
+
+Sniff wireless traffic on channel 1:
+
+    airport sniff 1
+
+Scan for available wireless networks:
+
+    airport --scan
+
+Disassociate from current airport network:
+
+    sudo airport --disassociate
+
+```
+
+All platforms:
+
+```console
+$ tldr -p all snoop
+snoop - /home/user/code/tldr/pages/sunos/snoop.md
+
+Network packet sniffer.
+SunOS equivalent of tcpdump.
+More information: <https://www.unix.com/man-page/sunos/1m/snoop>.
+
+Capture packets on a specific network interface:
+
+    snoop -d e1000g0
+
+Save captured packets in a file instead of displaying them:
+
+    snoop -o path/to/file
+
+Display verbose protocol layer summary of packets from a file:
+
+    snoop -V -i path/to/file
+
+Capture network packets that come from a hostname and go to a given port:
+
+    snoop to port port from host hostname
+
+Capture and show a hex-dump of network packets exchanged between two IP addresses:
+
+    snoop -x0 -p4 ip1 ip2
 
-```bash
-tldr -p osx airport    # only osx platform
-tldr -p all snoop      # all platforms
 ```
 
 ### List tldr page files path
 
 List all pages on all platforms:
 
-```bash
-tldr --list
+```console
+$ tldr --list | head -n 3
+/home/user/code/tldr/pages/linux/xbacklight.md
+/home/user/code/tldr/pages/linux/pacman-query.md
+/home/user/code/tldr/pages/linux/nmcli-agent.md
+```
+
+All platforms, only `tar` command:
+
+```console
+$ tldr --list tar
+/home/user/code/tldr/pages/common/tar.md
+```
+
+Only `linux` platform:
+
+```console
+$ tldr --list -p linux | head -n 3
+/home/user/code/tldr/pages/linux/xbacklight.md
+/home/user/code/tldr/pages/linux/pacman-query.md
+/home/user/code/tldr/pages/linux/nmcli-agent.md
+```
+
+Only `common` platform, only `du` command:
+
+```console
+$ tldr --list -p common du
+/home/user/code/tldr/pages/common/du.md
+```
+
+Only default platforms in config:
+
+```console
+$ tldr --list -p default | head -n 3
+/home/user/code/tldr/pages/linux/xbacklight.md
+/home/user/code/tldr/pages/linux/pacman-query.md
+/home/user/code/tldr/pages/linux/nmcli-agent.md
 ```
 
-Specify platform and/or a command:
+Only default platforms in config, only `tree` command:
 
-```bash
-tldr --list tar                # all platforms, only tar command
-tldr --list -p linux           # only linux platform
-tldr --list -p common du       # only common platform, only du command
-tldr --list -p default         # only default platforms in config
-tldr --list -p default tree    # only default platforms in config, only tree command
+```console
+$ tldr --list -p default tree
+/home/user/code/tldr/pages/common/tree.md
 ```
 
 Fuzzy find a command:
 
 ```console
 $ tldr -l | grep git | grep show
-/home/user/code/tldr/pages/common/git-show.md
+/home/user/code/tldr/pages/common/git-show-unmerged-branches.md
+/home/user/code/tldr/pages/common/git-show-index.md
+/home/user/code/tldr/pages/common/git-show-merged-branches.md
 /home/user/code/tldr/pages/common/git-show-ref.md
+/home/user/code/tldr/pages/common/git-show.md
 /home/user/code/tldr/pages/common/git-show-branch.md
+/home/user/code/tldr/pages/common/git-show-tree.md
 ```
 
 ### Check for updates
 
 `git pull` will be run in all dir paths of `repo_directory_list`, so that we can get the latest tldr pages.
 
 ```console
 $ tldr --update
-08:00:00 [INFO]:Check for updates in '/home/user/code/tldr/pages' ...
+08:00:00 [INFO]:Check for updates in all repo directories
+08:00:00 [INFO]:(1/2) Check for updates in '/home/user/code/tldr/pages' ...
 Already up to date.
-08:00:02 [INFO]:Command 'git pull --stat' return code 0
-08:00:02 [INFO]:Check for updates in '/home/user/code/tldr-private/pages' ...
+08:00:00 [INFO]:Command 'git pull --stat' return code 0
+08:00:00 [INFO]:(2/2) Check for updates in '/home/user/code/tldr-private/pages' ...
 Already up to date.
-08:00:04 [INFO]:Command 'git pull --stat' return code 0
+08:00:00 [INFO]:Command 'git pull --stat' return code 0
+08:00:00 [INFO]:Check for updates finished
 ```
 
 ## FAQ
 
 **Q: I want to add some custom command usages to a command, how to do it?**
 
 **Q: I want to create some private command pages, how?**
```

### Comparing `multi-tldr-0.15.0/multi_tldr.egg-info/PKG-INFO` & `multi-tldr-0.15.1/multi_tldr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-tldr
-Version: 0.15.0
+Version: 0.15.1
 Summary: Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
 Home-page: https://github.com/Phuker/multi-tldr
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: MIT
 Keywords: tldr cli man command usage
 Classifier: Environment :: Console
```

### Comparing `multi-tldr-0.15.0/setup.py` & `multi-tldr-0.15.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open('Readme.PyPI.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='multi-tldr',
     description='Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     author='Phuker',
     author_email='Phuker@users.noreply.github.com',
     url='https://github.com/Phuker/multi-tldr',
     license='MIT',
     keywords='tldr cli man command usage',
     packages=[],
     py_modules = ['tldr'],
```

### Comparing `multi-tldr-0.15.0/tldr.py` & `multi-tldr-0.15.1/tldr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 """
-multi-tldr
-
 Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.
-
+This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.
 https://github.com/Phuker/multi-tldr
 """
 
 import os
 import sys
 import argparse
 import logging
@@ -21,40 +19,44 @@
 # buggy: https://github.com/pallets/click/issues/665
 # import readline
 
 import click
 
 
 __title__ = 'multi-tldr'
-__version__ = '0.15.0'
+__version__ = '0.15.1'
 __author__ = 'Phuker'
 __homepage__ = 'https://github.com/Phuker/multi-tldr'
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) 2020 Phuker, Copyright (c) 2015 lord63'
 __specification__ = 'This tldr client is designed based on the tldr-pages client specification 1.4, but not 100% implemented.'
 
-# High coupling
-# make things just work at a minimal level, or can not even --init
-DEFAULT_CONFIG = {
+VERSION_STR_SHORT = f'{__title__} {__version__}'
+VERSION_STR_LONG = f'{__title__} {__version__}\n{__doc__.strip()}'
+ALL_PLATFORM_LIST = ('common', 'linux', 'osx', 'sunos', 'windows', 'android')
+SUPPORTED_COLORS = ('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'bright_black', 'bright_red', 'bright_green', 'bright_yellow', 'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white')
+
+logger = logging.getLogger(__name__)
+config = {
     'repo_directory_list': [],
-    'color_output': 'never',
+    'color_output': 'auto',
     'colors': {
         'description': 'bright_yellow',
         'usage': 'green',
         'command': 'white',
         'param': 'cyan',
     },
     'command_indent_size': 4,
-    'platform_list': [],
+    'platform_list': [
+        'common',
+        'linux',
+    ],
     'compact_output': False,
 }
 
-logger = logging.getLogger(__name__)
-shell_args = None
-
 
 def _assert(expr, msg=''):
     if not expr:
         raise AssertionError(msg)
 
 
 def _init_logging():
@@ -71,44 +73,57 @@
         level=logging_level,
         format=logging_format,
         datefmt=logging_date_format,
         stream=logging_stream,
     )
 
 
+def _logging_set_color_output():
+    handler = logging.root.handlers[0]
+    handler.setFormatter(logging.Formatter('\x1b[1m%(asctime)s [%(levelname)s]:\x1b[0m%(message)s', handler.formatter.datefmt))
+
+    logging.addLevelName(logging.CRITICAL, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.CRITICAL)))
+    logging.addLevelName(logging.ERROR, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.ERROR)))
+    logging.addLevelName(logging.WARNING, '\x1b[33m{}\x1b[39m'.format(logging.getLevelName(logging.WARNING)))
+    logging.addLevelName(logging.INFO, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.INFO)))
+    logging.addLevelName(logging.DEBUG, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.DEBUG)))
+
+
 def _parse_args(args=sys.argv[1:]):
+    choices_platform = ALL_PLATFORM_LIST + ('all', 'default')
+
     parser = argparse.ArgumentParser(
-        description='Yet another python client for tldr-pages/tldr. View tldr pages in multi repo, multi platform, any language at the same time.',
-        epilog='https://github.com/Phuker/multi-tldr',
+        description=VERSION_STR_LONG,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
         add_help=True
     )
+
     group = parser.add_mutually_exclusive_group(required=False)
     group.add_argument('-i', '--init', action='store_true', help='Interactively gererate config file')
     group.add_argument('-l', '--list', action='store_true', help='Print all tldr page files path (of a command if specified) in all repo on all/specified platform')
     group.add_argument('-u', '--update', action='store_true', help='Pull all git repo')
     
     parser.add_argument('command', help='Command to query', nargs='*')
-    parser.add_argument('-p', '--platform', help="Specify platform. Special virtual platform options are 'all' and 'default'", choices=['common', 'linux', 'osx', 'sunos', 'windows', 'all', 'default'])
+    parser.add_argument('-p', '--platform', metavar='platform', help="Specify platform, choices: %(choices)s", choices=choices_platform)
 
-    parser.add_argument('-V', '--version', action='store_true', help='Show version and exit')
+    parser.add_argument('-V', '--version', action='version', version=VERSION_STR_LONG, help='Show version and exit')
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase verbosity level (use -vv or more for greater effect)')
 
     result = parser.parse_args(args)
 
     if result.verbose >= 1:
         logging.root.setLevel(logging.DEBUG)
     
     if result.command:
         result.command = '-'.join(result.command)
     else:
         result.command = None
     
     ctrl_group_set = result.init or result.list or result.update
     ok_conditions = [
-        result.version,
         result.init and result.command is None and result.platform is None,
         result.list,
         result.update and result.command is None and result.platform is None,
         not ctrl_group_set and result.command is not None,
     ]
 
     if not any(ok_conditions):
@@ -119,98 +134,115 @@
     logger.debug('Command line arguments: %r', result)
 
     return result
 
 
 def get_config_dir_path():
     sub_dir_name = 'multi-tldr'
+
     if 'TLDR_CONFIG_DIR' in os.environ:
         config_dir_path = os.environ.get('TLDR_CONFIG_DIR')
     elif 'XDG_CONFIG_HOME' in os.environ:
         config_dir_path = os.path.join(os.environ.get('XDG_CONFIG_HOME'), sub_dir_name)
     else:
         config_dir_path = os.path.join('~', '.config', sub_dir_name)
     
     config_dir_path = os.path.abspath(os.path.expanduser(config_dir_path))
 
     return config_dir_path
 
 
-def get_config_path():
+def get_config_file_path():
     return os.path.join(get_config_dir_path(), 'tldr.config.json')
 
 
-def check_config(config):
-    _assert(isinstance(config, dict), 'Invalid config')
-    _assert(isinstance(config['color_output'], str), 'Invalid color_output')
-    _assert(isinstance(config['colors'], dict), 'Invalid colors')
-    _assert(isinstance(config['platform_list'], list), 'Invalid platform_list')
-    _assert(isinstance(config['repo_directory_list'], list), 'Invalid repo_directory_list')
-    _assert(isinstance(config['compact_output'], bool), 'Invalid compact_output')
-    _assert(isinstance(config['command_indent_size'], int), 'Invalid command_indent_size')
-
-    _assert(config['color_output'] in ('always', 'auto', 'never'))
-    _assert(config['command_indent_size'] >= 0, 'Invalid command_indent_size')
-    
-    supported_colors = ('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'bright_black', 'bright_red', 'bright_green', 'bright_yellow', 'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white')
-    if not set(config['colors'].values()).issubset(set(supported_colors)):
-        bad_colors = set(config['colors'].values()) - set(supported_colors)
-        bad_colors_str = ', '.join([repr(_) for _ in bad_colors])
-        raise ValueError(f'Unsupported colors in config file: {bad_colors_str}')
-
-    for platform in config['platform_list']:
-        _assert(isinstance(platform, str), 'Invalid platform_list')
-    
-    for _repo_dir in config['repo_directory_list']:
-        _assert(isinstance(_repo_dir, str), 'Invalid repo_directory_list')
-        _assert(os.path.exists(os.path.abspath(os.path.expanduser(_repo_dir))), f'Path in repo_directory_list not exist: {_repo_dir!r}')
+def check_config(json_data):
+    _assert(isinstance(json_data, dict), 'Invalid config')
+
+    if 'repo_directory_list' in json_data:
+        _assert(isinstance(json_data['repo_directory_list'], list), 'Invalid config: repo_directory_list')
+        for _repo_dir in json_data['repo_directory_list']:
+            _assert(isinstance(_repo_dir, str), 'Invalid config: repo_directory_list')
+            _assert(os.path.isdir(os.path.abspath(os.path.expanduser(_repo_dir))), f'Invalid config: repo_directory_list, repo directory not exist: {_repo_dir!r}')
+
+    if 'color_output' in json_data:
+        _assert(isinstance(json_data['color_output'], str), 'Invalid config: color_output')
+        _assert(json_data['color_output'] in ('always', 'auto', 'never'), 'Invalid config: color_output')
+    
+    if 'colors' in json_data:
+        _assert(isinstance(json_data['colors'], dict), 'Invalid config: colors')
+        _assert(json_data['colors'].keys() == config['colors'].keys(), 'Invalid config: colors')
+        if not set(json_data['colors'].values()).issubset(set(SUPPORTED_COLORS)):
+            bad_colors = set(json_data['colors'].values()) - set(SUPPORTED_COLORS)
+            bad_colors_str = ', '.join([repr(_) for _ in bad_colors])
+            raise ValueError(f'Invalid config: colors, unsupported colors: {bad_colors_str}')
+    
+    if 'command_indent_size' in json_data:
+        _assert(isinstance(json_data['command_indent_size'], int), 'Invalid config: command_indent_size')
+        _assert(json_data['command_indent_size'] >= 0, 'Invalid config: command_indent_size')
+
+    if 'platform_list' in json_data:
+        _assert(isinstance(json_data['platform_list'], list), 'Invalid config: platform_list')
+        for platform in json_data['platform_list']:
+            _assert(isinstance(platform, str), 'Invalid config: platform_list')
+    
+    if 'compact_output' in json_data:
+        _assert(isinstance(json_data['compact_output'], bool), 'Invalid config: compact_output')
 
 
 def load_json(file_path):
     _assert(isinstance(file_path, str))
 
     try:
         with open(file_path, 'r', encoding='utf-8') as f:
             return json.load(f)
     except Exception as e:
         logger.error('Error when load json file %r: %r %r', file_path, type(e), e)
         sys.exit(1)
 
 
-@functools.lru_cache
-def get_config():
-    """Get the configurations and return it as a dict."""
+def load_config():
+    """Load config file and overwrite default config object"""
 
-    config_path = get_config_path()
-    if not os.path.exists(config_path):
-        logger.error("Can't find config file at: %r", config_path)
+    config_file_path = get_config_file_path()
+    if not os.path.isfile(config_file_path):
+        logger.error("Can't find config file at: %r", config_file_path)
         logger.error('You may use `tldr --init` to init the config file')
-        return DEFAULT_CONFIG
+        return
 
-    logger.debug('Reading config file: %r', config_path)
-    config = load_json(config_path)
+    logger.debug('Reading config file: %r', config_file_path)
+    json_data = load_json(config_file_path)
 
+    logger.debug('Check config')
     try:
-        check_config(config)
+        check_config(json_data)
     except Exception as e:
         logger.error('Check config failed: %r', e)
         logger.error('You may use `tldr --init` to init the config file')
-        return DEFAULT_CONFIG
+        return
+    
+    logger.debug('Overwrite default config object')
+    for k in config:
+        if k in json_data:
+            config[k] = json_data[k]
 
     config['repo_directory_list'] = [os.path.abspath(os.path.expanduser(_)) for _ in config['repo_directory_list']]
+    logger.debug('Final config:\n%s', json.dumps(config, ensure_ascii=False, indent=4))
 
-    return config
+
+def do_color_output():
+    color_output = config['color_output']
+
+    return color_output == 'always' or (color_output == 'auto' and sys.stdout.isatty() and 'TERM' in os.environ)
 
 
 def style(text, *args, **kwargs):
     """Wrapper of click.style()"""
 
-    color_output = get_config()['color_output']
-
-    if color_output == 'always' or (color_output == 'auto' and sys.stdout.isatty() and 'TERM' in os.environ):
+    if do_color_output():
         return click.style(text, *args, **kwargs)
     else:
         return text
 
 
 @functools.lru_cache
 def get_escape_str(*args, **kwargs):
@@ -224,15 +256,15 @@
 
 @functools.lru_cache
 def get_escape_str_by_type(_type):
     """Get escape string by type"""
 
     _assert(_type is None or isinstance(_type, str))
 
-    colors = get_config()['colors']
+    colors = config['colors']
 
     if _type is None:
         return ''
     elif _type in ('description', 'usage', 'command'):
         return get_escape_str(fg=colors[_type], underline=False)
     elif _type == 'param':
         return get_escape_str(fg=colors[_type], underline=True)
@@ -273,16 +305,16 @@
     result += get_escape_str(reset=True)
     return result
 
 
 def parse_page(page_file_path):
     """Parse the command man page."""
 
-    compact_output = get_config()['compact_output']
-    command_indent_size = get_config()['command_indent_size']
+    compact_output = config['compact_output']
+    command_indent_size = config['command_indent_size']
 
     logger.debug('Reading file: %r', page_file_path)
     with open(page_file_path, 'r', encoding='utf-8') as f:
         lines = f.readlines() # with '\n' end
     
     output_lines = []
     for line in lines:
@@ -337,16 +369,16 @@
 
 def get_page_path_list(command=None, platform='default'):
     """Get page_path_list in all repo"""
 
     _assert(command is None or isinstance(command, str))
     _assert(isinstance(platform, str))
 
-    repo_directory_list = get_config()['repo_directory_list']
-    default_platform_set = set(get_config()['platform_list'])
+    repo_directory_list = config['repo_directory_list']
+    default_platform_set = set(config['platform_list'])
 
     page_path_list = []
     for repo_directory in repo_directory_list:
         index = get_index(repo_directory)
 
         if command is not None:
             filter_func = lambda entry: entry[1] == command
@@ -363,17 +395,17 @@
     
     return page_path_list
 
 
 def action_init():
     """Interactively gererate config file"""
 
-    config_path = get_config_path()
-    if os.path.exists(config_path):
-        logger.warning('A config file already exists: %r', config_path)
+    config_file_path = get_config_file_path()
+    if os.path.exists(config_file_path):
+        logger.warning('A config file already exists: %r', config_file_path)
         if click.prompt('Are you sure want to overwrite it? (yes/no)', default='no') != 'yes':
             return
     
     repo_path_list = []
     logger.info('Please input repo path line by line, to "pages/" level, empty line to end.')
     while True:
         repo_path = click.prompt('Input 1 tldr repo path', default='')
@@ -382,25 +414,25 @@
         repo_path = os.path.abspath(os.path.expanduser(repo_path))
         if not os.path.exists(repo_path):
             logger.error('Repo path not exist, clone it first.')
         elif repo_path not in repo_path_list:
             repo_path_list.append(repo_path)
 
     platform_list = []
-    platform_choice = click.Choice(('common', 'linux', 'osx', 'sunos', 'windows', ''))
+    platform_choice = click.Choice(ALL_PLATFORM_LIST + ('', ))
     logger.info('Please input default platforms line by line, empty line to end.')
     while True:
         platform = click.prompt('Input 1 platform', type=platform_choice, default='')
         if len(platform) == 0:
             break
         elif platform not in platform_list:
             platform_list.append(platform)
 
     logger.info('Please input colors, empty to use default.')
-    colors_choice = click.Choice(('black', 'red', 'green', 'yellow', 'blue', 'magenta', 'cyan', 'white', 'bright_black', 'bright_red', 'bright_green', 'bright_yellow', 'bright_blue', 'bright_magenta', 'bright_cyan', 'bright_white'))
+    colors_choice = click.Choice(SUPPORTED_COLORS)
     colors = {
         'description': click.prompt('Input color for description', type=colors_choice, default='bright_yellow'),
         'usage': click.prompt('Input color for usage', type=colors_choice, default='green'),
         'command': click.prompt('Input color for command', type=colors_choice, default='white'),
         'param': click.prompt('Input color for param', type=colors_choice, default='cyan'),
     }
 
@@ -423,37 +455,50 @@
     }
 
     config_dir_path = get_config_dir_path()
     if not os.path.exists(config_dir_path):
         logger.info('Make dir: %r', config_dir_path)
         os.makedirs(config_dir_path)
 
-    logger.info('Write to config file %r', config_path)
-    with open(config_path, 'w') as f:
-        f.write(json.dumps(config, ensure_ascii=True, indent=4))
+    logger.info('Write to config file %r', config_file_path)
+    with open(config_file_path, 'w') as f:
+        f.write(json.dumps(config, ensure_ascii=False, indent=4))
 
 
 def action_update():
     """Update all tldr pages repo."""
 
-    repo_directory_list = get_config()['repo_directory_list']
+    repo_directory_list = config['repo_directory_list']
     command = ['git', 'pull', '--stat']
     command_str = ' '.join(command)
 
-    for repo_directory in repo_directory_list:
+    exist_error = False
+    logger.info('Check for updates in all repo directories')
+    for i, repo_directory in enumerate(repo_directory_list):
         os.chdir(repo_directory)
-        logger.info('Check for updates in %r ...', repo_directory)
+        logger.info('(%d/%d) Check for updates in %r ...', i + 1, len(repo_directory_list), repo_directory)
         try:
             return_code = subprocess.call(command)
-            return_code_color = 'green' if return_code == 0 else 'bright_red'
+            if return_code == 0:
+                return_code_color = 'green'
+            else:
+                return_code_color = 'bright_red'
+                exist_error = True
+            
             return_code_str = style(str(return_code), fg=return_code_color)
-
             logger.info('Command %r return code %s', command_str, return_code_str)
         except Exception as e:
             logger.error('Error when run %r in %r: %r %r', command_str, repo_directory, type(e), e)
+            exist_error = True
+    
+    if exist_error:
+        logger.info('Check for updates finished with error')
+        sys.exit(1)
+    else:
+        logger.info('Check for updates finished')
 
 
 def action_find(command, platform):
     """Find and display the tldr pages of a command."""
 
     _assert(isinstance(command, str))
     _assert(platform is None or isinstance(platform, str))
@@ -488,20 +533,14 @@
     else:
         page_path_list = get_page_path_list(command, 'all')
     
     for page_path in page_path_list:
         print(page_path)
 
 
-def action_version():
-    print(f'{__title__}, by {__author__}, version {__version__}')
-    print(f'Homepage: {__homepage__}')
-    print(__specification__)
-
-
 def broken_pipe_error_wrapper(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         # https://docs.python.org/3/library/signal.html#note-on-sigpipe
         try:
             return func(*args, **kwargs)
         except BrokenPipeError:
@@ -510,26 +549,31 @@
             sys.exit(1)
 
     return wrapper
 
 
 @broken_pipe_error_wrapper
 def main():
+    global config
+
     _init_logging()
     shell_args = _parse_args()
 
-    if shell_args.version:
-        action_version()
-    elif shell_args.init:
+    if shell_args.init:
         action_init()
-    elif shell_args.list:
-        action_list_command(shell_args.command, shell_args.platform)
-    elif shell_args.update:
-        action_update()
     else:
-        action_find(shell_args.command, shell_args.platform)
+        load_config()
+        if do_color_output():
+            _logging_set_color_output()
+
+        if shell_args.list:
+            action_list_command(shell_args.command, shell_args.platform)
+        elif shell_args.update:
+            action_update()
+        else:
+            action_find(shell_args.command, shell_args.platform)
     
     sys.stdout.flush()
 
 
 if __name__ == '__main__':
     main()
```

