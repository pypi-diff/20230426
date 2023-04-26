# Comparing `tmp/nua_lib-0.5.14.tar.gz` & `tmp/nua_lib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_lib-0.5.14.tar", max compression
+gzip compressed data, was "nua_lib-0.5.9.tar", max compression
```

## Comparing `nua_lib-0.5.14.tar` & `nua_lib-0.5.9.tar`

### file list

```diff
@@ -1,23 +1,16 @@
--rw-r--r--   0        0        0      791 2023-04-24 21:25:56.867782 nua_lib-0.5.14/README.md
--rw-r--r--   0        0        0     1241 2023-04-26 06:46:32.426719 nua_lib-0.5.14/pyproject.toml
--rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.14/src/nua/lib/__init__.py
--rw-r--r--   0        0        0     1281 2023-04-26 06:41:08.605864 nua_lib-0.5.14/src/nua/lib/actions/__init__.py
--rw-r--r--   0        0        0     3944 2023-04-26 06:41:08.606054 nua_lib-0.5.14/src/nua/lib/actions/apt.py
--rw-r--r--   0        0        0       40 2023-04-26 06:41:08.606249 nua_lib-0.5.14/src/nua/lib/actions/constants.py
--rw-r--r--   0        0        0     3042 2023-04-26 06:41:08.606376 nua_lib-0.5.14/src/nua/lib/actions/misc.py
--rw-r--r--   0        0        0     2225 2023-04-26 06:41:08.606496 nua_lib-0.5.14/src/nua/lib/actions/nodejs.py
--rw-r--r--   0        0        0     6158 2023-04-26 06:41:08.606632 nua_lib-0.5.14/src/nua/lib/actions/python.py
--rw-r--r--   0        0        0     1395 2023-04-26 06:41:08.606806 nua_lib-0.5.14/src/nua/lib/actions/ruby.py
--rw-r--r--   0        0        0     7254 2023-04-26 06:41:08.606936 nua_lib-0.5.14/src/nua/lib/actions/util.py
--rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.14/src/nua/lib/backports.py
--rw-r--r--   0        0        0     1621 2023-04-24 21:25:56.869539 nua_lib-0.5.14/src/nua/lib/console.py
--rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.14/src/nua/lib/exec.py
--rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.14/src/nua/lib/gen_password.py
--rw-r--r--   0        0        0     3361 2023-04-24 21:25:56.869718 nua_lib-0.5.14/src/nua/lib/panic.py
--rw-r--r--   0        0        0     3983 2023-04-26 06:41:08.607112 nua_lib-0.5.14/src/nua/lib/shell.py
--rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.14/src/nua/lib/tool/__init__.py
--rw-r--r--   0        0        0     3572 2023-04-24 21:25:56.869858 nua_lib-0.5.14/src/nua/lib/tool/color_str.py
--rw-r--r--   0        0        0     1420 2023-04-26 05:47:08.293351 nua_lib-0.5.14/src/nua/lib/tool/state.py
--rw-r--r--   0        0        0     2121 2023-04-26 06:41:08.607282 nua_lib-0.5.14/src/nua/lib/unarchiver.py
--rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.14/src/nua/lib/version.py
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 nua_lib-0.5.14/PKG-INFO
+-rw-r--r--   0        0        0      544 2023-02-06 17:21:30.498783 nua_lib-0.5.9/README.md
+-rw-r--r--   0        0        0     1240 2023-04-18 16:37:02.790822 nua_lib-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-02-06 17:21:30.499791 nua_lib-0.5.9/src/nua/lib/__init__.py
+-rw-r--r--   0        0        0    21348 2023-04-18 14:45:14.195218 nua_lib-0.5.9/src/nua/lib/actions.py
+-rw-r--r--   0        0        0      769 2023-01-11 17:39:15.272394 nua_lib-0.5.9/src/nua/lib/backports.py
+-rw-r--r--   0        0        0     1344 2023-04-18 14:45:14.195754 nua_lib-0.5.9/src/nua/lib/console.py
+-rw-r--r--   0        0        0     5600 2023-03-06 16:13:43.253043 nua_lib-0.5.9/src/nua/lib/exec.py
+-rw-r--r--   0        0        0      828 2023-04-08 16:30:34.876808 nua_lib-0.5.9/src/nua/lib/gen_password.py
+-rw-r--r--   0        0        0     1948 2023-04-18 14:45:14.196144 nua_lib-0.5.9/src/nua/lib/panic.py
+-rw-r--r--   0        0        0     3932 2023-04-08 16:18:44.073176 nua_lib-0.5.9/src/nua/lib/shell.py
+-rw-r--r--   0        0        0       60 2023-02-06 17:21:30.499928 nua_lib-0.5.9/src/nua/lib/tool/__init__.py
+-rw-r--r--   0        0        0     3509 2023-04-08 16:30:35.028834 nua_lib-0.5.9/src/nua/lib/tool/color_str.py
+-rw-r--r--   0        0        0     1133 2023-02-13 14:04:49.214475 nua_lib-0.5.9/src/nua/lib/tool/state.py
+-rw-r--r--   0        0        0     2077 2023-03-21 16:25:52.745820 nua_lib-0.5.9/src/nua/lib/unarchiver.py
+-rw-r--r--   0        0        0       79 2023-01-03 14:14:59.347734 nua_lib-0.5.9/src/nua/lib/version.py
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 nua_lib-0.5.9/PKG-INFO
```

### Comparing `nua_lib-0.5.14/pyproject.toml` & `nua_lib-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-lib"
-version = "0.5.14"
+version = "0.5.9"
 description = "Nua common library"
 authors = ["Stefane Fermigier <sf@abilian.com>", "Jerome Dumonteil <jd@abilian.com>"]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
