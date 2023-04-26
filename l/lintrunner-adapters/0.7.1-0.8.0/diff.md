# Comparing `tmp/lintrunner_adapters-0.7.1.tar.gz` & `tmp/lintrunner_adapters-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lintrunner_adapters-0.7.1.tar", max compression
+gzip compressed data, was "lintrunner_adapters-0.8.0.tar", max compression
```

## Comparing `lintrunner_adapters-0.7.1.tar` & `lintrunner_adapters-0.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     4389 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/LICENSE
--rw-r--r--   0        0        0     1984 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/README.md
--rw-r--r--   0        0        0      711 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/__init__.py
--rw-r--r--   0        0        0     1752 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/__main__.py
--rw-r--r--   0        0        0     3546 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/_common/lintrunner_common.py
--rw-r--r--   0        0        0     4097 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/add_trailing_comma_linter.py
--rw-r--r--   0        0        0     5321 2023-04-08 22:42:45.178395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_isort_linter.py
--rw-r--r--   0        0        0     4790 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_linter.py
--rw-r--r--   0        0        0     6348 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clangformat_linter.py
--rw-r--r--   0        0        0     7640 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clippy_linter.py
--rw-r--r--   0        0        0     3453 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/cmake_linter.py
--rw-r--r--   0        0        0     4374 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/django_upgrade_linter.py
--rw-r--r--   0        0        0     3140 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/editorconfig_checker_linter.py
--rw-r--r--   0        0        0     1776 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/exec_linter.py
--rw-r--r--   0        0        0    10327 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/flake8_linter.py
--rw-r--r--   0        0        0     7062 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/grep_linter.py
--rw-r--r--   0        0        0     4269 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/isort_linter.py
--rw-r--r--   0        0        0     5933 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/mypy_linter.py
--rw-r--r--   0        0        0     4593 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/newlines_linter.py
--rw-r--r--   0        0        0     3371 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pip_init.py
--rw-r--r--   0        0        0     6048 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pylint_linter.py
--rw-r--r--   0        0        0     4532 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pyupgrade_linter.py
--rw-r--r--   0        0        0     4722 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/refurb_linter.py
--rw-r--r--   0        0        0     4135 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_fix_linter.py
--rw-r--r--   0        0        0     6413 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_linter.py
--rw-r--r--   0        0        0     7223 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/rustfmt_linter.py
--rw-r--r--   0        0        0     2305 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/shellcheck_linter.py
--rw-r--r--   0        0        0     3122 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ufmt_linter.py
--rw-r--r--   0        0        0     4060 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif.py
--rw-r--r--   0        0        0     6820 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif_test.py
--rw-r--r--   0        0        0     2335 2023-04-08 22:42:45.182395 lintrunner_adapters-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4389 2023-04-26 14:39:00.168660 lintrunner_adapters-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1984 2023-04-26 14:39:00.168660 lintrunner_adapters-0.8.0/README.md
+-rw-r--r--   0        0        0      711 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/__main__.py
+-rw-r--r--   0        0        0     3546 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/_common/lintrunner_common.py
+-rw-r--r--   0        0        0     4097 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py
+-rw-r--r--   0        0        0     5321 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_isort_linter.py
+-rw-r--r--   0        0        0     4790 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_linter.py
+-rw-r--r--   0        0        0     6348 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clangformat_linter.py
+-rw-r--r--   0        0        0     7641 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clippy_linter.py
+-rw-r--r--   0        0        0     3453 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/cmake_linter.py
+-rw-r--r--   0        0        0     4374 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/django_upgrade_linter.py
+-rw-r--r--   0        0        0     3140 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py
+-rw-r--r--   0        0        0     1776 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/exec_linter.py
+-rw-r--r--   0        0        0    10327 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/flake8_linter.py
+-rw-r--r--   0        0        0     7062 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/grep_linter.py
+-rw-r--r--   0        0        0     4269 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/isort_linter.py
+-rw-r--r--   0        0        0     5933 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/mypy_linter.py
+-rw-r--r--   0        0        0     4593 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/newlines_linter.py
+-rw-r--r--   0        0        0     3369 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pip_init.py
+-rw-r--r--   0        0        0     6048 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pylint_linter.py
+-rw-r--r--   0        0        0     4532 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pyupgrade_linter.py
+-rw-r--r--   0        0        0     4722 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/refurb_linter.py
+-rw-r--r--   0        0        0     4144 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_fix_linter.py
+-rw-r--r--   0        0        0     9672 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_linter.py
+-rw-r--r--   0        0        0     7223 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/rustfmt_linter.py
+-rw-r--r--   0        0        0     2305 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/shellcheck_linter.py
+-rw-r--r--   0        0        0     3122 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ufmt_linter.py
+-rw-r--r--   0        0        0     4060 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif.py
+-rw-r--r--   0        0        0     6820 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif_test.py
+-rw-r--r--   0        0        0     2413 2023-04-26 14:39:00.172660 lintrunner_adapters-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 lintrunner_adapters-0.8.0/PKG-INFO
```

### Comparing `lintrunner_adapters-0.7.1/LICENSE` & `lintrunner_adapters-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/README.md` & `lintrunner_adapters-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/__init__.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/__main__.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/__main__.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/_common/lintrunner_common.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/_common/lintrunner_common.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/add_trailing_comma_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/add_trailing_comma_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_isort_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/black_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/black_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clangformat_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clangformat_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/clippy_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/clippy_linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,21 @@
     all_cargo_tomls: set[pathlib.Path] = set()
     for filename in filenames:
         if any(
             is_relative_to(filename, cargo_toml.parent)
             for cargo_toml in all_cargo_tomls
         ):
             logging.debug(
-                f"Skipping finding Cargo.toml from '{filename}' because it is in a known "
-                "Cargo.toml directory"
+                "Skipping finding Cargo.toml from '%s' because it is in a known Cargo.toml directory",
+                filename,
             )
             continue
         cargo_toml = find_cargo_root(filename)
         if cargo_toml is None:
