# Comparing `tmp/ge25519-1.3.0.tar.gz` & `tmp/ge25519-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ge25519-1.3.0.tar", last modified: Mon Aug  8 15:29:46 2022, max compression
+gzip compressed data, was "ge25519-1.4.0.tar", last modified: Tue Apr 25 18:56:13 2023, max compression
```

## Comparing `ge25519-1.3.0.tar` & `ge25519-1.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-08-08 15:29:46.565024 ge25519-1.3.0/
--rw-rw-rw-   0        0        0     1093 2022-03-13 02:08:29.000000 ge25519-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     5672 2022-08-08 15:29:46.565024 ge25519-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5118 2022-07-17 09:23:54.000000 ge25519-1.3.0/README.rst
--rw-rw-rw-   0        0        0     1087 2022-08-07 20:12:35.000000 ge25519-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-08 15:29:46.567025 ge25519-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-08 15:29:46.550059 ge25519-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-08 15:29:46.552085 ge25519-1.3.0/src/ge25519/
--rw-rw-rw-   0        0        0      171 2022-03-13 02:08:29.000000 ge25519-1.3.0/src/ge25519/__init__.py
--rw-rw-rw-   0        0        0   123790 2022-07-31 06:17:04.000000 ge25519-1.3.0/src/ge25519/ge25519.py
-drwxrwxrwx   0        0        0        0 2022-08-08 15:29:46.562241 ge25519-1.3.0/src/ge25519.egg-info/
--rw-rw-rw-   0        0        0     5672 2022-08-08 15:29:46.000000 ge25519-1.3.0/src/ge25519.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2022-08-08 15:29:46.000000 ge25519-1.3.0/src/ge25519.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-08 15:29:46.000000 ge25519-1.3.0/src/ge25519.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      233 2022-08-08 15:29:46.000000 ge25519-1.3.0/src/ge25519.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-08 15:29:46.000000 ge25519-1.3.0/src/ge25519.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-08-08 15:29:46.562479 ge25519-1.3.0/test/
--rw-rw-rw-   0        0        0     8818 2022-08-08 15:24:36.000000 ge25519-1.3.0/test/test_ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103663 ge25519-1.4.0/
+-rw-r--r--   0 alapets    (502) staff       (20)     1072 2023-04-25 14:57:02.000000 ge25519-1.4.0/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-25 18:56:13.103733 ge25519-1.4.0/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5258 2023-04-15 14:00:02.000000 ge25519-1.4.0/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)     1034 2023-04-15 13:58:43.000000 ge25519-1.4.0/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-25 18:56:13.103947 ge25519-1.4.0/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.100913 ge25519-1.4.0/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.102225 ge25519-1.4.0/src/ge25519/
+-rw-r--r--   0 alapets    (502) staff       (20)      166 2023-04-25 14:57:02.000000 ge25519-1.4.0/src/ge25519/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)   121618 2023-04-25 14:57:02.000000 ge25519-1.4.0/src/ge25519/ge25519.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103363 ge25519-1.4.0/src/ge25519.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     5794 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      285 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      234 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        8 2023-04-25 18:56:13.000000 ge25519-1.4.0/src/ge25519.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:56:13.103497 ge25519-1.4.0/test/
+-rw-r--r--   0 alapets    (502) staff       (20)     8605 2023-04-25 14:57:02.000000 ge25519-1.4.0/test/test_ge25519.py
```

### Comparing `ge25519-1.3.0/LICENSE` & `ge25519-1.4.0/LICENSE`

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

### Comparing `ge25519-1.3.0/PKG-INFO` & `ge25519-1.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,138 @@
-Metadata-Version: 2.1
-Name: ge25519
-Version: 1.3.0
-Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/ge25519
-Project-URL: Documentation, https://ge25519.readthedocs.io
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
-ge25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
-   :target: https://badge.fury.io/py/ge25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
-   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-PInstallation and Usage
------------------------
-This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__::
-
-    python -m pip install ge25519
-
-The library can be imported in the usual ways::
-
-    import ge25519
-    from ge25519 import *
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
-    python test/test_ge25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/ge25519 test/test_ge25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: ge25519
+Version: 1.4.0
+Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/ge25519
+Project-URL: Documentation, https://ge25519.readthedocs.io
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
+ge25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
+   :target: https://badge.fury.io/py/ge25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
+   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+PInstallation and Usage
+-----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install ge25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import ge25519
+    from ge25519 import *
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
+    python test/test_ge25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/ge25519 test/test_ge25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `ge25519-1.3.0/README.rst` & `ge25519-1.4.0/src/ge25519.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,138 @@
-=======
-ge25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
-   :target: https://badge.fury.io/py/ge25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
-   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-PInstallation and Usage
------------------------
-This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__::
-
-    python -m pip install ge25519
-
-The library can be imported in the usual ways::
-
-    import ge25519
-    from ge25519 import *
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
-    python test/test_ge25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/ge25519 test/test_ge25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: ge25519
+Version: 1.4.0
+Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/nthparty/ge25519
+Project-URL: Documentation, https://ge25519.readthedocs.io
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
+ge25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
+   :target: https://badge.fury.io/py/ge25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
+   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+PInstallation and Usage
+-----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install ge25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import ge25519
+    from ge25519 import *
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
+    python test/test_ge25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/ge25519 test/test_ge25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `ge25519-1.3.0/src/ge25519.egg-info/PKG-INFO` & `ge25519-1.4.0/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,116 +1,120 @@
-Metadata-Version: 2.1
-Name: ge25519
-Version: 1.3.0
-Summary: Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/nthparty/ge25519
-Project-URL: Documentation, https://ge25519.readthedocs.io
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
-ge25519
-=======
-
-Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
-   :target: https://badge.fury.io/py/ge25519
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
-   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
-   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
-
-The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
-
-PInstallation and Usage
------------------------
-This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__::
-
-    python -m pip install ge25519
-
-The library can be imported in the usual ways::
-
-    import ge25519
-    from ge25519 import *
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
-    python test/test_ge25519.py
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/ge25519 test/test_ge25519.py
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+ge25519
+=======
+
+Pure-Python data structure for working with Ed25519 (and Ristretto) group elements and operations.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/ge25519.svg
+   :target: https://badge.fury.io/py/ge25519
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/ge25519/badge/?version=latest
+   :target: https://ge25519.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/nthparty/ge25519/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/nthparty/ge25519/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/nthparty/ge25519/badge.svg?branch=main
+   :target: https://coveralls.io/github/nthparty/ge25519?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a native Python implementation of `Ed25519 <https://ed25519.cr.yp.to>`__ group elements and a number of operations over them. The library makes it possible to fill gaps in application prototypes that may have specific limitations with respect to their operating environment or their ability to rely on non-Python dependencies.
+
+The implementation is based upon and is compatible with the corresponding implementation of Ed25519 and Ristretto group elements used in `libsodium <https://github.com/jedisct1/libsodium>`__. For more information and background about the underlying mathematical structures and primitives, consult materials about `Curve25519 <https://cr.yp.to/ecdh.html>`__, the `Ristretto <https://ristretto.group>`__ group, and the related `Ed25519 <https://ed25519.cr.yp.to>`__ system.
+
+PInstallation and Usage
+-----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/ge25519>`__:
+
+.. code-block:: bash
+
+    python -m pip install ge25519
+
+The library can be imported in the usual ways:
+
+.. code-block:: python
+
+    import ge25519
+    from ge25519 import *
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
+    python test/test_ge25519.py
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/ge25519 test/test_ge25519.py
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/nthparty/ge25519>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.1.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/ge25519>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `ge25519-1.3.0/test/test_ge25519.py` & `ge25519-1.4.0/test/test_ge25519.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-"""
-Test suite containing functional unit tests for the exported primitives and
-classes.
-"""
-# pylint: disable=missing-function-docstring
-from __future__ import annotations
-from typing import Union, Optional, Callable, Iterable
-from unittest import TestCase
-from parts import parts
-from bitlist import bitlist
-from fountains import fountains
-
-from ge25519.ge25519 import * # pylint: disable=wildcard-import,unused-wildcard-import
-
-# Constant for the number of input-output pairs to include in each test.
-TRIALS_PER_TEST = 256
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
-        lengths: Iterable[int],
-        bits: Optional[str]
-    ):
-    """
-    Wrapper that enables switching between performing a test or
-    generating specifications compatible with :obj:`fountains`.
-    """
-    fs = fountains( # Generate the input bit stream.
-        sum(lengths),
-        seed=bytes(0), # This is also the default; explicit for clarity.
-        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
-        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
-        function=fun
-    )
-    return check_or_generate(testcase, fs, bits)
-
-class Test_ge25519(TestCase):
-    """
-    Tests for all class methods.
-    """
-    def test_is_canonical(
-            self,
-            bits='ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff'
-        ):
-        def fun(bs):
-            return bitlist([ge25519.is_canonical(bs)])
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_has_small_order(
-            self,
-            bits='0000000000000000000000000000000000000000000000000000000000000000'
-        ):
-        def fun(bs):
-            return bitlist([ge25519.has_small_order(bs)])
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_is_on_curve(
-            self,
-            bits='4dbd939e58fc59860feac3f1e63fa428519472415073f2ca850b662c25bbd05b'
-        ):
-        def fun(bs):
-            return bitlist([ge25519_p3.from_bytes(bs).is_on_curve()])
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_is_on_main_subgroup(
-            self,
-            bits='4020000200040800090081804410040010003000000110028100040824020010'
-        ):
-        def fun(bs):
-            return bitlist([ge25519_p3.from_bytes(bs).is_on_main_subgroup()])
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_from_p3(
-            self,
-            bits='37b1cbf6ef16f5a00e5470ecc6b4c93b20893bb308962300b2081e8aa7e8702a'
-        ):
-        def fun(bs):
-            p1p1 = ge25519_p2.from_p3(ge25519_p3.from_bytes(bs)).dbl()
-            return ge25519_p3.from_p1p1(p1p1).to_bytes()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_dbl(self, bits='37b1cbf6ef16f5a00e5470ecc6b4c93b20893bb308962300b2081e8aa7e8702a'):
-        def fun(bs):
-            p1p1 = ge25519_p1p1.dbl(ge25519_p3.from_bytes(bs))
-            return ge25519_p3.from_p1p1(p1p1).to_bytes()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_mul_l(
-            self,
-            bits='22b0eb2b1d06d970c1dba41540d9255228625c871e2c4d1655c784167f43b104'
-        ):
-        fun = lambda bs: ge25519_p3.from_bytes(bs).mul_l().to_bytes()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_scalar_mult_base(
-            self,
-            bits='ec909cfc24cf1721d21dda8b350dafc277f29470ea03b5560e19d47f9e668f09'
-        ):
-        def fun(bs):
-            return ge25519_p3.scalar_mult_base(bs).to_bytes()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_scalar_mult(
-            self,
-            bits='242fd0294a256e12f5a82955d223baeab5a04b7db5f9d46552f34b08a858e9a8'
-        ):
-        def fun(bs):
-            (bs1, bs2) = parts(bs, length=32)
-            return ge25519_p3.from_bytes(bs1).scalar_mult(bs2).to_bytes()
-        return check_or_generate_operation(self, fun, [32, 32], bits)
-
-    def test_from_uniform(
-            self,
-            bits='fa3b6f0f3a7222b45d44ac42eb03f7beec0039f61f0814a4f3a2f178e44fd26d'
-        ):
-        fun = lambda bs: ge25519_p3.from_uniform(bs).to_bytes()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_from_hash_ristretto255(
-            self,
-            bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
-        ):
-        return check_or_generate_operation(self, ge25519_p3.from_hash_ristretto255, [64], bits)
-
-    def test_from_bytes_ristretto255(
-            self,
-            bits='80200300300085008000260000000800008a006000800c041040800420130182'
-        ):
-        def fun(bs):
-            p3 = ge25519_p3.from_bytes_ristretto255(bs)
-            return p3.to_bytes() if p3 is not None else bitlist([0])
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_to_bytes_ristretto255(
-            self,
-            bits='4240c56beef1f9d6b8dfe7856fbae94999b8bc5e27b350f01ee5db7ee2b5ad45'
-        ):
-        fun = lambda bs: ge25519_p3.from_bytes(bs).to_bytes_ristretto255()
-        return check_or_generate_operation(self, fun, [32], bits)
-
-    def test_add(self, bits='f9a298467cf064593c9998917f3e2b1fb00f738e92e3c3187ce9986b70389245'):
-        def fun(bs):
-            (bs1, bs2) = parts(bs, length=32)
-            p3 = ge25519_p3.from_bytes(bs1)
-            cached = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
-            return ge25519_p3.from_p1p1((ge25519_p1p1.add(p3, cached))).to_bytes()
-        return check_or_generate_operation(self, fun, [32, 32], bits)
-
-    def test_madd(self, bits='4b4d0b3a86c787f295d53e4a42656ba2ba6123f14a819b3c2d544f574d0030bb'):
-        def fun(bs):
-            (p3, i, j) = (ge25519_p3.from_bytes(bs[:32]), bs[32]%32, (bs[32]//32)%8)
-            # pylint: disable=protected-access,unsubscriptable-object
-            p2 = ge25519_p2.from_p1p1(ge25519_p1p1.madd(p3, ge25519_precomp._base[i][j]))
-            return ge25519_p3.from_p1p1(p2.dbl()).to_bytes()
-        return check_or_generate_operation(self, fun, [32, 1], bits)
-
-    def test_sub(self, bits='c349d67e124af7943ee8ceeaf774c43fca0472c245dad7e52585c62e71343082'):
-        def fun(bs):
-            (bs1, bs2) = parts(bs, length=32)
-            p3 = ge25519_p3.from_bytes(bs1)
-            cached = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
-            return ge25519_p3.from_p1p1((ge25519_p1p1.sub(p3, cached))).to_bytes()
-        return check_or_generate_operation(self, fun, [32, 32], bits)
-
-    def test_cmov8_base(
-            self,
-            bits='450fa303840940b93e104413b952865464b0fffc8321b030ac956537029bf61e'
-        ):
-        def fun(bs):
-            (pos, b) = (bs[0] % 32, (bs[0] // 32) % 8)
-            precomp = ge25519_precomp._cmov8_base(pos, b) # pylint: disable=protected-access
-            return \
-                precomp.yplusx.to_bytes() + \
-                precomp.yminusx.to_bytes() + \
-                precomp.xy2d.to_bytes()
-        return check_or_generate_operation(self, fun, [1], bits)
-
-    def test_cmov_cached(
-            self,
-            bits='2c81a643db31e92474c23b47d5a568fab19b90385855fccbe53fbfcd3ac32e45'
-        ):
-        def fun(bs):
-            ((bs1, bs2), b) = (parts(bs, length=32), bs[-1]%2)
-            cached1 = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs1))
-            cached2 = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
-            cached1._cmov_cached(cached2, b) # pylint: disable=protected-access
-            return \
-                cached1.YplusX.to_bytes() + \
-                cached1.YminusX.to_bytes() + \
-                cached1.Z.to_bytes() + \
-                cached1.T2d.to_bytes()
-        return check_or_generate_operation(self, fun, [32, 32], bits)
-
-if __name__ == '__main__':
-    # Generate specifications for tests.
-    test_ge25519 = Test_ge25519()
-    for m in [m for m in dir(test_ge25519) if m.startswith('test_')]:
-        print(m + ': ' + getattr(test_ge25519, m)(bits=None))
+"""
+Test suite containing functional unit tests for the exported primitives and
+classes.
+"""
+# pylint: disable=missing-function-docstring
+from __future__ import annotations
+from typing import Union, Optional, Callable, Iterable
+from unittest import TestCase
+from parts import parts
+from bitlist import bitlist
+from fountains import fountains
+
+from ge25519.ge25519 import * # pylint: disable=wildcard-import,unused-wildcard-import
+
+# Constant for the number of input-output pairs to include in each test.
+TRIALS_PER_TEST = 256
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
+        lengths: Iterable[int],
+        bits: Optional[str]
+    ):
+    """
+    Wrapper that enables switching between performing a test or
+    generating specifications compatible with :obj:`fountains`.
+    """
+    fs = fountains( # Generate the input bit stream.
+        sum(lengths),
+        seed=bytes(0), # This is also the default; explicit for clarity.
+        limit=min(TRIALS_PER_TEST, (len(bits) * 4) if bits is not None else 256),
+        bits=bits[:(TRIALS_PER_TEST // 4)] if bits is not None else None,
+        function=fun
+    )
+    return check_or_generate(testcase, fs, bits)
+
+class Test_ge25519(TestCase):
+    """
+    Tests for all class methods.
+    """
+    def test_is_canonical(
+            self,
+            bits='ffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffffff'
+        ):
+        def fun(bs):
+            return bitlist([ge25519.is_canonical(bs)])
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_has_small_order(
+            self,
+            bits='0000000000000000000000000000000000000000000000000000000000000000'
+        ):
+        def fun(bs):
+            return bitlist([ge25519.has_small_order(bs)])
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_is_on_curve(
+            self,
+            bits='4dbd939e58fc59860feac3f1e63fa428519472415073f2ca850b662c25bbd05b'
+        ):
+        def fun(bs):
+            return bitlist([ge25519_p3.from_bytes(bs).is_on_curve()])
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_is_on_main_subgroup(
+            self,
+            bits='4020000200040800090081804410040010003000000110028100040824020010'
+        ):
+        def fun(bs):
+            return bitlist([ge25519_p3.from_bytes(bs).is_on_main_subgroup()])
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_from_p3(
+            self,
+            bits='37b1cbf6ef16f5a00e5470ecc6b4c93b20893bb308962300b2081e8aa7e8702a'
+        ):
+        def fun(bs):
+            p1p1 = ge25519_p2.from_p3(ge25519_p3.from_bytes(bs)).dbl()
+            return ge25519_p3.from_p1p1(p1p1).to_bytes()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_dbl(self, bits='37b1cbf6ef16f5a00e5470ecc6b4c93b20893bb308962300b2081e8aa7e8702a'):
+        def fun(bs):
+            p1p1 = ge25519_p1p1.dbl(ge25519_p3.from_bytes(bs))
+            return ge25519_p3.from_p1p1(p1p1).to_bytes()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_mul_l(
+            self,
+            bits='22b0eb2b1d06d970c1dba41540d9255228625c871e2c4d1655c784167f43b104'
+        ):
+        fun = lambda bs: ge25519_p3.from_bytes(bs).mul_l().to_bytes()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_scalar_mult_base(
+            self,
+            bits='ec909cfc24cf1721d21dda8b350dafc277f29470ea03b5560e19d47f9e668f09'
+        ):
+        def fun(bs):
+            return ge25519_p3.scalar_mult_base(bs).to_bytes()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_scalar_mult(
+            self,
+            bits='242fd0294a256e12f5a82955d223baeab5a04b7db5f9d46552f34b08a858e9a8'
+        ):
+        def fun(bs):
+            (bs1, bs2) = parts(bs, length=32)
+            return ge25519_p3.from_bytes(bs1).scalar_mult(bs2).to_bytes()
+        return check_or_generate_operation(self, fun, [32, 32], bits)
+
+    def test_from_uniform(
+            self,
+            bits='fa3b6f0f3a7222b45d44ac42eb03f7beec0039f61f0814a4f3a2f178e44fd26d'
+        ):
+        fun = lambda bs: ge25519_p3.from_uniform(bs).to_bytes()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_from_hash_ristretto255(
+            self,
+            bits='baf12de24e54deae0aa116816bf5eee23b1168c78e892372e08a9884de9d4c1b'
+        ):
+        return check_or_generate_operation(self, ge25519_p3.from_hash_ristretto255, [64], bits)
+
+    def test_from_bytes_ristretto255(
+            self,
+            bits='80200300300085008000260000000800008a006000800c041040800420130182'
+        ):
+        def fun(bs):
+            p3 = ge25519_p3.from_bytes_ristretto255(bs)
+            return p3.to_bytes() if p3 is not None else bitlist([0])
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_to_bytes_ristretto255(
+            self,
+            bits='4240c56beef1f9d6b8dfe7856fbae94999b8bc5e27b350f01ee5db7ee2b5ad45'
+        ):
+        fun = lambda bs: ge25519_p3.from_bytes(bs).to_bytes_ristretto255()
+        return check_or_generate_operation(self, fun, [32], bits)
+
+    def test_add(self, bits='f9a298467cf064593c9998917f3e2b1fb00f738e92e3c3187ce9986b70389245'):
+        def fun(bs):
+            (bs1, bs2) = parts(bs, length=32)
+            p3 = ge25519_p3.from_bytes(bs1)
+            cached = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
+            return ge25519_p3.from_p1p1((ge25519_p1p1.add(p3, cached))).to_bytes()
+        return check_or_generate_operation(self, fun, [32, 32], bits)
+
+    def test_madd(self, bits='4b4d0b3a86c787f295d53e4a42656ba2ba6123f14a819b3c2d544f574d0030bb'):
+        def fun(bs):
+            (p3, i, j) = (ge25519_p3.from_bytes(bs[:32]), bs[32]%32, (bs[32]//32)%8)
+            # pylint: disable=protected-access,unsubscriptable-object
+            p2 = ge25519_p2.from_p1p1(ge25519_p1p1.madd(p3, ge25519_precomp._base[i][j]))
+            return ge25519_p3.from_p1p1(p2.dbl()).to_bytes()
+        return check_or_generate_operation(self, fun, [32, 1], bits)
+
+    def test_sub(self, bits='c349d67e124af7943ee8ceeaf774c43fca0472c245dad7e52585c62e71343082'):
+        def fun(bs):
+            (bs1, bs2) = parts(bs, length=32)
+            p3 = ge25519_p3.from_bytes(bs1)
+            cached = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
+            return ge25519_p3.from_p1p1((ge25519_p1p1.sub(p3, cached))).to_bytes()
+        return check_or_generate_operation(self, fun, [32, 32], bits)
+
+    def test_cmov8_base(
+            self,
+            bits='450fa303840940b93e104413b952865464b0fffc8321b030ac956537029bf61e'
+        ):
+        def fun(bs):
+            (pos, b) = (bs[0] % 32, (bs[0] // 32) % 8)
+            precomp = ge25519_precomp._cmov8_base(pos, b) # pylint: disable=protected-access
+            return \
+                precomp.yplusx.to_bytes() + \
+                precomp.yminusx.to_bytes() + \
+                precomp.xy2d.to_bytes()
+        return check_or_generate_operation(self, fun, [1], bits)
+
+    def test_cmov_cached(
+            self,
+            bits='2c81a643db31e92474c23b47d5a568fab19b90385855fccbe53fbfcd3ac32e45'
+        ):
+        def fun(bs):
+            ((bs1, bs2), b) = (parts(bs, length=32), bs[-1]%2)
+            cached1 = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs1))
+            cached2 = ge25519_cached.from_p3(ge25519_p3.from_bytes(bs2))
+            cached1._cmov_cached(cached2, b) # pylint: disable=protected-access
+            return \
+                cached1.YplusX.to_bytes() + \
+                cached1.YminusX.to_bytes() + \
+                cached1.Z.to_bytes() + \
+                cached1.T2d.to_bytes()
+        return check_or_generate_operation(self, fun, [32, 32], bits)
+
+if __name__ == '__main__':
+    # Generate specifications for tests.
+    test_ge25519 = Test_ge25519()
+    for m in [m for m in dir(test_ge25519) if m.startswith('test_')]:
+        print(m + ': ' + getattr(test_ge25519, m)(bits=None))
```

