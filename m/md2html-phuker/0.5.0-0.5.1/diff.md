# Comparing `tmp/md2html-phuker-0.5.0.tar.gz` & `tmp/md2html-phuker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2html-phuker-0.5.0.tar", last modified: Tue Apr 18 15:56:00 2023, max compression
+gzip compressed data, was "md2html-phuker-0.5.1.tar", last modified: Wed Apr 26 12:19:31 2023, max compression
```

## Comparing `md2html-phuker-0.5.0.tar` & `md2html-phuker-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/Readme.PyPI.md
--rw-r--r--   0 root         (0) root         (0)     5799 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.856723 md2html-phuker-0.5.0/md2html/
--rwxr-xr-x   0 root         (0) root         (0)     9671 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16608 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/github-markdown.css
--rw-r--r--   0 root         (0) root         (0)     3144 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/main.css
--rw-r--r--   0 root         (0) root         (0)     4394 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/pygments.css
--rw-r--r--   0 root         (0) root         (0)     1063 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/style-dark.css
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/md2html/style-sidebar-toc.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:00.856723 md2html-phuker-0.5.0/md2html_phuker.egg-info/
--rw-r--r--   0 root         (0) root         (0)      759 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-18 15:56:00.000000 md2html-phuker-0.5.0/md2html_phuker.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-04-18 15:56:00.860722 md2html-phuker-0.5.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1193 2023-04-18 15:55:06.000000 md2html-phuker-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/Readme.PyPI.md
+-rw-r--r--   0 root         (0) root         (0)     5895 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.876824 md2html-phuker-0.5.1/md2html/
+-rwxr-xr-x   0 root         (0) root         (0)     9586 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16608 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/github-markdown.css
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/main.css
+-rw-r--r--   0 root         (0) root         (0)     4394 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/pygments.css
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/style-dark.css
+-rw-r--r--   0 root         (0) root         (0)      419 2023-04-26 12:19:09.000000 md2html-phuker-0.5.1/md2html/style-sidebar-toc.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/md2html_phuker.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 12:19:31.000000 md2html-phuker-0.5.1/md2html_phuker.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-04-26 12:19:31.884824 md2html-phuker-0.5.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1193 2023-04-26 12:19:08.000000 md2html-phuker-0.5.1/setup.py
```

### Comparing `md2html-phuker-0.5.0/LICENSE` & `md2html-phuker-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.0/PKG-INFO` & `md2html-phuker-0.5.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `md2html-phuker-0.5.0/Readme.md` & `md2html-phuker-0.5.1/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -63,36 +63,38 @@
 
 ## Usage
 
 ### Show help
 
 ```console
 $ md2html --help
-usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert HTML] [--body-append HTML] [input_file]
+usage: md2html [-h] [-t TITLE] [-f] [-o FILE] [--style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert HTML] [--body-append HTML] [-V] [-v] [input_file]
 
+md2html version 0.5.0
 Yet another markdown to html converter, generate an offline all-in-one single HTML file.
+https://github.com/Phuker/md2html
 
 positional arguments:
   input_file            If omitted or "-", use stdin.
 
 options:
   -h, --help            show this help message and exit
-  -v, --verbose         Verbose output
-  -V, --version         Output version info and exit
   -t TITLE, --title TITLE
                         If omitted, generate from input filename
   -f, --force           Force overwrite if output file exists
   -o FILE, --output-file FILE
                         If omitted, auto decide. If "-", stdout.
   --style PRESET        Preset style addons, choices: sidebar-toc, dark
   --append-css FILE     Append embedded CSS files, may specify multiple times.
   --head-insert HTML    HTML to insert to the start of <head>, may specify multiple times.
   --head-append HTML    HTML to append to the end of <head>, may specify multiple times.
   --body-insert HTML    HTML to insert to the start of <body>, may specify multiple times.
   --body-append HTML    HTML to append to the end of <body>, may specify multiple times.