-            logging.debug(f"No Cargo.toml found in parents of {filename}")
+            logging.debug("No Cargo.toml found in parents of %s", filename)
             continue
         all_cargo_tomls.add(cargo_toml)
 
     if not all_cargo_tomls:
         logging.warning("No Cargo.toml found in parents of files to be linted")
 
     return all_cargo_tomls
@@ -197,15 +197,15 @@
     absolute_filenames = {str(path) for path in absolute_paths}
     # Recursively look up to find all the Cargo.toml files in the files to be linted
     all_cargo_tomls = find_cargo_toml_files(absolute_paths)
     logging.info("Found Cargo.toml files: %s", all_cargo_tomls)
     # Run clippy on each Cargo.toml file
     lint_messages: list[LintMessage] = []
     for cargo_toml in all_cargo_tomls:
-        logging.debug(f"Running clippy on {cargo_toml}")
+        logging.debug("Running clippy on %s", cargo_toml)
         lint_messages.extend(
             check_cargo_toml(cargo_toml, absolute_filenames, retries=retries)
         )
 
     return lint_messages
```

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/cmake_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/cmake_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/django_upgrade_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/django_upgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/editorconfig_checker_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/editorconfig_checker_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/exec_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/exec_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/flake8_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/flake8_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/grep_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/grep_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/isort_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/isort_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/mypy_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/mypy_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/newlines_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/newlines_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pip_init.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pip_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     if args.requirement:
         pip_args.extend(["-r", args.requirement])
 
     pip_args.extend(args.packages)
 
     for package in args.packages:
         package_name, _, version = package.partition("=")
-        if version == "":
+        if not version:
             raise RuntimeError(
                 f"Package '{package_name}' did not have a version specified. "
                 "Please specify a version to produce a consistent linting experience."
             )
         if args.no_black_binary and "black" in package_name:
             pip_args.append(f"--no-binary={package_name}")
```

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pylint_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pylint_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/pyupgrade_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/pyupgrade_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/refurb_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/refurb_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_fix_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_fix_linter.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,20 @@
     with concurrent.futures.ThreadPoolExecutor(
         max_workers=os.cpu_count(),
         thread_name_prefix="Thread",
     ) as executor:
         futures = {
             executor.submit(
                 check_file,
-                x,
+                path,
                 config=args.config,
                 retries=args.retries,
                 timeout=args.timeout,
-            ): x
-            for x in args.filenames
+            ): path
+            for path in args.filenames
         }
         for future in concurrent.futures.as_completed(futures):
             try:
                 for lint_message in future.result():
                     lint_message.display()
             except Exception:
                 logging.critical('Failed at "%s".', futures[future])