```

### Comparing `nua_lib-0.5.14/src/nua/lib/backports.py` & `nua_lib-0.5.9/src/nua/lib/backports.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.14/src/nua/lib/console.py` & `nua_lib-0.5.9/src/nua/lib/console.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,59 +17,39 @@
 
 @if_color
 def print_green(msg: str):
     print(ColorStr.green(msg))
 
 
 @if_color
-def print_gray(msg: str):
-    print(ColorStr.gray(msg))
-
-
-@if_color
 def print_blue(msg: str):
     print(ColorStr.blue(msg))
 
 
 @if_color
-def print_bold_blue(msg: str):
-    print(ColorStr.blue_bold(msg))
-
-
-@if_color
 def print_magenta(msg: str):
     print(ColorStr.magenta(msg))
 
 
 @if_color
 def print_red(msg: str):
-    print(ColorStr.red(msg))
-
-
-@if_color
-def print_bold_red(msg: str):
     print(ColorStr.red_bold(msg))
 
 
 @if_color
 def print_bold(msg: str):
     print(ColorStr.colorize(msg, bold=True))
 
 
 @if_color
 def print_bold_yellow(msg: str):
     print(ColorStr.yellow_bold(msg))
 
 
 @if_color
-def print_cyan(msg: str):
-    print(ColorStr.cyan(msg))
-
-
-@if_color
 def print_bold_yellow_white(msg: str):
     parts = msg.rsplit(" ", 1)
     if len(parts) == 2:
         print(ColorStr.yellow_bold(parts[0]), ColorStr.white_bold(parts[1]))
     else:
         print(ColorStr.yellow_bold(msg))
 
@@ -80,10 +60,10 @@
     if len(parts) == 2:
         print(ColorStr.green(parts[0]), ColorStr.cyan(parts[1]))
     else:
         print(ColorStr.green(msg))
 
 
 @if_color
-def print_magenta_no_lf(msg: str):
+def print_blue_bright_no_lf(msg: str):
     """Print specialized for lines including a LF (Docker build log)."""
-    print(ColorStr.magenta(msg), end="")
+    print(ColorStr.blue_bright(msg), end="")
```

### Comparing `nua_lib-0.5.14/src/nua/lib/exec.py` & `nua_lib-0.5.9/src/nua/lib/exec.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.14/src/nua/lib/gen_password.py` & `nua_lib-0.5.9/src/nua/lib/gen_password.py`

 * *Files identical despite different names*

### Comparing `nua_lib-0.5.14/src/nua/lib/shell.py` & `nua_lib-0.5.9/src/nua/lib/shell.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,34 @@
     with open(filename, encoding="utf8") as fd:
         print(fd.read())
 
 
 def chown_r(path: str | Path, user: str, group: str | None = None):
     """Apply recursively chown with str arguments.
 
-    Similar to `chown -R`.
-
     example:
         chown_r(document_root, "www-data", "www-data")
     """
     root = Path(path)
     for item in root.rglob("*"):
         shutil.chown(item, user, group or user)
     shutil.chown(root, user, group or user)
 
 
+def _dir_chmod_r(root: Path, file_mode: int, dir_mode: int):
+    for subpath in root.rglob(""):
+        if subpath.is_dir():
+            subpath.chmod(dir_mode)
+        else:
+            subpath.chmod(file_mode)
+
+
 def chmod_r(path: str | Path, file_mode: int, dir_mode: int | None = None):
     """Apply recursively chmod with int arguments.
 
-    Similar to `chmod -R` but with int arguments (usually expressed as octal numbers).
-
     example:
         chmod_r(document_root, 0o644, 0o755)
     """
     root = Path(path)
     if dir_mode is None:
         dir_mode = file_mode
     for item in root.rglob("*"):
@@ -44,23 +48,14 @@
             item.chmod(file_mode)
     if root.is_dir():
         root.chmod(dir_mode)
     else:
         root.chmod(file_mode)
 
 
