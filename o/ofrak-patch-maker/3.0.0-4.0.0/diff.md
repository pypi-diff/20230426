# Comparing `tmp/ofrak_patch_maker-3.0.0.tar.gz` & `tmp/ofrak_patch_maker-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofrak_patch_maker-3.0.0.tar", last modified: Tue Jan 24 04:05:55 2023, max compression
+gzip compressed data, was "ofrak_patch_maker-4.0.0.tar", last modified: Wed Apr 26 18:59:52 2023, max compression
```

## Comparing `ofrak_patch_maker-3.0.0.tar` & `ofrak_patch_maker-4.0.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:55.243984 ofrak_patch_maker-3.0.0/
--rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_patch_maker-3.0.0/LICENSE
--rw-r--r--   0 edward     (501) staff       (20)       41 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/MANIFEST.in
--rw-r--r--   0 edward     (501) staff       (20)     4276 2023-01-24 04:05:55.243491 ofrak_patch_maker-3.0.0/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     3342 2023-01-18 23:40:02.000000 ofrak_patch_maker-3.0.0/README.md
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:55.224744 ofrak_patch_maker-3.0.0/ofrak_patch_maker/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/__init__.py
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:55.229441 ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)      536 2022-08-23 19:53:06.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/abstract.py
--rw-r--r--   0 edward     (501) staff       (20)     3245 2022-08-24 21:38:35.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/gnu.py
--rw-r--r--   0 edward     (501) staff       (20)     4489 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/llvm.py
--rw-r--r--   0 edward     (501) staff       (20)     3107 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/model.py
--rw-r--r--   0 edward     (501) staff       (20)    18728 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/patch_maker.py
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/py.typed
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:55.242761 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/
--rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/__init__.py
--rw-r--r--   0 edward     (501) staff       (20)    16934 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/abstract.py
--rw-r--r--   0 edward     (501) staff       (20)    13008 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu.py
--rw-r--r--   0 edward     (501) staff       (20)     2880 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py
--rw-r--r--   0 edward     (501) staff       (20)     1830 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_arm.py
--rw-r--r--   0 edward     (501) staff       (20)     2286 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_avr.py
--rw-r--r--   0 edward     (501) staff       (20)     2249 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py
--rw-r--r--   0 edward     (501) staff       (20)     5999 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py
--rw-r--r--   0 edward     (501) staff       (20)     2796 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_x64.py
--rw-r--r--   0 edward     (501) staff       (20)    11425 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/llvm_12.py
--rw-r--r--   0 edward     (501) staff       (20)     3828 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/model.py
--rw-r--r--   0 edward     (501) staff       (20)     5258 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/utils.py
--rw-r--r--   0 edward     (501) staff       (20)     2081 2023-01-11 21:57:41.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain.conf
-drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-01-24 04:05:55.226944 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/
--rw-r--r--   0 edward     (501) staff       (20)     4276 2023-01-24 04:05:55.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/PKG-INFO
--rw-r--r--   0 edward     (501) staff       (20)     1032 2023-01-24 04:05:55.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/SOURCES.txt
--rw-r--r--   0 edward     (501) staff       (20)        1 2023-01-24 04:05:55.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/dependency_links.txt
--rw-r--r--   0 edward     (501) staff       (20)       96 2023-01-24 04:05:55.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/requires.txt
--rw-r--r--   0 edward     (501) staff       (20)       18 2023-01-24 04:05:55.000000 ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/top_level.txt
--rw-r--r--   0 edward     (501) staff       (20)       38 2023-01-24 04:05:55.244116 ofrak_patch_maker-3.0.0/setup.cfg
--rw-r--r--   0 edward     (501) staff       (20)     2083 2023-01-24 04:01:33.000000 ofrak_patch_maker-3.0.0/setup.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.767519 ofrak_patch_maker-4.0.0/
+-rw-r--r--   0 edward     (501) staff       (20)    14321 2022-08-24 21:38:35.000000 ofrak_patch_maker-4.0.0/LICENSE
+-rw-r--r--   0 edward     (501) staff       (20)       67 2023-03-20 14:52:33.000000 ofrak_patch_maker-4.0.0/MANIFEST.in
+-rw-r--r--   0 edward     (501) staff       (20)     4276 2023-04-26 18:59:52.766912 ofrak_patch_maker-4.0.0/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     3342 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.0/README.md
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.748170 ofrak_patch_maker-4.0.0/ofrak_patch_maker/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/__init__.py
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.752535 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)      770 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/abstract.py
+-rw-r--r--   0 edward     (501) staff       (20)     4610 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/gnu.py
+-rw-r--r--   0 edward     (501) staff       (20)     6099 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/llvm.py
+-rw-r--r--   0 edward     (501) staff       (20)     3623 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/model.py
+-rw-r--r--   0 edward     (501) staff       (20)    20807 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/patch_maker.py
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/py.typed
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.765783 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/
+-rw-r--r--   0 edward     (501) staff       (20)        0 2022-08-23 19:53:06.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/__init__.py
+-rw-r--r--   0 edward     (501) staff       (20)    18006 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/abstract.py
+-rw-r--r--   0 edward     (501) staff       (20)    13102 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu.py
+-rw-r--r--   0 edward     (501) staff       (20)     3018 2023-03-30 19:29:24.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py
+-rw-r--r--   0 edward     (501) staff       (20)     1830 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_arm.py
+-rw-r--r--   0 edward     (501) staff       (20)     2492 2023-02-02 23:02:32.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_avr.py
+-rw-r--r--   0 edward     (501) staff       (20)     2249 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py
+-rw-r--r--   0 edward     (501) staff       (20)     2919 2023-03-21 23:02:49.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_ppc.py
+-rw-r--r--   0 edward     (501) staff       (20)     5999 2023-03-17 18:25:04.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py
+-rw-r--r--   0 edward     (501) staff       (20)     2796 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_x64.py
+-rw-r--r--   0 edward     (501) staff       (20)    12252 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/llvm_12.py
+-rw-r--r--   0 edward     (501) staff       (20)     4047 2023-03-30 19:29:16.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/model.py
+-rw-r--r--   0 edward     (501) staff       (20)     5258 2023-01-11 21:57:41.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/utils.py
+-rw-r--r--   0 edward     (501) staff       (20)     2327 2023-03-21 23:02:49.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain.conf
+drwxr-xr-x   0 edward     (501) staff       (20)        0 2023-04-26 18:59:52.750628 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/
+-rw-r--r--   0 edward     (501) staff       (20)     4276 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/PKG-INFO
+-rw-r--r--   0 edward     (501) staff       (20)     1088 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 edward     (501) staff       (20)        1 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 edward     (501) staff       (20)      107 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/requires.txt
+-rw-r--r--   0 edward     (501) staff       (20)       18 2023-04-26 18:59:52.000000 ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/top_level.txt
+-rw-r--r--   0 edward     (501) staff       (20)       34 2023-02-16 21:44:18.000000 ofrak_patch_maker-4.0.0/requirements.txt
+-rw-r--r--   0 edward     (501) staff       (20)       38 2023-04-26 18:59:52.767694 ofrak_patch_maker-4.0.0/setup.cfg
+-rw-r--r--   0 edward     (501) staff       (20)     2387 2023-04-26 17:26:19.000000 ofrak_patch_maker-4.0.0/setup.py
```

### Comparing `ofrak_patch_maker-3.0.0/LICENSE` & `ofrak_patch_maker-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-3.0.0/PKG-INFO` & `ofrak_patch_maker-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak_patch_maker
-Version: 3.0.0
+Version: 4.0.0
 Summary: PatchMaker tool for applying source-code patches to binaries
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_patch_maker-3.0.0/README.md` & `ofrak_patch_maker-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/binary_parser/gnu.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/binary_parser/gnu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import re
-from typing import Tuple, Dict
+from typing import Dict, List, Tuple
 
 from ofrak_patch_maker.binary_parser.abstract import AbstractBinaryFileParser
 from ofrak_patch_maker.toolchain.model import BinFileType, Segment
 from ofrak_type.memory_permissions import MemoryPermissions
