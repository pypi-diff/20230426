# Comparing `tmp/fisinma-0.0.2.tar.gz` & `tmp/fisinma-0.1.0.tar.gz`

## Comparing `fisinma-0.0.2.tar` & `fisinma-0.1.0.tar`

### file list

```diff
@@ -1,93 +1,97 @@
--rw-r--r--   0        0        0    69632 2020-02-02 00:00:00.000000 fisinma-0.0.2/.coverage
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 fisinma-0.0.2/.git
--rw-r--r--   0        0        0    46344 2020-02-02 00:00:00.000000 fisinma-0.0.2/SpatSysBio-Python-Package-Find-Name.odt
--rw-r--r--   0        0        0    29123 2020-02-02 00:00:00.000000 fisinma-0.0.2/SpatSysBio-Python-Package-Find-Name.pdf
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fisinma-0.0.2/requirements.txt
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fisinma-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 fisinma-0.0.2/.github/workflows/linting.yml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fisinma-0.0.2/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 fisinma-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0    37646 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    88307 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/database/__init__.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/database/json.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/database/mongodb.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/model/__init__.py
--rw-r--r--   0        0        0    20795 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/model/fisher_model.py
--rw-r--r--   0        0        0     7341 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/model/preprocessing.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/optimization/__init__.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/optimization/caller.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/optimization/display.py
--rw-r--r--   0        0        0    10077 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/optimization/penalty.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/optimization/scipy_global_optim.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/plotting/__init__.py
--rw-r--r--   0        0        0     6530 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/plotting/plotting.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/solving/__init__.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/solving/criteria.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/solving/display.py
--rw-r--r--   0        0        0    13849 2020-02-02 00:00:00.000000 fisinma-0.0.2/FisInMa/solving/solve_fsm.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/Makefile
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/create_plots.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/make.bat
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/requirements-doc.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/conf.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/contributing.rst
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/index.rst
--rw-r--r--   0        0        0    30293 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/references.bib
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/_static/damped_osci_plots/output_example.txt
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/database.rst
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/index.rst
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/model.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/optimization.rst
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/plot_penalty_functions.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/plotting.rst
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/documentation/solving.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/index.rst
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/plot_discretization.py
--rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/examples/baranyi_roberts.rst
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/examples/damped_oscillator.rst
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/examples/index.rst
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/getting_started/examples/pool_model.rst
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/theoretical_overview/index.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fisinma-0.0.2/docs/source/theoretical_overview/theoretical_background/index.rst
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 fisinma-0.0.2/examples/baranyi_roberts.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 fisinma-0.0.2/examples/damped_oscillator.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 fisinma-0.0.2/examples/limited_growth.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 fisinma-0.0.2/examples/pool_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/database/__init__.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/database/test_json.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/model/__init__.py
--rw-r--r--   0        0        0    10208 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/model/test_fisher_model.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/model/test_preprocessing.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/optimization/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/optimization/test_caller.py
--rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/optimization/test_penalty.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/optimization/test_scipy_global_optim.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/setUp/__init__.py
--rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/setUp/fisher_model.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/setUp/pool_model.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/solving/__init__.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/solving/test_convergence.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/solving/test_covariance.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/solving/test_criterion.py
--rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 fisinma-0.0.2/test/solving/test_solver.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 fisinma-0.0.2/tools/analyze_docker.py
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 fisinma-0.0.2/tools/symbolic_diff.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fisinma-0.0.2/tools/tools.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fisinma-0.0.2/.gitignore
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fisinma-0.0.2/LICENSE
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 fisinma-0.0.2/README.md
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 fisinma-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 fisinma-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 fisinma-0.1.0/.git
+-rwxr-xr-x   0        0        0    46344 2020-02-02 00:00:00.000000 fisinma-0.1.0/SpatSysBio-Python-Package-Find-Name.odt
+-rwxr-xr-x   0        0        0    29123 2020-02-02 00:00:00.000000 fisinma-0.1.0/SpatSysBio-Python-Package-Find-Name.pdf
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 fisinma-0.1.0/requirements.txt
+-rwxr-xr-x   0        0        0      888 2020-02-02 00:00:00.000000 fisinma-0.1.0/.github/workflows/build.yml
+-rwxr-xr-x   0        0        0     1011 2020-02-02 00:00:00.000000 fisinma-0.1.0/.github/workflows/linting.yml
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 fisinma-0.1.0/.github/workflows/sphinx.yml
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 fisinma-0.1.0/.github/workflows/test.yml
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/.gitignore
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/README.md
+-rwxr-xr-x   0        0        0    37646 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/v/cache/lastfailed
+-rwxr-xr-x   0        0        0    88516 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/v/cache/nodeids
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.1.0/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/__init__.py
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/database/__init__.py
+-rwxr-xr-x   0        0        0     2091 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/database/json.py
+-rwxr-xr-x   0        0        0     2285 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/database/mongodb.py
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/model/__init__.py
+-rwxr-xr-x   0        0        0    20795 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/model/fisher_model.py
+-rwxr-xr-x   0        0        0     7341 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/model/preprocessing.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/optimization/__init__.py
+-rwxr-xr-x   0        0        0     6534 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/optimization/caller.py
+-rwxr-xr-x   0        0        0      746 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/optimization/display.py
+-rwxr-xr-x   0        0        0    10077 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/optimization/penalty.py
+-rwxr-xr-x   0        0        0     9923 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/optimization/scipy_global_optim.py
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/plotting/__init__.py
+-rwxr-xr-x   0        0        0     6530 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/plotting/plotting.py
+-rwxr-xr-x   0        0        0       72 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/solving/__init__.py
+-rwxr-xr-x   0        0        0     3144 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/solving/criteria.py
+-rwxr-xr-x   0        0        0     5166 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/solving/display.py
+-rwxr-xr-x   0        0        0    13830 2020-02-02 00:00:00.000000 fisinma-0.1.0/FisInMa/solving/solve_fsm.py
+-rwxr-xr-x   0        0        0      638 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/Makefile
+-rwxr-xr-x   0        0        0      448 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/create_plots.py
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/make.bat
+-rwxr-xr-x   0        0        0      103 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/requirements-doc.txt
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/.pytest_cache/.gitignore
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/.pytest_cache/CACHEDIR.TAG
+-rwxr-xr-x   0        0        0      302 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/.pytest_cache/README.md
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/.pytest_cache/v/cache/nodeids
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/.pytest_cache/v/cache/stepwise
+-rwxr-xr-x   0        0        0     1507 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/conf.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/contributing.rst
+-rwxr-xr-x   0        0        0     2705 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/index.rst
+-rwxr-xr-x   0        0        0    30293 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/references.bib
+-rwxr-xr-x   0        0        0     4267 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/_static/damped_osci_plots/output_example.txt
+-rwxr-xr-x   0        0        0      116 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/database.rst
+-rwxr-xr-x   0        0        0     2445 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/index.rst
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/model.rst
+-rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/optimization.rst
+-rwxr-xr-x   0        0        0     2498 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/plot_penalty_functions.py
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/plotting.rst
+-rwxr-xr-x   0        0        0      374 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/documentation/solving.rst
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/index.rst
+-rwxr-xr-x   0        0        0     1202 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/installation.rst
+-rwxr-xr-x   0        0        0     3572 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/examples/baranyi_roberts.rst
+-rwxr-xr-x   0        0        0     4539 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/examples/damped_oscillator.rst
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/examples/index.rst
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/getting_started/examples/pool_model.rst
+-rwxr-xr-x   0        0        0     1835 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/index.rst
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/theoretical_background/experimental_design.rst
+-rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/theoretical_background/index.rst
+-rwxr-xr-x   0        0        0      975 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/theoretical_background/model_formulation.rst
+-rwxr-xr-x   0        0        0     1076 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/theoretical_background/optimization.rst
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 fisinma-0.1.0/docs/source/theoretical_overview/theoretical_background/sensitivity_calculation.rst
+-rwxr-xr-x   0        0        0     2849 2020-02-02 00:00:00.000000 fisinma-0.1.0/examples/baranyi_roberts.py
+-rwxr-xr-x   0        0        0     2127 2020-02-02 00:00:00.000000 fisinma-0.1.0/examples/damped_oscillator.py
+-rwxr-xr-x   0        0        0     2184 2020-02-02 00:00:00.000000 fisinma-0.1.0/examples/limited_growth.py
+-rwxr-xr-x   0        0        0     3768 2020-02-02 00:00:00.000000 fisinma-0.1.0/examples/pool_model.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/database/__init__.py
+-rwxr-xr-x   0        0        0     1454 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/database/test_json.py
+-rwxr-xr-x   0        0        0       67 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/model/__init__.py
+-rwxr-xr-x   0        0        0    10208 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/model/test_fisher_model.py
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/model/test_preprocessing.py
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/optimization/__init__.py
+-rwxr-xr-x   0        0        0     2115 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/optimization/test_caller.py
+-rwxr-xr-x   0        0        0     6357 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/optimization/test_penalty.py
+-rwxr-xr-x   0        0        0     6958 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/optimization/test_scipy_global_optim.py
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/setUp/__init__.py
+-rwxr-xr-x   0        0        0     4969 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/setUp/extended_baranyi.py
+-rwxr-xr-x   0        0        0     5215 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/setUp/fisher_model.py
+-rwxr-xr-x   0        0        0     2829 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/setUp/pool_model.py
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/__init__.py
+-rwxr-xr-x   0        0        0     5629 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/test_convergence.py
+-rwxr-xr-x   0        0        0     2595 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/test_covariance.py
+-rwxr-xr-x   0        0        0     1237 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/test_criterion.py
+-rwxr-xr-x   0        0        0      884 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/test_observable_generation.py
+-rwxr-xr-x   0        0        0     4149 2020-02-02 00:00:00.000000 fisinma-0.1.0/test/solving/test_solver.py
+-rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 fisinma-0.1.0/tools/analyze_docker.py
+-rwxr-xr-x   0        0        0     3852 2020-02-02 00:00:00.000000 fisinma-0.1.0/tools/symbolic_diff.py
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 fisinma-0.1.0/tools/tools.md
+-rwxr-xr-x   0        0        0       60 2020-02-02 00:00:00.000000 fisinma-0.1.0/.gitignore
+-rwxr-xr-x   0        0        0     1055 2020-02-02 00:00:00.000000 fisinma-0.1.0/LICENSE
+-rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 fisinma-0.1.0/README.md
+-rwxr-xr-x   0        0        0     1038 2020-02-02 00:00:00.000000 fisinma-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 fisinma-0.1.0/PKG-INFO
```

