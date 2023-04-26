# Comparing `tmp/PyMPDATA-MPI-0.0.1.tar.gz` & `tmp/PyMPDATA-MPI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMPDATA-MPI-0.0.1.tar", last modified: Sat Apr  8 20:00:07 2023, max compression
+gzip compressed data, was "PyMPDATA-MPI-0.0.2.tar", last modified: Wed Apr 26 11:03:55 2023, max compression
```

## Comparing `PyMPDATA-MPI-0.0.1.tar` & `PyMPDATA-MPI-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.467047 PyMPDATA-MPI-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.467047 PyMPDATA-MPI-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/.github/workflows/tests+pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.467047 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/domain_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/hdf_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-08 20:00:07.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-08 20:00:07.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:00:07.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-08 20:00:07.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-08 20:00:07.000000 PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:00:07.471047 PyMPDATA-MPI-0.0.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/resources/ground_truth.hdf5
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/test_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/test_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-08 19:59:53.000000 PyMPDATA-MPI-0.0.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.597055 PyMPDATA-MPI-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/.github/workflows/tests+pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/domain_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/hdf_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-04-26 11:03:55.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 11:03:55.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:03:55.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 11:03:55.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 11:03:55.000000 PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:55.601055 PyMPDATA-MPI-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/test_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-26 11:03:41.000000 PyMPDATA-MPI-0.0.2/tests/utils.py
```

### Comparing `PyMPDATA-MPI-0.0.1/.github/workflows/stale.yml` & `PyMPDATA-MPI-0.0.2/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.1/.github/workflows/tests+pypi.yml` & `PyMPDATA-MPI-0.0.2/.github/workflows/tests+pypi.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 name: tests+pypi
 
 defaults:
   run:
     shell: bash
 
+env:
+  arbitrarily_selected_artefact_set: '3.10/ubuntu-latest/0/openmpi'
+
 on:
   push:
     branches: [ main ]
   pull_request:
     branches: [ main ]
   schedule:
     - cron: '0 13 * * 4'
@@ -116,15 +119,28 @@
         run: brew install hdf5-mpi && echo HDF5_DIR=/opt/homebrew >> $GITHUB_ENV
       - run: HDF5_MPI="ON" CC=mpicc pip install --no-binary=h5py "git+https://github.com/h5py/h5py@81f6c01#egg=h5py"
       - run: pip install -e .
       - run: python -We -c "import PyMPDATA_MPI"
       - run: pip install pytest pytest-timeout pytest-mpi matplotlib
       - if: matrix.mpi == 'openmpi'
         run: echo _mpiexec_args="--oversubscribe" >> $GITHUB_ENV
-      - run: NUMBA_DISABLE_JIT=${{ matrix.disable-jit }} mpiexec $_mpiexec_args -n ${{ matrix.mpi-np }} pytest --timeout=360 --timeout_method=thread -s -vv -We;
+      - name: "mpiexec pytest"
+        env:
+          NUMBA_DISABLE_JIT: ${{ matrix.disable-jit }} 
+        run: |
+          if [ "$arbitrarily_selected_artefact_set" == "${{ matrix.python-version }}/${{ matrix.platform }}/${{ matrix.disable-jit }}/${{ matrix.mpi }}" ]; then
+            export CI_PLOTS_PATH=plots/$arbitrarily_selected_artefact_set
+            mkdir -p $CI_PLOTS_PATH
+          fi
+          mpiexec $_mpiexec_args -n ${{ matrix.mpi-np }} pytest --timeout=600 --timeout_method=thread -s -vv -We;
+      - uses: actions/upload-artifact@v2
+        with:
+          name: plots
+          path: plots
+
   dist:
     runs-on: ubuntu-latest
     needs: [tests]
     steps:
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0  # https://github.com/pypa/setuptools_scm/issues/480
@@ -147,7 +163,37 @@
           repository_url: https://test.pypi.org/legacy/
 
       - if: startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@unstable/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
 
