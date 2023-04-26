# Comparing `tmp/bamnostic-1.1.7.tar.gz` & `tmp/bamnostic-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bamnostic-1.1.7.tar", last modified: Fri Apr 30 12:14:10 2021, max compression
+gzip compressed data, was "dist/bamnostic-1.1.8.tar", last modified: Thu Nov  4 22:00:17 2021, max compression
```

## Comparing `bamnostic-1.1.7.tar` & `bamnostic-1.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-30 12:14:10.000000 bamnostic-1.1.7/
--rw-r--r--   0 root         (0) root         (0)     3267 2021-02-09 23:08:06.000000 bamnostic-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     3320 2021-02-09 23:08:06.000000 bamnostic-1.1.7/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     1546 2021-02-09 23:08:06.000000 bamnostic-1.1.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      182 2021-02-09 23:08:06.000000 bamnostic-1.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6434 2021-04-30 12:14:10.000000 bamnostic-1.1.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14121 2021-04-30 12:12:40.000000 bamnostic-1.1.7/README.md
--rw-r--r--   0 root         (0) root         (0)     3962 2021-02-09 23:08:06.000000 bamnostic-1.1.7/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-30 12:14:10.000000 bamnostic-1.1.7/bamnostic/
--rw-r--r--   0 root         (0) root         (0)     1372 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/bai.py
--rw-r--r--   0 root         (0) root         (0)    50985 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/bam.py
--rw-r--r--   0 root         (0) root         (0)    21319 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/bgzf.py
--rw-r--r--   0 root         (0) root         (0)    34286 2021-04-30 12:12:40.000000 bamnostic-1.1.7/bamnostic/core.py
--rw-r--r--   0 root         (0) root         (0)    14792 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/csi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-30 12:14:10.000000 bamnostic-1.1.7/bamnostic/data/
--rw-r--r--   0 root         (0) root         (0)   124630 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/data/example.bam
--rw-r--r--   0 root         (0) root         (0)      176 2021-02-09 23:08:06.000000 bamnostic-1.1.7/bamnostic/data/example.bam.bai
--rw-r--r--   0 root         (0) root         (0)    29637 2021-04-30 12:12:40.000000 bamnostic-1.1.7/bamnostic/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-30 12:14:10.000000 bamnostic-1.1.7/bamnostic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6434 2021-04-30 12:14:09.000000 bamnostic-1.1.7/bamnostic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      554 2021-04-30 12:14:09.000000 bamnostic-1.1.7/bamnostic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-04-30 12:14:09.000000 bamnostic-1.1.7/bamnostic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-09 23:16:59.000000 bamnostic-1.1.7/bamnostic.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2021-04-30 12:14:09.000000 bamnostic-1.1.7/bamnostic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      126 2021-02-09 23:08:06.000000 bamnostic-1.1.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-09 23:08:06.000000 bamnostic-1.1.7/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       99 2021-04-30 12:14:10.000000 bamnostic-1.1.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2940 2021-02-09 23:35:30.000000 bamnostic-1.1.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-30 12:14:10.000000 bamnostic-1.1.7/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2021-02-09 23:08:06.000000 bamnostic-1.1.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2021-02-09 23:08:06.000000 bamnostic-1.1.7/tests/test_build.py
--rw-r--r--   0 root         (0) root         (0)        6 2021-04-30 12:13:33.000000 bamnostic-1.1.7/version
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-04 22:00:17.000000 bamnostic-1.1.8/
+-rw-r--r--   0 root         (0) root         (0)     3267 2021-11-04 21:57:57.000000 bamnostic-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     3320 2021-11-04 21:57:57.000000 bamnostic-1.1.8/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     1546 2021-11-04 21:57:57.000000 bamnostic-1.1.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      182 2021-11-04 21:57:57.000000 bamnostic-1.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5605 2021-11-04 22:00:17.000000 bamnostic-1.1.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14121 2021-11-04 21:57:57.000000 bamnostic-1.1.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     3962 2021-11-04 21:57:57.000000 bamnostic-1.1.8/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic/
+-rw-r--r--   0 root         (0) root         (0)     1372 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18002 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/bai.py
+-rw-r--r--   0 root         (0) root         (0)    50983 2021-11-04 21:58:35.000000 bamnostic-1.1.8/bamnostic/bam.py
+-rw-r--r--   0 root         (0) root         (0)    21319 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/bgzf.py
+-rw-r--r--   0 root         (0) root         (0)    34286 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/core.py
+-rw-r--r--   0 root         (0) root         (0)    14792 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/csi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic/data/
+-rw-r--r--   0 root         (0) root         (0)   124630 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/data/example.bam
+-rw-r--r--   0 root         (0) root         (0)      176 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/data/example.bam.bai
+-rw-r--r--   0 root         (0) root         (0)    29637 2021-11-04 21:57:57.000000 bamnostic-1.1.8/bamnostic/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5605 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      562 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2021-11-04 22:00:17.000000 bamnostic-1.1.8/bamnostic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      126 2021-11-04 21:57:57.000000 bamnostic-1.1.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-04 21:57:57.000000 bamnostic-1.1.8/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2021-11-04 22:00:17.000000 bamnostic-1.1.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2940 2021-11-04 21:57:57.000000 bamnostic-1.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-11-04 22:00:17.000000 bamnostic-1.1.8/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-11-04 21:57:57.000000 bamnostic-1.1.8/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2021-11-04 21:57:57.000000 bamnostic-1.1.8/tests/test_build.py
+-rw-r--r--   0 root         (0) root         (0)        6 2021-11-04 22:00:01.000000 bamnostic-1.1.8/version
```

### Comparing `bamnostic-1.1.7/CODE_OF_CONDUCT.md` & `bamnostic-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/CONTRIBUTING.md` & `bamnostic-1.1.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/LICENSE` & `bamnostic-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/PKG-INFO` & `bamnostic-1.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bamnostic
-Version: 1.1.7
+Version: 1.1.8
 Summary: Pure Python, OS-agnostic Binary Alignment Map (BAM) random access and parsing tool
 Home-page: https://github.com/betteridiot/bamnostic/
 Author: Marcus D. Sherman
 Author-email: mdsherm@umich.edu
 License: BSD 3-Clause