```

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ruff_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ruff_linter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Adapter for https://github.com/charliermarsh/ruff."""
 
 from __future__ import annotations
 
 import argparse
+import concurrent.futures
 import json
 import logging
+import os
 import subprocess
 import sys
 
 from lintrunner_adapters import (
     LintMessage,
     LintSeverity,
     add_default_options,
@@ -159,24 +161,94 @@
             original=None,
             replacement=None,
         )
         for vuln in vulnerabilities
     ]
 
 
+def check_file_for_fixes(
+    filename: str,
+    *,
+    config: str | None,
+    retries: int,
+    timeout: int,
+) -> list[LintMessage]:
+    try:
+        with open(filename, "rb") as f:
+            original = f.read()
+        with open(filename, "rb") as f:
+            proc_fix = run_command(
+                [
+                    sys.executable,
+                    "-m",
+                    "ruff",
+                    "--fix-only",
+                    "--exit-zero",
+                    *([f"--config={config}"] if config else []),
+                    "--stdin-filename",
+                    filename,
+                    "-",
+                ],
+                stdin=f,
+                retries=retries,
+                timeout=timeout,
+                check=True,
+            )
+    except (OSError, subprocess.CalledProcessError) as err:
+        return [
+            LintMessage(
+                path=None,
+                line=None,
+                char=None,
+                code=LINTER_CODE,
+                severity=LintSeverity.ERROR,
+                name="command-failed",
+                original=None,
+                replacement=None,
+                description=(
+                    f"Failed due to {err.__class__.__name__}:\n{err}"
+                    if not isinstance(err, subprocess.CalledProcessError)
+                    else (
+                        f"COMMAND (exit code {err.returncode})\n"
+                        f"{' '.join(as_posix(x) for x in err.cmd)}\n\n"
+                        f"STDERR\n{err.stderr.decode('utf-8').strip() or '(empty)'}\n\n"
+                        f"STDOUT\n{err.stdout.decode('utf-8').strip() or '(empty)'}"
+                    )
+                ),
+            )
+        ]
+
+    replacement = proc_fix.stdout
+    if original == replacement:
+        return []
+
+    return [
+        LintMessage(
+            path=filename,
+            name="format",
+            description="Run `lintrunner -a` to apply this patch.",
+            line=None,
+            char=None,
+            code=LINTER_CODE,
+            severity=LintSeverity.WARNING,
+            original=original.decode("utf-8"),
+            replacement=replacement.decode("utf-8"),
+        )
+    ]
+
+
 def main() -> None:
     parser = argparse.ArgumentParser(
         description=f"Ruff linter. Linter code: {LINTER_CODE}. Use with RUFF-FIX to auto-fix issues.",
         fromfile_prefix_chars="@",
     )
     parser.add_argument(
         "--config",
         default=None,
-        help="Path to the `pyproject.toml` "
-        "or `ruff.toml` file to use for configuration",
+        help="Path to the `pyproject.toml` or `ruff.toml` file to use for configuration",
     )
     parser.add_argument(
         "--explain",
         action="store_true",
         help="Explain a rule",
     )
     parser.add_argument(
@@ -189,16 +261,20 @@
         default=90,
         type=int,
         help="Seconds to wait for ruff",
     )
     parser.add_argument(
         "--severity",
         action="append",
-        help="map code to severity (e.g. `F401:advice`). "
-        "This option can be used multiple times.",
+        help="map code to severity (e.g. `F401:advice`). This option can be used multiple times.",
+    )
+    parser.add_argument(
+        "--no-fix",
+        action="store_true",
+        help="Do not suggest fixes",
     )
     add_default_options(parser)
     args = parser.parse_args()
 
     logging.basicConfig(
         format="<%(threadName)s:%(levelname)s> %(message)s",
         level=logging.NOTSET
@@ -224,10 +300,37 @@
         timeout=args.timeout,
         explain=args.explain,
         show_disable=args.show_disable,
     )
     for lint_message in lint_messages:
         lint_message.display()
 
+    if args.no_fix or not lint_messages:
+        # If we're not fixing, we can exit early
+        return
+
+    files_with_lints = {lint.path for lint in lint_messages if lint.path is not None}
+    with concurrent.futures.ThreadPoolExecutor(
+        max_workers=os.cpu_count(),
+        thread_name_prefix="Thread",
+    ) as executor:
+        futures = {
+            executor.submit(
+                check_file_for_fixes,
+                path,
+                config=args.config,
+                retries=args.retries,
+                timeout=args.timeout,
+            ): path
+            for path in files_with_lints
+        }
+        for future in concurrent.futures.as_completed(futures):
+            try:
+                for lint_message in future.result():
+                    lint_message.display()
+            except Exception:
+                logging.critical('Failed at "%s".', futures[future])
+                raise
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/rustfmt_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/rustfmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/shellcheck_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/shellcheck_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/adapters/ufmt_linter.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/adapters/ufmt_linter.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/lintrunner_adapters/tools/convert_to_sarif_test.py` & `lintrunner_adapters-0.8.0/lintrunner_adapters/tools/convert_to_sarif_test.py`

 * *Files identical despite different names*

