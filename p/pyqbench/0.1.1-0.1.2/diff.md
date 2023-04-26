# Comparing `tmp/pyqbench-0.1.1.tar.gz` & `tmp/pyqbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqbench-0.1.1.tar", last modified: Sat Dec 24 16:29:57 2022, max compression
+gzip compressed data, was "pyqbench-0.1.2.tar", last modified: Tue Apr 25 19:20:55 2023, max compression
```

## Comparing `pyqbench-0.1.1.tar` & `pyqbench-0.1.2.tar`

### file list

```diff
@@ -1,123 +1,133 @@
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.724323 pyqbench-0.1.1/
--rw-r--r--   0 dexter    (1000) dexter    (1000)       31 2022-07-05 14:37:08.000000 pyqbench-0.1.1/.flake8
--rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-07-05 14:37:08.000000 pyqbench-0.1.1/.git_archival.txt
--rw-r--r--   0 dexter    (1000) dexter    (1000)       32 2022-07-05 14:37:08.000000 pyqbench-0.1.1/.gitattributes
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.715323 pyqbench-0.1.1/.github/
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.717323 pyqbench-0.1.1/.github/workflows/
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1443 2022-11-14 12:48:19.000000 pyqbench-0.1.1/.github/workflows/quality_checks.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1825 2022-07-05 14:37:08.000000 pyqbench-0.1.1/.gitignore
--rw-r--r--   0 dexter    (1000) dexter    (1000)      651 2022-11-14 12:48:19.000000 pyqbench-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     4123 2022-12-24 16:10:48.000000 pyqbench-0.1.1/Hadamard example.ipynb
--rw-r--r--   0 dexter    (1000) dexter    (1000)    11357 2022-07-05 14:37:08.000000 pyqbench-0.1.1/LICENSE
--rw-r--r--   0 dexter    (1000) dexter    (1000)      896 2022-12-24 16:29:57.724323 pyqbench-0.1.1/PKG-INFO
--rw-r--r--   0 dexter    (1000) dexter    (1000)      156 2022-12-24 16:10:43.000000 pyqbench-0.1.1/README.md
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.718323 pyqbench-0.1.1/adr/
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2759 2022-11-14 12:48:19.000000 pyqbench-0.1.1/adr/async_backends.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2519 2022-11-14 12:48:19.000000 pyqbench-0.1.1/adr/backend_factory_model.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1113 2022-11-14 12:48:19.000000 pyqbench-0.1.1/adr/fourier-discrimination-cli.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2075 2022-11-14 12:48:19.000000 pyqbench-0.1.1/adr/general_form_of_the_cli.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1979 2022-11-14 12:48:19.000000 pyqbench-0.1.1/adr/simple_backend_model.md
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.718323 pyqbench-0.1.1/docs/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      638 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/Makefile
--rw-r--r--   0 dexter    (1000) dexter    (1000)      769 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/make.bat
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.719323 pyqbench-0.1.1/docs/source/
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.716323 pyqbench-0.1.1/docs/source/_static/
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.719323 pyqbench-0.1.1/docs/source/_static/css/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      434 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/_static/css/custom.css
--rw-r--r--   0 dexter    (1000) dexter    (1000)        9 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/citing.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      579 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/cli_usage.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1256 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/conf.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)        6 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/faq.md
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.719323 pyqbench-0.1.1/docs/source/img/
--rw-r--r--   0 dexter    (1000) dexter    (1000)   132519 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/img/hadamard_u_v0.svg
--rw-r--r--   0 dexter    (1000) dexter    (1000)      303 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/index.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3278 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/installing.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      189 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/mathematical_foundations.md
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.719323 pyqbench-0.1.1/docs/source/notebooks/
--rw-r--r--   0 dexter    (1000) dexter    (1000)    37160 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/notebooks/Example 01 discriminating measurements in Hadamard basis.ipynb
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.720323 pyqbench-0.1.1/docs/source/reference/
--rw-r--r--   0 dexter    (1000) dexter    (1000)       93 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/batching.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)       83 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/cli.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      103 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/common_models.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      235 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/fourier.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      121 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/index.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)       85 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/jobs.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)       89 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/limits.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)       91 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/logging.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      228 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/schemes.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)       91 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/reference/testing.md
--rw-r--r--   0 dexter    (1000) dexter    (1000)      600 2022-12-24 16:10:48.000000 pyqbench-0.1.1/docs/source/tutorial.md
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.720323 pyqbench-0.1.1/examples/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      103 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/backend-factory-with-run-options.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)       73 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/backend-factory.yml
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.721323 pyqbench-0.1.1/examples/backends/
--rw-r--r--   0 dexter    (1000) dexter    (1000)       98 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/backends/ibmq-qasm-simulator-async.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)       99 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/backends/ibmq-qasm-simulator-sync.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)       89 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/backends/ibmq-quito.yml
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.721323 pyqbench-0.1.1/examples/experiments/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      164 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/experiments/fourier-disc-direct-sum-ibmq.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)      167 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/experiments/fourier-disc-postselection-ibmq.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1252 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/fourier-discrimination-async-result.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)      225 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/fourier-discrimination-experiment.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3943 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/fourier-discrimination-result-with-mitigation.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1519 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/fourier-discrimination-result.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)       92 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/ibmq-backend.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)      125 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/simple-backend-with-run-options.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)       64 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/simple-backend.yml
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1249 2022-12-24 16:10:48.000000 pyqbench-0.1.1/examples/using_fourier_with_simulator.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1265 2022-11-14 12:48:19.000000 pyqbench-0.1.1/examples/using_fourier_with_simulator_postselection_all_cases.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1760 2022-12-24 16:10:48.000000 pyqbench-0.1.1/pyproject.toml
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.721323 pyqbench-0.1.1/pyqbench.egg-info/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      896 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/PKG-INFO
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3034 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/SOURCES.txt
--rw-r--r--   0 dexter    (1000) dexter    (1000)        1 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/dependency_links.txt
--rw-r--r--   0 dexter    (1000) dexter    (1000)       43 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/entry_points.txt
--rw-r--r--   0 dexter    (1000) dexter    (1000)      398 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/requires.txt
--rw-r--r--   0 dexter    (1000) dexter    (1000)       42 2022-12-24 16:29:57.000000 pyqbench-0.1.1/pyqbench.egg-info/top_level.txt
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.722323 pyqbench-0.1.1/qbench/
--rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-07-05 14:37:08.000000 pyqbench-0.1.1/qbench/__init__.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1367 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/_expressions.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3198 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/batching.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      548 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/cli.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     4785 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/common_models.py
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.722323 pyqbench-0.1.1/qbench/fourier/
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1220 2022-12-24 16:10:48.000000 pyqbench-0.1.1/qbench/fourier/__init__.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     6094 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_cli.py
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.722323 pyqbench-0.1.1/qbench/fourier/_components/
--rw-r--r--   0 dexter    (1000) dexter    (1000)     4228 2022-12-24 16:10:48.000000 pyqbench-0.1.1/qbench/fourier/_components/__init__.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1445 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_components/_generic.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      999 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_components/_ibmq.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1003 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_components/_lucy.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1118 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_components/_lucy_and_ibmq_common.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2729 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_components/_rigetti.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2570 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/_models.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)    14376 2022-12-24 16:10:48.000000 pyqbench-0.1.1/qbench/fourier/experiment_runner.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2221 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/fourier/testing.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      890 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/jobs.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1911 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/limits.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1298 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/logging.py
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.723323 pyqbench-0.1.1/qbench/schemes/
--rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/schemes/__init__.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      828 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/schemes/_utils.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     5315 2022-12-24 16:10:48.000000 pyqbench-0.1.1/qbench/schemes/direct_sum.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     6348 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/schemes/postselection.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     4151 2022-11-14 12:48:19.000000 pyqbench-0.1.1/qbench/testing.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)       38 2022-12-24 16:29:57.724323 pyqbench-0.1.1/setup.cfg
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.723323 pyqbench-0.1.1/tests/
--rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-07-05 14:37:08.000000 pyqbench-0.1.1/tests/__init__.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      799 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/conftest.py
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.724323 pyqbench-0.1.1/tests/fourier/
--rw-r--r--   0 dexter    (1000) dexter    (1000)     4176 2022-12-24 16:10:48.000000 pyqbench-0.1.1/tests/fourier/test_fourier.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     5976 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/fourier/test_fourier_cli.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3450 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/fourier/test_fourier_experiment_runner.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1543 2022-12-24 16:10:48.000000 pyqbench-0.1.1/tests/fourier/test_fourier_ibmq.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1581 2022-12-24 16:10:48.000000 pyqbench-0.1.1/tests/fourier/test_fourier_lucy.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1633 2022-12-24 16:10:48.000000 pyqbench-0.1.1/tests/fourier/test_fourier_rigetti.py
-drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2022-12-24 16:29:57.724323 pyqbench-0.1.1/tests/schemes/
--rw-r--r--   0 dexter    (1000) dexter    (1000)      838 2022-12-24 16:10:48.000000 pyqbench-0.1.1/tests/schemes/test_direct_sum.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)      851 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/schemes/test_postselection.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     3540 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/test_batching.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1540 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/test_ibmq_backend.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     2809 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/test_limits.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)     1208 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/test_mock_simulator.py
--rw-r--r--   0 dexter    (1000) dexter    (1000)    10097 2022-11-14 12:48:19.000000 pyqbench-0.1.1/tests/test_models.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.933277 pyqbench-0.1.2/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       31 2022-06-14 21:57:00.000000 pyqbench-0.1.2/.flake8
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-06-14 21:57:00.000000 pyqbench-0.1.2/.git_archival.txt
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       32 2022-06-14 21:57:00.000000 pyqbench-0.1.2/.gitattributes
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.922277 pyqbench-0.1.2/.github/
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.924277 pyqbench-0.1.2/.github/workflows/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1569 2023-04-25 18:11:08.000000 pyqbench-0.1.2/.github/workflows/quality_checks.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1825 2022-06-14 21:57:00.000000 pyqbench-0.1.2/.gitignore
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      680 2023-02-05 16:27:22.000000 pyqbench-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      121 2023-01-03 10:47:11.000000 pyqbench-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4123 2023-01-03 10:47:11.000000 pyqbench-0.1.2/Hadamard example.ipynb
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    11357 2022-01-17 10:25:46.000000 pyqbench-0.1.2/LICENSE
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4984 2023-04-25 19:20:55.932277 pyqbench-0.1.2/PKG-INFO
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4244 2023-04-25 18:11:08.000000 pyqbench-0.1.2/README.md
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.925277 pyqbench-0.1.2/adr/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2759 2022-09-25 22:53:31.000000 pyqbench-0.1.2/adr/async_backends.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2519 2022-09-13 16:41:45.000000 pyqbench-0.1.2/adr/backend_factory_model.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1113 2022-09-14 12:06:29.000000 pyqbench-0.1.2/adr/fourier-discrimination-cli.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2075 2022-09-14 12:06:29.000000 pyqbench-0.1.2/adr/general_form_of_the_cli.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1979 2022-09-13 16:41:45.000000 pyqbench-0.1.2/adr/simple_backend_model.md
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.925277 pyqbench-0.1.2/docs/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      638 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/Makefile
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      769 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/make.bat
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.926277 pyqbench-0.1.2/docs/source/
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.926277 pyqbench-0.1.2/docs/source/_static/
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.926277 pyqbench-0.1.2/docs/source/_static/css/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      599 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/_static/css/custom.css
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    97197 2023-01-03 12:04:04.000000 pyqbench-0.1.2/docs/source/_static/logo.png
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        9 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/citing.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    14139 2023-02-05 16:28:07.000000 pyqbench-0.1.2/docs/source/cli_usage.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2131 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/conf.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        6 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/faq.md
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.927277 pyqbench-0.1.2/docs/source/img/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    21927 2023-01-03 13:43:49.000000 pyqbench-0.1.2/docs/source/img/direct_sum.svg
+-rw-r--r--   0 dexter    (1000) dexter    (1000)   132519 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/img/hadamard_u_v0.svg
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    18590 2023-01-03 13:27:52.000000 pyqbench-0.1.2/docs/source/img/postselection_no_channels.svg
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    18510 2023-01-03 13:00:57.000000 pyqbench-0.1.2/docs/source/img/theoretical_scheme.svg
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    12569 2023-01-03 12:51:37.000000 pyqbench-0.1.2/docs/source/img/vonneumann.svg
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1085 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/index.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3303 2023-02-05 16:27:51.000000 pyqbench-0.1.2/docs/source/installing.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     7949 2023-01-03 14:20:20.000000 pyqbench-0.1.2/docs/source/mathematical_foundations.md
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.927277 pyqbench-0.1.2/docs/source/notebooks/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    37170 2023-02-05 12:27:30.000000 pyqbench-0.1.2/docs/source/notebooks/Example 01 discriminating measurements in Hadamard basis.ipynb
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.927277 pyqbench-0.1.2/docs/source/reference/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       93 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/batching.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       83 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/cli.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      103 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/common_models.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      133 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/reference/fourier.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      140 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/reference/index.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       85 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/jobs.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       89 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/limits.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       91 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/logging.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      267 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/reference/schemes.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       91 2023-01-03 10:47:11.000000 pyqbench-0.1.2/docs/source/reference/testing.md
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      542 2023-01-03 14:26:01.000000 pyqbench-0.1.2/docs/source/references.bib
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      621 2023-02-05 12:25:30.000000 pyqbench-0.1.2/docs/source/tutorial.md
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.928277 pyqbench-0.1.2/examples/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      103 2022-09-17 12:11:49.000000 pyqbench-0.1.2/examples/backend-factory-with-run-options.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       73 2022-09-17 12:11:49.000000 pyqbench-0.1.2/examples/backend-factory.yml
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.929277 pyqbench-0.1.2/examples/backends/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       98 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/backends/ibmq-qasm-simulator-async.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       99 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/backends/ibmq-qasm-simulator-sync.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       89 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/backends/ibmq-quito.yml
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.929277 pyqbench-0.1.2/examples/experiments/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      164 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/experiments/fourier-disc-direct-sum-ibmq.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      167 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/experiments/fourier-disc-postselection-ibmq.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1252 2022-10-25 03:46:00.000000 pyqbench-0.1.2/examples/fourier-discrimination-async-result.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      225 2022-09-17 12:11:49.000000 pyqbench-0.1.2/examples/fourier-discrimination-experiment.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3943 2022-10-25 03:46:00.000000 pyqbench-0.1.2/examples/fourier-discrimination-result-with-mitigation.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1519 2022-10-25 03:46:00.000000 pyqbench-0.1.2/examples/fourier-discrimination-result.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       92 2022-09-25 22:53:31.000000 pyqbench-0.1.2/examples/ibmq-backend.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      125 2022-09-17 12:11:49.000000 pyqbench-0.1.2/examples/simple-backend-with-run-options.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       64 2022-09-17 12:11:49.000000 pyqbench-0.1.2/examples/simple-backend.yml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1249 2023-01-04 17:40:32.000000 pyqbench-0.1.2/examples/using_fourier_with_simulator.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1265 2023-01-04 17:40:32.000000 pyqbench-0.1.2/examples/using_fourier_with_simulator_postselection_all_cases.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.929277 pyqbench-0.1.2/mathematics/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    16496 2023-04-25 18:11:08.000000 pyqbench-0.1.2/mathematics/optimal_final_measurement_discrimination.nb
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1844 2023-04-25 18:11:08.000000 pyqbench-0.1.2/pyproject.toml
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      256 2023-04-25 18:11:08.000000 pyqbench-0.1.2/pyqbench.bib
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.929277 pyqbench-0.1.2/pyqbench.egg-info/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4984 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/PKG-INFO
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3324 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/SOURCES.txt
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        1 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/dependency_links.txt
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       43 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/entry_points.txt
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      446 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/requires.txt
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       58 2023-04-25 19:20:55.000000 pyqbench-0.1.2/pyqbench.egg-info/top_level.txt
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.930277 pyqbench-0.1.2/qbench/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-06-14 21:57:00.000000 pyqbench-0.1.2/qbench/__init__.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1367 2022-09-29 17:11:10.000000 pyqbench-0.1.2/qbench/_expressions.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3199 2023-04-25 18:11:08.000000 pyqbench-0.1.2/qbench/batching.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      548 2023-04-25 19:20:49.000000 pyqbench-0.1.2/qbench/cli.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4785 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/common_models.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.930277 pyqbench-0.1.2/qbench/fourier/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1720 2023-04-25 19:20:49.000000 pyqbench-0.1.2/qbench/fourier/__init__.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     6094 2023-04-25 19:20:49.000000 pyqbench-0.1.2/qbench/fourier/_cli.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.931277 pyqbench-0.1.2/qbench/fourier/_components/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4850 2023-04-25 18:11:08.000000 pyqbench-0.1.2/qbench/fourier/_components/__init__.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1445 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_components/_generic.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      999 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_components/_ibmq.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1003 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_components/_lucy.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1118 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_components/_lucy_and_ibmq_common.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2729 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_components/_rigetti.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2570 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/_models.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    14376 2023-04-25 19:20:49.000000 pyqbench-0.1.2/qbench/fourier/experiment_runner.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2221 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/fourier/testing.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      899 2023-04-25 19:18:47.000000 pyqbench-0.1.2/qbench/jobs.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1911 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/limits.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1298 2022-09-29 17:11:10.000000 pyqbench-0.1.2/qbench/logging.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.931277 pyqbench-0.1.2/qbench/schemes/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/schemes/__init__.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      828 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/schemes/_utils.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     5315 2023-01-03 10:47:11.000000 pyqbench-0.1.2/qbench/schemes/direct_sum.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     6348 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/schemes/postselection.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4151 2022-10-25 03:46:00.000000 pyqbench-0.1.2/qbench/testing.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)       38 2023-04-25 19:20:55.933277 pyqbench-0.1.2/setup.cfg
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.932277 pyqbench-0.1.2/tests/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)        0 2022-06-14 21:57:00.000000 pyqbench-0.1.2/tests/__init__.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      799 2022-09-28 12:57:43.000000 pyqbench-0.1.2/tests/conftest.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.932277 pyqbench-0.1.2/tests/fourier/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     4176 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     5976 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier_cli.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3450 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier_experiment_runner.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1543 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier_ibmq.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1581 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier_lucy.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1633 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/fourier/test_fourier_rigetti.py
+drwxr-xr-x   0 dexter    (1000) dexter    (1000)        0 2023-04-25 19:20:55.932277 pyqbench-0.1.2/tests/schemes/
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      838 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/schemes/test_direct_sum.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)      851 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/schemes/test_postselection.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     3540 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/test_batching.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1540 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/test_ibmq_backend.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     2809 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/test_limits.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)     1208 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/test_mock_simulator.py
+-rw-r--r--   0 dexter    (1000) dexter    (1000)    10097 2023-01-04 17:40:32.000000 pyqbench-0.1.2/tests/test_models.py
```

### Comparing `pyqbench-0.1.1/.github/workflows/quality_checks.yml` & `pyqbench-0.1.2/.github/workflows/quality_checks.yml`

 * *Files 18% similar despite different names*

```diff
@@ -21,26 +21,31 @@
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies and the package
         run: |
           python -m pip install --upgrade pip
           pip install .[test]
       - name: Run unit tests
         run: pytest --cov=qbench --cov-report=xml