-# XXX: not used
-def _dir_chmod_r(root: Path, file_mode: int, dir_mode: int):
-    for subpath in root.rglob(""):
-        if subpath.is_dir():
-            subpath.chmod(dir_mode)
-        else:
-            subpath.chmod(file_mode)
-
-
 def echo(text: str, filename: str | Path) -> None:
     Path(filename).write_text(text + "\n", encoding="utf8")
 
 
 def mkdir_p(path: str | Path):
     Path(path).mkdir(parents=True, exist_ok=True)
 
@@ -138,14 +133,16 @@
                 f"shell command was: '{cmd}'\n"
                 f"{completed.stdout}\n"
                 f"{completed.stderr}"
             )
             raise Abort(msg, status)
     except OSError as e:
         raise Abort(f"Execution failed: {e}\nshell command was: '{cmd}'")
+        # Not used, actually, but silences warnings.
+        raise SystemExit(1)
 
     if capture_output:
         return completed.stdout
     else:
         return ""
```

### Comparing `nua_lib-0.5.14/src/nua/lib/tool/color_str.py` & `nua_lib-0.5.9/src/nua/lib/tool/color_str.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         kwargs are bools for keys "bright", "bold", "underline" and
         "reversed".
         """
         cmd = cls._command(color=color, bgcolor=bgcolor, **kwargs)
         return f"{cmd}{txt}{cls.COL['reset']}"
 
     black = partialmethod(colorize, color="black")
-    gray = partialmethod(colorize, color="black", bright=True)
     red = partialmethod(colorize, color="red")
     green = partialmethod(colorize, color="green")
     yellow = partialmethod(colorize, color="yellow")
     blue = partialmethod(colorize, color="blue")
     magenta = partialmethod(colorize, color="magenta")
     cyan = partialmethod(colorize, color="cyan")
     white = partialmethod(colorize, color="white")
```

### Comparing `nua_lib-0.5.14/src/nua/lib/tool/state.py` & `nua_lib-0.5.9/src/nua/lib/tool/state.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 import os
 from contextlib import contextmanager
 from functools import cache
 from pathlib import Path
 
-STATE = {
-    "verbose": 0,
-    "colorize": True,
-    "verbose_threshold": -1,
-    "packages_updated": False,
-}
+STATE = {"verbose": 0, "colorize": True, "verbose_threshold": -1}
 
 
 def set_verbosity(value: int):
-    assert isinstance(value, int)
     STATE["verbose"] = value
 
 
 def verbosity_level() -> int:
     return STATE["verbose"]
 
 
 def set_color(flag: bool):
-    assert isinstance(flag, bool)
     STATE["colorize"] = flag
     if flag:
         os.environ.pop("NO_COLOR", None)
     else:
         os.environ["NO_COLOR"] = "1"
 
 
@@ -52,15 +45,7 @@
 @cache
 def is_inside_container() -> bool:
     """Test if current execution environment is inside a container."""
     try:
         return Path("/nua/metadata/nua-config.json").is_file()
     except PermissionError:
         return False
-
-
-def set_packages_updated(flag: bool) -> None:
-    STATE["packages_updated"] = flag
-
-
-def packages_updated() -> bool:
-    return bool(STATE.get("packages_updated", False))
```

### Comparing `nua_lib-0.5.14/src/nua/lib/unarchiver.py` & `nua_lib-0.5.9/src/nua/lib/unarchiver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import abc
 import tarfile
 from pathlib import Path
 from zipfile import ZipFile
 
 
-class Unarchiver(abc.ABC):
+class Unarchiver:
     """ABC for unarchivers."""
 
     accepted_suffixes: list[str] = []
 
     @classmethod
     def accept(cls, src: str | Path) -> bool:
         src = str(src)
         for suffix in cls.accepted_suffixes:
             if src.endswith(suffix):
                 return True
         return False
 
     @classmethod
-    @abc.abstractmethod
     def extract(cls, src: str, dest_dir: str) -> None:
         raise NotImplementedError()
 
 
 class TarUnarchiver(Unarchiver):
     accepted_suffixes = [".tar", ".tar.gz", ".tar.bz2", ".tar.xz", ".tgz"]
```

### Comparing `nua_lib-0.5.14/PKG-INFO` & `nua_lib-0.5.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nua-lib
-Version: 0.5.14
+Version: 0.5.9
 Summary: Nua common library
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,21 +12,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: setuptools
 Description-Content-Type: text/markdown
 
 # Nua Lib
 
-[Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service)
+This subproject contains code that is shared between the various Nua subprojects.
 
-This subproject contains code that is shared between the various [Nua](https://nua.rocks/) subprojects.
-
-It is not intended to be useful outside of Nua, and is not intended to be used as a standalone library.
-
-Since the `nua-lib` code beeing used by `nua-agent`, it should have as little dependencies as possible
+The `nua-lib` code beeing used by `nua-agent`, It should have as little dependencies as possible
 
 ## Content
 
 `nua-lib` provides:
 
 - `shell`: shell shortcuts (mostly wrappers above subprocess and shutil)
 - `exec`: shortcuts to execute sub commands like exec_as_root(), exec_as_root()
```

