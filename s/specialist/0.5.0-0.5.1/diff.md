# Comparing `tmp/specialist-0.5.0.tar.gz` & `tmp/specialist-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specialist-0.5.0.tar", last modified: Thu Apr 20 19:16:06 2023, max compression
+gzip compressed data, was "specialist-0.5.1.tar", last modified: Wed Apr 26 20:08:43 2023, max compression
```

## Comparing `specialist-0.5.0.tar` & `specialist-0.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:16:06.639860 specialist-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-20 19:15:59.000000 specialist-0.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-20 19:16:06.639860 specialist-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-20 19:15:59.000000 specialist-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:16:06.639860 specialist-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-20 19:15:59.000000 specialist-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:16:06.639860 specialist-0.5.0/specialist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 19:16:06.000000 specialist-0.5.0/specialist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19758 2023-04-20 19:15:59.000000 specialist-0.5.0/specialist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:43.802691 specialist-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 20:08:34.000000 specialist-0.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-26 20:08:43.802691 specialist-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-04-26 20:08:34.000000 specialist-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 20:08:43.802691 specialist-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-26 20:08:34.000000 specialist-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:08:43.802691 specialist-0.5.1/specialist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 20:08:43.000000 specialist-0.5.1/specialist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21222 2023-04-26 20:08:34.000000 specialist-0.5.1/specialist.py
```

### Comparing `specialist-0.5.0/LICENSE.md` & `specialist-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `specialist-0.5.0/PKG-INFO` & `specialist-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `specialist-0.5.0/README.md` & `specialist-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `specialist-0.5.0/setup.py` & `specialist-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,9 +11,9 @@
     license="MIT",
     long_description=README.read_text(),
     long_description_content_type="text/markdown",
     name="specialist",
     py_modules=["specialist"],
     python_requires=">=3.11",
     url="https://github.com/brandtbucher/specialist",
-    version="0.5.0",
+    version="0.5.1",
 )
```

### Comparing `specialist-0.5.0/specialist.egg-info/PKG-INFO` & `specialist-0.5.1/specialist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specialist
-Version: 0.5.0
+Version: 0.5.1
 Summary: Visualize CPython 3.11's specializing, adaptive interpreter.
 Home-page: https://github.com/brandtbucher/specialist
 Author: Brandt Bucher
 Author-email: brandt@python.org
 License: MIT
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

### Comparing `specialist-0.5.0/specialist.py` & `specialist-0.5.1/specialist.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,20 @@
         "PRECALL_NO_KW_STR_1",
         "PRECALL_NO_KW_TUPLE_1",
         "PRECALL_NO_KW_TYPE_1",
         "STORE_FAST__LOAD_FAST",
         "STORE_FAST__STORE_FAST",
     }
 )
-_LIB = pathlib.Path(
-    os.path.commonpath([sysconfig.get_path("stdlib"), sysconfig.get_path("purelib")])
-).resolve()
-assert _LIB.is_dir()
+_PURELIB = pathlib.Path(sysconfig.get_path("purelib")).resolve()
+assert _PURELIB.is_dir(), _PURELIB
+_STDLIB = pathlib.Path(sysconfig.get_path("stdlib")).resolve()
+assert _STDLIB.is_dir(), _STDLIB
 _TMP = pathlib.Path(tempfile.gettempdir()).resolve()
-assert _TMP.is_dir()
+assert _TMP.is_dir(), _TMP
 
 
 class _HTMLWriter:
     """Write HTML for a source code view."""
 
     def __init__(self, *, blue: bool, dark: bool) -> None:
         self._blue = blue
@@ -187,14 +187,25 @@
     sys.argv[1:] = argv
     try:
         yield
     finally:
         sys.argv[1:] = sys_argv
 
 
+@contextlib.contextmanager
+def _insert_sys_path(path: pathlib.Path) -> typing.Generator[None, None, None]:
+    """Patch sys.path to simulate a normal python execution."""
+    sys_path = sys.path[:]
+    sys.path.insert(0, str(path))
+    try:
+        yield
+    finally:
+        sys.path[:] = sys_path
+
+
 def _main_file_for_module(module: str) -> pathlib.Path | None:
     """Get the main file for a module."""
     spec = importlib.util.find_spec(module)
     if spec is None:
         return None
     if spec.submodule_search_locations is not None:
         spec = importlib.util.find_spec(f"{module}.__main__")
@@ -318,14 +329,20 @@
     assert extra_chunk is None or (
         extra_chunk.start == chunk.stop
         and extra_chunk.stop == _LAST_POSITION
         and extra_chunk.stats == _Stats()
     ), extra_chunk
 
 