+      - name: Upload coverage reports to Codecov
+        uses: codecov/codecov-action@v3
 
   run_quality_cheks:
     runs-on: ubuntu-latest
     steps:
       - name: Set up Python
         uses: actions/setup-python@v2
         with:
           python-version: 3.9
       - uses: actions/checkout@v2
       - name: Install dependencies and the package
         run: |
           python -m pip install --upgrade pip
           pip install .[test,dev]
-      - name: Quality checks
-        run: |          
-          mypy --ignore-missing-imports --install-types --non-interactive tests qbench
-          flake8 --max-line-length=100 qbench
-          black --check .
-          isort --check-only --profile black qbench -c --diff
+      - name: Run pre-commit hook checks
+        run: |
+          pip install pre-commit
+          pre-commit install
+          pre-commit run -a
+      - name: Run mypy
+        run: |
+          pip install types-PyYAML
+          mypy --namespace-packages --ignore-missing-imports --explicit-package-bases qbench
```

### Comparing `pyqbench-0.1.1/.gitignore` & `pyqbench-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/Hadamard example.ipynb` & `pyqbench-0.1.2/Hadamard example.ipynb`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/LICENSE` & `pyqbench-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/adr/async_backends.md` & `pyqbench-0.1.2/adr/async_backends.md`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/adr/backend_factory_model.md` & `pyqbench-0.1.2/adr/backend_factory_model.md`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/adr/fourier-discrimination-cli.md` & `pyqbench-0.1.2/adr/fourier-discrimination-cli.md`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/adr/general_form_of_the_cli.md` & `pyqbench-0.1.2/adr/general_form_of_the_cli.md`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/adr/simple_backend_model.md` & `pyqbench-0.1.2/adr/simple_backend_model.md`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/docs/Makefile` & `pyqbench-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/docs/make.bat` & `pyqbench-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/docs/source/img/hadamard_u_v0.svg` & `pyqbench-0.1.2/docs/source/img/hadamard_u_v0.svg`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/docs/source/installing.md` & `pyqbench-0.1.2/docs/source/installing.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+(section/installation)=
+
 # Installing
 
 ## Basic installation
 
 The most up-to-date version of PyQBench can be installed from PyPI:
 
 ```shell
