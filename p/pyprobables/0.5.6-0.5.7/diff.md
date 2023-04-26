# Comparing `tmp/pyprobables-0.5.6.tar.gz` & `tmp/pyprobables-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprobables-0.5.6.tar", last modified: Thu Mar 10 14:16:20 2022, max compression
+gzip compressed data, was "pyprobables-0.5.7.tar", last modified: Wed Apr 26 01:58:17 2023, max compression
```

## Comparing `pyprobables-0.5.6.tar` & `pyprobables-0.5.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-03-10 14:16:08.000000 pyprobables-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7908 2022-03-10 14:16:20.763751 pyprobables-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6686 2022-03-10 14:16:08.000000 pyprobables-0.5.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/probables/
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/probables/blooms/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/blooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26708 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/blooms/bloom.py
--rw-r--r--   0 runner    (1001) docker     (121)    12806 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/blooms/countingbloom.py
--rw-r--r--   0 runner    (1001) docker     (121)    14093 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/blooms/expandingbloom.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/probables/countminsketch/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/countminsketch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31333 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/countminsketch/countminsketch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/probables/cuckoo/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/cuckoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14447 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/cuckoo/countingcuckoo.py
--rw-r--r--   0 runner    (1001) docker     (121)    18971 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/cuckoo/cuckoo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3961 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/hashes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2252 2022-03-10 14:16:08.000000 pyprobables-0.5.6/probables/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-10 14:16:20.763751 pyprobables-0.5.6/pyprobables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7908 2022-03-10 14:16:20.000000 pyprobables-0.5.6/pyprobables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-03-10 14:16:20.000000 pyprobables-0.5.6/pyprobables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-10 14:16:20.000000 pyprobables-0.5.6/pyprobables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-03-10 14:16:20.000000 pyprobables-0.5.6/pyprobables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-10 14:16:08.000000 pyprobables-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-03-10 14:16:20.763751 pyprobables-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-03-10 14:16:08.000000 pyprobables-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.247358 pyprobables-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-26 01:58:00.000000 pyprobables-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-26 01:58:17.243358 pyprobables-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-26 01:58:00.000000 pyprobables-0.5.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/blooms/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/countingbloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/blooms/expandingbloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/countminsketch/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/countminsketch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31337 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/countminsketch/countminsketch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/probables/cuckoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14027 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/countingcuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/cuckoo/cuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-04-26 01:58:00.000000 pyprobables-0.5.7/probables/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/pyprobables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 01:58:17.000000 pyprobables-0.5.7/pyprobables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-26 01:58:00.000000 pyprobables-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 01:58:17.247358 pyprobables-0.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 01:58:17.243358 pyprobables-0.5.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3954 2023-04-26 01:58:00.000000 pyprobables-0.5.7/tests/test_utilities.py
```

### Comparing `pyprobables-0.5.6/LICENSE` & `pyprobables-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.6/PKG-INFO` & `pyprobables-0.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyprobables
-Version: 0.5.6
+Version: 0.5.7
 Summary: Probabilistic data structures in python
-Home-page: https://github.com/barrust/pyprobables
-Author: Tyler Barrus
-Author-email: barrust@gmail.com
+Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
-Download-URL: https://github.com/barrust/pyprobables/tarball/v0.5.6
-Keywords: python probabilistic data-structure bloom filter count-min sketch bloom-filter count-min-sketch cuckoo-filter
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/barrust/pyprobables
+Project-URL: Bug-tracker, https://github.com/barrust/pyprobables/issues
+Project-URL: Documentation, https://pyprobables.readthedocs.io/
+Keywords: python,probabilistic,data-structure,bloom,filter,count-min,sketch,bloom-filter,count-min-sketch,cuckoo-filter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyProbables
 ===========
 
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
     :target: https://opensource.org/licenses/MIT/
@@ -81,15 +82,15 @@
 To install `pyprobables`, simply clone the `repository on GitHub
 <https://github.com/barrust/pyprobables>`__, then run from the folder:
 
 ::
 
     $ python setup.py install
 
-`pyprobables` supports python 3.5 - 3.9+
+`pyprobables` supports python 3.6 - 3.10+
 
 For *python 2.7* support, install `release 0.3.2 <https://github.com/barrust/pyprobables/releases/tag/v0.3.2>`__
 
 ::
 
     $ pip install pyprobables==0.3.2
 
@@ -244,9 +245,7 @@
         for t_str in tmp:
             hval ^= t_str
             hval *= fnv_64_prime
             hval %= max64mod
         return hval
 
     blm = BloomFilter(filpath="old-file-path.blm", hash_function=old_fnv1a)
-
-
```

### Comparing `pyprobables-0.5.6/README.rst` & `pyprobables-0.5.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 To install `pyprobables`, simply clone the `repository on GitHub
 <https://github.com/barrust/pyprobables>`__, then run from the folder:
 
 ::
 
     $ python setup.py install
 
-`pyprobables` supports python 3.5 - 3.9+
+`pyprobables` supports python 3.6 - 3.10+
 
 For *python 2.7* support, install `release 0.3.2 <https://github.com/barrust/pyprobables/releases/tag/v0.3.2>`__
 
 ::
 
     $ pip install pyprobables==0.3.2
