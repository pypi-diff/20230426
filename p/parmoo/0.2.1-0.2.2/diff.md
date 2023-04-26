# Comparing `tmp/parmoo-0.2.1.tar.gz` & `tmp/parmoo-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parmoo-0.2.1.tar", last modified: Mon Apr 10 20:02:01 2023, max compression
+gzip compressed data, was "parmoo-0.2.2.tar", last modified: Tue Apr 25 22:38:12 2023, max compression
```

## Comparing `parmoo-0.2.1.tar` & `parmoo-0.2.2.tar`

### file list

```diff
@@ -1,180 +1,180 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.935469 parmoo-0.2.1/
--rw-r--r--   0 tyler      (501) staff       (20)     4084 2023-04-10 20:01:13.000000 parmoo-0.2.1/CHANGELOG.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.2.1/CONTRIBUTING.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-21 22:52:41.000000 parmoo-0.2.1/LICENSE
--rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.2.1/MANIFEST.in
--rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-10 20:02:01.934879 parmoo-0.2.1/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)    11817 2023-04-10 20:01:13.000000 parmoo-0.2.1/README.rst
--rw-r--r--   0 tyler      (501) staff       (20)      113 2023-04-10 20:01:13.000000 parmoo-0.2.1/REQUIREMENTS
--rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-21 22:52:41.000000 parmoo-0.2.1/SUPPORT.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.778071 parmoo-0.2.1/docs/
--rw-r--r--   0 tyler      (501) staff       (20)      671 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/REQUIREMENTS.txt
--rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/about.rst
--rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/api.rst
--rw-r--r--   0 tyler      (501) staff       (20)     3586 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/conf.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.779875 parmoo-0.2.1/docs/dev-guide/
--rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/contributing.rst
--rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/modules.rst
--rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/dev-guide/release-notes.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1961 2023-02-21 22:52:43.000000 parmoo-0.2.1/docs/dev-guide/release-proc.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/extras.rst
--rw-r--r--   0 tyler      (501) staff       (20)    30292 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/how-to-write.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.793972 parmoo-0.2.1/docs/img/
--rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/algorithm-flowchart.png
--rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/des-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/des-sim-obj-space.png
--rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/icon-ParMOO_space.png
--rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/logo-ParMOO.png
--rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/logo-ParMOO.svg
--rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/img/logo-ParMOO_white.png
--rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop-uml.png
--rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop-uml.svg
--rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/img/moop.uml
--rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/img/parmoo_movie.gif
--rw-r--r--   0 tyler      (501) staff       (20)     1580 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/index.rst
--rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/install.rst
--rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/latex_index.rst
--rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.2.1/docs/make.bat
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.831032 parmoo-0.2.1/docs/modules/
--rw-r--r--   0 tyler      (501) staff       (20)     1090 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/acquisitions.rst
--rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/class_api.rst
--rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/constraints.rst
--rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/dev_tools.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/dtlz.rst
--rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/libe.rst
--rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/libraries.rst
--rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/moop.rst
--rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/objectives.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/optimizers.rst
--rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/searches.rst
--rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/simulations.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/structs.rst
--rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/surrogates.rst
--rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.2.1/docs/modules/util.rst
--rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/modules/viz.rst
--rw-r--r--   0 tyler      (501) staff       (20)    11145 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/quickstart.rst
--rw-r--r--   0 tyler      (501) staff       (20)     1390 2023-04-10 20:01:13.000000 parmoo-0.2.1/docs/refs.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.832016 parmoo-0.2.1/docs/tutorials/
--rw-r--r--   0 tyler      (501) staff       (20)     4527 2023-02-21 22:52:41.000000 parmoo-0.2.1/docs/tutorials/basic-tutorials.rst
--rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.2.1/docs/tutorials/libe-tutorial.rst
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.840847 parmoo-0.2.1/examples/
--rw-r--r--   0 tyler      (501) staff       (20)     1010 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/Makefile
--rw-r--r--   0 tyler      (501) staff       (20)    16534 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/Pareto Front.jpeg
--rw-r--r--   0 tyler      (501) staff       (20)     1972 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/advanced_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     3765 2022-05-10 17:20:56.000000 parmoo-0.2.1/examples/advanced_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)     1635 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/checkpointing.out
--rw-r--r--   0 tyler      (501) staff       (20)     2299 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/checkpointing.py
--rw-r--r--   0 tyler      (501) staff       (20)      955 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/libe_basic_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2243 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/libe_basic_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/named_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/named_var_ex.py
--rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/precomputed_data.out
--rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.2.1/examples/precomputed_data.py
--rw-r--r--   0 tyler      (501) staff       (20)     1409 2023-04-10 20:01:13.000000 parmoo-0.2.1/examples/quickstart.out
--rw-r--r--   0 tyler      (501) staff       (20)     1575 2023-02-21 22:52:41.000000 parmoo-0.2.1/examples/quickstart.py
--rw-r--r--   0 tyler      (501) staff       (20)      582 2022-07-11 19:27:11.000000 parmoo-0.2.1/examples/unnamed_var_ex.out
--rw-r--r--   0 tyler      (501) staff       (20)     2336 2022-05-10 21:22:59.000000 parmoo-0.2.1/examples/unnamed_var_ex.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.845865 parmoo-0.2.1/parmoo/
--rw-r--r--   0 tyler      (501) staff       (20)      385 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.851040 parmoo-0.2.1/parmoo/acquisitions/
--rw-r--r--   0 tyler      (501) staff       (20)      104 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/acquisitions/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     9122 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/acquisitions/epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15030 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/acquisitions/weighted_sum.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.854205 parmoo-0.2.1/parmoo/constraints/
--rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/constraints/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/constraints/const_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/constraints/const_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.860969 parmoo-0.2.1/parmoo/extras/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/extras/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    36753 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/extras/libe.py
--rw-r--r--   0 tyler      (501) staff       (20)   127469 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/moop.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.877774 parmoo-0.2.1/parmoo/objectives/
--rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/objectives/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/objectives/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/objectives/obj_func.py
--rw-r--r--   0 tyler      (501) staff       (20)    16981 2022-07-26 17:47:19.000000 parmoo-0.2.1/parmoo/objectives/obj_lib.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.890171 parmoo-0.2.1/parmoo/optimizers/
--rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/optimizers/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    17274 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)    20784 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     8330 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/optimizers/random_search.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.897334 parmoo-0.2.1/parmoo/searches/
--rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/searches/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/searches/latin_hypercube.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.904690 parmoo-0.2.1/parmoo/simulations/
--rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/simulations/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    31184 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/simulations/dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/simulations/sim_func.py
--rw-r--r--   0 tyler      (501) staff       (20)     3905 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/simulations/simple.py
--rw-r--r--   0 tyler      (501) staff       (20)    16723 2023-04-10 18:11:54.000000 parmoo-0.2.1/parmoo/structs.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.906931 parmoo-0.2.1/parmoo/surrogates/
--rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/surrogates/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    33863 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/surrogates/gaussian_proc.py
--rw-r--r--   0 tyler      (501) staff       (20)    17196 2023-03-17 16:31:56.000000 parmoo-0.2.1/parmoo/surrogates/linear_model.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.909032 parmoo-0.2.1/parmoo/tests/
--rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/.coveragerc
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.910518 parmoo-0.2.1/parmoo/tests/.pytest_cache/
--rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/README.md
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.767136 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.912068 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/
--rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.913990 parmoo-0.2.1/parmoo/tests/libe_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/libe_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/libe_tests/libe_funcs.py
--rw-r--r--   0 tyler      (501) staff       (20)     3003 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/libe_tests/test_libe_gen.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.921092 parmoo-0.2.1/parmoo/tests/regression_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/regression_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     2411 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_obj.py
--rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz5_sim.py
--rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_infeasible_prob.py
--rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_mixed_variables.py
--rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.2.1/parmoo/tests/regression_tests/test_user_func.py
--rwxr-xr-x   0 tyler      (501) staff       (20)     2691 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/run-tests.sh
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.930973 parmoo-0.2.1/parmoo/tests/unit_tests/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.1/parmoo/tests/unit_tests/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     8679 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_const_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     4039 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_epsilon_constraint.py
--rw-r--r--   0 tyler      (501) staff       (20)    15426 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_gaussian_proc.py
--rw-r--r--   0 tyler      (501) staff       (20)     7513 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_gps_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     1649 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_latin_hypercube.py
--rw-r--r--   0 tyler      (501) staff       (20)     8800 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_lbfgsb.py
--rw-r--r--   0 tyler      (501) staff       (20)     6545 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_libe.py
--rw-r--r--   0 tyler      (501) staff       (20)    79942 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop.py
--rw-r--r--   0 tyler      (501) staff       (20)    27995 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_embeddings.py
--rw-r--r--   0 tyler      (501) staff       (20)    16562 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_grads.py
--rw-r--r--   0 tyler      (501) staff       (20)     7035 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     8378 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_lib.py
--rw-r--r--   0 tyler      (501) staff       (20)     3572 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_random_search.py
--rw-r--r--   0 tyler      (501) staff       (20)     4745 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_dtlz.py
--rw-r--r--   0 tyler      (501) staff       (20)     1708 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_simple.py
--rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_structs.py
--rw-r--r--   0 tyler      (501) staff       (20)    10127 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_util.py
--rw-r--r--   0 tyler      (501) staff       (20)    24842 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_viz_without_dash.py
--rw-r--r--   0 tyler      (501) staff       (20)     7451 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/tests/unit_tests/test_weighted_sum.py
--rw-r--r--   0 tyler      (501) staff       (20)    18801 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/util.py
--rw-r--r--   0 tyler      (501) staff       (20)       22 2023-04-10 20:01:13.000000 parmoo-0.2.1/parmoo/version.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.934050 parmoo-0.2.1/parmoo/viz/
--rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/dashboard.py
--rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/graph.py
--rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/plot.py
--rw-r--r--   0 tyler      (501) staff       (20)    14045 2023-02-21 22:52:41.000000 parmoo-0.2.1/parmoo/viz/utilities.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-10 20:02:01.848597 parmoo-0.2.1/parmoo.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     4530 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)      120 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)        7 2023-04-10 20:02:01.000000 parmoo-0.2.1/parmoo.egg-info/top_level.txt
--rw-r--r--   0 tyler      (501) staff       (20)       38 2023-04-10 20:02:01.935667 parmoo-0.2.1/setup.cfg
--rw-r--r--   0 tyler      (501) staff       (20)     3421 2023-04-10 20:01:13.000000 parmoo-0.2.1/setup.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.745400 parmoo-0.2.2/
+-rw-r--r--   0 tyler      (501) staff       (20)     4222 2023-04-25 22:34:22.000000 parmoo-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3111 2022-05-10 21:22:59.000000 parmoo-0.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1525 2023-02-21 22:52:41.000000 parmoo-0.2.2/LICENSE
+-rw-r--r--   0 tyler      (501) staff       (20)      600 2022-05-10 21:22:59.000000 parmoo-0.2.2/MANIFEST.in
+-rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-25 22:38:12.745129 parmoo-0.2.2/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)    11817 2023-04-25 22:34:22.000000 parmoo-0.2.2/README.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      113 2023-04-10 20:01:13.000000 parmoo-0.2.2/REQUIREMENTS
+-rw-r--r--   0 tyler      (501) staff       (20)       91 2023-02-21 22:52:41.000000 parmoo-0.2.2/SUPPORT.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.627248 parmoo-0.2.2/docs/
+-rw-r--r--   0 tyler      (501) staff       (20)      671 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)       45 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/REQUIREMENTS.txt
+-rw-r--r--   0 tyler      (501) staff       (20)    12729 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/about.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      257 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     3586 2023-04-24 18:05:49.000000 parmoo-0.2.2/docs/conf.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.629319 parmoo-0.2.2/docs/dev-guide/
+-rw-r--r--   0 tyler      (501) staff       (20)       36 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/contributing.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      162 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/modules.rst
+-rw-r--r--   0 tyler      (501) staff       (20)       33 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/dev-guide/release-notes.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1961 2023-02-21 22:52:43.000000 parmoo-0.2.2/docs/dev-guide/release-proc.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2831 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/extras.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    30292 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/how-to-write.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.642820 parmoo-0.2.2/docs/img/
+-rw-r--r--   0 tyler      (501) staff       (20)   395713 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/algorithm-flowchart.png
+-rw-r--r--   0 tyler      (501) staff       (20)   142159 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/des-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)   133860 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/des-sim-obj-space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    24057 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     2551 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    36996 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/icon-ParMOO_space.png
+-rw-r--r--   0 tyler      (501) staff       (20)    51610 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/logo-ParMOO.png
+-rw-r--r--   0 tyler      (501) staff       (20)     4441 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/logo-ParMOO.svg
+-rw-r--r--   0 tyler      (501) staff       (20)    71259 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/img/logo-ParMOO_white.png
+-rw-r--r--   0 tyler      (501) staff       (20)   175826 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop-uml.png
+-rw-r--r--   0 tyler      (501) staff       (20)   261708 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop-uml.svg
+-rw-r--r--   0 tyler      (501) staff       (20)     1705 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/img/moop.uml
+-rw-r--r--   0 tyler      (501) staff       (20)  7658326 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/img/parmoo_movie.gif
+-rw-r--r--   0 tyler      (501) staff       (20)     1580 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     4789 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/install.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      862 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/latex_index.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      799 2022-05-10 17:20:56.000000 parmoo-0.2.2/docs/make.bat
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.670338 parmoo-0.2.2/docs/modules/
+-rw-r--r--   0 tyler      (501) staff       (20)     1090 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/acquisitions.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      366 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/class_api.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      795 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/constraints.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      211 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/dev_tools.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2698 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/dtlz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      493 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/libe.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      735 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/libraries.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      583 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/moop.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      753 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/objectives.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1639 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/optimizers.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      853 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/searches.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      253 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/simulations.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1098 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/structs.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      713 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/surrogates.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      338 2022-09-09 18:45:50.000000 parmoo-0.2.2/docs/modules/util.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     2890 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/modules/viz.rst
+-rw-r--r--   0 tyler      (501) staff       (20)    11145 2023-04-24 18:05:49.000000 parmoo-0.2.2/docs/quickstart.rst
+-rw-r--r--   0 tyler      (501) staff       (20)     1390 2023-04-25 22:34:22.000000 parmoo-0.2.2/docs/refs.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.672046 parmoo-0.2.2/docs/tutorials/
+-rw-r--r--   0 tyler      (501) staff       (20)     4527 2023-02-21 22:52:41.000000 parmoo-0.2.2/docs/tutorials/basic-tutorials.rst
+-rw-r--r--   0 tyler      (501) staff       (20)      678 2022-05-10 21:22:59.000000 parmoo-0.2.2/docs/tutorials/libe-tutorial.rst
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.684337 parmoo-0.2.2/examples/
+-rw-r--r--   0 tyler      (501) staff       (20)     1010 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/Makefile
+-rw-r--r--   0 tyler      (501) staff       (20)    16534 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/Pareto Front.jpeg
+-rw-r--r--   0 tyler      (501) staff       (20)     1972 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/advanced_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     3765 2022-05-10 17:20:56.000000 parmoo-0.2.2/examples/advanced_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1635 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/checkpointing.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2299 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/checkpointing.py
+-rw-r--r--   0 tyler      (501) staff       (20)      955 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/libe_basic_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2243 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/libe_basic_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)      153 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/named_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1620 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/named_var_ex.py
+-rw-r--r--   0 tyler      (501) staff       (20)      108 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/precomputed_data.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1409 2022-06-15 17:14:45.000000 parmoo-0.2.2/examples/precomputed_data.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1409 2023-04-24 18:05:49.000000 parmoo-0.2.2/examples/quickstart.out
+-rw-r--r--   0 tyler      (501) staff       (20)     1575 2023-02-21 22:52:41.000000 parmoo-0.2.2/examples/quickstart.py
+-rw-r--r--   0 tyler      (501) staff       (20)      582 2022-07-11 19:27:11.000000 parmoo-0.2.2/examples/unnamed_var_ex.out
+-rw-r--r--   0 tyler      (501) staff       (20)     2336 2022-05-10 21:22:59.000000 parmoo-0.2.2/examples/unnamed_var_ex.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.689890 parmoo-0.2.2/parmoo/
+-rw-r--r--   0 tyler      (501) staff       (20)      385 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.693600 parmoo-0.2.2/parmoo/acquisitions/
+-rw-r--r--   0 tyler      (501) staff       (20)      104 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/acquisitions/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     9122 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/acquisitions/epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15030 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/acquisitions/weighted_sum.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.695745 parmoo-0.2.2/parmoo/constraints/
+-rw-r--r--   0 tyler      (501) staff       (20)       60 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/constraints/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/constraints/const_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18473 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/constraints/const_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.697137 parmoo-0.2.2/parmoo/extras/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/extras/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    36753 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/extras/libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)   127469 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/moop.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.700816 parmoo-0.2.2/parmoo/objectives/
+-rw-r--r--   0 tyler      (501) staff       (20)       54 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/objectives/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    22933 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/objectives/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3448 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/objectives/obj_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16981 2022-07-26 17:47:19.000000 parmoo-0.2.2/parmoo/objectives/obj_lib.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.704385 parmoo-0.2.2/parmoo/optimizers/
+-rw-r--r--   0 tyler      (501) staff       (20)      122 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/optimizers/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17274 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)    20784 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8330 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/optimizers/random_search.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.705564 parmoo-0.2.2/parmoo/searches/
+-rw-r--r--   0 tyler      (501) staff       (20)       44 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/searches/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3736 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/searches/latin_hypercube.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.708606 parmoo-0.2.2/parmoo/simulations/
+-rw-r--r--   0 tyler      (501) staff       (20)       31 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/simulations/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    31184 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/simulations/dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1921 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/simulations/sim_func.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3905 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/simulations/simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16723 2023-04-10 18:11:54.000000 parmoo-0.2.2/parmoo/structs.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.710862 parmoo-0.2.2/parmoo/surrogates/
+-rw-r--r--   0 tyler      (501) staff       (20)       51 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/surrogates/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    33863 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/surrogates/gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17196 2023-03-17 16:31:56.000000 parmoo-0.2.2/parmoo/surrogates/linear_model.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.713497 parmoo-0.2.2/parmoo/tests/
+-rw-r--r--   0 tyler      (501) staff       (20)      103 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/.coveragerc
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.715011 parmoo-0.2.2/parmoo/tests/.pytest_cache/
+-rw-r--r--   0 tyler      (501) staff       (20)      194 2022-02-21 21:48:43.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 tyler      (501) staff       (20)      295 2022-02-21 21:48:43.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/README.md
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.614036 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.716990 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/
+-rw-r--r--   0 tyler      (501) staff       (20)     1948 2022-03-04 02:25:24.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 tyler      (501) staff       (20)        2 2022-03-04 02:25:24.000000 parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/__init__.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.718943 parmoo-0.2.2/parmoo/tests/libe_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/libe_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1305 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/libe_tests/libe_funcs.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3003 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/libe_tests/test_libe_gen.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.727130 parmoo-0.2.2/parmoo/tests/regression_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/regression_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2984 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3032 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2456 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2411 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3042 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_obj.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3391 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1941 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz5_sim.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2173 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_infeasible_prob.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2581 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_mixed_variables.py
+-rw-r--r--   0 tyler      (501) staff       (20)     2226 2022-05-10 17:20:56.000000 parmoo-0.2.2/parmoo/tests/regression_tests/test_user_func.py
+-rwxr-xr-x   0 tyler      (501) staff       (20)     2691 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/run-tests.sh
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.740940 parmoo-0.2.2/parmoo/tests/unit_tests/
+-rw-r--r--   0 tyler      (501) staff       (20)        0 2022-05-10 21:22:59.000000 parmoo-0.2.2/parmoo/tests/unit_tests/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8679 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_const_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4039 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_epsilon_constraint.py
+-rw-r--r--   0 tyler      (501) staff       (20)    15426 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_gaussian_proc.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7513 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_gps_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1649 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_latin_hypercube.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8800 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_lbfgsb.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6545 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_libe.py
+-rw-r--r--   0 tyler      (501) staff       (20)    79942 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop.py
+-rw-r--r--   0 tyler      (501) staff       (20)    27995 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_embeddings.py
+-rw-r--r--   0 tyler      (501) staff       (20)    16562 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_grads.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7035 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     8378 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_lib.py
+-rw-r--r--   0 tyler      (501) staff       (20)     3572 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_random_search.py
+-rw-r--r--   0 tyler      (501) staff       (20)     4745 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_dtlz.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1708 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_simple.py
+-rw-r--r--   0 tyler      (501) staff       (20)     1093 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_structs.py
+-rw-r--r--   0 tyler      (501) staff       (20)    10127 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_util.py
+-rw-r--r--   0 tyler      (501) staff       (20)    24842 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_viz_without_dash.py
+-rw-r--r--   0 tyler      (501) staff       (20)     7451 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/tests/unit_tests/test_weighted_sum.py
+-rw-r--r--   0 tyler      (501) staff       (20)    18801 2023-04-10 20:01:13.000000 parmoo-0.2.2/parmoo/util.py
+-rw-r--r--   0 tyler      (501) staff       (20)       22 2023-04-25 22:34:22.000000 parmoo-0.2.2/parmoo/version.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.744480 parmoo-0.2.2/parmoo/viz/
+-rw-r--r--   0 tyler      (501) staff       (20)      320 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/__init__.py
+-rw-r--r--   0 tyler      (501) staff       (20)    35252 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/dashboard.py
+-rw-r--r--   0 tyler      (501) staff       (20)     6079 2023-02-21 22:52:41.000000 parmoo-0.2.2/parmoo/viz/graph.py
+-rw-r--r--   0 tyler      (501) staff       (20)    17752 2023-04-24 17:53:17.000000 parmoo-0.2.2/parmoo/viz/plot.py
+-rw-r--r--   0 tyler      (501) staff       (20)    14067 2023-04-25 22:34:22.000000 parmoo-0.2.2/parmoo/viz/utilities.py
+drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-04-25 22:38:12.691837 parmoo-0.2.2/parmoo.egg-info/
+-rw-r--r--   0 tyler      (501) staff       (20)     1695 2023-04-25 22:38:11.000000 parmoo-0.2.2/parmoo.egg-info/PKG-INFO
+-rw-r--r--   0 tyler      (501) staff       (20)     4530 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/SOURCES.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        1 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/dependency_links.txt
+-rw-r--r--   0 tyler      (501) staff       (20)      120 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/requires.txt
+-rw-r--r--   0 tyler      (501) staff       (20)        7 2023-04-25 22:38:12.000000 parmoo-0.2.2/parmoo.egg-info/top_level.txt
+-rw-r--r--   0 tyler      (501) staff       (20)       38 2023-04-25 22:38:12.745518 parmoo-0.2.2/setup.cfg
+-rw-r--r--   0 tyler      (501) staff       (20)     3421 2023-04-24 18:05:49.000000 parmoo-0.2.2/setup.py
```

### Comparing `parmoo-0.2.1/CHANGELOG.rst` & `parmoo-0.2.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,23 @@
 =============
 
 Below are the release notes for ParMOO.
 
 May reference issues on:
 https://github.com/parmoo/parmoo/issues
 
