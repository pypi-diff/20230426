# Comparing `tmp/scalib-0.5.3.tar.gz` & `tmp/scalib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalib-0.5.3.tar", last modified: Tue Feb 21 10:20:12 2023, max compression
+gzip compressed data, was "scalib-0.5.4.tar", last modified: Wed Apr 26 15:01:45 2023, max compression
```

## Comparing `scalib-0.5.3.tar` & `scalib-0.5.4.tar`

### file list

```diff
@@ -1,571 +1,573 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.260930 scalib-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.264930 scalib-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-02-21 10:20:03.000000 scalib-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-02-21 10:20:03.000000 scalib-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.264930 scalib-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-02-21 10:20:03.000000 scalib-0.5.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-21 10:20:03.000000 scalib-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-21 10:20:03.000000 scalib-0.5.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-02-21 10:20:03.000000 scalib-0.5.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-02-21 10:20:03.000000 scalib-0.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-21 10:20:03.000000 scalib-0.5.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-02-21 10:20:03.000000 scalib-0.5.3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-02-21 10:20:03.000000 scalib-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-02-21 10:20:03.000000 scalib-0.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-02-21 10:20:12.320931 scalib-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-02-21 10:20:03.000000 scalib-0.5.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.260930 scalib-0.5.3/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/source/api_ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 10:20:03.000000 scalib-0.5.3/docs/source/copyright.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-02-21 10:20:03.000000 scalib-0.5.3/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-02-21 10:20:03.000000 scalib-0.5.3/examples/aes_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-21 10:20:03.000000 scalib-0.5.3/examples/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-02-21 10:20:03.000000 scalib-0.5.3/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/paper/
--rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-02-21 10:20:03.000000 scalib-0.5.3/paper/build_paper.sh
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-02-21 10:20:03.000000 scalib-0.5.3/paper/paper.bib
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-02-21 10:20:03.000000 scalib-0.5.3/paper/paper.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-21 10:20:03.000000 scalib-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-21 10:20:12.324931 scalib-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-21 10:20:03.000000 scalib-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.260930 scalib-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib/attacks/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/attacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/attacks/factor_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/attacks/sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib/build_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/config/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/metrics/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/metrics/ttest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/modeling/ldaclassifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.272930 scalib-0.5.3/src/scalib/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/postprocessing/rankestimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.268931 scalib-0.5.3/src/scalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26973 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 10:20:11.000000 scalib-0.5.3/src/scalib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-21 10:20:12.000000 scalib-0.5.3/src/scalib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.272930 scalib-0.5.3/src/scalib_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    43870 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.272930 scalib-0.5.3/src/scalib_ext/geigen/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.272930 scalib-0.5.3/src/scalib_ext/geigen/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.276930 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Cholesky
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/CholmodSupport
--rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Core
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Dense
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Eigen
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Eigenvalues
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Geometry
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Householder
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Jacobi
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/LU
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/MetisSupport
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/OrderingMethods
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/PardisoSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/QR
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SPQRSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SVD
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Sparse
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseCholesky
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseCore
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseLU
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseQR
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdDeque
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdList
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdVector
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.264930 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.276930 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.276930 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.260930 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.284931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.288931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.288931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/
--rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.292931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.292931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.292931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/
--rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.296931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.300931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/
--rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.300931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.304931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.308931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.308931 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.308931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.308931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
--rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
--rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
--rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/Version.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/include/geigen.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/geigen/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/src/geigen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/src/geigen.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/geigen/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/ranklib/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/build.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/ranklib/fuzz/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/fuzz/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/fuzz/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.312931 scalib-0.5.3/src/scalib_ext/ranklib/fuzz/fuzz_targets/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.316931 scalib-0.5.3/src/scalib_ext/ranklib/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/aes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/aes.h
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/bignumpoly.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/bignumpoly.h
--rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_enum.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_enum.h
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_execute.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_execute.h
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_histo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_histo.h
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_if.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_if.h
--rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_init.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_init.h
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_struct.h
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_util.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/hel_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/histogram.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/main_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/rank.rs
--rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/score_example_data.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example.h
--rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example_data.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/ranklib/src/top.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.316931 scalib-0.5.3/src/scalib_ext/scalib/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/src/scalib_ext/scalib/benches/
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/benches/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/benches/get_snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/benches/mttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/benches/snr_update.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/benches/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/src/scalib_ext/scalib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/matrixmul.rs
--rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/mttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/
--rw-r--r--   0 runner    (1001) docker     (123)    26588 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    20946 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/bp_compute.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/fg_build.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/fg_parser.rs
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/sasca/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/ttest.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/src/scalib_ext/scalib/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/tests/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/tests/multivarcs.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib/tests/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.316931 scalib-0.5.3/src/scalib_ext/scalib-py/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/src/scalib_ext/scalib-py/src/
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/belief_propagation.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/factor_graph.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/lda.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/ranking.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/snr.rs
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/thread_pool.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-02-21 10:20:03.000000 scalib-0.5.3/src/scalib_ext/scalib-py/src/ttest.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 10:20:12.320931 scalib-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/mttest_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22716 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_factorgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_lda.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_sascagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-21 10:20:03.000000 scalib-0.5.3/tests/test_ttest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-21 10:20:03.000000 scalib-0.5.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-26 15:01:30.000000 scalib-0.5.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 15:01:30.000000 scalib-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 15:01:30.000000 scalib-0.5.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-26 15:01:30.000000 scalib-0.5.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-26 15:01:30.000000 scalib-0.5.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 15:01:30.000000 scalib-0.5.4/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-26 15:01:30.000000 scalib-0.5.4/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-26 15:01:30.000000 scalib-0.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-26 15:01:30.000000 scalib-0.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 15:01:45.173366 scalib-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-04-26 15:01:30.000000 scalib-0.5.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/api_ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 15:01:30.000000 scalib-0.5.4/docs/source/copyright.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/aes_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 15:01:30.000000 scalib-0.5.4/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.097365 scalib-0.5.4/paper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/build_paper.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/paper.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-04-26 15:01:30.000000 scalib-0.5.4/paper/paper.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-26 15:01:30.000000 scalib-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-26 15:01:45.177367 scalib-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-04-26 15:01:30.000000 scalib-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/attacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/factor_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/attacks/sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib/build_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/config/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/metrics/ttest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/modeling/ldaclassifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/postprocessing/rankestimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27013 2023-04-26 15:01:45.000000 scalib-0.5.4/src/scalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 15:01:44.000000 scalib-0.5.4/src/scalib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    45960 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/geigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.101365 scalib-0.5.4/src/scalib_ext/geigen/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.105365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Cholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner    (1001) docker     (123)    18103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Core
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Dense
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigen
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Geometry
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Householder
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Jacobi
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/LU
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/MetisSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PaStiXSupport
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QR
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SVD
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Sparse
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCore
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseLU
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseQR
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdDeque
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdList
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdVector
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.093365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.105365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24480 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18395 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.109365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38153 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12479 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18064 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62197 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31424 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27551 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22205 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21123 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    41000 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19067 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20694 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45354 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51070 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37304 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29441 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.089365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner    (1001) docker     (123)    18037 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27841 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner    (1001) docker     (123)    15528 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    50865 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.117365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37671 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23547 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)    35476 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner    (1001) docker     (123)    17706 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28726 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    19426 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35843 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32283 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.121365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18263 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27946 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.125365 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner    (1001) docker     (123)    81646 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18887 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11570 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9901 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13867 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14722 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.129366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4360 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4026 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner    (1001) docker     (123)    38322 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner    (1001) docker     (123)    40579 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21356 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10518 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner    (1001) docker     (123)    34903 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.129366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22944 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner    (1001) docker     (123)    23586 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20749 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    33705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4104 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22444 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)    14815 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8308 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60555 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6190 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15234 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11527 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner    (1001) docker     (123)    13662 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner    (1001) docker     (123)    16396 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    62266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    22248 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.141366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    20060 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20805 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25478 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    11405 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/
+-rw-r--r--   0 runner    (1001) docker     (123)    49870 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32949 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.145366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.149366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner    (1001) docker     (123)    10670 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25592 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25840 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12487 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12589 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52401 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7049 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25721 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14831 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner    (1001) docker     (123)    27844 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner    (1001) docker     (123)    28373 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    34345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner    (1001) docker     (123)    17202 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.153366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    30560 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)  1058368 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16929 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)    37403 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18186 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.157366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14768 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10177 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/Version.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.161366 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    19212 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/include/geigen.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/geigen/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/geigen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/geigen.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/geigen/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/build.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.165366 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/ranklib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/aes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/aes.h
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22744 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_struct.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/histogram.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16237 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/main_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/rank.rs
+-rw-r--r--   0 runner    (1001) docker     (123)   274225 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/score_example_data.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.h
+-rw-r--r--   0 runner    (1001) docker     (123)   224884 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example_data.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/ranklib/src/top.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib/benches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/get_snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/mttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/snr_update.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/benches/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24746 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/matrixmul.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/mttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/
+-rw-r--r--   0 runner    (1001) docker     (123)    26307 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    22085 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/bp_compute.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    10791 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_build.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_parser.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/sasca/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    18507 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/ttest.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/src/scalib_ext/scalib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/multivarcs.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib/tests/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib-py/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.169366 scalib-0.5.4/src/scalib_ext/scalib-py/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/belief_propagation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12818 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/factor_graph.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/lda.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/ranking.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/snr.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/thread_pool.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-26 15:01:30.000000 scalib-0.5.4/src/scalib_ext/scalib-py/src/ttest.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:01:45.173366 scalib-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/mttest_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23611 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_factorgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_lda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_sascagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-26 15:01:30.000000 scalib-0.5.4/tests/test_ttest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-26 15:01:30.000000 scalib-0.5.4/tox.ini
```

### Comparing `scalib-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md` & `scalib-0.5.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md` & `scalib-0.5.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/.github/workflows/ci.yml` & `scalib-0.5.4/.github/workflows/ci.yml`

 * *Files 9% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             - name: Formatting
               run:
                 make codestyle
             - name: Docs
               run:
                 make docs
     test:
+        name: Run tests (on linux).
         needs: [build_wheel_linux]
         runs-on: ubuntu-latest
         strategy:
             fail-fast: false
             matrix:
                 python: ["3.8", "3.11"]
         steps:
@@ -121,65 +122,65 @@
               with:
                   path: |
                       ${{ runner.temp }}/cargo_build
                       ${{ runner.temp }}/cargo_home
                   key: windows-wheel-cache-rust-build-cargo-v1-${{ matrix.arch}}
             - uses: actions/setup-python@v3
               with:
-                  python-version: "3.10"
+                  python-version: "3.8"
             - name: wheels Windows ${{ matrix.arch}}
               uses: pypa/cibuildwheel@v2.12.0
               env:
                 CARGO_TARGET_DIR: "${{ runner.temp }}\\cargo_build"
                 CARGO_HOME: "${{ runner.temp }}\\cargo_home"
                 CIBW_PLATFORM: "windows"
                 CIBW_TEST_COMMAND: pytest {project}/tests
                 CIBW_TEST_REQUIRES: "-r tests/requirements.txt"
             - uses: actions/upload-artifact@v3
               with:
                   name: dist
                   path: ./wheelhouse/*.whl
 
-#    build_wheel_macos:
-#        name: Build wheels on macos ${{ matrix.vers }}
-#        runs-on: macos-10.15
-#        strategy:
-#            fail-fast: false
-#            matrix:
-#                include:
-#                   #- vers: arm64
-#                   - vers: x86_64
-#        env:
-#            CIBW_BUILD_VERBOSITY: "1"
-#            CIBW_ENVIRONMENT: 'RUST_BACKTRACE=full'
-#            CIBW_BUILD: "cp36-*"
-#            # I don't know how to make both normal and doctring tests work with only one command,
-#            # so I use shell &&.
-#            CIBW_TEST_COMMAND: pytest -ra {project}/tests && pytest -ra --pyargs --doctest-modules scalib
-#            CIBW_TEST_EXTRAS: test
-#            CIBW_ARCHS_MACOS: ${{ matrix.vers }}
-#            CARGO_TARGET_DIR: ${{ github.workspace }}/cargo_build
-#        steps:
-#            - uses: actions/checkout@v2
-#            - uses: actions/cache@v2
-#              with:
-#                  path: |
-#                      ~/.cargo/registry
-#                      ~/.cargo/git
-#                      ${{ github.workspace }}/cargo_build
-#                  key: cache-macos-cargo-v0
-#            - uses: actions/setup-python@v2
-#              with:
-#                  python-version: "3.6"
-#            - name: wheels Macos ${{ matrix.vers }}
-#              uses: joerick/cibuildwheel@v1.10.0
-#            - uses: actions/upload-artifact@v2
-#              with:
-#                  name: dist
-#                  path: ./wheelhouse/*.whl
+    build_wheel_macos:
+        name: Build wheels on Mac Os (${{ matrix.vers }})
+        runs-on: macos-latest
+        strategy:
+            fail-fast: false
+            matrix:
+                include:
+                   - vers: arm64
+                   - vers: x86_64
+        steps:
+            - uses: actions/checkout@v3
+            - uses: actions/cache@v3
+              with:
+                  path: |
+                      ${{ runner.temp }}/cargo_build
+                      ${{ runner.temp }}/cargo_home
+                  key: macos-wheel-cache-rust-build-cargo-v1-${{ matrix.arch}}
+            - uses: actions/setup-python@v3
+              with:
+                  python-version: "3.8"
+            - name: add aarch64 lib
+              if: ${{ matrix.vers }} == 'arm64'
+              run: "rustup target add aarch64-apple-darwin"
+            - name: wheels Mac Os ${{ matrix.vers }}
+              uses: joerick/cibuildwheel@v2.12.0
+              env:
+                CARGO_TARGET_DIR: "${{ runner.temp }}\\cargo_build"
+                CARGO_HOME: "${{ runner.temp }}\\cargo_home"
+                CIBW_PLATFORM: "macos"
+                CIBW_TEST_COMMAND: pytest {project}/tests
+                CIBW_TEST_REQUIRES: "-r tests/requirements.txt"
+                CIBW_ARCHS_MACOS: "${{ matrix.vers}}"
+                CIBW_ENVIRONMENT_MACOS: "SCALIB_AVX2=0"
+            - uses: actions/upload-artifact@v3
+              with:
+                  name: dist
+                  path: ./wheelhouse/*.whl
 
     build_sdist:
         name: Build source distribution
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v3
             - name: Build sdist
@@ -188,15 +189,15 @@
                   python -m build --sdist .
             - uses: actions/upload-artifact@v3
               with:
                   name: dist
                   path: dist/*.tar.gz
 
     check_dist:
-        needs: [build_wheel_linux, build_wheel_windows, build_sdist]
+        needs: [build_wheel_linux, build_wheel_windows, build_wheel_macos, build_sdist]
         runs-on: ubuntu-latest
         steps:
             - uses: actions/download-artifact@v3
               with:
                   name: dist
                   path: dist
             - name: Install twine
```