+from ofrak_type.symbol_type import LinkableSymbolType
 
 
 class GNU_ELF_Parser(AbstractBinaryFileParser):
     file_format = BinFileType.ELF
 
     _re_symbol_prog = re.compile(
-        r"^(?P<address>[0-9A-Fa-f]{8})[ \t]+"
+        r"^(?P<address>[0-9A-Fa-f]+)[ \t]+"
         r"(?P<flags>[lg!\s][w\s][C\s][W\s][I\s][dD\s][fFO\s])?[ \t]+"
         r"(?P<section>\S+)[ \t]"
-        r"(?P<size_or_alignment>[0-9A-Fa-f]{8})[ \t]*"
+        r"(?P<size_or_alignment>[0-9A-Fa-f]+)[ \t]*"
         r"(?P<name>.+)?$",
         flags=re.MULTILINE,
     )
     _re_section_prog = re.compile(
         r"^[\s|\t]*"
         r"(?P<idx>[0-9]+)[ \t]+"
         r"(?P<name>\S+)[ \t]+"
@@ -26,28 +27,28 @@
         r"(?P<lma>[0-9A-Fa-f]+)[ \t]+"
         r"(?P<offset>[0-9A-Fa-f]+)[ \t]+"
         r"(?P<alignment>[0-9]\*\*[0-9])\n[ \n]+"
         r"(?P<flags>[\S, ]+)",
         flags=re.MULTILINE,
     )
 
-    def parse_symbols(self, output: str) -> Dict[str, int]:
+    def parse_symbols(self, output: str) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         """
-        Use `objdump` with the `--syms` flag to get info on all symbols in a file. Parses columns
-        based on: <https://stackoverflow.com/a/16471895/16690095>.
+        Use `objdump` with the `--syms` flag to get info on all defined symbols in a file. Parses
+        columns based on: <https://stackoverflow.com/a/16471895/16690095>.
         """
         result = {}
-        for symbol_data in self._re_symbol_prog.finditer(output):
-            name = symbol_data.group("name")
-            addr = symbol_data.group("address")
-            symbol_section = symbol_data.group("section")
-
-            if name and addr:
-                if symbol_section and symbol_section != "*UND*":
-                    result[name] = int(addr, 16)
+        symbols = self._get_all_symbols(output)
+        for sym_name, sym_vaddr, sym_section, sym_type in symbols:
+            if sym_section != "*UND*" and "w" not in sym_type:
+                if "F" in sym_type:
+                    result[sym_name] = (sym_vaddr, LinkableSymbolType.FUNC)
+                else:
+                    # TODO: handle data symbols and distinguish between RO and RW symbols with section info
+                    result[sym_name] = (sym_vaddr, LinkableSymbolType.UNDEF)
         return result
 
     def parse_sections(self, output: str) -> Tuple[Segment, ...]:
         """
         Uses `objdump` with the `--section-headers` flag to get info on all symbols in a file.
         Parses the returned columns.
         """
@@ -68,19 +69,43 @@
                 is_entry=is_entry,
                 length=int(section_data.group("size"), 16),
                 access_perms=permissions,
             )
             segments.append(seg)
         return tuple(segments)
 
+    def parse_relocations(self, output: str) -> Dict[str, Tuple[int, LinkableSymbolType]]:
+        """
+        Use `objdump` with the `--syms` flag to get info on all undefined symbols in a file. Parses
+        columns based on: <https://stackoverflow.com/a/16471895/16690095>.
+        """
+        result = {}
+        symbols = self._get_all_symbols(output)
+        for sym_name, sym_vaddr, sym_section, sym_type in symbols:
+            if sym_section == "*UND*" or "w" in sym_type:
+                result[sym_name] = (sym_vaddr, LinkableSymbolType.UNDEF)
+        return result
+
+    def _get_all_symbols(self, output: str) -> List[Tuple[str, int, str, str]]:
+        result = []
+        for symbol_data in self._re_symbol_prog.finditer(output):
+            name = symbol_data.group("name")
+            addr = symbol_data.group("address")
+            symbol_section = symbol_data.group("section")
+            symbol_type = symbol_data.group("flags")
+
+            if name and addr:
+                result.append((name, int(addr, 16), symbol_section, symbol_type))
+        return result
+
 
 class GNU_V10_ELF_Parser(GNU_ELF_Parser):
     file_format = BinFileType.ELF
 
-    def parse_symbols(self, tool_output: str) -> Dict[str, int]:
+    def parse_symbols(self, tool_output: str) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         symbols = {}
         lines = tool_output.split("\n")
         for l in lines:
             tokens = l.split()
             if "O" in tokens or "F" in tokens:
-                symbols.update({tokens[-1]: int(tokens[0], 16)})
+                symbols.update({tokens[-1]: (int(tokens[0], 16), LinkableSymbolType.FUNC)})
         return symbols
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/model.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 These classes must only ever contain "immutable" data.
 
 We never want to worry about the state of these objects at any point during a patch injection.
 """
 from dataclasses import dataclass
-from typing import Mapping, Optional, Tuple
+from enum import Enum
+from typing import Mapping, Optional, Set, Tuple
 
 from ofrak_patch_maker.toolchain.model import Segment, BinFileType
+from ofrak_type.symbol_type import LinkableSymbolType
 
 AUTOGENERATE_WARNING = """/*
 *
 * WARNING: DO NOT EDIT THIS FILE MANUALLY
 *      This is an autogenerated file
 *
 */