+Release 0.2.2
+-------------
+
+:Date: Apr 25, 2023
+
+Hot-fix for a minor issue in the plotting library without workaround.
+
+ - Resolves #58
+
 Release 0.2.1
 -------------
 
 :Date: Apr 10, 2023
 
 Minor performance improvements, maintenance, and restructuring of test cases.
```

### Comparing `parmoo-0.2.1/CONTRIBUTING.rst` & `parmoo-0.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/LICENSE` & `parmoo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/MANIFEST.in` & `parmoo-0.2.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/PKG-INFO` & `parmoo-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
 Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `parmoo-0.2.1/README.rst` & `parmoo-0.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.1},
+        number      = {Version 0.2.2},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
 .. _Actions: https://github.com/parmoo/parmoo/actions
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _dash: https://dash.plotly.com
```

### Comparing `parmoo-0.2.1/docs/Makefile` & `parmoo-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/about.rst` & `parmoo-0.2.2/docs/about.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/conf.py` & `parmoo-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/dev-guide/release-proc.rst` & `parmoo-0.2.2/docs/dev-guide/release-proc.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/extras.rst` & `parmoo-0.2.2/docs/extras.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/how-to-write.rst` & `parmoo-0.2.2/docs/how-to-write.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/algorithm-flowchart.png` & `parmoo-0.2.2/docs/img/algorithm-flowchart.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/des-obj-space.png` & `parmoo-0.2.2/docs/img/des-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/des-sim-obj-space.png` & `parmoo-0.2.2/docs/img/des-sim-obj-space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/icon-ParMOO.png` & `parmoo-0.2.2/docs/img/icon-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/icon-ParMOO.svg` & `parmoo-0.2.2/docs/img/icon-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/icon-ParMOO_space.png` & `parmoo-0.2.2/docs/img/icon-ParMOO_space.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/logo-ParMOO.png` & `parmoo-0.2.2/docs/img/logo-ParMOO.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/logo-ParMOO.svg` & `parmoo-0.2.2/docs/img/logo-ParMOO.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/logo-ParMOO_white.png` & `parmoo-0.2.2/docs/img/logo-ParMOO_white.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/moop-uml.png` & `parmoo-0.2.2/docs/img/moop-uml.png`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/moop-uml.svg` & `parmoo-0.2.2/docs/img/moop-uml.svg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/moop.uml` & `parmoo-0.2.2/docs/img/moop.uml`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/img/parmoo_movie.gif` & `parmoo-0.2.2/docs/img/parmoo_movie.gif`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/index.rst` & `parmoo-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/install.rst` & `parmoo-0.2.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/latex_index.rst` & `parmoo-0.2.2/docs/latex_index.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/make.bat` & `parmoo-0.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/acquisitions.rst` & `parmoo-0.2.2/docs/modules/acquisitions.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/constraints.rst` & `parmoo-0.2.2/docs/modules/constraints.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/dtlz.rst` & `parmoo-0.2.2/docs/modules/dtlz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/libraries.rst` & `parmoo-0.2.2/docs/modules/libraries.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/moop.rst` & `parmoo-0.2.2/docs/modules/moop.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/objectives.rst` & `parmoo-0.2.2/docs/modules/objectives.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/optimizers.rst` & `parmoo-0.2.2/docs/modules/optimizers.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/searches.rst` & `parmoo-0.2.2/docs/modules/searches.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/structs.rst` & `parmoo-0.2.2/docs/modules/structs.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/surrogates.rst` & `parmoo-0.2.2/docs/modules/surrogates.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/modules/viz.rst` & `parmoo-0.2.2/docs/modules/viz.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/quickstart.rst` & `parmoo-0.2.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/refs.rst` & `parmoo-0.2.2/docs/refs.rst`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 .. code-block:: bibtex
 
     @techreport{parmoo-docs,
         title       = {{ParMOO}: {P}ython library for parallel multiobjective simulation optimization},
         author      = {Chang, Tyler H. and Wild, Stefan M. and Dickinson, Hyrum},
         institution = {Argonne National Laboratory},
-        number      = {Version 0.2.1},
+        number      = {Version 0.2.2},
         year        = {2023},
         url         = {https://parmoo.readthedocs.io/en/latest}
     }
 
 .. _CONTRIBUTING: https://github.com/parmoo/parmoo/blob/main/CONTRIBUTING.rst
 .. _LICENSE: https://github.com/parmoo/parmoo/blob/main/LICENSE
 .. _ReadTheDocs: https://parmoo.readthedocs.org
```

### Comparing `parmoo-0.2.1/docs/tutorials/basic-tutorials.rst` & `parmoo-0.2.2/docs/tutorials/basic-tutorials.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/docs/tutorials/libe-tutorial.rst` & `parmoo-0.2.2/docs/tutorials/libe-tutorial.rst`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/Makefile` & `parmoo-0.2.2/examples/Makefile`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/Pareto Front.jpeg` & `parmoo-0.2.2/examples/Pareto Front.jpeg`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/advanced_ex.out` & `parmoo-0.2.2/examples/advanced_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/advanced_ex.py` & `parmoo-0.2.2/examples/advanced_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/checkpointing.out` & `parmoo-0.2.2/examples/checkpointing.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/checkpointing.py` & `parmoo-0.2.2/examples/checkpointing.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/libe_basic_ex.out` & `parmoo-0.2.2/examples/libe_basic_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/libe_basic_ex.py` & `parmoo-0.2.2/examples/libe_basic_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/named_var_ex.py` & `parmoo-0.2.2/examples/named_var_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/precomputed_data.py` & `parmoo-0.2.2/examples/precomputed_data.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/quickstart.out` & `parmoo-0.2.2/examples/quickstart.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/quickstart.py` & `parmoo-0.2.2/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/unnamed_var_ex.out` & `parmoo-0.2.2/examples/unnamed_var_ex.out`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/examples/unnamed_var_ex.py` & `parmoo-0.2.2/examples/unnamed_var_ex.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/acquisitions/epsilon_constraint.py` & `parmoo-0.2.2/parmoo/acquisitions/epsilon_constraint.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/acquisitions/weighted_sum.py` & `parmoo-0.2.2/parmoo/acquisitions/weighted_sum.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/constraints/const_func.py` & `parmoo-0.2.2/parmoo/constraints/const_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/constraints/const_lib.py` & `parmoo-0.2.2/parmoo/constraints/const_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/extras/libe.py` & `parmoo-0.2.2/parmoo/extras/libe.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/moop.py` & `parmoo-0.2.2/parmoo/moop.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/objectives/dtlz.py` & `parmoo-0.2.2/parmoo/objectives/dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/objectives/obj_func.py` & `parmoo-0.2.2/parmoo/objectives/obj_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/objectives/obj_lib.py` & `parmoo-0.2.2/parmoo/objectives/obj_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/optimizers/gps_search.py` & `parmoo-0.2.2/parmoo/optimizers/gps_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/optimizers/lbfgsb.py` & `parmoo-0.2.2/parmoo/optimizers/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/optimizers/random_search.py` & `parmoo-0.2.2/parmoo/optimizers/random_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/searches/latin_hypercube.py` & `parmoo-0.2.2/parmoo/searches/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/simulations/dtlz.py` & `parmoo-0.2.2/parmoo/simulations/dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/simulations/sim_func.py` & `parmoo-0.2.2/parmoo/simulations/sim_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/simulations/simple.py` & `parmoo-0.2.2/parmoo/simulations/simple.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/structs.py` & `parmoo-0.2.2/parmoo/structs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/surrogates/gaussian_proc.py` & `parmoo-0.2.2/parmoo/surrogates/gaussian_proc.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/surrogates/linear_model.py` & `parmoo-0.2.2/parmoo/surrogates/linear_model.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/.pytest_cache/v/cache/nodeids` & `parmoo-0.2.2/parmoo/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/libe_tests/libe_funcs.py` & `parmoo-0.2.2/parmoo/tests/libe_tests/libe_funcs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/libe_tests/test_libe_gen.py` & `parmoo-0.2.2/parmoo/tests/libe_tests/test_libe_gen.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_obj.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz1_sim.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz1_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_obj.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz2_sim.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz2_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_obj.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_obj.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz3_sim.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz3_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_dtlz5_sim.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_dtlz5_sim.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_infeasible_prob.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_infeasible_prob.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_mixed_variables.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_mixed_variables.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/regression_tests/test_user_func.py` & `parmoo-0.2.2/parmoo/tests/regression_tests/test_user_func.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/run-tests.sh` & `parmoo-0.2.2/parmoo/tests/run-tests.sh`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_const_lib.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_const_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_epsilon_constraint.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_epsilon_constraint.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_gaussian_proc.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_gaussian_proc.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_gps_search.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_gps_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_latin_hypercube.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_lbfgsb.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_lbfgsb.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_libe.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_libe.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_moop.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_embeddings.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_embeddings.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_moop_grads.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_moop_grads.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_dtlz.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_obj_lib.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_obj_lib.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_random_search.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_random_search.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_dtlz.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_dtlz.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_sims_simple.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_sims_simple.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_structs.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_structs.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_util.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_util.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_viz_without_dash.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_viz_without_dash.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/tests/unit_tests/test_weighted_sum.py` & `parmoo-0.2.2/parmoo/tests/unit_tests/test_weighted_sum.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/util.py` & `parmoo-0.2.2/parmoo/util.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/viz/dashboard.py` & `parmoo-0.2.2/parmoo/viz/dashboard.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/viz/graph.py` & `parmoo-0.2.2/parmoo/viz/graph.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/viz/plot.py` & `parmoo-0.2.2/parmoo/viz/plot.py`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/parmoo/viz/utilities.py` & `parmoo-0.2.2/parmoo/viz/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,22 +103,22 @@
     else:
         if points == 'constraint_satisfying':
             constraints = moop.getConstraintType().names
             df = database.copy(deep=True)
             for constraint in constraints:
                 indices = df[df[constraint] > 0].index
                 df.drop(indices, inplace=True)
-                df.reset_index(inplace=True)
+                df.reset_index(inplace=True, drop=True)
         elif points == 'constraint_violating':
             constraints = moop.getConstraintType().names
             df = database.copy(deep=True)
             for constraint in constraints:
                 indices = df[df[constraint] <= 0].index
                 df.drop(indices, inplace=True)
-                df.reset_index(inplace=True)
+                df.reset_index(inplace=True, drop=True)
         elif points == 'all':
             df = database
         elif points == 'none':
             df = database[0:0]
     return df
```

### Comparing `parmoo-0.2.1/parmoo.egg-info/PKG-INFO` & `parmoo-0.2.2/parmoo.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parmoo
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python library for parallel multiobjective simulation optimization
 Home-page: https://github.com/parmoo/parmoo
 Author: Tyler H. Chang, Stefan M. Wild, et al.
 Author-email: parmoo@mcs.anl.gov
 License: BSD 3-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `parmoo-0.2.1/parmoo.egg-info/SOURCES.txt` & `parmoo-0.2.2/parmoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parmoo-0.2.1/setup.py` & `parmoo-0.2.2/setup.py`

 * *Files identical despite different names*