+def _is_quickened(code: types.CodeType) -> bool:
+    return any(  # pragma: no cover
+        chunk.stats.specialized or chunk.stats.adaptive for chunk in _parse(code)
+    )
+
+
 def _view(
     path: pathlib.Path,
     *,
     blue: bool = False,
     dark: bool = False,
     out: pathlib.Path | None = None,
     name: str | None = None,
@@ -354,27 +371,40 @@
     return True
 
 
 def _suggest_target_glob(args: typing.Sequence[str]) -> None:
     """Suggest possible glob patterns for targets."""
     paths = [
         path
-        for path in _code
-        # Also filter these for containing quickend code?
-        if path.is_file() and _TMP not in path.parents and _LIB not in path.parents
+        for path, code in _code.items()
+        if path.is_file()
+        and _PURELIB not in path.parents
+        and _STDLIB not in path.parents
+        and _TMP not in path.parents
+        and _is_quickened(code)
     ]
     if not paths:
         return
     if len(paths) == 1:
         glob = paths[0]
     else:
-        common = pathlib.Path(os.path.commonpath(paths)).resolve()
+        try:
+            common = pathlib.Path(os.path.commonpath(paths)).resolve()
+        except ValueError:  # pragma: no cover
+            # Different drives on Windows:
+            return
         assert common.is_dir()
-        assert _LIB not in common.parents
-        if common in _LIB.parents:
+        assert _PURELIB not in common.parents, common
+        assert _STDLIB not in common.parents, common
+        assert _TMP not in common.parents, common
+        if (
+            common in _PURELIB.parents
+            or common in _STDLIB.parents
+            or common in _TMP.parents
+        ):
             return  # pragma: no cover
         longest = max(len(path.parts) for path in paths)
         if len(common.parts) == longest - 1:
             glob = common / "*"
         else:
             glob = common / "**" / "*"
     cwd = pathlib.Path.cwd().resolve()
@@ -476,15 +506,17 @@
     )
     parser.add_argument(
         action="extend", nargs="...", dest="file", help=argparse.SUPPRESS
     )
     return typing.cast(_Args, vars(parser.parse_args(args)))
 
 
-def main(args: typing.Sequence[str] | None = None) -> None:
+def main(  # pylint: disable = too-many-branches
+    args: typing.Sequence[str] | None = None,
+) -> None:
     """Run the main program."""
     parsed = _parse_args(args)
     output = parsed["output"]
     path: pathlib.Path | None
     with tempfile.TemporaryDirectory() as work:
         match parsed:
             case {"command": [source, *argv], "module": [], "file": []}:
@@ -492,22 +524,30 @@
                 path.write_text(source, encoding="utf-8")
                 name: str | None = "the provided command"
                 with _patch_sys_argv(argv), _catch_exceptions() as caught:
                     runpy.run_path(  # pylint: disable = no-member
                         str(path), run_name="__main__"
                     )
             case {"command": [], "module": [source, *argv], "file": []}:
-                with _patch_sys_argv(argv), _catch_exceptions() as caught:
+                with (
+                    _patch_sys_argv(argv),
+                    _insert_sys_path(pathlib.Path().resolve()),
+                    _catch_exceptions() as caught,
+                ):
+                    path = _main_file_for_module(source)
                     runpy.run_module(  # pylint: disable = no-member
-                        source, run_name="__main__"
+                        source, run_name="__main__", alter_sys=True
                     )
-                path = _main_file_for_module(source)
                 name = source
             case {"command": [], "module": [], "file": [source, *argv]}:
-                with _patch_sys_argv(argv), _catch_exceptions() as caught:
+                with (
+                    _patch_sys_argv(argv),
+                    _insert_sys_path(pathlib.Path(source).parent.resolve()),
+                    _catch_exceptions() as caught,
+                ):
                     runpy.run_path(  # pylint: disable = no-member
                         source, run_name="__main__"
                     )
                 path = pathlib.Path(source).resolve()
                 name = source
             case _:  # pragma: no cover
                 assert False, parsed
@@ -519,17 +559,21 @@
                     paths.append(match.resolve())
         elif path is not None and path in _code:
             paths.append(path)
         if not paths:
             _stderr("No source files found!")
         else:
             if output is not None:
-                common = pathlib.Path(
-                    os.path.commonpath(paths)  # pylint: disable = no-member
-                ).resolve()
+                try:
+                    common = pathlib.Path(os.path.commonpath(paths)).resolve()
+                except ValueError:  # pragma: no cover
+                    _stderr("Unable to resolve source files (different drives)!")
+                    if caught:
+                        raise caught[0] from None
+                    return
                 if common.is_file():
                     common = common.parent
                 assert common.is_dir(), common
                 output = output.resolve()
                 path_and_out: typing.Generator[
                     tuple[pathlib.Path, pathlib.Path | None], None, None
                 ] = (
```

