# Comparing `tmp/docker-compose-all-0.2.1.tar.gz` & `tmp/docker-compose-all-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-compose-all-0.2.1.tar", last modified: Mon Apr 17 14:05:42 2023, max compression
+gzip compressed data, was "docker-compose-all-0.2.2.tar", last modified: Wed Apr 26 11:56:01 2023, max compression
```

## Comparing `docker-compose-all-0.2.1.tar` & `docker-compose-all-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      824 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/Readme.PyPI.md
--rw-r--r--   0 root         (0) root         (0)     1931 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/docker_compose_all.egg-info/
--rw-r--r--   0 root         (0) root         (0)      824 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-17 14:05:42.000000 docker-compose-all-0.2.1/docker_compose_all.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    11610 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/docker_compose_all.py
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-17 14:05:42.794036 docker-compose-all-0.2.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1123 2023-04-17 14:05:36.000000 docker-compose-all-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:56:01.648826 docker-compose-all-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      824 2023-04-26 11:56:01.648826 docker-compose-all-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:56:01.648826 docker-compose-all-0.2.2/docker_compose_all.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      824 2023-04-26 11:56:01.000000 docker-compose-all-0.2.2/docker_compose_all.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-26 11:56:01.000000 docker-compose-all-0.2.2/docker_compose_all.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:56:01.000000 docker-compose-all-0.2.2/docker_compose_all.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 11:56:01.000000 docker-compose-all-0.2.2/docker_compose_all.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-26 11:56:01.000000 docker-compose-all-0.2.2/docker_compose_all.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    11410 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/docker_compose_all.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-04-26 11:56:01.648826 docker-compose-all-0.2.2/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1122 2023-04-26 11:53:21.000000 docker-compose-all-0.2.2/setup.py
```

### Comparing `docker-compose-all-0.2.1/LICENSE` & `docker-compose-all-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-compose-all-0.2.1/PKG-INFO` & `docker-compose-all-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-compose-all
-Version: 0.2.1
+Version: 0.2.2
 Summary: A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 Home-page: https://github.com/Phuker/docker-compose-all
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
```

### Comparing `docker-compose-all-0.2.1/Readme.md` & `docker-compose-all-0.2.2/Readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 docker-compose-all version 0.2.1
 A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 https://github.com/Phuker/docker-compose-all
 
 positional arguments:
   dir_path       A directory which contains Docker Compose projects, default: '.'
 
-optional arguments:
+options:
   -h, --help     show this help message and exit
   --restart      Completely rebuild and rerun all. Including the following steps: stop, down, build, up, ps.
   --stop         Stop all containers
   --down         Make all down. Stop and remove containers, networks, images
   --build        Rebuild all
   --up           Make all up
   --ps           Each ps
```

### Comparing `docker-compose-all-0.2.1/docker_compose_all.egg-info/PKG-INFO` & `docker-compose-all-0.2.2/docker_compose_all.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-compose-all
-Version: 0.2.1
+Version: 0.2.2
 Summary: A very simple Docker cluster management tool, recursively search and control all Docker Compose projects in a directory.
 Home-page: https://github.com/Phuker/docker-compose-all
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
```

### Comparing `docker-compose-all-0.2.1/docker_compose_all.py` & `docker-compose-all-0.2.2/docker_compose_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,20 +13,17 @@
 import atexit
 import time
 import subprocess
 import shlex
 from datetime import timedelta
 
 
-__version__ = '0.2.1'
-logger = logging.getLogger(__name__)
-shell_args = None
-
-VERSION_STR_SHORT = f'docker-compose-all version {__version__}'
-VERSION_STR_LONG = f'docker-compose-all version {__version__}\n{__doc__.strip()}'
+__version__ = '0.2.2'
+VERSION_STR_SHORT = f'docker-compose-all {__version__}'
+VERSION_STR_LONG = f'docker-compose-all {__version__}\n{__doc__.strip()}'
 
 # https://docs.docker.com/compose/compose-file/03-compose-file/
 DOCKER_COMPOSE_FILENAME_SET = {
     'compose.yaml',
     'compose.yml',
     'docker-compose.yaml',
     'docker-compose.yml',
@@ -44,14 +41,17 @@
 COMMAND_CLEAN_BUILDER = ('Remove build cache', ['docker', 'builder', 'prune', '-f'])
 COMMANDS_CLEAN = [
     COMMAND_CLEAN_NETWORKS,
     COMMAND_CLEAN_IMAGES,
     COMMAND_CLEAN_BUILDER,
 ]
 
+logger = logging.getLogger(__name__)
+shell_args = None
+
 
 def _assert(expr, msg=''):
     if not expr:
         raise AssertionError(msg)
 
 
 def _init_logging():
@@ -74,17 +74,15 @@
     logging.addLevelName(logging.CRITICAL, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.CRITICAL)))
     logging.addLevelName(logging.ERROR, '\x1b[31m{}\x1b[39m'.format(logging.getLevelName(logging.ERROR)))
     logging.addLevelName(logging.WARNING, '\x1b[33m{}\x1b[39m'.format(logging.getLevelName(logging.WARNING)))
     logging.addLevelName(logging.INFO, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.INFO)))
     logging.addLevelName(logging.DEBUG, '\x1b[36m{}\x1b[39m'.format(logging.getLevelName(logging.DEBUG)))
 
 
