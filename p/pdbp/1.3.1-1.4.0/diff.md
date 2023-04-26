# Comparing `tmp/pdbp-1.3.1.tar.gz` & `tmp/pdbp-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbp-1.3.1.tar", last modified: Wed Apr 19 18:40:42 2023, max compression
+gzip compressed data, was "pdbp-1.4.0.tar", last modified: Wed Apr 26 19:53:08 2023, max compression
```

## Comparing `pdbp-1.3.1.tar` & `pdbp-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.433124 pdbp-1.3.1/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.3.1/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.3.1/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.3.1/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.3.1/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.3.1/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     6294 2023-04-19 18:40:42.433176 pdbp-1.3.1/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     4278 2023-04-19 18:37:55.000000 pdbp-1.3.1/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.3.1/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-19 18:40:42.433332 pdbp-1.3.1/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-19 18:37:55.000000 pdbp-1.3.1/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.432404 pdbp-1.3.1/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.3.1/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-19 18:40:42.433027 pdbp-1.3.1/src/pdbp.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     6294 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-19 18:40:42.000000 pdbp-1.3.1/src/pdbp.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    52815 2023-04-19 18:37:55.000000 pdbp-1.3.1/src/pdbp.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.885245 pdbp-1.4.0/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 pdbp-1.4.0/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1536 2022-11-28 00:30:19.000000 pdbp-1.4.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1664 2022-11-28 00:28:34.000000 pdbp-1.4.0/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1066 2022-11-28 00:19:16.000000 pdbp-1.4.0/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 pdbp-1.4.0/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     6298 2023-04-26 19:53:08.885299 pdbp-1.4.0/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     4282 2023-04-26 19:51:46.000000 pdbp-1.4.0/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      303 2022-11-28 07:12:13.000000 pdbp-1.4.0/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-26 19:53:08.885477 pdbp-1.4.0/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5324 2023-04-26 19:51:46.000000 pdbp-1.4.0/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.884357 pdbp-1.4.0/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       39 2022-11-28 05:30:45.000000 pdbp-1.4.0/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-26 19:53:08.885122 pdbp-1.4.0/src/pdbp.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     6298 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      293 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      121 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-04-26 19:53:08.000000 pdbp-1.4.0/src/pdbp.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    54036 2023-04-26 19:51:46.000000 pdbp-1.4.0/src/pdbp.py
```

### Comparing `pdbp-1.3.1/.gitignore` & `pdbp-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.1/CODE_OF_CONDUCT.md` & `pdbp-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.1/CONTRIBUTING.md` & `pdbp-1.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.1/LICENSE` & `pdbp-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbp-1.3.1/PKG-INFO` & `pdbp-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.3.1
+Version: 1.4.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,25 +44,25 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -101,17 +101,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbp-1.3.1/README.md` & `pdbp-1.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -53,17 +53,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbp-1.3.1/setup.py` & `pdbp-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="pdbp",
-    version="1.3.1",
+    version="1.4.0",
     description="pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="pdb debugger tab color completion",
     url="https://github.com/mdmintz/pdbp",
     project_urls={
         "Changelog": "https://github.com/mdmintz/pdbp/releases",
```

### Comparing `pdbp-1.3.1/src/pdbp.egg-info/PKG-INFO` & `pdbp-1.4.0/src/pdbp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbp
-Version: 1.3.1
+Version: 1.4.0
 Summary: pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 Home-page: https://github.com/mdmintz/pdbp
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/pdbp/releases
@@ -44,25 +44,25 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pdbp (Pdb+) [![](https://img.shields.io/pypi/v/pdbp.svg)](https://pypi.python.org/pypi/pdbp)
 
-<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/207774790-fb63af65-5f98-4d92-afe3-12c2733d4db6.png">
+<img width="650" alt="Pdb+ Advanced Python Console Debugger" src="https://user-images.githubusercontent.com/6788579/234679015-b1daa50f-94a8-4ef2-b3f5-3157b7a3733b.png">
 
 --------
 
 **[pdbp (Pdb+)](https://github.com/mdmintz/pdbp)** is an advanced console debugger for Python. It can be used as a drop-in replacement for ``pdb`` and [pdbpp](https://github.com/pdbpp/pdbpp).
 
 <p><b>pdbp (Pdb+)</b> makes Python debugging a lot easier (and more fun!)</p>
 
 --------
 
-<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/232536483-9236c513-c5ba-4444-8faa-e8ea64eb5ce2.png">
+<img width="650" alt="Pdb+" src="https://user-images.githubusercontent.com/6788579/234669562-30dae4ad-1207-47e4-8327-fbd5662c8b9c.png">
 
 
 ## Installation & Usage:
 
 ```bash
 pip install pdbp
 ```
@@ -101,17 +101,17 @@
 ```
 
 Here's how to customize **``pdbp``**/``pdb`` options if you don't like the default settings: (<i>Shown below are the default settings.</i>)
 
 ```python
 import pdb
 if hasattr(pdb, "DefaultConfig"):
-    pdb.DefaultConfig.filename_color = pdb.Color.blue
+    pdb.DefaultConfig.filename_color = pdb.Color.fuchsia
     pdb.DefaultConfig.line_number_color = pdb.Color.turquoise
-    pdb.DefaultConfig.truncate_long_lines = True
+    pdb.DefaultConfig.truncate_long_lines = False
     pdb.DefaultConfig.sticky_by_default = True
 ```
 
 You can also trigger **``Pdb+``** activation like this:
 
 ```python
 import pdbp
```

### Comparing `pdbp-1.3.1/src/pdbp.py` & `pdbp-1.4.0/src/pdbp.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pdbp (Pdb+): A drop-in replacement for pdb and pdbpp.
 =====================================================
 """
 from __future__ import print_function
 import code
 import codecs
 import inspect
+import math
 import os.path
 import pprint
 import re
 import signal
 import sys
 import traceback
 import types
@@ -67,15 +68,15 @@
     line_length = len(line)
     for char in line:
         if is_char_wide(char):
             line_length += 1
     return line_length
 
 
-def set_line_width(line, width):
+def set_line_width(line, width, tll=True):
     """Trim line if too long. Fill line if too short. Return line."""
     line_width = get_width(line)
     new_line = ""
     width = int(width)
     if width <= 0:
         return new_line
     elif line_width == width:
@@ -84,30 +85,32 @@
         new_line = line
     else:
         for char in line:
             updated_line = "%s%s" % (new_line, char)
             if get_width(updated_line) > width:
                 break
             new_line = updated_line
-    extra_spaces = " " * (width - get_width(new_line))
+    extra_spaces = ""
+    if tll:
+        extra_spaces = " " * (width - get_width(new_line))
     return "%s%s" % (new_line, extra_spaces)
 
 
 class DefaultConfig(object):
     prompt = "(Pdb+) "
     highlight = True
     sticky_by_default = True
     bg = "dark"
     use_pygments = True
     colorscheme = None
     use_terminal256formatter = None  # Defaults to `"256color" in $TERM`.
     editor = "${EDITOR:-vi}"  # Use $EDITOR if set; else default to vi.
     stdin_paste = None
     exec_if_unfocused = None  # This option was removed!
-    truncate_long_lines = True
+    truncate_long_lines = False
     disable_pytest_capturing = True
     enable_hidden_frames = False
     show_hidden_frames_count = False
     encodings = ("utf-8", "latin-1")
     filename_color = Color.fuchsia
     line_number_color = Color.turquoise
     regular_stack_color = Color.yellow
@@ -459,14 +462,15 @@
     def format_stack_entry(self, frame_lineno, lprefix=": "):
         entry = super().format_stack_entry(frame_lineno, lprefix)
         entry = self.try_to_decode(entry)
         if self.config.highlight:
             match = self.stack_entry_regexp.match(entry)
             if match:
                 filename, lineno, other = match.groups()
+                other = self.format_source(other.rstrip()).rstrip()
                 filename = Color.set(self.config.filename_color, filename)
                 lineno = Color.set(self.config.line_number_color, lineno)
                 entry = "%s(%s)%s" % (filename, lineno, other)
         return entry
 
     def try_to_decode(self, s):
         for encoding in self.config.encodings:
@@ -619,16 +623,17 @@
         else:
             try:
                 self.curframe.f_lineno = arg
                 self.stack[self.curindex] = self.stack[self.curindex][0], arg
                 self.print_current_stack_entry()
             except ValueError as e:
                 self.error('Jump failed: %s' % e)
+    do_j = do_jump
 
-    def _printlonglist(self, linerange=None, fnln=None):
+    def _printlonglist(self, linerange=None, fnln=None, nc_fnln=""):
         try:
             if self.curframe.f_code.co_name == "<module>":
                 lines, _ = inspect.findsource(self.curframe)
                 lineno = 1
             else:
                 try:
                     lines, lineno = inspect.getsourcelines(self.curframe)
@@ -651,17 +656,19 @@
                 return
         if linerange:
             start, end = linerange
             start = max(start, lineno)
             end = min(end, lineno + len(lines))
             lines = lines[start - lineno:end - lineno]
             lineno = start
-        self._print_lines_pdbp(lines, lineno, fnln=fnln)
+        self._print_lines_pdbp(lines, lineno, fnln=fnln, nc_fnln=nc_fnln)
 
-    def _print_lines_pdbp(self, lines, lineno, print_markers=True, fnln=None):
+    def _print_lines_pdbp(
+        self, lines, lineno, print_markers=True, fnln=None, nc_fnln=""
+    ):
         dots = "..."
         offset = 0
         try:
             lineno_int = int(lineno)
         except Exception:
             lineno = 1
             lineno_int = 1
@@ -681,38 +688,51 @@
             dots = "   ."
         max_line = int(lineno) + len(lines) - 1
         if max_line > 9999:
             offset = 1
         if max_line > 99999:
             offset = 2
         exc_lineno = self.tb_lineno.get(self.curframe, None)
-        lines = [line[:-1] for line in lines]  # remove the trailing "\n"
         lines = [line.replace("\t", "    ")
                  for line in lines]  # force tabs to 4 spaces
+        lines = [line.rstrip() for line in lines]
         width, height = self.get_terminal_size()
         width = width - offset
         height = height - 1
+        overflow = 0
+        height_counter = height
+        if not self.config.truncate_long_lines:
+            for line in lines:
+                if len(line) > width - 9:
+                    overflow += 1
+                height_counter -= 1
+                if height_counter <= 0:
+                    break
         if self.config.truncate_long_lines:
             maxlength = max(width - 9, 16)
             lines = [set_line_width(line, maxlength) for line in lines]
         else:
             maxlength = max(map(len, lines))
         if self.config.highlight:
             # Fill line with spaces. This is important when a bg color is
             # is used for highlighting the current line (via setbgcolor).
-            lines = [set_line_width(line, maxlength) for line in lines]
+            tll = self.config.truncate_long_lines
+            lines = [set_line_width(line, maxlength, tll) for line in lines]
             src = self.format_source("\n".join(lines))
             lines = src.splitlines()
         if height >= 6:
             last_marker_line = max(
                 self.curframe.f_lineno,
                 exc_lineno if exc_lineno else 0
             ) - lineno
             if last_marker_line >= 0:
-                maxlines = last_marker_line + height * 2 // 3
+                more_overflow = int(len(nc_fnln) / width)
+                overflow = overflow + more_overflow
+                maxlines = last_marker_line + (height * 2 // 3)
+                maxlines = maxlines - math.ceil(overflow * 1 / 3)
                 if len(lines) > maxlines:
                     lines = lines[:maxlines]
                     lines.append(Color.set("39;49;1", "..."))
         self.config.exception_caught = False
         for i, line in enumerate(lines):
             marker = ""
             if lineno == self.curframe.f_lineno and print_markers:
@@ -942,16 +962,17 @@
             lno = Color.set(self.config.line_number_color, "%r" % lineno)
             fname = Color.set(self.config.filename_color, filename)
             fnln = None
             if not self.curindex:
                 self.curindex = 0
             colored_index = Color.set(self.config.stack_color, self.curindex)
             fnln = "[%s] > %s(%s)" % (colored_index, fname, lno)
+            nc_fnln = "[%s] > %s(%s)" % (self.curindex, filename, lineno)
             sticky_range = self.sticky_ranges.get(self.curframe, None)
-            self._printlonglist(sticky_range, fnln=fnln)
+            self._printlonglist(sticky_range, fnln=fnln, nc_fnln=nc_fnln)
             needs_extra_line = False
             if "__exception__" in frame.f_locals:
                 s = self._format_exc_for_sticky(
                     frame.f_locals["__exception__"]
                 )
                 if s:
                     last_return_color = self.config.last_return_color
@@ -1029,16 +1050,17 @@
             self._print_if_sticky()
         else:
             print(file=self.stdout)
             self.print_stack_entry(self.stack[self.curindex])
             print(file=self.stdout, end="\n\033[F")
 
     def do_truncate(self, arg):
-        # Toggle line truncation. Usage: "truncate".
-        # (The changes only appear in "sticky" mode.)
+        # Toggle line truncation. Usage: "truncate" / "trun".
+        # (Changes only appear when "sticky" mode is active.)
+        # When enabled, all lines take on the screen width.
         self.config.truncate_long_lines = not self.config.truncate_long_lines
         self.print_current_stack_entry()
     do_trun = do_truncate
 
     def print_stack_trace(self):
         try:
             for frame_index, frame_lineno in enumerate(self.stack):
@@ -1107,15 +1129,23 @@
             return None, None, None
         return filename, lineno, lines
 
     def do_source(self, arg):
         _, lineno, lines = self._get_position_of_arg(arg)
         if lineno is None:
             return
-        self._print_lines_pdbp(lines, lineno, print_markers=False)
+        try:
+            frame = self.curframe
+            filename = self.canonic(frame.f_code.co_filename)
+            nc_fnln = "[%s] > %s(%s)" % (self.curindex, filename, lineno)
+            self._print_lines_pdbp(
+                lines, lineno, print_markers=False, nc_fnln=nc_fnln
+            )
+        except Exception:
+            self._print_lines_pdbp(lines, lineno, print_markers=False)
 
     def do_frame(self, arg):
         try:
             arg = int(arg)
         except (ValueError, TypeError):
             print(
                 '*** Expected a number, got "{0}"'.format(arg),
```

