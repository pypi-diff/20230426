# Comparing `tmp/fountains-2.0.0.tar.gz` & `tmp/fountains-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fountains-2.0.0.tar", last modified: Fri Aug  5 02:48:55 2022, max compression
+gzip compressed data, was "fountains-2.1.0.tar", last modified: Wed Apr 26 19:29:02 2023, max compression
```

## Comparing `fountains-2.0.0.tar` & `fountains-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-05 02:48:55.719993 fountains-2.0.0/
--rw-rw-rw-   0        0        0     1087 2022-03-13 02:07:37.000000 fountains-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     7455 2022-08-05 02:48:55.719882 fountains-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6886 2022-07-26 07:32:01.000000 fountains-2.0.0/README.rst
--rw-rw-rw-   0        0        0     1082 2022-06-27 02:12:55.000000 fountains-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-05 02:48:55.719993 fountains-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-05 02:48:55.708024 fountains-2.0.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-05 02:48:55.709497 fountains-2.0.0/src/fountains/
--rw-rw-rw-   0        0        0       90 2022-03-13 02:07:37.000000 fountains-2.0.0/src/fountains/__init__.py
--rw-rw-rw-   0        0        0    11711 2022-08-05 02:38:11.000000 fountains-2.0.0/src/fountains/fountains.py
-drwxrwxrwx   0        0        0        0 2022-08-05 02:48:55.718827 fountains-2.0.0/src/fountains.egg-info/
--rw-rw-rw-   0        0        0     7455 2022-08-05 02:48:55.000000 fountains-2.0.0/src/fountains.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2022-08-05 02:48:55.000000 fountains-2.0.0/src/fountains.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-05 02:48:55.000000 fountains-2.0.0/src/fountains.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      227 2022-08-05 02:48:55.000000 fountains-2.0.0/src/fountains.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-05 02:48:55.000000 fountains-2.0.0/src/fountains.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:29:02.572013 fountains-2.1.0/
+-rw-r--r--   0 alapets    (502) staff       (20)     1066 2023-04-26 19:11:20.000000 fountains-2.1.0/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     7649 2023-04-26 19:29:02.571852 fountains-2.1.0/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     7098 2023-04-26 19:21:40.000000 fountains-2.1.0/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)     1031 2023-04-26 19:19:48.000000 fountains-2.1.0/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-26 19:29:02.572056 fountains-2.1.0/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:29:02.569707 fountains-2.1.0/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:29:02.570884 fountains-2.1.0/src/fountains/
+-rw-r--r--   0 alapets    (502) staff       (20)       88 2023-04-26 19:11:20.000000 fountains-2.1.0/src/fountains/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)    11430 2023-04-26 19:11:20.000000 fountains-2.1.0/src/fountains/fountains.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-26 19:29:02.571677 fountains-2.1.0/src/fountains.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     7649 2023-04-26 19:29:02.000000 fountains-2.1.0/src/fountains.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      270 2023-04-26 19:29:02.000000 fountains-2.1.0/src/fountains.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-26 19:29:02.000000 fountains-2.1.0/src/fountains.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      228 2023-04-26 19:29:02.000000 fountains-2.1.0/src/fountains.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)       10 2023-04-26 19:29:02.000000 fountains-2.1.0/src/fountains.egg-info/top_level.txt
```

### Comparing `fountains-2.0.0/LICENSE` & `fountains-2.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Reity LLC
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
+Copyright (c) 2020 Reity LLC
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