+  tip-release-uploads:
+    runs-on: ubuntu-latest
+    needs: [tests]
+    steps:
+      - uses: actions/download-artifact@v2
+        with:
+          name: plots
+          path: plots
+      - run: |
+          sudo apt install -y librsvg2-bin
+          for path in plots/${{ env.arbitrarily_selected_artefact_set }}/*; do
+              for file in $path/*.svg; do
+                  rsvg-convert $file -o tmp.png
+                  convert tmp.png -flatten -trim +repage -bordercolor white -border 10 $file.png
+              done;
+              rm tmp.png
+              convert $path/*.png plots/`basename $path`-anim.gif 
+          done;
+
+      - uses: actions/upload-artifact@v2
+        with:
+          name: anims
+          path: plots/*-anim.gif
+
+      - if: github.ref == 'refs/heads/main'
+        uses: eine/tip@master
+        with:
+          token: ${{ secrets.GITHUB_TOKEN }}
+          files: plots/*-anim.gif
+          tag: 'latest-generated-plots'
```

### Comparing `PyMPDATA-MPI-0.0.1/.gitignore` & `PyMPDATA-MPI-0.0.2/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -153,8 +153,11 @@
 cython_debug/
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
-.idea/
+.idea/
+
+# macos
+.DS_Store
```

### Comparing `PyMPDATA-MPI-0.0.1/LICENSE` & `PyMPDATA-MPI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.1/PKG-INFO` & `PyMPDATA-MPI-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: PyMPDATA-MPI
-Version: 0.0.1
-Summary: TODO
-License: GPL-3.0
-Keywords: TODO,TODO
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyMPDATA-MPI
 
 [![Python 3](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3)](https://www.python.org/)
 [![LLVM](https://img.shields.io/static/v1?label=LLVM&logo=LLVM&color=gold&message=Numba)](https://numba.pydata.org)
 [![Linux OK](https://img.shields.io/static/v1?label=Linux&logo=Linux&color=yellow&message=%E2%9C%93)](https://en.wikipedia.org/wiki/Linux)
 [![macOS OK](https://img.shields.io/static/v1?label=macOS&logo=Apple&color=silver&message=%E2%9C%93)](https://en.wikipedia.org/wiki/macOS)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/open-atmos/PyMPDATA-MPI/graphs/commit-activity)
@@ -35,14 +17,45 @@
 [![Github Actions Build Status](https://github.com/open-atmos/PyMPDATA-MPI/workflows/tests+pypi/badge.svg?branch=main)](https://github.com/open-atmos/PyMPDATA-MPI/actions)
 [![PyPI version](https://badge.fury.io/py/PyMPDATA-MPI.svg)](https://pypi.org/project/PyMPDATA-MPI)
 [![API docs](https://img.shields.io/badge/API_docs-pdoc3-blue.svg)](https://open-atmos.github.io/PyMPDATA-MPI/)
 
 [PyMPDATA](https://github.com/open-atmos/PyMPDATA) +
 [numba-mpi](https://github.com/numba-mpi/numba-mpi) coupler sandbox (with a long-term goal of developing a pure-Python LES system)
 
+In principle, PyMPDATA-MPI adapts to API of PyMPDATA to solve the following equation in an environment with multiple nodes:
+$$\partial_t (G \psi) + \nabla \cdot (Gu \psi)= 0$$
+
+It is done with the help of MPI(Message Passing Interface). Every worker is responsible for computing its part of the decomposed domain.
+
+### 1 worker
+<p align="middle">
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_1_c_field_.-0.5.-0.25.-anim.gif" width="49%" /> 
+</p>
+
+### 2 workers
+<p align="middle">
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_2_c_field_.-0.5.-0.25.-anim.gif" width="49%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_2_c_field_.-0.5.-0.25.-anim.gif"  width="49%" /> 
+</p>
+
+### 3 workers
+<p align="middle">
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_3_c_field_.-0.5.-0.25.-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_3_c_field_.-0.5.-0.25.-anim.gif" width="32%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_3_c_field_.-0.5.-0.25.-anim.gif" width="32%" />
+</p>
+
+### 4 workers
+<p align="middle">
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_0_size_4_c_field_.-0.5.-0.25.-anim.gif" width="24%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_1_size_4_c_field_.-0.5.-0.25.-anim.gif" width="24%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_2_size_4_c_field_.-0.5.-0.25.-anim.gif" width="24%" />
+  <img src="https://github.com/open-atmos/PyMPDATA-MPI/releases/download/latest-generated-plots/n_iters.3_rank_3_size_4_c_field_.-0.5.-0.25.-anim.gif" width="24%" />
+</p>
+
 ## Credits:
 
 Development of PyMPDATA-MPI has been supported by the [Poland's National Science Centre](https://www.ncn.gov.pl/?language=en)  
 (grant no. 2020/39/D/ST10/01220).
 
 copyright: [Jagiellonian University](https://en.uj.edu.pl/en)    
 licence: [GPL v3](https://www.gnu.org/licenses/gpl-3.0.html)
```

### Comparing `PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/hdf_storage.py` & `PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/hdf_storage.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/periodic.py` & `PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 def _make_send_recv(set_value, jit_flags, fill_buf):
     @numba.njit(**jit_flags)
     def _send_recv(size, psi, i_rng, j_rng, k_rng, sign, dim, output):
         buf = np.empty(
             (
                 len(i_rng),
                 len(k_rng),
-            )
+            ),
+            dtype=output.dtype,
         )
 
         rank = mpi.rank()
         peers = (-1, (rank - 1) % size, (rank + 1) % size)  # LEFT  # RIGHT
 
         if SIGN_LEFT == sign:
             fill_buf(buf, psi, i_rng, k_rng, sign, dim)
```

### Comparing `PyMPDATA-MPI-0.0.1/PyMPDATA_MPI/simulation.py` & `PyMPDATA-MPI-0.0.2/PyMPDATA_MPI/simulation.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.1/PyMPDATA_MPI.egg-info/SOURCES.txt` & `PyMPDATA-MPI-0.0.2/PyMPDATA_MPI.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_2d.py
 tests/test_dependencies.py
 tests/test_hdf5.py
 tests/test_simulation.py
 tests/test_version.py
-tests/utils.py
-tests/resources/ground_truth.hdf5
+tests/utils.py
```

### Comparing `PyMPDATA-MPI-0.0.1/pyproject.toml` & `PyMPDATA-MPI-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Atmospheric Science",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Physics"
 ]
 dependencies = [
     "numba_mpi>=0.30",
-    "PyMPDATA>=1.0.10",
+    "PyMPDATA==1.0.10",
     "mpi4py",
     "h5py",
     "pytest-mpi"
 ]
 dynamic = ["version"]
```

### Comparing `PyMPDATA-MPI-0.0.1/tests/test_2d.py` & `PyMPDATA-MPI-0.0.2/tests/test_2d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # pylint: disable=missing-module-docstring,missing-function-docstring,
 # pylint: disable=missing-class-docstring,invalid-name,too-many-locals,too-many-arguments,c-extension-no-member
 # based on PyMPDATA README example
 
+import os
+import shutil
+from pathlib import Path
+
 import mpi4py
 import numba_mpi as mpi
 import numpy as np
 import pytest
 from matplotlib import pyplot
 from PyMPDATA import Options
 
@@ -44,55 +48,60 @@
             axis.pane.set_edgecolor("black")
             axis.pane.set_alpha(1)
         ax.grid(False)
         ax.set_zticks([])
         ax.set_xlabel("x/dx")
         ax.set_ylabel("y/dy")
         ax.set_proj_type("ortho")
-        cnt = ax.contourf(xi + 0.5, yi + 0.5, psi, zdir="z", offset=-1, norm=norm)
+        cnt = ax.contourf(
+            xi + 0.5,
+            yi + 0.5,
+            psi,
+            zdir="z",
+            offset=-1,
+            norm=norm,
+            levels=np.linspace(*zlim, 11),
+        )
         cbar = pyplot.colorbar(cnt, pad=0.1, aspect=10, fraction=0.04)
         return cbar.norm
 
 
-@pytest.mark.parametrize(
-    "options_kwargs",
-    (
-        {"n_iters": 1},
-        {"n_iters": 2},
-        {"n_iters": 2, "third_order_terms": True},
-        # {'n_iters': 2, 'nonoscillatory': True},  # TODO #36
-        {"n_iters": 3},
-    ),
+OPTIONS_KWARGS = (
+    {"n_iters": 1},
+    {"n_iters": 2, "third_order_terms": True},
+    {"n_iters": 2, "nonoscillatory": True},
+    {"n_iters": 3},
 )
-@pytest.mark.parametrize("n_threads", (1,))  # TODO #35 : 2+
-@pytest.mark.parametrize(
-    "output_steps",
-    (
-        (0,),
-        (0, 1),
-    ),
-)
-@pytest.mark.parametrize(
-    "courant_field",
-    (
-        (0.5, 0.25),
-        (-0.5, 0.25),
-        (0.5, -0.25),
-        (-0.5, -0.25),
-    ),
+
+COURANT_FIELDS = (
+    (0.5, 0.25),
+    (-0.5, 0.25),
+    (0.5, -0.25),
+    (-0.5, -0.25),
 )
+
+
+@pytest.mark.parametrize("options_kwargs", OPTIONS_KWARGS)
+@pytest.mark.parametrize("n_threads", (1,))  # TODO #35 : 2+
+@pytest.mark.parametrize("courant_field", COURANT_FIELDS)
 def test_2d(
     mpi_tmp_path_fixed,
     options_kwargs,
     n_threads,
-    output_steps,
     courant_field,
+    output_steps=range(0, 25, 2),
     grid=(24, 24),
-    plot=False,
 ):  # pylint: disable=redefined-outer-name
+    plot = (
+        "CI_PLOTS_PATH" in os.environ
+        and courant_field == COURANT_FIELDS[-1]
+        and options_kwargs == OPTIONS_KWARGS[-1]
+    )
+
+    # arrange
     options_str = (
         str(options_kwargs)
         .replace(", ", "_")
         .replace(": ", "=")
         .replace("'", "")
         .replace("{", "")
         .replace("}", "")
@@ -104,18 +113,29 @@
     }
 
     Storage = HDFStorage
     dataset_name = "test"
 
     settings = ReadmeSettings(output_steps)
 
+    # act
     for mpi_max_size, path in paths.items():
         truncated_size = min(mpi_max_size, mpi.size())
         rank = mpi.rank()
 
+        courant_str = str(courant_field).replace(" ", "")
+
+        plot_path = None
+        if plot:
+            plot_path = Path(os.environ["CI_PLOTS_PATH"]) / Path(
+                f"{options_str}_rank_{mpi.rank()}_size_{mpi.size()}_c_field_{courant_str}"
+            )
+            shutil.rmtree(plot_path, ignore_errors=True)
+            os.mkdir(plot_path)
+
         if rank == 0:
             Storage.create_dataset(
                 name=dataset_name, path=path, grid=grid, steps=settings.output_steps
             )
 
         with Storage.mpi_context(
             path, "r+", mpi4py.MPI.COMM_WORLD.Split(rank < truncated_size, rank)
@@ -128,33 +148,38 @@
                     grid=grid,
                     rank=rank,
                     size=truncated_size,
                     initial_condition=settings.initial_condition,
                     courant_field=courant_field,
                 )
                 steps_done = 0
+                x_range = slice(*subdomain(grid[0], rank, truncated_size))
+
                 for i, output_step in enumerate(settings.output_steps):
                     n_steps = output_step - steps_done
                     simulation.advance(n_steps=n_steps)
                     steps_done += n_steps
-
-                    x_range = slice(*subdomain(grid[0], rank, truncated_size))
                     dataset[x_range, :, i] = simulation.advectee.get()
 
+                # plot
+                if plot:
+                    tmp = np.empty_like(dataset[:, :, -1])
+                    for i, _ in enumerate(settings.output_steps):
+                        tmp[:] = np.nan
+                        tmp[x_range, :] = dataset[x_range, :, i]
+                        settings.quick_look(tmp, zlim=(-1, 1))
+                        filename = f"step={i:04d}.svg"
+                        pyplot.savefig(plot_path / filename)
+                        pyplot.close()
+
+    # assert
     with barrier_enclosed():
         if mpi.rank() != 0:
             with Storage.non_mpi_contex(
                 paths[1], "r"
             ) as storage_expected, Storage.non_mpi_contex(
                 paths[mpi.rank() + 1], "r"
             ) as storage_actual:
-                settings.quick_look(
-                    storage_actual[dataset_name][:, :, -1], zlim=(-1, 1)
-                )
-                if plot:
-                    plot_path = f"{options_str}_threads_{n_threads}.pdf"
-                    pyplot.savefig(mpi_tmp_path_fixed / plot_path)
-                pyplot.close()
                 np.testing.assert_array_equal(
                     storage_expected[dataset_name][:, :, -1],
                     storage_actual[dataset_name][:, :, -1],
                 )
```

### Comparing `PyMPDATA-MPI-0.0.1/tests/test_hdf5.py` & `PyMPDATA-MPI-0.0.2/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `PyMPDATA-MPI-0.0.1/tests/test_simulation.py` & `PyMPDATA-MPI-0.0.2/tests/test_simulation.py`

 * *Files identical despite different names*

