# Comparing `tmp/parts-1.5.2.tar.gz` & `tmp/parts-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parts-1.5.2.tar", last modified: Mon Aug  1 07:02:00 2022, max compression
+gzip compressed data, was "parts-1.6.0.tar", last modified: Tue Apr 25 18:47:54 2023, max compression
```

## Comparing `parts-1.5.2.tar` & `parts-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 07:02:00.280562 parts-1.5.2/
--rw-rw-rw-   0        0        0     1091 2022-03-12 17:59:35.000000 parts-1.5.2/LICENSE
--rw-rw-rw-   0        0        0     6379 2022-08-01 07:02:00.280562 parts-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     5849 2022-07-24 20:26:02.000000 parts-1.5.2/README.rst
--rw-rw-rw-   0        0        0      998 2022-08-01 06:51:18.000000 parts-1.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-08-01 07:02:00.280819 parts-1.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-01 07:02:00.271856 parts-1.5.2/src/
-drwxrwxrwx   0        0        0        0 2022-08-01 07:02:00.274637 parts-1.5.2/src/parts/
--rw-rw-rw-   0        0        0       81 2022-03-12 17:59:35.000000 parts-1.5.2/src/parts/__init__.py
--rw-rw-rw-   0        0        0    18273 2022-08-01 06:54:31.000000 parts-1.5.2/src/parts/parts.py
-drwxrwxrwx   0        0        0        0 2022-08-01 07:02:00.279364 parts-1.5.2/src/parts.egg-info/
--rw-rw-rw-   0        0        0     6379 2022-08-01 07:02:00.000000 parts-1.5.2/src/parts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2022-08-01 07:02:00.000000 parts-1.5.2/src/parts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 07:02:00.000000 parts-1.5.2/src/parts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      214 2022-08-01 07:02:00.000000 parts-1.5.2/src/parts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-08-01 07:02:00.000000 parts-1.5.2/src/parts.egg-info/top_level.txt
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:47:54.748040 parts-1.6.0/
+-rw-r--r--   0 alapets    (502) staff       (20)     1070 2023-04-07 14:37:50.000000 parts-1.6.0/LICENSE
+-rw-r--r--   0 alapets    (502) staff       (20)     6454 2023-04-25 18:47:54.747899 parts-1.6.0/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)     5942 2023-04-25 14:22:00.000000 parts-1.6.0/README.rst
+-rw-r--r--   0 alapets    (502) staff       (20)      950 2023-04-25 14:18:43.000000 parts-1.6.0/pyproject.toml
+-rw-r--r--   0 alapets    (502) staff       (20)       38 2023-04-25 18:47:54.748084 parts-1.6.0/setup.cfg
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:47:54.745961 parts-1.6.0/src/
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:47:54.746842 parts-1.6.0/src/parts/
+-rw-r--r--   0 alapets    (502) staff       (20)       79 2023-04-07 14:37:50.000000 parts-1.6.0/src/parts/__init__.py
+-rw-r--r--   0 alapets    (502) staff       (20)    17815 2023-04-07 14:37:50.000000 parts-1.6.0/src/parts/parts.py
+drwxr-xr-x   0 alapets    (502) staff       (20)        0 2023-04-25 18:47:54.747698 parts-1.6.0/src/parts.egg-info/
+-rw-r--r--   0 alapets    (502) staff       (20)     6454 2023-04-25 18:47:54.000000 parts-1.6.0/src/parts.egg-info/PKG-INFO
+-rw-r--r--   0 alapets    (502) staff       (20)      238 2023-04-25 18:47:54.000000 parts-1.6.0/src/parts.egg-info/SOURCES.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        1 2023-04-25 18:47:54.000000 parts-1.6.0/src/parts.egg-info/dependency_links.txt
+-rw-r--r--   0 alapets    (502) staff       (20)      215 2023-04-25 18:47:54.000000 parts-1.6.0/src/parts.egg-info/requires.txt
+-rw-r--r--   0 alapets    (502) staff       (20)        6 2023-04-25 18:47:54.000000 parts-1.6.0/src/parts.egg-info/top_level.txt
```

### Comparing `parts-1.5.2/PKG-INFO` & `parts-1.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,174 @@
-Metadata-Version: 2.1
-Name: parts
-Version: 1.5.2
-Summary: Minimal library that enables partitioning of iterable objects in a concise manner.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/parts
-Project-URL: Documentation, https://parts.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=====
-parts
-=====
-
-Minimal library that enables partitioning of iterable objects in a concise manner.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/parts.svg
-   :target: https://badge.fury.io/py/parts
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
-   :target: https://parts.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
-   :target: https://coveralls.io/github/lapets/parts?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/parts>`__::
-
-    python -m pip install parts
-
-The library can be imported in the usual manner::
-
-    import parts
-    from parts import parts
-
-Examples
-^^^^^^^^
-Several examples are presented below::
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
-    [[1, 2], [3, 4], [5, 6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
-    [[1, 2, 3, 4], [5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
-    [[1, 2, 3, 4, 5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
-    [[1], [2], [3], [4, 5], [6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
-    [[1, 2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
-    [[1], [2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
-    Traceback (most recent call last):
-      ...
-    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
-    python src/parts/parts.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/parts
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: parts
+Version: 1.6.0
+Summary: Minimal library that enables partitioning of iterable objects in a concise manner.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/parts
+Project-URL: Documentation, https://parts.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=====
+parts
+=====
+
+Minimal library that enables partitioning of iterable objects in a concise manner.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/parts.svg
+   :target: https://badge.fury.io/py/parts
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
+   :target: https://parts.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
+   :target: https://coveralls.io/github/lapets/parts?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/parts>`__:
+
+.. code-block:: bash
+
+    python -m pip install parts
+
+The library can be imported in the usual manner:
+
+.. code-block:: python
+
+    import parts
+    from parts import parts
+
+Examples
+^^^^^^^^
+Several examples are presented below:
+
+.. code-block:: python
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
+    [[1, 2], [3, 4], [5, 6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
+    [[1, 2, 3, 4], [5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
+    [[1, 2, 3, 4, 5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
+    [[1], [2], [3], [4, 5], [6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
+    [[1, 2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
+    [[1], [2], [3], [4], [5], [6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
+    [[1], [2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
+    Traceback (most recent call last):
+      ...
+    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
+    python src/parts/parts.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/parts
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `parts-1.5.2/README.rst` & `parts-1.6.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,132 +1,156 @@
-=====
-parts
-=====
-
-Minimal library that enables partitioning of iterable objects in a concise manner.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/parts.svg
-   :target: https://badge.fury.io/py/parts
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
-   :target: https://parts.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
-   :target: https://coveralls.io/github/lapets/parts?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/parts>`__::
-
-    python -m pip install parts
-
-The library can be imported in the usual manner::
-
-    import parts
-    from parts import parts
-
-Examples
-^^^^^^^^
-Several examples are presented below::
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
-    [[1, 2], [3, 4], [5, 6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
-    [[1, 2, 3, 4], [5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
-    [[1, 2, 3, 4, 5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
-    [[1], [2], [3], [4, 5], [6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
-    [[1, 2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
-    [[1], [2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
-    Traceback (most recent call last):
-      ...
-    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
-    python src/parts/parts.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/parts
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+=====
+parts
+=====
+
+Minimal library that enables partitioning of iterable objects in a concise manner.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/parts.svg
+   :target: https://badge.fury.io/py/parts
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
+   :target: https://parts.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
+   :target: https://coveralls.io/github/lapets/parts?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/parts>`__:
+
+.. code-block:: bash
+
+    python -m pip install parts
+
+The library can be imported in the usual manner:
+
+.. code-block:: python
+
+    import parts
+    from parts import parts
+
+Examples
+^^^^^^^^
+Several examples are presented below:
+
+.. code-block:: python
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
+    [[1, 2], [3, 4], [5, 6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
+    [[1, 2, 3, 4], [5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
+    [[1, 2, 3, 4, 5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
+    [[1], [2], [3], [4, 5], [6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
+    [[1, 2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
+    [[1], [2], [3], [4], [5], [6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
+    [[1], [2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
+    Traceback (most recent call last):
+      ...
+    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
+    python src/parts/parts.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/parts
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

### Comparing `parts-1.5.2/src/parts/parts.py` & `parts-1.6.0/src/parts/parts.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,458 +1,458 @@
-"""
-Minimal library that enables partitioning of iterable objects in a concise
-manner.
-"""
-import doctest
-from typing import Tuple, Union, Optional, Iterable
-import collections.abc
-from itertools import islice, chain
-
-def _empty(xs: Iterable) -> Tuple[Iterable, bool]:
-    """
-    Determine whether a sequential type instance is empty.
-
-    >>> def error():
-    ...     for i in range(2):
-    ...         if i == 0:
-    ...             yield i
-    ...         else:
-    ...             raise RuntimeError('error in generator')
-    ...
-    >>> list(parts(error(), length=1))
-    Traceback (most recent call last):
-      ...
-    RuntimeError: error in generator
-    """
-    try:
-        return (xs, len(xs) == 0)
-    except TypeError:
-        try:
-            x = next(xs)
-            return (iter(chain([x], xs)), False)
-        except StopIteration:
-            return (xs, True)
-        except Exception as e:
-            raise e from None
-
-def _slice(xs: Iterable, lower: int, upper: int) -> Iterable:
-    """
-    Attempt to retrieve a subsequence of a sequential type instance
-    using slice notation or :obj:`itertools.islice`.
-    """
-    try:
-        return xs[lower: min(len(xs), upper)]
-    except TypeError:
-        try:
-            return islice(xs, 0, upper - lower)
-        except:
-            raise TypeError(
-                'object does not support retrieval of slices'
-            ) from None
-
-def parts(
-        xs: Iterable,
-        number: Optional[int] = None,
-        length: Union[int, Iterable[int], None] = None
-    ) -> Iterable:
-    """
-    This function splits an :obj:`~collections.abc.Iterable` object into either
-    the specified number of parts or a number of parts each of the specified
-    length. When input parameters lead to ambiguous or conflicting constraints,
-    either elements are distributed in a best-effort manner or an exception is
-    raised (depending on the specific scenario).
-
-    :param xs: Iterable to split into parts.
-    :param number: Number of parts.
-    :param length: Length of every part or iterable of part lengths.
-
-    In the simplest case, the target number of parts can be specified.
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 1))
-    [[1, 2, 3, 4, 5, 6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 2))
-    [[1, 2, 3], [4, 5, 6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 3))
-    [[1, 2], [3, 4], [5, 6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 4))
-    [[1], [2, 3], [4, 5], [6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
-    [[1], [2], [3], [4, 5], [6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 6))
-    [[1], [2], [3], [4], [5], [6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7))
-    [[1], [2], [3], [4], [5], [6], [7]]
-
-    The target length for each part can be specified; the number of parts will
-    be determined based on the length and the available number of items.
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=1))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
-    [[1, 2], [3, 4], [5, 6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=3))
-    [[1, 2, 3], [4, 5, 6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
-    [[1, 2, 3, 4], [5, 6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=5))
-    [[1, 2, 3, 4, 5], [6, 7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=6))
-    [[1, 2, 3, 4, 5, 6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=7))
-    [[1, 2, 3, 4, 5, 6, 7]]
-    >>> list(map(list, parts(iter([1, 2, 3, 4, 5, 6, 7]), length=4)))
-    [[1, 2, 3, 4], [5, 6, 7]]
-
-    An iterable of length values can be specified. The entry at each position
-    in the iterable of lengths dictates the length of the part in the
-    corresponding position in the output.
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=[1, 1, 1, 1, 1, 1, 1]))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
-    [[1, 2], [3, 4], [5, 6]]
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
-    [[1], [2, 3], [4, 5, 6]]
-
-    The type of input objects (for built-in types) is preserved in the output.
-
-    >>> isinstance(next(parts([1, 2, 3, 4, 5], length=2)), list)
-    True
-    >>> isinstance(next(parts([1, 2, 3, 4, 5], length=[2, 2, 1])), list)
-    True
-    >>> isinstance(next(parts([1, 2, 3, 4, 5], number=2)), list)
-    True
-    >>> isinstance(next(parts([1, 2, 3, 4], number=2, length=2)), list)
-    True
-    >>> isinstance(next(parts([1, 2, 3, 4], number=2, length=[2, 2])), list)
-    True
-    >>> isinstance(next(parts((1, 2, 3, 4, 5), length=2)), tuple)
-    True
-    >>> isinstance(next(parts((1, 2, 3, 4, 5), length=[2, 2, 1])), tuple)
-    True
-    >>> isinstance(next(parts((1, 2, 3, 4, 5), number=2)), tuple)
-    True
-    >>> isinstance(next(parts((1, 2, 3, 4), number=2, length=2)), tuple)
-    True
-    >>> isinstance(next(parts((1, 2, 3, 4), number=2, length=[2, 2])), tuple)
-    True
-    >>> isinstance(next(parts('abc', length=2)), str)
-    True
-    >>> isinstance(next(parts('abc', length=[2, 1])), str)
-    True
-    >>> isinstance(next(parts('abc', number=2)), str)
-    True
-    >>> isinstance(next(parts('abcd', number=2, length=2)), str)
-    True
-    >>> isinstance(next(parts('abcd', number=2, length=[2, 2])), str)
-    True
-    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), length=2)), bytes)
-    True
-    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), length=[2, 2, 1])), bytes)
-    True
-    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), number=2)), bytes)
-    True
-    >>> isinstance(next(parts(bytes([1, 2, 3, 4]), number=2, length=2)), bytes)
-    True
-    >>> isinstance(next(parts(bytes([1, 2, 3, 4]), number=2, length=[2, 2])), bytes)
-    True
-    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), length=2)), bytearray)
-    True
-    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), length=[2, 2, 1])), bytearray)
-    True
-    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), number=2)), bytearray)
-    True
-    >>> isinstance(next(parts(bytearray([1, 2, 3, 4]), number=2, length=2)), bytearray)
-    True
-    >>> isinstance(next(parts(bytearray([1, 2, 3, 4]), number=2, length=[2, 2])), bytearray)
-    True
-    >>> isinstance(next(parts(range(0, 10), length=2)), range)
-    True
-    >>> isinstance(next(parts(range(0, 5), length=[2, 2, 1])), range)
-    True
-    >>> isinstance(next(parts(range(0, 10), number=2)), range)
-    True
-    >>> isinstance(next(parts(range(0, 4), number=2, length=2)), range)
-    True
-    >>> isinstance(next(parts(range(0, 4), number=2, length=[2, 2])), range)
-    True
-    >>> isinstance(next(parts(iter([1, 2, 3, 4]), length=2)), Iterable)
-    True
-
-    The type of input :obj:`~collections.abc.Sequence` objects is preserved in
-    the output.
-
-    >>> class wrap:
-    ...     def __init__(self, xs): self.xs = xs
-    ...     def __len__(self): return len(self.xs)
-    ...     def __getitem__(self, key): return wrap(self.xs[key])
-    ...     def __repr__(self): return 'wrap(' + str(self.xs) + ')'
-    >>> isinstance(next(parts(wrap([1, 2, 3, 4]), number=2)), wrap)
-    True
-    >>> list(parts(wrap([1, 2, 3, 4]), number=2))
-    [wrap([1, 2]), wrap([3, 4])]
-    >>> list(parts(wrap([1, 2, 3, 4]), length=2))
-    [wrap([1, 2]), wrap([3, 4])]
-    >>> list(parts(wrap([1, 2, 3, 4]), length=[2, 2]))
-    [wrap([1, 2]), wrap([3, 4])]
-    >>> list(parts(wrap([1, 2, 3, 4]), number=2, length=2))
-    [wrap([1, 2]), wrap([3, 4])]
-    >>> list(parts(wrap([1, 2, 3, 4]), number=2, length=[2, 2]))
-    [wrap([1, 2]), wrap([3, 4])]
-
-    The type of input objects *derived* from a :obj:`~collections.abc.Sequence`
-    type is also preserved in the output.
-
-    >>> class inherit(tuple):
-    ...     def __getitem__(self, key): return inherit(tuple(self)[key])
-    ...     def __repr__(self): return 'inherit' + str(tuple(self))
-    >>> isinstance(next(parts(inherit([1, 2, 3, 4]), 2)), inherit)
-    True
-    >>> list(parts(inherit([1, 2, 3, 4]), number=2))
-    [inherit(1, 2), inherit(3, 4)]
-    >>> list(parts(inherit([1, 2, 3, 4]), length=2))
-    [inherit(1, 2), inherit(3, 4)]
-    >>> list(parts(inherit([1, 2, 3, 4]), length=[2, 2]))
-    [inherit(1, 2), inherit(3, 4)]
-    >>> list(parts(inherit([1, 2, 3, 4]), number=2, length=2))
-    [inherit(1, 2), inherit(3, 4)]
-    >>> list(parts(inherit([1, 2, 3, 4]), number=2, length=[2, 2]))
-    [inherit(1, 2), inherit(3, 4)]
-
-    Iterable inputs yield iterable outputs when possible.
-
-    >>> def iterable():
-    ...     for i in range(10):
-    ...         yield i
-    >>> isinstance((next(parts(iterable(), number=2))), Iterable)
-    Traceback (most recent call last):
-      ...
-    TypeError: object must have length to determine part lengths from number parameter
-    >>> isinstance((next(parts(iterable(), length=2))), Iterable)
-    True
-    >>> isinstance((next(parts(iterable(), length=[2, 2]))), Iterable)
-    True
-    >>> ps = parts(iterable(), number=2, length=2)
-    >>> isinstance(next(ps), Iterable) # doctest: +NORMALIZE_WHITESPACE
-    Traceback (most recent call last):
-      ...
-    TypeError: object must have length to determine if number of \
-parts having specified length(s) can be retrieved
-    >>> ps = parts(iterable(), number=2, length=[2, 2])
-    >>> isinstance(next(ps), Iterable) # doctest: +NORMALIZE_WHITESPACE
-    Traceback (most recent call last):
-      ...
-    TypeError: object must have length to determine if number of \
-parts having specified length(s) can be retrieved
-    >>> not isinstance((next(parts(iterable(), length=2))), list)
-    True
-    >>> list(parts(123, length=2))
-    Traceback (most recent call last):
-      ...
-    TypeError: object does not support retrieval of slices
-
-    A descriptive exception is raised when parameter values cannot be satisfied,
-    cause a conflict, or have an incorrect type.
-
-    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
-    [[1, 2, 3], [4, 5, 6]]
-    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
-    [[1, 2], [3, 4], [5, 6]]
-    >>> list(parts(iter([1, 2, 3, 4, 5, 6]), number=3, length=2))
-    Traceback (most recent call last):
-      ...
-    TypeError: object must have length to determine if number of \
-parts having specified length(s) can be retrieved
-    >>> list(parts(iter([1, 2, 3, 4, 5, 6, 7]), 1))
-    Traceback (most recent call last):
-      ...
-    TypeError: object must have length to determine part lengths from number parameter
-    >>> list(parts([1, 2, 3, 4, 5, 6], 1.2))
-    Traceback (most recent call last):
-      ...
-    TypeError: number parameter must be an integer
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=1.23))
-    Traceback (most recent call last):
-      ...
-    TypeError: length parameter must be an integer or iterable of integers
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1.23]))
-    Traceback (most recent call last):
-      ...
-    TypeError: length parameter must be an integer or iterable of integers
-    >>> list(parts([1, 2, 3, 4, 5, 6], 2, length=[1, 2, 3]))
-    Traceback (most recent call last):
-      ...
-    ValueError: number parameter does not match number of specified part lengths
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
-    Traceback (most recent call last):
-      ...
-    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
-    >>> list(parts([1, 2, 3], length=4))
-    [[1, 2, 3]]
-    >>> list(parts([1, 2, 3], number=2, length=[1, 2]))
-    [[1], [2, 3]]
-    >>> list(parts([1, 2, 3], number=3, length=[1, 2, 3]))
-    Traceback (most recent call last):
-      ...
-    ValueError: object has too few items to retrieve parts having specified part lengths
-    >>> list(parts([1, 2, 3]))
-    Traceback (most recent call last):
-      ...
-    ValueError: missing number of parts parameter and part length(s) parameter
-    >>> list(parts([1, 2, 3], length=[4]))
-    [[1, 2, 3]]
-    >>> list(parts([1, 2, 3], length=[3, 1]))
-    Traceback (most recent call last):
-      ...
-    ValueError: object has too few items to retrieve parts having specified part lengths
-    >>> list(parts([1, 2, 3], number=2, length=[1, 1]))
-    Traceback (most recent call last):
-      ...
-    ValueError: object has too many items to retrieve parts having specified part lengths
-    >>> list(parts([1, 2, 3], number=1, length=[4]))
-    [[1, 2, 3]]
-    >>> list(parts([1, 2, 3], number=2, length=[3, 1]))
-    Traceback (most recent call last):
-      ...
-    ValueError: object has too few items to retrieve parts having specified part lengths
-    >>> list(parts([1, 2, 3], length=[1, 1, 1, 1]))
-    Traceback (most recent call last):
-      ...
-    ValueError: object has too few items to retrieve parts having specified part lengths
-    >>> list(parts([1, 2, 3], number=1, length=[1.2]))
-    Traceback (most recent call last):
-      ...
-    TypeError: length parameter must be an integer or list of integers
-    """
-    # pylint: disable=too-many-branches,too-many-statements
-    if number is not None and not isinstance(number, int):
-        raise TypeError('number parameter must be an integer')
-
-    if length is not None:
-        if not isinstance(length, int) and not isinstance(length, collections.abc.Iterable):
-            raise TypeError(
-                'length parameter must be an integer or iterable of integers'
-            )
-
-    if number is not None and length is None:
-        try:
-            len_ = len(xs)
-        except:
-            raise TypeError(
-                'object must have length to determine part lengths from number parameter'
-            ) from None
-
-        number = max(1, min(len_, number)) # Number should be reasonable.
-        length = len_ // number
-
-        # Produce parts by updating length after each part to ensure
-        # an even distribution.
-        i = 0
-        while number > 0 and i < len_:
-            number -= 1
-            if number == 0:
-                yield xs[i:]
-                break
-            yield xs[i:i + length]
-            i += length
-            length = (len_ - i) // number
-
-    elif number is None and length is not None:
-        if isinstance(length, int):
-            length = max(1, length)
-            index = 0
-            while True:
-                part = _slice(xs, index, index + length)
-                index += length
-
-                # The type of each part will match that of the original
-                # object to the extent that `_slice` can do so.
-                (part, empty) = _empty(part)
-                if empty:
-                    break
-                yield part
-
-        else: # Length can only be an iterable of integers.
-            lengths = iter(length)
-            index = 0
-            while True:
-                try:
-                    length = next(lengths)
-                    if not isinstance(length, int):
-                        raise TypeError(
-                            'length parameter must be an integer or iterable of integers'
-                        )
-
-                    part = _slice(xs, index, index + length)
-                    index += length
-
-                    # The type of each part will match that of the original
-                    # object to the extent that `_slice` can do so.
-                    (part, empty) = _empty(part)
-                    if empty:
-                        raise ValueError(
-                            'object has too few items to retrieve parts having ' + \
-                            'specified part lengths'
-                        )
-                    yield part
-                except StopIteration:
-                    break
-
-    elif number is not None and length is not None:
-        try:
-            len_ = len(xs)
-        except:
-            raise TypeError(
-                'object must have length to determine if number of ' + \
-                'parts having specified length(s) can be retrieved'
-            ) from None
-
-        if isinstance(length, int):
-            length = max(1, length)
-            if len_ > (length * number) or len_ <= (length * (number - 1)):
-                raise ValueError(
-                    'cannot retrieve ' + str(number) + ' parts from object ' + \
-                    'given part length parameter of ' + str(length)
-                )
-            for i in range(0, len_, length): # Yield parts of specified length.
-                yield xs[i:i + length]
-        elif (not isinstance(length, list)) or \
-             (not all(isinstance(l, int) for l in length)):
-            raise TypeError(
-                'length parameter must be an integer or list of integers'
-            )
-        else: # Length must be a list of integers.
-            if len(length) != number:
-                raise ValueError(
-                    'number parameter does not match number of specified part lengths'
-                )
-
-            if len_ <= sum(length[:-1]):
-                raise ValueError(
-                    'object has too few items to retrieve parts having ' + \
-                    'specified part lengths'
-                )
-
-            if len_ > sum(length):
-                raise ValueError(
-                    'object has too many items to retrieve parts having ' + \
-                    'specified part lengths'
-                )
-
-            lengths = iter(length)
-            index = 0
-            while True:
-                try:
-                    length = next(lengths)
-                    part = _slice(xs, index, index + length)
-                    index += length
-                    yield part
-                except StopIteration:
-                    break
-
-    else: # Neither is specified.
-        raise ValueError('missing number of parts parameter and part length(s) parameter')
-
-if __name__ == '__main__':
-    doctest.testmod() # pragma: no cover
+"""
+Minimal library that enables partitioning of iterable objects in a concise
+manner.
+"""
+import doctest
+from typing import Tuple, Union, Optional, Iterable
+import collections.abc
+from itertools import islice, chain
+
+def _empty(xs: Iterable) -> Tuple[Iterable, bool]:
+    """
+    Determine whether a sequential type instance is empty.
+
+    >>> def error():
+    ...     for i in range(2):
+    ...         if i == 0:
+    ...             yield i
+    ...         else:
+    ...             raise RuntimeError('error in generator')
+    ...
+    >>> list(parts(error(), length=1))
+    Traceback (most recent call last):
+      ...
+    RuntimeError: error in generator
+    """
+    try:
+        return (xs, len(xs) == 0)
+    except TypeError:
+        try:
+            x = next(xs)
+            return (iter(chain([x], xs)), False)
+        except StopIteration:
+            return (xs, True)
+        except Exception as e:
+            raise e from None
+
+def _slice(xs: Iterable, lower: int, upper: int) -> Iterable:
+    """
+    Attempt to retrieve a subsequence of a sequential type instance
+    using slice notation or :obj:`itertools.islice`.
+    """
+    try:
+        return xs[lower: min(len(xs), upper)]
+    except TypeError:
+        try:
+            return islice(xs, 0, upper - lower)
+        except:
+            raise TypeError(
+                'object does not support retrieval of slices'
+            ) from None
+
+def parts(
+        xs: Iterable,
+        number: Optional[int] = None,
+        length: Union[int, Iterable[int], None] = None
+    ) -> Iterable:
+    """
+    This function splits an :obj:`~collections.abc.Iterable` object into either
+    the specified number of parts or a number of parts each of the specified
+    length. When input parameters lead to ambiguous or conflicting constraints,
+    either elements are distributed in a best-effort manner or an exception is
+    raised (depending on the specific scenario).
+
+    :param xs: Iterable to split into parts.
+    :param number: Number of parts.
+    :param length: Length of every part or iterable of part lengths.
+
+    In the simplest case, the target number of parts can be specified.
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 1))
+    [[1, 2, 3, 4, 5, 6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 2))
+    [[1, 2, 3], [4, 5, 6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 3))
+    [[1, 2], [3, 4], [5, 6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 4))
+    [[1], [2, 3], [4, 5], [6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
+    [[1], [2], [3], [4, 5], [6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 6))
+    [[1], [2], [3], [4], [5], [6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7))
+    [[1], [2], [3], [4], [5], [6], [7]]
+
+    The target length for each part can be specified; the number of parts will
+    be determined based on the length and the available number of items.
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=1))
+    [[1], [2], [3], [4], [5], [6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
+    [[1, 2], [3, 4], [5, 6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=3))
+    [[1, 2, 3], [4, 5, 6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
+    [[1, 2, 3, 4], [5, 6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=5))
+    [[1, 2, 3, 4, 5], [6, 7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=6))
+    [[1, 2, 3, 4, 5, 6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=7))
+    [[1, 2, 3, 4, 5, 6, 7]]
+    >>> list(map(list, parts(iter([1, 2, 3, 4, 5, 6, 7]), length=4)))
+    [[1, 2, 3, 4], [5, 6, 7]]
+
+    An iterable of length values can be specified. The entry at each position
+    in the iterable of lengths dictates the length of the part in the
+    corresponding position in the output.
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
+    [[1], [2], [3], [4], [5], [6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=[1, 1, 1, 1, 1, 1, 1]))
+    [[1], [2], [3], [4], [5], [6], [7]]
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
+    [[1, 2], [3, 4], [5, 6]]
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
+    [[1], [2, 3], [4, 5, 6]]
+
+    The type of input objects (for built-in types) is preserved in the output.
+
+    >>> isinstance(next(parts([1, 2, 3, 4, 5], length=2)), list)
+    True
+    >>> isinstance(next(parts([1, 2, 3, 4, 5], length=[2, 2, 1])), list)
+    True
+    >>> isinstance(next(parts([1, 2, 3, 4, 5], number=2)), list)
+    True
+    >>> isinstance(next(parts([1, 2, 3, 4], number=2, length=2)), list)
+    True
+    >>> isinstance(next(parts([1, 2, 3, 4], number=2, length=[2, 2])), list)
+    True
+    >>> isinstance(next(parts((1, 2, 3, 4, 5), length=2)), tuple)
+    True
+    >>> isinstance(next(parts((1, 2, 3, 4, 5), length=[2, 2, 1])), tuple)
+    True
+    >>> isinstance(next(parts((1, 2, 3, 4, 5), number=2)), tuple)
+    True
+    >>> isinstance(next(parts((1, 2, 3, 4), number=2, length=2)), tuple)
+    True
+    >>> isinstance(next(parts((1, 2, 3, 4), number=2, length=[2, 2])), tuple)
+    True
+    >>> isinstance(next(parts('abc', length=2)), str)
+    True
+    >>> isinstance(next(parts('abc', length=[2, 1])), str)
+    True
+    >>> isinstance(next(parts('abc', number=2)), str)
+    True
+    >>> isinstance(next(parts('abcd', number=2, length=2)), str)
+    True
+    >>> isinstance(next(parts('abcd', number=2, length=[2, 2])), str)
+    True
+    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), length=2)), bytes)
+    True
+    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), length=[2, 2, 1])), bytes)
+    True
+    >>> isinstance(next(parts(bytes([1, 2, 3, 4, 5]), number=2)), bytes)
+    True
+    >>> isinstance(next(parts(bytes([1, 2, 3, 4]), number=2, length=2)), bytes)
+    True
+    >>> isinstance(next(parts(bytes([1, 2, 3, 4]), number=2, length=[2, 2])), bytes)
+    True
+    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), length=2)), bytearray)
+    True
+    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), length=[2, 2, 1])), bytearray)
+    True
+    >>> isinstance(next(parts(bytearray([1, 2, 3, 4, 5]), number=2)), bytearray)
+    True
+    >>> isinstance(next(parts(bytearray([1, 2, 3, 4]), number=2, length=2)), bytearray)
+    True
+    >>> isinstance(next(parts(bytearray([1, 2, 3, 4]), number=2, length=[2, 2])), bytearray)
+    True
+    >>> isinstance(next(parts(range(0, 10), length=2)), range)
+    True
+    >>> isinstance(next(parts(range(0, 5), length=[2, 2, 1])), range)
+    True
+    >>> isinstance(next(parts(range(0, 10), number=2)), range)
+    True
+    >>> isinstance(next(parts(range(0, 4), number=2, length=2)), range)
+    True
+    >>> isinstance(next(parts(range(0, 4), number=2, length=[2, 2])), range)
+    True
+    >>> isinstance(next(parts(iter([1, 2, 3, 4]), length=2)), Iterable)
+    True
+
+    The type of input :obj:`~collections.abc.Sequence` objects is preserved in
+    the output.
+
+    >>> class wrap:
+    ...     def __init__(self, xs): self.xs = xs
+    ...     def __len__(self): return len(self.xs)
+    ...     def __getitem__(self, key): return wrap(self.xs[key])
+    ...     def __repr__(self): return 'wrap(' + str(self.xs) + ')'
+    >>> isinstance(next(parts(wrap([1, 2, 3, 4]), number=2)), wrap)
+    True
+    >>> list(parts(wrap([1, 2, 3, 4]), number=2))
+    [wrap([1, 2]), wrap([3, 4])]
+    >>> list(parts(wrap([1, 2, 3, 4]), length=2))
+    [wrap([1, 2]), wrap([3, 4])]
+    >>> list(parts(wrap([1, 2, 3, 4]), length=[2, 2]))
+    [wrap([1, 2]), wrap([3, 4])]
+    >>> list(parts(wrap([1, 2, 3, 4]), number=2, length=2))
+    [wrap([1, 2]), wrap([3, 4])]
+    >>> list(parts(wrap([1, 2, 3, 4]), number=2, length=[2, 2]))
+    [wrap([1, 2]), wrap([3, 4])]
+
+    The type of input objects *derived* from a :obj:`~collections.abc.Sequence`
+    type is also preserved in the output.
+
+    >>> class inherit(tuple):
+    ...     def __getitem__(self, key): return inherit(tuple(self)[key])
+    ...     def __repr__(self): return 'inherit' + str(tuple(self))
+    >>> isinstance(next(parts(inherit([1, 2, 3, 4]), 2)), inherit)
+    True
+    >>> list(parts(inherit([1, 2, 3, 4]), number=2))
+    [inherit(1, 2), inherit(3, 4)]
+    >>> list(parts(inherit([1, 2, 3, 4]), length=2))
+    [inherit(1, 2), inherit(3, 4)]
+    >>> list(parts(inherit([1, 2, 3, 4]), length=[2, 2]))
+    [inherit(1, 2), inherit(3, 4)]
+    >>> list(parts(inherit([1, 2, 3, 4]), number=2, length=2))
+    [inherit(1, 2), inherit(3, 4)]
+    >>> list(parts(inherit([1, 2, 3, 4]), number=2, length=[2, 2]))
+    [inherit(1, 2), inherit(3, 4)]
+
+    Iterable inputs yield iterable outputs when possible.
+
+    >>> def iterable():
+    ...     for i in range(10):
+    ...         yield i
+    >>> isinstance((next(parts(iterable(), number=2))), Iterable)
+    Traceback (most recent call last):
+      ...
+    TypeError: object must have length to determine part lengths from number parameter
+    >>> isinstance((next(parts(iterable(), length=2))), Iterable)
+    True
+    >>> isinstance((next(parts(iterable(), length=[2, 2]))), Iterable)
+    True
+    >>> ps = parts(iterable(), number=2, length=2)
+    >>> isinstance(next(ps), Iterable) # doctest: +NORMALIZE_WHITESPACE
+    Traceback (most recent call last):
+      ...
+    TypeError: object must have length to determine if number of \
+parts having specified length(s) can be retrieved
+    >>> ps = parts(iterable(), number=2, length=[2, 2])
+    >>> isinstance(next(ps), Iterable) # doctest: +NORMALIZE_WHITESPACE
+    Traceback (most recent call last):
+      ...
+    TypeError: object must have length to determine if number of \
+parts having specified length(s) can be retrieved
+    >>> not isinstance((next(parts(iterable(), length=2))), list)
+    True
+    >>> list(parts(123, length=2))
+    Traceback (most recent call last):
+      ...
+    TypeError: object does not support retrieval of slices
+
+    A descriptive exception is raised when parameter values cannot be satisfied,
+    cause a conflict, or have an incorrect type.
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
+    [[1, 2, 3], [4, 5, 6]]
+    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
+    [[1, 2], [3, 4], [5, 6]]
+    >>> list(parts(iter([1, 2, 3, 4, 5, 6]), number=3, length=2))
+    Traceback (most recent call last):
+      ...
+    TypeError: object must have length to determine if number of \
+parts having specified length(s) can be retrieved
+    >>> list(parts(iter([1, 2, 3, 4, 5, 6, 7]), 1))
+    Traceback (most recent call last):
+      ...
+    TypeError: object must have length to determine part lengths from number parameter
+    >>> list(parts([1, 2, 3, 4, 5, 6], 1.2))
+    Traceback (most recent call last):
+      ...
+    TypeError: number parameter must be an integer
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=1.23))
+    Traceback (most recent call last):
+      ...
+    TypeError: length parameter must be an integer or iterable of integers
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1.23]))
+    Traceback (most recent call last):
+      ...
+    TypeError: length parameter must be an integer or iterable of integers
+    >>> list(parts([1, 2, 3, 4, 5, 6], 2, length=[1, 2, 3]))
+    Traceback (most recent call last):
+      ...
+    ValueError: number parameter does not match number of specified part lengths
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
+    Traceback (most recent call last):
+      ...
+    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
+    >>> list(parts([1, 2, 3], length=4))
+    [[1, 2, 3]]
+    >>> list(parts([1, 2, 3], number=2, length=[1, 2]))
+    [[1], [2, 3]]
+    >>> list(parts([1, 2, 3], number=3, length=[1, 2, 3]))
+    Traceback (most recent call last):
+      ...
+    ValueError: object has too few items to retrieve parts having specified part lengths
+    >>> list(parts([1, 2, 3]))
+    Traceback (most recent call last):
+      ...
+    ValueError: missing number of parts parameter and part length(s) parameter
+    >>> list(parts([1, 2, 3], length=[4]))
+    [[1, 2, 3]]
+    >>> list(parts([1, 2, 3], length=[3, 1]))
+    Traceback (most recent call last):
+      ...
+    ValueError: object has too few items to retrieve parts having specified part lengths
+    >>> list(parts([1, 2, 3], number=2, length=[1, 1]))
+    Traceback (most recent call last):
+      ...
+    ValueError: object has too many items to retrieve parts having specified part lengths
+    >>> list(parts([1, 2, 3], number=1, length=[4]))
+    [[1, 2, 3]]
+    >>> list(parts([1, 2, 3], number=2, length=[3, 1]))
+    Traceback (most recent call last):
+      ...
+    ValueError: object has too few items to retrieve parts having specified part lengths
+    >>> list(parts([1, 2, 3], length=[1, 1, 1, 1]))
+    Traceback (most recent call last):
+      ...
+    ValueError: object has too few items to retrieve parts having specified part lengths
+    >>> list(parts([1, 2, 3], number=1, length=[1.2]))
+    Traceback (most recent call last):
+      ...
+    TypeError: length parameter must be an integer or list of integers
+    """
+    # pylint: disable=too-many-branches,too-many-statements
+    if number is not None and not isinstance(number, int):
+        raise TypeError('number parameter must be an integer')
+
+    if length is not None:
+        if not isinstance(length, int) and not isinstance(length, collections.abc.Iterable):
+            raise TypeError(
+                'length parameter must be an integer or iterable of integers'
+            )
+
+    if number is not None and length is None:
+        try:
+            len_ = len(xs)
+        except:
+            raise TypeError(
+                'object must have length to determine part lengths from number parameter'
+            ) from None
+
+        number = max(1, min(len_, number)) # Number should be reasonable.
+        length = len_ // number
+
+        # Produce parts by updating length after each part to ensure
+        # an even distribution.
+        i = 0
+        while number > 0 and i < len_:
+            number -= 1
+            if number == 0:
+                yield xs[i:]
+                break
+            yield xs[i:i + length]
+            i += length
+            length = (len_ - i) // number
+
+    elif number is None and length is not None:
+        if isinstance(length, int):
+            length = max(1, length)
+            index = 0
+            while True:
+                part = _slice(xs, index, index + length)
+                index += length
+
+                # The type of each part will match that of the original
+                # object to the extent that `_slice` can do so.
+                (part, empty) = _empty(part)
+                if empty:
+                    break
+                yield part
+
+        else: # Length can only be an iterable of integers.
+            lengths = iter(length)
+            index = 0
+            while True:
+                try:
+                    length = next(lengths)
+                    if not isinstance(length, int):
+                        raise TypeError(
+                            'length parameter must be an integer or iterable of integers'
+                        )
+
+                    part = _slice(xs, index, index + length)
+                    index += length
+
+                    # The type of each part will match that of the original
+                    # object to the extent that `_slice` can do so.
+                    (part, empty) = _empty(part)
+                    if empty:
+                        raise ValueError(
+                            'object has too few items to retrieve parts having ' + \
+                            'specified part lengths'
+                        )
+                    yield part
+                except StopIteration:
+                    break
+
+    elif number is not None and length is not None:
+        try:
+            len_ = len(xs)
+        except:
+            raise TypeError(
+                'object must have length to determine if number of ' + \
+                'parts having specified length(s) can be retrieved'
+            ) from None
+
+        if isinstance(length, int):
+            length = max(1, length)
+            if len_ > (length * number) or len_ <= (length * (number - 1)):
+                raise ValueError(
+                    'cannot retrieve ' + str(number) + ' parts from object ' + \
+                    'given part length parameter of ' + str(length)
+                )
+            for i in range(0, len_, length): # Yield parts of specified length.
+                yield xs[i:i + length]
+        elif (not isinstance(length, list)) or \
+             (not all(isinstance(l, int) for l in length)):
+            raise TypeError(
+                'length parameter must be an integer or list of integers'
+            )
+        else: # Length must be a list of integers.
+            if len(length) != number:
+                raise ValueError(
+                    'number parameter does not match number of specified part lengths'
+                )
+
+            if len_ <= sum(length[:-1]):
+                raise ValueError(
+                    'object has too few items to retrieve parts having ' + \
+                    'specified part lengths'
+                )
+
+            if len_ > sum(length):
+                raise ValueError(
+                    'object has too many items to retrieve parts having ' + \
+                    'specified part lengths'
+                )
+
+            lengths = iter(length)
+            index = 0
+            while True:
+                try:
+                    length = next(lengths)
+                    part = _slice(xs, index, index + length)
+                    index += length
+                    yield part
+                except StopIteration:
+                    break
+
+    else: # Neither is specified.
+        raise ValueError('missing number of parts parameter and part length(s) parameter')
+
+if __name__ == '__main__':
+    doctest.testmod() # pragma: no cover
```

### Comparing `parts-1.5.2/src/parts.egg-info/PKG-INFO` & `parts-1.6.0/src/parts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,174 @@
-Metadata-Version: 2.1
-Name: parts
-Version: 1.5.2
-Summary: Minimal library that enables partitioning of iterable objects in a concise manner.
-Author: Andrei Lapets
-Author-email: a@lapets.io
-License: MIT
-Project-URL: Repository, https://github.com/lapets/parts
-Project-URL: Documentation, https://parts.readthedocs.io
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: test
-Provides-Extra: lint
-Provides-Extra: coveralls
-Provides-Extra: publish
-License-File: LICENSE
-
-=====
-parts
-=====
-
-Minimal library that enables partitioning of iterable objects in a concise manner.
-
-|pypi| |readthedocs| |actions| |coveralls|
-
-.. |pypi| image:: https://badge.fury.io/py/parts.svg
-   :target: https://badge.fury.io/py/parts
-   :alt: PyPI version and link.
-
-.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
-   :target: https://parts.readthedocs.io/en/latest/?badge=latest
-   :alt: Read the Docs documentation status.
-
-.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
-   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
-   :alt: GitHub Actions status.
-
-.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
-   :target: https://coveralls.io/github/lapets/parts?branch=main
-   :alt: Coveralls test coverage summary.
-
-Purpose
--------
-This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
-
-Installation and Usage
-----------------------
-This library is available as a `package on PyPI <https://pypi.org/project/parts>`__::
-
-    python -m pip install parts
-
-The library can be imported in the usual manner::
-
-    import parts
-    from parts import parts
-
-Examples
-^^^^^^^^
-Several examples are presented below::
-
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
-    [[1, 2], [3, 4], [5, 6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
-    [[1, 2, 3, 4], [5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
-    [[1, 2, 3, 4, 5, 6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
-    [[1], [2], [3], [4, 5], [6, 7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
-    [[1, 2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
-    [[1], [2], [3], [4], [5], [6], [7]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
-    [[1, 2], [3, 4], [5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
-    [[1], [2, 3], [4, 5, 6]]
-    
-    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
-    Traceback (most recent call last):
-      ...
-    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
-    python src/parts/parts.py -v
-
-Style conventions are enforced using `Pylint <https://pylint.pycqa.org>`__::
-
-    python -m pip install .[lint]
-    python -m pylint src/parts
-
-Contributions
-^^^^^^^^^^^^^
-In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
-
-Versioning
-^^^^^^^^^^
-Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
-
-Publishing
-^^^^^^^^^^
-This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing::
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
+Name: parts
+Version: 1.6.0
+Summary: Minimal library that enables partitioning of iterable objects in a concise manner.
+Author: Andrei Lapets
+Author-email: a@lapets.io
+License: MIT
+Project-URL: Repository, https://github.com/lapets/parts
+Project-URL: Documentation, https://parts.readthedocs.io
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: docs
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: coveralls
+Provides-Extra: publish
+License-File: LICENSE
+
+=====
+parts
+=====
+
+Minimal library that enables partitioning of iterable objects in a concise manner.
+
+|pypi| |readthedocs| |actions| |coveralls|
+
+.. |pypi| image:: https://badge.fury.io/py/parts.svg
+   :target: https://badge.fury.io/py/parts
+   :alt: PyPI version and link.
+
+.. |readthedocs| image:: https://readthedocs.org/projects/parts/badge/?version=latest
+   :target: https://parts.readthedocs.io/en/latest/?badge=latest
+   :alt: Read the Docs documentation status.
+
+.. |actions| image:: https://github.com/lapets/parts/workflows/lint-test-cover-docs/badge.svg
+   :target: https://github.com/lapets/parts/actions/workflows/lint-test-cover-docs.yml
+   :alt: GitHub Actions status.
+
+.. |coveralls| image:: https://coveralls.io/repos/github/lapets/parts/badge.svg?branch=main
+   :target: https://coveralls.io/github/lapets/parts?branch=main
+   :alt: Coveralls test coverage summary.
+
+Purpose
+-------
+This library provides a function for partitioning `iterable <https://docs.python.org/3/glossary.html#term-iterable>`__ data structure instances. When the number of parts is specified explicitly, it is treated as a strict requirement and an exception is raised when it cannot be satisfied. When a length for all parts (or each part) is specified explicitly, a best-effort approach is used: as many parts of the specified length are retrieved as possible, with the possibility that some parts at the end of the partition sequence have a shorter (but still non-zero) length.
+
+Installation and Usage
+----------------------
+This library is available as a `package on PyPI <https://pypi.org/project/parts>`__:
+
+.. code-block:: bash
+
+    python -m pip install parts
+
+The library can be imported in the usual manner:
+
+.. code-block:: python
+
+    import parts
+    from parts import parts
+
+Examples
+^^^^^^^^
+Several examples are presented below:
+
+.. code-block:: python
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=2))
+    [[1, 2], [3, 4], [5, 6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], length=4))
+    [[1, 2, 3, 4], [5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=1))
+    [[1, 2, 3, 4, 5, 6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 5))
+    [[1], [2], [3], [4, 5], [6, 7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], 2, 3))
+    [[1, 2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], number=3, length=2))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], 7, [1, 1, 1, 1, 1, 1, 1]))
+    [[1], [2], [3], [4], [5], [6], [7]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[2, 2, 2]))
+    [[1, 2], [3, 4], [5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6], length=[1, 2, 3]))
+    [[1], [2, 3], [4, 5, 6]]
+
+    >>> list(parts([1, 2, 3, 4, 5, 6, 7], number=3, length=2))
+    Traceback (most recent call last):
+      ...
+    ValueError: cannot retrieve 3 parts from object given part length parameter of 2
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
+    python src/parts/parts.py -v
+
+Style conventions are enforced using `Pylint <https://pylint.readthedocs.io>`__:
+
+.. code-block:: bash
+
+    python -m pip install .[lint]
+    python -m pylint src/parts
+
+Contributions
+^^^^^^^^^^^^^
+In order to contribute to the source code, open an issue or submit a pull request on the `GitHub page <https://github.com/lapets/parts>`__ for this library.
+
+Versioning
+^^^^^^^^^^
+Beginning with version 0.2.0, the version number format for this library and the changes to the library associated with version number increments conform with `Semantic Versioning 2.0.0 <https://semver.org/#semantic-versioning-200>`__.
+
+Publishing
+^^^^^^^^^^
+This library can be published as a `package on PyPI <https://pypi.org/project/parts>`__ by a package maintainer. First, install the dependencies required for packaging and publishing:
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