-Description: |Documentation Status| |Conda Version| |PyPI version| |Maintainability|
-        
-        |status| |DOI| |License|
-        
-        +----------+-------------------------+
-        | Platform | Build Status            |
-        +==========+=========================+
-        | Linux    | |Build Status TravisCI| |
-        +----------+-------------------------+
-        | Windows  | |Build status Appveyor| |
-        +----------+-------------------------+
-        | conda    | |noarch|                |
-        +----------+-------------------------+
-        
-        +-------+-------------------+
-        | Host  | Downloads         |
-        +=======+===================+
-        | PyPI  | |Downloads|       |
-        +-------+-------------------+
-        | conda | |Conda Downloads| |
-        +-------+-------------------+
-        
-        BAMnostic
-        =========
-        
-        a *pure Python*, **OS-agnositic** Binary Alignment Map (BAM) file parser
-        and random access tool.
-        
-        Note:
-        ~~~~~
-        
-        Documentation can be found at `here`_ or by going to this address:
-        http://bamnostic.readthedocs.io. Documentation was made available
-        through `Read the Docs`_.
-        
-        --------------
-        
-        Installation
-        ------------
-        
-        There are 4 methods of installation available (choose one):
-        
-        Through the ``conda`` package manager (`Anaconda Cloud`_)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           # first, add the conda-forge channel to your conda build
-           conda config --add channels conda-forge
-        
-           # now bamnostic is available for install
-           conda install bamnostic
-        
-        Through the Python Package Index (`PyPI`_)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           pip install bamnostic
-        
-           # or, if you don't have superuser access
-           pip install --user bamnostic
-        
-        Through pip+Github
-        ~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           # again, use --user if you don't have superuser access
-           pip install -e git+https://github.com/betteridiot/bamnostic.git#egg=bamnostic
-        
-           # or, if you don't have superuser access
-           pip install --user -e git+https://github.com/betteridiot/bamnostic.git#bamnostic#egg=bamnostic
-        
-        Traditiona
-        ~~~~~~~~~~
-        
-        .. _here: http://bamnostic.readthedocs.io/en/latest/
-        .. _Read the Docs: https://readthedocs.org/
-        .. _Anaconda Cloud: https://anaconda.org/conda-forge/bamnostic
-        .. _PyPI: https://pypi.org/
-        
-        .. |Documentation Status| image:: https://readthedocs.org/projects/bamnostic/badge/?version=latest
-           :target: https://bamnostic.readthedocs.io/en/latest/?badge=latest
-        .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/bamnostic.svg
-           :target: https://anaconda.org/conda-forge/bamnostic
-        .. |PyPI version| image:: https://badge.fury.io/py/bamnostic.svg
-           :target: https://badge.fury.io/py/bamnostic
-        .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/d7e36e72f109c598c86d/maintainability
-           :target: https://codeclimate.com/github/betteridiot/bamnostic/maintainability
-        .. |status| image:: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8/status.svg
-           :target: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1341959.svg
-           :target: https://doi.org/10.5281/zenodo.1341959
-        .. |License| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-           :target: https://github.com/betteridiot/bamnostic/blob/master/LICENSE
-        .. |Build Status TravisCI| image:: https://travis-ci.org/betteridiot/bamnostic.svg?branch=master
-           :target: https://travis-ci.org/betteridiot/bamnostic
-        .. |Build status Appveyor| image:: https://ci.appveyor.com/api/projects/status/y95q02gkv3lgmlf4/branch/master?svg=true
-           :target: https://ci.appveyor.com/project/betteridiot/bamnostic/branch/master
-        .. |noarch| image:: https://img.shields.io/circleci/project/github/conda-forge/bamnostic-feedstock/master.svg?label=noarch
-           :target: https://circleci.com/gh/conda-forge/bamnostic-feedstock
-        .. |Downloads| image:: http://pepy.tech/badge/bamnostic
-           :target: http://pepy.tech/project/bamnostic
-        .. |Conda Downloads| image:: https://img.shields.io/conda/dn/conda-forge/bamnostic.svg
-           :target: https://anaconda.org/conda-forge/bamnostic
 Keywords: BAM pysam genomics genetics struct
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -135,7 +29,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE
+
+|Documentation Status| |Conda Version| |PyPI version| |Maintainability|
+
+|status| |DOI| |License|
+
++----------+-------------------------+
+| Platform | Build Status            |
++==========+=========================+
+| Linux    | |Build Status TravisCI| |
++----------+-------------------------+
+| Windows  | |Build status Appveyor| |
++----------+-------------------------+
+| conda    | |noarch|                |
++----------+-------------------------+
+
++-------+-------------------+
+| Host  | Downloads         |
++=======+===================+
+| PyPI  | |Downloads|       |
++-------+-------------------+
+| conda | |Conda Downloads| |
++-------+-------------------+
+
+BAMnostic
+=========
+
+a *pure Python*, **OS-agnositic** Binary Alignment Map (BAM) file parser
+and random access tool.
+
+Note:
+~~~~~
+
+Documentation can be found at `here`_ or by going to this address:
+http://bamnostic.readthedocs.io. Documentation was made available
+through `Read the Docs`_.
+
+--------------
+
+Installation
+------------
+
+There are 4 methods of installation available (choose one):
+
+Through the ``conda`` package manager (`Anaconda Cloud`_)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   # first, add the conda-forge channel to your conda build
+   conda config --add channels conda-forge
+
+   # now bamnostic is available for install
+   conda install bamnostic
+
+Through the Python Package Index (`PyPI`_)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   pip install bamnostic
+
+   # or, if you don't have superuser access
+   pip install --user bamnostic
+
+Through pip+Github
+~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   # again, use --user if you don't have superuser access
+   pip install -e git+https://github.com/betteridiot/bamnostic.git#egg=bamnostic
+
+   # or, if you don't have superuser access
+   pip install --user -e git+https://github.com/betteridiot/bamnostic.git#bamnostic#egg=bamnostic
+
+Traditiona
+~~~~~~~~~~
+
+.. _here: http://bamnostic.readthedocs.io/en/latest/
+.. _Read the Docs: https://readthedocs.org/
+.. _Anaconda Cloud: https://anaconda.org/conda-forge/bamnostic
+.. _PyPI: https://pypi.org/
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/bamnostic/badge/?version=latest
+   :target: https://bamnostic.readthedocs.io/en/latest/?badge=latest
+.. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/bamnostic.svg
+   :target: https://anaconda.org/conda-forge/bamnostic
+.. |PyPI version| image:: https://badge.fury.io/py/bamnostic.svg
+   :target: https://badge.fury.io/py/bamnostic
+.. |Maintainability| image:: https://api.codeclimate.com/v1/badges/d7e36e72f109c598c86d/maintainability
+   :target: https://codeclimate.com/github/betteridiot/bamnostic/maintainability
+.. |status| image:: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8/status.svg
+   :target: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1341959.svg
+   :target: https://doi.org/10.5281/zenodo.1341959
+.. |License| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+   :target: https://github.com/betteridiot/bamnostic/blob/master/LICENSE
+.. |Build Status TravisCI| image:: https://travis-ci.org/betteridiot/bamnostic.svg?branch=master
+   :target: https://travis-ci.org/betteridiot/bamnostic
+.. |Build status Appveyor| image:: https://ci.appveyor.com/api/projects/status/y95q02gkv3lgmlf4/branch/master?svg=true
+   :target: https://ci.appveyor.com/project/betteridiot/bamnostic/branch/master
+.. |noarch| image:: https://img.shields.io/circleci/project/github/conda-forge/bamnostic-feedstock/master.svg?label=noarch
+   :target: https://circleci.com/gh/conda-forge/bamnostic-feedstock
+.. |Downloads| image:: http://pepy.tech/badge/bamnostic
+   :target: http://pepy.tech/project/bamnostic
+.. |Conda Downloads| image:: https://img.shields.io/conda/dn/conda-forge/bamnostic.svg
+   :target: https://anaconda.org/conda-forge/bamnostic
+
```

### Comparing `bamnostic-1.1.7/README.md` & `bamnostic-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/README.rst` & `bamnostic-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/__init__.py` & `bamnostic-1.1.8/bamnostic/__init__.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/bai.py` & `bamnostic-1.1.8/bamnostic/bai.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/bam.py` & `bamnostic-1.1.8/bamnostic/bam.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,15 +294,15 @@
             >>> bam.check_index('not_a_file.bai')
             False
 
         """
 
         if index_filename is None:
             for ext in ('csi', 'bai'):
-                possible_index_path = r'./{}.{}'.format(os.path.relpath(self._handle.name), ext)
+                possible_index_path = r'{}.{}'.format(os.path.abspath(self._handle.name), ext)
                 if os.path.isfile(possible_index_path):
                     self._index_path = possible_index_path
                     self._random_access = True
                     self._index_ext = ext
                     return True
                 else:
                     if req_idx:
```

### Comparing `bamnostic-1.1.7/bamnostic/bgzf.py` & `bamnostic-1.1.8/bamnostic/bgzf.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/core.py` & `bamnostic-1.1.8/bamnostic/core.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/csi.py` & `bamnostic-1.1.8/bamnostic/csi.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/data/example.bam` & `bamnostic-1.1.8/bamnostic/data/example.bam`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic/utils.py` & `bamnostic-1.1.8/bamnostic/utils.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/bamnostic.egg-info/PKG-INFO` & `bamnostic-1.1.8/bamnostic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,121 +1,15 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: bamnostic
-Version: 1.1.7
+Version: 1.1.8
 Summary: Pure Python, OS-agnostic Binary Alignment Map (BAM) random access and parsing tool
 Home-page: https://github.com/betteridiot/bamnostic/
 Author: Marcus D. Sherman
 Author-email: mdsherm@umich.edu
 License: BSD 3-Clause
-Description: |Documentation Status| |Conda Version| |PyPI version| |Maintainability|
-        
-        |status| |DOI| |License|
-        
-        +----------+-------------------------+
-        | Platform | Build Status            |
-        +==========+=========================+
-        | Linux    | |Build Status TravisCI| |
-        +----------+-------------------------+
-        | Windows  | |Build status Appveyor| |
-        +----------+-------------------------+
-        | conda    | |noarch|                |
-        +----------+-------------------------+
-        
-        +-------+-------------------+
-        | Host  | Downloads         |
-        +=======+===================+
-        | PyPI  | |Downloads|       |
-        +-------+-------------------+
-        | conda | |Conda Downloads| |
-        +-------+-------------------+
-        
-        BAMnostic
-        =========
-        
-        a *pure Python*, **OS-agnositic** Binary Alignment Map (BAM) file parser
-        and random access tool.
-        
-        Note:
-        ~~~~~
-        
-        Documentation can be found at `here`_ or by going to this address:
-        http://bamnostic.readthedocs.io. Documentation was made available
-        through `Read the Docs`_.
-        
-        --------------
-        
-        Installation
-        ------------
-        
-        There are 4 methods of installation available (choose one):
-        
-        Through the ``conda`` package manager (`Anaconda Cloud`_)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           # first, add the conda-forge channel to your conda build
-           conda config --add channels conda-forge
-        
-           # now bamnostic is available for install
-           conda install bamnostic
-        
-        Through the Python Package Index (`PyPI`_)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           pip install bamnostic
-        
-           # or, if you don't have superuser access
-           pip install --user bamnostic
-        
-        Through pip+Github
-        ~~~~~~~~~~~~~~~~~~
-        
-        .. code:: bash
-        
-           # again, use --user if you don't have superuser access
-           pip install -e git+https://github.com/betteridiot/bamnostic.git#egg=bamnostic
-        
-           # or, if you don't have superuser access
-           pip install --user -e git+https://github.com/betteridiot/bamnostic.git#bamnostic#egg=bamnostic
-        
-        Traditiona
-        ~~~~~~~~~~
-        
-        .. _here: http://bamnostic.readthedocs.io/en/latest/
-        .. _Read the Docs: https://readthedocs.org/
-        .. _Anaconda Cloud: https://anaconda.org/conda-forge/bamnostic
-        .. _PyPI: https://pypi.org/
-        
-        .. |Documentation Status| image:: https://readthedocs.org/projects/bamnostic/badge/?version=latest
-           :target: https://bamnostic.readthedocs.io/en/latest/?badge=latest
-        .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/bamnostic.svg
-           :target: https://anaconda.org/conda-forge/bamnostic
-        .. |PyPI version| image:: https://badge.fury.io/py/bamnostic.svg
-           :target: https://badge.fury.io/py/bamnostic
-        .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/d7e36e72f109c598c86d/maintainability
-           :target: https://codeclimate.com/github/betteridiot/bamnostic/maintainability
-        .. |status| image:: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8/status.svg
-           :target: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8
-        .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1341959.svg
-           :target: https://doi.org/10.5281/zenodo.1341959
-        .. |License| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-           :target: https://github.com/betteridiot/bamnostic/blob/master/LICENSE
-        .. |Build Status TravisCI| image:: https://travis-ci.org/betteridiot/bamnostic.svg?branch=master
-           :target: https://travis-ci.org/betteridiot/bamnostic
-        .. |Build status Appveyor| image:: https://ci.appveyor.com/api/projects/status/y95q02gkv3lgmlf4/branch/master?svg=true
-           :target: https://ci.appveyor.com/project/betteridiot/bamnostic/branch/master
-        .. |noarch| image:: https://img.shields.io/circleci/project/github/conda-forge/bamnostic-feedstock/master.svg?label=noarch
-           :target: https://circleci.com/gh/conda-forge/bamnostic-feedstock
-        .. |Downloads| image:: http://pepy.tech/badge/bamnostic
-           :target: http://pepy.tech/project/bamnostic
-        .. |Conda Downloads| image:: https://img.shields.io/conda/dn/conda-forge/bamnostic.svg
-           :target: https://anaconda.org/conda-forge/bamnostic
 Keywords: BAM pysam genomics genetics struct
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
@@ -135,7 +29,116 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
+License-File: LICENSE
+
+|Documentation Status| |Conda Version| |PyPI version| |Maintainability|
+
+|status| |DOI| |License|
+
++----------+-------------------------+
+| Platform | Build Status            |
++==========+=========================+
+| Linux    | |Build Status TravisCI| |
++----------+-------------------------+
+| Windows  | |Build status Appveyor| |
++----------+-------------------------+
+| conda    | |noarch|                |
++----------+-------------------------+
+
++-------+-------------------+
+| Host  | Downloads         |
++=======+===================+
+| PyPI  | |Downloads|       |
++-------+-------------------+
+| conda | |Conda Downloads| |
++-------+-------------------+
+
+BAMnostic
+=========
+
+a *pure Python*, **OS-agnositic** Binary Alignment Map (BAM) file parser
+and random access tool.
+
+Note:
+~~~~~
+
+Documentation can be found at `here`_ or by going to this address:
+http://bamnostic.readthedocs.io. Documentation was made available
+through `Read the Docs`_.
+
+--------------
+
+Installation
+------------
+
+There are 4 methods of installation available (choose one):
+
+Through the ``conda`` package manager (`Anaconda Cloud`_)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   # first, add the conda-forge channel to your conda build
+   conda config --add channels conda-forge
+
+   # now bamnostic is available for install
+   conda install bamnostic
+
+Through the Python Package Index (`PyPI`_)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   pip install bamnostic
+
+   # or, if you don't have superuser access
+   pip install --user bamnostic
+
+Through pip+Github
+~~~~~~~~~~~~~~~~~~
+
+.. code:: bash
+
+   # again, use --user if you don't have superuser access
+   pip install -e git+https://github.com/betteridiot/bamnostic.git#egg=bamnostic
+
+   # or, if you don't have superuser access
+   pip install --user -e git+https://github.com/betteridiot/bamnostic.git#bamnostic#egg=bamnostic
+
+Traditiona
+~~~~~~~~~~
+
+.. _here: http://bamnostic.readthedocs.io/en/latest/
+.. _Read the Docs: https://readthedocs.org/
+.. _Anaconda Cloud: https://anaconda.org/conda-forge/bamnostic
+.. _PyPI: https://pypi.org/
+
+.. |Documentation Status| image:: https://readthedocs.org/projects/bamnostic/badge/?version=latest
+   :target: https://bamnostic.readthedocs.io/en/latest/?badge=latest
+.. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/bamnostic.svg
+   :target: https://anaconda.org/conda-forge/bamnostic
+.. |PyPI version| image:: https://badge.fury.io/py/bamnostic.svg
+   :target: https://badge.fury.io/py/bamnostic
+.. |Maintainability| image:: https://api.codeclimate.com/v1/badges/d7e36e72f109c598c86d/maintainability
+   :target: https://codeclimate.com/github/betteridiot/bamnostic/maintainability
+.. |status| image:: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8/status.svg
+   :target: http://joss.theoj.org/papers/9952b35bbb30ca6c01e6a27b80006bd8
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.1341959.svg
+   :target: https://doi.org/10.5281/zenodo.1341959
+.. |License| image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+   :target: https://github.com/betteridiot/bamnostic/blob/master/LICENSE
+.. |Build Status TravisCI| image:: https://travis-ci.org/betteridiot/bamnostic.svg?branch=master
+   :target: https://travis-ci.org/betteridiot/bamnostic
+.. |Build status Appveyor| image:: https://ci.appveyor.com/api/projects/status/y95q02gkv3lgmlf4/branch/master?svg=true
+   :target: https://ci.appveyor.com/project/betteridiot/bamnostic/branch/master
+.. |noarch| image:: https://img.shields.io/circleci/project/github/conda-forge/bamnostic-feedstock/master.svg?label=noarch
+   :target: https://circleci.com/gh/conda-forge/bamnostic-feedstock
+.. |Downloads| image:: http://pepy.tech/badge/bamnostic
+   :target: http://pepy.tech/project/bamnostic
+.. |Conda Downloads| image:: https://img.shields.io/conda/dn/conda-forge/bamnostic.svg
+   :target: https://anaconda.org/conda-forge/bamnostic
+
```

### Comparing `bamnostic-1.1.7/bamnostic.egg-info/SOURCES.txt` & `bamnostic-1.1.8/bamnostic.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 ./CODE_OF_CONDUCT.md
```

### Comparing `bamnostic-1.1.7/setup.py` & `bamnostic-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `bamnostic-1.1.7/tests/test_build.py` & `bamnostic-1.1.8/tests/test_build.py`

 * *Files identical despite different names*

