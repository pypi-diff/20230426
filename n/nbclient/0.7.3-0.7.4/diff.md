# Comparing `tmp/nbclient-0.7.3.tar.gz` & `tmp/nbclient-0.7.4.tar.gz`

## Comparing `nbclient-0.7.3.tar` & `nbclient-0.7.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/__init__.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/_version.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/cli.py
--rw-r--r--   0        0        0    49504 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/client.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/exceptions.py
--rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/jsonutil.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/output_widget.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/py.typed
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/__init__.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/base.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/conftest.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0    70296 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/test_client.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/test_util.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Autokill.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Check History in Memory.ipynb
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Clear Output.ipynb
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Disable Stdin.ipynb
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Empty Cell.ipynb
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Error.ipynb
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Factorials.ipynb
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Inline Image.ipynb
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Interrupt.ipynb
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/JupyterWidgets.ipynb
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Other Comms.ipynb
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Output.ipynb
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Parallel Execute A.ipynb
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Parallel Execute B.ipynb
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/SVG.ipynb
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Skip Exceptions.ipynb
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Skip Execution with Cell Tag.ipynb
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Sleep1s.ipynb
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/Unicode.ipynb
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/UnicodePy3.ipynb
--rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/python.png
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 nbclient-0.7.3/nbclient/tests/files/update-display-id.ipynb
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 nbclient-0.7.3/.gitignore
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nbclient-0.7.3/LICENSE
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nbclient-0.7.3/README.md
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 nbclient-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     7981 2020-02-02 00:00:00.000000 nbclient-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/__init__.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/_version.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/cli.py
+-rw-r--r--   0        0        0    49505 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/client.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/exceptions.py
+-rw-r--r--   0        0        0     4541 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/jsonutil.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/output_widget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/py.typed
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/__init__.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/base.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/conftest.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0    71162 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/test_client.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/test_util.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Autokill.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Check History in Memory.ipynb
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Clear Output.ipynb
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Disable Stdin.ipynb
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Empty Cell.ipynb
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Error.ipynb
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Factorials.ipynb
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0    14333 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Inline Image.ipynb
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Interrupt.ipynb
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/JupyterWidgets.ipynb
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Other Comms.ipynb
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Output.ipynb
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Parallel Execute A.ipynb
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Parallel Execute B.ipynb
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/SVG.ipynb
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Exceptions with Cell Tags.ipynb
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Exceptions.ipynb
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Skip Execution with Cell Tag.ipynb
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Sleep1s.ipynb
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/Unicode.ipynb
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/UnicodePy3.ipynb
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/python.png
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 nbclient-0.7.4/nbclient/tests/files/update-display-id.ipynb
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 nbclient-0.7.4/.gitignore
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 nbclient-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 nbclient-0.7.4/README.md
+-rw-r--r--   0        0        0     5133 2020-02-02 00:00:00.000000 nbclient-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 nbclient-0.7.4/PKG-INFO
```

### Comparing `nbclient-0.7.3/nbclient/cli.py` & `nbclient-0.7.4/nbclient/cli.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/client.py` & `nbclient-0.7.4/nbclient/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1013,15 +1013,14 @@
                 raise
 
         if execution_count:
             cell['execution_count'] = execution_count
         await run_hook(
             self.on_cell_executed, cell=cell, cell_index=cell_index, execute_reply=exec_reply
         )
-        await self._check_raise_for_error(cell, cell_index, exec_reply)
 
         if self.coalesce_streams and cell.outputs:
             new_outputs = []
             streams: dict[str, NotebookNode] = {}
             for output in cell.outputs:
                 if output["output_type"] == "stream":
                     if output["name"] in streams:
@@ -1052,14 +1051,16 @@
                         and new_outputs[i + 1]["name"] == "stdout"
                     ):
                         stdout = new_outputs.pop(i + 1)
                         new_outputs.insert(i, stdout)
 
             cell.outputs = new_outputs
 