```

### Comparing `pyprobables-0.5.6/probables/__init__.py` & `pyprobables-0.5.7/probables/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     RotatingBloomFilterError,
 )
 
 __author__ = "Tyler Barrus"
 __maintainer__ = "Tyler Barrus"
 __email__ = "barrust@gmail.com"
 __license__ = "MIT"
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 __credits__ = []  # type: ignore
 __url__ = "https://github.com/barrust/pyprobables"
 __bugtrack_url__ = "https://github.com/barrust/pyprobables/issues"
 
 __all__ = [
     "BloomFilter",
     "BloomFilterOnDisk",
```

### Comparing `pyprobables-0.5.6/probables/blooms/bloom.py` & `pyprobables-0.5.7/probables/blooms/bloom.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from shutil import copyfile
 from struct import Struct
 from textwrap import wrap
 from typing import ByteString, Tuple, Union
 
 from ..exceptions import InitializationError, NotSupportedError
 from ..hashes import HashFuncT, HashResultsT, KeyT, default_fnv_1a
-from ..utilities import MMap, is_hex_string, is_valid_file
+from ..utilities import MMap, is_hex_string, is_valid_file, resolve_path
 
 MISMATCH_MSG = "The parameter second must be of type BloomFilter or a BloomFilterOnDisk"
 
 SimpleBloomT = Union["BloomFilter", "BloomFilterOnDisk"]
 
 
 def _verify_not_type_mismatch(second: SimpleBloomT) -> bool:
@@ -45,43 +45,55 @@
     Note:
         Initialization order of operations:
             1) From file
             2) From Hex String
             3) From params
     """
 
-    __slots__ = [
+    __slots__ = (
         "_on_disk",
         "_type",
         "_typecode",
         "_bits_per_elm",
         "_bloom",
         "_est_elements",
         "_fpr",
         "_bloom_length",
         "_hash_func",
         "_els_added",
         "_number_hashes",
         "_num_bits",
-    ]
+    )
 
     def __init__(
         self,
         est_elements: Union[int, None] = None,
         false_positive_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
         hex_string: Union[str, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ):
         # set some things up
         self._on_disk = False
         self._type = "regular"
         self._typecode = "B"
+        self._fpr = 0.0
+        self._bloom_length = 0
+        self._est_elements = 0
         self._bits_per_elm = 8.0
+        self._bloom = []
+        self._hash_func = None
+        self._els_added = 0
+        self._number_hashes = 0
+        self._num_bits = 0
+
+        self._load_init(filepath, hash_function, hex_string, est_elements, false_positive_rate)
 
+    def _load_init(self, filepath, hash_function, hex_string, est_elements, false_positive_rate):
+        """Handle setting params and loading everything as needed"""
         if is_valid_file(filepath):
             self._load(filepath, hash_function)
         elif is_hex_string(hex_string):
             self._load_hex(hex_string, hash_function)
         else:
             if est_elements is None or false_positive_rate is None:
                 raise InitializationError("Insufecient parameters to set up the Bloom Filter")
@@ -285,14 +297,15 @@
 
     def export(self, file: Union[Path, str, IOBase, mmap]) -> None:
         """Export the Bloom Filter to disk
 
         Args:
             filename (str): The filename to which the Bloom Filter will be written."""
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with open(file, "wb") as filepointer:
                 self.export(filepointer)  # type: ignore
         else:
             self._bloom.tofile(file)  # type: ignore
             file.write(
                 self._FOOTER_STRUCT.pack(
                     self.estimated_elements,
@@ -302,44 +315,53 @@
             )
 
     def export_c_header(self, filename: Union[str, Path]) -> None:
         """Export the Bloom Filter to disk as a C header file.
 
         Args:
             filename (str): The filename to which the Bloom Filter will be written."""
-        data = (
-            "  " + line
-            for line in wrap(", ".join(("0x{:02x}".format(e) for e in bytearray.fromhex(self.export_hex()))), 80)
-        )
+        data = ("  " + line for line in wrap(", ".join(f"0x{e:02x}" for e in bytearray.fromhex(self.export_hex())), 80))
         if self._type in ["regular", "regular-on-disk"]:
             bloom_type = "standard BloomFilter"
         else:
             bloom_type = "CountingBloomFilter"
 
-        with open(filename, "w") as file:
-            print("/* BloomFilter Export of a {} */".format(bloom_type), file=file)
+        with open(filename, "w", encoding="utf-8") as file:
+            print(f"/* BloomFilter Export of a {bloom_type} */", file=file)
             print("#include <inttypes.h>", file=file)
-            print("const uint64_t estimated_elements = ", self.estimated_elements, ";", sep="", file=file)
+            print(
+                "const uint64_t estimated_elements = ",
+                self.estimated_elements,
+                ";",
+                sep="",
+                file=file,
+            )
             print("const uint64_t elements_added = ", self.elements_added, ";", sep="", file=file)
-            print("const float false_positive_rate = ", self.false_positive_rate, ";", sep="", file=file)
+            print(
+                "const float false_positive_rate = ",
+                self.false_positive_rate,
+                ";",
+                sep="",
+                file=file,
+            )
             print("const uint64_t number_bits = ", self.number_bits, ";", sep="", file=file)
             print("const unsigned int number_hashes = ", self.number_hashes, ";", sep="", file=file)
             print("const unsigned char bloom[] = {", *data, "};", sep="\n", file=file)
 
     @classmethod
     def frombytes(cls, b: ByteString, hash_function: Union[HashFuncT, None] = None) -> "BloomFilter":
         """
         Args:
             b (ByteString): The bytes to load as a Bloom Filter
             hash_function (function): Hashing strategy function to use `hf(key, number)`
         Returns:
             BloomFilter: A Bloom Filter object
         """
         offset = cls._FOOTER_STRUCT.size
-        est_els, els_added, fpr, _, _ = cls._parse_footer(cls._FOOTER_STRUCT, bytes(b[-offset:]))
+        est_els, els_added, fpr, _, _ = cls._parse_footer(cls._FOOTER_STRUCT, bytes(b[-1 * offset :]))
         blm = BloomFilter(est_elements=est_els, false_positive_rate=fpr, hash_function=hash_function)
         blm._load(b, hash_function=blm.hash_function)
         blm._els_added = els_added
         return blm
 
     def estimate_elements(self) -> int:
         """Estimate the number of unique elements added
@@ -486,15 +508,20 @@
 
         if number_hashes == 0:
             raise InitializationError("Bloom: Number hashes is zero; unusable parameters provided")
 
         return t_fpr, number_hashes, m_bt
 
     def _set_values(
-        self, est_els: int, fpr: float, n_hashes: int, n_bits: int, hash_func: Union[HashFuncT, None]
+        self,
+        est_els: int,
+        fpr: float,
+        n_hashes: int,
+        n_bits: int,
+        hash_func: Union[HashFuncT, None],
     ) -> None:
         self._est_elements = est_els
         self._fpr = fpr
         self._bloom_length = math.ceil(n_bits / self._bits_per_elm)
         if hash_func is not None:
             self._hash_func = hash_func
         else:
@@ -516,21 +543,21 @@
     def _load(
         self,
         file: Union[Path, str, IOBase, mmap, ByteString],
         hash_function: Union[HashFuncT, None] = None,
     ) -> None:
         """load the Bloom Filter from file or bytes"""
         if not isinstance(file, (IOBase, mmap, ByteString)):
-            file = Path(file)
+            file = resolve_path(file)
             with MMap(file) as filepointer:
                 self._load(filepointer, hash_function)
         else:
             offset = self._FOOTER_STRUCT.size
             est_els, els_added, fpr, n_hashes, n_bits = self._parse_footer(
-                self._FOOTER_STRUCT, file[-offset:]  # type: ignore
+                self._FOOTER_STRUCT, file[-1 * offset :]  # type: ignore
             )
             self._set_values(est_els, fpr, n_hashes, n_bits, hash_function)
             # now read in the bit array!
             self._parse_bloom_array(file, self._IMPT_STRUCT.size * self.bloom_length)  # type: ignore
             self._els_added = els_added
 
     @classmethod
@@ -600,33 +627,34 @@
         filepath: Union[str, Path],
         est_elements: Union[int, None] = None,
         false_positive_rate: Union[float, None] = None,
         hex_string: Union[str, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ) -> None:
         # set some things up
-        self._filepath = Path(filepath)
+        self._filepath = resolve_path(filepath)
         self.__file_pointer = None
+        super().__init__(est_elements, false_positive_rate, filepath, hex_string, hash_function)
+
+    def _load_init(self, filepath, hash_function, hex_string, est_elements, false_positive_rate):
+        """Handle setting params and loading everything as needed"""
         self._type = "regular-on-disk"
-        self._typecode = "B"
-        self._bits_per_elm = 8.0
         self._on_disk = True
-
         if is_hex_string(hex_string):
             msg = "Loading from hex_string is currently not supported by the on disk Bloom Filter"
             raise NotSupportedError(msg)
         if est_elements is not None and false_positive_rate is not None:
             fpr, n_hashes, n_bits = self._get_optimized_params(est_elements, false_positive_rate)
             self._set_values(est_elements, fpr, n_hashes, n_bits, hash_function)
 
-            with open(filepath, "wb") as filepointer:
+            with open(self._filepath, "wb") as filepointer:
                 (array(self._typecode, [0]) * self.bloom_length).tofile(filepointer)
                 filepointer.write(self._FOOTER_STRUCT.pack(est_elements, 0, false_positive_rate))
                 filepointer.flush()