@@ -67,15 +69,15 @@
 
 This section discusses dependencies used by PyQBench and their role in the project. Please note
 that transitive dependencies are not included in the list.
 
 ### Mandatory dependencies
 
 - `qiskit`: used for constructing quantum circuits and interfacing with quantum devices
-- `amaozn-braket-sdk` and `qiskit-braket-provider`: used for interacting with Amazon Braket devices
+- `amazon-braket-sdk` and `qiskit-braket-provider`: used for interacting with Amazon Braket devices
 - `mthree`: used for readout error mitigation
 - `numpy` and `scipy`: basic libraries for numerical calculations
 - `tqdm`: used for rendering progress bars in CLI
 - `pyaml` and `pydantic`: for reading/writing input/output files in the CLI, and validating their
   contents
 - `pandas`: used for outputting final CSV file with discrimination probabilities
```

### Comparing `pyqbench-0.1.1/docs/source/notebooks/Example 01 discriminating measurements in Hadamard basis.ipynb` & `pyqbench-0.1.2/docs/source/notebooks/Example 01 discriminating measurements in Hadamard basis.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999281609195403%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(0, 'from qiskit.providers.aer import noise\\n')], delete: "*

 * *            '[0]}}}'}*

```diff
@@ -564,15 +564,15 @@
                     },
                     "execution_count": 85,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "from qiskit_aer import noise\n",
+                "from qiskit.providers.aer import noise\n",
                 "\n",
                 "error = noise.ReadoutError([[0.75, 0.25], [0.8, 0.2]])\n",
                 "\n",
                 "noise_model = noise.NoiseModel()\n",
                 "noise_model.add_readout_error(error, [0])\n",
                 "noise_model.add_readout_error(error, [1])\n",
                 "\n",
```