+        await self._check_raise_for_error(cell, cell_index, exec_reply)
+
         self.nb['cells'][cell_index] = cell
         return cell
 
     execute_cell = run_sync(async_execute_cell)
 
     def process_message(
         self, msg: t.Dict, cell: NotebookNode, cell_index: int
```

### Comparing `nbclient-0.7.3/nbclient/jsonutil.py` & `nbclient-0.7.4/nbclient/jsonutil.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/output_widget.py` & `nbclient-0.7.4/nbclient/output_widget.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/base.py` & `nbclient-0.7.4/nbclient/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/fake_kernelmanager.py` & `nbclient-0.7.4/nbclient/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/test_client.py` & `nbclient-0.7.4/nbclient/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import concurrent.futures
 import copy
 import datetime
 import functools
 import os
 import re
+import sys
 import threading
 import warnings
 from base64 import b64decode, b64encode
 from queue import Empty
 from typing import Any
 from unittest.mock import MagicMock, Mock
 
@@ -319,15 +320,15 @@
         ("Factorials.ipynb", {"kernel_name": "python"}),
         ("HelloWorld.ipynb", {"kernel_name": "python"}),
         ("Inline Image.ipynb", {"kernel_name": "python"}),
         (
             "Interrupt.ipynb",
             {
                 "kernel_name": "python",
-                "timeout": 1,
+                "timeout": 3,
                 "interrupt_on_timeout": True,
                 "allow_errors": True,
             },
         ),
         ("JupyterWidgets.ipynb", {"kernel_name": "python"}),
         ("Skip Exceptions with Cell Tags.ipynb", {"kernel_name": "python"}),
         ("Skip Exceptions.ipynb", {"kernel_name": "python", "allow_errors": True}),
@@ -704,29 +705,49 @@
         Check that conversion halts if ``allow_errors`` is False.
         """
         filename = os.path.join(current_dir, 'files', 'Skip Exceptions.ipynb')
         res = self.build_resources()
         res['metadata']['path'] = os.path.dirname(filename)
         with pytest.raises(CellExecutionError) as exc:
             run_notebook(filename, {"allow_errors": False}, res)
-            self.assertIsInstance(str(exc.value), str)
-            assert "# üñîçø∂é" in str(exc.value)
+
+        assert isinstance(str(exc.value), str)
+        exc_str = strip_ansi(str(exc.value))
+        # FIXME: we seem to have an encoding problem on Windows
+        # same check in force_raise_errors
+        if not sys.platform.startswith("win"):
+            assert "# üñîçø∂é" in exc_str
 
     def test_force_raise_errors(self):
         """
         Check that conversion halts if the ``force_raise_errors`` traitlet on
         NotebookClient is set to True.
         """
         filename = os.path.join(current_dir, 'files', 'Skip Exceptions with Cell Tags.ipynb')
         res = self.build_resources()
         res['metadata']['path'] = os.path.dirname(filename)
         with pytest.raises(CellExecutionError) as exc:
             run_notebook(filename, {"force_raise_errors": True}, res)
-            self.assertIsInstance(str(exc.value), str)
-            assert "# üñîçø∂é" in str(exc.value)
+
+        # verify CellExecutionError contents
+        exc_str = strip_ansi(str(exc.value))
+        # print for better debugging with captured output
+        # print(exc_str)
+        assert "Exception: message" in exc_str
+        # FIXME: unicode handling seems to have a problem on Windows
+        # same check in allow_errors
+        if not sys.platform.startswith("win"):
+            assert "# üñîçø∂é" in exc_str
+        assert "stderr" in exc_str
+        assert "stdout" in exc_str
+        assert "hello\n" in exc_str
+        assert "errorred\n" in exc_str
+        # stricter check for stream output format
+        assert "\n".join(["", "----- stdout -----", "hello", "---"]) in exc_str
+        assert "\n".join(["", "----- stderr -----", "errorred", "---"]) in exc_str
 
     def test_reset_kernel_client(self):
         filename = os.path.join(current_dir, 'files', 'HelloWorld.ipynb')
 
         with open(filename) as f:
             input_nb = nbformat.read(f, 4)
```

### Comparing `nbclient-0.7.3/nbclient/tests/test_util.py` & `nbclient-0.7.4/nbclient/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Autokill.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Autokill.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Clear Output.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Clear Output.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Empty Cell.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Empty Cell.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Error.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Error.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Factorials.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Factorials.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Inline Image.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Inline Image.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Interrupt.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Interrupt.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/JupyterWidgets.ipynb` & `nbclient-0.7.4/nbclient/tests/files/JupyterWidgets.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Other Comms.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Other Comms.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Output.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Output.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Parallel Execute A.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Parallel Execute A.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Parallel Execute B.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Parallel Execute B.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/SVG.ipynb` & `nbclient-0.7.4/nbclient/tests/files/SVG.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Skip Exceptions.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Skip Exceptions.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/Sleep1s.ipynb` & `nbclient-0.7.4/nbclient/tests/files/Sleep1s.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/python.png` & `nbclient-0.7.4/nbclient/tests/files/python.png`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/nbclient/tests/files/update-display-id.ipynb` & `nbclient-0.7.4/nbclient/tests/files/update-display-id.ipynb`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/.gitignore` & `nbclient-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/LICENSE` & `nbclient-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nbclient-0.7.3/README.md` & `nbclient-0.7.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter/nbclient/main?filepath=binder%2Frun_nbclient.ipynb)
 [![Build Status](https://github.com/jupyter/nbclient/workflows/CI/badge.svg)](https://github.com/jupyter/nbclient/actions)
 [![Documentation Status](https://readthedocs.org/projects/nbclient/badge/?version=latest)](https://nbclient.readthedocs.io/en/latest/?badge=latest)
-[![CodeCov](https://codecov.io/gh/jupyter/nbclient/coverage.svg?branch=main)](https://codecov.io/gh/jupyter/nbclient?branch=main)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

### Comparing `nbclient-0.7.3/pyproject.toml` & `nbclient-0.7.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 features = ["test"]
 [tool.hatch.envs.test.scripts]
 test = "python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.cov]
 features = ["test"]
-dependencies = ["coverage", "pytest-cov"]
+dependencies = ["coverage[toml]", "pytest-cov"]
 [tool.hatch.envs.cov.scripts]
 test = "python -m pytest -vv --cov nbclient --cov-branch --cov-report term-missing:skip-covered {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.typing]
 features = ["test"]
 dependencies = ["mypy>=0.990"]
@@ -152,14 +152,18 @@
   "raise NotImplementedError",
   "if 0:",
   "if __name__ == .__main__.:",
   "class .*\bProtocol\\):",
 "@(abc\\.)?abstractmethod",
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["nbclient"]
+
 [tool.mypy]
 python_version = 3.9
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
```

### Comparing `nbclient-0.7.3/PKG-INFO` & `nbclient-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbclient
-Version: 0.7.3
+Version: 0.7.4
 Summary: A client library for executing notebooks. Formerly nbconvert's ExecutePreprocessor.
 Project-URL: Documentation, https://nbclient.readthedocs.io
 Project-URL: Funding, https://numfocus.org/
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Source, https://github.com/jupyter/nbclient
 Project-URL: Tracker, https://github.com/jupyter/nbclient/issues
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
@@ -79,15 +79,14 @@
 Requires-Dist: testpath; extra == 'test'
 Requires-Dist: xmltodict; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter/nbclient/main?filepath=binder%2Frun_nbclient.ipynb)
 [![Build Status](https://github.com/jupyter/nbclient/workflows/CI/badge.svg)](https://github.com/jupyter/nbclient/actions)
 [![Documentation Status](https://readthedocs.org/projects/nbclient/badge/?version=latest)](https://nbclient.readthedocs.io/en/latest/?badge=latest)
-[![CodeCov](https://codecov.io/gh/jupyter/nbclient/coverage.svg?branch=main)](https://codecov.io/gh/jupyter/nbclient?branch=main)
 [![Python 3.7](https://img.shields.io/badge/python-3.7-blue.svg)](https://www.python.org/downloads/release/python-370/)
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/downloads/release/python-3110/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