### Comparing `scalib-0.5.3/CHANGELOG.rst` & `scalib-0.5.4/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 =========
 Changelog
 =========
 
 Not released
 ------------
 
+v0.5.4 (2023/04/26)
+-------------------
+
+* Run CI on Mac Os and build wheels (x86_64 and arm64, but we test only x86_64). No AVX2 due to old runner in github CI.
+* Add ``scalib.tools.ContextExecutor``, as a solution to ``LookupError`` in
+  ``get_config()``.
+* Fix numerical underflow in ``BPState`` when multiple traces are used.
+* Fix missing import in ``MultiLDA``.
+* Run ``BPState`` methods on the threadpool.
+* Make threadpool initalization lazy -- makes SCALib play more nicely with ``ProcessPoolExecutor``.
+
 v0.5.3 (2023/02/21)
 -------------------
 
 * Add ``vars`` and ``factors`` methods on `FactorGraph`.
 * Add ``fg`` property on `BPState`.
 * Fix bug in belief propagation. Numerical instabilities could lead to negative
   probabilities for AND (and probably XOR and ADD) factors.
```

### Comparing `scalib-0.5.3/CONTRIBUTING.rst` & `scalib-0.5.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/COPYING` & `scalib-0.5.4/COPYING`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/COPYRIGHT` & `scalib-0.5.4/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/MANIFEST.in` & `scalib-0.5.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/Makefile` & `scalib-0.5.4/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	@echo "    wheel_avx2: Build a wheel with AVX2 instruction (should work on any recent x86-64)."
 
 dev:
 	tox run -e dev
 
 test:
 	tox run -e fmt -- --check
+	RUST_BACKTRACE=1 CARGO_TARGET_DIR=.cargo_build cargo test --workspace --manifest-path src/scalib_ext/Cargo.toml
 	tox run -e test
 
 coverage:
 	tox run -e test
 	tox run -e coverage
 	@echo "Open htmlcov/index.html to see detailled coverage information."
```

### Comparing `scalib-0.5.3/PKG-INFO` & `scalib-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
 Requires-Python: >=3.8
@@ -27,15 +27,15 @@
 The Side-Channel Analysis Library (SCALib) is a Python package that
 contains state-of-the-art tools for side-channel security evaluation. It focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
-SCALib should be useful for any side-channel practitionner who wants to
+SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
 
 See the documentation_ for the list of implemented tools.
 
 We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
 announcements, questions, community support and discussions.
@@ -89,15 +89,15 @@
 
 Please also let us know your needs by opening a 
 `feature request <https://github.com/simple-crypto/SCALib/issues/new?assignees=&labels=&template=feature_request.md&title=>`_.
 
 Versioning policy
 =================
 