+  -V, --version         Show version and exit
+  -v, --verbose         Increase verbosity level (use -vv or more for greater effect)
 ```
 
 If you are not sure about what will happen if you combine `[-o FILE]`, `[input_file]` and `[-t TITLE]`, see `test.py`, which contains tens of input cases and their intended behaviors.
 
 ### Convert a file
 
 Generate `foo.html` in the same dir, with HTML title `foo`:
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_o8npswei_/tmpqf2x8t9a_TarContainer/0/5.md", line 175, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_o8npswei_/tmpqf2x8t9a_TarContainer/0/5.md", line 175, column 0: CDATA terminal not found*

```diff
@@ -29,32 +29,34 @@
 dark.html](https://phuker.github.io/md2html/demo-sidebar-toc-dark.html) All
 above files are generated from [docs/demo.md](./docs/demo.md). You can view its
 content to see supported syntax. ## Requirements - Python >= `3.6`, with `pip`
 installed ## Install ```bash python3 -m pip install -U md2html-phuker ``` There
 are too many similar projects with similar names in PyPI, `md2html`, `md-to-
 html`, `markdown2html`, `markdown-to-html`, `mrkdwn2html` ... I have to add a
 suffix to keep away from this war of naming. ## Usage ### Show help ```console
-$ md2html --help usage: md2html [-h] [-v] [-V] [-t TITLE] [-f] [-o FILE] [--
-style PRESET] [--append-css FILE] [--head-insert HTML] [--head-append HTML] [--
-body-insert HTML] [--body-append HTML] [input_file] Yet another markdown to
-html converter, generate an offline all-in-one single HTML file. positional
-arguments: input_file If omitted or "-", use stdin. options: -h, --help show
-this help message and exit -v, --verbose Verbose output -V, --version Output
-version info and exit -t TITLE, --title TITLE If omitted, generate from input
-filename -f, --force Force overwrite if output file exists -o FILE, --output-
-file FILE If omitted, auto decide. If "-", stdout. --style PRESET Preset style
-addons, choices: sidebar-toc, dark --append-css FILE Append embedded CSS files,
-may specify multiple times. --head-insert HTML HTML to insert to the start of
+$ md2html --help usage: md2html [-h] [-t TITLE] [-f] [-o FILE] [--style PRESET]
+[--append-css FILE] [--head-insert HTML] [--head-append HTML] [--body-insert
+HTML] [--body-append HTML] [-V] [-v] [input_file] md2html version 0.5.0 Yet
+another markdown to html converter, generate an offline all-in-one single HTML
+file. https://github.com/Phuker/md2html positional arguments: input_file If
+omitted or "-", use stdin. options: -h, --help show this help message and exit
+-t TITLE, --title TITLE If omitted, generate from input filename -f, --force
+Force overwrite if output file exists -o FILE, --output-file FILE If omitted,
+auto decide. If "-", stdout. --style PRESET Preset style addons, choices:
+sidebar-toc, dark --append-css FILE Append embedded CSS files, may specify
+multiple times. --head-insert HTML HTML to insert to the start of
 , may specify multiple times. --head-append HTML HTML to append to the end of
 , may specify multiple times. --body-insert HTML HTML to insert to the start of
 , may specify multiple times. --body-append HTML HTML to append to the end of
-, may specify multiple times. ``` If you are not sure about what will happen if
-you combine `[-o FILE]`, `[input_file]` and `[-t TITLE]`, see `test.py`, which
-contains tens of input cases and their intended behaviors. ### Convert a file
-Generate `foo.html` in the same dir, with HTML title `foo`: ```bash md2html
-foo.md ``` Force overwrite output file if it exists: ```bash md2html -f foo.md
-``` ### Convert from pipe and/or to pipe Read from `stdin`, output to `stdout`,
-specify HTML title: ```bash md2html --title 'baz'
+, may specify multiple times. -V, --version Show version and exit -v, --verbose
+Increase verbosity level (use -vv or more for greater effect) ``` If you are
+not sure about what will happen if you combine `[-o FILE]`, `[input_file]` and
+`[-t TITLE]`, see `test.py`, which contains tens of input cases and their
+intended behaviors. ### Convert a file Generate `foo.html` in the same dir,
+with HTML title `foo`: ```bash md2html foo.md ``` Force overwrite output file
+if it exists: ```bash md2html -f foo.md ``` ### Convert from pipe and/or to
+pipe Read from `stdin`, output to `stdout`, specify HTML title: ```bash md2html
+--title 'baz'
 md >bar.html cat foo.md | md2html -t 'baz' >bar.html ``` Send output to the
 screen, and write the same contents to a file: ```bash md2html foo.md -o - |
 tee bar.html ``` ### Modify generated HTML file Append CSS files, embed their
 contents inside `
```

### Comparing `md2html-phuker-0.5.0/md2html/__init__.py` & `md2html-phuker-0.5.1/md2html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 import markdown.extensions.toc
 import markdown.extensions.nl2br
 import markdown.extensions.admonition
 import markdown_link_attr_modifier
 import gfm
 
 
-__version__ = '0.5.0'
-logger = logging.getLogger(__name__)
+__version__ = '0.5.1'
+VERSION_STR_SHORT = f'md2html {__version__}'
+VERSION_STR_LONG = f'md2html {__version__}\n{__doc__.strip()}'
 
-VERSION_STR_SHORT = f'md2html version {__version__}'
-VERSION_STR_LONG = f'md2html version {__version__}\n{__doc__.strip()}'
+logger = logging.getLogger(__name__)
 
 
 def _assert(expr, msg=''):
     if not expr:
         raise AssertionError(msg)
 
 
@@ -73,24 +73,24 @@
     )
 
     parser.add_argument('-t', '--title', help='If omitted, generate from input filename')
     parser.add_argument('-f', '--force', action='store_true', help='Force overwrite if output file exists')
     parser.add_argument('input_file', nargs='?', help='If omitted or "-", use stdin.')
     parser.add_argument('-o', '--output-file', metavar='FILE', dest='output_file', help='If omitted, auto decide. If "-", stdout.')
 
