# Comparing `tmp/idefix_cli-1.2.0.tar.gz` & `tmp/idefix_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-1.2.0.tar", last modified: Fri Apr 14 09:54:36 2023, max compression
+gzip compressed data, was "idefix_cli-2.0.0.tar", last modified: Wed Apr 26 19:41:39 2023, max compression
```

## Comparing `idefix_cli-1.2.0.tar` & `idefix_cli-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.338201 idefix_cli-1.2.0/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 09:54:36.000000 idefix_cli-1.2.0/idefix_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:54:36.342202 idefix_cli-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-14 09:54:27.000000 idefix_cli-1.2.0/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.039720 idefix_cli-2.0.0/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-26 19:41:39.000000 idefix_cli-2.0.0/idefix_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 19:41:39.043721 idefix_cli-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-26 19:41:24.000000 idefix_cli-2.0.0/tests/test_write.py
```

### Comparing `idefix_cli-1.2.0/LICENSE` & `idefix_cli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/PKG-INFO` & `idefix_cli-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 1.2.0
+Version: 2.0.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-1.2.0/README.md` & `idefix_cli-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_backports.py` & `idefix_cli-2.0.0/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/clean.py` & `idefix_cli-2.0.0/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/clone.py` & `idefix_cli-2.0.0/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/conf.py` & `idefix_cli-2.0.0/idefix_cli/_commands/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         if arch_req := get_option("compilation", "CPU"):
             args.extend(["-arch", arch_req])
         if arch_req := get_option("compilation", "GPU"):
             args.extend(["-arch", arch_req])
             if "-gpu" not in args:
                 args.append("-gpu")
 
-    parser = ArgumentParser()
+    parser = ArgumentParser(allow_abbrev=False)
     parser.add_argument("-arch", nargs="+", required=False)
     _args, unknown_args = parser.parse_known_args(args)
 
     if _args.arch is None:
         return args
 
     return unknown_args + [f"-DKokkos_ARCH_{_.upper()}=ON" for _ in _args.arch]
@@ -198,15 +198,15 @@
 def substitute_cmake_cxx(args: list[str]) -> list[str]:
     if not (
         "-cxx" in args or any(re.match(r"-DCMAKE_CXX_COMPILER=\w+", _) for _ in args)
     ):
         if compiler_req := get_option("compilation", "compiler"):
             args.extend(["-cxx", compiler_req])
 
-    parser = ArgumentParser()
+    parser = ArgumentParser(allow_abbrev=False)
     parser.add_argument("-cxx")
     _args, unknown_args = parser.parse_known_args(args)
 
     if _args.cxx is None:
         return args
 
     return unknown_args + [f"-DCMAKE_CXX_COMPILER={_args.cxx}"]