-SCALib uses `semantic versioing <https://semver.org/>`_, see the `CHANGELOG
+SCALib uses `semantic versioning <https://semver.org/>`_, see the `CHANGELOG
 <CHANGELOG.rst>`_ for breaking changes and novelties.
 
 About us
 ========
 SCALib was initiated by Olivier Bronchain and Gaëtan Cassiers during their PhD
 at UCLouvain. It is now developed as a project of
 `SIMPLE-Crypto <https://www.simple-crypto.dev/>`_ and maintained by Gaëtan Cassiers (@cassiersg).
```

### Comparing `scalib-0.5.3/README.rst` & `scalib-0.5.4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 The Side-Channel Analysis Library (SCALib) is a Python package that
 contains state-of-the-art tools for side-channel security evaluation. It focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
-SCALib should be useful for any side-channel practitionner who wants to
+SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
 
 See the documentation_ for the list of implemented tools.
 
 We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
 announcements, questions, community support and discussions.
@@ -76,15 +76,15 @@
 
 Please also let us know your needs by opening a 
 `feature request <https://github.com/simple-crypto/SCALib/issues/new?assignees=&labels=&template=feature_request.md&title=>`_.
 
 Versioning policy
 =================
 
-SCALib uses `semantic versioing <https://semver.org/>`_, see the `CHANGELOG
+SCALib uses `semantic versioning <https://semver.org/>`_, see the `CHANGELOG
 <CHANGELOG.rst>`_ for breaking changes and novelties.
 
 About us
 ========
 SCALib was initiated by Olivier Bronchain and Gaëtan Cassiers during their PhD
 at UCLouvain. It is now developed as a project of
 `SIMPLE-Crypto <https://www.simple-crypto.dev/>`_ and maintained by Gaëtan Cassiers (@cassiersg).
```

### Comparing `scalib-0.5.3/docs/Makefile` & `scalib-0.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/docs/_templates/autosummary/class.rst` & `scalib-0.5.4/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/docs/_templates/autosummary/module.rst` & `scalib-0.5.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/docs/conf.py` & `scalib-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/docs/index.rst` & `scalib-0.5.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/docs/make.bat` & `scalib-0.5.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/examples/README.rst` & `scalib-0.5.4/examples/README.rst`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/examples/aes_simulation.py` & `scalib-0.5.4/examples/aes_simulation.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/examples/utils.py` & `scalib-0.5.4/examples/utils.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/paper/paper.bib` & `scalib-0.5.4/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/paper/paper.md` & `scalib-0.5.4/paper/paper.md`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/pyproject.toml` & `scalib-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/setup.cfg` & `scalib-0.5.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = Side-Channel Analysis Library
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/simple-crypto/scalib
 author = Olivier Bronchain, Gaëtan Cassiers
 author_email = olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 license = GNU AGPL v3+
-license_file = COPYING
+license_files = COPYING
 
 [options]
 package_dir = 
 	=src
 packages = find:
 zip_safe = False
 python_requires = >=3.8
```

### Comparing `scalib-0.5.3/setup.py` & `scalib-0.5.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,25 +19,27 @@
     raise ValueError("Cannot have both SCALIB_PORTABLE and SCALIB_AVX2.")
 
 # We check only for AVX2, as this is the CI default, otherwise we assume local
 # builds.
 with open("src/scalib/build_config.py", "w") as f:
     f.write(f"REQUIRE_AVX2 = {use_avx2}\n")
 
+
 if noflags or portable:
     rustflags = None
 elif use_avx2:
     rustflags = "-C target-feature=+avx2"
 else:
     rustflags = "-C target-cpu=native"
 
 if rustflags:
     rustflags = os.environ.get('RUSTFLAGS', '') + ' ' + rustflags
     os.environ["RUSTFLAGS"] = rustflags
 
