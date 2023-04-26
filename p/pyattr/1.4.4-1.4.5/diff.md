# Comparing `tmp/pyattr-1.4.4.tar.gz` & `tmp/pyattr-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyattr-1.4.4.tar", last modified: Sun Feb 19 15:09:18 2023, max compression
+gzip compressed data, was "pyattr-1.4.5.tar", last modified: Tue Apr 25 15:49:11 2023, max compression
```

## Comparing `pyattr-1.4.4.tar` & `pyattr-1.4.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 15:09:18.470929 pyattr-1.4.4/
--rw-rw-rw-   0        0        0     1084 2023-02-18 14:11:46.000000 pyattr-1.4.4/LICENSE
--rw-rw-rw-   0        0        0     3966 2023-02-19 15:09:18.467928 pyattr-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     3301 2023-02-19 15:07:55.000000 pyattr-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-02-19 15:09:18.450978 pyattr-1.4.4/pyattr/
--rw-rw-rw-   0        0        0     4064 2023-02-19 14:59:10.000000 pyattr-1.4.4/pyattr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-19 15:09:18.463925 pyattr-1.4.4/pyattr.egg-info/
--rw-rw-rw-   0        0        0     3966 2023-02-19 15:09:18.000000 pyattr-1.4.4/pyattr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-02-19 15:09:18.000000 pyattr-1.4.4/pyattr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 15:09:18.000000 pyattr-1.4.4/pyattr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-02-19 15:09:18.000000 pyattr-1.4.4/pyattr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 15:09:18.471932 pyattr-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      926 2023-02-19 08:09:56.000000 pyattr-1.4.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-25 15:49:11.694640 pyattr-1.4.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1063 2023-04-25 15:44:29.000000 pyattr-1.4.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3674 2023-04-25 15:49:11.694640 pyattr-1.4.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3027 2023-04-25 15:47:33.000000 pyattr-1.4.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-25 15:49:11.694640 pyattr-1.4.5/pyattr/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3941 2023-04-25 15:47:39.000000 pyattr-1.4.5/pyattr/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-25 15:49:11.694640 pyattr-1.4.5/pyattr.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3674 2023-04-25 15:49:11.000000 pyattr-1.4.5/pyattr.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      165 2023-04-25 15:49:11.000000 pyattr-1.4.5/pyattr.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-25 15:49:11.000000 pyattr-1.4.5/pyattr.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        7 2023-04-25 15:49:11.000000 pyattr-1.4.5/pyattr.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-25 15:49:11.694640 pyattr-1.4.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      897 2023-04-25 15:44:29.000000 pyattr-1.4.5/setup.py
```

### Comparing `pyattr-1.4.4/LICENSE` & `pyattr-1.4.5/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 skifli
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 skifli
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyattr-1.4.4/PKG-INFO` & `pyattr-1.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,90 @@
-Metadata-Version: 2.1
-Name: pyattr
-Version: 1.4.4
-Summary: Proper access modifiers for Python classes.
-Home-page: https://github.com/skifli/pyattr
-Author: skifli
-License: MIT
-Project-URL: Documentation, https://github.com/skifli/pyattr#example
-Project-URL: Source, https://github.com/skifli/pyattr
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyattr
-
-[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
-![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
-
-- [pyattr](#pyattr)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Example](#example)
-  - [How it works](#how-it-works)
-  - [Benchmarks](#benchmarks)
-
-While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
-
-## Installation
-
-Installation via **pip**:
-
-```
-pip install pyattr
-```
-
-## Usage
-
-All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
-
-## Example
-
-Here is a simple example involving a *private* variable.
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-        self.__name = "pyattr"
-
-example = Example()
-print(example.__name) # Error - '__name' is a private attribute of 'Example'.
-```
-
-As well as variables, **pyattr** also supports access control of *functions*!
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __example(self) -> None:
-        pass
-
-
-example = Example()
-print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
-```
-
-## How it works
-
-> **Note** For a more in-depth explanation on how **pyattr** works, see my [blog post](https://skifli.github.io/blog/2023/pyattr_in_depth_explanation.html#how-does-pyattr-work#how-does-pyattr-work).
-
-**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
-
-The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`inspect.stack()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
-
-## Benchmarks
-
-The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
-
-[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
+Metadata-Version: 2.1
+Name: pyattr
+Version: 1.4.5
+Summary: Proper access modifiers for Python classes.
+Home-page: https://github.com/skifli/pyattr
+Author: skifli
+License: MIT
+Project-URL: Documentation, https://github.com/skifli/pyattr#example
+Project-URL: Source, https://github.com/skifli/pyattr
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyattr
+
+[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
+![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
+
+- [pyattr](#pyattr)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Example](#example)
+  - [How it works](#how-it-works)
+  - [Benchmarks](#benchmarks)
+
+While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
+
+## Installation
+
+Installation via **pip**:
+
+```
+pip install pyattr
+```
+
+## Usage
+
+All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
+
+## Example
+
+Here is a simple example involving a *private* variable.
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.__name = "pyattr"
+
+example = Example()
+print(example.__name) # Error - '__name' is a private attribute of 'Example'.
+```
+
+As well as variables, **pyattr** also supports access control of *functions*!
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __example(self) -> None:
+        pass
+
+
+example = Example()
+print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
+```
+
+## How it works
+
+**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
+
+The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`sys._getframe()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
+
+## Benchmarks
+
+The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
+
+[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
```

### Comparing `pyattr-1.4.4/README.md` & `pyattr-1.4.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-# pyattr
-
-[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
-![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
-
-- [pyattr](#pyattr)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Example](#example)
-  - [How it works](#how-it-works)
-  - [Benchmarks](#benchmarks)
-
-While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
-
-## Installation
-
-Installation via **pip**:
-
-```
-pip install pyattr
-```
-
-## Usage
-
-All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
-
-## Example
-
-Here is a simple example involving a *private* variable.
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-        self.__name = "pyattr"
-
-example = Example()
-print(example.__name) # Error - '__name' is a private attribute of 'Example'.
-```
-
-As well as variables, **pyattr** also supports access control of *functions*!
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __example(self) -> None:
-        pass
-
-
-example = Example()
-print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
-```
-
-## How it works
-
-> **Note** For a more in-depth explanation on how **pyattr** works, see my [blog post](https://skifli.github.io/blog/2023/pyattr_in_depth_explanation.html#how-does-pyattr-work#how-does-pyattr-work).
-
-**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
-
-The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`inspect.stack()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
-
-## Benchmarks
-
-The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
-
-[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
+# pyattr
+
+[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
+![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
+
+- [pyattr](#pyattr)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Example](#example)
+  - [How it works](#how-it-works)
+  - [Benchmarks](#benchmarks)
+
+While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
+
+## Installation
+
+Installation via **pip**:
+
+```
+pip install pyattr
+```
+
+## Usage
+
+All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
+
+## Example
+
+Here is a simple example involving a *private* variable.
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.__name = "pyattr"
+
+example = Example()
+print(example.__name) # Error - '__name' is a private attribute of 'Example'.
+```
+
+As well as variables, **pyattr** also supports access control of *functions*!
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __example(self) -> None:
+        pass
+
+
+example = Example()
+print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
+```
+
+## How it works
+
+**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
+
+The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`sys._getframe()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
+
+## Benchmarks
+
+The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
+
+[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
```

### Comparing `pyattr-1.4.4/pyattr/__init__.py` & `pyattr-1.4.5/pyattr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-"""
-Copyright skifli under the MIT license. ALl rights reserved.
-See '../LICENSE' for license information.
-SPDX-License-Identifier: MIT License.
-"""
-
-from types import FrameType, TracebackType
-from sys import _getframe
-from typing import Any, final
-
-__version__ = "1.4.4"
-
-
-def _pyattr_stack() -> list[FrameType]:
-    frame = _getframe().f_back
-    frames = []
-
-    while frame:
-        frames.append(frame)
-        frame = frame.f_back
-
-    return frames
-
-
-class PyattrError(Exception):
-    pass
-
-
-class _PyattrDict(dict):
-    @final
-    def __pyattr_check(self, __key: str, class_object: object, i: int = 3) -> str:
-        caller = _pyattr_stack()[i].f_locals
-
-        if "self" in caller:
-            caller_class = caller["self"].__class__.__name__
-
-            if __key.startswith(f"_{caller_class}"):
-                __key = __key.removeprefix(f"_{caller_class}")
-
-        try:
-            if __key.startswith("__"):
-                if "self" in caller:
-                    if caller["self"].__class__ != class_object:
-                        raise AttributeError(
-                            f"Attribute '{__key}' of '{class_object.__name__}' object is private."
-                        )
-                else:
-                    raise AttributeError(
-                        f"Attribute '{__key}' of '{class_object.__name__}' object is private."
-                    )
-            elif __key.startswith("_"):
-                if "self" in caller:
-                    if class_object not in caller["self"].__class__.__mro__:
-                        raise AttributeError(
-                            f"Attribute '{__key}' of '{class_object.__name__}' object is protected."
-                        )
-                else:
-                    raise AttributeError(
-                        f"Attribute '{__key}' of '{class_object.__name__}' object is protected."
-                    )
-        except AttributeError as e:
-            last_frame = _pyattr_stack()[3]
-
-            raise AttributeError(*e.args, name=e.name, obj=e.obj).with_traceback(
-                TracebackType(
-                    tb_next=None,
-                    tb_frame=last_frame,
-                    tb_lasti=last_frame.f_lasti,
-                    tb_lineno=last_frame.f_lineno,
-                )
-            )
-
-        return __key
-
-    @final
-    def __getitem__(self, __key: str, class_object: object) -> Any:
-        return super().__getitem__(self.__pyattr_check(__key, class_object))
-
-    @final
-    def __setitem__(self, __key: str, __value: str, class_object: object) -> None:
-        super().__setitem__(self.__pyattr_check(__key, class_object), __value)
-
-
-class Pyattr(_PyattrDict):
-    def __init__(self, **kwargs) -> None:
-        object.__setattr__(
-            self, "pyattr_class_object", _pyattr_stack()[1].f_locals["__class__"]
-        )
-
-        super().update(kwargs)
-
-    @final
-    def pyattr_get_class_object(self) -> object:
-        try:
-            return object.__getattribute__(self, "pyattr_class_object")
-        except AttributeError:
-            last_frame = _pyattr_stack()[2]
-
-            raise PyattrError(
-                "Did you forget to add 'super().__init__()' at the start of the '__init__' function of your class?"
-            ).with_traceback(
-                TracebackType(
-                    tb_next=None,
-                    tb_frame=last_frame,
-                    tb_lasti=last_frame.f_lasti,
-                    tb_lineno=last_frame.f_lineno,
-                )
-            )
-
-    @final
-    def __getattribute__(self, __name: str) -> Any:
-        try:
-            obj = object.__getattribute__(self, __name)
-
-            return obj
-        except AttributeError:
-            pass
-
-        return super().__getitem__(__name, self.pyattr_get_class_object())
-
-    @final
-    def __setattr__(self, __name: str, __value: Any) -> None:
-        return super().__setitem__(__name, __value, self.pyattr_get_class_object())
+"""
+Copyright skifli under the MIT license. ALl rights reserved.
+See '../LICENSE' for license information.
+SPDX-License-Identifier: MIT License.
+"""
+
+from types import FrameType, TracebackType
+from sys import _getframe
+from typing import Any, final
+
+__version__ = "1.4.5"
+
+
+def _pyattr_stack() -> list[FrameType]:
+    frame = _getframe().f_back
+    frames = []
+
+    while frame:
+        frames.append(frame)
+        frame = frame.f_back
+
+    return frames
+
+
+class PyattrError(Exception):
+    pass
+
+
+class _PyattrDict(dict):
+    @final
+    def __pyattr_check(self, __key: str, class_object: object, i: int = 3) -> str:
+        caller = _pyattr_stack()[i].f_locals
+
+        if "self" in caller:
+            caller_class = caller["self"].__class__.__name__
+
+            if __key.startswith(f"_{caller_class}"):
+                __key = __key.removeprefix(f"_{caller_class}")
+
+        try:
+            if __key.startswith("__"):
+                if "self" in caller:
+                    if caller["self"].__class__ != class_object:
+                        raise AttributeError(
+                            f"Attribute '{__key}' of '{class_object.__name__}' object is private."
+                        )
+                else:
+                    raise AttributeError(
+                        f"Attribute '{__key}' of '{class_object.__name__}' object is private."
+                    )
+            elif __key.startswith("_"):
+                if "self" in caller:
+                    if class_object not in caller["self"].__class__.__mro__:
+                        raise AttributeError(
+                            f"Attribute '{__key}' of '{class_object.__name__}' object is protected."
+                        )
+                else:
+                    raise AttributeError(
+                        f"Attribute '{__key}' of '{class_object.__name__}' object is protected."
+                    )
+        except AttributeError as e:
+            last_frame = _pyattr_stack()[3]
+
+            raise AttributeError(*e.args, name=e.name, obj=e.obj).with_traceback(
+                TracebackType(
+                    tb_next=None,
+                    tb_frame=last_frame,
+                    tb_lasti=last_frame.f_lasti,
+                    tb_lineno=last_frame.f_lineno,
+                )
+            )
+
+        return __key
+
+    @final
+    def __getitem__(self, __key: str, class_object: object) -> Any:
+        return super().__getitem__(self.__pyattr_check(__key, class_object))
+
+    @final
+    def __setitem__(self, __key: str, __value: str, class_object: object) -> None:
+        super().__setitem__(self.__pyattr_check(__key, class_object), __value)
+
+
+class Pyattr(_PyattrDict):
+    def __init__(self, **kwargs) -> None:
+        object.__setattr__(
+            self, "pyattr_class_object", _pyattr_stack()[1].f_locals["__class__"]
+        )
+
+        super().update(kwargs)
+
+    @final
+    def pyattr_get_class_object(self) -> object:
+        try:
+            return object.__getattribute__(self, "pyattr_class_object")
+        except AttributeError:
+            last_frame = _pyattr_stack()[2]
+
+            raise PyattrError(
+                "Did you forget to add 'super().__init__()' at the start of the '__init__' function of your class?"
+            ).with_traceback(
+                TracebackType(
+                    tb_next=None,
+                    tb_frame=last_frame,
+                    tb_lasti=last_frame.f_lasti,
+                    tb_lineno=last_frame.f_lineno,
+                )
+            )
+
+    @final
+    def __getattribute__(self, __name: str) -> Any:
+        try:
+            obj = object.__getattribute__(self, __name)
+
+            return obj
+        except AttributeError:
+            pass
+
+        return super().__getitem__(__name, self.pyattr_get_class_object())
+
+    @final
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        return super().__setitem__(__name, __value, self.pyattr_get_class_object())
```

### Comparing `pyattr-1.4.4/pyattr.egg-info/PKG-INFO` & `pyattr-1.4.5/pyattr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,90 @@
-Metadata-Version: 2.1
-Name: pyattr
-Version: 1.4.4
-Summary: Proper access modifiers for Python classes.
-Home-page: https://github.com/skifli/pyattr
-Author: skifli
-License: MIT
-Project-URL: Documentation, https://github.com/skifli/pyattr#example
-Project-URL: Source, https://github.com/skifli/pyattr
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pyattr
-
-[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
-![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
-
-- [pyattr](#pyattr)
-  - [Installation](#installation)
-  - [Usage](#usage)
-  - [Example](#example)
-  - [How it works](#how-it-works)
-  - [Benchmarks](#benchmarks)
-
-While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
-
-## Installation
-
-Installation via **pip**:
-
-```
-pip install pyattr
-```
-
-## Usage
-
-All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
-
-## Example
-
-Here is a simple example involving a *private* variable.
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-        self.__name = "pyattr"
-
-example = Example()
-print(example.__name) # Error - '__name' is a private attribute of 'Example'.
-```
-
-As well as variables, **pyattr** also supports access control of *functions*!
-
-```python
-from pyattr import Pyattr
-
-class Example(Pyattr):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __example(self) -> None:
-        pass
-
-
-example = Example()
-print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
-```
-
-## How it works
-
-> **Note** For a more in-depth explanation on how **pyattr** works, see my [blog post](https://skifli.github.io/blog/2023/pyattr_in_depth_explanation.html#how-does-pyattr-work#how-does-pyattr-work).
-
-**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
-
-The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`inspect.stack()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
-
-## Benchmarks
-
-The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
-
-[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
+Metadata-Version: 2.1
+Name: pyattr
+Version: 1.4.5
+Summary: Proper access modifiers for Python classes.
+Home-page: https://github.com/skifli/pyattr
+Author: skifli
+License: MIT
+Project-URL: Documentation, https://github.com/skifli/pyattr#example
+Project-URL: Source, https://github.com/skifli/pyattr
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pyattr
+
+[![PyPI](https://img.shields.io/pypi/v/pyattr)](https://pypi.org/project/pyattr)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pyattr)](https://pypi.org/project/pyattr/#files)
+![Lines of Code](https://img.shields.io/github/languages/code-size/skifli/pyattr)
+
+- [pyattr](#pyattr)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Example](#example)
+  - [How it works](#how-it-works)
+  - [Benchmarks](#benchmarks)
+
+While Python does have name mangling, it is not nearly as powerful as access modifiers found in languages such as C++. **pyattr** provides an easy-to-use API for access modifiers in Python.
+
+## Installation
+
+Installation via **pip**:
+
+```
+pip install pyattr
+```
+
+## Usage
+
+All you have to do is make your class inherit from the *`pyattr.Pyattr`* class, and add *`super().__init__()`* as the first line in the *`__init__`* function of your class. And that's it! **pyattr** will handle the magic to make sure variables cannot be accessed / set where the shouldn't be. It also provides useful error messages to users.
+
+## Example
+
+Here is a simple example involving a *private* variable.
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.__name = "pyattr"
+
+example = Example()
+print(example.__name) # Error - '__name' is a private attribute of 'Example'.
+```
+
+As well as variables, **pyattr** also supports access control of *functions*!
+
+```python
+from pyattr import Pyattr
+
+class Example(Pyattr):
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __example(self) -> None:
+        pass
+
+
+example = Example()
+print(example.__example())  # Error - '__example' is a private attribute of 'Example'.
+```
+
+## How it works
+
+**pyattr** overrides the default *set* and *get* functions of your class. The overridden functions defined by **pyattr** are merged into your class when you inherit from the *`pyattr.Pyattr`* class. As well as this, the *`pyattr.Pyattr`* class inherits from the *`pyattr._PyattrDict`* class, which provides a custom dictionary implementation. This is because you can change the variables in a class using *`class.__dict__["var"] = "val"`*, meaning a custom dictionary would be the best way to prevent the access system being circumvented.
+
+The overriden *set* and *get* functions of your class call the respective *set* and *get* functions of the custom dictionary. This dictionary, using *`sys._getframe()`*, works out the caller's function, and the caller's class (if any). It uses this data to work out if the caller should be allowed to access the specified variables. If it shouldn't, an *`AttributeError`* is raised, with an error message explaining the cause.
+
+## Benchmarks
+
+The code for the benchmarks can be found in the [benchmark](https://github.com/skifli/pyattr/blob/main/benchmark/) folder.
+
+[![Benchmark Output](https://raw.githubusercontent.com/skifli/pyattr/main/benchmark/output.png)](https://github.com/skifli/pyattr/blob/main/benchmark/bench_test.py)
```

### Comparing `pyattr-1.4.4/setup.py` & `pyattr-1.4.5/setup.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from setuptools import setup
-from pyattr import __version__
-
-with open("README.md", "r") as f:
-    long_description = f.read()
-
-setup(
-    name="pyattr",
-    version=__version__,
-    author="skifli",
-    url="https://github.com/skifli/pyattr",
-    project_urls={
-        "Documentation": "https://github.com/skifli/pyattr#example",
-        "Source": "https://github.com/skifli/pyattr",
-    },
-    description="Proper access modifiers for Python classes.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license="MIT",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-    ],
-    packages=["pyattr"],
-)
+from setuptools import setup
+from pyattr import __version__
+
+with open("README.md", "r") as f:
+    long_description = f.read()
+
+setup(
+    name="pyattr",
+    version=__version__,
+    author="skifli",
+    url="https://github.com/skifli/pyattr",
+    project_urls={
+        "Documentation": "https://github.com/skifli/pyattr#example",
+        "Source": "https://github.com/skifli/pyattr",
+    },
+    description="Proper access modifiers for Python classes.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license="MIT",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+    ],
+    packages=["pyattr"],
+)
```