-def _parse_args():
-    global shell_args
-
+def _parse_args(args=sys.argv[1:]):
     default_docker_files_dir = '.'
 
     parser = argparse.ArgumentParser(
         description=VERSION_STR_LONG,
         formatter_class=argparse.RawDescriptionHelpFormatter,
         add_help=True
     )
@@ -100,32 +98,30 @@
 
     dc_opt_group = parser.add_argument_group('docker-compose options')
     dc_opt_group.add_argument('--dokill', action='store_true', help='Run "docker-compose kill" instead of "docker-compose stop"')
     dc_opt_group.add_argument('--normi', action='store_true', help='Do NOT remove Docker images when running "docker-compose down"')
     dc_opt_group.add_argument('--nopull', action='store_true', help='Do NOT pull images when running "docker-compose build"')
     dc_opt_group.add_argument('--doclean', action='store_true', help='Clean up before exit, if no error. Remove ALL unused networks, images and build cache. WARN: This may cause data loss.')
 
-    parser.add_argument('docker_files_dir', metavar='dir_path', nargs='?', default=default_docker_files_dir, help=f'A directory which contains Docker Compose projects, default: {default_docker_files_dir!r}')
+    parser.add_argument('docker_files_dir', metavar='dir_path', nargs='?', default=default_docker_files_dir, help='A directory which contains Docker Compose projects, default: %(default)r')
 
-    parser.add_argument('-V', '--version', action='store_true', help='Show version and exit')
+    parser.add_argument('-V', '--version', action='version', version=VERSION_STR_LONG, help='Show version and exit')
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase verbosity level (use -vv or more for greater effect)')
 
-    shell_args = parser.parse_args()
+    result = parser.parse_args(args)
 
-    if shell_args.verbose >= 1:
+    if result.verbose >= 1:
         logging.root.setLevel(logging.DEBUG)
     
-    shell_args.docker_files_dir = os.path.abspath(os.path.expanduser(shell_args.docker_files_dir))
-    _assert(os.path.isdir(shell_args.docker_files_dir), f'Dir not found: {shell_args.docker_files_dir!r}')
+    result.docker_files_dir = os.path.abspath(os.path.expanduser(result.docker_files_dir))
+    _assert(os.path.isdir(result.docker_files_dir), f'Dir not found: {result.docker_files_dir!r}')
 
-    logger.debug('Command line arguments: %r', shell_args)
+    logger.debug('Command line arguments: %r', result)
 
-    if shell_args.version:
-        print(VERSION_STR_LONG)
-        sys.exit(0)
+    return result
 
 
 def colored(s, foreground, background=None, **kwargs):
     if kwargs.get('repr', False):
         s = repr(s)
     else:
         s = str(s)
@@ -273,14 +269,19 @@
         COMMAND_BUILD = ['docker-compose', 'build']
 
     if shell_args.dokill:
         COMMAND_STOP = ['docker-compose', 'kill']
 
 
 def main():
+    global shell_args
+
+    _init_logging()
+    shell_args = _parse_args()
+
     if sys.stdout.isatty():
         atexit.register(lambda: logger.info('Exiting'))
     else:
         atexit.register(lambda: logger.info('Exiting\n'))
 
     _start_time_stamp = time.time()
     atexit.register(lambda: logger.info('Time elapsed: %s', timedelta(seconds=int(time.time() - _start_time_stamp))))
@@ -330,20 +331,9 @@
     else:
         if shell_args.doclean:
             clean()
 
         logger.info('Command %s exit with no error', colored(get_command_str(sys.argv), 'default', bold=True))
 
 
-def _main():
-    _init_logging()
-    _parse_args()
-
-    try:
-        main()
-    except Exception as e:
-        logger.exception('%r: %r', type(e), e)
-        sys.exit(1)
-
-
 if __name__ == '__main__':
-    _main()
+    main()
```

### Comparing `docker-compose-all-0.2.1/setup.py` & `docker-compose-all-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     license='GNU General Public License v3.0',
     packages=[],
     py_modules = ['docker_compose_all'],
     install_requires=[],
     include_package_data=True,
     entry_points={
         'console_scripts': [
-            'docker-compose-all=docker_compose_all:_main'
+            'docker-compose-all=docker_compose_all:main'
         ]
     },
     classifiers=[
         'Environment :: Console',
         'Operating System :: POSIX',
         'Operating System :: POSIX :: Linux',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
```