### Comparing `pyqbench-0.1.1/docs/source/tutorial.md` & `pyqbench-0.1.2/docs/source/tutorial.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+(section/tutorial)=
+
 # User guide
 
 PyQBench can be used in two different ways:
 
 - As a library. This is a more extensible, but also more laborious way of using PyQBench.
   Most importantly, this way allows for more advanced scripting defining your own measurements
   scheme.
```

### Comparing `pyqbench-0.1.1/examples/fourier-discrimination-async-result.yml` & `pyqbench-0.1.2/examples/fourier-discrimination-async-result.yml`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/examples/fourier-discrimination-result-with-mitigation.yml` & `pyqbench-0.1.2/examples/fourier-discrimination-result-with-mitigation.yml`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/examples/fourier-discrimination-result.yml` & `pyqbench-0.1.2/examples/fourier-discrimination-result.yml`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/examples/using_fourier_with_simulator.py` & `pyqbench-0.1.2/examples/using_fourier_with_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/examples/using_fourier_with_simulator_postselection_all_cases.py` & `pyqbench-0.1.2/examples/using_fourier_with_simulator_postselection_all_cases.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/pyproject.toml` & `pyqbench-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,35 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
     "numpy ~= 1.22.0",
     "scipy ~= 1.7.0",
     "pandas ~= 1.5.0",
     "amazon-braket-sdk >= 1.11.1",
-    "pydantic ~= 1.9.1",
+    "pydantic > 1.9.1",
     "qiskit ~= 0.37.2",
     "mthree ~= 1.1.0",
     "tqdm ~= 4.64.1",
     "pyyaml ~= 6.0",
     "qiskit-braket-provider ~= 0.0.3"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest>=6.1.2", "pytest-mock>=3.3.1", "pytest-cov>=2.12.1"]
-dev = ["flake8>=4.0.1", "black>=21.12b0", "isort>=5.10.1", "mypy>=0.961"]
-docs = ["sphinx>=5.3.0", "pydata-sphinx-theme>=0.11.0", "sphinx_math_dollar>=1.2.1", "myst_nb~=0.17.1", "iplantuml~=0.1.1"]
+dev = ["flake8>=4.0.1", "black>=21.12b0", "isort>=5.10.1", "mypy>=0.982"]
+docs = [
+    "sphinx>=5.3.0",
+    "pydata-sphinx-theme>=0.11.0",
+    "sphinx_math_dollar>=1.2.1",
+    "myst_nb~=0.17.1",
+    "iplantuml~=0.1.1",
+    "sphinxcontrib-bibtex~=2.5.0",
+    "sphinx-design~=0.3.0"
+]
 
 [project.scripts]
 qbench = "qbench.cli:main"
 
 [project.urls]
 "Source Code" = "https://github.com/iitis/PyQBench"
```

