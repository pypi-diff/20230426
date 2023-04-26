# Comparing `tmp/fe25519-1.3.0.tar.gz` & `tmp/fe25519-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fe25519-1.3.0.tar", last modified: Mon Aug  8 15:27:12 2022, max compression
+gzip compressed data, was "fe25519-1.4.0.tar", last modified: Tue Apr 25 18:54:05 2023, max compression
```

## Comparing `fe25519-1.3.0.tar` & `fe25519-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-08 15:27:12.756646 fe25519-1.3.0/
--rw-rw-rw-   0        0        0     1093 2022-03-13 02:08:32.000000 fe25519-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5676 2022-08-08 15:27:12.756913 fe25519-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5122 2022-07-17 08:09:32.000000 fe25519-1.3.0/README.rst
--rw-rw-rw-   0        0        0     1046 2022-07-17 07:48:10.000000 fe25519-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-08 15:27:12.756913 fe25519-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-08 15:27:12.742038 fe25519-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-08 15:27:12.747824 fe25519-1.3.0/src/fe25519/
--rw-rw-rw-   0        0        0       80 2022-03-13 02:08:32.000000 fe25519-1.3.0/src/fe25519/__init__.py
--rw-rw-rw-   0        0        0    22130 2022-07-30 18:15:09.000000 fe25519-1.3.0/src/fe25519/fe25519.py
-drwxrwxrwx   0        0        0        0 2022-08-08 15:27:12.755787 fe25519-1.3.0/src/fe25519.egg-info/
--rw-rw-rw-   0        0        0     5676 2022-08-08 15:27:12.000000 fe25519-1.3.0/src/fe25519.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-08-08 15:27:12.000000 fe25519-1.3.0/src/fe25519.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-08 15:27:12.000000 fe25519-1.3.0/src/fe25519.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2022-08-08 15:27:12.000000 fe25519-1.3.0/src/fe25519.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-08 15:27:12.000000 fe25519-1.3.0/src/fe25519.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-08 15:27:12.756312 fe25519-1.3.0/test/
--rw-rw-rw-   0        0        0     9372 2022-08-05 07:57:55.000000 fe25519-1.3.0/test/test_fe25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917619 fe25519-1.4.0/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-15 14:39:26.000000 fe25519-1.4.0/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-25 18:54:05.917703 fe25519-1.4.0/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5262 2023-04-15 13:28:07.000000 fe25519-1.4.0/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)      996 2023-04-15 13:26:56.000000 fe25519-1.4.0/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-25 18:54:05.917979 fe25519-1.4.0/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.915043 fe25519-1.4.0/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.916456 fe25519-1.4.0/src/fe25519/
+-rw-r--r--   0 alapets    (502) staff       (20)       78 2023-04-15 14:39:26.000000 fe25519-1.4.0/src/fe25519/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)    21433 2023-04-15 14:39:26.000000 fe25519-1.4.0/src/fe25519/fe25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917332 fe25519-1.4.0/src/fe25519.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     5798 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      221 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-25 18:54:05.000000 fe25519-1.4.0/src/fe25519.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:54:05.917468 fe25519-1.4.0/test/
+-rw-r--r--   0 alapets    (502) staff       (20)     9114 2023-04-15 14:39:26.000000 fe25519-1.4.0/test/test_fe25519.py
```

### Comparing `fe25519-1.3.0/LICENSE` & `fe25519-1.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Nth Party, Ltd.
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
+Copyright (c) 2020 Nth Party, Ltd.
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