-            self._load(filepath, hash_function)
+            self._load(self._filepath, hash_function)
         elif is_valid_file(self._filepath):
             self._load(self._filepath.name, hash_function)  # need .name for python 3.5
         else:
             raise InitializationError("Insufecient parameters to set up the On Disk Bloom Filter")
 
     def __del__(self) -> None:
         """handle if user doesn't close the on disk Bloom Filter"""
@@ -655,15 +683,16 @@
             copyfile(self._filepath.name, str(filename))
         # otherwise, nothing to do!
 
     def _load(self, filepath: Union[str, Path], hash_function: Union[HashFuncT, None] = None):  # type: ignore
         """load the Bloom Filter on disk"""
         # read the file, set the optimal params
         # mmap everything
-        with open(filepath, "r+b") as filepointer:
+        file = resolve_path(filepath)
+        with open(file, "r+b") as filepointer:
             offset = self._FOOTER_STRUCT.size
             filepointer.seek(offset * -1, os.SEEK_END)
             est_els, _, fpr = self._FOOTER_STRUCT.unpack_from(filepointer.read(offset))
 
             fpr, n_hashes, n_bits = self._get_optimized_params(est_els, fpr)
             self._set_values(est_els, fpr, n_hashes, n_bits, hash_function)
         # setup a few additional items
@@ -689,10 +718,10 @@
     def _get_element(self, idx: int) -> int:
         """wrappper to use similar functions always!"""
         return int(self._IMPT_STRUCT.unpack(bytes([self._bloom[idx]]))[0])
 
     def __update(self):
         """update the on disk Bloom Filter and ensure everything is out to disk"""
         self._bloom.flush()
-        self.__file_pointer.seek(-self._UPDATE_OFFSET.size, os.SEEK_END)
+        self.__file_pointer.seek(-1 * self._UPDATE_OFFSET.size, os.SEEK_END)
         self.__file_pointer.write(self._EXPECTED_ELM_STRUCT.pack(self.elements_added))
         self.__file_pointer.flush()
```

### Comparing `pyprobables-0.5.6/probables/blooms/countingbloom.py` & `pyprobables-0.5.7/probables/blooms/countingbloom.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from struct import Struct
 from typing import ByteString, Union
 
 from ..constants import UINT32_T_MAX, UINT64_T_MAX
 from ..exceptions import InitializationError
 from ..hashes import HashFuncT, HashResultsT, KeyT
-from ..utilities import is_hex_string, is_valid_file
+from ..utilities import is_hex_string, is_valid_file, resolve_path
 from .bloom import BloomFilter
 
 MISMATCH_MSG = "The parameter second must be of type CountingBloomFilter"
 
 
 def _verify_not_type_mismatch(second: "CountingBloomFilter") -> bool:
     """verify that there is not a type mismatch"""
@@ -38,32 +38,37 @@
 
     Note:
         Initialization order of operations:
             1) From file
             2) From Hex String
             3) From params"""
 
-    __slots__ = BloomFilter.__slots__
+    __slots__ = ("_filepath",)
 
     def __init__(
         self,
         est_elements: Union[int, None] = None,
         false_positive_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
         hex_string: Union[str, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ) -> None:
         """setup the basic values needed"""
+        self._filepath = None
+        super().__init__(est_elements, false_positive_rate, filepath, hex_string, hash_function)
+
+    def _load_init(self, filepath, hash_function, hex_string, est_elements, false_positive_rate):
+        """Handle setting params and loading everything as needed"""
         self._bits_per_elm = 1.0
-        self._on_disk = False
         self._type = "counting"
         self._typecode = "I"
-        self._els_added = 0
+
         if is_valid_file(filepath):
-            self._load(filepath, hash_function)
+            self._filepath = resolve_path(filepath)
+            self._load(self._filepath, hash_function)
         elif is_hex_string(hex_string):
             self._load_hex(hex_string, hash_function)
         else:
             if est_elements is None or false_positive_rate is None:
                 raise InitializationError("Insufecient parameters to set up the Counting Bloom Filter")
             # calc values
             fpr, n_hashes, n_bits = self._get_optimized_params(est_elements, false_positive_rate)
@@ -79,26 +84,26 @@
         Args:
             b (ByteString): the bytes to load as a Counting Bloom Filter
             hash_function (function): Hashing strategy function to use `hf(key, number)`
         Returns:
             CountingBloomFilter: A Counting Bloom Filter object
         """
         offset = cls._FOOTER_STRUCT.size
-        est_els, els_added, fpr, n_hashes, n_bits = cls._parse_footer(cls._FOOTER_STRUCT, bytes(b[-offset:]))
+        est_els, els_added, fpr, n_hashes, n_bits = cls._parse_footer(cls._FOOTER_STRUCT, bytes(b[-1 * offset :]))
         blm = CountingBloomFilter(est_elements=est_els, false_positive_rate=fpr, hash_function=hash_function)
         blm._set_values(est_els, fpr, n_hashes, n_bits, hash_function)
         blm._els_added = els_added
         blm._parse_bloom_array(b, cls._IMPT_STRUCT.size * blm.bloom_length)
         return blm
 
     def __str__(self) -> str:
         """string representation of the counting bloom filter"""
         on_disk = "no" if self.is_on_disk is False else "yes"
 