```

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/read.py` & `idefix_cli-2.0.0/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/run.py` & `idefix_cli-2.0.0/idefix_cli/_commands/run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,98 @@
 """run an Idefix problem"""
 from __future__ import annotations
 
 import os
+import re
 import subprocess
 import sys
 from copy import deepcopy
 from enum import auto
 from multiprocessing import cpu_count
 from pathlib import Path
 from subprocess import CalledProcessError, check_call
 from tempfile import NamedTemporaryFile
+from time import sleep, time
 from typing import Final
 
 import inifix
 from rich.prompt import Confirm
 
 from idefix_cli.lib import (
     files_from_patterns,
     get_config_file,
     get_option,
     print_err,
     print_subcommand,
+    print_success,
     print_warning,
     requires_idefix,
 )
 
 if sys.version_info >= (3, 11):
     from contextlib import chdir
     from enum import StrEnum
     from typing import assert_never
 else:
     from typing_extensions import assert_never
 
     from idefix_cli._backports import StrEnum
     from idefix_cli.lib import chdir
 
+MAIN_LOG_FILE = "idefix.0.log"
+TIME_INTEGRATOR_LOG_LINE = re.compile(
+    "^TimeIntegrator:\\s*(?P<time>.+) \\|\\s*(?P<cycle>\\d+) \\|"
+)
+JOB_COMPLETED = re.compile("Main: Job completed")
+
+
+def spawn_idefix(cmd: list[str], *, step_count: int) -> int:
+    if step_count < 0:
+        # infinite steps: simple call
+        return subprocess.call(cmd)
+
+    if sys.platform.startswith("win"):
+        print_err("idfx run --one isn't supported on Windows")
+        return -3
+    else:
+        from signal import SIGUSR2  # not available on Windows
+
+    # spawn idefix in the background and kill it (or exit) as soon as completion is detected
+    if os.path.exists(MAIN_LOG_FILE):
+        os.remove(MAIN_LOG_FILE)
+    prog = subprocess.Popen(cmd)
+    start_wait = time()
+    while not os.path.exists(MAIN_LOG_FILE):
+        # idefix is not necessarily well behaved regarding retcodes,
+        # so we don't have a simple way to check wether the process
+        # has returned already or not, creating the opportunity for
+        # an infinite loop here, hence the timeout mechanism
+        if (time() - start_wait) > 60:
+            return -2
+        sleep(0.1)
+
+    complete = False
+    last_edit = -1.0
+    while not complete:
+        if last_edit != (new_edit := os.stat(MAIN_LOG_FILE).st_mtime):
+            with open(MAIN_LOG_FILE) as fh:
+                for line in fh:
+                    if JOB_COMPLETED.match(line):
+                        complete = True
+                        break
+                    if (match := TIME_INTEGRATOR_LOG_LINE.match(line)) is None:
+                        continue
+                    if int(match["cycle"]) == step_count:
+                        prog.send_signal(SIGUSR2)
+                        complete = True
+                        break
+            last_edit = new_edit
+        sleep(0.01)
+    return -1
+
 
 class RebuildMode(StrEnum):
     ALWAYS = auto()
     PROMPT = auto()
 
 
 # known end messages in Idefix
@@ -71,35 +125,42 @@
         "-i",
         dest="inifile",
         action="store",
         type=str,
         default="idefix.ini",
         help="target inifile",
     )
-    time_group = parser.add_mutually_exclusive_group()
-    time_group.add_argument(
+    tstop_group = parser.add_mutually_exclusive_group()
+    tstop_group.add_argument(
         "--duration",
         action="store",
         type=float,
-        help="run for specified time (in code units)",
+        help="run for specified time (in code units) DEPRECATED",
     )
+    tstop_group.add_argument(
+        "--tstop",
+        action="store",
+        type=float,
+        help="override TimeIntegrator.tstop",
+    )
+    time_group = parser.add_mutually_exclusive_group()
     time_group.add_argument(
         "--one",
         "--one-step",
         dest="one_step",
         nargs="*",
         help="run only for one time step. "
         "Accepts arbitrary output type name(s) (e.g. dmp or vtk).",
     )
     parser.add_argument(
         "--time-step",
         dest="time_step",
         action="store",
         type=float,
-        help="patch the inifile TimeIntegrator.first_dt parameter",
+        help="override TimeIntegrator.first_dt",
     )
     parser.add_argument(
         "--nproc",
         action="store",
         type=int,
         default=1,
         help=(
@@ -107,29 +168,42 @@
             "Requires the code to be configured for MPI."
         ),
     )
     parser.add_argument(
         "--times",
         dest="multiplier",
         type=int,
-        default=1,
+        default=-1,
         help="multiplier for --one (use `--one --times 2` to run for 2 steps)",
     )
 
 
 def command(
     *unknown_args: str,
     directory: str = ".",
     inifile: str = "idefix.ini",
+    tstop: float | None = None,
     duration: float | None = None,
     time_step: float | None = None,
     one_step: list[str] | None = None,
-    multiplier: int = 1,
+    multiplier: int | None = None,
     nproc: int = 1,
 ) -> int:
+    if multiplier is not None:
+        if one_step is None:
+            print_err(
+                "--times argument is invalid if --one/--one-step isn't passed too"
+            )
+            return 1
+        if multiplier < 1:
+            print_err(
+                f"--times argument expects a strictly positive integer (got {multiplier})"
+            )
+            return 1
+
     d = Path(directory).resolve()
     exe = d / "idefix"
     if not exe.is_file() and not (d / "Makefile").is_file():
         print_err(
             f"No idefix executable or Makefile found in the target directory {d} "
             "Run `idfx conf` first"
         )
@@ -154,33 +228,43 @@
         print_err(
             "configuration file seems malformed, "
             "expected 'TimeIntegrator' to be a section title, not a parameter name."
         )
         return 1
 
     if one_step is not None:
-        output_types = one_step
-
+        output_types = set(one_step) - {"log"}
         if time_step is None:
             conf["TimeIntegrator"].setdefault("first_dt", 1e-6)
             time_step = conf["TimeIntegrator"]["first_dt"]
 
-        duration = multiplier * time_step
+        conf.setdefault("Output", {})
+        output_sec = conf["Output"]
+        if not isinstance(output_sec, dict):
+            print_err(
+                "configuration file seems malformed, "
+                "expected 'Output' to be a section title, not a parameter name."
+            )
+            return 1
+
+        output_sec["log"] = 1
 
         if len(output_types) > 0:
-            conf.setdefault("Output", {})
-            output_sec = conf["Output"]
-            if not isinstance(output_sec, dict):
-                print_err(
-                    "configuration file seems malformed, "
-                    "expected 'Output' to be a section title, not a parameter name."
-                )
-                return 1
             for entry in output_types:
-                output_sec[entry] = time_step
+                output_sec[entry] = 0  # output on every time step
+
+    multiplier = multiplier or 1
+
+    if time_step is not None:
+        conf["TimeIntegrator"]["first_dt"] = time_step
+    if duration is not None:
+        print_warning("The --duration argument is deprecated. Use --tstop instead.")
+        conf["TimeIntegrator"]["tstop"] = duration
+    elif tstop is not None:
+        conf["TimeIntegrator"]["tstop"] = tstop
 
     rebuild_mode_str: str = get_option("idfx run", "recompile") or "always"
 
     try:
         rebuild_mode = RebuildMode(rebuild_mode_str)
     except ValueError:
         print_warning(
@@ -248,19 +332,14 @@
                 build_is_required = False
     else:
         assert_never(rebuild_mode)
 
     if build_is_required and (ret := build_idefix(directory)) != 0:
         return ret
 
-    if time_step is not None:
-        conf["TimeIntegrator"]["first_dt"] = time_step
-    if duration is not None:
-        conf["TimeIntegrator"]["tstop"] = duration
-
     if conf != base_conf:
         tmp_inifile = NamedTemporaryFile()
         with open(tmp_inifile.name, "wb") as fh:
             inifix.dump(conf, fh)
         inputfile = tmp_inifile.name
     else:
         inputfile = str(pinifile.relative_to(d.resolve()))
@@ -268,19 +347,29 @@
     cmd = ["./idefix", "-i", inputfile, *unknown_args]
 
     if nproc > 1:
         cmd = ["mpirun", "-n", str(nproc), *cmd]
 
     print_subcommand(cmd, loc=d)
     with chdir(d):
-        ret = subprocess.call(cmd)
+        ret = spawn_idefix(cmd, step_count=multiplier)
 
-    if ret == 0:
+    if ret < 0:
+        # special retcodes from spawn_idefix
+        if ret == -1:
+            print_success("Sucessfully stopped idefix mid-air")
+        elif ret == -2:
+            print_err("idefix timed out (startup took more than a minute)")
+        elif ret == -3:
+            # unsupported operation
+            ret = 1
+        ret = 0
+    elif ret == 0:
         # Idefix newer than 1.0 intentionally always returns 0, even on failure
-        with open(d / "idefix.0.log") as fh:
+        with open(d / MAIN_LOG_FILE) as fh:
             last_line = fh.read().strip().split("\n")[-1].strip()
         if last_line in KNOWN_FAIL:
             ret = 1
         elif last_line not in KNOWN_SUCCESS:
             print_warning(
                 "Command completed with an unknown status. Please check log files."
             )
```

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/stamp.py` & `idefix_cli-2.0.0/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_commands/write.py` & `idefix_cli-2.0.0/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/idefix_cli/_main.py` & `idefix_cli-2.0.0/idefix_cli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
 def main(
     argv: "List[str] | None" = None, parser: "ArgumentParser | None" = None
 ) -> Any:
     # the return value is deleguated to sub commands so its type is arbitrary
     # In practice it should be either 'int' or 'typing.NoReturn'
     if parser is None:
-        parser = ArgumentParser(prog="idfx")
+        parser = ArgumentParser(prog="idfx", allow_abbrev=False)
     parser.add_argument("-v", "--version", action="version", version=__version__)
     commands = _setup_commands(parser)
 
     known_args, unknown_args = parser.parse_known_args(argv)
 
     vargs = vars(known_args)
     cmd_name = vargs.pop("command")
@@ -150,13 +150,17 @@
 
 def alt_main(argv: "List[str] | None" = None) -> Any:
     console = Console(width=500, highlight=False)
     console.print(":tennis: :arrow_forward:")
 
     set_theme("baballe")
     try:
-        retv = main(argv, parser=ArgumentParser(prog="baballe"))
+        retv = main(argv, parser=ArgumentParser(prog="baballe", allow_abbrev=False))
     finally:
         set_theme("default")
         console.print(":arrow_backward: :tennis:")
 
     return retv
+
+
+if __name__ == "__main__":
+    sys.exit(main())
```

### Comparing `idefix_cli-1.2.0/idefix_cli/lib.py` & `idefix_cli-2.0.0/idefix_cli/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,39 @@
     elif THEME is Theme.BABALLE:
         emoji = ":paw_print:"
     else:
         assert_never(THEME)
     err_console.print(f"{emoji}[italic magenta] {message}[/]")
 
 