### Comparing `fe25519-1.3.0/PKG-INFO` & `fe25519-1.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,116 +1,138 @@
-Metadata-Version: 2.1
-Name: fe25519
-Version: 1.3.0
-Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/fe25519
-Project-URL: Documentation, https://fe25519.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=======
-fe25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
-   :target: https://badge.fury.io/py/fe25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
-   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__::
-
-    python -m pip install fe25519
-
-The library can be imported in the usual ways::
-
-    import fe25519
-    from fe25519 import fe25519
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
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly::
-
-    python test/test_fe25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fe25519 test/test_fe25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: fe25519
+Version: 1.4.0
+Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/fe25519
+Project-URL: Documentation, https://fe25519.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=======
+fe25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
+   :target: https://badge.fury.io/py/fe25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
+   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install fe25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fe25519
+    from fe25519 import fe25519
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
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly:
+
+.. code-block:: bash
+
+    python test/test_fe25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fe25519 test/test_fe25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `fe25519-1.3.0/README.rst` & `fe25519-1.4.0/src/fe25519.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,98 +1,138 @@
-=======
-fe25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
-   :target: https://badge.fury.io/py/fe25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
-   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__::
-
-    python -m pip install fe25519
-
-The library can be imported in the usual ways::
-
-    import fe25519
-    from fe25519 import fe25519
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
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly::
-
-    python test/test_fe25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fe25519 test/test_fe25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: fe25519
+Version: 1.4.0
+Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/fe25519
+Project-URL: Documentation, https://fe25519.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=======
+fe25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
+   :target: https://badge.fury.io/py/fe25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
+   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install fe25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fe25519
+    from fe25519 import fe25519
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
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly:
+
+.. code-block:: bash
+
+    python test/test_fe25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fe25519 test/test_fe25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `fe25519-1.3.0/src/fe25519/fe25519.py` & `fe25519-1.4.0/src/fe25519/fe25519.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,697 +1,697 @@
-"""
-Pure-Python data structure for working with Ed25519 (and Ristretto)
-field elements and operations.
-"""
-from __future__ import annotations
-from typing import Tuple, Sequence
-import doctest
-
-_TWO_TO_64 = 2 ** 64
-_TWO_TO_128 = 2 ** 128
-
-class fe25519:
-    """
-    Class for creating and operating on field elements. The public
-    interface of this class is determined primarily by the needs of
-    the `ge25519 <https://pypi.org/project/ge25519>`__ library.
-    However, use of some built-in Python operators is supported via
-    special methods.
-    """
-    # Precomputed static constants.
-    d = None
-    d2 = None
-    sqrtm1 = None
-    invsqrtamd = None
-    onemsqd = None
-    sqdmone = None
-    sqrtadm1 = None
-    curve25519_A = None
-
-    @staticmethod
-    def zero() -> fe25519:
-        """
-        Constant corresponding to the zero element.
-
-        >>> fe25519.zero() + fe25519.one() == fe25519.one()
-        True
-        """
-        return fe25519([0, 0, 0, 0, 0])
-
-    @staticmethod
-    def one() -> fe25519:
-        """
-        Constant corresponding to the multiplicative identity element.
-
-        >>> fe25519.one() * fe25519.one() == fe25519.one()
-        True
-        """
-        return fe25519([1, 0, 0, 0, 0])
-
-    def __init__(self: fe25519, ns: Sequence[int]):
-        """Create field element using a list of five 64-bit integers."""
-        self.ns = ns # pylint: disable=invalid-name
-
-    def copy(self: fe25519) -> fe25519:
-        """
-        Create a copy of this element instance.
-
-        >>> fe25519.one().copy() == fe25519.one()
-        True
-        """
-        return fe25519(list(self.ns))
-
-    def reduce(self: fe25519) -> fe25519:
-        """
-        Reduce this element to a canonical representation.
-
-        >>> (~fe25519.one()).reduce()
-        fe25519([1, 0, 0, 0, 0])
-        """
-        t = self.ns # 128-bit integers.
-        mask = 2251799813685247
-
-        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
-        t[0] &= mask
-        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
-        t[1] &= mask
-        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
-        t[2] &= mask
-        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
-        t[3] &= mask
-        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
-        t[4] &= mask
-
-        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
-        t[0] &= mask
-        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
-        t[1] &= mask
-        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
-        t[2] &= mask
-        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
-        t[3] &= mask
-        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
-        t[4] &= mask
-
-        # Now t is between 0 and 2^255-1, properly carried.
-        # Сase 1: between 0 and 2^255-20. Case 2: between 2^255-19 and 2^255-1.
-
-        t[0] = (t[0] + 19) % _TWO_TO_128
-
-        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
-        t[0] &= mask
-        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
-        t[1] &= mask
-        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
-        t[2] &= mask
-        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
-        t[3] &= mask
-        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
-        t[4] &= mask
-
-        # Now between 19 and 2^255-1 in both cases, and offset by 19.
-
-        t[0] = (t[0] + 2251799813685248 - 19) % _TWO_TO_128
-        t[1] = (t[1] + 2251799813685248 - 1) % _TWO_TO_128
-        t[2] = (t[2] + 2251799813685248 - 1) % _TWO_TO_128
-        t[3] = (t[3] + 2251799813685248 - 1) % _TWO_TO_128
-        t[4] = (t[4] + 2251799813685248 - 1) % _TWO_TO_128
-
-        # Now between 2^255 and 2^256-20, and offset by 2^255.
-
-        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
-        t[0] &= mask
-        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
-        t[1] &= mask
-        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
-        t[2] &= mask
-        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
-        t[3] &= mask
-        t[4] &= mask
-
-        return fe25519(t)
-
-    def __add__(self: fe25519, other: fe25519) -> fe25519:
-        """
-        Compute the sum of this element and another element.
-
-        >>> fe25519.zero() + fe25519.zero() == fe25519.zero()
-        True
-        """
-        return fe25519([(m+n)%_TWO_TO_64 for (m, n) in zip(self.ns, other.ns)])
-
-    def __neg__(self: fe25519) -> fe25519:
-        """
-        Compute the negation of this element.
-
-        >>> fe25519.one().cneg(1) != fe25519.one()
-        True
-        """
-        return fe25519.zero() - self
-
-    def cmov(self: fe25519, g: fe25519, b: int) -> fe25519:
-        """Conditionally select this element or another based on a boolean integer."""
-        mask = _TWO_TO_64 - b
-        pairs = zip(self.ns, g.ns)
-        return fe25519([fi ^ ((fi ^ gi) & mask) for (fi, gi) in pairs])
-
-    def cneg(self: fe25519, b: int) -> fe25519:
-        """
-        Compute the conditional negation of this element.
-
-        >>> fe25519.one().cneg(0) == fe25519.one()
-        True
-        >>> (fe25519.one().cneg(1) + fe25519.one()).is_zero()
-        1
-        """
-        return self.copy().cmov(-self, b)
-
-    def __abs__(self: fe25519) -> fe25519:
-        """
-        Compute the absolute value of this element.
-
-        >>> abs(-fe25519.one()).is_negative()
-        0
-        """
-        return self.cneg(self.is_negative())
-
-    def __sub__(self: fe25519, other: fe25519) -> fe25519:
-        """
-        Compute the result of subtracting another element from this element.
-
-        >>> fe25519.zero() - fe25519.one() == fe25519.one().cneg(1)
-        True
-        """
-        mask = 2251799813685247
-
-        (h0, h1, h2, h3, h4) = other.ns
-
-        h1 = (h1 + (h0 >> 51)) % _TWO_TO_64
-        h0 &= mask
-        h2 = (h2 + (h1 >> 51)) % _TWO_TO_64
-        h1 &= mask
-        h3 = (h3 + (h2 >> 51)) % _TWO_TO_64
-        h2 &= mask
-        h4 = (h4 + (h3 >> 51)) % _TWO_TO_64
-        h3 &= mask
-        h0 = (h0 + 19 * (h4 >> 51)) % _TWO_TO_64
-        h4 &= mask
-
-        return fe25519([
-            ((self.ns[0] + 4503599627370458) - h0) % _TWO_TO_64,
-            ((self.ns[1] + 4503599627370494) - h1) % _TWO_TO_64,
-            ((self.ns[2] + 4503599627370494) - h2) % _TWO_TO_64,
-            ((self.ns[3] + 4503599627370494) - h3) % _TWO_TO_64,
-            ((self.ns[4] + 4503599627370494) - h4) % _TWO_TO_64
-        ])
-
-    def __mul__(self: fe25519, other: fe25519) -> fe25519:
-        """
-        Compute the product of this element and another element.
-
-        >>> fe25519.one() * fe25519.zero() == fe25519.zero()
-        True
-        """
-        mask = 2251799813685247 # 64-bit integer.
-        (f, g) = (self.ns, other.ns) # 64-bit integers.
-        r = [None, None, None, None, None] # 128-bit integers.
-        carry = None # 128-bit integer.
-        r0 = [None, None, None, None, None] # 64-bit integers.
-
-        f1_19 = (19 * f[1]) % _TWO_TO_64
-        f2_19 = (19 * f[2]) % _TWO_TO_64
-        f3_19 = (19 * f[3]) % _TWO_TO_64
-        f4_19 = (19 * f[4]) % _TWO_TO_64
-
-        r[0] = (f[0]*g[0] + f1_19*g[4] + f2_19*g[3] + f3_19*g[2] + f4_19*g[1]) % _TWO_TO_128
-        r[1] = (f[0]*g[1] + f[1]*g[0] + f2_19*g[4] + f3_19*g[3] + f4_19*g[2]) % _TWO_TO_128
-        r[2] = (f[0]*g[2] + f[1]*g[1] + f[2]*g[0] + f3_19*g[4] + f4_19*g[3]) % _TWO_TO_128
-        r[3] = (f[0]*g[3] + f[1]*g[2] + f[2]*g[1] + f[3]*g[0] + f4_19*g[4]) % _TWO_TO_128
-        r[4] = (f[0]*g[4] + f[1]*g[3] + f[2]*g[2] + f[3]*g[1] + f[4]*g[0]) % _TWO_TO_128
-
-        r0[0] = (r[0] % _TWO_TO_64) & mask
-        r[1] = (r[1] + (r[0] >> 51)) % _TWO_TO_128
-        r0[1] = (r[1] % _TWO_TO_64) & mask
-        r[2] = (r[2] + (r[1] >> 51)) % _TWO_TO_128
-        r0[2] = (r[2] % _TWO_TO_64) & mask
-        r[3] = (r[3] + (r[2] >> 51)) % _TWO_TO_128
-        r0[3] = (r[3] % _TWO_TO_64) & mask
-        r[4] = (r[4] + (r[3] >> 51)) % _TWO_TO_128
-        r0[4] = (r[4] % _TWO_TO_64) & mask
-        r0[0] = (r0[0] + (19*((r[4] >> 51) % _TWO_TO_64))) % _TWO_TO_64
-        carry = r0[0] >> 51
-        r0[0] &= mask
-        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
-        carry = r0[1] >> 51
-        r0[1] &= mask
-        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
-
-        return fe25519(r0)
-
-    def sq(self: fe25519) -> fe25519: # pylint: disable=invalid-name
-        """
-        Compute the square of this element.
-
-        >>> two = fe25519.one() + fe25519.one()
-        >>> four = two + two
-        >>> two.sq() == four
-        True
-        """
-        mask = 2251799813685247 # 64-bit integer.
-        f = self.ns # 64-bit integers.
-        r = [None, None, None, None, None] # 128-bit integers.
-        carry = None # 128-bit integer.
-        r0 = [None, None, None, None, None] # 64-bit integers.
-
-        f0_2 = (f[0] << 1) % _TWO_TO_64
-        f1_2 = (f[1] << 1) % _TWO_TO_64
-
-        f1_38 = (38 * f[1]) % _TWO_TO_64
-        f2_38 = (38 * f[2]) % _TWO_TO_64
-        f3_38 = (38 * f[3]) % _TWO_TO_64
-
-        f3_19 = (19 * f[3]) % _TWO_TO_64
-        f4_19 = (19 * f[4]) % _TWO_TO_64
-
-        r[0] = (f[0]*f[0] + f1_38*f[4] + f2_38*f[3]) % _TWO_TO_128
-        r[1] = (f0_2*f[1] + f2_38*f[4] + f3_19*f[3]) % _TWO_TO_128
-        r[2] = (f0_2*f[2] + f[1]*f[1] + f3_38*f[4]) % _TWO_TO_128
-        r[3] = (f0_2*f[3] + f1_2*f[2] + f4_19*f[4]) % _TWO_TO_128
-        r[4] = (f0_2*f[4] + f1_2*f[3] + f[2]*f[2]) % _TWO_TO_128
-
-        r0[0] = (r[0] % _TWO_TO_64) & mask
-        r[1] = (r[1] + (r[0] >> 51)) % _TWO_TO_128
-        r0[1] = (r[1] % _TWO_TO_64) & mask
-        r[2] = (r[2] + (r[1] >> 51)) % _TWO_TO_128
-        r0[2] = (r[2] % _TWO_TO_64) & mask
-        r[3] = (r[3] + (r[2] >> 51)) % _TWO_TO_128
-        r0[3] = (r[3] % _TWO_TO_64) & mask
-        r[4] = (r[4] + (r[3] >> 51)) % _TWO_TO_128
-        r0[4] = (r[4] % _TWO_TO_64) & mask
-        r0[0] = (r0[0] + (19*((r[4] >> 51) % _TWO_TO_64))) % _TWO_TO_64
-        carry = r0[0] >> 51
-        r0[0] &= mask
-        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
-        carry = r0[1] >> 51
-        r0[1] &= mask
-        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
-
-        return fe25519(r0)
-
-    def sq2(self: fe25519) -> fe25519:
-        """
-        Compute the element that is twice the square of this element.
-
-        >>> two = fe25519.one() + fe25519.one()
-        >>> two.sq2() == two.sq() + two.sq()
-        True
-        """
-        mask = 2251799813685247
-        f = self.ns # 64-bit integers.
-        r = [None, None, None, None, None] # 128-bit integers.
-        carry = None # 128-bit integer.
-        r0 = [None, None, None, None, None] # 64-bit integers.
-
-        f0_2 = (f[0] << 1) % _TWO_TO_64
-        f1_2 = (f[1] << 1) % _TWO_TO_64
-
-        f1_38 = (38 * f[1]) % _TWO_TO_64
-        f2_38 = (38 * f[2]) % _TWO_TO_64
-        f3_38 = (38 * f[3]) % _TWO_TO_64
-
-        f3_19 = (19 * f[3]) % _TWO_TO_64
-        f4_19 = (19 * f[4]) % _TWO_TO_64
-
-        r[0] = (f[0]*f[0] + f1_38*f[4] + f2_38*f[3]) % _TWO_TO_128
-        r[1] = (f0_2*f[1] + f2_38*f[4] + f3_19*f[3]) % _TWO_TO_128
-        r[2] = (f0_2*f[2] + f[1]*f[1] + f3_38*f[4]) % _TWO_TO_128
-        r[3] = (f0_2*f[3] + f1_2*f[2] + f4_19*f[4]) % _TWO_TO_128
-        r[4] = (f0_2*f[4] + f1_2*f[3] + f[2]*f[2]) % _TWO_TO_128
-
-        r[0] <<= 1
-        r[1] <<= 1
-        r[2] <<= 1
-        r[3] <<= 1
-        r[4] <<= 1
-
-        r0[0] = (r[0] % _TWO_TO_64) & mask
-        carry = r[0] >> 51
-        r[1] = (r[1] + carry) % _TWO_TO_128
-        r0[1] = (r[1] % _TWO_TO_64) & mask
-        carry = r[1] >> 51
-        r[2] = (r[2] + carry) % _TWO_TO_128
-
-        r0[2] = (r[2] % _TWO_TO_64) & mask
-        carry = r[2] >> 51
-        r[3] = (r[3] + carry) % _TWO_TO_128
-        r0[3] = (r[3] % _TWO_TO_64) & mask
-        carry = r[3] >> 51
-        r[4] = (r[4] + carry) % _TWO_TO_128
-        r0[4] = (r[4] % _TWO_TO_64) & mask
-        carry = r[4] >> 51
-        r0[0] = (r0[0] + 19*carry) % _TWO_TO_64
-        carry = r0[0] >> 51
-        r0[0] &= mask
-        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
-        carry = r0[1] >> 51
-        r0[1] &= mask
-        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
-
-        return fe25519(r0)
-
-    def pow22523(self: fe25519) -> fe25519:
-        """
-        Compute the result of the exponentiation of this element by a
-        special fixed exponent.
-        """
-        z = self.copy()
-        t0 = z.sq()
-        t1 = t0.sq()
-        t1 = t1.sq()
-        t1 = z * t1
-        t0 = t0 * t1
-        t0 = t0.sq()
-        t0 = t1 * t0
-        t1 = t0.sq()
-        for _ in range(1, 5):
-            t1 = t1.sq()
-        t0 = t1 * t0
-        t1 = t0.sq()
-        for _ in range(1, 10):
-            t1 = t1.sq()
-        t1 = t1 * t0
-        t2 = t1.sq()
-        for _ in range(1, 20):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t1 = t1.sq()
-        for _ in range(1, 10):
-            t1 = t1.sq()
-        t0 = t1 * t0
-        t1 = t0.sq()
-        for _ in range(1, 50):
-            t1 = t1.sq()
-        t1 = t1 * t0
-        t2 = t1.sq()
-        for _ in range(1, 100):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t1 = t1.sq()
-        for _ in range(1, 50):
-            t1 = t1.sq()
-        t0 = t1 * t0
-        t0 = t0.sq()
-        t0 = t0.sq()
-        return t0 * z
-
-    def invert(self: fe25519) -> fe25519:
-        """
-        Compute the multiplicative inverse of this element.
-
-        >>> two = fe25519.one() + fe25519.one()
-        >>> (two.invert() * two).reduce() == fe25519.one()
-        True
-        """
-        z = self.copy()
-        t0 = z.sq()
-        t1 = t0.sq()
-        t1 = t1.sq()
-        t1 = z * t1
-        t0 = t0 * t1
-        t2 = t0.sq()
-        t1 = t1 * t2
-        t2 = t1.sq()
-        for _ in range(1, 5):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t2 = t1.sq()
-        for _ in range(1, 10):
-            t2 = t2.sq()
-        t2 = t2 * t1
-        t3 = t2.sq()
-        for _ in range(1, 20):
-            t3 = t3.sq()
-        t2 = t3 * t2
-        t2 = t2.sq()
-        for _ in range(1, 10):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t2 = t1.sq()
-        for _ in range(1, 50):
-            t2 = t2.sq()
-        t2 = t2 * t1
-        t3 = t2.sq()
-        for _ in range(1, 100):
-            t3 = t3.sq()
-        t2 = t3 * t2
-        t2 = t2.sq()
-        for _ in range(1, 50):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t1 = t1.sq()
-        for _ in range(1, 5):
-            t1 = t1.sq()
-        return t1 * t0
-
-    def __invert__(self: fe25519) -> fe25519:
-        """
-        Compute the multiplicative inverse of this element.
-
-        >>> two = fe25519.one() + fe25519.one()
-        >>> (((~two) * two) - fe25519.one()).is_zero()
-        1
-        """
-        return self.invert()
-
-    def __pow__(self: fe25519, e: int) -> fe25519:
-        """
-        Exponentiation is a synonym for squaring and inversion.
-
-        >>> two = fe25519.one() + fe25519.one()
-        >>> two**2 == two * two == two.sq()
-        True
-        >>> ~fe25519.one() == fe25519.one() ** (-1)
-        True
-        """
-        if e == 2: # Squaring.
-            return self.sq()
-        if e == -1: # Inversion.
-            return self.invert()
-
-        # Supplied exponent is not supported.
-        return None
-
-    def sqrt_ratio_m1_ristretto255(self: fe25519, v: fe25519) -> Tuple[fe25519, int]:
-        """
-        Compute the result of a specialized root operation.
-        """
-        u = self
-
-        v3 = v.sq()
-        v3 = v3 * v                         # v3 = v^3
-        x = v3.sq()
-        x = x * v
-        x = x * u                           # x = uv^7
-
-        x = x.pow22523()                    # x = (uv^7)^((q-5)/8)
-        x = x * v3
-        x = x * u                           # x = uv^3(uv^7)^((q-5)/8)
-
-        vxx = x.sq()
-        vxx = vxx * v                       # vx^2
-        m_root_check = vxx - u              # vx^2-u
-        p_root_check = vxx + u              # vx^2+u
-        f_root_check = u * fe25519.sqrtm1   # u*sqrt(-1)
-        f_root_check = vxx + f_root_check   # vx^2+u*sqrt(-1)
-        has_m_root = m_root_check.is_zero()
-        has_p_root = p_root_check.is_zero()
-        has_f_root = f_root_check.is_zero()
-        x_sqrtm1 = x * fe25519.sqrtm1       # x*sqrt(-1)
-
-        x = x.cmov(x_sqrtm1, has_p_root | has_f_root)
-        x = abs(x)
-
-        return (x, has_m_root | has_p_root)
-
-    def chi25519(self: fe25519) -> fe25519:
-        """
-        Compute the result of a specialized root operation (for elligator).
-        """
-        t0 = self.sq()
-        t1 = t0 * self
-        t0 = t1.sq()
-        t2 = t0.sq()
-        t2 = t2.sq()
-        t2 = t2 * t0
-        t1 = t2 * self
-        t2 = t1.sq()
-
-        for _ in range(1, 5):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t2 = t1.sq()
-        for _ in range(1, 10):
-            t2 = t2.sq()
-        t2 = t2 * t1
-        t3 = t2.sq()
-        for _ in range(1, 20):
-            t3 = t3.sq()
-        t2 = t3 * t2
-        t2 = t2.sq()
-        for _ in range(1, 10):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t2 = t1.sq()
-        for _ in range(1, 50):
-            t2 = t2.sq()
-        t2 = t2 * t1
-        t3 = t2.sq()
-        for _ in range(1, 100):
-            t3 = t3.sq()
-        t2 = t3 * t2
-        t2 = t2.sq()
-        for _ in range(1, 50):
-            t2 = t2.sq()
-        t1 = t2 * t1
-        t1 = t1.sq()
-        for _ in range(1, 4):
-            t1 = t1.sq()
-
-        return t1 * t0
-
-    def __eq__(self: fe25519, other: fe25519) -> bool:
-        """
-        Determine whether this element and another are equivalent.
-
-        >>> fe25519.zero() == fe25519.one()
-        False
-        >>> fe25519.one() == fe25519.one()
-        True
-        """
-        return self.ns == other.ns
-
-    def is_zero(self: fe25519) -> int:
-        """
-        Determine whether this element is zero.
-
-        >>> fe25519.zero().is_zero()
-        1
-        >>> fe25519.one().is_zero()
-        0
-        """
-        bs = self.to_bytes()
-        d = 0
-        for b in bs:
-            d |= b
-        return 1 & ((d - 1) >> 8)
-
-    def is_negative(self: fe25519) -> int:
-        """
-        Determine whether the negation bit is set in this element.
-
-        >>> fe25519.zero().is_negative()
-        0
-        """
-        bs = self.to_bytes()
-        return bs[0] & 1
-
-    @staticmethod
-    def from_bytes(bs: bytes) -> fe25519:
-        """
-        Assemble an element instance from its byte representation.
-
-        >>> s = '0100000000000000000000000000000000000000000000000000000000000000'
-        >>> fe25519.from_bytes(bytes.fromhex(s))
-        fe25519([1, 0, 0, 0, 0])
-        """
-        mask = 2251799813685247
-
-        def load64_le(bs):
-            w = bs[0]
-            w |= bs[1] <<  8
-            w |= bs[2] << 16
-            w |= bs[3] << 24
-            w |= bs[4] << 32
-            w |= bs[5] << 40
-            w |= bs[6] << 48
-            w |= bs[7] << 56
-            return w
-
-        return fe25519([
-            (load64_le(bs[0:8])) & mask,
-            (load64_le(bs[6:14]) >> 3) & mask,
-            (load64_le(bs[12:20]) >> 6) & mask,
-            (load64_le(bs[19:27]) >> 1) & mask,
-            (load64_le(bs[24:32]) >> 12) & mask
-        ])
-
-    def to_bytes(self: fe25519) -> bytes:
-        """
-        Build the byte representation of this element.
-
-        >>> fe25519.one().to_bytes().hex()
-        '0100000000000000000000000000000000000000000000000000000000000000'
-        """
-        t = self.reduce().ns
-
-        t0 = t[0] | ((t[1] << 51) % _TWO_TO_64)
-        t1 = (t[1] >> 13) | ((t[2] << 38) % _TWO_TO_64)
-        t2 = (t[2] >> 26) | ((t[3] << 25) % _TWO_TO_64)
-        t3 = (t[3] >> 39) | ((t[4] << 12) % _TWO_TO_64)
-
-        bs = bytearray()
-        bs.extend(t0.to_bytes(8, 'little'))
-        bs.extend(t1.to_bytes(8, 'little'))
-        bs.extend(t2.to_bytes(8, 'little'))
-        bs.extend(t3.to_bytes(8, 'little'))
-        return bytes(bs)
-
-    def __bytes__(self: fe25519) -> bytes:
-        """
-        Build the byte representation of this element.
-
-        >>> bytes(fe25519.one()).hex()
-        '0100000000000000000000000000000000000000000000000000000000000000'
-        """
-        return self.to_bytes()
-
-    def __str__(self: fe25519) -> str:
-        """
-        Obtain the string representation of an element.
-
-        >>> str(fe25519.one())
-        'fe25519([1, 0, 0, 0, 0])'
-        """
-        return 'fe25519(' + str(self.ns) + ')'
-
-    def __repr__(self: fe25519) -> str:
-        """
-        Obtain the string representation of an element.
-        """
-        return str(self) # pragma: no cover
-
-# Precomputed static constants.
-fe25519.d = fe25519([
-    929955233495203, 466365720129213, 1662059464998953, 2033849074728123, 1442794654840575
-])
-fe25519.d2 = fe25519([
-    1859910466990425, 932731440258426, 1072319116312658, 1815898335770999, 633789495995903
-])
-fe25519.sqrtm1 = fe25519([
-    1718705420411056, 234908883556509, 2233514472574048, 2117202627021982, 765476049583133
-])
-fe25519.invsqrtamd = fe25519([
-    278908739862762, 821645201101625, 8113234426968, 1777959178193151, 2118520810568447
-])
-fe25519.onemsqd = fe25519([
-    1136626929484150, 1998550399581263, 496427632559748, 118527312129759, 45110755273534
-])
-fe25519.sqdmone = fe25519([
-    1507062230895904, 1572317787530805, 683053064812840, 317374165784489, 1572899562415810
-])
-fe25519.sqrtadm1 = fe25519([
-    2241493124984347, 425987919032274, 2207028919301688, 1220490630685848, 974799131293748
-])
-fe25519.curve25519_A = fe25519([486662, 0, 0, 0, 0])
-
-if __name__ == '__main__':
-    doctest.testmod() # pragma: no cover
+"""
+Pure-Python data structure for working with Ed25519 (and Ristretto)
+field elements and operations.
+"""
+from __future__ import annotations
+from typing import Tuple, Sequence
+import doctest
+
+_TWO_TO_64 = 2 ** 64
+_TWO_TO_128 = 2 ** 128
+
+class fe25519:
+    """
+    Class for creating and operating on field elements. The public
+    interface of this class is determined primarily by the needs of
+    the `ge25519 <https://pypi.org/project/ge25519>`__ library.
+    However, use of some built-in Python operators is supported via
+    special methods.
+    """
+    # Precomputed static constants.
+    d = None
+    d2 = None
+    sqrtm1 = None
+    invsqrtamd = None
+    onemsqd = None
+    sqdmone = None
+    sqrtadm1 = None
+    curve25519_A = None
+
+    @staticmethod
+    def zero() -> fe25519:
+        """
+        Constant corresponding to the zero element.
+
+        >>> fe25519.zero() + fe25519.one() == fe25519.one()
+        True
+        """
+        return fe25519([0, 0, 0, 0, 0])
+
+    @staticmethod
+    def one() -> fe25519:
+        """
+        Constant corresponding to the multiplicative identity element.
+
+        >>> fe25519.one() * fe25519.one() == fe25519.one()
+        True
+        """
+        return fe25519([1, 0, 0, 0, 0])
+
+    def __init__(self: fe25519, ns: Sequence[int]):
+        """Create field element using a list of five 64-bit integers."""
+        self.ns = ns # pylint: disable=invalid-name
+
+    def copy(self: fe25519) -> fe25519:
+        """
+        Create a copy of this element instance.
+
+        >>> fe25519.one().copy() == fe25519.one()
+        True
+        """
+        return fe25519(list(self.ns))
+
+    def reduce(self: fe25519) -> fe25519:
+        """
+        Reduce this element to a canonical representation.
+
+        >>> (~fe25519.one()).reduce()
+        fe25519([1, 0, 0, 0, 0])
+        """
+        t = self.ns # 128-bit integers.
+        mask = 2251799813685247
+
+        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
+        t[0] &= mask
+        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
+        t[1] &= mask
+        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
+        t[2] &= mask
+        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
+        t[3] &= mask
+        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
+        t[4] &= mask
+
+        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
+        t[0] &= mask
+        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
+        t[1] &= mask
+        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
+        t[2] &= mask
+        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
+        t[3] &= mask
+        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
+        t[4] &= mask
+
+        # Now t is between 0 and 2^255-1, properly carried.
+        # Сase 1: between 0 and 2^255-20. Case 2: between 2^255-19 and 2^255-1.
+
+        t[0] = (t[0] + 19) % _TWO_TO_128
+
+        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
+        t[0] &= mask
+        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
+        t[1] &= mask
+        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
+        t[2] &= mask
+        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
+        t[3] &= mask
+        t[0] = (t[0] + 19 * (t[4] >> 51)) % _TWO_TO_128
+        t[4] &= mask
+
+        # Now between 19 and 2^255-1 in both cases, and offset by 19.
+
+        t[0] = (t[0] + 2251799813685248 - 19) % _TWO_TO_128
+        t[1] = (t[1] + 2251799813685248 - 1) % _TWO_TO_128
+        t[2] = (t[2] + 2251799813685248 - 1) % _TWO_TO_128
+        t[3] = (t[3] + 2251799813685248 - 1) % _TWO_TO_128
+        t[4] = (t[4] + 2251799813685248 - 1) % _TWO_TO_128
+
+        # Now between 2^255 and 2^256-20, and offset by 2^255.
+
+        t[1] = (t[1] + (t[0] >> 51)) % _TWO_TO_128
+        t[0] &= mask
+        t[2] = (t[2] + (t[1] >> 51)) % _TWO_TO_128
+        t[1] &= mask
+        t[3] = (t[3] + (t[2] >> 51)) % _TWO_TO_128
+        t[2] &= mask
+        t[4] = (t[4] + (t[3] >> 51)) % _TWO_TO_128
+        t[3] &= mask
+        t[4] &= mask
+
+        return fe25519(t)
+
+    def __add__(self: fe25519, other: fe25519) -> fe25519:
+        """
+        Compute the sum of this element and another element.
+
+        >>> fe25519.zero() + fe25519.zero() == fe25519.zero()
+        True
+        """
+        return fe25519([(m+n)%_TWO_TO_64 for (m, n) in zip(self.ns, other.ns)])
+
+    def __neg__(self: fe25519) -> fe25519:
+        """
+        Compute the negation of this element.
+
+        >>> fe25519.one().cneg(1) != fe25519.one()
+        True
+        """
+        return fe25519.zero() - self
+
+    def cmov(self: fe25519, g: fe25519, b: int) -> fe25519:
+        """Conditionally select this element or another based on a boolean integer."""
+        mask = _TWO_TO_64 - b
+        pairs = zip(self.ns, g.ns)
+        return fe25519([fi ^ ((fi ^ gi) & mask) for (fi, gi) in pairs])
+
+    def cneg(self: fe25519, b: int) -> fe25519:
+        """
+        Compute the conditional negation of this element.
+
+        >>> fe25519.one().cneg(0) == fe25519.one()
+        True
+        >>> (fe25519.one().cneg(1) + fe25519.one()).is_zero()
+        1
+        """
+        return self.copy().cmov(-self, b)
+
+    def __abs__(self: fe25519) -> fe25519:
+        """
+        Compute the absolute value of this element.
+
+        >>> abs(-fe25519.one()).is_negative()
+        0
+        """
+        return self.cneg(self.is_negative())
+
+    def __sub__(self: fe25519, other: fe25519) -> fe25519:
+        """
+        Compute the result of subtracting another element from this element.
+
+        >>> fe25519.zero() - fe25519.one() == fe25519.one().cneg(1)
+        True
+        """
+        mask = 2251799813685247
+
+        (h0, h1, h2, h3, h4) = other.ns
+
+        h1 = (h1 + (h0 >> 51)) % _TWO_TO_64
+        h0 &= mask
+        h2 = (h2 + (h1 >> 51)) % _TWO_TO_64
+        h1 &= mask
+        h3 = (h3 + (h2 >> 51)) % _TWO_TO_64
+        h2 &= mask
+        h4 = (h4 + (h3 >> 51)) % _TWO_TO_64
+        h3 &= mask
+        h0 = (h0 + 19 * (h4 >> 51)) % _TWO_TO_64
+        h4 &= mask
+
+        return fe25519([
+            ((self.ns[0] + 4503599627370458) - h0) % _TWO_TO_64,
+            ((self.ns[1] + 4503599627370494) - h1) % _TWO_TO_64,
+            ((self.ns[2] + 4503599627370494) - h2) % _TWO_TO_64,
+            ((self.ns[3] + 4503599627370494) - h3) % _TWO_TO_64,
+            ((self.ns[4] + 4503599627370494) - h4) % _TWO_TO_64
+        ])
+
+    def __mul__(self: fe25519, other: fe25519) -> fe25519:
+        """
+        Compute the product of this element and another element.
+
+        >>> fe25519.one() * fe25519.zero() == fe25519.zero()
+        True
+        """
+        mask = 2251799813685247 # 64-bit integer.
+        (f, g) = (self.ns, other.ns) # 64-bit integers.
+        r = [None, None, None, None, None] # 128-bit integers.
+        carry = None # 128-bit integer.
+        r0 = [None, None, None, None, None] # 64-bit integers.
+
+        f1_19 = (19 * f[1]) % _TWO_TO_64
+        f2_19 = (19 * f[2]) % _TWO_TO_64
+        f3_19 = (19 * f[3]) % _TWO_TO_64
+        f4_19 = (19 * f[4]) % _TWO_TO_64
+
+        r[0] = (f[0]*g[0] + f1_19*g[4] + f2_19*g[3] + f3_19*g[2] + f4_19*g[1]) % _TWO_TO_128
+        r[1] = (f[0]*g[1] + f[1]*g[0] + f2_19*g[4] + f3_19*g[3] + f4_19*g[2]) % _TWO_TO_128
+        r[2] = (f[0]*g[2] + f[1]*g[1] + f[2]*g[0] + f3_19*g[4] + f4_19*g[3]) % _TWO_TO_128
+        r[3] = (f[0]*g[3] + f[1]*g[2] + f[2]*g[1] + f[3]*g[0] + f4_19*g[4]) % _TWO_TO_128
+        r[4] = (f[0]*g[4] + f[1]*g[3] + f[2]*g[2] + f[3]*g[1] + f[4]*g[0]) % _TWO_TO_128
+
+        r0[0] = (r[0] % _TWO_TO_64) & mask
+        r[1] = (r[1] + (r[0] >> 51)) % _TWO_TO_128
+        r0[1] = (r[1] % _TWO_TO_64) & mask
+        r[2] = (r[2] + (r[1] >> 51)) % _TWO_TO_128
+        r0[2] = (r[2] % _TWO_TO_64) & mask
+        r[3] = (r[3] + (r[2] >> 51)) % _TWO_TO_128
+        r0[3] = (r[3] % _TWO_TO_64) & mask
+        r[4] = (r[4] + (r[3] >> 51)) % _TWO_TO_128
+        r0[4] = (r[4] % _TWO_TO_64) & mask
+        r0[0] = (r0[0] + (19*((r[4] >> 51) % _TWO_TO_64))) % _TWO_TO_64
+        carry = r0[0] >> 51
+        r0[0] &= mask
+        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
+        carry = r0[1] >> 51
+        r0[1] &= mask
+        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
+
+        return fe25519(r0)
+
+    def sq(self: fe25519) -> fe25519: # pylint: disable=invalid-name
+        """
+        Compute the square of this element.
+
+        >>> two = fe25519.one() + fe25519.one()
+        >>> four = two + two
+        >>> two.sq() == four
+        True
+        """
+        mask = 2251799813685247 # 64-bit integer.
+        f = self.ns # 64-bit integers.
+        r = [None, None, None, None, None] # 128-bit integers.
+        carry = None # 128-bit integer.
+        r0 = [None, None, None, None, None] # 64-bit integers.
+
+        f0_2 = (f[0] << 1) % _TWO_TO_64
+        f1_2 = (f[1] << 1) % _TWO_TO_64
+
+        f1_38 = (38 * f[1]) % _TWO_TO_64
+        f2_38 = (38 * f[2]) % _TWO_TO_64
+        f3_38 = (38 * f[3]) % _TWO_TO_64
+
+        f3_19 = (19 * f[3]) % _TWO_TO_64
+        f4_19 = (19 * f[4]) % _TWO_TO_64
+
+        r[0] = (f[0]*f[0] + f1_38*f[4] + f2_38*f[3]) % _TWO_TO_128
+        r[1] = (f0_2*f[1] + f2_38*f[4] + f3_19*f[3]) % _TWO_TO_128
+        r[2] = (f0_2*f[2] + f[1]*f[1] + f3_38*f[4]) % _TWO_TO_128
+        r[3] = (f0_2*f[3] + f1_2*f[2] + f4_19*f[4]) % _TWO_TO_128
+        r[4] = (f0_2*f[4] + f1_2*f[3] + f[2]*f[2]) % _TWO_TO_128
+
+        r0[0] = (r[0] % _TWO_TO_64) & mask
+        r[1] = (r[1] + (r[0] >> 51)) % _TWO_TO_128
+        r0[1] = (r[1] % _TWO_TO_64) & mask
+        r[2] = (r[2] + (r[1] >> 51)) % _TWO_TO_128
+        r0[2] = (r[2] % _TWO_TO_64) & mask
+        r[3] = (r[3] + (r[2] >> 51)) % _TWO_TO_128
+        r0[3] = (r[3] % _TWO_TO_64) & mask
+        r[4] = (r[4] + (r[3] >> 51)) % _TWO_TO_128
+        r0[4] = (r[4] % _TWO_TO_64) & mask
+        r0[0] = (r0[0] + (19*((r[4] >> 51) % _TWO_TO_64))) % _TWO_TO_64
+        carry = r0[0] >> 51
+        r0[0] &= mask
+        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
+        carry = r0[1] >> 51
+        r0[1] &= mask
+        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
+
+        return fe25519(r0)
+
+    def sq2(self: fe25519) -> fe25519:
+        """
+        Compute the element that is twice the square of this element.
+
+        >>> two = fe25519.one() + fe25519.one()
+        >>> two.sq2() == two.sq() + two.sq()
+        True
+        """
+        mask = 2251799813685247
+        f = self.ns # 64-bit integers.
+        r = [None, None, None, None, None] # 128-bit integers.
+        carry = None # 128-bit integer.
+        r0 = [None, None, None, None, None] # 64-bit integers.
+
+        f0_2 = (f[0] << 1) % _TWO_TO_64
+        f1_2 = (f[1] << 1) % _TWO_TO_64
+
+        f1_38 = (38 * f[1]) % _TWO_TO_64
+        f2_38 = (38 * f[2]) % _TWO_TO_64
+        f3_38 = (38 * f[3]) % _TWO_TO_64
+
+        f3_19 = (19 * f[3]) % _TWO_TO_64
+        f4_19 = (19 * f[4]) % _TWO_TO_64
+
+        r[0] = (f[0]*f[0] + f1_38*f[4] + f2_38*f[3]) % _TWO_TO_128
+        r[1] = (f0_2*f[1] + f2_38*f[4] + f3_19*f[3]) % _TWO_TO_128
+        r[2] = (f0_2*f[2] + f[1]*f[1] + f3_38*f[4]) % _TWO_TO_128
+        r[3] = (f0_2*f[3] + f1_2*f[2] + f4_19*f[4]) % _TWO_TO_128
+        r[4] = (f0_2*f[4] + f1_2*f[3] + f[2]*f[2]) % _TWO_TO_128
+
+        r[0] <<= 1
+        r[1] <<= 1
+        r[2] <<= 1
+        r[3] <<= 1
+        r[4] <<= 1
+
+        r0[0] = (r[0] % _TWO_TO_64) & mask
+        carry = r[0] >> 51
+        r[1] = (r[1] + carry) % _TWO_TO_128
+        r0[1] = (r[1] % _TWO_TO_64) & mask
+        carry = r[1] >> 51
+        r[2] = (r[2] + carry) % _TWO_TO_128
+
+        r0[2] = (r[2] % _TWO_TO_64) & mask
+        carry = r[2] >> 51
+        r[3] = (r[3] + carry) % _TWO_TO_128
+        r0[3] = (r[3] % _TWO_TO_64) & mask
+        carry = r[3] >> 51
+        r[4] = (r[4] + carry) % _TWO_TO_128
+        r0[4] = (r[4] % _TWO_TO_64) & mask
+        carry = r[4] >> 51
+        r0[0] = (r0[0] + 19*carry) % _TWO_TO_64
+        carry = r0[0] >> 51
+        r0[0] &= mask
+        r0[1] = (r0[1] + (carry % _TWO_TO_64)) % _TWO_TO_64
+        carry = r0[1] >> 51
+        r0[1] &= mask
+        r0[2] = (r0[2] + (carry % _TWO_TO_64)) % _TWO_TO_64
+
+        return fe25519(r0)
+
+    def pow22523(self: fe25519) -> fe25519:
+        """
+        Compute the result of the exponentiation of this element by a
+        special fixed exponent.
+        """
+        z = self.copy()
+        t0 = z.sq()
+        t1 = t0.sq()
+        t1 = t1.sq()
+        t1 = z * t1
+        t0 = t0 * t1
+        t0 = t0.sq()
+        t0 = t1 * t0
+        t1 = t0.sq()
+        for _ in range(1, 5):
+            t1 = t1.sq()
+        t0 = t1 * t0
+        t1 = t0.sq()
+        for _ in range(1, 10):
+            t1 = t1.sq()
+        t1 = t1 * t0
+        t2 = t1.sq()
+        for _ in range(1, 20):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t1 = t1.sq()
+        for _ in range(1, 10):
+            t1 = t1.sq()
+        t0 = t1 * t0
+        t1 = t0.sq()
+        for _ in range(1, 50):
+            t1 = t1.sq()
+        t1 = t1 * t0
+        t2 = t1.sq()
+        for _ in range(1, 100):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t1 = t1.sq()
+        for _ in range(1, 50):
+            t1 = t1.sq()
+        t0 = t1 * t0
+        t0 = t0.sq()
+        t0 = t0.sq()
+        return t0 * z
+
+    def invert(self: fe25519) -> fe25519:
+        """
+        Compute the multiplicative inverse of this element.
+
+        >>> two = fe25519.one() + fe25519.one()
+        >>> (two.invert() * two).reduce() == fe25519.one()
+        True
+        """
+        z = self.copy()
+        t0 = z.sq()
+        t1 = t0.sq()
+        t1 = t1.sq()
+        t1 = z * t1
+        t0 = t0 * t1
+        t2 = t0.sq()
+        t1 = t1 * t2
+        t2 = t1.sq()
+        for _ in range(1, 5):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t2 = t1.sq()
+        for _ in range(1, 10):
+            t2 = t2.sq()
+        t2 = t2 * t1
+        t3 = t2.sq()
+        for _ in range(1, 20):
+            t3 = t3.sq()
+        t2 = t3 * t2
+        t2 = t2.sq()
+        for _ in range(1, 10):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t2 = t1.sq()
+        for _ in range(1, 50):
+            t2 = t2.sq()
+        t2 = t2 * t1
+        t3 = t2.sq()
+        for _ in range(1, 100):
+            t3 = t3.sq()
+        t2 = t3 * t2
+        t2 = t2.sq()
+        for _ in range(1, 50):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t1 = t1.sq()
+        for _ in range(1, 5):
+            t1 = t1.sq()
+        return t1 * t0
+
+    def __invert__(self: fe25519) -> fe25519:
+        """
+        Compute the multiplicative inverse of this element.
+
+        >>> two = fe25519.one() + fe25519.one()
+        >>> (((~two) * two) - fe25519.one()).is_zero()
+        1
+        """
+        return self.invert()
+
+    def __pow__(self: fe25519, e: int) -> fe25519:
+        """
+        Exponentiation is a synonym for squaring and inversion.
+
+        >>> two = fe25519.one() + fe25519.one()
+        >>> two**2 == two * two == two.sq()
+        True
+        >>> ~fe25519.one() == fe25519.one() ** (-1)
+        True
+        """
+        if e == 2: # Squaring.
+            return self.sq()
+        if e == -1: # Inversion.
+            return self.invert()
+
+        # Supplied exponent is not supported.
+        return None
+
+    def sqrt_ratio_m1_ristretto255(self: fe25519, v: fe25519) -> Tuple[fe25519, int]:
+        """
+        Compute the result of a specialized root operation.
+        """
+        u = self
+
+        v3 = v.sq()
+        v3 = v3 * v                         # v3 = v^3
+        x = v3.sq()
+        x = x * v
+        x = x * u                           # x = uv^7
+
+        x = x.pow22523()                    # x = (uv^7)^((q-5)/8)
+        x = x * v3
+        x = x * u                           # x = uv^3(uv^7)^((q-5)/8)
+
+        vxx = x.sq()
+        vxx = vxx * v                       # vx^2
+        m_root_check = vxx - u              # vx^2-u
+        p_root_check = vxx + u              # vx^2+u
+        f_root_check = u * fe25519.sqrtm1   # u*sqrt(-1)
+        f_root_check = vxx + f_root_check   # vx^2+u*sqrt(-1)
+        has_m_root = m_root_check.is_zero()
+        has_p_root = p_root_check.is_zero()
+        has_f_root = f_root_check.is_zero()
+        x_sqrtm1 = x * fe25519.sqrtm1       # x*sqrt(-1)
+
+        x = x.cmov(x_sqrtm1, has_p_root | has_f_root)
+        x = abs(x)
+
+        return (x, has_m_root | has_p_root)
+
+    def chi25519(self: fe25519) -> fe25519:
+        """
+        Compute the result of a specialized root operation (for elligator).
+        """
+        t0 = self.sq()
+        t1 = t0 * self
+        t0 = t1.sq()
+        t2 = t0.sq()
+        t2 = t2.sq()
+        t2 = t2 * t0
+        t1 = t2 * self
+        t2 = t1.sq()
+
+        for _ in range(1, 5):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t2 = t1.sq()
+        for _ in range(1, 10):
+            t2 = t2.sq()
+        t2 = t2 * t1
+        t3 = t2.sq()
+        for _ in range(1, 20):
+            t3 = t3.sq()
+        t2 = t3 * t2
+        t2 = t2.sq()
+        for _ in range(1, 10):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t2 = t1.sq()
+        for _ in range(1, 50):
+            t2 = t2.sq()
+        t2 = t2 * t1
+        t3 = t2.sq()
+        for _ in range(1, 100):
+            t3 = t3.sq()
+        t2 = t3 * t2
+        t2 = t2.sq()
+        for _ in range(1, 50):
+            t2 = t2.sq()
+        t1 = t2 * t1
+        t1 = t1.sq()
+        for _ in range(1, 4):
+            t1 = t1.sq()
+
+        return t1 * t0
+
+    def __eq__(self: fe25519, other: fe25519) -> bool:
+        """
+        Determine whether this element and another are equivalent.
+
+        >>> fe25519.zero() == fe25519.one()
+        False
+        >>> fe25519.one() == fe25519.one()
+        True
+        """
+        return self.ns == other.ns
+
+    def is_zero(self: fe25519) -> int:
+        """
+        Determine whether this element is zero.
+
+        >>> fe25519.zero().is_zero()
+        1
+        >>> fe25519.one().is_zero()
+        0
+        """
+        bs = self.to_bytes()
+        d = 0
+        for b in bs:
+            d |= b
+        return 1 & ((d - 1) >> 8)
+
+    def is_negative(self: fe25519) -> int:
+        """
+        Determine whether the negation bit is set in this element.
+
+        >>> fe25519.zero().is_negative()
+        0
+        """
+        bs = self.to_bytes()
+        return bs[0] & 1
+
+    @staticmethod
+    def from_bytes(bs: bytes) -> fe25519:
+        """
+        Assemble an element instance from its byte representation.
+
+        >>> s = '0100000000000000000000000000000000000000000000000000000000000000'
+        >>> fe25519.from_bytes(bytes.fromhex(s))
+        fe25519([1, 0, 0, 0, 0])
+        """
+        mask = 2251799813685247
+
+        def load64_le(bs):
+            w = bs[0]
+            w |= bs[1] <<  8
+            w |= bs[2] << 16
+            w |= bs[3] << 24
+            w |= bs[4] << 32
+            w |= bs[5] << 40
+            w |= bs[6] << 48
+            w |= bs[7] << 56
+            return w
+
+        return fe25519([
+            (load64_le(bs[0:8])) & mask,
+            (load64_le(bs[6:14]) >> 3) & mask,
+            (load64_le(bs[12:20]) >> 6) & mask,
+            (load64_le(bs[19:27]) >> 1) & mask,
+            (load64_le(bs[24:32]) >> 12) & mask
+        ])
+
+    def to_bytes(self: fe25519) -> bytes:
+        """
+        Build the byte representation of this element.
+
+        >>> fe25519.one().to_bytes().hex()
+        '0100000000000000000000000000000000000000000000000000000000000000'
+        """
+        t = self.reduce().ns
+
+        t0 = t[0] | ((t[1] << 51) % _TWO_TO_64)
+        t1 = (t[1] >> 13) | ((t[2] << 38) % _TWO_TO_64)
+        t2 = (t[2] >> 26) | ((t[3] << 25) % _TWO_TO_64)
+        t3 = (t[3] >> 39) | ((t[4] << 12) % _TWO_TO_64)
+
+        bs = bytearray()
+        bs.extend(t0.to_bytes(8, 'little'))
+        bs.extend(t1.to_bytes(8, 'little'))
+        bs.extend(t2.to_bytes(8, 'little'))
+        bs.extend(t3.to_bytes(8, 'little'))
+        return bytes(bs)
+
+    def __bytes__(self: fe25519) -> bytes:
+        """
+        Build the byte representation of this element.
+
+        >>> bytes(fe25519.one()).hex()
+        '0100000000000000000000000000000000000000000000000000000000000000'
+        """
+        return self.to_bytes()
+
+    def __str__(self: fe25519) -> str:
+        """
+        Obtain the string representation of an element.
+
+        >>> str(fe25519.one())
+        'fe25519([1, 0, 0, 0, 0])'
+        """
+        return 'fe25519(' + str(self.ns) + ')'
+
+    def __repr__(self: fe25519) -> str:
+        """
+        Obtain the string representation of an element.
+        """
+        return str(self) # pragma: no cover
+
+# Precomputed static constants.
+fe25519.d = fe25519([
+    929955233495203, 466365720129213, 1662059464998953, 2033849074728123, 1442794654840575
+])
+fe25519.d2 = fe25519([
+    1859910466990425, 932731440258426, 1072319116312658, 1815898335770999, 633789495995903
+])
+fe25519.sqrtm1 = fe25519([
+    1718705420411056, 234908883556509, 2233514472574048, 2117202627021982, 765476049583133
+])
+fe25519.invsqrtamd = fe25519([
+    278908739862762, 821645201101625, 8113234426968, 1777959178193151, 2118520810568447
+])
+fe25519.onemsqd = fe25519([
+    1136626929484150, 1998550399581263, 496427632559748, 118527312129759, 45110755273534
+])
+fe25519.sqdmone = fe25519([
+    1507062230895904, 1572317787530805, 683053064812840, 317374165784489, 1572899562415810
+])
+fe25519.sqrtadm1 = fe25519([
+    2241493124984347, 425987919032274, 2207028919301688, 1220490630685848, 974799131293748
+])
+fe25519.curve25519_A = fe25519([486662, 0, 0, 0, 0])
+
+if __name__ == '__main__':
+    doctest.testmod() # pragma: no cover
```

### Comparing `fe25519-1.3.0/src/fe25519.egg-info/PKG-INFO` & `fe25519-1.4.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,120 @@
-Metadata-Version: 2.1
-Name: fe25519
-Version: 1.3.0
-Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/fe25519
-Project-URL: Documentation, https://fe25519.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=======
-fe25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
-   :target: https://badge.fury.io/py/fe25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
-   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__::
-
-    python -m pip install fe25519
-
-The library can be imported in the usual ways::
-
-    import fe25519
-    from fe25519 import fe25519
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
-Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly::
-
-    python test/test_fe25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/fe25519 test/test_fe25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+=======
+fe25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) field elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/fe25519.svg
+   :target: https://badge.fury.io/py/fe25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/fe25519/badge/?version=latest
+   :target: https://fe25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/fe25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/fe25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/fe25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/fe25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ field elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto field elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/fe25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install fe25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import fe25519
+    from fe25519 import fe25519
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
+Concise unit tests are implemented with the help of `fountains <https://pypi.org/project/fountains>`__; new reference specifications for these tests can be generated by running the testing module directly:
+
+.. code-block:: bash
+
+    python test/test_fe25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/fe25519 test/test_fe25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/fe25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/fe25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `fe25519-1.3.0/test/test_fe25519.py` & `fe25519-1.4.0/test/test_fe25519.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-"""
-Test suite containing functional unit tests for the exported primitives and
-classes.
-"""
-from __future__ import annotations
-from typing import Tuple, Union, Optional, Callable, Iterable
-from unittest import TestCase
-from parts import parts
-from bitlist import bitlist
-from fountains import fountains
-
-from fe25519.fe25519 import fe25519
-
-def one_from_bytes(bs: bytes) -> fe25519:
-    """
-    Generate one element from a given bit sequence obtained
-    using :obj:`fountains`.
-    """
-    ps = list(parts(bs, length=8))
-    return fe25519([int.from_bytes(p, 'little') for p in ps])
-
-def two_from_bytes(bs: bytes) -> Tuple[fe25519, fe25519]:
-    """
-    Generate two elements from a given bit sequence obtained
-    using :obj:`fountains`.
-    """
-    ps = list(parts(bs, length=8))
-    f1 = fe25519([int.from_bytes(p, 'little') for p in ps[:5]])
-    f2 = fe25519([int.from_bytes(p, 'little') for p in ps[5:]])
-    return (f1, f2)
-
-def check_or_generate(
-        testcase: TestCase,
-        fs: Union[Iterable[int], Iterable[bool]],
-        bits: Optional[str]
-    ) -> Optional[str]:
-    """
-    Wrapper that enables switching between performing a test or
-    generating specifications compatible with :obj:`fountains`.
-    """
-    if bits is None:
-        return bitlist(list(fs)).hex() # Return target bits for this test.
-
-    testcase.assertTrue(all(fs)) # Check that all tests succeeded.
-    return None # Do not return a test input.
-
-def check_or_generate_operation(
-        testcase: TestCase,
-        fun: Union[Callable[[bytes], bytes], Callable[[bytes], bitlist]],
-        arity: int,
-        bits: Optional[str]
-    ) -> Optional[str]:
-    """
-    Wrapper that enables switching between performing a test or
-    generating specifications compatible with :obj:`fountains`.
-    """
-    fs = fountains(
-        8 * 5 * arity,
-        seed=bytes(0), # This is also the default; explicit for clarity.
-        limit=256,
-        bits=bits,
-        function=fun
-    )
-    return check_or_generate(testcase, fs, bits)
-
-class Test_fe25519(TestCase):
-    """
-    Tests for all class methods.
-    """
-    # pylint: disable=too-many-public-methods,missing-function-docstring
-    def test_one(
-            self,
-            bits='b71ee55494c10540b2d3c4221793de6c6c722100387cab827ae1522affb5fd66'
-        ):
-        fun = lambda bs: (one_from_bytes(bs) * fe25519.one()).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_reduce(
-            self,
-            bits='b71ee55494c10540b2d3c4221793de6c6c722100387cab827ae1522affb5fd66'
-        ):
-        fun = lambda bs: (one_from_bytes(bs).reduce()).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_add(
-            self,
-            bits='397e060905e137528ecc8421702c17535eda8d56683a018167d6f319f45a8234'
-        ):
-        def fun(bs):
-            (f1, f2) = two_from_bytes(bs)
-            return (f1 + f2).to_bytes()
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_neg(
-            self,
-            bits='7ee11aab6b3efabf4d2c3bdde86c2193938ddeffc783547d851eadd5004a0219'
-        ):
-        fun = lambda bs: (-one_from_bytes(bs)).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_abs(
-            self,
-            bits='fe4c4c172782fc006c73f6cc09ade2f4b82d57c562bea9887c2c525886a1ef17'
-        ):
-        fun = lambda bs: (abs(one_from_bytes(bs))).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_sub(
-            self,
-            bits='70989bdb9b7f9ac91dcf56f3175efd39952d96f1a53c597f41dc0f59aa936d34'
-        ):
-        def fun(bs):
-            (f1, f2) = two_from_bytes(bs)
-            return (f1 - f2).to_bytes()
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_mul(
-            self,
-            bits='90a408821c55fd4e09213b390698021f2ae37265053d086be45c3bceffefe27b'
-        ):
-        def fun(bs):
-            (f1, f2) = two_from_bytes(bs)
-            return (f1 * f2).to_bytes()
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_sq(
-            self,
-            bits='8a7c83d71aacf24fcd76e5d24fa4d9fc7f6ee0e56333305ed8c4ae69565af95a'
-        ):
-        fun = lambda bs: (one_from_bytes(bs)**2).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_sq2(
-            self,
-            bits='69730f8c46dea00aa3377189a87c07277a6be1d3efec442b5c11a99fdd67f230'
-        ):
-        fun = lambda bs: (one_from_bytes(bs).sq2()).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_pow22523(
-            self,
-            bits='4601cde640c8e05a4e63df3edc2a9d472851072b6b361eaaebcf781c0a116150'
-        ):
-        fun = lambda bs: (one_from_bytes(bs).pow22523()).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_invert(
-            self,
-            bits='f103890f12e1533aee66007a2a7b051a8e9f378fded8291bb0110a95ac55d059'
-        ):
-        fun = lambda bs: (one_from_bytes(bs)**(-1)).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_invert_op(
-            self,
-            bits='f103890f12e1533aee66007a2a7b051a8e9f378fded8291bb0110a95ac55d059'
-        ):
-        fun = lambda bs: (~one_from_bytes(bs)).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_sqrt_ratio_m1_ristretto255(
-            self,
-            bits='e08f25034216acaf3d92d080192fa7ec1585693caa6931a84b4261100c071d08'
-        ):
-        def fun(bs):
-            (f1, f2) = two_from_bytes(bs)
-            return f1.sqrt_ratio_m1_ristretto255(f2)[0].to_bytes()
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_chi25519(
-            self,
-            bits='64a9f0ae1ce3dda09b86ff4d1ca0fcf31bad8f65f3ce025b6debdb20abefc85a'
-        ):
-        fun = lambda bs: (one_from_bytes(bs).chi25519()).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_eq_true(
-            self,
-            bits='0101010101010101010101010101010101010101010101010101010101010101'
-        ):
-        def fun(bs):
-            f0 = one_from_bytes(bs)
-            return bytes([f0 == f0]) # pylint: disable=comparison-with-itself
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_eq_false(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        def fun(bs):
-            (f1, f2) = two_from_bytes(bs)
-            return bytes([f1 == f2])
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_is_zero(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        fun = lambda bs: bitlist([one_from_bytes(bs).is_zero()])
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_is_negative(
-            self,
-            bits='5d52a943b343f940dea032ee1e3e3c98d45f76c55ac2020a06cd007279141271'
-        ):
-        fun = lambda bs: bitlist([one_from_bytes(bs).is_negative()])
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_cmov(
-            self,
-            bits='01da9d156e3e03043adaad53bcf8af55150ef319da198f44d6c8df44ca5fb324'
-        ):
-        def fun(bs):
-            ((f1, f2), b) = (two_from_bytes(bs), bs[0] % 2)
-            return f1.cmov(f2, b).to_bytes()
-        return check_or_generate_operation(self, fun, 2, bits)
-
-    def test_pow(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        fun = lambda bs: bitlist([0 if one_from_bytes(bs)**(0) is None else 255]).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_str(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        def fun(bs):
-            f = one_from_bytes(bs)
-            return bitlist([
-                0 if eval(str(f)) == f else 255 # pylint: disable=eval-used
-            ]).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_bytes(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        def fun(bs):
-            f = one_from_bytes(bs)
-            return bitlist([0 if fe25519.from_bytes(f.to_bytes()) == f else 255]).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-    def test_bytes_op(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        def fun(bs):
-            f = one_from_bytes(bs)
-            return bitlist([0 if fe25519.from_bytes(bytes(f)) == f else 255]).to_bytes()
-        return check_or_generate_operation(self, fun, 1, bits)
-
-if __name__ == '__main__':
-    # Generate specifications for tests.
-    test_fe25519 = Test_fe25519()
-    for m in [m for m in dir(test_fe25519) if m.startswith('test_')]:
-        print(m + ': ' + getattr(test_fe25519, m)(bits=None))
+"""
+Test suite containing functional unit tests for the exported primitives and
+classes.
+"""
+from __future__ import annotations
+from typing import Tuple, Union, Optional, Callable, Iterable
+from unittest import TestCase
+from parts import parts
+from bitlist import bitlist
+from fountains import fountains
+
+from fe25519.fe25519 import fe25519
+
+def one_from_bytes(bs: bytes) -> fe25519:
+    """
+    Generate one element from a given bit sequence obtained
+    using :obj:`fountains`.
+    """
+    ps = list(parts(bs, length=8))
+    return fe25519([int.from_bytes(p, 'little') for p in ps])
+
+def two_from_bytes(bs: bytes) -> Tuple[fe25519, fe25519]:
+    """
+    Generate two elements from a given bit sequence obtained
+    using :obj:`fountains`.
+    """
+    ps = list(parts(bs, length=8))
+    f1 = fe25519([int.from_bytes(p, 'little') for p in ps[:5]])
+    f2 = fe25519([int.from_bytes(p, 'little') for p in ps[5:]])
+    return (f1, f2)
+
+def check_or_generate(
+        testcase: TestCase,
+        fs: Union[Iterable[int], Iterable[bool]],
+        bits: Optional[str]
+    ) -> Optional[str]:
+    """
+    Wrapper that enables switching between performing a test or
+    generating specifications compatible with :obj:`fountains`.
+    """
+    if bits is None:
+        return bitlist(list(fs)).hex() # Return target bits for this test.
+
+    testcase.assertTrue(all(fs)) # Check that all tests succeeded.
+    return None # Do not return a test input.
+
+def check_or_generate_operation(
+        testcase: TestCase,
+        fun: Union[Callable[[bytes], bytes], Callable[[bytes], bitlist]],
+        arity: int,
+        bits: Optional[str]
+    ) -> Optional[str]:
+    """
+    Wrapper that enables switching between performing a test or
+    generating specifications compatible with :obj:`fountains`.
+    """
+    fs = fountains(
+        8 * 5 * arity,
+        seed=bytes(0), # This is also the default; explicit for clarity.
+        limit=256,
+        bits=bits,
+        function=fun
+    )
+    return check_or_generate(testcase, fs, bits)
+
+class Test_fe25519(TestCase):
+    """
+    Tests for all class methods.
+    """
+    # pylint: disable=too-many-public-methods,missing-function-docstring
+    def test_one(
+            self,
+            bits='b71ee55494c10540b2d3c4221793de6c6c722100387cab827ae1522affb5fd66'
+        ):
+        fun = lambda bs: (one_from_bytes(bs) * fe25519.one()).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_reduce(
+            self,
+            bits='b71ee55494c10540b2d3c4221793de6c6c722100387cab827ae1522affb5fd66'
+        ):
+        fun = lambda bs: (one_from_bytes(bs).reduce()).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_add(
+            self,
+            bits='397e060905e137528ecc8421702c17535eda8d56683a018167d6f319f45a8234'
+        ):
+        def fun(bs):
+            (f1, f2) = two_from_bytes(bs)
+            return (f1 + f2).to_bytes()
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_neg(
+            self,
+            bits='7ee11aab6b3efabf4d2c3bdde86c2193938ddeffc783547d851eadd5004a0219'
+        ):
+        fun = lambda bs: (-one_from_bytes(bs)).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_abs(
+            self,
+            bits='fe4c4c172782fc006c73f6cc09ade2f4b82d57c562bea9887c2c525886a1ef17'
+        ):
+        fun = lambda bs: (abs(one_from_bytes(bs))).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_sub(
+            self,
+            bits='70989bdb9b7f9ac91dcf56f3175efd39952d96f1a53c597f41dc0f59aa936d34'
+        ):
+        def fun(bs):
+            (f1, f2) = two_from_bytes(bs)
+            return (f1 - f2).to_bytes()
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_mul(
+            self,
+            bits='90a408821c55fd4e09213b390698021f2ae37265053d086be45c3bceffefe27b'
+        ):
+        def fun(bs):
+            (f1, f2) = two_from_bytes(bs)
+            return (f1 * f2).to_bytes()
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_sq(
+            self,
+            bits='8a7c83d71aacf24fcd76e5d24fa4d9fc7f6ee0e56333305ed8c4ae69565af95a'
+        ):
+        fun = lambda bs: (one_from_bytes(bs)**2).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_sq2(
+            self,
+            bits='69730f8c46dea00aa3377189a87c07277a6be1d3efec442b5c11a99fdd67f230'
+        ):
+        fun = lambda bs: (one_from_bytes(bs).sq2()).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_pow22523(
+            self,
+            bits='4601cde640c8e05a4e63df3edc2a9d472851072b6b361eaaebcf781c0a116150'
+        ):
+        fun = lambda bs: (one_from_bytes(bs).pow22523()).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_invert(
+            self,
+            bits='f103890f12e1533aee66007a2a7b051a8e9f378fded8291bb0110a95ac55d059'
+        ):
+        fun = lambda bs: (one_from_bytes(bs)**(-1)).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_invert_op(
+            self,
+            bits='f103890f12e1533aee66007a2a7b051a8e9f378fded8291bb0110a95ac55d059'
+        ):
+        fun = lambda bs: (~one_from_bytes(bs)).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_sqrt_ratio_m1_ristretto255(
+            self,
+            bits='e08f25034216acaf3d92d080192fa7ec1585693caa6931a84b4261100c071d08'
+        ):
+        def fun(bs):
+            (f1, f2) = two_from_bytes(bs)
+            return f1.sqrt_ratio_m1_ristretto255(f2)[0].to_bytes()
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_chi25519(
+            self,
+            bits='64a9f0ae1ce3dda09b86ff4d1ca0fcf31bad8f65f3ce025b6debdb20abefc85a'
+        ):
+        fun = lambda bs: (one_from_bytes(bs).chi25519()).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_eq_true(
+            self,
+            bits='0101010101010101010101010101010101010101010101010101010101010101'
+        ):
+        def fun(bs):
+            f0 = one_from_bytes(bs)
+            return bytes([f0 == f0]) # pylint: disable=comparison-with-itself
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_eq_false(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        def fun(bs):
+            (f1, f2) = two_from_bytes(bs)
+            return bytes([f1 == f2])
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_is_zero(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        fun = lambda bs: bitlist([one_from_bytes(bs).is_zero()])
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_is_negative(
+            self,
+            bits='5d52a943b343f940dea032ee1e3e3c98d45f76c55ac2020a06cd007279141271'
+        ):
+        fun = lambda bs: bitlist([one_from_bytes(bs).is_negative()])
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_cmov(
+            self,
+            bits='01da9d156e3e03043adaad53bcf8af55150ef319da198f44d6c8df44ca5fb324'
+        ):
+        def fun(bs):
+            ((f1, f2), b) = (two_from_bytes(bs), bs[0] % 2)
+            return f1.cmov(f2, b).to_bytes()
+        return check_or_generate_operation(self, fun, 2, bits)
+
+    def test_pow(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        fun = lambda bs: bitlist([0 if one_from_bytes(bs)**(0) is None else 255]).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_str(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        def fun(bs):
+            f = one_from_bytes(bs)
+            return bitlist([
+                0 if eval(str(f)) == f else 255 # pylint: disable=eval-used
+            ]).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_bytes(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        def fun(bs):
+            f = one_from_bytes(bs)
+            return bitlist([0 if fe25519.from_bytes(f.to_bytes()) == f else 255]).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+    def test_bytes_op(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        def fun(bs):
+            f = one_from_bytes(bs)
+            return bitlist([0 if fe25519.from_bytes(bytes(f)) == f else 255]).to_bytes()
+        return check_or_generate_operation(self, fun, 1, bits)
+
+if __name__ == '__main__':
+    # Generate specifications for tests.
+    test_fe25519 = Test_fe25519()
+    for m in [m for m in dir(test_fe25519) if m.startswith('test_')]:
+        print(m + ': ' + getattr(test_fe25519, m)(bits=None))
```