@@ -26,20 +28,24 @@
 class AssembledObject:
     """
     The result of any `compile` or `assemble` step
 
     :var path: .o file path
     :var file_format: .elf, .coff, etc.
     :var segment_map: e.g. `{".text", Segment(...)}`
+    :var strong_symbols:
+    :var unresolved_symbols: {symbol name: (address, symbol type)}
+    :var bss_size_required:
     """
 
     path: str
     file_format: BinFileType
     segment_map: Mapping[str, Segment]  # segment name to Segment
-    symbols: Mapping[str, int]
+    strong_symbols: Mapping[str, Tuple[int, LinkableSymbolType]]
+    unresolved_symbols: Mapping[str, Tuple[int, LinkableSymbolType]]
     bss_size_required: int
 
 
 @dataclass(frozen=True)
 class LinkedExecutable:
     """
     The result of any `link` step.
@@ -50,15 +56,15 @@
     :var symbols: the global function and data symbol mapping information for this executable
     :var relocatable: TODO: whether or not the executable is relocatable
     """
 
     path: str
     file_format: BinFileType
     segments: Tuple[Segment, ...]
-    symbols: Mapping[str, int]
+    symbols: Mapping[str, Tuple[int, LinkableSymbolType]]
     relocatable: bool
 
 
 @dataclass(frozen=True)
 class PatchRegionConfig:
     """
     PatchRegionConfig is the dataclass required to generate an .ld script. That describes
@@ -104,16 +110,24 @@
     Keeping this class frozen ensures we have a hash for every instance.
 
     Instances of this class should never be declared outside of
     [PatchMaker][ofrak_patch_maker.patch_maker.PatchMaker].
 
     :var name: a name
     :var object_map: {source file path: AssembledObject}
+    :var unresolved_symbols: symbols used but undefined within the BOM source files
     :var bss_size_required:
     :var entry_point_symbol: symbol of the patch entrypoint, when relevant
     """
 
     name: str
     object_map: Mapping[str, AssembledObject]
+    unresolved_symbols: Set[str]
     bss_size_required: int
     entry_point_symbol: Optional[str]
     segment_alignment: int
