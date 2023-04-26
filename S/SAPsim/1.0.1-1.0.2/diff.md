# Comparing `tmp/SAPsim-1.0.1.tar.gz` & `tmp/SAPsim-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAPsim-1.0.1.tar", last modified: Tue Apr 25 11:20:59 2023, max compression
+gzip compressed data, was "SAPsim-1.0.2.tar", last modified: Wed Apr 26 02:07:09 2023, max compression
```

## Comparing `SAPsim-1.0.1.tar` & `SAPsim-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.517633 SAPsim-1.0.1/
--rw-r--r--   0 jesse      (501) staff       (20)     1066 2023-02-23 19:54:52.000000 SAPsim-1.0.1/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)     2621 2023-04-25 11:20:59.517478 SAPsim-1.0.1/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1766 2023-04-25 11:20:34.000000 SAPsim-1.0.1/README.md
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.511919 SAPsim-1.0.1/SAPsim/
--rw-r--r--   0 jesse      (501) staff       (20)      685 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.515590 SAPsim-1.0.1/SAPsim/utils/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     7470 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     5593 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/execute.py
--rw-r--r--   0 jesse      (501) staff       (20)     2110 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/globs.py
--rw-r--r--   0 jesse      (501) staff       (20)     7692 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     5936 2023-04-23 03:19:25.000000 SAPsim-1.0.1/SAPsim/utils/instructions.py
--rw-r--r--   0 jesse      (501) staff       (20)     3749 2023-04-25 11:20:18.000000 SAPsim-1.0.1/SAPsim/utils/parser.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.512779 SAPsim-1.0.1/SAPsim.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)     2621 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)      521 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       20 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)       13 2023-04-25 11:20:59.000000 SAPsim-1.0.1/SAPsim.egg-info/top_level.txt
--rw-r--r--   0 jesse      (501) staff       (20)      903 2023-04-25 11:20:18.000000 SAPsim-1.0.1/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-04-25 11:20:59.517676 SAPsim-1.0.1/setup.cfg
--rw-r--r--   0 jesse      (501) staff       (20)     1393 2023-04-25 11:20:18.000000 SAPsim-1.0.1/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-04-25 11:20:59.517136 SAPsim-1.0.1/tests/
--rw-r--r--   0 jesse      (501) staff       (20)      121 2023-02-23 20:02:21.000000 SAPsim-1.0.1/tests/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     3029 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_example_progs.py
--rw-r--r--   0 jesse      (501) staff       (20)      524 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_exceptions.py
--rw-r--r--   0 jesse      (501) staff       (20)     1389 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_helpers.py
--rw-r--r--   0 jesse      (501) staff       (20)     4765 2023-04-23 03:19:25.000000 SAPsim-1.0.1/tests/test_instructions.py
--rw-r--r--   0 jesse      (501) staff       (20)     2620 2023-04-25 11:20:18.000000 SAPsim-1.0.1/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 02:07:00.000000 SAPsim-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 02:07:09.522108 SAPsim-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-26 02:07:00.000000 SAPsim-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 02:07:00.000000 SAPsim-1.0.2/SAPsim/utils/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/SAPsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 02:07:09.000000 SAPsim-1.0.2/SAPsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 02:07:00.000000 SAPsim-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 02:07:09.522108 SAPsim-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-26 02:07:00.000000 SAPsim-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 02:07:09.522108 SAPsim-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_example_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-26 02:07:00.000000 SAPsim-1.0.2/tests/test_run.py
```

### Comparing `SAPsim-1.0.1/LICENSE` & `SAPsim-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/PKG-INFO` & `SAPsim-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -16,19 +16,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SAPsim
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/test.yml/badge.svg)
+![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
+> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+
+<p align="center">
+    <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
+</p>
 
 ## Install
 
 Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
 
 Next, install SAPsim.
 
@@ -38,29 +42,29 @@
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
-Now, open a Python terminal or file. You'll pass the path to your SAP program as an argument.
+Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
 from SAPsim import run
+
 run("path/to/your/SAP/program.csv")                 # run at full speed (default)
 run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
 ```
 
-Additional settings are described [here](https://SAPsim.readthedocs.io/en/latest/#settings).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easiest to just mimic the example programs [above](#usage).
-
-But if you need it, the list of rules for SAP programs is [here](https://SAPsim.readthedocs.io/en/latest/rules.html).
+It's easy to just mimic the example programs [above](#usage).
+But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.1/README.md` & `SAPsim-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # SAPsim
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/test.yml/badge.svg)
+![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
+> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+
+<p align="center">
+    <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
+</p>
 
 ## Install
 
 Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
 
 Next, install SAPsim.
 
@@ -18,29 +22,29 @@
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
-Now, open a Python terminal or file. You'll pass the path to your SAP program as an argument.
+Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
 from SAPsim import run
+
 run("path/to/your/SAP/program.csv")                 # run at full speed (default)
 run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
 ```
 
-Additional settings are described [here](https://SAPsim.readthedocs.io/en/latest/#settings).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easiest to just mimic the example programs [above](#usage).
-
-But if you need it, the list of rules for SAP programs is [here](https://SAPsim.readthedocs.io/en/latest/rules.html).
+It's easy to just mimic the example programs [above](#usage).
+But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.1/SAPsim/__init__.py` & `SAPsim-1.0.2/SAPsim/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 from typing import Any
 from SAPsim.utils.helpers import is_documented_by
 import SAPsim.utils.execute as execute
 
 
 # Weird glitch, passing in the function doesn't actually get its docstring? Just append then
-@is_documented_by(execute.run, 0, execute.run.__doc__)
+@is_documented_by(execute.run, 0, "", execute.run.__doc__)
 def run(prog_path: str, **kwargs) -> None:
     execute.run(prog_path, **kwargs)
 
 
 # Weird glitch, passing in the function doesn't actually get its docstring? Just append then
-@is_documented_by(execute.run_and_return_state, 0, execute.run.__doc__)
+@is_documented_by(
+    execute.run_and_return_state, 0, "", execute.run_and_return_state.__doc__
+)
 def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
     return execute.run_and_return_state(prog_path, **kwargs)
```

### Comparing `SAPsim-1.0.1/SAPsim/utils/exceptions.py` & `SAPsim-1.0.2/SAPsim/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/SAPsim/utils/execute.py` & `SAPsim-1.0.2/SAPsim/utils/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
         helpers.print_info()
         print("Program halted.")
 
 
 @is_documented_by(
     run,
     2,
+    "",
     r"""
     :return: ``dict`` containing program state (see ``helpers.get_state``)
     :rtype: ``dict[str, Any]``
     """,
 )
 def run_and_return_state(prog_path: str, **kwargs) -> dict[str, Any]:
     run(prog_path, **kwargs)
```

### Comparing `SAPsim-1.0.1/SAPsim/utils/globs.py` & `SAPsim-1.0.2/SAPsim/utils/globs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/SAPsim/utils/helpers.py` & `SAPsim-1.0.2/SAPsim/utils/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,40 @@
 
 from tabulate import tabulate
 from typing import Any
 import SAPsim.utils.globs as globs
 import SAPsim.utils.exceptions as exceptions
 
 
+def is_documented_by(
+    original, lines_to_remove: int = 0, prepend: str = "", append: str = ""
+):
+    r"""Use for wrapper functions that should have the original function's docstring.
+
+    :param original: The original function
+    :param lines_to_remove: How many lines to remove from the end of the docstring (i.e., to remove old return)
+    :type lines_to_remove: ``int``
+    :param preprend: What to prepend to docstring. Pass in a docstring (i.e., triple quotation marks), and there should be a trailing newline
+    :type prepend: ``str``
+    :param append: What to append to docstring. Pass in a docstring (i.e., triple quotation marks), and there should be a leading newline
+    :type append: ``str``"""
+
+    def wrapper(target):
+        original_doc = original.__doc__.rstrip("\n")
+        target.__doc__ = "\n".join(original_doc.split("\n")[:-lines_to_remove])
+        # append_with_newline = append
+        # if append_with_newline and append_with_newline[0] != "\n":
+        #     append_with_newline = "\n" + append_with_newline
+        target.__doc__ = f"{prepend}{target.__doc__}"
+        target.__doc__ += f"{append}"
+        return target
+
+    return wrapper
+
+
 def parse_byte(byte: int):
     """Given a byte (2 hexits), return the opcode (1 hexit) and arg (1 hexit). Return as dict for readability.
 
     :param byte:
     :type byte: int
     :return: {'opcode': opcode, 'arg': arg}
     :rtype: dict[str, int]"""
@@ -62,16 +88,23 @@
     ):
         raise exceptions.InvalidInstructionString(instruction)
     return (globs.MNEMONIC_TO_OPCODE[instruction[:space_position].upper()] << 4) | int(
         instruction[space_position + 1 :]
     )
 
 
+@is_documented_by(
+    instruction_to_byte,
+    0,
+    ""
+    r"""
+                  Alias for ``instruction_to_byte()``.
+                  """,
+)
 def i2b(instruction: str) -> int:
-    """Alias for ``instruction_to_byte()``."""
     return instruction_to_byte(instruction)
 
 
 def print_RAM(**kwargs):
     """Pretty print the contents of RAM, sorted by address. | <PC (optional)> | Addr | Instruction | Dec | Hex | (since we can't distinguish instructions from data). Display arrow on current PC value if ``dispPC=True`` in kwargs. Set ``format=`` to set tabulate pretty-print format."""
     table = []
     for addr in sorted(globs.RAM.keys()):
@@ -204,28 +237,7 @@
         assert kwargs["B"] == globs.B
     if "FLAG_C" in kwargs:
         assert kwargs["FLAG_C"] == globs.FLAG_C
     if "FLAG_Z" in kwargs:
         assert kwargs["FLAG_Z"] == globs.FLAG_Z
     if "EXECUTING" in kwargs:
         assert kwargs["EXECUTING"] == globs.EXECUTING
-
-
-def is_documented_by(original, lines_to_remove: int = 0, append: str = ""):
-    r"""Use for wrapper functions that should have the original function's docstring.
-
-    :param original: The original function
-    :param lines_to_remove: How many lines to remove from the end of the docstring (i.e., to remove old return)
-    :type lines_to_remove: ``int``
-    :param append: What to append to docstring. Pass in a docstring (i.e., triple quotation marks), and there should be a leading newline
-    :type append: ``str``"""
-
-    def wrapper(target):
-        original_doc = original.__doc__.rstrip("\n")
-        target.__doc__ = "\n".join(original_doc.split("\n")[:-lines_to_remove])
-        # append_with_newline = append
-        # if append_with_newline and append_with_newline[0] != "\n":
-        #     append_with_newline = "\n" + append_with_newline
-        target.__doc__ += f"{append}"
-        return target
-
-    return wrapper
```

### Comparing `SAPsim-1.0.1/SAPsim/utils/instructions.py` & `SAPsim-1.0.2/SAPsim/utils/instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/SAPsim/utils/parser.py` & `SAPsim-1.0.2/SAPsim/utils/parser.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/SAPsim.egg-info/PKG-INFO` & `SAPsim-1.0.2/SAPsim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SAPsim
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC
 Home-page: https://github.com/jesse-wei/SAPsim
 Download-URL: https://github.com/jesse-wei/SAPsim/releases
 Author: Jesse Wei
 Author-email: Jesse Wei <jesse@cs.unc.edu>
 Project-URL: Homepage, https://github.com/jesse-wei/SAPsim
 Project-URL: Bug Tracker, https://github.com/jesse-wei/SAPsim/issues
@@ -16,19 +16,23 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SAPsim
 
-![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/test.yml/badge.svg)
+![Test badge](https://github.com/jesse-wei/SAPsim/actions/workflows/tests.yml/badge.svg)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
 ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54)
 
-> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu)
+> Simulation of [SAP (Simple As Possible) computer](https://jessewei.dev/img/sap.jpg) programs from COMP311 (Computer Organization) @ [UNC](https://unc.edu).
+
+<p align="center">
+    <img src="https://jessewei.dev/img/SAPsim_demo.gif" alt="SAPsim demo">
+</p>
 
 ## Install
 
 Your Python version needs to be 3.9+. Check with `python --version` or `python3 --version`, if `python` doesn't work.
 
 Next, install SAPsim.
 
@@ -38,29 +42,29 @@
 
 If `pip` doesn't work, try `pip3`.
 
 ## Usage
 
 Write a SAP program in the format shown in [ex2.csv](https://github.com/jesse-wei/SAPsim/blob/main/tests/public_prog/ex2.csv). See [template.csv](https://github.com/jesse-wei/SAPsim/blob/main/template.csv) for a blank template. You may edit the `.csv` files in Microsoft Excel.
 
-Now, open a Python terminal or file. You'll pass the path to your SAP program as an argument.
+Open a Python terminal. You'll pass the path to your SAP program as an argument.
 
 ```py
 from SAPsim import run
+
 run("path/to/your/SAP/program.csv")                 # run at full speed (default)
 run("path/to/your/SAP/program.csv", debug=True)     # run in debug (step) mode
 ```
 
-Additional settings are described [here](https://SAPsim.readthedocs.io/en/latest/#settings).
+Here's a list of [additional settings](https://SAPsim.readthedocs.io/en/latest/#settings) (e.g., table format).
 
 ## Rules
 
-It's easiest to just mimic the example programs [above](#usage).
-
-But if you need it, the list of rules for SAP programs is [here](https://SAPsim.readthedocs.io/en/latest/rules.html).
+It's easy to just mimic the example programs [above](#usage).
+But if you need it, here's the list of [rules for SAPsim programs](https://SAPsim.readthedocs.io/en/latest/rules.html).
 
 ## SAP instruction set
 
 ![SAP instruction set](https://user-images.githubusercontent.com/55986131/220041985-da3060d2-18c3-4158-8d30-a5d88e08acc4.png)
 
 ## Documentation
```

### Comparing `SAPsim-1.0.1/SAPsim.egg-info/SOURCES.txt` & `SAPsim-1.0.2/SAPsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/pyproject.toml` & `SAPsim-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/setup.py` & `SAPsim-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 ]
 """All required (i.e., for functionality) dependencies that are installed when running `pip install SAPsim`.
 
 Non-functional (e.g., formatting, documentation) dependencies listed in requirements.txt."""
 
 setup(
     name="SAPsim",
-    # Version number that appears on PyPI and Test PyPI
-    version="1.0.1",
-    description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC",
+    version="1.0.2",
+    description="Simulation of SAP (Simple As Possible) computer programs from COMP311 (Computer Organization) @ UNC.",
     author="Jesse Wei",
     author_email="jesse@cs.unc.edu",
     url="https://github.com/jesse-wei/SAPsim",
     download_url="https://github.com/jesse-wei/SAPsim/releases",
     keywords=[
         "SAP",
         "SAPsim",
```

### Comparing `SAPsim-1.0.1/tests/test_example_progs.py` & `SAPsim-1.0.2/tests/test_example_progs.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/tests/test_exceptions.py` & `SAPsim-1.0.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/tests/test_helpers.py` & `SAPsim-1.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/tests/test_instructions.py` & `SAPsim-1.0.2/tests/test_instructions.py`

 * *Files identical despite different names*

### Comparing `SAPsim-1.0.1/tests/test_run.py` & `SAPsim-1.0.2/tests/test_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Test the run function in SAPsim.__init__.py
+"""Test the run function in SAPsim.__init__.py.
+
+Ideally, would like to test run(..., debug=True) but can't really send keyboard input, might require threading.
 
 Remove the TEMP_FILE_PATH in the final test."""
 
 __author__ = "Jesse Wei <jesse@cs.unc.edu>"
 
 import sys
 import os
```