-    parser.add_argument('--style', metavar='PRESET', action='append', default=[], choices=choices_style, help=f'Preset style addons, choices: {", ".join(choices_style)}')
+    parser.add_argument('--style', metavar='PRESET', action='append', default=[], choices=choices_style, help='Preset style addons, choices: %(choices)s')
 
     parser.add_argument('--append-css', metavar='FILE', action='append', default=[], help='Append embedded CSS files, may specify multiple times.')
 
     parser.add_argument('--head-insert', metavar='HTML', action='append', default=[], help='HTML to insert to the start of <head>, may specify multiple times.')
     parser.add_argument('--head-append', metavar='HTML', action='append', default=[], help='HTML to append to the end of <head>, may specify multiple times.')
     parser.add_argument('--body-insert', metavar='HTML', action='append', default=[], help='HTML to insert to the start of <body>, may specify multiple times.')
     parser.add_argument('--body-append', metavar='HTML', action='append', default=[], help='HTML to append to the end of <body>, may specify multiple times.')
 
-    parser.add_argument('-V', '--version', action='store_true', help='Show version and exit')
+    parser.add_argument('-V', '--version', action='version', version=VERSION_STR_LONG, help='Show version and exit')
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase verbosity level (use -vv or more for greater effect)')
 
     result = parser.parse_args(args)
 
     if result.verbose >= 1:
         logging.root.setLevel(logging.DEBUG)
 
@@ -125,18 +125,14 @@
     result.append_css = [os.path.abspath(os.path.expanduser(_)) for _ in result.append_css]
 
     # set result.script_dir
     result.script_dir = os.path.abspath(os.path.dirname(__file__))
 
     logger.debug('Command line arguments: %r', result)
 
-    if result.version:
-        print(VERSION_STR_LONG)
-        sys.exit(0)
-
     return result
 
 
 # obj: fd or str
 def read_file(obj):
     if isinstance(obj, str):
         logger.info('Reading %r', obj)
```

### Comparing `md2html-phuker-0.5.0/md2html/github-markdown.css` & `md2html-phuker-0.5.1/md2html/github-markdown.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.0/md2html/main.css` & `md2html-phuker-0.5.1/md2html/main.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.0/md2html/pygments.css` & `md2html-phuker-0.5.1/md2html/pygments.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.0/md2html/style-dark.css` & `md2html-phuker-0.5.1/md2html/style-dark.css`

 * *Files identical despite different names*

### Comparing `md2html-phuker-0.5.0/md2html_phuker.egg-info/PKG-INFO` & `md2html-phuker-0.5.1/md2html_phuker.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2html-phuker
-Version: 0.5.0
+Version: 0.5.1
 Summary: Yet another markdown to html converter, generate an offline all-in-one single HTML file.
 Home-page: https://github.com/Phuker/md2html
 Author: Phuker
 Author-email: Phuker@users.noreply.github.com
 License: GNU General Public License v3.0
 Keywords: markdown html convert
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `md2html-phuker-0.5.0/setup.py` & `md2html-phuker-0.5.1/setup.py`

 * *Files identical despite different names*