+def print_success(message: str) -> None:
+    """Print some exciting news to stdout.
+
+    Args:
+        message (str): the message to be printed
+
+    Returns:
+        None
+
+    Examples:
+        >>> def my_command() -> int:
+        ...    print_success("Successfully did nothing !")
+        ...    return 0
+    """
+    console = Console(width=500, file=sys.stdout)
+    THEME = get_theme()
+    if THEME is Theme.DEFAULT:
+        emoji = ":tada:"
+    elif THEME is Theme.BABALLE:
+        emoji = ":guide_dog:"
+    else:
+        assert_never(THEME)
+    console.print(f"{emoji}[bold chartreuse1] {message}[/]")
+
+
 def print_subcommand(cmd: list[str], *, loc: Path | None = None) -> None:
     """Print a command, which is to be executed as a subprocess.
 
     Args:
         cmd (list[str]): equivalent argument to be passed to, e.g., subprocess.run
         loc (pathlib.Path | None): the directory (other than cwd)
             from which the command is meant to be executed.
```

### Comparing `idefix_cli-1.2.0/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.0.0/idefix_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 1.2.0
+Version: 2.0.0
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `idefix_cli-1.2.0/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.0.0/idefix_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 idefix_cli/__init__.py
+idefix_cli/__main__.py
 idefix_cli/_backports.py
-idefix_cli/_main.py
 idefix_cli/_theme.py
 idefix_cli/lib.py
 idefix_cli.egg-info/PKG-INFO
 idefix_cli.egg-info/SOURCES.txt
 idefix_cli.egg-info/dependency_links.txt
 idefix_cli.egg-info/entry_points.txt
 idefix_cli.egg-info/requires.txt
@@ -22,10 +22,11 @@
 idefix_cli/_commands/write.py
 tests/test_app_structure.py
 tests/test_clean.py
 tests/test_clone.py
 tests/test_commons.py
 tests/test_conf.py
 tests/test_read.py
+tests/test_run.py
 tests/test_stamp.py
 tests/test_ux.py
 tests/test_write.py
```

### Comparing `idefix_cli-1.2.0/pyproject.toml` & `idefix_cli-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "idefix_cli"
-version = "1.2.0"
+version = "2.0.0"
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
@@ -37,16 +37,16 @@
 ]
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
 
 [project.scripts]
-idfx = "idefix_cli._main:main"
-baballe = "idefix_cli._main:alt_main"
+idfx = "idefix_cli.__main__:main"
+baballe = "idefix_cli.__main__:alt_main"
 
 [project.urls]
 Homepage = "https://github.com/neutrinoceros/idefix_cli"
 
 [tool.setuptools]
 license-files = [
     "LICENSE",
```

### Comparing `idefix_cli-1.2.0/tests/test_app_structure.py` & `idefix_cli-2.0.0/tests/test_app_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import re
 import sys
 from tempfile import NamedTemporaryFile
 from textwrap import dedent
 
 import pytest
 
-from idefix_cli._main import _setup_commands, main
+from idefix_cli.__main__ import _setup_commands, main
 from idefix_cli.lib import print_err
 
 
 @pytest.mark.skipif(
     sys.platform.startswith("win"), reason="plugin system tests are broken on windows"
 )
 @pytest.mark.parametrize(
@@ -56,15 +56,15 @@
         fh.seek(0)  # force flush
         module_name, _ = os.path.splitext(os.path.basename(fh.name))
 
         with pytest.raises(
             RuntimeError,
             match=re.escape(f"command plugin {module_name}{msg}"),
         ):
-            _setup_commands(argparse.ArgumentParser())
+            _setup_commands(argparse.ArgumentParser(allow_abbrev=False))
 
 
 def test_unknown_args(capsys):
     args = "--an_invalid_argument", "-another"
     ret = main(["clean", *args])
     assert ret != 0
     out, err = capsys.readouterr()
@@ -89,15 +89,15 @@
                     return 0
                 """
             )
         )
 
     def _main_mock(argv):
         """A simplified version of the main function that can be trashed with no side effects on other tests"""