### Comparing `fountains-2.0.0/PKG-INFO` & `fountains-2.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,183 @@
-Metadata-Version: 2.1
-Name: fountains
-Version: 2.0.0
-Summary: Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/reity/fountains
-Project-URL: Documentation, https://fountains.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=========
-fountains
-=========
-
-Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fountains.svg
-   :target: https://badge.fury.io/py/fountains
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
-   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
-   :target: https://coveralls.io/github/reity/fountains?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__::
-
-    python -m pip install fountains
-
-The library can be imported in the usual ways::
-
-    import fountains
-    from fountains import fountains
-
-Examples
-^^^^^^^^
-
-.. |fountains| replace:: ``fountains``
-.. _fountains: https://fountains.readthedocs.io/en/2.0.0/_source/fountains.html#fountains.fountains.fountains
-
-An object of the |fountains|_ class can be used to generate pseudorandom binary test data::
-
-    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
-    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
-
-Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs::
-
-    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
-    >>> bits = list(fountains(3, 8, function=add))
-    >>> bits
-    [0, 0, 1, 1, 1, 0, 1, 0]
-    
-When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character::
-    
-    >>> from bitlist import bitlist
-    >>> bitlist(bits).hex()
-    '3a' # Partial outputs from eight distinct tests.
-
-Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior::
-
-    >>> list(fountains(3, 8, function=add, bits='3a'))
-    [True, True, True, True, True, True, True, True]
-
-Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification::
-
-    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
-    >>> list(fountains(3, 8, function=mul, bits='3a'))
-    [True, False, True, True, False, True, False, True]
-
-Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/fountains/fountains.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fountains
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: fountains
+Version: 2.1.0
+Summary: Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/reity/fountains
+Project-URL: Documentation, https://fountains.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=========
+fountains
+=========
+
+Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fountains.svg
+   :target: https://badge.fury.io/py/fountains
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
+   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
+   :target: https://coveralls.io/github/reity/fountains?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__:
+
+.. code-block:: bash
+
+    python -m pip install fountains
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fountains
+    from fountains import fountains
+
+Examples
+^^^^^^^^
+
+.. |fountains| replace:: ``fountains``
+.. _fountains: https://fountains.readthedocs.io/en/2.1.0/_source/fountains.html#fountains.fountains.fountains
+
+An object of the |fountains|_ class can be used to generate pseudorandom binary test data:
+
+.. code-block:: python
+
+    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
+    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
+
+Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs:
+
+.. code-block:: python
+
+    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
+    >>> bits = list(fountains(3, 8, function=add))
+    >>> bits
+    [0, 0, 1, 1, 1, 0, 1, 0]
+
+When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character:
+
+.. code-block:: python
+
+    >>> from bitlist import bitlist
+    >>> bitlist(bits).hex()
+    '3a' # Partial outputs from eight distinct tests.
+
+Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior:
+
+.. code-block:: python
+
+    >>> list(fountains(3, 8, function=add, bits='3a'))
+    [True, True, True, True, True, True, True, True]
+
+Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification:
+
+.. code-block:: python
+
+    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
+    >>> list(fountains(3, 8, function=mul, bits='3a'))
+    [True, False, True, True, False, True, False, True]
+
+Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/fountains/fountains.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fountains
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `fountains-2.0.0/README.rst` & `fountains-2.1.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,133 +1,165 @@
-=========
-fountains
-=========
-
-Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fountains.svg
-   :target: https://badge.fury.io/py/fountains
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
-   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
-   :target: https://coveralls.io/github/reity/fountains?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__::
-
-    python -m pip install fountains
-
-The library can be imported in the usual ways::
-
-    import fountains
-    from fountains import fountains
-
-Examples
-^^^^^^^^
-
-.. |fountains| replace:: ``fountains``
-.. _fountains: https://fountains.readthedocs.io/en/2.0.0/_source/fountains.html#fountains.fountains.fountains
-
-An object of the |fountains|_ class can be used to generate pseudorandom binary test data::
-
-    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
-    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
-
-Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs::
-
-    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
-    >>> bits = list(fountains(3, 8, function=add))
-    >>> bits
-    [0, 0, 1, 1, 1, 0, 1, 0]
-    
-When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character::
-    
-    >>> from bitlist import bitlist
-    >>> bitlist(bits).hex()
-    '3a' # Partial outputs from eight distinct tests.
-
-Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior::
-
-    >>> list(fountains(3, 8, function=add, bits='3a'))
-    [True, True, True, True, True, True, True, True]
-
-Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification::
-
-    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
-    >>> list(fountains(3, 8, function=mul, bits='3a'))
-    [True, False, True, True, False, True, False, True]
-
-Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/fountains/fountains.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fountains
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+=========
+fountains
+=========
+
+Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fountains.svg
+   :target: https://badge.fury.io/py/fountains
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
+   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
+   :target: https://coveralls.io/github/reity/fountains?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__:
+
+.. code-block:: bash
+
+    python -m pip install fountains
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fountains
+    from fountains import fountains
+
+Examples
+^^^^^^^^
+
+.. |fountains| replace:: ``fountains``
+.. _fountains: https://fountains.readthedocs.io/en/2.1.0/_source/fountains.html#fountains.fountains.fountains
+
+An object of the |fountains|_ class can be used to generate pseudorandom binary test data:
+
+.. code-block:: python
+
+    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
+    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
+
+Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs:
+
+.. code-block:: python
+
+    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
+    >>> bits = list(fountains(3, 8, function=add))
+    >>> bits
+    [0, 0, 1, 1, 1, 0, 1, 0]
+
+When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character:
+
+.. code-block:: python
+
+    >>> from bitlist import bitlist
+    >>> bitlist(bits).hex()
+    '3a' # Partial outputs from eight distinct tests.
+
+Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior:
+
+.. code-block:: python
+
+    >>> list(fountains(3, 8, function=add, bits='3a'))
+    [True, True, True, True, True, True, True, True]
+
+Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification:
+
+.. code-block:: python
+
+    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
+    >>> list(fountains(3, 8, function=mul, bits='3a'))
+    [True, False, True, True, False, True, False, True]
+
+Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/fountains/fountains.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fountains
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

### Comparing `fountains-2.0.0/pyproject.toml` & `fountains-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-[project]
-name = "fountains"
-version = "2.0.0"
-description = """\
-    Python library for generating and concisely specifying \
-    reproducible pseudorandom binary data for unit testing.\
-    """
-license = {text = "MIT"}
-authors = [
-    {name = "Andrei Lapets"},
-    {email = "a@lapets.io"}
-]
-readme = "README.rst"
-requires-python = ">=3.7"
-dependencies = [
-    "bitlist~=1.0"
-]
-
-[project.urls]
-Repository = "https://github.com/reity/fountains"
-Documentation = "https://fountains.readthedocs.io"
-
-[project.optional-dependencies]
-docs = [
-    "toml~=0.10.2",
-    "sphinx~=4.2.0",
-    "sphinx-rtd-theme~=1.0.0",
-    "sphinx-autodoc-typehints~=1.12.0"
-]
-test = [
-    "pytest~=7.0",
-    "pytest-cov~=3.0"
-]
-lint = [
-    "pylint~=2.14.0"
-]
-coveralls = [
-    "coveralls~=3.3.1"
-]
-publish = [
-    "build~=0.8",
-    "twine~=4.0"
-]
-
-[build-system]
-requires = [
-    "setuptools~=62.0"
-]
-build-backend = "setuptools.build_meta"
-
-[tool.pytest.ini_options]
-addopts = "--doctest-modules --ignore=docs --cov=fountains --cov-report term-missing"
+[project]
+name = "fountains"
+version = "2.1.0"
+description = """\
+    Python library for generating and concisely specifying \
+    reproducible pseudorandom binary data for unit testing.\
+    """
+license = {text = "MIT"}
+authors = [
+    {name = "Andrei Lapets"},
+    {email = "a@lapets.io"}
+]
+readme = "README.rst"
+requires-python = ">=3.7"
+dependencies = [
+    "bitlist~=1.1"
+]
+
+[project.urls]
+Repository = "https://github.com/reity/fountains"
+Documentation = "https://fountains.readthedocs.io"
+
+[project.optional-dependencies]
+docs = [
+    "toml~=0.10.2",
+    "sphinx~=4.2.0",
+    "sphinx-rtd-theme~=1.0.0",
+    "sphinx-autodoc-typehints~=1.12.0"
+]
+test = [
+    "pytest~=7.2",
+    "pytest-cov~=4.0"
+]
+lint = [
+    "pylint~=2.17.0"
+]
+coveralls = [
+    "coveralls~=3.3.1"
+]
+publish = [
+    "build~=0.10",
+    "twine~=4.0"
+]
+
+[build-system]
+requires = [
+    "setuptools~=67.6"
+]
+build-backend = "setuptools.build_meta"
+
+[tool.pytest.ini_options]
+addopts = "--doctest-modules --ignore=docs --cov=fountains --cov-report term-missing"
```

### Comparing `fountains-2.0.0/src/fountains/fountains.py` & `fountains-2.1.0/src/fountains/fountains.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-"""
-Python library for generating and concisely specifying
-reproducible pseudorandom binary data for unit testing.
-"""
-from __future__ import annotations
-from typing import Tuple, Union, Optional, Callable, Sequence, Iterable
-import doctest
-import string
-from math import log2
-import hashlib
-from bitlist import bitlist
-
-class fountains: # pylint: disable=too-many-arguments,too-few-public-methods
-    """
-    Class that can act as a pseudorandom test data generator and a testing
-    harness for functions.
-
-    :param length: Size in bytes of each pseudorandom bytes-like object.
-    :param limit: Number of pseudorandom bytes-like objects to generate.
-    :param seed: Seed to use for generating pseudorandom bytes-like objects.
-    :param bits: Output specification to use for testing a function.
-    :param function: Function to test against the supplied specification.
-
-    An object of this class can be used to generate pseudorandom binary test data.
-
-    >>> [bs.hex() for bs in fountains(2, limit=3)]
-    ['e3b0', 'ce1b', '2ed5']
-    >>> [int.from_bytes(bs, 'little') for bs in fountains(2, 3, seed=123)]
-    [7938, 11702, 64114]
-    >>> [int.from_bytes(bs, 'little') for bs in fountains(2, 3, seed='abc')]
-    [30906, 57846, 34365]
-    >>> fountains(2, seed=-1)
-    Traceback (most recent call last):
-      ...
-    ValueError: integer seed must be non-negative
-    >>> fountains(2, seed=0.1)
-    Traceback (most recent call last):
-      ...
-    ValueError: seed must be of type int, str, bytes, or bytearray
-    >>> [int.from_bytes(bs, 'little') for bs in fountains(1, 3)]
-    [227, 206, 46]
-
-    Supplying a function as a parameter makes it possible to generate a concise
-    specification for that function's behavior across a sequence of pseudorandom
-    inputs. The sequence of inputs corresponds exactly to the test data that is
-    emitted (as in the above example) when the function parameter is not used.
-
-    >>> fun = lambda bs: bytes(reversed(bs))
-    >>> bitlist(list(fountains(8, limit=5 * 8, function=fun))).hex()
-    '30a2657266'
-
-    Supplying the specification generated in the manner above as an additional
-    parameter makes it possible to test a function's behavior. In this case, an
-    iterable of boolean values is returned, with each boolean value in the sequence
-    indicating whether the function's behavior on the corresponding input (within
-    the sequence of pseudorandom test inputs) is consistent with the specification.
-    Note that *false negatives may occur*, but *false positives never occur*.
-
-    >>> list(fountains(4, 4, function=fun, bits=bytes([123])))
-    [True, True, True, True, False, True, True, True]
-    >>> list(fountains(4, 4, function=fun, bits='7b'))
-    [True, True, True, True, False, True, True, True]
-    >>> list(fountains(4, 4, function=fun, bits=0.1)) # doctest: +ELLIPSIS
-    Traceback (most recent call last):
-      ...
-    ValueError: target bits must be a sequence of integers ... bytearray
-    >>> list(fountains(4, 4, function=fun, bits=[0, 1, 0, 1]))
-    [True, True, False, True]
-    >>> [check(bitlist(fun(bs))) for (bs, check) in list(fountains(4, 4, bits=[0, 1, 0, 1]))]
-    [True, True, False, True]
-    >>> fun = lambda bs: bitlist([1])
-    >>> list(fountains(4, 4, function=fun, bits=[0, 1, 0, 1]))
-    [False, True, False, True]
-    >>> fun = lambda bs: ['this is a list']
-    >>> list(fountains(1, 1, function=fun, bits=[1]))
-    Traceback (most recent call last):
-      ...
-    TypeError: test output must be a bytes-like object or bitlist
-
-    It is possible to limit the number of pseudorandom test values
-    that are yielded (or, depending on the other parameters, the
-    number of tests that are conducted) when iterating over an object.
-
-    >>> len(list(fountains(32, limit=10)))
-    10
-    >>> len(list(fountains(32, limit=5)))
-    5
-    >>> from itertools import islice
-    >>> len(list(islice(fountains(32, limit=10), 0, 5)))
-    5
-    >>> len(list(islice(fountains(32), 0, 5)))
-    5
-    """
-    def __init__(
-            self: fountains,
-            length: int = 1,
-            limit: Optional[int] = None,
-            seed: Union[int, str, bytes, bytearray, None] = bytes(0),
-            bits: Union[Sequence[int], str, bytes, bytearray, None] = None,
-            function:
-                Union[
-                    Callable[[bytes], bytes],
-                    Callable[[bytes], bytearray],
-                    Callable[[bytes], bitlist],
-                    None
-                ] = None
-        ):
-        self.length = length
-        self.limit = limit
-        self.count = 0
-        self.bit_ = 0
-
-        if isinstance(seed, int):
-            if seed < 0:
-                raise ValueError('integer seed must be non-negative')
-            self.state = seed.to_bytes(1 + (int(log2(max(seed, 1))) // 8), 'little')
-        elif isinstance(seed, str):
-            self.state = str.encode(seed)
-        elif isinstance(seed, (bytes, bytearray)):
-            self.state = seed
-        else:
-            raise ValueError('seed must be of type int, str, bytes, or bytearray')
-
-        if bits is None:
-            self.bits = None
-        elif isinstance(bits, (bytes, bytearray)):
-            self.bits = bitlist(bits)
-            self.limit = len(self.bits) # Only enough data for target bits.
-        elif isinstance(bits, list) and all(isinstance(n, int) for n in bits):
-            self.bits = bitlist(bits)
-            self.limit = len(self.bits) # Only enough data for target bits.
-        elif isinstance(bits, str) and all(c in string.hexdigits for c in bits):
-            self.bits = bitlist.fromhex(bits)
-            self.limit = len(self.bits) # Only enough data for target bits.
-        else:
-            raise ValueError(
-                'target bits must be a sequence of integers (each either 0 or 1)' +
-                'or of type int, str (of hexdigits), bytes, or bytearray'
-            )
-
-        self.function = function
-
-    def _bit(self: fountains, bs: Union[bytes, bytearray, bitlist]) -> int:
-        """
-        Obtain the next bit from the output.
-        """
-        if isinstance(bs, (bytes, bytearray)):
-            bs = bitlist(bs)
-
-        if not isinstance(bs, bitlist):
-            raise TypeError('test output must be a bytes-like object or bitlist')
-
-        # Reset the bit counter if the output is too short.
-        self.bit_ = self.bit_ if self.bit_ < len(bs) else 0
-
-        return bs[self.bit_]
-
-    def __iter__(
-            self: fountains
-        ) -> Union[
-            Iterable[int],
-            Iterable[bool],
-            Iterable[Tuple[bytes, Callable[[bitlist], bool]]],
-            Iterable[bytes]
-        ]:
-        """
-        Return a generator that yields values based on the parameters
-        supplied at this object's instantiation. If the supplied arguments
-        contain no specification and no function, an iterable of infinitely
-        many pseudorandom test inputs is returned (where each input has
-        ``length`` bytes).
-
-        >>> from itertools import islice
-        >>> [bs.hex() for bs in islice(fountains(length=3), 0, 3)]
-        ['e3b0c4', 'ce1bc4', '2ed5b5']
-
-        If an integer value is provided for the ``limit`` argument, then
-        exactly that many test inputs are returned.
-
-        >>> [bs.hex() for bs in fountains(length=3, limit=4)]
-        ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
-
-        If a function is supplied but no specification is provided, an iterable
-        of individual bit values is returned. This output can act as a
-        specification (*e.g.*, in a subsequent invocation).
-
-        >>> fun = lambda bs: hashlib.md5(bs).digest()
-        >>> list(fountains(
-        ...     length=2,
-        ...     limit=4,
-        ...     function=fun
-        ... ))
-        [0, 0, 1, 1]
-
-        In the example below, the specification generated above is supplied.
-        In this case, an iterable of boolean values is returned. Each boolean
-        value represents whether the function satisfies the corresponding entry
-        in the specification.
-
-        >>> list(fountains(
-        ...     length=2,
-        ...     limit=4,
-        ...     bits=[0, 0, 1, 1],
-        ...     function=fun
-        ... ))
-        [True, True, True, True]
-        >>> list(fountains(
-        ...     length=2,
-        ...     limit=4,
-        ...     bits=[0, 0, 1, 0],
-        ...     function=fun
-        ... ))
-        [True, True, True, False]
-
-        If no function is supplied but a specification is supplied, then an
-        iterable of tuples is returned. Each tuple consists of a test input
-        and a predicate that can be applied to the output of a function
-        (represented as a :obj:`~bitlist.bitlist.bitlist` object).
-
-        >>> bcs = list(fountains(
-        ...     length=2,
-        ...     limit=4,
-        ...     bits=[0, 0, 1, 1]
-        ... ))
-
-        For a given index ``i`` of the output ``bcs``, suppose that the entry
-        is the tuple ``(bs, check)``. Normally, the function being tested would
-        be applied to the input ``bs`` to obtain an output. When the predicate
-        ``check`` is applied to this output, it determines whether that output
-        satisfies the entry at index ``i`` within the specification (*i.e.*,
-        ``[0, 0, 1, 1]`` in this example).
-
-        The example below utilizes the above output ``bcs`` to test the
-        function ``fun``. Note that in the below example, the output of ``fun``
-        is converted in the below into a :obj:`~bitlist.bitlist.bitlist` object
-        (because ``fun`` returns an output of type :obj:`bytes` but each
-        predicate expects a :obj:`~bitlist.bitlist.bitlist` object).
-
-        >>> [check(bitlist(fun(bs))) for (bs, check) in bcs]
-        [True, True, True, True]
-        """
-        while self.limit is None or self.count < self.limit:
-            bs = bytearray()
-            while len(bs) < self.length:
-                bs_ = hashlib.sha256(self.state).digest()
-                bs.extend(bs_[:16])
-                self.state = bs_[16:]
-
-            if self.function is not None and self.bits is None:
-                # Return the output bits of the function on the
-                # generated test inputs, one at a time.
-                yield self._bit(self.function(bytes(bs[:self.length])))
-
-            elif self.function is not None and self.bits is not None:
-                # Return whether the function has the correct bit
-                # in its output for this generated input.
-                yield \
-                    self.bits[self.count] == \
-                        self._bit(self.function(bytes(bs[:self.length])))
-
-            elif self.function is None and self.bits is not None:
-                # If a target bit sequence has been supplied
-                # but no function has been supplied, return a
-                # function that checks an output for that bit.
-                yield (
-                    bytes(bs[:self.length]),
-                    eval( # pylint: disable=eval-used
-                        'lambda bs: bs[' + str(self.bit_) + '] == ' + \
-                        str(self.bits[self.count])
-                    )
-                )
-
-            else:
-                # Return the generated test input.
-                yield bytes(bs[:self.length])
-
-            self.count += 1
-            self.bit_ += 1
-
-if __name__ == '__main__':
-    doctest.testmod() # pragma: no cover
+"""
+Python library for generating and concisely specifying
+reproducible pseudorandom binary data for unit testing.
+"""
+from __future__ import annotations
+from typing import Tuple, Union, Optional, Callable, Sequence, Iterable
+import doctest
+import string
+from math import log2
+import hashlib
+from bitlist import bitlist
+
+class fountains: # pylint: disable=too-many-arguments,too-few-public-methods
+    """
+    Class that can act as a pseudorandom test data generator and a testing
+    harness for functions.
+
+    :param length: Size in bytes of each pseudorandom bytes-like object.
+    :param limit: Number of pseudorandom bytes-like objects to generate.
+    :param seed: Seed to use for generating pseudorandom bytes-like objects.
+    :param bits: Output specification to use for testing a function.
+    :param function: Function to test against the supplied specification.
+
+    An object of this class can be used to generate pseudorandom binary test data.
+
+    >>> [bs.hex() for bs in fountains(2, limit=3)]
+    ['e3b0', 'ce1b', '2ed5']
+    >>> [int.from_bytes(bs, 'little') for bs in fountains(2, 3, seed=123)]
+    [7938, 11702, 64114]
+    >>> [int.from_bytes(bs, 'little') for bs in fountains(2, 3, seed='abc')]
+    [30906, 57846, 34365]
+    >>> fountains(2, seed=-1)
+    Traceback (most recent call last):
+      ...
+    ValueError: integer seed must be non-negative
+    >>> fountains(2, seed=0.1)
+    Traceback (most recent call last):
+      ...
+    ValueError: seed must be of type int, str, bytes, or bytearray
+    >>> [int.from_bytes(bs, 'little') for bs in fountains(1, 3)]
+    [227, 206, 46]
+
+    Supplying a function as a parameter makes it possible to generate a concise
+    specification for that function's behavior across a sequence of pseudorandom
+    inputs. The sequence of inputs corresponds exactly to the test data that is
+    emitted (as in the above example) when the function parameter is not used.
+
+    >>> fun = lambda bs: bytes(reversed(bs))
+    >>> bitlist(list(fountains(8, limit=5 * 8, function=fun))).hex()
+    '30a2657266'
+
+    Supplying the specification generated in the manner above as an additional
+    parameter makes it possible to test a function's behavior. In this case, an
+    iterable of boolean values is returned, with each boolean value in the sequence
+    indicating whether the function's behavior on the corresponding input (within
+    the sequence of pseudorandom test inputs) is consistent with the specification.
+    Note that *false negatives may occur*, but *false positives never occur*.
+
+    >>> list(fountains(4, 4, function=fun, bits=bytes([123])))
+    [True, True, True, True, False, True, True, True]
+    >>> list(fountains(4, 4, function=fun, bits='7b'))
+    [True, True, True, True, False, True, True, True]
+    >>> list(fountains(4, 4, function=fun, bits=0.1)) # doctest: +ELLIPSIS
+    Traceback (most recent call last):
+      ...
+    ValueError: target bits must be a sequence of integers ... bytearray
+    >>> list(fountains(4, 4, function=fun, bits=[0, 1, 0, 1]))
+    [True, True, False, True]
+    >>> [check(bitlist(fun(bs))) for (bs, check) in list(fountains(4, 4, bits=[0, 1, 0, 1]))]
+    [True, True, False, True]
+    >>> fun = lambda bs: bitlist([1])
+    >>> list(fountains(4, 4, function=fun, bits=[0, 1, 0, 1]))
+    [False, True, False, True]
+    >>> fun = lambda bs: ['this is a list']
+    >>> list(fountains(1, 1, function=fun, bits=[1]))
+    Traceback (most recent call last):
+      ...
+    TypeError: test output must be a bytes-like object or bitlist
+
+    It is possible to limit the number of pseudorandom test values
+    that are yielded (or, depending on the other parameters, the
+    number of tests that are conducted) when iterating over an object.
+
+    >>> len(list(fountains(32, limit=10)))
+    10
+    >>> len(list(fountains(32, limit=5)))
+    5
+    >>> from itertools import islice
+    >>> len(list(islice(fountains(32, limit=10), 0, 5)))
+    5
+    >>> len(list(islice(fountains(32), 0, 5)))
+    5
+    """
+    def __init__(
+            self: fountains,
+            length: int = 1,
+            limit: Optional[int] = None,
+            seed: Union[int, str, bytes, bytearray, None] = bytes(0),
+            bits: Union[Sequence[int], str, bytes, bytearray, None] = None,
+            function:
+                Union[
+                    Callable[[bytes], bytes],
+                    Callable[[bytes], bytearray],
+                    Callable[[bytes], bitlist],
+                    None
+                ] = None
+        ):
+        self.length = length
+        self.limit = limit
+        self.count = 0
+        self.bit_ = 0
+
+        if isinstance(seed, int):
+            if seed < 0:
+                raise ValueError('integer seed must be non-negative')
+            self.state = seed.to_bytes(1 + (int(log2(max(seed, 1))) // 8), 'little')
+        elif isinstance(seed, str):
+            self.state = str.encode(seed)
+        elif isinstance(seed, (bytes, bytearray)):
+            self.state = seed
+        else:
+            raise ValueError('seed must be of type int, str, bytes, or bytearray')
+
+        if bits is None:
+            self.bits = None
+        elif isinstance(bits, (bytes, bytearray)):
+            self.bits = bitlist(bits)
+            self.limit = len(self.bits) # Only enough data for target bits.
+        elif isinstance(bits, list) and all(isinstance(n, int) for n in bits):
+            self.bits = bitlist(bits)
+            self.limit = len(self.bits) # Only enough data for target bits.
+        elif isinstance(bits, str) and all(c in string.hexdigits for c in bits):
+            self.bits = bitlist.fromhex(bits)
+            self.limit = len(self.bits) # Only enough data for target bits.
+        else:
+            raise ValueError(
+                'target bits must be a sequence of integers (each either 0 or 1)' +
+                'or of type int, str (of hexdigits), bytes, or bytearray'
+            )
+
+        self.function = function
+
+    def _bit(self: fountains, bs: Union[bytes, bytearray, bitlist]) -> int:
+        """
+        Obtain the next bit from the output.
+        """
+        if isinstance(bs, (bytes, bytearray)):
+            bs = bitlist(bs)
+
+        if not isinstance(bs, bitlist):
+            raise TypeError('test output must be a bytes-like object or bitlist')
+
+        # Reset the bit counter if the output is too short.
+        self.bit_ = self.bit_ if self.bit_ < len(bs) else 0
+
+        return bs[self.bit_]
+
+    def __iter__(
+            self: fountains
+        ) -> Union[
+            Iterable[int],
+            Iterable[bool],
+            Iterable[Tuple[bytes, Callable[[bitlist], bool]]],
+            Iterable[bytes]
+        ]:
+        """
+        Return a generator that yields values based on the parameters
+        supplied at this object's instantiation. If the supplied arguments
+        contain no specification and no function, an iterable of infinitely
+        many pseudorandom test inputs is returned (where each input has
+        ``length`` bytes).
+
+        >>> from itertools import islice
+        >>> [bs.hex() for bs in islice(fountains(length=3), 0, 3)]
+        ['e3b0c4', 'ce1bc4', '2ed5b5']
+
+        If an integer value is provided for the ``limit`` argument, then
+        exactly that many test inputs are returned.
+
+        >>> [bs.hex() for bs in fountains(length=3, limit=4)]
+        ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
+
+        If a function is supplied but no specification is provided, an iterable
+        of individual bit values is returned. This output can act as a
+        specification (*e.g.*, in a subsequent invocation).
+
+        >>> fun = lambda bs: hashlib.md5(bs).digest()
+        >>> list(fountains(
+        ...     length=2,
+        ...     limit=4,
+        ...     function=fun
+        ... ))
+        [0, 0, 1, 1]
+
+        In the example below, the specification generated above is supplied.
+        In this case, an iterable of boolean values is returned. Each boolean
+        value represents whether the function satisfies the corresponding entry
+        in the specification.
+
+        >>> list(fountains(
+        ...     length=2,
+        ...     limit=4,
+        ...     bits=[0, 0, 1, 1],
+        ...     function=fun
+        ... ))
+        [True, True, True, True]
+        >>> list(fountains(
+        ...     length=2,
+        ...     limit=4,
+        ...     bits=[0, 0, 1, 0],
+        ...     function=fun
+        ... ))
+        [True, True, True, False]
+
+        If no function is supplied but a specification is supplied, then an
+        iterable of tuples is returned. Each tuple consists of a test input
+        and a predicate that can be applied to the output of a function
+        (represented as a :obj:`~bitlist.bitlist.bitlist` object).
+
+        >>> bcs = list(fountains(
+        ...     length=2,
+        ...     limit=4,
+        ...     bits=[0, 0, 1, 1]
+        ... ))
+
+        For a given index ``i`` of the output ``bcs``, suppose that the entry
+        is the tuple ``(bs, check)``. Normally, the function being tested would
+        be applied to the input ``bs`` to obtain an output. When the predicate
+        ``check`` is applied to this output, it determines whether that output
+        satisfies the entry at index ``i`` within the specification (*i.e.*,
+        ``[0, 0, 1, 1]`` in this example).
+
+        The example below utilizes the above output ``bcs`` to test the
+        function ``fun``. Note that in the below example, the output of ``fun``
+        is converted in the below into a :obj:`~bitlist.bitlist.bitlist` object
+        (because ``fun`` returns an output of type :obj:`bytes` but each
+        predicate expects a :obj:`~bitlist.bitlist.bitlist` object).
+
+        >>> [check(bitlist(fun(bs))) for (bs, check) in bcs]
+        [True, True, True, True]
+        """
+        while self.limit is None or self.count < self.limit:
+            bs = bytearray()
+            while len(bs) < self.length:
+                bs_ = hashlib.sha256(self.state).digest()
+                bs.extend(bs_[:16])
+                self.state = bs_[16:]
+
+            if self.function is not None and self.bits is None:
+                # Return the output bits of the function on the
+                # generated test inputs, one at a time.
+                yield self._bit(self.function(bytes(bs[:self.length])))
+
+            elif self.function is not None and self.bits is not None:
+                # Return whether the function has the correct bit
+                # in its output for this generated input.
+                yield \
+                    self.bits[self.count] == \
+                        self._bit(self.function(bytes(bs[:self.length])))
+
+            elif self.function is None and self.bits is not None:
+                # If a target bit sequence has been supplied
+                # but no function has been supplied, return a
+                # function that checks an output for that bit.
+                yield (
+                    bytes(bs[:self.length]),
+                    eval( # pylint: disable=eval-used
+                        'lambda bs: bs[' + str(self.bit_) + '] == ' + \
+                        str(self.bits[self.count])
+                    )
+                )
+
+            else:
+                # Return the generated test input.
+                yield bytes(bs[:self.length])
+
+            self.count += 1
+            self.bit_ += 1
+
+if __name__ == '__main__':
+    doctest.testmod() # pragma: no cover
```

### Comparing `fountains-2.0.0/src/fountains.egg-info/PKG-INFO` & `fountains-2.1.0/src/fountains.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,183 @@
-Metadata-Version: 2.1
-Name: fountains
-Version: 2.0.0
-Summary: Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/reity/fountains
-Project-URL: Documentation, https://fountains.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=========
-fountains
-=========
-
-Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fountains.svg
-   :target: https://badge.fury.io/py/fountains
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
-   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
-   :target: https://coveralls.io/github/reity/fountains?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__::
-
-    python -m pip install fountains
-
-The library can be imported in the usual ways::
-
-    import fountains
-    from fountains import fountains
-
-Examples
-^^^^^^^^
-
-.. |fountains| replace:: ``fountains``
-.. _fountains: https://fountains.readthedocs.io/en/2.0.0/_source/fountains.html#fountains.fountains.fountains
-
-An object of the |fountains|_ class can be used to generate pseudorandom binary test data::
-
-    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
-    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
-
-Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs::
-
-    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
-    >>> bits = list(fountains(3, 8, function=add))
-    >>> bits
-    [0, 0, 1, 1, 1, 0, 1, 0]
-    
-When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character::
-    
-    >>> from bitlist import bitlist
-    >>> bitlist(bits).hex()
-    '3a' # Partial outputs from eight distinct tests.
-
-Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior::
-
-    >>> list(fountains(3, 8, function=add, bits='3a'))
-    [True, True, True, True, True, True, True, True]
-
-Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification::
-
-    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
-    >>> list(fountains(3, 8, function=mul, bits='3a'))
-    [True, False, True, True, False, True, False, True]
-
-Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
-
-Development
------------
-All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__::
-
-    python -m pip install .[docs,lint]
-
-Documentation
-^^^^^^^^^^^^^
-The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__::
-
-    python -m pip install .[docs]
-    cd docs
-    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
-
-Testing and Conventions
-^^^^^^^^^^^^^^^^^^^^^^^
-All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details)::
-
-    python -m pip install .[test]
-    python -m pytest
-
-Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__::
-
-    python src/fountains/fountains.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fountains
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
-
-    python -m pip install .[publish]
-
-Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number)::
-
-    git tag ?.?.?
-    git push origin ?.?.?
-
-Remove any old build/distribution files. Then, package the source into a distribution archive::
-
-    rm -rf build dist src/*.egg-info
-    python -m build --sdist --wheel .
-
-Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__::
-
-    python -m twine upload dist/*
+Metadata-Version: 2.1
+Name: fountains
+Version: 2.1.0
+Summary: Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/reity/fountains
+Project-URL: Documentation, https://fountains.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=========
+fountains
+=========
+
+Python library for generating and concisely specifying reproducible pseudorandom binary data for unit testing.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fountains.svg
+   :target: https://badge.fury.io/py/fountains
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fountains/badge/?version=latest
+   :target: https://fountains.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/reity/fountains/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/reity/fountains/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/reity/fountains/badge.svg?branch=main
+   :target: https://coveralls.io/github/reity/fountains?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library makes it possible to generate pseudorandom binary test data in a reproducible way, as well as to embed concise specifications of correct function behavior on that test data. This enables the construction of functional tests within unit testing suites that fit within one-line definitions but still test a function's behavior against a large number of inputs. More background information about this library's purpose, design, and implementation can be found in a `related article <https://github.com/reity/article-specifications-for-distinguishing-functions>`__.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fountains>`__:
+
+.. code-block:: bash
+
+    python -m pip install fountains
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fountains
+    from fountains import fountains
+
+Examples
+^^^^^^^^
+
+.. |fountains| replace:: ``fountains``
+.. _fountains: https://fountains.readthedocs.io/en/2.1.0/_source/fountains.html#fountains.fountains.fountains
+
+An object of the |fountains|_ class can be used to generate pseudorandom binary test data:
+
+.. code-block:: python
+
+    >>> [bs.hex() for bs in fountains(length=3, limit=4)]
+    ['e3b0c4', 'ce1bc4', '2ed5b5', '781f5a']
+
+Supplying a function as a parameter to a |fountains|_ object makes it possible to generate a concise (but necessarily incomplete) specification for that function's behavior on a stream of pseudorandom inputs:
+
+.. code-block:: python
+
+    >>> add = lambda bs: bytes([(bs[0] + bs[1] + bs[2]) % 256])
+    >>> bits = list(fountains(3, 8, function=add))
+    >>> bits
+    [0, 0, 1, 1, 1, 0, 1, 0]
+
+When converted to a hexadecimal string, this specification encodes partial information about four distinct input-output test cases in every character:
+
+.. code-block:: python
+
+    >>> from bitlist import bitlist
+    >>> bitlist(bits).hex()
+    '3a' # Partial outputs from eight distinct tests.
+
+Supplying the specification generated in the manner above as an additional parameter makes it possible to test the function's behavior:
+
+.. code-block:: python
+
+    >>> list(fountains(3, 8, function=add, bits='3a'))
+    [True, True, True, True, True, True, True, True]
+
+Each individual boolean value in the above represents the result of an individual test case. A different function might not satisfy the same partial specification:
+
+.. code-block:: python
+
+    >>> mul = lambda bs: bytes([(bs[0] * bs[1] * bs[2]) % 256])
+    >>> list(fountains(3, 8, function=mul, bits='3a'))
+    [True, False, True, True, False, True, False, True]
+
+Each boolean value in the outputs of the last two code blocks above may be a false negative (i.e., ``True`` may mean that the function satisfies the specification only in a portion of its output for the corresponding input) but is *never a false positive signal of incorrect behavior* (i.e., ``False`` indicates the function does not satisfy the specification for the corresponding input-output pair).
+
+Development
+-----------
+All installation and development dependencies are fully specified in ``pyproject.toml``. The ``project.optional-dependencies`` object is used to `specify optional requirements <https://peps.python.org/pep-0621>`__ for various development tasks. This makes it possible to specify additional options (such as ``docs``, ``lint``, and so on) when performing installation using `pip <https://pypi.org/project/pip>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs,lint]
+
+Documentation
+^^^^^^^^^^^^^
+The documentation can be generated automatically from the source files using `Sphinx <https://www.sphinx-doc.org>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[docs]
+    cd docs
+    sphinx-apidoc -f -E --templatedir=_templates -o _source .. && make html
+
+Testing and Conventions
+^^^^^^^^^^^^^^^^^^^^^^^
+All unit tests are executed and their coverage is measured when using `pytest <https://docs.pytest.org>`__ (see the ``pyproject.toml`` file for configuration details):
+
+.. code-block:: bash
+
+    python -m pip install .[test]
+    python -m pytest
+
+Alternatively, all unit tests are included in the module itself and can be executed using `doctest <https://docs.python.org/3/library/doctest.html>`__:
+
+.. code-block:: bash
+
+    python src/fountains/fountains.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fountains
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/reity/fountains>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fountains>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
+
+.. code-block:: bash
+
+    python -m pip install .[publish]
+
+Ensure that the correct version number appears in ``pyproject.toml``, and that any links in this README document to the Read the Docs documentation of this package (or its dependencies) have appropriate version numbers. Also ensure that the Read the Docs project for this library has an `automation rule <https://docs.readthedocs.io/en/stable/automation-rules.html>`__ that activates and sets as the default all tagged versions. Create and push a tag for this version (replacing ``?.?.?`` with the version number):
+
+.. code-block:: bash
+
+    git tag ?.?.?
+    git push origin ?.?.?
+
+Remove any old build/distribution files. Then, package the source into a distribution archive:
+
+.. code-block:: bash
+
+    rm -rf build dist src/*.egg-info
+    python -m build --sdist --wheel .
+
+Finally, upload the package distribution archive to `PyPI <https://pypi.org>`__:
+
+.. code-block:: bash
+
+    python -m twine upload dist/*
```