+
+
+class SourceFileType(Enum):
+    DEFAULT = 0
+    C = 1
+    ASM = 2
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/patch_maker.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/patch_maker.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,34 +27,37 @@
 
 fem = patch_maker.make_fem([(bom, region_config)], ofrak_fw_resource, verbose=True)
 
 await ofrak_fw_resource.run(SegmentInjectorModifier, SegmentInjectorModifierConfig.from_fem(fem))
 ```
 """
 import logging
+import itertools
 import os
 import tempfile
-from typing import Dict, Iterable, List, Mapping, Optional, Tuple
+from typing import Dict, Iterable, List, Mapping, Optional, Set, Tuple
 from warnings import warn
 
 from immutabledict import immutabledict
 
 from ofrak_patch_maker.model import (
     AssembledObject,
     BOM,
     FEM,
     PatchRegionConfig,
     LinkedExecutable,
     PatchMakerException,
+    SourceFileType,
 )
 from ofrak_patch_maker.toolchain.abstract import Toolchain
 from ofrak_patch_maker.toolchain.model import (
     Segment,
 )
 from ofrak_type.memory_permissions import MemoryPermissions
+from ofrak_type.symbol_type import LinkableSymbolType
 
 
 class PatchMaker:
     def __init__(
         self,
         toolchain: Toolchain,
         platform_includes: Optional[Iterable[str]] = None,
@@ -105,15 +108,15 @@
             self._base_symbol_file = self._toolchain.generate_linker_include_file(
                 base_symbols, filename
             )
             self._base_symbols.update(base_symbols)
 
         self.logger = logger
 
-    def _extract_symbols(self, path: str) -> Dict[str, int]:
+    def _extract_symbols(self, path: str) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         """
         :param path: path to a program or library binary with symbols
 
         :return: mapping symbol name to effective address
         """
         return self._toolchain.get_bin_file_symbols(path)
 
@@ -141,31 +144,34 @@
         :return: immutable, pre-analyzed `AssembledObject` containing section info
         """
         if os.path.isdir(object_path) or not os.path.exists(object_path):
             raise PatchMakerException("PatchMaker.prepare_object expects a valid object file path!")
 
         segments = self._toolchain.get_bin_file_segments(object_path)
         symbols = self._toolchain.get_bin_file_symbols(object_path)
+        # Symbols defined in another file which may or may not be another patch source file or the target binary.
+        relocation_symbols = self._toolchain.get_bin_file_rel_symbols(object_path)
+
         bss_size_required = 0
         segment_map = {}
         for s in segments:
             if self._toolchain.keep_section(s.segment_name):
                 segment_map[s.segment_name] = s
             if s.segment_name.startswith(".bss"):
                 if s.length > 0 and self._toolchain._config.no_bss_section:
                     raise PatchMakerException(
                         f"{s.segment_name} found but `no_bss_section` is set in the provided ToolchainConfig!"
                     )
                 bss_size_required += s.length
-
         return AssembledObject(
             object_path,
             self._toolchain.file_format,
             immutabledict(segment_map),
             immutabledict(symbols),
+            immutabledict(relocation_symbols),
             bss_size_required,
         )
 
     @staticmethod
     def _validate_bom_input(
         name: str,
         source_list: List[str],
@@ -236,45 +242,92 @@
         for o_file in object_list:
             assembled_object = self.prepare_object(o_file)
             object_map.update({o_file: assembled_object})
 
         out_dir = os.path.join(self.build_dir, name + "_bom_files")
         os.mkdir(out_dir)
 
-        for c_file in list(filter(lambda x: x.endswith(".c"), source_list)):
-            assembled_object_path = self._toolchain.compile(c_file, header_dirs, out_dir=out_dir)
-            assembled_object = self.prepare_object(assembled_object_path)
-            object_map.update({c_file: assembled_object})
-
-        for asm_file in list(filter(lambda x: x.endswith(".as") or x.endswith(".S"), source_list)):
-            original_asm_file = asm_file
-            if asm_file.endswith(".S"):
-                asm_file = self._toolchain.preprocess(asm_file, header_dirs, out_dir=out_dir)
-            assembled_object_path = self._toolchain.assemble(asm_file, header_dirs, out_dir=out_dir)
-            assembled_object = self.prepare_object(assembled_object_path)
-            object_map.update({original_asm_file: assembled_object})
+        c_files = list(filter(lambda x: x.endswith(".c"), source_list))
+        c_args = zip(
+            c_files,
+            itertools.repeat(header_dirs),
+            itertools.repeat(out_dir),
+            itertools.repeat(SourceFileType.C),
+        )
+        result = itertools.starmap(self._create_object_file, c_args)
+        for r in result:
+            object_map.update(r)
+
+        asm_files = list(filter(lambda x: x.endswith(".as") or x.endswith(".S"), source_list))
+        asm_args = zip(
+            asm_files,
+            itertools.repeat(header_dirs),
+            itertools.repeat(out_dir),
+            itertools.repeat(SourceFileType.ASM),
+        )
+        result = itertools.starmap(self._create_object_file, asm_args)
+        for r in result:
+            object_map.update(r)
 
         # Compute the required size for the .bss segment
-        bss_size_required = 0
-        symbols: Dict[str, int] = {}
-        for o in object_map.values():
-            bss_size_required += o.bss_size_required
-            symbols.update(o.symbols)
-
-        if entry_point_name and entry_point_name not in symbols:
-            raise PatchMakerException(f"Entry point {entry_point_name} not found in object files")
+        bss_size_required, unresolved_sym_set = self._resolve_symbols_within_BOM(
+            object_map, entry_point_name
+        )
 
         return BOM(
             name,
             immutabledict(object_map),
+            unresolved_sym_set,
             bss_size_required,
             entry_point_name,
             self._toolchain.segment_alignment,
         )
 
+    def _create_object_file(
+        self,
+        file: str,
+        header_dirs: List[str],
+        out_dir: str,
+        file_type: SourceFileType,
+    ) -> Mapping[str, AssembledObject]:
+        original_file = file
+        if file.endswith(".S"):
+            file = self._toolchain.preprocess(file, header_dirs, out_dir=out_dir)
+        if file_type is SourceFileType.C:
+            object_path = self._toolchain.compile(file, header_dirs, out_dir=out_dir)
+        elif file_type is SourceFileType.ASM:
+            object_path = self._toolchain.assemble(file, header_dirs, out_dir=out_dir)
+        else:
+            self.logger.error(f"Source file type '{file_type}' invalid, unable to prepare object.")
+        obj = self.prepare_object(object_path)
+        return {original_file: obj}
+
+    def _resolve_symbols_within_BOM(
+        self, object_map: Dict[str, AssembledObject], entry_point_name: Optional[str] = None
+    ) -> Tuple[int, Set[str]]:
+        bss_size_required = 0
+        symbols: Dict[str, Tuple[int, LinkableSymbolType]] = {}
+        unresolved_symbols: Dict[str, Tuple[int, LinkableSymbolType]] = {}
+        for o in object_map.values():
+            bss_size_required += o.bss_size_required
+            symbols.update(o.strong_symbols)
+            # Resolve symbols defined within different patch files within the same patch BOM
+            for sym, values in o.unresolved_symbols.items():
+                # Have not already seen this symbol in a previous patch object
+                if sym not in symbols.keys():
+                    unresolved_symbols.update({sym: values})
+
+        unresolved_sym_set: Set[str]
+        unresolved_sym_set = set(unresolved_symbols.keys()) - set(symbols.keys())
+
+        if entry_point_name and entry_point_name not in symbols:
+            raise PatchMakerException(f"Entry point {entry_point_name} not found in object files")
+
+        return bss_size_required, unresolved_sym_set
+
     def create_unsafe_bss_segment(self, vm_address: int, size: int) -> Segment:
         """
         The user may at times require the use of known unused `.bss` space.
 
         When this is required the data cannot be "properly", statically allocated, so an unsafe
         `.bss` section must be defined for where the data will be placed at runtime.
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/abstract.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/abstract.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from ofrak_type import ArchInfo
 from ofrak_patch_maker.binary_parser.abstract import AbstractBinaryFileParser
 from ofrak_patch_maker.toolchain.model import Segment, ToolchainConfig
 from ofrak_patch_maker.toolchain.utils import get_repository_config
 from ofrak_type.architecture import InstructionSet
 from ofrak_type.bit_width import BitWidth
 from ofrak_type.memory_permissions import MemoryPermissions
+from ofrak_type.symbol_type import LinkableSymbolType
 
 RBS_AUTOGEN_WARNING = (
     "/*\n"
     "*\n"
     "* WARNING: DO NOT EDIT THIS FILE MANUALLY\n"
     "*      This is an autogenerated file\n"
     "*\n"
@@ -77,40 +78,41 @@
         self._linker_flags: List[str] = []
         self._config = toolchain_config
         self._logger = logger
 
         # The keep_list should only contain FUNCTIONALLY important sections
         # (not empty .got.plt, for instance).
         # TODO: Come up with a better system to handle this...
-        self._linker_keep_list = [".data", ".rodata", ".text"]
+        self._linker_keep_list = [".data", ".rodata", ".text", ".rel"]
         self._linker_discard_list = [
             ".gnu.hash",
             ".comment",
             ".ARM.attributes",
             ".dynamic",
             ".ARM.exidx",
             ".hash",
             ".dynsym",
             ".dynstr",
             ".eh_frame",
+            ".altinstructions",
         ]
 
         self._assembler_target = self._get_assembler_target(processor)
         self._compiler_target = self._get_compiler_target(processor)
 
     @property
     @abstractmethod
     def name(self) -> str:
         """
         :return str: name property that matches the value used in `toolchain.conf` to access paths
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def _get_assembler_target(self, processor: ArchInfo) -> str:
+    def _get_assembler_target(self, processor: ArchInfo) -> Optional[str]:
         """
         Red Balloon Security strongly recommends all users provide their specific hardware target
         for best results.
 
         :param processor:
 
         :raises PatchMakerException: if no target provided and program attributes do not correspond
@@ -251,23 +253,27 @@
         final_flags.extend(flags)
 
         if out_file is not None:
             final_flags.extend([f"-o{out_file}"])
 
         args = [tool_path] + final_flags + in_files
         self._logger.info(" ".join(args))
-        if env:
-            my_env = os.environ.copy()
-            my_env.update(env)
-            self._logger.info(f"With env: {my_env}")
-            proc = subprocess.run(
-                args, stdout=subprocess.PIPE, encoding="utf-8", check=True, env=my_env
-            )
-        else:
-            proc = subprocess.run(args, stdout=subprocess.PIPE, encoding="utf-8", check=True)
+        try:
+            if env:
+                my_env = os.environ.copy()
+                my_env.update(env)
+                self._logger.info(f"With env: {my_env}")
+                proc = subprocess.run(
+                    args, stdout=subprocess.PIPE, encoding="utf-8", check=True, env=my_env
+                )
+            else:
+                proc = subprocess.run(args, stdout=subprocess.PIPE, encoding="utf-8", check=True)
+        except subprocess.CalledProcessError as e:
+            cmd = " ".join(args)
+            raise ValueError(f'Command "{cmd}" returned non-zero exit status {e.returncode}')
 
         return proc.stdout
 
     def preprocess(self, source_file: str, header_dirs: List[str], out_dir: str = ".") -> str:
         """
         Runs the Toolchain's C preprocessor on the input file.
 
@@ -277,16 +283,15 @@
 
         self._execute_tool(
             self._preprocessor_path,
             self._preprocessor_flags,
             [source_file] + ["-I" + x for x in header_dirs],
             out_file=out_file,
         )
-        # Note that we return the source file here!!!
-        return os.path.abspath(source_file)
+        return os.path.abspath(out_file)
 
     def compile(self, c_file: str, header_dirs: List[str], out_dir: str = ".") -> str:
         """
         Runs the Toolchain's C compiler on the input file.
 
         :return str: path to the object file
         """
@@ -349,19 +354,24 @@
 
         self._execute_tool(self._linker_path, flags, o_files, out_file=exec_path)
 
     @staticmethod
     def linker_include_filter(symbol_name: str) -> bool:
         return "." in symbol_name or "_DYNAMIC" in symbol_name
 
-    def keep_section(self, section_name: str) -> bool:
-        if self._config.separate_data_sections:
-            raise NotImplementedError("you must override keep_section() in your Toolchain sublass")
+    def keep_section(self, section_name: str):
+        if section_name in self._linker_keep_list:
+            return True
+        if self._config.separate_data_sections or self._config.include_subsections:
+            for keep_section in self._linker_keep_list:
+                if section_name.startswith(keep_section):
+                    return True
+            return False
         else:
-            return section_name in self._linker_keep_list
+            return False
 
     @abstractmethod
     def generate_linker_include_file(self, symbols: Mapping[str, int], out_path: str) -> str:
         """
         This utility function receives the generated symbols dictionary that results
         from preprocessing a firmware image and generates a `.inc` file for use
         with linker scripts, enabling direct function calls when using the complete
@@ -472,30 +482,48 @@
         :param symbol_files:
 
         :return str: path to the generated linker script
         """
         raise NotImplementedError()
 
     @abstractmethod
-    def get_bin_file_symbols(self, executable_path: str) -> Dict[str, int]:
+    def get_bin_file_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         """
         For now, this utility only searches for global function and data symbols which are
         actually contained in a section in the file, as opposed to symbols which are referenced
         but undefined.
 
         :param executable_path: path to the program to be analyzed for symbols
 
-        :return Dict[str, int]: mapping of symbol string to effective address.
+        :return Dict[str, Tuple[int, LinkableSymbolType]]: mapping of symbol string to tuple of
+        effective address, symbol type.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def get_bin_file_segments(self, path: str) -> Tuple[Segment, ...]:
         """
         Parses all segments found in the executable path provided.
 
         :param path: path to the program to be analyzed for symbols
 
         :return Tuple[Segment, ...]: Tuple of [Segment][ofrak_patch_maker.toolchain.model.Segment]
         objects
         """
         raise NotImplementedError()
+
+    @abstractmethod
+    def get_bin_file_rel_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
+        """
+        This utility searches for global function and data symbols which are
+        referenced in a section in the file but are undefined.
+
+        :param executable_path: path to the program to be analyzed for symbols
+
+        :return Dict[str, Tuple[int, LinkableSymbolType]]: mapping of symbol string to tuple of
+        effective address, symbol type.
+        """
+        raise NotImplementedError()
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     BinFileType,
     ToolchainConfig,
     CompilerOptimizationLevel,
     ToolchainException,
 )
 from ofrak_patch_maker.toolchain.utils import get_file_format
 from ofrak_type.memory_permissions import MemoryPermissions
+from ofrak_type.symbol_type import LinkableSymbolType
 
 
 class Abstract_GNU_Toolchain(Toolchain, ABC):
     def __init__(
         self,
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
@@ -108,25 +109,14 @@
     def _linker_script_flag(self) -> str:
         return "-T"
 
     @staticmethod
     def _get_linker_map_flag(exec_path: str) -> Iterable[str]:
         return "-Map", f"{exec_path}.map"
 
-    def keep_section(self, section_name: str):
-        if section_name in self._linker_keep_list:
-            return True
-        if self._config.separate_data_sections:
-            for keep_section in self._linker_keep_list:
-                if section_name.startswith(keep_section):
-                    return True
-            return False
-        else:
-            return False
-
     def add_linker_include_values(self, symbols: Mapping[str, int], path: str):
         with open(path, "a") as f:
             for name, addr in symbols.items():
                 if self.linker_include_filter(name):
                     continue
                 f.write(f"PROVIDE({name} = {hex(addr)});\n")
 
@@ -191,15 +181,15 @@
 
     @staticmethod
     def ld_generate_bss_section(
         memory_region_name: str,
     ) -> str:
         bss_section_name = ".bss"
         return (
-            f"    {bss_section_name} : {{\n"
+            f"    {bss_section_name} : SUBALIGN(0) {{\n"
             f"        *.o({bss_section_name}, {bss_section_name}.*)\n"
             f"    }} > {memory_region_name}"
         )
 
     def _ld_generate_got_plt_region(
         self,
         vm_address: int,
@@ -324,15 +314,17 @@
         return ld_script_path
 
     @property
     @abstractmethod
     def segment_alignment(self) -> int:
         raise NotImplementedError()
 
-    def get_bin_file_symbols(self, executable_path: str) -> Dict[str, int]:
+    def get_bin_file_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         # This happens to be the same as LLVM but it really doesn't belong in Parent code.
         # Note: readobj for gcc is objdump
         readobj_output = self._execute_tool(self._readobj_path, ["--syms"], [executable_path])
 
         return self._parser.parse_symbols(readobj_output)
 
     def get_bin_file_segments(self, path: str) -> Tuple[Segment, ...]:
@@ -341,14 +333,21 @@
                 "Extracted file format does not match this toolchain instance!"
             )
 
         readobj_output = self._execute_tool(self._readobj_path, ["--section-headers"], [path])
 
         return self._parser.parse_sections(readobj_output)
 
+    def get_bin_file_rel_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
+        readobj_output = self._execute_tool(self._readobj_path, ["--syms"], [executable_path])
+
+        return self._parser.parse_relocations(readobj_output)
+
 
 class GNU_10_Toolchain(Abstract_GNU_Toolchain):
     def __init__(
         self,
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
         logger: logging.Logger = logging.getLogger(__name__),
@@ -356,20 +355,22 @@
         super().__init__(processor, toolchain_config, logger=logger)
 
         if self._compiler_target is not None:
             self._compiler_flags.append(f"-march={self._compiler_target}")
         if self._config.compiler_cpu:
             self._compiler_flags.append(f"-mcpu={self._config.compiler_cpu}")
 
-        self._assembler_flags.append(f"-march={self._get_assembler_target(processor)}")
+        if self._assembler_target is not None:
+            self._assembler_flags.append(f"-march={self._assembler_target}")
         if self._config.assembler_cpu:
             self._assembler_flags.append(f"-mcpu={self._config.assembler_cpu}")
 
         self._linker_flags.append(
             "--no-eh-frame-hdr",
         )
 
         if self._config.relocatable:
             self._compiler_flags.append("-pie")
             self._linker_flags.append("--pic-executable")
         else:
             self._compiler_flags.append("-fno-plt")
+            self._compiler_flags.append("-fno-pic")
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_aarch64.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
         logger: logging.Logger = logging.getLogger(__name__),
     ):
         super().__init__(processor, toolchain_config, logger=logger)
         # Enable compilation of the GNU atomics intrinsics.
         self._compiler_flags.append("-mno-outline-atomics")
+        # Force literal pools at end of functions, rather than .rodata
+        self._compiler_flags.append("-mpc-relative-literal-loads")
 
     @property
     def name(self) -> str:
         return "GNU_AARCH64_LINUX_10"
 
     @property
     def segment_alignment(self) -> int:
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_arm.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_arm.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_avr.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,70 @@
+from typing import Tuple
+
+from ofrak_type.memory_permissions import MemoryPermissions
+
+from ofrak_type.architecture import InstructionSet, ArchInfo
+from ofrak_patch_maker.toolchain.gnu import GNU_10_Toolchain
 from ofrak_patch_maker.binary_parser.gnu import GNU_ELF_Parser
-from ofrak_patch_maker.toolchain.gnu import Abstract_GNU_Toolchain
 from ofrak_patch_maker.toolchain.model import ToolchainConfig
-from ofrak_type.architecture import InstructionSet, ArchInfo
 import logging
 
 
-class GNU_AVR_5_Toolchain(Abstract_GNU_Toolchain):
+class GNU_M68K_LINUX_10_Toolchain(GNU_10_Toolchain):
     binary_file_parsers = [GNU_ELF_Parser()]
 
     def __init__(
         self,
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
         logger: logging.Logger = logging.getLogger(__name__),
     ):
         super().__init__(processor, toolchain_config, logger=logger)
-
-        if self._config.relocatable:
-            raise ValueError("-pie not supported for AVR")
-
-        if toolchain_config.hard_float:
-            raise ValueError("hard float not supported for AVR")
-
-        # avr-gcc's -mmcu flag allows you to specify either the exact target chip, or a chip
-        #      architecture. Specifying an exact chip will choose the correct avr/io.h and startup
-        #      code for the chip. Here, we will first look for an exact chip supplied in the
-        #      ToolchainConfig, and fall back on sub-ISA.
-        #      See https://gcc.gnu.org/wiki/avr-gcc#Supporting_.22unsupported.22_Devices
-        if processor.sub_isa is not None:
-            self._linker_flags.append(f"-m{processor.sub_isa.value}")
-            self._compiler_flags.append(
-                f"-mmcu={self._config.compiler_cpu or processor.sub_isa.value}"
-            )
-            self._assembler_flags.append(
-                f"-mmcu={self._config.assembler_cpu or processor.sub_isa.value}"
-            )
+        if self._config.hard_float:
+            self._compiler_flags.append("-mfloat-abi=hard")
         else:
-            raise ValueError("sub_isa is required for AVR linking")
+            self._compiler_flags.append("-msoft-float")
 
     @property
     def name(self) -> str:
-        return "GNU_AVR_5"
+        return "GNU_M68K_LINUX_10"
 
     @property
     def segment_alignment(self) -> int:
-        return 2
+        return 4
 
-    def _get_assembler_target(self, processor: ArchInfo) -> str:
-        if processor.isa is not InstructionSet.AVR:
+    def _get_assembler_target(self, processor: ArchInfo):
+        if processor.isa is not InstructionSet.M68K:
             raise ValueError(
-                f"The GNU AVR toolchain does not support ISAs which are not AVR; "
+                f"The GNU M68K toolchain does not support ISAs which are not M68K; "
                 f"given ISA {processor.isa.name}"
             )
         if self._config.assembler_target:
             return self._config.assembler_target
-        return InstructionSet.AVR.value.lower()
+        arch = processor.isa.value
+        if processor.sub_isa is not None:
+            arch = processor.sub_isa.value
+        return arch
+
+    def _ld_generate_rel_dyn_region(
+        self,
+        vm_address: int,
+        length: int,
+    ) -> Tuple[str, str]:
+        region_name = '".rela.dyn_mem"'
+        perms_string = self._ld_perm2str(MemoryPermissions.RW)
+        return (
+            f"    {region_name} ({perms_string}) : ORIGIN = {hex(vm_address)}, "
+            f"LENGTH = {hex(length)}",
+            region_name,
+        )
+
+    @staticmethod
+    def _ld_generate_rel_dyn_section(
+        memory_region_name: str,
+    ) -> str:
+        rel_dyn_section_name = ".rela.dyn"
+        return (
+            f"    {rel_dyn_section_name} : {{\n"
+            f"        *.o({rel_dyn_section_name})\n"
+            f"    }} > {memory_region_name}"
+        )
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_m68k.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_x64.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,68 @@
-from typing import Tuple
-
-from ofrak_type.memory_permissions import MemoryPermissions
-
-from ofrak_type.architecture import InstructionSet, ArchInfo
 from ofrak_patch_maker.toolchain.gnu import GNU_10_Toolchain
-from ofrak_patch_maker.binary_parser.gnu import GNU_ELF_Parser
+from ofrak_patch_maker.binary_parser.gnu import GNU_V10_ELF_Parser
 from ofrak_patch_maker.toolchain.model import ToolchainConfig
 import logging
 
+from ofrak_type.architecture import ArchInfo
+
 
-class GNU_M68K_LINUX_10_Toolchain(GNU_10_Toolchain):
-    binary_file_parsers = [GNU_ELF_Parser()]
+class GNU_X86_64_LINUX_EABI_10_3_0_Toolchain(GNU_10_Toolchain):
+    binary_file_parsers = [GNU_V10_ELF_Parser()]
 
     def __init__(
         self,
         processor: ArchInfo,
         toolchain_config: ToolchainConfig,
         logger: logging.Logger = logging.getLogger(__name__),
     ):
         super().__init__(processor, toolchain_config, logger=logger)
-        if self._config.hard_float:
-            self._compiler_flags.append("-mfloat-abi=hard")
-        else:
+
+        self._compiler_flags.extend(
+            [
+                "-malign-data=abi",  # further relaxes compiler data alignment policy
+                "-mno-sse2",  # restricts usage of xmm register / avx instruction usage.
+            ]
+        )
+
+        if not self._config.hard_float:
             self._compiler_flags.append("-msoft-float")
 
     @property
     def name(self) -> str:
-        return "GNU_M68K_LINUX_10"
+        return "GNU_X86_64_LINUX_EABI_10_3_0"
 
     @property
     def segment_alignment(self) -> int:
-        return 4
+        return 16
 
     def _get_assembler_target(self, processor: ArchInfo):
-        if processor.isa is not InstructionSet.M68K:
-            raise ValueError(
-                f"The GNU M68K toolchain does not support ISAs which are not M68K; "
-                f"given ISA {processor.isa.name}"
-            )
         if self._config.assembler_target:
             return self._config.assembler_target
-        arch = processor.isa.value
-        if processor.sub_isa is not None:
-            arch = processor.sub_isa.value
-        return arch
-
-    def _ld_generate_rel_dyn_region(
-        self,
-        vm_address: int,
-        length: int,
-    ) -> Tuple[str, str]:
-        region_name = '".rela.dyn_mem"'
-        perms_string = self._ld_perm2str(MemoryPermissions.RW)
-        return (
-            f"    {region_name} ({perms_string}) : ORIGIN = {hex(vm_address)}, "
-            f"LENGTH = {hex(length)}",
-            region_name,
-        )
+        return "generic64"
 
     @staticmethod
-    def _ld_generate_rel_dyn_section(
+    def ld_generate_bss_section(
         memory_region_name: str,
     ) -> str:
-        rel_dyn_section_name = ".rela.dyn"
+        """
+        We override this for x64 so we can provide SUBALIGN(1)
+        This is required to correctly estimate how much size we need for bss
+        when splitting up data structures into their own individual bss sections.
+        If we were to let the linker align every structure's section to 8 or 16, it would
+        insert empty space that we had not allocated for the bss memory region.
+        gcc/ld do prefer 8 alignment for data if you don't force this, but it is not likely to be
+        hugely faster on recent hardware for most situations (ie not locked instructions
+        across a cache line):
+        https://lemire.me/blog/2012/05/31/data-alignment-for-speed-myth-or-reality/
+        Pre-2011 x64 chips might be slower with these kinds of accesses, but:
+           - We should not bend over backwards for processors we've not evaluated yet.
+           - .bss handling is already difficult enough as is.
+           - The flexibility granted by this feature likely justifies a relatively small performance impact.
+        We should address this as a problem if future users find that performance is noticeably/severely impacted.
+        """
+        bss_section_name = ".bss"
         return (
-            f"    {rel_dyn_section_name} : {{\n"
-            f"        *.o({rel_dyn_section_name})\n"
+            f"    {bss_section_name} : SUBALIGN(1) {{\n"
+            f"        *.o({bss_section_name}, {bss_section_name}.*)\n"
             f"    }} > {memory_region_name}"
         )
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/llvm_12.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/llvm_12.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import tempfile
 from typing import List, Mapping, Optional, Tuple, Dict
 
 from ofrak_type import ArchInfo
 from ofrak_type.architecture import InstructionSet
 from ofrak_type.memory_permissions import MemoryPermissions
+from ofrak_type.symbol_type import LinkableSymbolType
 
 from ofrak_patch_maker.binary_parser.llvm import LLVM_ELF_Parser
 from ofrak_patch_maker.toolchain.abstract import Toolchain, RBS_AUTOGEN_WARNING
 from ofrak_patch_maker.toolchain.model import (
     Segment,
     BinFileType,
     ToolchainConfig,
@@ -38,29 +39,35 @@
         self._preprocessor_flags.append("-E")
 
         self._assembler_flags.append(f"-march={self._assembler_target}")
         if self._config.assembler_cpu:
             self._assembler_flags.append(f"-mcpu={self._config.assembler_cpu}")
         self._compiler_flags.extend(
             [
-                "-cc1",
-                "-triple",
+                "-c",
+                "-target",
                 self._compiler_target,  # type: ignore
+                "-Xclang",
                 "-emit-obj",
-                "-msoft-float",
-                "-mfloat-abi",
-                "soft",
                 "-Wall",
             ]
         )
+        if processor.isa is InstructionSet.ARM:
+            # Without this option, Clang will ignore target("arm"/"thumb") attributes
+            self._compiler_flags.append("-marm")
+
+        if self._config.hard_float:
+            self._compiler_flags.append("-mno-soft-float")
+        else:
+            self._compiler_flags.append("-msoft-float")
 
         if self._config.separate_data_sections:
-            raise NotImplementedError("separate sections not supported by LLVM Toolchain yet")
+            self._compiler_flags.append("-fdata-sections")
         if self._config.compiler_cpu:
-            self._compiler_flags.append(f"-mcpu={self._config.compiler_cpu}")
+            self._logger.warning("compiler_cpu option set, but has no meaning for LLVM toolchain")
 
         llvm12_compiler_optimization_map = {
             CompilerOptimizationLevel.NONE: "-O0",
             CompilerOptimizationLevel.SOME: "-O1",
             CompilerOptimizationLevel.SPACE: "-Oz",
             CompilerOptimizationLevel.FULL: "-O3",
         }
@@ -71,31 +78,35 @@
         if not self.is_userspace():
             self._compiler_flags.append("-ffreestanding")
 
         if self._config.force_inlines:
             self._compiler_flags.append("-finline-hint-functions")
 
         if self._config.relocatable:
-            self._compiler_flags.extend(["-fno-direct-access-external-data", "-pic-is-pie"])
+            self._compiler_flags.extend(["-fno-direct-access-external-data", "-fPIE"])
             self._linker_flags.append("--pie")
         else:
+            self._compiler_flags.append("-fno-pic")
             self._linker_flags.append("--no-pie")
 
         if self._config.no_bss_section:
             self._compiler_flags.append("-fno-zero-initialized-in-bss")
 
         if self._config.no_jump_tables:
             self._compiler_flags.append("-fno-jump-tables")
 
         if self._config.debug_info:
             self._compiler_flags.extend(
                 [
                     "-fno-split-dwarf-inlining",
+                    "-Xclang",
                     "-debug-info-kind=limited",
+                    "-Xclang",
                     "-dwarf-version=4",
+                    "-Xclang",
                     "-debugger-tuning=gdb",
                 ]
             )
 
         self._linker_flags.extend(
             [
                 "--error-unresolved-symbols",
@@ -229,15 +240,15 @@
         memory_region_name: str,
     ) -> str:
         stripped_seg_name = segment_name.strip(".")
         stripped_obj_name = os.path.basename(object_path).split(".")[0]
         abs_path = os.path.abspath(object_path)
         return (
             f"    .rbs_{stripped_obj_name}_{stripped_seg_name} : {{\n"
-            f"        {abs_path}({segment_name})\n"
+            f"        {abs_path}({segment_name}*)\n"
             f"    }} > {memory_region_name}"
         )
 
     @staticmethod
     def ld_generate_bss_section(
         memory_region_name: str,
     ) -> str:
@@ -292,15 +303,17 @@
         # Plus, some other memory will also be aligned to 16
         # https://stackoverflow.com/a/49397524/2753454
         # Let's just do it for every section; we already allocated 16 extra earlier
         if self._processor.isa == InstructionSet.X86:
             return 16
         return 1
 
-    def get_bin_file_symbols(self, executable_path: str) -> Dict[str, int]:
+    def get_bin_file_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
         readobj_output = self._execute_tool(
             self._readobj_path, ["--symbols"], [executable_path], out_file=None
         )
 
         return self._parser.parse_symbols(readobj_output)
 
     def get_bin_file_segments(self, path: str) -> Tuple[Segment, ...]:
@@ -313,7 +326,16 @@
             )
 
         readobj_output = self._execute_tool(
             self._readobj_path, ["--section-details"], [path], out_file=None
         )
 
         return self._parser.parse_sections(readobj_output)
+
+    def get_bin_file_rel_symbols(
+        self, executable_path: str
+    ) -> Dict[str, Tuple[int, LinkableSymbolType]]:
+        readobj_output = self._execute_tool(
+            self._readobj_path, ["--symbols"], [executable_path], out_file=None
+        )
+
+        return self._parser.parse_relocations(readobj_output)
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/model.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,14 +93,16 @@
     :var create_map_files: Creates `.map` files from link step (Default: `True`)
     :var debug_info: Should most closely mirror GNU `-g` functionality (Default: `True`)
     :var check_overlap: Enables the Toolchain Linker to assert memory boundaries (Default: `True`)
     :var userspace_dynamic_linker: Signals compilation for userspace and libc usage.
     :var isysroot: Specifies the root directory for header files
     :var c_standard: Specifies the version of C to use, e.g. C89, C99, etc
     :var separate_data_sections: Whether to put each data object in a separate section in .o file
+    :var include_subsections: In addition to normal keep sections, keep "sub"-sections sharing name
+    prefix e.g. .text.foo (this flag is treated as True if separate_data_sections is True)
     :var hard_float: Compile with support for hardware floating point operations (Default: `False`)
     """
 
     file_format: BinFileType
     force_inlines: bool
     relocatable: bool
     no_std_lib: bool
@@ -113,9 +115,10 @@
     assembler_cpu: Optional[str] = None
     create_map_files: bool = True
     debug_info: bool = True
     check_overlap: bool = True
     userspace_dynamic_linker: Optional[str] = None
     isysroot: Optional[str] = None
     c_standard: Optional[CStandardVersion] = CStandardVersion.C99
-    separate_data_sections: Optional[bool] = False
+    separate_data_sections: bool = False
+    include_subsections: bool = False
     hard_float: Optional[bool] = False
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain/utils.py` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain/utils.py`

 * *Files identical despite different names*

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker/toolchain.conf` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker/toolchain.conf`

 * *Files 17% similar despite different names*

```diff
@@ -40,13 +40,20 @@
 
 [GNU_AVR_5]
 PREPROCESSOR = /usr/bin/avr-gcc
 COMPILER = /usr/bin/avr-gcc
 LINKER = /usr/bin/avr-ld
 BIN_PARSER = /usr/bin/avr-objdump
 