-        cnt = sum([x for x in self._bloom if x > 0])
+        cnt = sum(x for x in self._bloom if x > 0)
         total = sum(self._bloom)
         largest = max(self._bloom)
         largest_idx = (self._bloom).index(largest)
         fullness = cnt / self.number_bits
         els_added = total // self.number_hashes
 
         stats = (
@@ -154,17 +159,15 @@
         for i, v in enumerate(vals):
             k = indices[i]
             if v > UINT32_T_MAX:
                 self._bloom[k] = UINT32_T_MAX
                 vals[i] = UINT32_T_MAX
             else:
                 self._bloom[k] += num_els  # This keeps the original methodology
-        self.elements_added += num_els
-        if self.elements_added > UINT64_T_MAX:
-            self.elements_added = UINT64_T_MAX
+        self.elements_added = min(self.elements_added + num_els, UINT64_T_MAX)
         return min(vals)
 
     def check(self, key: KeyT) -> int:  # type: ignore
         """Check if the key is likely in the Counting Bloom Filter
 
         Args:
             key (str): The element to be checked
@@ -176,15 +179,15 @@
         """Check if the element represented by hashes is in the Counting
         Bloom Filter
 
         Args:
             hashes (list): A list of integers representing the key to check
         Returns:
             int: Maximum number of insertions"""
-        return min([self._bloom[x % self.number_bits] for x in hashes])
+        return min(self._bloom[x % self.number_bits] for x in hashes)
 
     def remove(self, key: KeyT, num_els: int = 1) -> int:
         """Remove the element from the counting bloom
 
         Args:
             key (str): The element to be removed
             num_els (int): Number of times to remove the element
@@ -308,8 +311,8 @@
             tmp = self._bloom[i] + second._bloom[i]
             res._bloom[i] = tmp
         res.elements_added = res.estimate_elements()
         return res
 
     def _cnt_number_bits_set(self) -> int:
         """calculate the total number of set bits in the bloom"""
-        return sum([1 for x in self._bloom if x > 0])
+        return sum(1 for x in self._bloom if x > 0)
```

### Comparing `pyprobables-0.5.6/probables/blooms/expandingbloom.py` & `pyprobables-0.5.7/probables/blooms/expandingbloom.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmap import mmap
 from pathlib import Path
 from struct import Struct
 from typing import ByteString, Tuple, Union
 
 from ..exceptions import RotatingBloomFilterError
 from ..hashes import HashFuncT, HashResultsT, KeyT
-from ..utilities import MMap, is_valid_file
+from ..utilities import MMap, is_valid_file, resolve_path
 from .bloom import BloomFilter
 
 
 class ExpandingBloomFilter:
     """Simple expanding Bloom Filter implementation for use in python; the
     Bloom Fiter will automatically expand, or grow, if the false
     positive rate is about to become greater than the desired false
@@ -31,31 +31,31 @@
     Returns:
         ExpandingBloomFilter: An expanding Bloom Filter object
     Note:
         Initialization order of operations:
             1) Filepath
             2) est_elements and false_positive_rate"""
 
-    __slots__ = [
+    __slots__ = (
         "_blooms",
         "__fpr",
         "__est_elements",
         "__hash_func",
         "_added_elements",
-    ]
+    )
 
     def __init__(
         self,
         est_elements: Union[int, None] = None,
         false_positive_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ):
         """initialize"""
-        self._blooms = list()  # type: ignore
+        self._blooms = []  # type: ignore
         self.__fpr = false_positive_rate
         self.__est_elements = est_elements
         self.__hash_func = hash_function
         self._added_elements = 0  # total added...
 
         if is_valid_file(filepath):
             self.__load(filepath)
@@ -96,27 +96,32 @@
     @property
     def expansions(self) -> int:
         """int: The number of expansions"""
         return len(self._blooms) - 1
 
     @property
     def false_positive_rate(self) -> float:
-        """ float: The desired false positive rate of the expanding Bloom Filter """
+        """float: The desired false positive rate of the expanding Bloom Filter"""
         return self.__fpr
 
     @property
     def estimated_elements(self) -> int:
-        """int: The original number of elements estimated to be in the Bloom Filter """
+        """int: The original number of elements estimated to be in the Bloom Filter"""
         return self.__est_elements
 
     @property
     def elements_added(self) -> int:
         """int: The total number of elements added"""
         return self._added_elements
 
+    @property
+    def hash_function(self) -> HashFuncT:
+        """int: The total number of elements added"""
+        return self.__hash_func
+
     def push(self) -> None:
         """Push a new expansion onto the Bloom Filter"""
         self.__add_bloom_filter()
 
     def check(self, key: KeyT) -> bool:
         """Check to see if the key is in the Bloom Filter
 
@@ -177,14 +182,15 @@
 
     def export(self, file: Union[Path, str, IOBase, mmap]) -> None:
         """Export an expanding Bloom Filter, or subclass, to disk
 
         Args:
             filepath (str): The path to the file to import"""
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with open(file, "wb") as filepointer:
                 self.export(filepointer)  # type:ignore
         else:
             filepointer = file  # type:ignore
             # add all the different Bloom bit arrays...
             for blm in self._blooms:
                 filepointer.write(self.__S_INT64_STRUCT.pack(blm.elements_added))
@@ -197,33 +203,34 @@
                     self.false_positive_rate,
                 )
             )
 
     def __load(self, file: Union[Path, str, IOBase, mmap]):
         """load a file"""
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with MMap(file) as filepointer:
                 self.__load(filepointer)
         else:
             size, est_els, els_added, fpr = self._parse_footer(file)  # type: ignore
-            self._blooms = list()
+            self._blooms = []
             self._added_elements = els_added
             self.__fpr = fpr
             self.__est_elements = est_els
             self._parse_blooms(file, size)  # type:ignore
 
     @classmethod
     def _parse_footer(cls, b: ByteString) -> Tuple[int, int, int, float]:
         offset = cls.__FOOTER_STRUCT.size
-        size, est_els, els_added, fpr = cls.__FOOTER_STRUCT.unpack(bytes(b[-offset:]))
+        size, est_els, els_added, fpr = cls.__FOOTER_STRUCT.unpack(bytes(b[-1 * offset :]))
         return int(size), int(est_els), int(els_added), float(fpr)
 
     def _parse_blooms(self, b: ByteString, size: int) -> None:
         # reset the bloom list
-        self._blooms = list()
+        self._blooms = []
         blm_size = 0
         start = 0
         end = 0
         for _ in range(size):
             blm = BloomFilter(
                 est_elements=self.__est_elements,
                 false_positive_rate=self.__fpr,
@@ -254,22 +261,15 @@
         hash_function (function): Hashing strategy function to use `hf(key, number)`
     Note:
         Initialization order of operations:
             1) Filepath
             2) est_elements and false_positive_rate
     """
 
-    __slots__ = [
-        "_blooms",
-        "__fpr",
-        "__est_elements",
-        "__hash_func",
-        "_added_elements",
-        "_queue_size",
-    ]
+    __slots__ = ("_queue_size",)
 
     def __init__(
         self,
         est_elements: Union[int, None] = None,
         false_positive_rate: Union[float, None] = None,
         max_queue_size: int = 10,
         filepath: Union[str, Path, None] = None,
@@ -279,18 +279,14 @@
         super().__init__(
             est_elements=est_elements,
             false_positive_rate=false_positive_rate,
             filepath=filepath,
             hash_function=hash_function,
         )
         self._queue_size = max_queue_size
-        self._added_elements = self.elements_added
-        self.__est_elements = self.estimated_elements
-        self.__fpr = self.false_positive_rate
-        self.__hash_func = hash_function
 
     @classmethod
     def frombytes(  # type:ignore
         cls, b: ByteString, max_queue_size: int, hash_function: Union[HashFuncT, None] = None
     ) -> "RotatingBloomFilter":
         """
         Args:
@@ -361,12 +357,12 @@
         elif ready_to_rotate:
             blm = self._blooms.pop(0)
             self.__add_bloom_filter()
 
     def __add_bloom_filter(self):
         """build a new bloom and add it on!"""
         blm = BloomFilter(
-            est_elements=self.__est_elements,
-            false_positive_rate=self.__fpr,
-            hash_function=self.__hash_func,
+            est_elements=self.estimated_elements,
+            false_positive_rate=self.false_positive_rate,
+            hash_function=self.hash_function,
         )
         self._blooms.append(blm)
```

### Comparing `pyprobables-0.5.6/probables/countminsketch/countminsketch.py` & `pyprobables-0.5.7/probables/countminsketch/countminsketch.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pathlib import Path
 from struct import Struct
 from typing import ByteString, Dict, Tuple, Union
 
 from ..constants import INT32_T_MAX, INT32_T_MIN, INT64_T_MAX, INT64_T_MIN
 from ..exceptions import CountMinSketchError, InitializationError, NotSupportedError
 from ..hashes import HashFuncT, HashResultsT, KeyT, default_fnv_1a
-from ..utilities import MMap, is_valid_file
+from ..utilities import MMap, is_valid_file, resolve_path
 
 
 class CountMinSketch:
     """Simple Count-Min Sketch implementation for use in python;
     It can read and write the same format as the c version
     (https://github.com/barrust/count-min-sketch)
 
@@ -41,24 +41,24 @@
             3) Confidence and error rate
     Note:
         Default query type is `min`
     Note:
         For width and depth, width may realistically be in the thousands while depth \
             is in the single digit to teens"""
 
-    __slots__ = [
+    __slots__ = (
         "__width",
         "__depth",
         "__confidence",
         "__error_rate",
         "__elements_added",
         "__query_method",
         "_bins",
         "_hash_function",
-    ]
+    )
 
     def __init__(
         self,
         width: Union[int, None] = None,
         depth: Union[int, None] = None,
         confidence: Union[float, None] = None,
         error_rate: Union[float, None] = None,
@@ -71,14 +71,15 @@
         self.__depth = 0
         self.__confidence = 0.0
         self.__error_rate = 0.0
         self.__elements_added = 0
         self.__query_method = self.__min_query
 
         if is_valid_file(filepath):
+            filepath = resolve_path(filepath)
             self.__load(filepath)
         else:
             if width is not None and depth is not None:
                 valid_prms = isinstance(width, Number) and width > 0 and isinstance(depth, Number) and depth > 0
                 if not valid_prms:
                     msg = "CountMinSketch: width and depth must be greater than 0"
                     raise InitializationError(msg)
@@ -155,15 +156,15 @@
         Args:
             b (ByteString): The bytes to load as a Count-Min Sketch
             hash_function (function): Hashing strategy function to use `hf(key, number)`
         Returns:
             CountMinSketch: A count-min sketch object
         """
         offset = cls.__FOOTER_STRUCT.size
-        width, depth, _ = cls.__FOOTER_STRUCT.unpack_from(bytes(b[-offset:]))
+        width, depth, _ = cls.__FOOTER_STRUCT.unpack_from(bytes(b[-1 * offset :]))
         cms = CountMinSketch(width=width, depth=depth, hash_function=hash_function)
         cms._parse_bytes(b)
         return cms
 
     @property
     def width(self) -> int:
         """int: The width of the count-min sketch
@@ -340,14 +341,15 @@
 
     def export(self, file: Union[Path, str, IOBase, mmap]) -> None:
         """Export the count-min sketch to disk
 
         Args:
             filename (str): The filename to which the count-min sketch will be written."""
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with open(file, "wb") as filepointer:
                 self.export(filepointer)  # type: ignore
         else:
             # write out the bins
             self._bins.tofile(file)  # type: ignore
             file.write(self.__FOOTER_STRUCT.pack(self.width, self.depth, self.elements_added))
 
@@ -362,15 +364,15 @@
                 or :class:`CountMeanMinSketch`
             CountMinSketchError: Raised when the count-min sketches are not of the same dimensions
         Note:
             The calling count-min sketch will contain the combined data
             once complete
         """
         if not isinstance(second, (CountMinSketch)):
-            msg = "Unable to merge a count-min sketch with {}".format(type(second))
+            msg = f"Unable to merge a count-min sketch with {type(second)}"
             raise TypeError(msg)
         if (
             (self.width != second.width)
             or (self.depth != second.depth)
             or (self.hashes("test") != second.hashes("test"))
         ):
             raise CountMinSketchError("Unable to merge as the count-min sketches are mismatched")
@@ -395,25 +397,25 @@
             self.__elements_added = INT64_T_MAX
         elif self.elements_added < INT64_T_MIN:
             self.__elements_added = INT64_T_MIN
 
     def __load(self, file: Union[Path, str, IOBase, mmap]):
         """load the count-min sketch from file"""
         if not isinstance(file, (IOBase, mmap)):
-            file = Path(file)
+            file = resolve_path(file)
             with MMap(file) as filepointer:
                 self.__load(filepointer)
         else:
             self._parse_bytes(file)  # type: ignore
 
     @classmethod
     def _parse_footer(cls, file: ByteString) -> Tuple[int, int, int]:
         """return width, depth and elements added, in that order"""
         offset = cls.__FOOTER_STRUCT.size
-        width, depth, elements_added = cls.__FOOTER_STRUCT.unpack_from(bytes(file[-offset:]))
+        width, depth, elements_added = cls.__FOOTER_STRUCT.unpack_from(bytes(file[-1 * offset :]))
         return width, depth, elements_added
 
     def _parse_bytes(self, file: ByteString):
         """parse bytes or a mapped file to setup the CountMin-Sketch"""
         width, depth, els_added = self._parse_footer(file)
         self.__width = width
         self.__depth = depth
@@ -433,15 +435,15 @@
         """generate the mean query; assumes sorted list"""
         return sum(results) // self.depth
 
     def __mean_min_query(self, results: HashResultsT) -> int:
         """generate the mean-min query; assumes sorted list"""
         if results[0] == 0 and results[-1] == 0:
             return 0
-        meanmin = list()
+        meanmin = []
         for t_bin in results:
             diff = self.elements_added - t_bin
             calc = t_bin - diff // (self.width - 1)
             meanmin.append(calc)
         meanmin.sort()
         if self.depth % 2 == 0:
             calc = meanmin[self.depth // 2] + meanmin[self.depth // 2 - 1]
@@ -472,16 +474,14 @@
             3) Confidence and error rate
     Note:
         Default query type is `mean`
     Note:
         For width and depth, width may realistically be in the thousands while depth is \
             in the single digit to teens"""
 
-    __slots__ = CountMinSketch.__slots__
-
     def __init__(
         self,
         width: Union[int, None] = None,
         depth: Union[int, None] = None,
         confidence: Union[float, None] = None,
         error_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
@@ -512,16 +512,14 @@
             3) Confidence and error rate
     Note:
         Default query type is `mean-min`
     Note:
         For width and depth, width may realistically be in the thousands while depth is \
             in the single digit to teens"""
 
-    __slots__ = CountMinSketch.__slots__
-
     def __init__(
         self,
         width: Union[int, None] = None,
         depth: Union[int, None] = None,
         confidence: Union[float, None] = None,
         error_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
@@ -566,15 +564,15 @@
         confidence: Union[float, None] = None,
         error_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ) -> None:
 
         super().__init__(width, depth, confidence, error_rate, filepath, hash_function)
-        self.__top_x = dict()  # type: ignore
+        self.__top_x = {}  # type: ignore
         self.__top_x_size = 0
         self.__num_hitters = num_hitters
         self.__smallest = 0
 
     @classmethod
     def frombytes(  # type: ignore
         cls, b: ByteString, num_hitters: int = 100, hash_function: Union[HashFuncT, None] = None
@@ -674,15 +672,15 @@
             "make sense)!"
         )
         raise NotSupportedError(msg)
 
     def clear(self) -> None:
         """Clear out the heavy hitters!"""
         super().clear()
-        self.__top_x = dict()
+        self.__top_x = {}
         self.__top_x_size = 0
         self.__smallest = 0
 
     def join(self, second: "HeavyHitters"):  # type: ignore
         """Join is not supported by HeavyHitters
 
         Raises:
@@ -725,15 +723,15 @@
         confidence: Union[float, None] = None,
         error_rate: Union[float, None] = None,
         filepath: Union[str, Path, None] = None,
         hash_function: Union[HashFuncT, None] = None,
     ) -> None:
         super().__init__(width, depth, confidence, error_rate, filepath, hash_function)
         self.__threshold = threshold
-        self.__meets_threshold = dict()  # type: ignore
+        self.__meets_threshold = {}  # type: ignore
 
     @classmethod
     def frombytes(  # type: ignore
         cls, b: ByteString, threshold: int = 100, hash_function: Union[HashFuncT, None] = None
     ) -> "StreamThreshold":
         """
         Args:
@@ -763,15 +761,15 @@
     def threshold(self) -> int:
         """int: The threshold at which a key is tracked"""
         return self.__threshold
 
     def clear(self) -> None:
         """Clear out the stream threshold!"""
         super().clear()
-        self.__meets_threshold = dict()
+        self.__meets_threshold = {}
 
     def add(self, key: str, num_els: int = 1) -> int:  # type: ignore
         """Add the element for key into the data structure
 
         Args:
             key (str): The element to add
             num_els (int): The number of instances to add
```

### Comparing `pyprobables-0.5.6/probables/cuckoo/countingcuckoo.py` & `pyprobables-0.5.7/probables/cuckoo/countingcuckoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from mmap import mmap
 from pathlib import Path
 from struct import Struct
 from typing import ByteString, List, Union
 
 from ..exceptions import CuckooFilterFullError
 from ..hashes import KeyT, SimpleHashT
-from ..utilities import MMap
+from ..utilities import MMap, resolve_path
 from .cuckoo import CuckooFilter
 
 
 class CountingCuckooFilter(CuckooFilter):
     """Simple Counting Cuckoo Filter implementation
 
     Args:
@@ -29,23 +29,15 @@
         finger_size (int): The size of the fingerprint to use in bytes \
             (between 1 and 4); exported as 4 bytes; up to the user to \
             reset the size correctly on import
         filename (str): The path to the file to load or None if no file
     Returns:
         CountingCuckooFilter: A Cuckoo Filter object"""
 
-    __slots__ = [
-        "__unique_elements",
-        "_inserted_elements",
-        "_bucket_size",
-        "__max_cuckoo_swaps",
-        "_cuckoo_capacity",
-        "_buckets",
-        "_fingerprint_size",
-    ]
+    __slots__ = ("__unique_elements",)
 
     def __init__(
         self,
         capacity: int = 10000,
         bucket_size: int = 4,
         max_swaps: int = 500,
         expansion_rate: int = 2,
@@ -114,14 +106,15 @@
             error_rate (float):
             filepath (str): The path to the file to load or None if no file
             hash_function (function): Hashing strategy function to use \
             `hf(key)`
         Returns:
             CuckooFilter: A Cuckoo Filter object
         """
+        filepath = resolve_path(filepath)
         cku = CountingCuckooFilter(filepath=filepath, hash_function=hash_function)
         cku._set_error_rate(error_rate)
         return cku
 
     @classmethod
     def frombytes(
         cls, b: ByteString, error_rate: Union[float, None] = None, hash_function: Union[SimpleHashT, None] = None
@@ -225,14 +218,15 @@
 
     def export(self, file: Union[Path, str, IOBase, mmap]) -> None:
         """Export cuckoo filter to file
 
         Args:
             file (str): Path to file to export"""
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with open(file, "wb") as filepointer:
                 self.export(filepointer)  # type:ignore
         else:
             self.__bucket_decomposition(self.buckets, self.bucket_size).tofile(file)
             # now put out the required information at the end
             file.write(self.__COUNTING_CUCKOO_FOOTER_STRUCT.pack(self.bucket_size, self.max_swaps))
 
@@ -280,39 +274,31 @@
         if fingerprint in [x.finger for x in self.buckets[idx_2]]:
             return idx_2
         return None
 
     def _load(self, file: Union[Path, str, IOBase, mmap, bytes, ByteString]) -> None:
         """load a cuckoo filter from file"""
         if not isinstance(file, (IOBase, mmap, bytes, ByteString)):
-            file = Path(file)
+            file = resolve_path(file)
             with MMap(file) as filepointer:
                 self._load(filepointer)
         else:
-            self._parse_footer(file)  # type: ignore
+            self._parse_footer(file, self.__COUNTING_CUCKOO_FOOTER_STRUCT)  # type: ignore
             self._inserted_elements = 0
             self._parse_buckets(file)  # type: ignore
 
-    def _parse_footer(self, d: ByteString) -> None:
-        """Parse bytes to pull out and set footer information"""
-        bucket_size, max_swaps = self.__COUNTING_CUCKOO_FOOTER_STRUCT.unpack(
-            bytes(d[-self.__COUNTING_CUCKOO_FOOTER_STRUCT.size :])
-        )
-        self._bucket_size = int(bucket_size)
-        self.__max_cuckoo_swaps = int(max_swaps)
-
     def _parse_buckets(self, d: ByteString) -> None:
         """Parse bytes to pull out and set the buckets"""
         bin_size = self.__BIN_STRUCT.size
         self._cuckoo_capacity = (len(bytes(d)) - bin_size) // bin_size // self.bucket_size
         start = 0
         end = bin_size
-        self._buckets = list()
+        self._buckets = []
         for i in range(self.capacity):
-            self.buckets.append(list())
+            self.buckets.append([])
             for _ in range(self.bucket_size):
                 finger, count = self.__BIN_STRUCT.unpack(bytes(d[start:end]))
                 if finger > 0:
                     ccb = CountingCuckooBin(finger, count)
                     self.buckets[i].append(ccb)
                     self._inserted_elements += count
                     self.__unique_elements += 1
@@ -381,15 +367,15 @@
 
     def __repr__(self) -> str:
         """how do we represent this?"""
         return self.__str__()
 
     def __str__(self) -> str:
         """convert it into a string"""
-        return "(fingerprint:{} count:{})".format(self.__bin[0], self.__bin[1])
+        return f"(fingerprint:{self.__bin[0]} count:{self.__bin[1]})"
 
     def increment(self) -> int:
         """increment"""
         self.__bin[1] += 1
         return self.__bin[1]
 
     def decrement(self) -> int:
```

### Comparing `pyprobables-0.5.6/probables/cuckoo/cuckoo.py` & `pyprobables-0.5.7/probables/cuckoo/cuckoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from numbers import Number
 from pathlib import Path
 from struct import Struct
 from typing import ByteString, List, Tuple, Union
 
 from ..exceptions import CuckooFilterFullError, InitializationError
 from ..hashes import KeyT, SimpleHashT, fnv_1a
-from ..utilities import MMap, get_x_bits, is_valid_file
+from ..utilities import MMap, get_x_bits, is_valid_file, resolve_path
 
 
 class CuckooFilter:
     """Simple Cuckoo Filter implementation
 
     Args:
         capacity (int): The number of bins
@@ -31,26 +31,26 @@
             (between 1 and 4); exported as 4 bytes; up to the user to \
             reset the size correctly on import
         filepath (str): The path to the file to load or None if no file
         hash_function (function): Hashing strategy function to use `hf(key)`
     Returns:
         CuckooFilter: A Cuckoo Filter object"""
 
-    __slots__ = [
+    __slots__ = (
         "_bucket_size",
         "_cuckoo_capacity",
         "__max_cuckoo_swaps",
         "__expansion_rate",
         "__auto_expand",
         "_fingerprint_size",
         "__hash_func",
         "_inserted_elements",
         "_buckets",
         "_error_rate",
-    ]
+    )
 
     def __init__(
         self,
         capacity: int = 10000,
         bucket_size: int = 4,
         max_swaps: int = 500,
         expansion_rate: int = 2,
@@ -83,18 +83,19 @@
 
         if hash_function is None:
             self.__hash_func = fnv_1a
         else:
             self.__hash_func = hash_function  # type: ignore
         self._inserted_elements = 0
         if filepath is None:
-            self._buckets = list()  # type: ignore
+            self._buckets = []  # type: ignore
             for _ in range(self.capacity):
-                self.buckets.append(list())
+                self.buckets.append([])
         elif is_valid_file(filepath):
+            filepath = resolve_path(filepath)
             self._load(filepath)
         else:
             msg = "CuckooFilter: failed to load provided file"
             raise InitializationError(msg)
 
         self._error_rate = float(self._calc_error_rate())
 
@@ -131,31 +132,38 @@
             hash_function=hash_function,
         )
         cku._set_error_rate(error_rate)
         return cku
 
     @classmethod
     def load_error_rate(
-        cls, error_rate: float, filepath: Union[str, Path], hash_function: Union[SimpleHashT, None] = None
+        cls,
+        error_rate: float,
+        filepath: Union[str, Path],
+        hash_function: Union[SimpleHashT, None] = None,
     ):
         """Initialize a previously exported Cuckoo Filter based on error rate
 
         Args:
             error_rate (float):
             filepath (str): The path to the file to load or None if no file
             hash_function (function): Hashing strategy function to use `hf(key)`
         Returns:
             CuckooFilter: A Cuckoo Filter object"""
+        filepath = resolve_path(filepath)
         cku = CuckooFilter(filepath=filepath, hash_function=hash_function)
         cku._set_error_rate(error_rate)
         return cku
 
     @classmethod
     def frombytes(
-        cls, b: ByteString, error_rate: Union[float, None] = None, hash_function: Union[SimpleHashT, None] = None
+        cls,
+        b: ByteString,
+        error_rate: Union[float, None] = None,
+        hash_function: Union[SimpleHashT, None] = None,
     ) -> "CuckooFilter":
         """
         Args:
             b (ByteString): The bytes to load as a Expanding Bloom Filter
             error_rate (float): The error rate of the cuckoo filter, if used to generate the original filter
             hash_function (function): Hashing strategy function to use `hf(key, number)`
         Returns:
@@ -276,15 +284,15 @@
         return math.ceil(self.fingerprint_size_bits / 8)
 
     @fingerprint_size.setter
     def fingerprint_size(self, val: int):
         """set the fingerprint size"""
         tmp = val
         if not 1 <= tmp <= 4:
-            msg = ("{}: fingerprint size must be between 1 and 4").format(self.__class__.__name__)
+            msg = f"{self.__class__.__name__}: fingerprint size must be between 1 and 4"
             raise ValueError(msg)
         # bytes to bits
         self._fingerprint_size = tmp * 8
         self._calc_error_rate()  # if updating fingerprint size then error rate may change
 
     def load_factor(self) -> float:
         """float: How full the Cuckoo Filter is currently"""
@@ -336,20 +344,21 @@
     def export(self, file: Union[Path, str, IOBase, mmap]) -> None:
         """Export cuckoo filter to file
 
         Args:
             file: Path to file to export"""
 
         if not isinstance(file, (IOBase, mmap)):
+            file = resolve_path(file)
             with open(file, "wb") as filepointer:
                 self.export(filepointer)  # type:ignore
         else:
             filepointer = file  # type:ignore
-            for i in range(len(self.buckets)):
-                bucket = array(self._CUCKOO_SINGLE_INT_C, self.buckets[i])
+            for _, val in enumerate(self.buckets):
+                bucket = array(self._CUCKOO_SINGLE_INT_C, val)
                 bucket.extend([0] * (self.bucket_size - len(bucket)))
                 bucket.tofile(filepointer)
             # now put out the required information at the end
             filepointer.write(self._CUCKOO_FOOTER_STRUCT.pack(self.bucket_size, self.max_swaps))
 
     def __bytes__(self) -> bytes:
         """Export cuckoo filter to `bytes`"""
@@ -393,36 +402,36 @@
 
         # if we got here we have an error... we might need to know what is left
         return fingerprint
 
     def _load(self, file: Union[Path, str, IOBase, mmap, bytes]) -> None:
         """load a cuckoo filter from file"""
         if not isinstance(file, (IOBase, mmap, bytes)):
-            file = Path(file)
+            file = resolve_path(file)
             with MMap(file) as filepointer:
                 self._load(filepointer)
         else:
-            self._parse_footer(file)  # type: ignore
+            self._parse_footer(file, self._CUCKOO_FOOTER_STRUCT)  # type: ignore
             self._inserted_elements = 0
             # now pull everything in!
             self._parse_buckets(file)  # type: ignore
 
     _CUCKOO_SINGLE_INT_C = "I"
     _CUCKOO_SINGLE_INT_SIZE = Struct(_CUCKOO_SINGLE_INT_C).size
     _CUCKOO_FOOTER_STRUCT = Struct("II")
 
-    def _parse_footer(self, d: ByteString) -> None:
+    def _parse_footer(self, d: ByteString, stct: Struct) -> None:
         """parse bytes and set footer information"""
-        list_size = len(d) - self._CUCKOO_FOOTER_STRUCT.size
-        self._bucket_size, self.__max_cuckoo_swaps = self._CUCKOO_FOOTER_STRUCT.unpack(d[list_size:])  # type:ignore
+        list_size = len(d) - stct.size
+        self._bucket_size, self.__max_cuckoo_swaps = stct.unpack(d[list_size:])  # type:ignore
         self._cuckoo_capacity = list_size // self._CUCKOO_SINGLE_INT_SIZE // self.bucket_size
 
     def _parse_buckets(self, d: ByteString) -> None:
         """parse bytes and set buckets"""
-        self._buckets = list()
+        self._buckets = []
         bucket_byte_size = self.bucket_size * self._CUCKOO_SINGLE_INT_SIZE
         offs = 0
         for _ in range(self.capacity):
             next_offs = offs + bucket_byte_size
             self.buckets.append(self._parse_bucket(d[offs:next_offs]))  # type: ignore
             offs = next_offs
 
@@ -465,25 +474,25 @@
             res = self._insert_fingerprint(finger, idx_1, idx_2)
             if res is not None:  # again, this *shouldn't* happen
                 msg = "The CuckooFilter failed to expand"
                 raise CuckooFilterFullError(msg)
 
     def _setup_expand(self, extra_fingerprint):
         """setup this thing"""
-        fingerprints = list()
+        fingerprints = []
         if extra_fingerprint is not None:
             fingerprints.append(extra_fingerprint)
         for idx in range(self.capacity):
             fingerprints.extend(self.buckets[idx])
 
         self._cuckoo_capacity = self.capacity * self.expansion_rate
-        self._buckets = list()
+        self._buckets = []
         self._inserted_elements = 0
         for _ in range(self.capacity):
-            self.buckets.append(list())
+            self.buckets.append([])
 
         return fingerprints
 
     def _indicies_from_fingerprint(self, fingerprint):
         """Generate the possible insertion indicies from a fingerprint
 
         Args:
@@ -512,15 +521,15 @@
     def _deal_with_insertion(self, finger):
         """some code to handle the insertion the same"""
         if finger is None:
             return
         if self.auto_expand:
             self._expand_logic(finger)
         else:
-            msg = "The {} is currently full".format(self.__class__.__name__)
+            msg = f"The {self.__class__.__name__} is currently full"
             raise CuckooFilterFullError(msg)
 
     def _calc_error_rate(self):
         """calculate error rate based on fingerprint size (bits) and bucket size"""
         return float(1 / (2 ** (self.fingerprint_size_bits - (math.log2(self.bucket_size) + 1))))
 
     def _calc_fingerprint_size(self) -> int:
```

### Comparing `pyprobables-0.5.6/probables/exceptions.py` & `pyprobables-0.5.7/probables/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyprobables-0.5.6/probables/hashes.py` & `pyprobables-0.5.7/probables/hashes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Probables Hashing Utilities """
 
 from functools import wraps
 from hashlib import md5, sha256
 from struct import unpack
 from typing import Callable, List, Union
 
-from .constants import UINT32_T_MAX, UINT64_T_MAX
+from .constants import UINT64_T_MAX
 
 KeyT = Union[str, bytes]
 SimpleHashT = Callable[[KeyT, int], int]
 HashResultsT = List[int]
 HashFuncT = Callable[[KeyT, int], HashResultsT]
 HashFuncBytesT = Callable[[KeyT, int], bytes]
 
@@ -26,15 +26,15 @@
         list(int): 64-bit hashed representation of key
     Note:
         Arguments shown are as it will be after decorated"""
 
     @wraps(func)
     def hashing_func(key, depth=1):
         """wrapper function"""
-        res = list()
+        res = []
         tmp = key if not isinstance(key, str) else key.encode("utf-8")
         for idx in range(depth):
             tmp = func(tmp, idx)
             res.append(unpack("Q", tmp[:8])[0])  # turn into 64 bit number
         return res
 
     return hashing_func
@@ -52,19 +52,19 @@
         list(int): 64-bit hashed representation of key
     Note:
         Arguments shown are as it will be after decorated"""
 
     @wraps(func)
     def hashing_func(key, depth=1):
         """wrapper function"""
-        res = list()
+        res = []
         tmp = func(key, 0)
         res.append(tmp)
         for idx in range(1, depth):
-            tmp = func("{0:x}".format(tmp), idx)
+            tmp = func(f"{tmp:x}", idx)
             res.append(tmp)
         return res
 
     return hashing_func
 
 
 def default_fnv_1a(key: KeyT, depth: int = 1) -> List[int]:
@@ -72,15 +72,15 @@
 
     Args:
         key (str): The element to be hashed
         depth (int): The number of hash permutations to compute
     Returns:
         list(int): List of size depth hashes"""
 
-    res = list()
+    res = []
     for idx in range(depth):
         res.append(fnv_1a(key, idx))
     return res
 
 
 def fnv_1a(key: KeyT, seed: int = 0) -> int:
     """Pure python implementation of the 64 bit fnv-1a hash
@@ -100,29 +100,29 @@
         hval ^= t_str
         hval *= fnv_64_prime
         hval %= max64mod
     return hval
 
 
 @hash_with_depth_bytes
-def default_md5(key: KeyT, seed: int = 0) -> bytes:
+def default_md5(key: KeyT, *args, **kwargs) -> bytes:
     """The default md5 hashing routine
 
     Args:
         key (str): The element to be hashed
         depth (int): The number of hash permutations to compute
     Returns:
         list(int): List of 64-bit hashed representation of key hashes
     Note:
         Returns the upper-most 64 bits"""
     return md5(key).digest()  # type: ignore
 
 
 @hash_with_depth_bytes
-def default_sha256(key: KeyT, seed: int = 0) -> bytes:
+def default_sha256(key: KeyT, *args, **kwargs) -> bytes:
     """The default sha256 hashing routine
 
     Args:
         key (str): The element to be hashed
         depth (int): The number of hash permutations to compute
     Returns:
         list(int): List of 64-bit hashed representation of key hashes
```

### Comparing `pyprobables-0.5.6/probables/utilities.py` & `pyprobables-0.5.7/probables/utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 def is_valid_file(filepath: Union[str, Path, None]) -> bool:
     """check if the passed filepath points to a real file"""
     if filepath is None:
         return False
     return Path(filepath).exists()
 
 
+def resolve_path(filepath: Union[str, Path]) -> Path:
+    """fully resolve the path by expanding user and resolving"""
+    return Path(filepath).expanduser().resolve()
+
+
 def get_x_bits(num: int, max_bits: int, num_bits: int, right_bits: bool = True) -> int:
     """ensure the correct number of bits and pull the upper x bits"""
     bits = bin(num).lstrip("0b")
     bits = bits.zfill(max_bits)
     if right_bits:
         return int(bits[-num_bits:], 2)
     return int(bits[:num_bits], 2)
```

### Comparing `pyprobables-0.5.6/pyprobables.egg-info/PKG-INFO` & `pyprobables-0.5.7/pyprobables.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: pyprobables
-Version: 0.5.6
+Version: 0.5.7
 Summary: Probabilistic data structures in python
-Home-page: https://github.com/barrust/pyprobables
-Author: Tyler Barrus
-Author-email: barrust@gmail.com
+Author-email: Tyler Barrus <barrust@gmail.com>
 License: MIT
-Download-URL: https://github.com/barrust/pyprobables/tarball/v0.5.6
-Keywords: python probabilistic data-structure bloom filter count-min sketch bloom-filter count-min-sketch cuckoo-filter
-Platform: UNKNOWN
+Project-URL: Homepage, https://github.com/barrust/pyprobables
+Project-URL: Bug-tracker, https://github.com/barrust/pyprobables/issues
+Project-URL: Documentation, https://pyprobables.readthedocs.io/
+Keywords: python,probabilistic,data-structure,bloom,filter,count-min,sketch,bloom-filter,count-min-sketch,cuckoo-filter
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 PyProbables
 ===========
 
 .. image:: https://img.shields.io/badge/license-MIT-blue.svg
     :target: https://opensource.org/licenses/MIT/
@@ -81,15 +82,15 @@
 To install `pyprobables`, simply clone the `repository on GitHub
 <https://github.com/barrust/pyprobables>`__, then run from the folder:
 
 ::
 
     $ python setup.py install
 
-`pyprobables` supports python 3.5 - 3.9+
+`pyprobables` supports python 3.6 - 3.10+
 
 For *python 2.7* support, install `release 0.3.2 <https://github.com/barrust/pyprobables/releases/tag/v0.3.2>`__
 
 ::
 
     $ pip install pyprobables==0.3.2
 
@@ -244,9 +245,7 @@
         for t_str in tmp:
             hval ^= t_str
             hval *= fnv_64_prime
             hval %= max64mod
         return hval
 
     blm = BloomFilter(filpath="old-file-path.blm", hash_function=old_fnv1a)
-
-
```

### Comparing `pyprobables-0.5.6/pyprobables.egg-info/SOURCES.txt` & `pyprobables-0.5.7/pyprobables.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 LICENSE
 README.rst
 pyproject.toml
-setup.cfg
-setup.py
 probables/__init__.py
 probables/constants.py
 probables/exceptions.py
 probables/hashes.py
 probables/utilities.py
 probables/blooms/__init__.py
 probables/blooms/bloom.py
@@ -16,8 +14,9 @@
 probables/countminsketch/countminsketch.py
 probables/cuckoo/__init__.py
 probables/cuckoo/countingcuckoo.py
 probables/cuckoo/cuckoo.py
 pyprobables.egg-info/PKG-INFO
 pyprobables.egg-info/SOURCES.txt
 pyprobables.egg-info/dependency_links.txt
-pyprobables.egg-info/top_level.txt
+pyprobables.egg-info/top_level.txt
+tests/test_utilities.py
```