### Comparing `pyqbench-0.1.1/pyqbench.egg-info/SOURCES.txt` & `pyqbench-0.1.2/pyqbench.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 .flake8
 .git_archival.txt
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 Hadamard example.ipynb
 LICENSE
 README.md
 pyproject.toml
+pyqbench.bib
 .github/workflows/quality_checks.yml
 adr/async_backends.md
 adr/backend_factory_model.md
 adr/fourier-discrimination-cli.md
 adr/general_form_of_the_cli.md
 adr/simple_backend_model.md
 docs/Makefile
@@ -18,17 +20,23 @@
 docs/source/citing.md
 docs/source/cli_usage.md
 docs/source/conf.py
 docs/source/faq.md
 docs/source/index.md
 docs/source/installing.md
 docs/source/mathematical_foundations.md
+docs/source/references.bib
 docs/source/tutorial.md
+docs/source/_static/logo.png
 docs/source/_static/css/custom.css
+docs/source/img/direct_sum.svg
 docs/source/img/hadamard_u_v0.svg
+docs/source/img/postselection_no_channels.svg
+docs/source/img/theoretical_scheme.svg
+docs/source/img/vonneumann.svg
 docs/source/notebooks/Example 01 discriminating measurements in Hadamard basis.ipynb
 docs/source/reference/batching.md
 docs/source/reference/cli.md
 docs/source/reference/common_models.md
 docs/source/reference/fourier.md
 docs/source/reference/index.md
 docs/source/reference/jobs.md