+[GNU_PPC_LINUX_10]
+PREPROCESSOR = /usr/bin/powerpc-linux-gnu-gcc-10
+COMPILER = /usr/bin/powerpc-linux-gnu-gcc-10
+LINKER = /usr/bin/powerpc-linux-gnu-ld
+BIN_PARSER = /usr/bin/powerpc-linux-gnu-objdump
+
 [ASM]
 ARM_ASM_PATH = /opt/rbs/toolchain/gcc-arm-none-eabi-10-2020-q4-major/bin/arm-none-eabi-as
 X86_64_ASM_PATH = /opt/rbs/toolchain/binutils-2.34/gas/as-new
 M68K_ASM_PATH = /usr/bin/m68k-linux-gnu-as
 AARCH64_ASM_PATH = /usr/bin/aarch64-linux-gnu-as
 AVR_ASM_PATH = /usr/bin/avr-as
+PPC_ASM_PATH = /usr/bin/powerpc-linux-gnu-as
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/PKG-INFO` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofrak-patch-maker
-Version: 3.0.0
+Version: 4.0.0
 Summary: PatchMaker tool for applying source-code patches to binaries
 Home-page: https://ofrak.com/
 Download-URL: https://github.com/redballoonsecurity/ofrak
 Author: Red Balloon Security
 Author-email: ofrak@redballoonsecurity.com
 License: Proprietary
 Project-URL: Documentation, https://ofrak.com/docs/
```

