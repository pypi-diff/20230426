# Comparing `tmp/json_dotenv-0.0.7-py3-none-any.whl.zip` & `tmp/json_dotenv-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14284 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx    14253 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.data/scripts/json-dotenv
--rw-r--r--  2.0 unx    18092 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     7758 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      510 b- defN 19-Sep-03 11:45 json_dotenv-0.0.7.dist-info/RECORD
-6 files, 40706 bytes uncompressed, 13356 bytes compressed:  67.2%
+Zip file size: 14377 bytes, number of entries: 6
+-rwxr-xr-x  2.0 unx    14362 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.data/scripts/json-dotenv
+-rw-r--r--  2.0 unx    18092 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     7857 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      510 b- defN 19-Sep-06 08:38 json_dotenv-0.0.9.dist-info/RECORD
+6 files, 40914 bytes uncompressed, 13449 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: json_dotenv-0.0.7.data/scripts/json-dotenv
+Filename: json_dotenv-0.0.9.data/scripts/json-dotenv
 Comment: 
 
-Filename: json_dotenv-0.0.7.dist-info/LICENSE.txt
+Filename: json_dotenv-0.0.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: json_dotenv-0.0.7.dist-info/METADATA
+Filename: json_dotenv-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: json_dotenv-0.0.7.dist-info/WHEEL
+Filename: json_dotenv-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: json_dotenv-0.0.7.dist-info/top_level.txt
+Filename: json_dotenv-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: json_dotenv-0.0.7.dist-info/RECORD
+Filename: json_dotenv-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `json_dotenv-0.0.7.data/scripts/json-dotenv` & `json_dotenv-0.0.9.data/scripts/json-dotenv`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
-__version__ = '0.0.4'
+__version__ = '0.0.9'
 
 import argparse
 import json
 import os
 import re
 import shutil
 import sys
@@ -35,16 +35,17 @@
 
 from collections import OrderedDict
 
 import logging
 from logging.handlers import WatchedFileHandler
 
 import six
+
 try:
-    from StringIO import CStringIO as StringIO
+    from six.moves import cStringIO as StringIO
 except ImportError:
     from six import StringIO
 
 import dotenv
 
 warnings.filterwarnings('ignore')
 
@@ -146,15 +147,15 @@
 
     return options
 
 
 class JsonDotEnvExit(SystemExit):
     pass
 
-class JsonDotEnv(object):
+class JsonDotEnv(object): # pylint: disable=bad-option-value,useless-object-inheritance
     def __init__(self, options):
         self.options  = options
         self.fcontent = None
 
     @staticmethod
     def flush_sync_file_object(fo):
         """
@@ -184,15 +185,15 @@
 
     @staticmethod
     def raw_string(value):
         def repl_crtl_chars(match):
             s = match.group()
             if six.PY2 and isinstance(s, str):
                 return s.encode('string-escape')
-            elif isinstance(s, six.text_type):
+            if isinstance(s, six.text_type):
                 r = s.encode('unicode-escape')
                 if six.PY3 and isinstance(r, six.binary_type):
                     return six.ensure_text(r)
                 return r
 
             return repr(s)[1:-1]
 
@@ -262,15 +263,15 @@
 
         self.fcontent = StringIO("\n".join(content) + "\n")
 
     def _valid_varname(self, key):
         if not key:
             LOG.error("missing variable name for command %s", self.options.command)
             raise JsonDotEnvExit(1)
-        elif not isinstance(key, six.string_types) \
+        if not isinstance(key, six.string_types) \
              or not MATCH_VAR_NAME("%s=" % key):
             LOG.error("invalid variable name for command %s", self.options.command)
             raise JsonDotEnvExit(2)
 
         return True
 
     def _valid_varvalue(self, value):
@@ -339,14 +340,15 @@
         try:
             fpath = self.file_w_tmp(self.fcontent.getvalue())
 
             for i, key in enumerate(self.options.key):
                 value = self.options.value[i]
                 self._valid_varname(key)
                 self._valid_varvalue(value)
+                #pylint: disable=unused-variable
                 success, k, v = dotenv.set_key(fpath,
                                                key,
                                                value,
                                                self.options.quote)
 
                 if success:
                     continue
```

## Comparing `json_dotenv-0.0.7.dist-info/LICENSE.txt` & `json_dotenv-0.0.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `json_dotenv-0.0.7.dist-info/METADATA` & `json_dotenv-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-dotenv
-Version: 0.0.7
+Version: 0.0.9
 Summary: json-dotenv
 Home-page: https://github.com/decryptus/json-dotenv
 Author: Adrien Delle Cave
 Author-email: pypi@doowan.net
 License: License GPL-2
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -27,14 +27,19 @@
 # json-dotenv project
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-dotenv.svg)](https://pypi.org/project/json-dotenv/)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-dotenv.svg)](https://pypi.org/project/json-dotenv/)
 
 json-dotenv is a free and open-source, we develop it to manipulate and extract envfiles in json format.
 
+## Table of Contents
+1. [Installation](#installation)
+2. [Usage](#usage)
+3. [Commands](#commands)
+
 ## Installation
 
 `pip install json-dotenv`
 
 ## Usage
 
 ```
```

