# Comparing `tmp/pwntools_stubs-0.1.1.tar.gz` & `tmp/pwntools_stubs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwntools_stubs-0.1.1.tar", max compression
+gzip compressed data, was "pwntools_stubs-0.1.2.tar", max compression
```

## Comparing `pwntools_stubs-0.1.1.tar` & `pwntools_stubs-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      207 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/README.md
--rw-r--r--   0        0        0     1281 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwn-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/__init__.pyi
--rw-r--r--   0        0        0      279 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/asm.pyi
--rw-r--r--   0        0        0      136 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/context.pyi
--rw-r--r--   0        0        0      537 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/elf/__init__.pyi
--rw-r--r--   0        0        0      657 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/fiddling.pyi
--rw-r--r--   0        0        0      612 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/fmtstr.pyi
--rw-r--r--   0        0        0      330 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/gdb.pyi
--rw-r--r--   0        0        0      176 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/log.pyi
--rw-r--r--   0        0        0       21 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/shellcraft.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/__init__.pyi
--rw-r--r--   0        0        0      293 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/listen.pyi
--rw-r--r--   0        0        0      637 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/process.pyi
--rw-r--r--   0        0        0      520 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/remote.pyi
--rw-r--r--   0        0        0      444 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/ssh.pyi
--rw-r--r--   0        0        0     7068 2023-04-25 10:46:25.678549 pwntools_stubs-0.1.1/pwnlib-stubs/tubes/tube.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:46:25.682549 pwntools_stubs-0.1.1/pwnlib-stubs/util/__init__.pyi
--rw-r--r--   0        0        0      157 2023-04-25 10:46:25.682549 pwntools_stubs-0.1.1/pwnlib-stubs/util/cyclic.pyi
--rw-r--r--   0        0        0     1010 2023-04-25 10:46:25.682549 pwntools_stubs-0.1.1/pwnlib-stubs/util/packing.pyi
--rw-r--r--   0        0        0      491 2023-04-25 10:46:25.682549 pwntools_stubs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 pwntools_stubs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      207 2023-04-26 10:12:31.434710 pwntools_stubs-0.1.2/README.md
+-rw-r--r--   0        0        0     1281 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwn-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/__init__.pyi
+-rw-r--r--   0        0        0      279 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/asm.pyi
+-rw-r--r--   0        0        0      136 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/context.pyi
+-rw-r--r--   0        0        0      537 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/elf/__init__.pyi
+-rw-r--r--   0        0        0      657 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/fiddling.pyi
+-rw-r--r--   0        0        0      612 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/fmtstr.pyi
+-rw-r--r--   0        0        0      330 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/gdb.pyi
+-rw-r--r--   0        0        0      176 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/log.pyi
+-rw-r--r--   0        0        0       21 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/shellcraft.pyi
+-rw-r--r--   0        0        0        0 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/__init__.pyi
+-rw-r--r--   0        0        0      293 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/listen.pyi
+-rw-r--r--   0        0        0      643 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/process.pyi
+-rw-r--r--   0        0        0      520 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/remote.pyi
+-rw-r--r--   0        0        0      444 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/ssh.pyi
+-rw-r--r--   0        0        0     7068 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/tubes/tube.pyi
+-rw-r--r--   0        0        0        0 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0      157 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/util/cyclic.pyi
+-rw-r--r--   0        0        0     1010 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pwnlib-stubs/util/packing.pyi
+-rw-r--r--   0        0        0      491 2023-04-26 10:12:31.438710 pwntools_stubs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 pwntools_stubs-0.1.2/PKG-INFO
```

### Comparing `pwntools_stubs-0.1.1/pwn-stubs/__init__.pyi` & `pwntools_stubs-0.1.2/pwn-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/elf/__init__.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/elf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/fiddling.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/fiddling.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/fmtstr.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/fmtstr.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/tubes/process.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/tubes/process.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pwnlib.tubes.tube import tube
 from typing import Any
 from collections.abc import Callable
 
 class process(tube):
     def __init__(
         self,
-        argv: list[str] = ...,
+        argv: list[str] | str = ...,
         shell: bool = ...,
         executable: str = ...,
         cwd: str = ...,
         env: dict[str, str] = ...,
         stdin: int = ...,
         stdout: int = ...,
         stderr: int = ...,
```

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/tubes/remote.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/tubes/remote.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/tubes/tube.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/tubes/tube.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/pwnlib-stubs/util/packing.pyi` & `pwntools_stubs-0.1.2/pwnlib-stubs/util/packing.pyi`

 * *Files identical despite different names*

### Comparing `pwntools_stubs-0.1.1/PKG-INFO` & `pwntools_stubs-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwntools-stubs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Incomplete, and probably incorrect, stubs for pwntools
 Author: rikyiso01
 Author-email: riky.isola@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