### Comparing `ofrak_patch_maker-3.0.0/ofrak_patch_maker.egg-info/SOURCES.txt` & `ofrak_patch_maker-4.0.0/ofrak_patch_maker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 ofrak_patch_maker/__init__.py
 ofrak_patch_maker/model.py
 ofrak_patch_maker/patch_maker.py
 ofrak_patch_maker/py.typed
 ofrak_patch_maker/toolchain.conf
 ofrak_patch_maker.egg-info/PKG-INFO
@@ -19,12 +20,13 @@
 ofrak_patch_maker/toolchain/__init__.py
 ofrak_patch_maker/toolchain/abstract.py
 ofrak_patch_maker/toolchain/gnu.py
 ofrak_patch_maker/toolchain/gnu_aarch64.py
 ofrak_patch_maker/toolchain/gnu_arm.py
 ofrak_patch_maker/toolchain/gnu_avr.py
 ofrak_patch_maker/toolchain/gnu_m68k.py
+ofrak_patch_maker/toolchain/gnu_ppc.py
 ofrak_patch_maker/toolchain/gnu_vbcc_m68k.py
 ofrak_patch_maker/toolchain/gnu_x64.py
 ofrak_patch_maker/toolchain/llvm_12.py
 ofrak_patch_maker/toolchain/model.py
 ofrak_patch_maker/toolchain/utils.py