@@ -48,14 +56,15 @@
 examples/using_fourier_with_simulator.py
 examples/using_fourier_with_simulator_postselection_all_cases.py
 examples/backends/ibmq-qasm-simulator-async.yml
 examples/backends/ibmq-qasm-simulator-sync.yml
 examples/backends/ibmq-quito.yml
 examples/experiments/fourier-disc-direct-sum-ibmq.yml
 examples/experiments/fourier-disc-postselection-ibmq.yml
+mathematics/optimal_final_measurement_discrimination.nb
 pyqbench.egg-info/PKG-INFO
 pyqbench.egg-info/SOURCES.txt
 pyqbench.egg-info/dependency_links.txt
 pyqbench.egg-info/entry_points.txt
 pyqbench.egg-info/requires.txt
 pyqbench.egg-info/top_level.txt
 qbench/__init__.py
```

### Comparing `pyqbench-0.1.1/qbench/_expressions.py` & `pyqbench-0.1.2/qbench/_expressions.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/batching.py` & `pyqbench-0.1.2/qbench/batching.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 def execute_in_batches(
     backend: Backend,
     circuits: Sequence[QuantumCircuit],
     keys: Sequence[Any],
     shots: int,
     batch_size: Optional[int],
     show_progress: bool = False,
-    **kwargs
+    **kwargs,
 ) -> Iterable[BatchJob]:
     """Execute given sequence of circuits with corresponding keys in batches on a backend.
 
     :param backend: backend which will be usd for executing circuits.
     :param circuits: sequence of circuits to be executed.
     :param keys: sequence of keys corresponding to the circuits.
     :param shots: number of shots for each circuit.
```

### Comparing `pyqbench-0.1.1/qbench/cli.py` & `pyqbench-0.1.2/qbench/cli.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/common_models.py` & `pyqbench-0.1.2/qbench/common_models.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/__init__.py` & `pyqbench-0.1.2/qbench/fourier/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,30 @@
 """Functionalities relating specifically to Fourier-discrimination experiments.
 
-This module contains the following:
 
-- Components (in the form of Qiskit Instructions) needed for performing postselection
-  or direct sum experiment using Fourier parametrized family.
-- Utility function computing upper bound on probability of correct discrimination.
+This package defines all instructions (components) needed for assembling
+circuits for benchmarking using Fourier-parametrized family.
+
+The Fourier family of measurements is defined as:
+
+$$
+U(\\varphi) = H \\begin{pmatrix} 1&0\\\\0&e^{i\\varphi}\\end{pmatrix}H^\\dagger
+$$
+
+All components are available as properties of :class:`FourierComponents` class. The
+instances of this class can be constructed in such a way that the instructions they
+provide are compatible with several different quantum devices available on the market.
+
+Additionally, this module provides a function computing optimal discrimination probability
+for Fourier family of measurements, which is defined as:
+
+$$
+p_{U(\\varphi)} = \\frac12 + \\frac14 \\lvert 1 - e^{i \\varphi}\\rvert.
+$$
+
 """
 from typing import Union
 
 import numpy as np
 
 from ._cli import add_fourier_parser
 from ._components import FourierComponents
@@ -21,15 +37,15 @@
 
 def discrimination_probability_upper_bound(
     phi: Union[float, np.ndarray]
 ) -> Union[float, np.ndarray]:
     """Compute exact upper bound on the probability of discrimination.
 
     :param phi: angle parametrizing the performed measurement.