### Comparing `lintrunner_adapters-0.7.1/pyproject.toml` & `lintrunner_adapters-0.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lintrunner-adapters"
-version = "0.7.1"
+version = "0.8.0"
 description = "Adapters and tools for lintrunner"
 authors = ["Justin Chu <justinchu@microsoft.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/justinchuby/lintrunner-adapters"
 keywords = ["lintrunner", "lint", "cli", "sarif", "linting", "ci", "linter", "flake8", "clippy", "ruff", "rustfmt", "github-code-scanning"]
 classifiers = [
@@ -78,28 +78,35 @@
 python_version = "3.7"
 disable = ["FURB101", "FURB150"] # disable suggestions using pathlib
 
 [tool.ruff]
 target-version = "py37"
 ignore-init-module-imports = true
 select = [
+    "B",
+    "C4",
     "D",
     "E",
     "F",
-    "W",
-    "B",
+    "G",
+    "ISC",
     "N",
-    "UP",
-    "YTT",
-    "PLE",
+    "NPY",
     "PLC",
+    "PLE",
     "PLW",
     "RUF",
+    "SIM",
+    "TID252",
+    "UP",
+    "W",
+    "YTT",
 ]
 ignore = [
+    "C408",
     "D1",
     "D202",
     "D205",
     "D212",
     "D400",
     "D401",
     "D415",
```

### Comparing `lintrunner_adapters-0.7.1/PKG-INFO` & `lintrunner_adapters-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lintrunner-adapters
-Version: 0.7.1
+Version: 0.8.0
 Summary: Adapters and tools for lintrunner
 Home-page: https://github.com/justinchuby/lintrunner-adapters
 License: MIT
 Keywords: lintrunner,lint,cli,sarif,linting,ci,linter,flake8,clippy,ruff,rustfmt,github-code-scanning
 Author: Justin Chu
 Author-email: justinchu@microsoft.com
 Requires-Python: >=3.7,<4.0
```