```

### Comparing `ofrak_patch_maker-3.0.0/setup.py` & `ofrak_patch_maker-4.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import setuptools
+import pkg_resources
 from setuptools.command.egg_info import egg_info
 
 
 class egg_info_ex(egg_info):
     """Includes license file into `.egg-info` folder."""
 
     def run(self):
@@ -15,25 +16,33 @@
         egg_info.run(self)
 
 
 with open("README.md") as f:
     long_description = f.read()
 
 
+# Should be the same as in build_image.py
+def read_requirements(requirements_path):
+    with open(requirements_path) as requirements_handle:
+        return [
+            str(requirement)
+            for requirement in pkg_resources.parse_requirements(requirements_handle)
+        ]
+
+
 setuptools.setup(
     name="ofrak_patch_maker",
-    version="3.0.0",
+    version="4.0.0",
     description="PatchMaker tool for applying source-code patches to binaries",
     packages=setuptools.find_packages(exclude=("ofrak_patch_maker_test",)),
     package_data={"ofrak_patch_maker": ["py.typed"]},
     install_requires=[
-        "ofrak_type~=2.0",
-        "immutabledict==2.2.0",
-        "python-magic",
-    ],
+        "ofrak_type>=2.2.0rc0,==2.*",
+    ]
+    + read_requirements("requirements.txt"),
     extras_require={
         "test": [
             "fun-coverage==0.2.0",
             "pytest",
             "pytest-cov",
         ]
     },
```