### Comparing `fisinma-0.0.2/SpatSysBio-Python-Package-Find-Name.odt` & `fisinma-0.1.0/SpatSysBio-Python-Package-Find-Name.odt`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/SpatSysBio-Python-Package-Find-Name.pdf` & `fisinma-0.1.0/SpatSysBio-Python-Package-Find-Name.pdf`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.github/workflows/build.yml` & `fisinma-0.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.github/workflows/linting.yml` & `fisinma-0.1.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.github/workflows/sphinx.yml` & `fisinma-0.1.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.github/workflows/test.yml` & `fisinma-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.pytest_cache/v/cache/lastfailed` & `fisinma-0.1.0/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/.pytest_cache/v/cache/nodeids` & `fisinma-0.1.0/.pytest_cache/v/cache/nodeids`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978189749182116%*

 * *Differences: {'insert': '[(525, '*

 * *           "'test/solving/test_observable_generation.py::TestObservableGeneration::test_ode_sol_identical[False]'), "*

 * *           '(526, '*

 * *           "'test/solving/test_observable_generation.py::TestObservableGeneration::test_ode_sol_identical[True]')]"}*

```diff
@@ -520,14 +520,16 @@
     "test/solving/test_covariance.py::TestCovariance::test_covariance_def_2[True-True-True-3.0]",
     "test/solving/test_criterion.py::Test_Criteria::test_determinant",
     "test/solving/test_criterion.py::Test_Criteria::test_fisher_determinant",
     "test/solving/test_criterion.py::Test_Criteria::test_fisher_mineigenval",
     "test/solving/test_criterion.py::Test_Criteria::test_fisher_ratioeigenval",
     "test/solving/test_criterion.py::Test_Criteria::test_fisher_sumeigval",
     "test/solving/test_criterion.py::Test_Criteria::test_sumeigval",
+    "test/solving/test_observable_generation.py::TestObservableGeneration::test_ode_sol_identical[False]",
+    "test/solving/test_observable_generation.py::TestObservableGeneration::test_ode_sol_identical[True]",
     "test/solving/test_solver.py::TestClass::test_something1",
     "test/solving/test_solver.py::TestClass::test_something1[1]",
     "test/solving/test_solver.py::TestClass::test_something1[2]",
     "test/solving/test_solver.py::TestClass::test_something1[3]",
     "test/solving/test_solver.py::TestClass::test_something1[4]",
     "test/solving/test_solver.py::TestClass::test_something1[covar]",
     "test/solving/test_solver.py::TestClass::test_something1[critertion]",
```