+print(f"Build config: {noflags=} {portable=} {use_avx2=} {rustflags=}.")
 
 scalib_features = ["pyo3/abi3"]
 
 if sys.platform == "linux":
     scalib_features.append("blis")
 
 setup(
```

### Comparing `scalib-0.5.3/src/scalib/__init__.py` & `scalib-0.5.4/src/scalib/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
-__all__ = ["metrics", "attacks", "modeling", "postprocessing", "config", "ScalibError"]
+__all__ = [
+    "config",
+    "attacks",
+    "metrics",
+    "modeling",
+    "postprocessing",
+    "tools",
+    "ScalibError",
+]
 
 import cpuinfo
 
 from .build_config import REQUIRE_AVX2
 from .version import version as __version__
 
 cpu = cpuinfo.get_cpu_info()
 
-
-if REQUIRE_AVX2 and cpu["arch"] == "X68_64" and "avx2" not in cpu["flags"]:
+if REQUIRE_AVX2 and cpu["arch"] == "X86_64" and "avx2" not in cpu["flags"]:
     raise ImportError(
         "SCALib has been compiled with AVX2 instructions, which are not "
         + "supported by your CPU or OS. See "
         + "https://github.com/simple-crypto/SCALib/blob/main/README.rst "
         + "for compiling without AVX2 instructions."
     )
```

### Comparing `scalib-0.5.3/src/scalib/attacks/factor_graph.py` & `scalib-0.5.4/src/scalib/attacks/factor_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Sequence, Mapping, Union, Optional
 
 import numpy as np
 import numpy.typing as npt
 
 from scalib import _scalib_ext
+from scalib.config import get_config
 
 __all__ = ["FactorGraph", "BPState"]
 
 CstValue = Union[int, Sequence[int]]
 ValsAssign = Mapping[str, CstValue]
 
 
@@ -218,16 +219,16 @@
         it :
             Number of iterations of belief propagation.
         initialize_states:
             Whether to update variable distributions before running the BP iterations.
             Recommended after using :func:`BPState.set_evidence`.
         """
         if initialize_states:
-            self._inner.propagate_all_vars()
-        self._inner.propagate_loopy_step(it)
+            self._inner.propagate_all_vars(get_config())
+        self._inner.propagate_loopy_step(it, get_config())
 
     def bp_acyclic(
         self,
         dest: str,
         *,
         clear_intermediates: bool = True,
         clear_evidence: bool = False,
@@ -240,15 +241,17 @@
         dest:
             Variable for which the belief propagation is computed.
         clear_intermediates:
             Drop the intermetidate distributions and beliefs that are computed.
         clear_evidence:
             Drop the evidence for the variables, once used in the algorithm.
         """
-        self._inner.propagate_acyclic(dest, clear_intermediates, clear_evidence)
+        self._inner.propagate_acyclic(
+            dest, clear_intermediates, clear_evidence, get_config()
+        )
 
     def get_distribution(self, var: str) -> Optional[npt.NDArray[np.float64]]:
         r"""Returns the current distribution of a variable `var`.
 
         Parameters
         ----------
         var : string
@@ -340,29 +343,29 @@
 
         Parameters
         ----------
         var : string
             Identifier of the variable.
 
         """
-        return self._inner.propagate_var(var)
+        return self._inner.propagate_var(var, get_config())
 
     def propagate_factor(self, factor: str):
         """Run belief propagation on the given factor.
 
         This fetches beliefs from adjacent variables and sends updated beliefs
         to all adjacent variables.
 
         Parameters
         ----------
         var : string
             Identifier of the variable.
 
         """
-        return self._inner.propagate_factor_all(factor)
+        return self._inner.propagate_factor_all(factor, get_config())
 
     def debug(self):
         """Debug-print the current state."""
         s = []
         s.append("VAR DISTRIBUTION")
         for var in self._inner.graph().var_names():
             s.append(f"\tVar {var}")
```

### Comparing `scalib-0.5.3/src/scalib/attacks/sascagraph.py` & `scalib-0.5.4/src/scalib/attacks/sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib/config/__init__.py` & `scalib-0.5.4/src/scalib/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,8 +139,17 @@
     # Use __init__ function instead of creating new object as we want to update
     # the object in-place.
     _default.__init__(**kwargs)
 
 
 def get_config():
     """Get the current config, to give to Rust functions."""
-    return _current.get()
+    try:
+        return _current.get()
+    except LookupError:
+        # TODO: use add_note on the orignal exception once we drop support for python 3.10.
+        raise Exception(
+            "Using SCALib from a thread without contextvars propagation is not supported.\n"
+            + "We provide scalib.tools.ContextExecutor as a contextvars-aware replacement\n"
+            + "for concurrent.futures.ThreadPoolExecutor.\n"
+            + "See https://github.com/simple-crypto/SCALib/issues/89 for more information."
+        )
```

### Comparing `scalib-0.5.3/src/scalib/metrics/snr.py` & `scalib-0.5.4/src/scalib/metrics/snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib/metrics/ttest.py` & `scalib-0.5.4/src/scalib/metrics/ttest.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib/modeling/__init__.py` & `scalib-0.5.4/src/scalib/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib/modeling/ldaclassifier.py` & `scalib-0.5.4/src/scalib/modeling/ldaclassifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 import numpy as np
 
 from scalib import _scalib_ext
 from scalib.config import get_config
+import scalib.tools
 import scalib.utils
 
 
 class LDAClassifier:
     r"""Models the leakage :math:`\mathbf{l}` with :math:`n_s` dimensions using
     the linear discriminant analysis classifier (LDA) with integrated
     dimensionality reduction.
@@ -256,29 +257,29 @@
             must be `uint16`.
         """
         # Try to avoid the over-subscription of CPUs.
         num_threads = get_config().threadpool.n_threads
         if self.gemm_mode != 0:
             num_threads = max(1, num_threads // self.gemm_mode)
         with scalib.utils.interruptible():
-            with scalib.utils.ContextExecutor(max_workers=num_threads) as executor:
+            with scalib.tools.ContextExecutor(max_workers=num_threads) as executor:
                 list(
                     executor.map(
                         lambda i: self.ldas[i].fit_u(
                             l[:, self.pois[i]], x[:, i], self.gemm_mode
                         ),
                         range(len(self.ldas)),
                     )
                 )
 
     def solve(self, done=False):
         """See `LDAClassifier.solve`."""
         # Put as much work as needed to fill rayon threadpool
         with scalib.utils.interruptible():
-            with scalib.utils.ContextExecutor(
+            with scalib.tools.ContextExecutor(
                 max_workers=get_config().threadpool.n_threads
             ) as executor:
                 list(executor.map(lambda lda: lda.solve(done), self.ldas))
 
     def predict_proba(self, l):
         """Predict probabilities for all variables.
 
@@ -292,15 +293,15 @@
         -------
         list of array_like, f64
             Probabilities. `nv` arrays of shape `(n, nc)`.
         See `LDAClassifier.solve`.
         """
         # Put as much work as needed to fill rayon threadpool
         with scalib.utils.interruptible():
-            with scalib.utils.ContextExecutor(
+            with scalib.tools.ContextExecutor(
                 max_workers=get_config().threadpool.n_threads
             ) as executor:
                 return list(
                     executor.map(
                         lambda i: self.ldas[i].predict_proba(l[:, self.pois[i]]),
                         range(len(self.ldas)),
                     )
```

### Comparing `scalib-0.5.3/src/scalib/postprocessing/rankestimation.py` & `scalib-0.5.4/src/scalib/postprocessing/rankestimation.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,16 @@
         Correct full key split in sub-keys. Array must be of shape `(ns,)`.
     nbins : int
         Number of bins for each of the distributions.
     method : string
         Method used to estimate the rank. Can be the following:
 
         * "hist": using histograms (default).
-        * "ntl": using NTL library, allows better precision.
+        * "naive": enumerate possible keys (very slow).
+        * "histbignum": using NTL library, allows better precision.
 
     Returns
     -------
     (rmin, r, rmax): (float, float, float)
 
             - **rmin** is a lower bound for the key rank.
             - **r** is the estimated key rank.
```

### Comparing `scalib-0.5.3/src/scalib.egg-info/PKG-INFO` & `scalib-0.5.4/src/scalib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Side-Channel Analysis Library
 Home-page: https://github.com/simple-crypto/scalib
 Author: Olivier Bronchain, Gaëtan Cassiers
 Author-email: olivier.bronchain@uclouvain.be, gaetan.cassiers@uclouvain.be
 License: GNU AGPL v3+
 Project-URL: Bug Tracker, https://github.com/simple-crypto/scalib/issues
 Requires-Python: >=3.8
@@ -27,15 +27,15 @@
 The Side-Channel Analysis Library (SCALib) is a Python package that
 contains state-of-the-art tools for side-channel security evaluation. It focuses on
 
 - simple interface,
 - state-of-the art algorithms,
 - excellent performance (see `benchmarks <https://github.com/cassiersg/SCABench>`_).
 
-SCALib should be useful for any side-channel practitionner who wants to
+SCALib should be useful for any side-channel practitioner who wants to
 evaluate, but not necessarily attack, protected or non-protected
 implementations.
 
 See the documentation_ for the list of implemented tools.
 
 We have a `matrix chat <https://matrix.to/#/#scalib:matrix.org>`_ for
 announcements, questions, community support and discussions.
@@ -89,15 +89,15 @@
 
 Please also let us know your needs by opening a 
 `feature request <https://github.com/simple-crypto/SCALib/issues/new?assignees=&labels=&template=feature_request.md&title=>`_.
 
 Versioning policy
 =================
 
-SCALib uses `semantic versioing <https://semver.org/>`_, see the `CHANGELOG
+SCALib uses `semantic versioning <https://semver.org/>`_, see the `CHANGELOG
 <CHANGELOG.rst>`_ for breaking changes and novelties.
 
 About us
 ========
 SCALib was initiated by Olivier Bronchain and Gaëtan Cassiers during their PhD
 at UCLouvain. It is now developed as a project of
 `SIMPLE-Crypto <https://www.simple-crypto.dev/>`_ and maintained by Gaëtan Cassiers (@cassiersg).
```

### Comparing `scalib-0.5.3/src/scalib.egg-info/SOURCES.txt` & `scalib-0.5.4/src/scalib.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 examples/test_examples.py
 examples/utils.py
 paper/build_paper.sh
 paper/paper.bib
 paper/paper.md
 src/scalib/__init__.py
 src/scalib/build_config.py
+src/scalib/tools.py
 src/scalib/utils.py
 src/scalib/version.py
 src/scalib.egg-info/PKG-INFO
 src/scalib.egg-info/SOURCES.txt
 src/scalib.egg-info/dependency_links.txt
 src/scalib.egg-info/not-zip-safe
 src/scalib.egg-info/requires.txt
@@ -482,8 +483,9 @@
 tests/mttest_test.py
 tests/requirements.txt
 tests/test_factorgraph.py
 tests/test_lda.py
 tests/test_postprocessing.py
 tests/test_sascagraph.py
 tests/test_snr.py
+tests/test_tools.py
 tests/test_ttest.py
```

### Comparing `scalib-0.5.3/src/scalib_ext/.gitignore` & `scalib-0.5.4/src/scalib_ext/.gitignore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/Cargo.lock` & `scalib-0.5.4/src/scalib_ext/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.3.8"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e8fd72866655d1904d6b0997d0b07ba561047d070fbe29de039031c641b61217"
+checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
 dependencies = [
- "const-random",
+ "getrandom",
+ "once_cell",
+ "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
 version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
+name = "anes"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
+
+[[package]]
 name = "ansi_term"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
 dependencies = [
  "winapi",
 ]
@@ -35,14 +43,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f2a05fd1bd10b2527e20a2cd32d8873d115b8b39fe219ee25f42a8aca6ba278"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "approx"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "arbitrary"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e90af4de65aa7b293ef2d09daff88501eb254f58edde2e1ac02c82d873eadad"
 dependencies = [
  "derive_arbitrary",
 ]
@@ -96,15 +113,15 @@
 version = "0.58.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f8523b410d7187a43085e7e064416ea32ded16bd0a4e6fc025e21616d01258f"
 dependencies = [
  "bitflags",
  "cexpr 0.4.0",
  "clang-sys",
- "clap",
+ "clap 2.34.0",
  "env_logger",
  "lazy_static",
  "lazycell",
  "log",
  "peeking_take_while",
  "proc-macro2",
  "quote",
@@ -140,45 +157,47 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blis-src"
-version = "0.2.1-alpha.0"
-source = "git+https://github.com/cassiersg/blis-src?branch=include#b8b63235d1dc79fd2011e357bac7026314646da2"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "890f81b2cda67a66e45ae13a35363502e84d6a7da86e429d609ede4f3463d086"
 
 [[package]]
-name = "blis-sys"
-version = "0.2.1-alpha.0"
-source = "git+https://github.com/cassiersg/blis-sys#900fbede9a0a05c8e9a4415d1aa12680daaee68e"
+name = "blis-sys2"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d718a14b1fd18063a14830fea23025a6c5b9f521fe8a641279790eaca0f8ab29"
 dependencies = [
  "bindgen 0.58.1",
  "blis-src",
 ]
 
 [[package]]
-name = "bstr"
-version = "0.2.17"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba3569f383e8f1598449f1a423e72e99569137b47740b1da11ef19af3d5c3223"
-dependencies = [
- "lazy_static",
- "memchr",
- "regex-automata",
- "serde",
-]
-
-[[package]]
 name = "bumpalo"
 version = "3.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
 
 [[package]]
+name = "bytemuck"
+version = "1.13.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+
+[[package]]
+name = "byteorder"
+version = "1.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+
+[[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
@@ -208,19 +227,47 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chumsky"
-version = "0.8.0"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d02796e4586c6c41aeb68eae9bfb4558a522c35f1430c14b40136c3706e09e4"
+checksum = "23170228b96236b5a7299057ac284a321457700bc8c41a4476052f0f4ba5349d"
 dependencies = [
- "ahash",
+ "hashbrown",
+ "stacker",
+]
+
+[[package]]
+name = "ciborium"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+dependencies = [
+ "ciborium-io",
+ "ciborium-ll",
+ "serde",
+]
+
+[[package]]
+name = "ciborium-io"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+
+[[package]]
+name = "ciborium-ll"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+dependencies = [
+ "ciborium-io",
+ "half",
 ]
 
 [[package]]
 name = "clang-sys"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa2e27ae6ab525c3d369ded447057bca5438d86dc3a68f6faafb8269ba82ebf3"
@@ -236,95 +283,100 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
 dependencies = [
  "ansi_term",
  "atty",
  "bitflags",
  "strsim",
- "textwrap",
+ "textwrap 0.11.0",
  "unicode-width",
  "vec_map",
 ]
 
 [[package]]
+name = "clap"
+version = "3.2.23"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+dependencies = [
+ "bitflags",
+ "clap_lex",
+ "indexmap",
+ "textwrap 0.16.0",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+dependencies = [
+ "os_str_bytes",
+]
+
+[[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
 ]
 
 [[package]]
+name = "color_quant"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
+
+[[package]]
 name = "console"
 version = "0.15.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3d79fbe8970a77e3e34151cc13d3b3e248aa0faaecb9f6091fa07ebefe5ad60"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
  "unicode-width",
  "windows-sys 0.42.0",
 ]
 
 [[package]]
-name = "const-random"
-version = "0.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "368a7a772ead6ce7e1de82bfb04c485f3db8ec744f72925af5735e29a22cc18e"
-dependencies = [
- "const-random-macro",
- "proc-macro-hack",
-]
-
-[[package]]
-name = "const-random-macro"
-version = "0.1.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d7d6ab3c3a2282db210df5f02c4dab6e0a7057af0fb7ebd4070f30fe05c0ddb"
-dependencies = [
- "getrandom",
- "once_cell",
- "proc-macro-hack",
- "tiny-keccak",
-]
-
-[[package]]
 name = "criterion"
-version = "0.3.6"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b01d6de93b2b6c65e17c634a26653a29d107b3c98c607c765bf38d041531cd8f"
+checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
 dependencies = [
+ "anes",
  "atty",
  "cast",
- "clap",
+ "ciborium",
+ "clap 3.2.23",
  "criterion-plot",
- "csv",
  "itertools",
  "lazy_static",
  "num-traits",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
- "serde_cbor",
  "serde_derive",
  "serde_json",
  "tinytemplate",
  "walkdir",
 ]
 
 [[package]]
 name = "criterion-plot"
-version = "0.4.5"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2673cc8207403546f45f5fd319a974b1e6983ad1a3ee7e6041650013be041876"
+checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
  "itertools",
 ]
 
 [[package]]
 name = "crossbeam-channel"
@@ -366,42 +418,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "crunchy"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
-
-[[package]]
-name = "csv"
-version = "1.1.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22813a6dc45b335f9bade10bf7271dc477e81113e89eb251a0bc2a8a81c536e1"
-dependencies = [
- "bstr",
- "csv-core",
- "itoa 0.4.8",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "csv-core"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
-dependencies = [
- "memchr",
-]
-
-[[package]]
 name = "cxx"
 version = "1.0.89"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bc831ee6a32dd495436e317595e639a587aa9907bef96fe6e6abc290ab6204e9"
 dependencies = [
  "cc",
  "cxxbridge-flags",
@@ -519,14 +543,17 @@
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+dependencies = [
+ "ahash",
+]
 
 [[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
@@ -558,14 +585,27 @@
  "crossbeam-utils",
  "num-traits",
  "rayon",
  "thread_local",
 ]
 
 [[package]]
+name = "image"
+version = "0.24.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69b7ea949b537b0fd0af141fff8c77690f2ce96f4f41f042ccb6c69c6c965945"
+dependencies = [
+ "bytemuck",
+ "byteorder",
+ "color_quant",
+ "num-rational",
+ "num-traits",
+]
+
+[[package]]
 name = "index_vec"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74086667896a940438f2118212f313abba4aff3831fef6f4b17d02add5c8bb60"
 dependencies = [
  "serde",
 ]
@@ -606,20 +646,14 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "0.4.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b71991ff56294aa922b450139ee08b3bfc70982c6b2c7562771375cf73542dd4"
-
-[[package]]
-name = "itoa"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
 
 [[package]]
 name = "js-sys"
 version = "0.3.61"
@@ -728,36 +762,63 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "nalgebra"
-version = "0.26.2"
+version = "0.30.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "476d1d59fe02fe54c86356e91650cd892f392782a1cb9fc524ec84f7aa9e1d06"
+checksum = "4fb2d0de08694bed883320212c18ee3008576bfe8c306f4c3c4a58b4876998be"
 dependencies = [
- "approx",
+ "approx 0.5.1",
  "matrixmultiply",
- "num-complex 0.3.1",
+ "num-complex",
  "num-rational",
  "num-traits",
- "simba",
+ "simba 0.7.3",
  "typenum",
 ]
 
 [[package]]
+name = "nalgebra"
+version = "0.32.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f6515c882ebfddccaa73ead7320ca28036c4bc84c9bcca3cc0cbba8efe89223a"
+dependencies = [
+ "approx 0.5.1",
+ "matrixmultiply",
+ "nalgebra-macros",
+ "num-complex",
+ "num-rational",
+ "num-traits",
+ "simba 0.8.0",
+ "typenum",
+]
+
+[[package]]
+name = "nalgebra-macros"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d232c68884c0c99810a5a4d333ef7e47689cfd0edc85efc9e54e1e6bf5212766"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
- "approx",
+ "approx 0.4.0",
  "matrixmultiply",
- "num-complex 0.4.3",
+ "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
  "rayon",
  "serde",
 ]
 
@@ -814,28 +875,21 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "nshare"
-version = "0.5.1-alpha.0"
-source = "git+https://github.com/cassiersg/nshare?branch=rm_lt#5b449afd22d9a8afb4d6c6af107d15d5a354c5c4"
-dependencies = [
- "nalgebra",
- "ndarray",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.3.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "747d632c0c558b87dbabbe6a82f3b4ae03720d0646ac5b7b4dae89394be5f2c5"
+checksum = "4447657cd40e3107416ec4f2ac3e61a18781b00061789e3b8f4bbcbccb26c4c6"
 dependencies = [
- "num-traits",
+ "image",
+ "nalgebra 0.30.1",
+ "ndarray",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
@@ -851,17 +905,17 @@
 dependencies = [
  "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.3.2"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12ac428b1cb17fce6f731001d307d351ec70a6d202fc2e60f7d4c5e42d8f4f07"
+checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -894,15 +948,15 @@
 name = "numpy"
 version = "0.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
 dependencies = [
  "libc",
  "ndarray",
- "num-complex 0.4.3",
+ "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
@@ -914,14 +968,20 @@
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
+name = "os_str_bytes"
+version = "6.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -1010,29 +1070,32 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9df7f93fd637f083201473dab4fee2db4c429d32e55e3299980ab3957ab916a0"
 dependencies = [
  "num-integer",
 ]
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
-
-[[package]]
 name = "proc-macro2"
 version = "1.0.51"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "psm"
+version = "0.1.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
+dependencies = [
+ "cc",
+]
+
+[[package]]
 name = "pyo3"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
 dependencies = [
  "cfg-if",
  "indoc",
@@ -1161,27 +1224,27 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.2"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "356a0625f1954f730c0201cdab48611198dc6ce21f4acff55089b5a78e6e835b"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
@@ -1220,20 +1283,14 @@
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
-name = "regex-automata"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
-
-[[package]]
 name = "regex-syntax"
 version = "0.6.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
 
 [[package]]
 name = "rustc-hash"
@@ -1243,15 +1300,15 @@
 
 [[package]]
 name = "rustfft"
 version = "6.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e17d4f6cbdb180c9f4b2a26bbf01c4e647f1e1dea22fe8eb9db54198b32f9434"
 dependencies = [
- "num-complex 0.4.3",
+ "num-complex",
  "num-integer",
  "num-traits",
  "primal-check",
  "strength_reduce",
  "transpose",
  "version_check",
 ]
@@ -1259,49 +1316,57 @@
 [[package]]
 name = "ryu"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
 
 [[package]]
+name = "safe_arch"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
+dependencies = [
+ "bytemuck",
+]
+
+[[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "scalib"
 version = "0.1.0"
 dependencies = [
- "approx",
+ "approx 0.5.1",
  "ariadne",
  "blis-src",
- "blis-sys",
+ "blis-sys2",
  "chumsky",
  "criterion",
  "crossbeam-utils",
  "geigen",
  "hytra",
  "index_vec",
  "indexmap",
  "indicatif",
  "itertools",
  "matrixmultiply",
- "nalgebra",
+ "nalgebra 0.32.1",
  "ndarray",
  "ndarray-rand",
  "ndarray-stats",
  "nshare",
  "num-integer",
  "num-traits",
  "petgraph",
- "pyo3",
  "rand_xoshiro",
  "rayon",
  "realfft 2.0.1",
  "serde",
  "thiserror",
 ]
 
@@ -1338,24 +1403,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
-name = "serde_cbor"
-version = "0.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bef2ebfde456fb76bbcf9f59315333decc4fda0b2b44b420243c11e0f5ec1f5"
-dependencies = [
- "half",
- "serde",
-]
-
-[[package]]
 name = "serde_derive"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -1364,44 +1419,71 @@
 
 [[package]]
 name = "serde_json"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
 dependencies = [
- "itoa 1.0.5",
+ "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "shlex"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
 
 [[package]]
 name = "simba"
-version = "0.4.0"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5132a955559188f3d13c9ba831e77c802ddc8782783f050ed0c52f5988b95f4c"
+checksum = "2f3fd720c48c53cace224ae62bef1bbff363a70c68c4802a78b5cc6159618176"
 dependencies = [
- "approx",
- "num-complex 0.3.1",
+ "approx 0.5.1",
+ "num-complex",
  "num-traits",
  "paste",
+ "wide",
+]
+
+[[package]]
+name = "simba"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50582927ed6f77e4ac020c057f37a268fc6aebc29225050365aacbb9deeeddc4"
+dependencies = [
+ "approx 0.5.1",
+ "num-complex",
+ "num-traits",
+ "paste",
+ "wide",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
+name = "stacker"
+version = "0.1.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c886bd4480155fd3ef527d45e9ac8dd7118a898a46530b7b94c3e21866259fce"
+dependencies = [
+ "cc",
+ "cfg-if",
+ "libc",
+ "psm",
+ "winapi",
+]
+
+[[package]]
 name = "strength_reduce"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe895eb47f22e2ddd4dabc02bce419d2e643c8e3b585c78158b349195bc24d82"
 
 [[package]]
 name = "strsim"
@@ -1441,14 +1523,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
 dependencies = [
  "unicode-width",
 ]
 
 [[package]]
+name = "textwrap"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+
+[[package]]
 name = "thiserror"
 version = "1.0.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
 dependencies = [
  "thiserror-impl",
 ]
@@ -1471,23 +1559,14 @@
 checksum = "50f297120ff9d4efe680df143d5631bba9c75fa371992b7fcb33eb3453cb0a07"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
-name = "tiny-keccak"
-version = "2.0.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
-dependencies = [
- "crunchy",
-]
-
-[[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
@@ -1637,14 +1716,24 @@
 dependencies = [
  "either",
  "libc",
  "once_cell",
 ]
 
 [[package]]
+name = "wide"
+version = "0.7.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+dependencies = [
+ "bytemuck",
+ "safe_arch",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
```

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/build.rs` & `scalib-0.5.4/src/scalib_ext/geigen/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Cholesky` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/CholmodSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Core` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Eigenvalues` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Geometry` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Householder` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Jacobi` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/LU` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/MetisSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/OrderingMethods` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/PaStiXSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/PardisoSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/QR` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SPQRSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SVD` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/Sparse` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseCholesky` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseCore` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseLU` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SparseQR` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdDeque` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdList` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/StdVector` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/SuperLUSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/UmfPackSupport` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/DavidsonSymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsComplexShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsRealShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/GenEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/JDSymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Arnoldi.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/BKLDLT.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/DoubleShiftQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Lanczos.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/Orthogonalization.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/RitzPairs.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/SearchSpace.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/TridiagEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergEigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/LinAlg/UpperHessenbergQR.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/DenseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseCholesky.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenComplexShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseGenRealShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseRegularInverse.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymMatProd.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SparseSymShiftSolve.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/SymShiftInvert.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/ArnoldiOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsBucklingOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCayleyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsCholeskyOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsRegInvOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/MatOp/internal/SymGEigsShiftInvertOp.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsBase.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsShiftSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/SymGEigsSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/CompInfo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/GEigsMode.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SelectionRule.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/SimpleRandom.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/TypeTraits.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/Util/Version.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/Util/Version.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/LOBPCGSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/Spectra/contrib/PartialSVDSolver.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/include/geigen.h` & `scalib-0.5.4/src/scalib_ext/geigen/include/geigen.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/src/geigen.cpp` & `scalib-0.5.4/src/scalib_ext/geigen/src/geigen.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/src/geigen.rs` & `scalib-0.5.4/src/scalib_ext/geigen/src/geigen.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/geigen/src/lib.rs` & `scalib-0.5.4/src/scalib_ext/geigen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/build.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/fuzz/Cargo.toml` & `scalib-0.5.4/src/scalib_ext/ranklib/fuzz/Cargo.toml`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/fuzz/fuzz_targets/rank2vsnaive_2.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/aes.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/aes.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/bignumpoly.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/bignumpoly.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/bignumpoly.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_enum.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_enum.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_enum.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_execute.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_execute.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_histo.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_histo.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_histo.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_if.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_if.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_if.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_init.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_init.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_init.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_struct.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_struct.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_util.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/hel_util.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/hel_util.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/histogram.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/src/histogram.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/lib.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/main_example.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/main_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/rank.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/src/rank.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/score_example_data.rs` & `scalib-0.5.4/src/scalib_ext/ranklib/src/score_example_data.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example.h` & `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example.h`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/scores_example_data.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/scores_example_data.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/ranklib/src/top.cpp` & `scalib-0.5.4/src/scalib_ext/ranklib/src/top.cpp`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/benches/belief_propagation.rs` & `scalib-0.5.4/src/scalib_ext/scalib/benches/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/benches/get_snr.rs` & `scalib-0.5.4/src/scalib_ext/scalib/benches/get_snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/benches/mttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib/benches/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/benches/snr_update.rs` & `scalib-0.5.4/src/scalib_ext/scalib/benches/snr_update.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/benches/ttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib/benches/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/belief_propagation.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/lda.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/lib.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/matrixmul.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/matrixmul.rs`

 * *Files 16% similar despite different names*

```diff
@@ -17,43 +17,43 @@
         unsafe {
             let rsa = a.stride_of(ndarray::Axis(0));
             let csa = a.stride_of(ndarray::Axis(1));
             let rsb = b.stride_of(ndarray::Axis(0));
             let csb = b.stride_of(ndarray::Axis(1));
             let rsc = c.stride_of(ndarray::Axis(0));
             let csc = c.stride_of(ndarray::Axis(1));
-            let mut rntm = blis_sys::rntm_t {
+            let mut rntm = blis_sys2::rntm_t {
                 auto_factor: true,
                 num_threads: num_threads as i64,
                 thrloop: [-1; 6usize],
                 pack_a: false,
                 pack_b: false,
                 l3_sup: true,
                 sba_pool: std::ptr::null_mut(),
-                membrk: std::ptr::null_mut(),
+                pba: std::ptr::null_mut(),
             };
             rntm.thrloop[0] = 1;
-            blis_sys::bli_dgemm_ex(
-                blis_sys::trans_t_BLIS_NO_TRANSPOSE,
-                blis_sys::trans_t_BLIS_NO_TRANSPOSE,
-                m as blis_sys::dim_t,
-                n as blis_sys::dim_t,
-                k as blis_sys::dim_t,
+            blis_sys2::bli_dgemm_ex(
+                blis_sys2::trans_t_BLIS_NO_TRANSPOSE,
+                blis_sys2::trans_t_BLIS_NO_TRANSPOSE,
+                m as blis_sys2::dim_t,
+                n as blis_sys2::dim_t,
+                k as blis_sys2::dim_t,
                 &alpha as *const _ as *mut _,
                 a.as_ptr() as *mut _,
-                rsa as blis_sys::dim_t,
-                csa as blis_sys::dim_t,
+                rsa as blis_sys2::dim_t,
+                csa as blis_sys2::dim_t,
                 b.as_ptr() as *mut _,
-                rsb as blis_sys::dim_t,
-                csb as blis_sys::dim_t,
+                rsb as blis_sys2::dim_t,
+                csb as blis_sys2::dim_t,
                 &beta as *const _ as *mut _,
                 c.as_mut_ptr(),
-                rsc as blis_sys::dim_t,
-                csc as blis_sys::dim_t,
-                blis_sys::bli_gks_query_cntx(),
+                rsc as blis_sys2::dim_t,
+                csc as blis_sys2::dim_t,
+                blis_sys2::bli_gks_query_cntx(),
                 &mut rntm,
             );
         }
     } else {
         ndarray::linalg::general_mat_mul(alpha, &a, &b, beta, &mut c);
     }
 }
```

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/mttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/mttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/belief_propagation.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/belief_propagation.rs`

 * *Files 0% similar despite different names*

```diff
@@ -196,18 +196,16 @@
             .edges
             .values()
             .map(|e| &self.belief_to_var[*e]);
         self.var_state[var] = self.evidence[var].take_or_clone(clear_evidence);
         // We multiply_reg to avoid having very low values in the product.
         // Since inputs should not be too big, we should not have any overflow.
         // Underflow my happen, since probas are lower-bounded by MIN_PROBA**2.
+        // This also normalizes the result.
         self.var_state[var].multiply_reg(distr_iter);
-        // Now we'll make to sum equal one to avoid underflows or overflows in the long run, and keep the exposed probas nice.
-        // Just multiply, don't add anything, underflows are taken care of above.
-        self.var_state[var].normalize();
     }
     pub fn propagate_from_var(&mut self, edge: EdgeId) {
         // Dividing here is ok if we ensure that there is no zero element and no
         // underflow (or denormalization).
         // This is guaranteed as long as min_proba > var_degree * MIN_POSITIVE
         let var = self.graph.edges[edge].var;
         self.belief_from_var[edge].reset();
@@ -282,17 +280,14 @@
         clear_intermediates: bool,
         clear_evidence: bool,
     ) -> Result<(), BPError> {
         if self.is_cyclic() {
             return Err(BPError::NotAcyclic);
         }
         for (node, parent) in self.graph.propagation_order(var) {
-            dbg!(&self);
-            dbg!(node);
-            dbg!(parent);
             match node {
                 Node::Var(var_id) => {
                     self.propagate_to_var(var_id, clear_evidence);
                     if let Some(dest_factor) = parent {
                         let edge_id = self.graph.var(var_id).edges[&dest_factor.factor().unwrap()];
                         self.propagate_from_var(edge_id);
                     }
```

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/bp_compute.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/bp_compute.rs`

 * *Files 3% similar despite different names*

```diff
@@ -132,67 +132,85 @@
             self.reset()
         } else {
             self.clone()
         }
     }
 
     pub fn multiply<'a>(&mut self, factors: impl Iterator<Item = &'a Distribution>) {
-        self.multiply_inner(factors, 0.0, 0.0);
+        self.multiply_inner(factors, false);
     }
 
     pub fn multiply_reg<'a>(&mut self, factors: impl Iterator<Item = &'a Distribution>) {
-        self.multiply_inner(factors, MIN_PROBA, MIN_PROBA * MIN_PROBA);
+        self.multiply_inner(factors, true);
     }
 
-    fn multiply_inner<'a>(
-        &mut self,
-        factors: impl Iterator<Item = &'a Distribution>,
-        offset: Proba,
-        offset_prod: Proba,
-    ) {
+    fn multiply_inner<'a>(&mut self, factors: impl Iterator<Item = &'a Distribution>, reg: bool) {
         for factor in factors {
             assert_eq!(self.shape.1, factor.shape.1);
             if self.multi & factor.multi {
                 assert_eq!(self.shape.0, factor.shape.0);
             }
             if let DistrRepr::Full(d) = &factor.value {
                 assert_eq!(d.dim(), factor.shape);
                 match (self.multi, factor.multi, &mut self.value) {
                     (_, false, DistrRepr::Uniform) => {
                         self.value = DistrRepr::Full(ndarray::Array::from_shape_fn(
                             self.shape,
-                            |(_i, j)| d[(0, j)] + offset,
+                            |(_i, j)| d[(0, j)],
                         ));
                     }
                     (false, true, DistrRepr::Uniform) => {
                         let mut v = ndarray::Array2::ones(self.shape);
-                        for d in d.axis_iter(ndarray::Axis(0)) {
-                            azip!(v.slice_mut(s![0, ..]), d).for_each(|v, d| {
-                                *v = *v * (*d + offset) + offset_prod;
-                            });
+                        // Here we can't simply rely on the normalization at
+                        // the end of the factors loop, since we could multiply
+                        // many distributions at once.
+                        // We therefore compute the maximum at every iteration,
+                        // and correct to keep the maximum at 1. at the next
+                        // iteration.
+                        if reg {
+                            let mut max_proba = 1.0f64;
+                            for d in d.axis_iter(ndarray::Axis(0)) {
+                                let norm_factor = 1.0 / max_proba;
+                                max_proba = 0.0;
+                                azip!(v.slice_mut(s![0, ..]), d).for_each(|v, d| {
+                                    *v = *v * norm_factor * *d;
+                                    max_proba = max_proba.max(*v);
+                                });
+                            }
+                        } else {
+                            for d in d.axis_iter(ndarray::Axis(0)) {
+                                azip!(v.slice_mut(s![0, ..]), d).for_each(|v, d| {
+                                    *v = *v * *d;
+                                });
+                            }
                         }
                         self.value = DistrRepr::Full(v);
                     }
                     (true, true, DistrRepr::Uniform) => {
-                        self.value = DistrRepr::Full(d.map(|d| *d + offset));
+                        self.value = DistrRepr::Full(d.map(|d| *d));
                     }
                     (true, _, DistrRepr::Full(ref mut v)) => {
                         azip!(v, d).for_each(|v, d| {
-                            *v = *v * (*d + offset) + offset_prod;
+                            *v = *v * *d;
                         });
                     }
                     (false, _, DistrRepr::Full(ref mut v)) => {
                         for d in d.axis_iter(ndarray::Axis(0)) {
                             azip!(v.slice_mut(s![0, ..]), d).for_each(|v, d| {
-                                *v = *v * (*d + offset) + offset_prod;
+                                *v = *v * *d;
                             });
                         }
                     }
                 }
             }
+            // Now we'll make to sum equal one to avoid underflows or overflows in the long run, and keep the exposed probas nice.
+            // Just multiply, don't add anything, underflows are taken care of above.
+            if reg {
+                self.normalize();
+            }
         }
     }
     pub fn divide_reg(state: &Distribution, div: &Distribution) -> Self {
         let mut res = Self {
             multi: state.multi | div.multi,
             shape: (std::cmp::max(state.shape.0, div.shape.0), state.shape.1),
             value: DistrRepr::Uniform,
```

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/factor_graph.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/factor_graph.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/fg_build.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_build.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/fg_parser.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/fg_parser.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/sasca/mod.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/sasca/mod.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/snr.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/ttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/src/utils.rs` & `scalib-0.5.4/src/scalib_ext/scalib/src/utils.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/tests/lda.rs` & `scalib-0.5.4/src/scalib_ext/scalib/tests/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/tests/multivarcs.rs` & `scalib-0.5.4/src/scalib_ext/scalib/tests/multivarcs.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib/tests/ttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib/tests/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/Cargo.toml` & `scalib-0.5.4/src/scalib_ext/scalib-py/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [package]
 name = "scalib-py"
 version = "0.1.0"
 authors = [
     "Olivier Bronchain <olivier.bronchain@uclouvain.be>",
     "Gaëtan Cassiers <gaetan.cassiers@uclouvain.be>"
 ]
-edition = "2018"
+edition = "2021"
 
 [lib]
 name = "scalib_py"
 crate-type = ["cdylib"]
 
 [features]
 ntl = ["ranklib/ntl"]
 hellib = ["ranklib/hellib"]
 blis = ["scalib/blis"]
 
 [dependencies]
-rayon = "1.5.0"
-ndarray = { version = "0.15.1", features = ["rayon"] }
-numpy = "0.18.0"
-indicatif = "0.17.3"
-num_cpus = "1.15.0"
-bincode = "1.3.3" # Serialization for pickle support
+rayon = "1.7"
+ndarray = { version = "0.15", features = ["rayon"] }
+numpy = "0.18"
+indicatif = "0.17"
+num_cpus = "1.15"
+bincode = "1.3" # Serialization for pickle support
 
 [dependencies.pyo3]
-version = "0.18.0"
-features = ["extension-module"]
+version = "0.18"
+features = ["extension-module", "abi3-py38"]
 
 [dependencies.ranklib]
 path = "../ranklib"
 
 [dependencies.scalib]
 path = "../scalib"
```

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/belief_propagation.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/belief_propagation.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/factor_graph.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/factor_graph.rs`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,14 @@
 pub(crate) struct FactorGraph {
     inner: Option<Arc<sasca::FactorGraph>>,
 }
 impl FactorGraph {
     fn get_inner(&self) -> &Arc<sasca::FactorGraph> {
         self.inner.as_ref().unwrap()
     }
-    fn get_var(&self, var: &str) -> PyResult<sasca::VarId> {
-        self.get_inner()
-            .get_varid(var)
-            .map_err(|e| PyValueError::new_err(e.to_string()))
-    }
     fn get_factor(&self, factor: &str) -> PyResult<sasca::FactorId> {
         self.get_inner()
             .get_factorid(factor)
             .map_err(|e| PyValueError::new_err(e.to_string()))
     }
 }
 
@@ -239,27 +234,43 @@
         let edge_id = self.get_edge_named(var, factor)?;
         distr2py(py, self.get_inner().get_belief_to_var(edge_id))
     }
     pub fn get_belief_from_var(&self, py: Python, var: &str, factor: &str) -> PyResult<PyObject> {
         let edge_id = self.get_edge_named(var, factor)?;
         distr2py(py, self.get_inner().get_belief_from_var(edge_id))
     }
-    pub fn propagate_var(&mut self, var: &str) -> PyResult<()> {
-        let var_id = self.get_var(var)?;
-        self.get_inner_mut().propagate_var(var_id);
-        Ok(())
+    pub fn propagate_var(
+        &mut self,
+        py: Python,
+        var: &str,
+        config: crate::ConfigWrapper,
+    ) -> PyResult<()> {
+        config.on_worker(py, |_| {
+            let var_id = self.get_var(var)?;
+            self.get_inner_mut().propagate_var(var_id);
+            Ok(())
+        })
     }
-    pub fn propagate_all_vars(&mut self) -> PyResult<()> {
-        self.get_inner_mut().propagate_all_vars();
-        Ok(())
+    pub fn propagate_all_vars(&mut self, py: Python, config: crate::ConfigWrapper) -> PyResult<()> {
+        config.on_worker(py, |_| {
+            self.get_inner_mut().propagate_all_vars();
+            Ok(())
+        })
     }
-    pub fn propagate_factor_all(&mut self, factor: &str) -> PyResult<()> {
-        let factor_id = self.get_factor(factor)?;
-        self.get_inner_mut().propagate_factor_all(factor_id);
-        Ok(())
+    pub fn propagate_factor_all(
+        &mut self,
+        py: Python,
+        factor: &str,
+        config: crate::ConfigWrapper,
+    ) -> PyResult<()> {
+        config.on_worker(py, |_| {
+            let factor_id = self.get_factor(factor)?;
+            self.get_inner_mut().propagate_factor_all(factor_id);
+            Ok(())
+        })
     }
     pub fn set_belief_from_var(
         &mut self,
         py: Python,
         var: &str,
         factor: &str,
         distr: PyObject,
@@ -283,45 +294,55 @@
         let distr = obj2distr(py, distr, bp.get_graph().edge_multi(edge_id))?;
         bp.set_belief_to_var(edge_id, distr)
             .map_err(|e| PyTypeError::new_err(e.to_string()))?;
         Ok(())
     }
     pub fn propagate_factor(
         &mut self,
+        py: Python,
         factor: &str,
         dest: Vec<&str>,
         clear_incoming: bool,
+        config: crate::ConfigWrapper,
     ) -> PyResult<()> {
-        let factor_id = self.get_factor(factor)?;
-        let dest = dest
-            .iter()
-            .map(|v| self.get_var(v))
-            .collect::<Result<Vec<_>, _>>()?;
-        self.get_inner_mut()
-            .propagate_factor(factor_id, dest.as_slice(), clear_incoming);
-        Ok(())
+        config.on_worker(py, |_| {
+            let factor_id = self.get_factor(factor)?;
+            let dest = dest
+                .iter()
+                .map(|v| self.get_var(v))
+                .collect::<Result<Vec<_>, _>>()?;
+            self.get_inner_mut()
+                .propagate_factor(factor_id, dest.as_slice(), clear_incoming);
+            Ok(())
+        })
     }
-    pub fn propagate_loopy_step(&mut self, n_steps: u32) {
-        self.get_inner_mut().propagate_loopy_step(n_steps);
+    pub fn propagate_loopy_step(&mut self, py: Python, n_steps: u32, config: crate::ConfigWrapper) {
+        config.on_worker(py, |_| {
+            self.get_inner_mut().propagate_loopy_step(n_steps);
+        });
     }
     pub fn graph(&self) -> FactorGraph {
         FactorGraph {
             inner: Some(self.get_inner().get_graph().clone()),
         }
     }
     pub fn propagate_acyclic(
         &mut self,
+        py: Python,
         dest: &str,
         clear_intermediates: bool,
         clear_evidence: bool,
+        config: crate::ConfigWrapper,
     ) -> PyResult<()> {
-        let var = self.get_var(dest)?;
-        self.get_inner_mut()
-            .propagate_acyclic(var, clear_intermediates, clear_evidence)
-            .map_err(|e| PyValueError::new_err(e.to_string()))
+        config.on_worker(py, |_| {
+            let var = self.get_var(dest)?;
+            self.get_inner_mut()
+                .propagate_acyclic(var, clear_intermediates, clear_evidence)
+                .map_err(|e| PyValueError::new_err(e.to_string()))
+        })
     }
 }
 
 fn obj2distr(py: Python, distr: PyObject, multi: bool) -> PyResult<sasca::Distribution> {
     if multi {
         let distr: &PyArray2<f64> = distr.extract(py)?;
         sasca::Distribution::from_array_multi(
```

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/lda.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/lda.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/lib.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/lib.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/ranking.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/ranking.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/snr.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/snr.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/thread_pool.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/thread_pool.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/src/scalib_ext/scalib-py/src/ttest.rs` & `scalib-0.5.4/src/scalib_ext/scalib-py/src/ttest.rs`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/tests/mttest_test.py` & `scalib-0.5.4/tests/mttest_test.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/tests/test_factorgraph.py` & `scalib-0.5.4/tests/test_factorgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -900,7 +900,39 @@
     fg = FactorGraph(factor_graph)
     bp = BPState(fg, 1, public_values={"IV": 0xC})
     for k, v in priors.items():
         bp.set_evidence(k, distribution=np.array([v]))
     bp.bp_loopy(5, initialize_states=False)
     assert (bp.get_distribution("K0") >= 0.0).all()
     assert (bp.get_distribution("K1") >= 0.0).all()
+
+
+def test_manytraces():
+    """No numerical underflow with many traces."""
+    nc = 8
+    n = 500
+    distri_x = np.ones((n, nc))
+    distri_x[:, 0] = 2.0
+    distri_x[:, 1] = 1.5
+    distri_x = (distri_x.T / np.sum(distri_x, axis=1)).T
+
+    graph = f"""
+            NC {nc}
+            VAR MULTI x
+            VAR SINGLE y
+            PUB SINGLE c
+            PROPERTY y = x ^ c
+            """
+    graph = FactorGraph(graph)
+    bp_state = BPState(graph, n, {"c": 0})
+
+    bp_state.set_evidence("x", distri_x)
+
+    bp_state.bp_acyclic("y")
+    distri_y = bp_state.get_distribution("y")
+
+    distri_y_ref = np.log2(distri_x).sum(axis=0, keepdims=True)
+    distri_y_ref = distri_y_ref - np.max(distri_y_ref[0, :])
+    distri_y_ref = 2**distri_y_ref
+    distri_y_ref = distri_y_ref / distri_y_ref.sum(axis=1, keepdims=True)
+
+    assert np.allclose(distri_y_ref, distri_y, rtol=1e-5, atol=1e-19)
```

### Comparing `scalib-0.5.3/tests/test_lda.py` & `scalib-0.5.4/tests/test_lda.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LDA_sklearn
 from scalib import ScalibError
-from scalib.modeling import LDAClassifier
+from scalib.modeling import LDAClassifier, MultiLDA
 import numpy as np
 import scipy.stats
 import pickle
 
 
 def is_parallel(x, y):
     z = np.abs(x.dot(y))
@@ -171,7 +171,18 @@
     nc = 4
     lda = LDAClassifier(nc, 3, ns)
     traces_bad = np.random.randint(0, 1, (n, ns), dtype=np.int16)
     y = np.random.randint(0, nc, n, dtype=np.uint16)
     lda.fit_u(traces_bad, y, 0)
     with pytest.raises(ScalibError):
         lda.solve()
+
+
+def test_multilda():
+    x = np.random.randint(0, 256, (5000, 50), dtype=np.int16)
+    y = np.random.randint(0, 256, (5000, 5), dtype=np.uint16)
+    pois = [list(range(7 * i, 7 * i + 10)) for i in range(5)]
+    lda = MultiLDA(5 * [256], 5 * [3], pois)
+    lda.fit_u(x, y)
+    lda.solve()
+    x = np.random.randint(0, 256, (20, 50), dtype=np.int16)
+    predicted_proba = lda.predict_proba(x)
```

### Comparing `scalib-0.5.3/tests/test_sascagraph.py` & `scalib-0.5.4/tests/test_sascagraph.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/tests/test_snr.py` & `scalib-0.5.4/tests/test_snr.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/tests/test_ttest.py` & `scalib-0.5.4/tests/test_ttest.py`

 * *Files identical despite different names*

### Comparing `scalib-0.5.3/tox.ini` & `scalib-0.5.4/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 [base]
 setenv =
     RUST_BACKTRACE=1
     CARGO_TARGET_DIR={toxinidir}/.cargo_build
 deps =
     -r{toxinidir}/tests/requirements.txt
 commands =
-    cargo test --workspace --manifest-path {toxinidir}/src/scalib_ext/Cargo.toml
     pip freeze
     pytest {tty:--color=yes} {posargs}
 
 [testenv]
 description =
     test: run tests (defaut local python)
     coverage: run tests with coverage
 setenv = {[base]setenv}
 deps = {[base]deps}
 commands = {[base]commands}
 package = wheel
 wheel_build_env = .pkg
-allowlist_externals = cargo
 
 [testenv:dev]
 description = Editable install with debug build.
 setenv = {[base]setenv}
 deps = {[base]deps}
 commands = {[base]commands}
 package = editable
@@ -58,13 +56,14 @@
 
 [testenv:fmt]
 description = Check code style. Pass '--check' to instead check formatting.
 skip_install = True
 changedir = .
 deps =
     black ~= 23.0
+allowlist_externals = cargo
 commands =
     black --version
     black {posargs} src/scalib tests examples
     cargo fmt --version
     cargo fmt --manifest-path src/scalib_ext/Cargo.toml --all -- {posargs}
```