-    :return: maximum probability with which identity and P_U(phi) can be discriminated.
+    :return: maximum probability with which identity and $p_{U(\\varphi)}$ can be discriminated.
     """
     return 0.5 + 0.25 * np.abs(1 - np.exp(1j * phi))
 
 
 __all__ = [
     "discrimination_probability_upper_bound",
     "add_fourier_parser",
```

### Comparing `pyqbench-0.1.1/qbench/fourier/_cli.py` & `pyqbench-0.1.2/qbench/fourier/_cli.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/__init__.py` & `pyqbench-0.1.2/qbench/fourier/_components/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,40 @@
 
 from . import _generic, _ibmq, _lucy, _rigetti
 
 
 class FourierComponents:
     """Class defining components for Fourier-discrimination experiment.
 
-    :param phi: Fourier angle of measurement to discriminate. May be a qiskit Parameter.
-    :param gateset: one of the predefined basis gate sets to use:
-      ["lucy", "rigetti", "ibmq"]. If not provided, high-level definitions of gates
-      will be used without restrictions on basis gates.
+    :param phi: angle defining measurement to discriminate. May be a number or an instance of
+      a Qiskit Parameter. See
+      :qiskit_tutorial:`here <circuits_advanced/01_advanced_circuits.html#Parameterized-circuits>`_
+      if you are new to parametrized circuits in Qiskit.
+
+    :param gateset: name of the one of the predefined basis gate sets to use. It controls which
+      gates will be used to construct the circuit components. Available choices are:
+
+      - :code:`"lucy"`: gateset comprising gates native to
+        `OQC Lucy <https://aws.amazon.com/braket/quantum-computers/oqc/>`_ computer.
+      - :code:`"rigetti"`: gateset comprising gates native to
+        `Rigetti <https://www.rigetti.com/>`_ computers.
+      - :code:`"ibmq"`: gateset comprising gates native to
+        `IBMQ <https://quantum-computing.ibm.com/lab>`_ computers.
+
+      If no gateset is provided, high-level gates will be used without restriction on basis gates.
     """
 
     def __init__(self, phi: Union[float, Parameter], gateset: Optional[str] = None):
         """Initialize new instance of FourierComponents."""
         self.phi = phi
         self._module = _GATESET_MAPPING[gateset]
 
     @property
     def state_preparation(self) -> Instruction:
-        """Instruction performing state preparation |00> -> bell state
+        """Instruction performing transformation $|00\\rangle$ -> Bell state
 
         The corresponding circuit is:
 
         .. code::
 
                    ┌───┐
               q_0: ┤ H ├──■──
@@ -35,23 +47,23 @@
                         └───┘
 
         """
         return self._module.state_preparation()
 
     @property
     def u_dag(self) -> Instruction:
-        r"""Unitary $U^\dagger$ defining alternative measurement.
+        r"""Unitary $U^\dagger$ defining Fourier measurement.
 
         The corresponding circuit is:
 
         .. code::
 
-                 ┌───┐┌─────────────┐┌───┐
-              q: ┤ H ├┤ Phase(-phi) ├┤ H ├
-                 └───┘└─────────────┘└───┘
+                 ┌───┐┌───────────┐┌───┐
+              q: ┤ H ├┤ Phase(-φ) ├┤ H ├
+                 └───┘└───────────┘└───┘
 
         .. note::
 
            This instruction is needed because on actual devices we can only measure in Z-basis.
            The $U^\dagger$ unitary changes basis so that subsequent measurement in Z-basis can
            be considered as performing desired von Neumann measurement to be discriminated from
            the Z-basis one.
@@ -63,38 +75,38 @@
     def v0_dag(self) -> Instruction:
         """Instruction corresponding to the positive part of Holevo-Helstrom measurement.
 
         The corresponding circuit is:
 
         .. code::
 
-                 ┌──────────┐┌──────────────────┐
-              q: ┤ Rz(-π/2) ├┤ Ry(-phi/2 - π/2) ├
-                 └──────────┘└──────────────────┘
+                 ┌──────────┐┌────────────────┐
+              q: ┤ Rz(-π/2) ├┤ Ry(-φ/2 - π/2) ├
+                 └──────────┘└────────────────┘
 
         """
         return self._module.v0_dag(self.phi)
 
     @property
     def v1_dag(self) -> Instruction:
         """Instruction corresponding to the negative part of Holevo-Helstrom measurement.
 
         The corresponding circuit is:
 
         .. code::
 
-                 ┌──────────┐┌──────────────────┐┌────────┐
-              q: ┤ Rz(-π/2) ├┤ Ry(-phi/2 - π/2) ├┤ Rx(-π) ├
-                 └──────────┘└──────────────────┘└────────┘
+                 ┌──────────┐┌────────────────┐┌────────┐
+              q: ┤ Rz(-π/2) ├┤ Ry(-φ/2 - π/2) ├┤ Rx(-π) ├
+                 └──────────┘└────────────────┘└────────┘
         """
         return self._module.v1_dag(self.phi)
 
     @property
     def v0_v1_direct_sum_dag(self) -> Instruction:
-        r"""Direct sum $V_0^\dagger\oplusV_1^\dagger$ of both parts of Holevo-Helstrom measurement.
+        r"""Direct sum $V_0^\dagger\oplus V_1^\dagger$ of both parts of Holevo-Helstrom measurement.
 
         .. note::
            In usual basis ordering, the unitaries returned by this property would be
            block-diagonal, with blocks corresponding to positive and negative parts
            of Holevo-Helstrom measurement.
 
            However, Qiskit enumerates basis vectors in reverse, so the produced unitaries
```

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/_generic.py` & `pyqbench-0.1.2/qbench/fourier/_components/_generic.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/_ibmq.py` & `pyqbench-0.1.2/qbench/fourier/_components/_ibmq.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/_lucy.py` & `pyqbench-0.1.2/qbench/fourier/_components/_lucy.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/_lucy_and_ibmq_common.py` & `pyqbench-0.1.2/qbench/fourier/_components/_lucy_and_ibmq_common.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_components/_rigetti.py` & `pyqbench-0.1.2/qbench/fourier/_components/_rigetti.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/_models.py` & `pyqbench-0.1.2/qbench/fourier/_models.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/experiment_runner.py` & `pyqbench-0.1.2/qbench/fourier/experiment_runner.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/fourier/testing.py` & `pyqbench-0.1.2/qbench/fourier/testing.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/jobs.py` & `pyqbench-0.1.2/qbench/jobs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Implementation of utilities for interacting with jobs."""
 from functools import singledispatch
 from typing import Sequence
 
 from qiskit.providers import JobV1
-from qiskit.providers.ibmq import IBMQBackend, IBMQJob
+
+# from qiskit.providers.ibmq import IBMQBackend, IBMQJob
 
 
 @singledispatch
 def retrieve_jobs(backend, job_ids: Sequence[str]) -> Sequence[JobV1]:
     """Retrieve jobs with given ids from a backend.
 
     :param backend: backend which was used to run the jobs.
     :param job_ids: identifiers of jobs to obtain.
     :return: sequence of jobs. Note that it is not guaranteed that the order of this sequence
      will match order of ids in job_ids parameter.
     """
     return [backend.retrieve_job(job_id) for job_id in job_ids]
 
 
-@retrieve_jobs.register
-def _retrieve_jobs_from_ibmq(backend: IBMQBackend, job_ids: Sequence[str]) -> Sequence[IBMQJob]:
-    return backend.jobs(db_filter={"id": {"inq": job_ids}}, limit=len(job_ids))
+# @retrieve_jobs.register
+# def _retrieve_jobs_from_ibmq(backend: IBMQBackend, job_ids: Sequence[str]) -> Sequence[IBMQJob]:
+#     return backend.jobs(db_filter={"id": {"inq": job_ids}}, limit=len(job_ids))
```

### Comparing `pyqbench-0.1.1/qbench/limits.py` & `pyqbench-0.1.2/qbench/limits.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/logging.py` & `pyqbench-0.1.2/qbench/logging.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/schemes/_utils.py` & `pyqbench-0.1.2/qbench/schemes/_utils.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/schemes/direct_sum.py` & `pyqbench-0.1.2/qbench/schemes/direct_sum.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/schemes/postselection.py` & `pyqbench-0.1.2/qbench/schemes/postselection.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/qbench/testing.py` & `pyqbench-0.1.2/qbench/testing.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/conftest.py` & `pyqbench-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier.py` & `pyqbench-0.1.2/tests/fourier/test_fourier.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier_cli.py` & `pyqbench-0.1.2/tests/fourier/test_fourier_cli.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier_experiment_runner.py` & `pyqbench-0.1.2/tests/fourier/test_fourier_experiment_runner.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier_ibmq.py` & `pyqbench-0.1.2/tests/fourier/test_fourier_ibmq.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier_lucy.py` & `pyqbench-0.1.2/tests/fourier/test_fourier_lucy.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/fourier/test_fourier_rigetti.py` & `pyqbench-0.1.2/tests/fourier/test_fourier_rigetti.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/schemes/test_direct_sum.py` & `pyqbench-0.1.2/tests/schemes/test_direct_sum.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/schemes/test_postselection.py` & `pyqbench-0.1.2/tests/schemes/test_postselection.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/test_batching.py` & `pyqbench-0.1.2/tests/test_batching.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/test_ibmq_backend.py` & `pyqbench-0.1.2/tests/test_ibmq_backend.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/test_limits.py` & `pyqbench-0.1.2/tests/test_limits.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/test_mock_simulator.py` & `pyqbench-0.1.2/tests/test_mock_simulator.py`

 * *Files identical despite different names*

### Comparing `pyqbench-0.1.1/tests/test_models.py` & `pyqbench-0.1.2/tests/test_models.py`

 * *Files identical despite different names*