### Comparing `fisinma-0.0.2/FisInMa/database/json.py` & `fisinma-0.1.0/FisInMa/database/json.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/database/mongodb.py` & `fisinma-0.1.0/FisInMa/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/model/fisher_model.py` & `fisinma-0.1.0/FisInMa/model/fisher_model.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/model/preprocessing.py` & `fisinma-0.1.0/FisInMa/model/preprocessing.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/optimization/caller.py` & `fisinma-0.1.0/FisInMa/optimization/caller.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/optimization/display.py` & `fisinma-0.1.0/FisInMa/optimization/display.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/optimization/penalty.py` & `fisinma-0.1.0/FisInMa/optimization/penalty.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/optimization/scipy_global_optim.py` & `fisinma-0.1.0/FisInMa/optimization/scipy_global_optim.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/plotting/plotting.py` & `fisinma-0.1.0/FisInMa/plotting/plotting.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/solving/criteria.py` & `fisinma-0.1.0/FisInMa/solving/criteria.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/solving/display.py` & `fisinma-0.1.0/FisInMa/solving/display.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/FisInMa/solving/solve_fsm.py` & `fisinma-0.1.0/FisInMa/solving/solve_fsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,15 @@
         # Calculate the first term of the equation
         term1 = np.array([fsmp.obs_dgdp(ti, x[:,i_t], Q, fsmp.parameters, fsmp.ode_args) for i_t, ti in enumerate(t)]).reshape((n_t, n_obs, n_p)).swapaxes(0, 2)
 
         # Calculate the second term of the equation and add them
         term2 = np.array([
             # This has shape (n_x, n_obs)
             np.array(fsmp.obs_dgdx(ti, x[:,i], Q, fsmp.parameters, fsmp.ode_args), dtype=float)
-                .reshape((n_x, n_obs))
-                .T
+                .reshape((n_obs, n_x))
                 .dot(s[:n_p,:,i].T)
             for i, ti in enumerate(t)
         ]).reshape((n_t, n_obs, n_p)).swapaxes(0, 2)
 
         if callable(fsmp.ode_dfdx0) and callable(fsmp.obs_dgdx0):
             # Calculate term1_add which is dgdx0_ik for every time point in t
             term1_add = np.array([
```

### Comparing `fisinma-0.0.2/docs/Makefile` & `fisinma-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/make.bat` & `fisinma-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/conf.py` & `fisinma-0.1.0/docs/source/conf.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'FisInMa'
 copyright = '2022, Jonas Pleyer, Polina Gaindrik'
 author = 'Jonas Pleyer, Polina Gaindrik'
-release = '0.0.1'
+release = '0.0.2'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
@@ -36,9 +36,15 @@
 templates_path = ['_templates']
 exclude_patterns = ['_build', '_templates', 'Thumbs.db', '.DS_Store']
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = 'pydata_sphinx_theme'
+html_theme_options = {
+   "logo": {
+      "image_light": "logo-light.png",
+      "image_dark": "logo-dark.png",
+   }
+}
 html_static_path = ['_static']
 bibtex_bibfiles = ['references.bib']
```

### Comparing `fisinma-0.0.2/docs/source/index.rst` & `fisinma-0.1.0/docs/source/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,19 +16,19 @@
    \end{alignat}
    :label: overview_ode_def
 
 When designing real-life experiments, researchers need to choose appropriate time- and input-datapoints to gain the maximum amount of information to accurately determine the parameters describing the system.
 This package assumes that the structure of the experiment is determined by an ODE which can in general be written in explicit form as in equation :eq:`overview_ode_def`.
 The input variables :math:`u` are known numerical values and alter the behaviour of the system while the experiment aims to estimate the parameters :math:`p`.
 To optimally design an experiment (ie. choose time-points :math:`t_i` or configurations for input values :math:`u`), we want to maximize the total information obtained by the measurements.
-The package uses the Fisher Information method in which we calculate the sensitivities.
+The package uses the Fisher Information method in which we calculate the sensitivities
 
 .. math::
    \begin{equation}
-      S_{ij} = \frac{\partial x_i}{\partial p_j}(t_k, u_l)
+      s_{ij} = \frac{\partial x_i}{\partial p_j}(t_k, u_l)
    \end{equation}
 
 and afterwards the Fisher Information matrix :math:`F` (optionally with covariance matrix :math:`C` determined by specified uncertainties).
 
 .. math::
    \begin{equation}
       F = S^T C^{-1} S
```

### Comparing `fisinma-0.0.2/docs/source/references.bib` & `fisinma-0.1.0/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/_static/damped_osci_plots/output_example.txt` & `fisinma-0.1.0/docs/source/_static/damped_osci_plots/output_example.txt`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/documentation/index.rst` & `fisinma-0.1.0/docs/source/documentation/index.rst`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/documentation/optimization.rst` & `fisinma-0.1.0/docs/source/documentation/optimization.rst`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/documentation/plot_penalty_functions.py` & `fisinma-0.1.0/docs/source/documentation/plot_penalty_functions.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/getting_started/installation.rst` & `fisinma-0.1.0/docs/source/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/getting_started/examples/baranyi_roberts.rst` & `fisinma-0.1.0/docs/source/getting_started/examples/baranyi_roberts.rst`

 * *Files 4% similar despite different names*

```diff
@@ -35,70 +35,68 @@
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
    :lineno-start: 8
    :lines: 8-53
 
-As an observable, it is pretty common to measure the bacteria count :math:`x_1` or the logarithm of this value. 
-For simplicity, we would consider the prior case :math:`y(t_i) = x_1(t_i)`.
-
-.. literalinclude:: ../../../../examples/baranyi_roberts.py
-   :language: python
-   :linenos:
-   :lineno-start: 55
-   :lines: 55-77
-
 Define the parameters of the system :code:`p` and initial conditions :code:`x0`.
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 82
-   :lines: 82-83
+   :lineno-start: 58
+   :lines: 58-59
 
 Define optimization of 6 time points with lower bound :code:`0.0`, upper bound :code:`10.0`.
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 86
-   :lines: 86
+   :lineno-start: 62
+   :lines: 62
 
 Define optimization of one input value (temperature) with lower bound :code:`3.0`, upper bound :code:`12.0`.
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 89
-   :lines: 89
+   :lineno-start: 65
+   :lines: 65
+
+As an observable, it is pretty common to measure the bacteria count :math:`x_1` or the logarithm of this value. 
+For simplicity, we would consider the prior case where the observable is the null-component of the state variable vector :math:`y(t_i) = x_1(t_i)`.
+
+.. code-block:: python3
+
+   obs_fun = 0
 
 The resulting Fisher Model:
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 93
-   :lines: 93-107
+   :lineno-start: 69
+   :lines: 69-81
 
 The optimization is then held using relative sensitivities and D-optimality criterion (determinant).
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 109
-   :lines: 109-117
+   :lineno-start: 83
+   :lines: 83-91
 
 Save and plot the results of optimization.
 
 .. literalinclude:: ../../../../examples/baranyi_roberts.py
    :language: python
    :linenos:
-   :lineno-start: 121
-   :lines: 121-122
+   :lineno-start: 95
+   :lines: 95-96
 
 The resulting Optimal Experimental Design:
 
 .. figure:: ../../../source/_static/baranyi_roberts/Observable_Results_baranyi_roberts_ode_fisher_determinant_rel_sensit_cont_6times_1temps_000_x_00.svg
     :align: center
     :width: 400
```

### Comparing `fisinma-0.0.2/docs/source/getting_started/examples/damped_oscillator.rst` & `fisinma-0.1.0/docs/source/getting_started/examples/damped_oscillator.rst`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/docs/source/theoretical_overview/index.rst` & `fisinma-0.1.0/docs/source/theoretical_overview/index.rst`

 * *Files 23% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 
 .. toctree::
    :maxdepth: 2
    :hidden:
 
    Theoretical Background <theoretical_background/index>
 
-Mathematical modeling is a widely used tool to describe, understand and predict further behavior of living systems.
-In particular, in the field of Predictive Biology, one can find a large variety of works that dwell on building models of different levels of complexity controlled by model parameters, e.g., to describe bacteria growth :cite:p:`bernaertsConceptsToolsPredictive2004`.
-Based on a chosen model structure, these parameters can be estimated from the gathered experimental data.
-Taking into account that the real experimental data always contains measurement noise, the parameter estimates can be only provided with some uncertainty. 
-To decrease the error of the parameter values, not only enough experimental data should be gathered but the quality of this data is also pretty sufficient.
-That rises quite an important question of finding the Optimal Experimental Design (OED) where optimized experimental conditions and/or times allow one to reduce the number of measurements without loss of information thus sparing an effort of experimenters :cite:p:`derlindenImpactExperimentDesign2013, balsa-cantoe.bangaj.r.COMPUTINGOPTIMALDYNAMIC2008`.
+The parameter estimation from the gathered experimental data is a significant part of the mathematical modeling of the real-life system.
+However, due to constant measurement noise, the parameter values are always found with some uncertainty.
+To reduce this error, the Experimental Design should be optimized to increase the informational worth of the data :cite:p:`derlindenImpactExperimentDesign2013, balsa-cantoe.bangaj.r.COMPUTINGOPTIMALDYNAMIC2008`.
 
 The Experimental Design works iteratively with parameter estimation process.
-Firstly, based on the literature review or prior data from pilot experiments, the first parameter estimation of the chosen model structure should be done.
-The obtained values can be applied to propose the first optimal experimental design accounting for different constraints, e.g., the lab limitations, human resources, etc. 
-Depending on availability, either real or numerical experiments should be conducted based on this design to gather measurement or in-silico data. 
-This new data can be used for the new parameter estimations values with corresponding uncertainties.
+Firstly, using the chosen model structure and the first parameter estimated values, the first optimal experimental design can be proposed accounting for different constraints.
+Then depending on availability, either real or numerical experiments should be conducted based on this design to gather measurement or in-silico data. 
+This new data can be used for the new parameter estimations with corresponding uncertainties.
 After this, using new parameter values, the process can be repeated several times to increase the precision of the parameter estimates till the desired accuracy is achieved.
 
 .. figure:: ExpDesign_workflow.png
     :align: center
     :width: 300
 
     The workflow of the iterative process of model optimization for parameter estimation.
 
 In this library, we present the implementation of the Experimental Design part of the described process for a specific type of model.
 We are interested in systems widely used in Systems Biology and described by Ordinary Differential Equations (ODE).
 
 .. bibliography::
     :style: plain
+    :filter: False
+
+    derlindenImpactExperimentDesign2013
+    balsa-cantoe.bangaj.r.COMPUTINGOPTIMALDYNAMIC2008
```

### Comparing `fisinma-0.0.2/examples/baranyi_roberts.py` & `fisinma-0.1.0/examples/baranyi_roberts.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,51 +3,52 @@
 import os, sys
 sys.path.append(os.getcwd())
 from FisInMa import *
 
 
 def baranyi_roberts_ode(t, x, u, p, ode_args):
     x1, x2 = x
-    Temp, = u
-    x_max, b, Temp_min = p
+    (Temp, ) = u
+    (x_max, b, Temp_min) = p
+    # Define the maximum growth rate
     mu_max = b**2 * (Temp - Temp_min)**2
     return [
-        mu_max * (x2/(x2 + 1)) * (1 - x1/x_max) * x1,
-        mu_max * x2
+        mu_max * (x2/(x2 + 1)) * (1 - x1/x_max) * x1,           # f1
+        mu_max * x2                                             # f2
     ]
 
 def ode_dfdp(t, x, u, p, ode_args):
     x1, x2 = x
-    Temp, = u
-    x_max, b, Temp_min = p
+    (Temp, ) = u
+    (x_max, b, Temp_min) = p
     mu_max = b**2 * (Temp - Temp_min)**2
     return [
         [
-            mu_max*(x2/(x2 + 1))*(x1/x_max)**2,
-             2*b*(Temp - Temp_min)**2*(x2/(x2 + 1))
-                *(1 - x1/x_max)*x1,
-            -2*b**2 * (Temp - Temp_min)*(x2/(x2 + 1))
-                *(1 - x1/x_max)*x1
+            mu_max * (x2/(x2 + 1)) * (x1/x_max)**2,             # df1/dx_max
+             2 * b * (Temp - Temp_min)**2 * (x2/(x2 + 1))
+                * (1 - x1/x_max)*x1,                            # df1/db
+            -2 * b**2 * (Temp - Temp_min) * (x2/(x2 + 1))
+                * (1 - x1/x_max)*x1                             # df1/dTemp_min
         ],
         [
-            0,
-            2*b*(Temp - Temp_min)**2*x2,
-            2*b**2*(Temp - Temp_min)*x2
+            0,                                                  # df2/dx_max
+            2 * b * (Temp - Temp_min)**2 * x2,                  # df2/db
+            -2 * b**2 * (Temp - Temp_min) * x2                  # df2/dTemp_min
         ]
     ]
 
 def ode_dfdx(t, x, u, p, ode_args):
     x1, x2 = x
-    Temp, = u
-    x_max, b, Temp_min = p
+    (Temp, ) = u
+    (x_max, b, Temp_min) = p
     mu_max = b**2 * (Temp - Temp_min)**2
     return [
         [
-            mu_max * (x2/(x2 + 1)) * (1 - 2*x1/x_max),
-            mu_max * 1/(x2 + 1)**2 * (1 - x1/x_max)*x1
+            mu_max * (x2/(x2 + 1)) * (1 - 2*x1/x_max),          # df1/dx1
+            mu_max * 1/(x2 + 1)**2 * (1 - x1/x_max)*x1          # df1/dx2
         ],
         [
             0,                                                  # df2/dx1
             mu_max                                              # df2/dx2
         ]
     ]
 
@@ -57,22 +58,15 @@
     p = (1e8, 0.2, 1.0) # (x_max, b, T_min)
     x0 = np.array([1e3, 0.1]) 
 
     # Define interval and number of sampling points for times
     times = {"lb": 0.0, "ub": 10.0, "n": 6}
 
     # Define explicit temperature points
-    Temp_low = 8.0
-    Temp_high = 10.0
-    n_Temp = 1
-
-    # Summarize all input definitions in list (only temperatures)
-    inputs = [
-        np.linspace(Temp_low, Temp_high, n_Temp)
-    ]
+    inputs = [{"lb": 3.0, "ub": 12.0, "n": 1}]
 
     # Create the FisherModel which serves as the entry point
     #  for the solving and optimization algorithms
     fsm = FisherModel(
         ode_x0=x0,
         ode_t0=0.0,
         ode_fun=baranyi_roberts_ode,
```

### Comparing `fisinma-0.0.2/examples/damped_oscillator.py` & `fisinma-0.1.0/examples/damped_oscillator.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/examples/limited_growth.py` & `fisinma-0.1.0/examples/limited_growth.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/examples/pool_model.py` & `fisinma-0.1.0/examples/pool_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ### USER DEFINES ODE SYSTEM ###
 ###############################
 def pool_model(t, y, Q, P, Const):
     a, b = P
     Temp, = Q
     n0, c, n_max = Const
     n, = y
-    return (a*Temp + c) * (n - n0*np.exp(-b*Temp*t))*(1-n/n_max)
+    return [(a*Temp + c) * (n - n0*np.exp(-b*Temp*t))*(1-n/n_max)]
 
 def dfdx(t, y, Q, P, Const):
     a, b = P
     Temp, = Q
     n0, c, n_max = Const
     n, = y
     return (a*Temp + c) * (1-n/n_max) + (a*Temp + c) * (n - n0*np.exp(-b*Temp*t))*(-1/n_max)
@@ -55,32 +55,34 @@
     return [
         [(a*Temp + c) * (- np.exp(-b*Temp*t))*(1-n/n_max)]
     ]
 
 def g(t, y, Q, P, Const):
     n0, c, n_max = Const
     n, = y
-    return [np.log((n+n0)/n0), n, n**2]
+    return [np.log((n+n0)/n0)]
 
 def dgdx(t, y, Q, P, Const):
     n0, c, n_max = Const
     n, = y
-    return [1 / (n+n0), 1, 2*n]
+    return [
+        [1 / (n+n0)]
+    ]
 
 def dgdp(t, y, Q, P, Const):
     return [
-        [0, 0],
-        [0, 0],
-        [0, 0],
+        [0, 0]
     ]
 
 def dgdx0(t, y, Q, P, Const):
     n0, c, n_max = Const
     n, = y
-    return [- n /(n0*(n+n0)), 0, 0]
+    return [
+        [- n /(n0*(n+n0))]
+    ]
 
 
 if __name__ == "__main__":
     ###############################
     ### USER DEFINES PARAMETERS ###
     ###############################
 
@@ -106,16 +108,16 @@
     times_low = t0
     times_high = 16.0
     # Discretize explicitly
     # dtimes = [2.0, 4.0, 5.0]
     dtimes = 0.5
 
     # Construct parameter hyperspace
-    n_times = 2
-    n_temps = 2
+    n_times = 6
+    n_temps = 1
 
     # Values for temperatures (Q-Values)
     inputs = [
         np.linspace(temp_low, temp_high, n_temps),
         # {"lb": temp_low, "ub": temp_high, "n": n_temps},
     ]
     # Values for times (can be same for every temperature or different)
```

### Comparing `fisinma-0.0.2/test/database/test_json.py` & `fisinma-0.1.0/test/database/test_json.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/model/test_fisher_model.py` & `fisinma-0.1.0/test/model/test_fisher_model.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/model/test_preprocessing.py` & `fisinma-0.1.0/test/model/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/optimization/test_caller.py` & `fisinma-0.1.0/test/optimization/test_caller.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/optimization/test_penalty.py` & `fisinma-0.1.0/test/optimization/test_penalty.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/optimization/test_scipy_global_optim.py` & `fisinma-0.1.0/test/optimization/test_scipy_global_optim.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/setUp/fisher_model.py` & `fisinma-0.1.0/test/setUp/fisher_model.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/setUp/pool_model.py` & `fisinma-0.1.0/test/setUp/pool_model.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/solving/test_convergence.py` & `fisinma-0.1.0/test/solving/test_convergence.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/solving/test_covariance.py` & `fisinma-0.1.0/test/solving/test_covariance.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/solving/test_criterion.py` & `fisinma-0.1.0/test/solving/test_criterion.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/test/solving/test_solver.py` & `fisinma-0.1.0/test/solving/test_solver.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/tools/symbolic_diff.py` & `fisinma-0.1.0/tools/symbolic_diff.py`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/tools/tools.md` & `fisinma-0.1.0/tools/tools.md`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/LICENSE` & `fisinma-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fisinma-0.0.2/README.md` & `fisinma-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Build%20Package?style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Create%20Docs?label=docs&style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Test-Suite?label=tests&style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Check%20Linting?label=checks&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/build.yml?style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/sphinx.yml?label=docs&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/test.yml?label=tests&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/linting.yml?label=checks&style=flat-square)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fisinma?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/fisinma?style=flat-square)
 
 # Fischer Information Matrix (FisInMa)
 This tools analyzes ODEs for optimality criteria and maximes their Fischer Information Matrix (see [Wikipedia](https://en.wikipedia.org/wiki/Fisher_information) )
```

### Comparing `fisinma-0.0.2/pyproject.toml` & `fisinma-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FisInMa"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Jonas Pleyer", email="jonas.pleyer@fdm.uni-freiburg.de" },
   { name="Polina Gaindrik", email="p.gaindrik@tsenso.com" },
 ]
 dependencies = [
   "matplotlib",
   "numpy",
```

### Comparing `fisinma-0.0.2/PKG-INFO` & `fisinma-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FisInMa
-Version: 0.0.2
+Version: 0.1.0
 Summary: Optimal experimental design utilizing the Fischer information matrix
 Project-URL: Home-page, https://github.com/Spatial-Systems-Biology-Freiburg/Model-Design-Fischer-Information-Matrix
 Project-URL: Bug Tracker, https://github.com/Spatial-Systems-Biology-Freiburg/Model-Design-Fischer-Information-Matrix/issues
 Project-URL: Documentation, https://spatial-systems-biology-freiburg.github.io/FisInMa/
 Project-URL: Source code, https://github.com/Spatial-Systems-Biology-Freiburg/FisInMa
 Author-email: Jonas Pleyer <jonas.pleyer@fdm.uni-freiburg.de>, Polina Gaindrik <p.gaindrik@tsenso.com>
 License-File: LICENSE
@@ -16,18 +16,18 @@
 Requires-Dist: numpy
 Requires-Dist: pydantic
 Requires-Dist: pymongo
 Requires-Dist: pytest
 Requires-Dist: scipy
 Description-Content-Type: text/markdown
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Build%20Package?style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Create%20Docs?label=docs&style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Test-Suite?label=tests&style=flat-square)
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/Check%20Linting?label=checks&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/build.yml?style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/sphinx.yml?label=docs&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/test.yml?label=tests&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/Spatial-Systems-Biology-Freiburg/FisInMa/linting.yml?label=checks&style=flat-square)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fisinma?style=flat-square)
 ![PyPI - License](https://img.shields.io/pypi/l/fisinma?style=flat-square)
 
 # Fischer Information Matrix (FisInMa)
 This tools analyzes ODEs for optimality criteria and maximes their Fischer Information Matrix (see [Wikipedia](https://en.wikipedia.org/wiki/Fisher_information) )
```