-        parser = argparse.ArgumentParser()
+        parser = argparse.ArgumentParser(allow_abbrev=False)
         commands = _setup_commands(parser)
 
         known_args, unknown_args = parser.parse_known_args(argv)
 
         vargs = vars(known_args)
         cmd_name = vargs.pop("command")
```

### Comparing `idefix_cli-1.2.0/tests/test_clean.py` & `idefix_cli-2.0.0/tests/test_clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import StringIO
 
 import pytest
 
+from idefix_cli.__main__ import main
 from idefix_cli._commands.clean import gpatterns, kokkos_files
-from idefix_cli._main import main
 
 
 def replace_wildcards(names):
     return [name.replace("*", "a") for name in names]
 
 
 @pytest.fixture()
```

### Comparing `idefix_cli-1.2.0/tests/test_clone.py` & `idefix_cli-2.0.0/tests/test_clone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
 import pytest
 
-from idefix_cli._main import main
+from idefix_cli.__main__ import main
 
 DATADIR = Path(__file__).parent / "data"
 BASE_SETUP = DATADIR / "OrszagTang3D"
 
 
 def test_clone_basic(capsys, tmp_path):
     dest = str(tmp_path / "new")
```

### Comparing `idefix_cli-1.2.0/tests/test_commons.py` & `idefix_cli-2.0.0/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-1.2.0/tests/test_conf.py` & `idefix_cli-2.0.0/tests/test_conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 import pytest
 from packaging.version import Version
 from pytest_check import check
 
+from idefix_cli.__main__ import main
 from idefix_cli._commands.conf import substitute_cmake_args
-from idefix_cli._main import main
 
 
 def test_conf_without_setup_cpp(capsys, tmp_path, monkeypatch):
     tmp_idefix_dir = tmp_path / "idefix"
     os.makedirs(tmp_idefix_dir / ".git")
     monkeypatch.setenv("IDEFIX_DIR", str(tmp_idefix_dir))
```

### Comparing `idefix_cli-1.2.0/tests/test_read.py` & `idefix_cli-2.0.0/tests/test_read.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 
 from pytest_check import check
 
-from idefix_cli._main import main
+from idefix_cli.__main__ import main
 
 
 def test_read_not_a_file(tmp_path, capsys):
     target = tmp_path / "not_a_file"
     ret = main(["read", str(target.absolute())])
     with check:
         assert ret != 0
```

### Comparing `idefix_cli-1.2.0/tests/test_stamp.py` & `idefix_cli-2.0.0/tests/test_stamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from getpass import getuser
 from socket import gethostname
 from typing import Tuple
 
 import pytest
 from pytest_check import check
 
-from idefix_cli._main import main
+from idefix_cli.__main__ import main
 
 mock_data = {
     "latest ancestor version": "unknown version",
     "sha": "864e17a23eebbccMOCKSHA1e3db466325d54b51a",
     "user": getuser(),
     "host": gethostname(),
 }
```

### Comparing `idefix_cli-1.2.0/tests/test_ux.py` & `idefix_cli-2.0.0/tests/test_ux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 import pytest
 from pytest_check import check
 
-from idefix_cli._main import main
+from idefix_cli.__main__ import main
 
 if sys.version_info >= (3, 10):
     OPTIONAL_SEC = "options"
 else:
     OPTIONAL_SEC = "optional arguments"
 HELP_MESSAGE = (
     "usage: idfx [-h] [-v] {clean,clone,conf,read,run,stamp,write} ...\n"
```

### Comparing `idefix_cli-1.2.0/tests/test_write.py` & `idefix_cli-2.0.0/tests/test_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import re
 import subprocess
 
 import pytest
 from pytest_check import check
 
-from idefix_cli._main import main
+from idefix_cli.__main__ import main
 
 jq_available = subprocess.run(["which", "jq"]).returncode == 0
 
 data = {"Grid": {"x": 1, "y": 2}}
 simple_conf = json.dumps(data)
 simple_conf_as_ini = "[Grid]\nx 1\ny 2"
```

