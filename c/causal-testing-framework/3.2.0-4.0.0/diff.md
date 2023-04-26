# Comparing `tmp/causal_testing_framework-3.2.0.tar.gz` & `tmp/causal_testing_framework-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causal_testing_framework-3.2.0.tar", last modified: Tue Apr 11 10:17:13 2023, max compression
+gzip compressed data, was "causal_testing_framework-4.0.0.tar", last modified: Wed Apr 26 09:59:05 2023, max compression
```

## Comparing `causal_testing_framework-3.2.0.tar` & `causal_testing_framework-4.0.0.tar`

### file list

```diff
@@ -1,156 +1,157 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.756882 causal_testing_framework-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/lint-format.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.github/workflows/publish-to-pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.mega-linter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/data_collection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/data_collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/data_collection/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/generation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12746 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/generation/abstract_causal_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/json_front/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/json_front/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14630 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/json_front/json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.760882 causal_testing_framework-3.2.0/causal_testing/specification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26479 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/causal_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/metamorphic_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/specification/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/causal_testing/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/base_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    30688 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/causal_testing/testing/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 10:17:13.000000 causal_testing_framework-3.2.0/causal_testing_framework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.764882 causal_testing_framework-3.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/description.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/frontends/json_front_end.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/frontends/test_suite.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/glossary.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/docs/source/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/causal_specification.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/causal_tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/modules/data_collector.rst
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/docs/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/examples/covasim_/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.768882 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/example_beta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.png
--rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/lr91/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.772882 causal_testing_framework-3.2.0/examples/lr91/data/
--rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/data/normalised_results.csv
--rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/data/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/example_max_conductances.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/lr91/example_max_conductances_test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/causal_tests.json
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson/example_run_causal_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/dag.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/
--rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/data_random_1000.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.776882 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/
--rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9131 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/examples/poisson-line-process/example_poisson_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/images/
--rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/images/workflow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/data/nhefs.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/data_collection_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/data_collection_tests/test_observational_data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/generation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9111 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/generation_tests/test_abstract_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.780882 causal_testing_framework-3.2.0/tests/json_front_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/json_front_tests/test_json_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.752882 causal_testing_framework-3.2.0/tests/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/resources/data/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/dag.dot
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/data_with_meta.csv
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/resources/data/tests.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/specification_tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_causal_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_metamorphic_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/specification_tests/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:17:13.784882 causal_testing_framework-3.2.0/tests/testing_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_outcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-04-11 10:15:52.000000 causal_testing_framework-3.2.0/tests/testing_tests/test_estimators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/workflows/lint-format.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.github/workflows/publish-to-pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.mega-linter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20375 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/causal_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/causal_testing/data_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/data_collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/data_collection/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/causal_testing/generation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/generation/abstract_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/generation/enum_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/causal_testing/json_front/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/json_front/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19122 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/json_front/json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.560511 causal_testing_framework-4.0.0/causal_testing/specification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26803 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/causal_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/metamorphic_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/specification/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/causal_testing/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/base_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13663 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/causal_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30782 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/causal_testing/testing/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-26 09:59:05.000000 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-26 09:59:05.000000 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:59:05.000000 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 09:59:05.000000 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 09:59:05.000000 causal_testing_framework-4.0.0/causal_testing_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/description.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/docs/source/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/frontends/json_front_end.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/frontends/test_suite.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/glossary.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/docs/source/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/modules/causal_specification.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/modules/causal_tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/modules/data_collector.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.564511 causal_testing_framework-4.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.556511 causal_testing_framework-4.0.0/examples/covasim_/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.568512 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    24596 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.568512 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1355776 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15718 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/example_beta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.568512 causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/dag.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11845 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/example_vaccine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.568512 causal_testing_framework-4.0.0/examples/lr91/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    73886 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.568512 causal_testing_framework-4.0.0/examples/lr91/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    40715 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/data/normalised_results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40686 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/data/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/example_max_conductances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/lr91/example_max_conductances_test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/examples/poisson/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson/causal_tests.json
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    61017 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson/example_run_causal_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/examples/poisson-line-process/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)    53765 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/dag.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.556511 causal_testing_framework-4.0.0/examples/poisson-line-process/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/examples/poisson-line-process/data/random/
+-rw-r--r--   0 runner    (1001) docker     (123)   102007 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/random/data_random_1000.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12100 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24851 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14925 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13682 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26544 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17103 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26889 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/examples/poisson-line-process/example_poisson_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   184134 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/images/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.572512 causal_testing_framework-4.0.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   374288 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/data/nhefs.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/data_collection_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/data_collection_tests/test_observational_data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/generation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/generation_tests/test_abstract_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/json_front_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10798 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/json_front_tests/test_json_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.556511 causal_testing_framework-4.0.0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/resources/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/resources/data/dag.dot
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/resources/data/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/resources/data/data_with_meta.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/resources/data/tests.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/specification_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/specification_tests/test_causal_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/specification_tests/test_metamorphic_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/specification_tests/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:59:05.576511 causal_testing_framework-4.0.0/tests/testing_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13873 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18696 2023-04-26 09:58:16.000000 causal_testing_framework-4.0.0/tests/testing_tests/test_estimators.py
```

### Comparing `causal_testing_framework-3.2.0/.github/CONTRIBUTING.md` & `causal_testing_framework-4.0.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `causal_testing_framework-4.0.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `causal_testing_framework-4.0.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.github/workflows/ci-tests.yaml` & `causal_testing_framework-4.0.0/.github/workflows/ci-tests.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.github/workflows/lint-format.yaml` & `causal_testing_framework-4.0.0/.github/workflows/lint-format.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.github/workflows/publish-to-pypi.yaml` & `causal_testing_framework-4.0.0/.github/workflows/publish-to-pypi.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.gitignore` & `causal_testing_framework-4.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.pylintrc` & `causal_testing_framework-4.0.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/.readthedocs.yaml` & `causal_testing_framework-4.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/LICENSE` & `causal_testing_framework-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/PKG-INFO` & `causal_testing_framework-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal_testing_framework
-Version: 3.2.0
+Version: 4.0.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-3.2.0/README.md` & `causal_testing_framework-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/data_collection/data_collector.py` & `causal_testing_framework-4.0.0/causal_testing/data_collection/data_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         for _, row in data.iterrows():
             solver.push()
             # Need to explicitly cast variables to their specified type. Z3 will not take e.g. np.int64 to be an int.
             model = [
                 self.scenario.variables[var].z3
                 == self.scenario.variables[var].z3_val(self.scenario.variables[var].z3, row[var])
                 for var in self.scenario.variables
-                if var in row
+                if var in row and not pd.isnull(row[var])
             ]
             for c in model:
                 solver.assert_and_track(c, f"model: {c}")
             check = solver.check()
             if check == z3.unsat and unsat_core is None:
                 unsat_core = solver.unsat_core()
             sat.append(check == z3.sat)
@@ -143,13 +143,14 @@
         Data is invalid if it does not meet the constraints outlined in the scenario-under-test (Scenario).
 
         :return: A pandas dataframe containing execution data that is valid for the scenario-under-test.
         """
 
         execution_data_df = self.data
         for meta in self.scenario.metas():
-            meta.populate(execution_data_df)
+            if meta.name not in self.data:
+                meta.populate(execution_data_df)
         scenario_execution_data_df = self.filter_valid_data(execution_data_df)
         for var_name, var in self.scenario.variables.items():
             if issubclass(var.datatype, Enum):
                 scenario_execution_data_df[var_name] = [var.datatype(x) for x in scenario_execution_data_df[var_name]]
         return scenario_execution_data_df
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/generation/abstract_causal_test_case.py` & `causal_testing_framework-4.0.0/causal_testing/generation/abstract_causal_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
                 ),
                 expected_causal_effect=list(self.expected_causal_effect.values())[0],
                 estimate_type=self.estimate_type,
                 effect_modifier_configuration={v: v.cast(model[v.z3]) for v in self.effect_modifiers},
             )
 
             for v in self.scenario.inputs():
-                if row[v.name] != v.cast(model[v.z3]):
+                if v.name in row and row[v.name] != v.cast(model[v.z3]):
                     constraints = "\n  ".join([str(c) for c in self.scenario.constraints if v.name in str(c)])
                     logger.warning(
                         f"Unable to set variable {v.name} to {row[v.name]} because of constraints\n"
                         + f"{constraints}\nUsing value {v.cast(model[v.z3])} instead in test\n{concrete_test}"
                     )
 
             if not any((vars(t) == vars(concrete_test) for t in concrete_tests)):
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/json_front/json_class.py` & `causal_testing_framework-4.0.0/causal_testing/json_front/json_class.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains the JsonUtility class, details of using this class can be found here:
 https://causal-testing-framework.readthedocs.io/en/latest/json_front_end.html"""
 
 import argparse
 import json
 import logging
 
+from collections.abc import Iterable, Mapping
 from dataclasses import dataclass
 from pathlib import Path
 from statistics import StatisticsError
 
 import pandas as pd
 import scipy
 from fitter import Fitter, get_common_distributions
@@ -18,14 +19,15 @@
 from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.specification.causal_specification import CausalSpecification
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.variable import Input, Meta, Output
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_engine import CausalTestEngine
 from causal_testing.testing.estimators import Estimator
+from causal_testing.testing.base_test_case import BaseTestCase
 
 logger = logging.getLogger(__name__)
 
 
 class JsonUtility:
     """
     The JsonUtility Class provides the functionality to use structured JSON to setup and run causal tests on the
@@ -35,21 +37,21 @@
     :attr {Path} dag_path: Path to the dag.dot file containing the Causal DAG.
     :attr {Path} data_path: Path to the csv data file.
     :attr {Input} inputs: Causal variables representing inputs.
     :attr {Output} outputs: Causal variables representing outputs.
     :attr {Meta} metas: Causal variables representing metavariables.
     :attr {pd.DataFrame}: Pandas DataFrame containing runtime data.
     :attr {dict} test_plan: Dictionary containing the key value pairs from the loaded json test plan.
-    :attr {Scenario} modelling_scenario:
+    :attr {Scenario} scenario:
     :attr {CausalSpecification} causal_specification:
     """
 
     def __init__(self, output_path: str, output_overwrite: bool = False):
         self.input_paths = None
-        self.variables = None
+        self.variables = {"inputs": {}, "outputs": {}, "metas": {}}
         self.data = []
         self.test_plan = None
         self.scenario = None
         self.causal_specification = None
         self.output_path = Path(output_path)
         self.check_file_exists(self.output_path, output_overwrite)
 
@@ -61,69 +63,139 @@
         :param data_paths: string path representation to the data files
         """
         self.input_paths = JsonClassPaths(json_path=json_path, dag_path=dag_path, data_paths=data_paths)
 
     def setup(self, scenario: Scenario):
         """Function to populate all the necessary parts of the json_class needed to execute tests"""
         self.scenario = scenario
+        self._get_scenario_variables()
         self.scenario.setup_treatment_variables()
         self.causal_specification = CausalSpecification(
             scenario=self.scenario, causal_dag=CausalDAG(self.input_paths.dag_path)
         )
         self._json_parse()
         self._populate_metas()
 
     def _create_abstract_test_case(self, test, mutates, effects):
         assert len(test["mutations"]) == 1
+        treatment_var = next(self.scenario.variables[v] for v in test["mutations"])
+        if not treatment_var.distribution:
+            fitter = Fitter(self.data[treatment_var.name], distributions=get_common_distributions())
+            fitter.fit()
+            (dist, params) = list(fitter.get_best(method="sumsquare_error").items())[0]
+            treatment_var.distribution = getattr(scipy.stats, dist)(**params)
+            self._append_to_file(treatment_var.name + f" {dist}({params})", logging.INFO)
+
         abstract_test = AbstractCausalTestCase(
             scenario=self.scenario,
             intervention_constraints=[mutates[v](k) for k, v in test["mutations"].items()],
-            treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
+            treatment_variable=treatment_var,
             expected_causal_effect={
                 self.scenario.variables[variable]: effects[effect]
-                for variable, effect in test["expectedEffect"].items()
+                for variable, effect in test["expected_effect"].items()
             },
             effect_modifiers={self.scenario.variables[v] for v in test["effect_modifiers"]}
             if "effect_modifiers" in test
             else {},
             estimate_type=test["estimate_type"],
             effect=test.get("effect", "total"),
         )
         return abstract_test
 
-    def generate_tests(self, effects: dict, mutates: dict, estimators: dict, f_flag: bool):
+    def run_json_tests(self, effects: dict, estimators: dict, f_flag: bool = False, mutates: dict = None):
         """Runs and evaluates each test case specified in the JSON input
 
         :param effects: Dictionary mapping effect class instances to string representations.
         :param mutates: Dictionary mapping mutation functions to string representations.
         :param estimators: Dictionary mapping estimator classes to string representations.
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         """
         failures = 0
+        msg = ""
         for test in self.test_plan["tests"]:
             if "skip" in test and test["skip"]:
                 continue
-            abstract_test = self._create_abstract_test_case(test, mutates, effects)
+            test["estimator"] = estimators[test["estimator"]]
+            if "mutations" in test:
+                if test["estimate_type"] == "coefficient":
+                    base_test_case = BaseTestCase(
+                        treatment_variable=next(self.scenario.variables[v] for v in test["mutations"]),
+                        outcome_variable=next(self.scenario.variables[v] for v in test["expected_effect"]),
+                        effect=test.get("effect", "direct"),
+                    )
+                    assert len(test["expected_effect"]) == 1, "Can only have one expected effect."
+                    concrete_tests = [
+                        CausalTestCase(
+                            base_test_case=base_test_case,
+                            expected_causal_effect=next(
+                                effects[effect] for variable, effect in test["expected_effect"].items()
+                            ),
+                            estimate_type="coefficient",
+                            effect_modifier_configuration={
+                                self.scenario.variables[v] for v in test.get("effect_modifiers", [])
+                            },
+                        )
+                    ]
+                    failures = self._execute_tests(concrete_tests, test, f_flag)
+                    msg = (
+                        f"Executing test: {test['name']} \n"
+                        + f"  {concrete_tests[0]} \n"
+                        + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
+                    )
+                else:
+                    abstract_test = self._create_abstract_test_case(test, mutates, effects)
+                    concrete_tests, dummy = abstract_test.generate_concrete_tests(5, 0.05)
+                    failures = self._execute_tests(concrete_tests, test, f_flag)
+
+                    msg = (
+                        f"Executing test: {test['name']} \n"
+                        + "  abstract_test \n"
+                        + f"  {abstract_test} \n"
+                        + f"  {abstract_test.treatment_variable.name},"
+                        + f"  {abstract_test.treatment_variable.distribution} \n"
+                        + f"  Number of concrete tests for test case: {str(len(concrete_tests))} \n"
+                        + f"  {failures}/{len(concrete_tests)} failed for {test['name']}"
+                    )
+                self._append_to_file(msg, logging.INFO)
+            else:
+                outcome_variable = next(
+                    iter(test["expected_effect"])
+                )  # Take first key from dictionary of expected effect
+                base_test_case = BaseTestCase(
+                    treatment_variable=self.variables["inputs"][test["treatment_variable"]],
+                    outcome_variable=self.variables["outputs"][outcome_variable],
+                )
 
-            concrete_tests, dummy = abstract_test.generate_concrete_tests(5, 0.05)
-            failures = self._execute_tests(concrete_tests, estimators, test, f_flag)
-            msg = (
-                f"Executing test: {test['name']} \n"
-                + "abstract_test \n"
-                + f"{abstract_test} \n"
-                + f"{abstract_test.treatment_variable.name},{abstract_test.treatment_variable.distribution} \n"
-                + f"Number of concrete tests for test case: {str(len(concrete_tests))} \n"
-                + f"{failures}/{len(concrete_tests)} failed for {test['name']}"
-            )
-            self._append_to_file(msg, logging.INFO)
+                causal_test_case = CausalTestCase(
+                    base_test_case=base_test_case,
+                    expected_causal_effect=effects[test["expected_effect"][outcome_variable]],
+                    control_value=test["control_value"],
+                    treatment_value=test["treatment_value"],
+                    estimate_type=test["estimate_type"],
+                )
+                if self._execute_test_case(causal_test_case=causal_test_case, test=test, f_flag=f_flag):
+                    result = "failed"
+                else:
+                    result = "passed"
+
+                msg = (
+                    f"Executing concrete test: {test['name']} \n"
+                    + f"treatment variable: {test['treatment_variable']} \n"
+                    + f"outcome_variable = {outcome_variable} \n"
+                    + f"control value = {test['control_value']}, treatment value = {test['treatment_value']} \n"
+                    + f"result - {result}"
+                )
+                self._append_to_file(msg, logging.INFO)
 
-    def _execute_tests(self, concrete_tests, estimators, test, f_flag):
+    def _execute_tests(self, concrete_tests, test, f_flag):
         failures = 0
+        if "formula" in test:
+            self._append_to_file(f"Estimator formula used for test: {test['formula']}")
         for concrete_test in concrete_tests:
-            failed = self._execute_test_case(concrete_test, estimators[test["estimator"]], f_flag)
+            failed = self._execute_test_case(concrete_test, test, f_flag)
             if failed:
                 failures += 1
         return failures
 
     def _json_parse(self):
         """Parse a JSON input file into inputs, outputs, metas and a test plan"""
         with open(self.input_paths.json_path, encoding="utf-8") as f:
@@ -135,40 +207,41 @@
 
     def _populate_metas(self):
         """
         Populate data with meta-variable values and add distributions to Causal Testing Framework Variables
         """
         for meta in self.scenario.variables_of_type(Meta):
             meta.populate(self.data)
-        for var in self.scenario.variables_of_type(Meta).union(self.scenario.variables_of_type(Output)):
-            if not var.distribution:
-                fitter = Fitter(self.data[var.name], distributions=get_common_distributions())
-                fitter.fit()
-                (dist, params) = list(fitter.get_best(method="sumsquare_error").items())[0]
-                var.distribution = getattr(scipy.stats, dist)(**params)
-                self._append_to_file(var.name + f" {dist}({params})", logging.INFO)
 
-    def _execute_test_case(self, causal_test_case: CausalTestCase, estimator: Estimator, f_flag: bool) -> bool:
+    def _execute_test_case(self, causal_test_case: CausalTestCase, test: Iterable[Mapping], f_flag: bool) -> bool:
         """Executes a singular test case, prints the results and returns the test case result
         :param causal_test_case: The concrete test case to be executed
+        :param test: Single JSON test definition stored in a mapping (dict)
         :param f_flag: Failure flag that if True the script will stop executing when a test fails.
         :return: A boolean that if True indicates the causal test case passed and if false indicates the test case
          failed.
         :rtype: bool
         """
         failed = False
 
-        causal_test_engine, estimation_model = self._setup_test(causal_test_case, estimator)
+        for var in self.scenario.variables_of_type(Meta).union(self.scenario.variables_of_type(Output)):
+            if not var.distribution:
+                fitter = Fitter(self.data[var.name], distributions=get_common_distributions())
+                fitter.fit()
+                (dist, params) = list(fitter.get_best(method="sumsquare_error").items())[0]
+                var.distribution = getattr(scipy.stats, dist)(**params)
+                self._append_to_file(var.name + f" {dist}({params})", logging.INFO)
+
+        causal_test_engine, estimation_model = self._setup_test(causal_test_case, test)
         causal_test_result = causal_test_engine.execute_test(
             estimation_model, causal_test_case, estimate_type=causal_test_case.estimate_type
         )
 
         test_passes = causal_test_case.expected_causal_effect.apply(causal_test_result)
 
-        result_string = str()
         if causal_test_result.ci_low() and causal_test_result.ci_high():
             result_string = (
                 f"{causal_test_result.ci_low()} < {causal_test_result.test_value.value} <  "
                 f"{causal_test_result.ci_high()}"
             )
         else:
             result_string = f"{causal_test_result.test_value.value} no confidence intervals"
@@ -179,63 +252,70 @@
                     f"{causal_test_case}\n    FAILED - expected {causal_test_case.expected_causal_effect}, "
                     f"got {result_string}"
                 )
             failed = True
             logger.warning("   FAILED- expected %s, got %s", causal_test_case.expected_causal_effect, result_string)
         return failed
 
-    def _setup_test(self, causal_test_case: CausalTestCase, estimator: Estimator) -> tuple[CausalTestEngine, Estimator]:
+    def _setup_test(
+        self, causal_test_case: CausalTestCase, test: Mapping, conditions: list[str] = None
+    ) -> tuple[CausalTestEngine, Estimator]:
         """Create the necessary inputs for a single test case
         :param causal_test_case: The concrete test case to be executed
+        :param test: Single JSON test definition stored in a mapping (dict)
+        :param conditions: A list of conditions which should be applied to the
+        data. Conditions should be in the query format detailed at
+        https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.query.html
         :returns:
                 - causal_test_engine - Test Engine instance for the test being run
                 - estimation_model - Estimator instance for the test being run
         """
 
-        data_collector = ObservationalDataCollector(self.scenario, self.data)
+        data_collector = ObservationalDataCollector(
+            self.scenario, self.data.query(" & ".join(conditions)) if conditions else self.data
+        )
         causal_test_engine = CausalTestEngine(self.causal_specification, data_collector, index_col=0)
 
         minimal_adjustment_set = self.causal_specification.causal_dag.identification(causal_test_case.base_test_case)
         treatment_var = causal_test_case.treatment_variable
         minimal_adjustment_set = minimal_adjustment_set - {treatment_var}
-        estimation_model = estimator(
-            treatment=treatment_var.name,
-            treatment_value=causal_test_case.treatment_value,
-            control_value=causal_test_case.control_value,
-            adjustment_set=minimal_adjustment_set,
-            outcome=causal_test_case.outcome_variable.name,
-            df=causal_test_engine.scenario_execution_data_df,
-            effect_modifiers=causal_test_case.effect_modifier_configuration,
-        )
-
-        self.add_modelling_assumptions(estimation_model)
-
+        estimator_kwargs = {
+            "treatment": treatment_var.name,
+            "treatment_value": causal_test_case.treatment_value,
+            "control_value": causal_test_case.control_value,
+            "adjustment_set": minimal_adjustment_set,
+            "outcome": causal_test_case.outcome_variable.name,
+            "df": causal_test_engine.scenario_execution_data_df,
+            "effect_modifiers": causal_test_case.effect_modifier_configuration,
+        }
+        if "formula" in test:
+            estimator_kwargs["formula"] = test["formula"]
+        estimation_model = test["estimator"](**estimator_kwargs)
         return causal_test_engine, estimation_model
 
-    def add_modelling_assumptions(self, estimation_model: Estimator):  # pylint: disable=unused-argument
-        """Optional abstract method where user functionality can be written to determine what assumptions are required
-        for specific test cases
-        :param estimation_model: estimator model instance for the current running test.
-        """
-        return
-
     def _append_to_file(self, line: str, log_level: int = None):
         """Appends given line(s) to the current output file. If log_level is specified it also logs that message to the
         logging level.
         :param line: The line or lines of text to be appended to the file
         :param log_level: An integer representing the logging level as specified by pythons inbuilt logging module. It
         is possible to use the inbuilt logging level variables such as logging.INFO and logging.WARNING
         """
         with open(self.output_path, "a", encoding="utf-8") as f:
-            f.write(
-                line + "\n",
-            )
+            f.write(line + "\n")
         if log_level:
             logger.log(level=log_level, msg=line)
 
+    def _get_scenario_variables(self):
+        for input_var in self.scenario.inputs():
+            self.variables["inputs"][input_var.name] = input_var
+        for output_var in self.scenario.outputs():
+            self.variables["outputs"][output_var.name] = output_var
+        for meta_var in self.scenario.metas():
+            self.variables["metas"][meta_var.name] = meta_var
+
     @staticmethod
     def check_file_exists(output_path: Path, overwrite: bool):
         """Method that checks if the given path to an output file already exists. If overwrite is true the check is
         passed.
         :param output_path: File path for the output file of the JSON Frontend
         :param overwrite: bool that if true, the current file can be overwritten
         """
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/specification/causal_dag.py` & `causal_testing_framework-4.0.0/causal_testing/specification/causal_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,9 +517,18 @@
             )
         else:
             raise ValueError("Causal effect should be 'total' or 'direct'")
 
         minimal_adjustment_set = min(minimal_adjustment_sets, key=len)
         return minimal_adjustment_set
 
+    def to_dot_string(self) -> str:
+        """Return a string of the DOT representation of the causal DAG.
+        :return DOT string of the DAG.
+        """
+        dotstring = "digraph G {\n"
+        dotstring += "".join([f"{a} -> {b};\n" for a, b in self.graph.edges])
+        dotstring += "}"
+        return dotstring
+
     def __str__(self):
         return f"Nodes: {self.graph.nodes}\nEdges: {self.graph.edges}"
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/specification/causal_specification.py` & `causal_testing_framework-4.0.0/causal_testing/specification/causal_specification.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/specification/metamorphic_relation.py` & `causal_testing_framework-4.0.0/causal_testing/specification/metamorphic_relation.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,14 +99,18 @@
         return test_results
 
     @abstractmethod
     def assertion(self, source_output, follow_up_output):
         """An assertion that should be applied to an individual metamorphic test run."""
 
     @abstractmethod
+    def to_json_stub(self, skip=True) -> dict:
+        """Convert to a JSON frontend stub string for user customisation"""
+
+    @abstractmethod
     def test_oracle(self, test_results):
         """A test oracle that assert whether the MR holds or not based on ALL test results.
 
         This method must raise an assertion, not return a bool."""
 
     def __eq__(self, other):
         same_type = self.__class__ == other.__class__
@@ -125,14 +129,26 @@
 
     def test_oracle(self, test_results):
         """A single passing test is sufficient to show presence of a causal effect."""
         assert len(test_results["fail"]) < len(
             self.tests
         ), f"{str(self)}: {len(test_results['fail'])}/{len(self.tests)} tests failed."
 
+    def to_json_stub(self, skip=True) -> dict:
+        """Convert to a JSON frontend stub string for user customisation"""
+        return {
+            "name": str(self),
+            "estimator": "LinearRegressionEstimator",
+            "estimate_type": "coefficient",
+            "effect": "direct",
+            "mutations": [self.treatment_var],
+            "expected_effect": {self.output_var: "SomeEffect"},
+            "skip": skip,
+        }
+
     def __str__(self):
         formatted_str = f"{self.treatment_var} --> {self.output_var}"
         if self.adjustment_vars:
             formatted_str += f" | {self.adjustment_vars}"
         return formatted_str
 
 
@@ -145,14 +161,26 @@
 
     def test_oracle(self, test_results):
         """A single passing test is sufficient to show presence of a causal effect."""
         assert (
             len(test_results["fail"]) == 0
         ), f"{str(self)}: {len(test_results['fail'])}/{len(self.tests)} tests failed."
 
+    def to_json_stub(self, skip=True) -> dict:
+        """Convert to a JSON frontend stub string for user customisation"""
+        return {
+            "name": str(self),
+            "estimator": "LinearRegressionEstimator",
+            "estimate_type": "coefficient",
+            "effect": "direct",
+            "mutations": [self.treatment_var],
+            "expected_effect": {self.output_var: "NoEffect"},
+            "skip": skip,
+        }
+
     def __str__(self):
         formatted_str = f"{self.treatment_var} _||_ {self.output_var}"
         if self.adjustment_vars:
             formatted_str += f" | {self.adjustment_vars}"
         return formatted_str
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/specification/scenario.py` & `causal_testing_framework-4.0.0/causal_testing/specification/scenario.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/specification/variable.py` & `causal_testing_framework-4.0.0/causal_testing/specification/variable.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/base_test_case.py` & `causal_testing_framework-4.0.0/causal_testing/testing/base_test_case.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_case.py` & `causal_testing_framework-4.0.0/causal_testing/testing/causal_test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     """
 
     def __init__(
         # pylint: disable=too-many-arguments
         self,
         base_test_case: BaseTestCase,
         expected_causal_effect: CausalTestOutcome,
-        control_value: Any,
+        control_value: Any = None,
         treatment_value: Any = None,
         estimate_type: str = "ate",
         effect_modifier_configuration: dict[Variable:Any] = None,
     ):
         """
         :param base_test_case: A BaseTestCase object consisting of a treatment variable, outcome variable and effect
         :param expected_causal_effect: The expected causal effect (Positive, Negative, No Effect).
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_engine.py` & `causal_testing_framework-4.0.0/causal_testing/testing/causal_test_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,23 @@
             risk_ratio, confidence_intervals = estimator.estimate_risk_ratio()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("risk_ratio", risk_ratio),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
                 confidence_intervals=confidence_intervals,
             )
+        elif estimate_type == "coefficient":
+            logger.debug("calculating coefficient")
+            coefficient, confidence_intervals = estimator.estimate_unit_ate()
+            causal_test_result = CausalTestResult(
+                estimator=estimator,
+                test_value=TestValue("coefficient", coefficient),
+                effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
+                confidence_intervals=confidence_intervals,
+            )
         elif estimate_type == "ate":
             logger.debug("calculating ate")
             ate, confidence_intervals = estimator.estimate_ate()
             causal_test_result = CausalTestResult(
                 estimator=estimator,
                 test_value=TestValue("ate", ate),
                 effect_modifier_configuration=causal_test_case.effect_modifier_configuration,
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_outcome.py` & `causal_testing_framework-4.0.0/causal_testing/testing/causal_test_outcome.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,27 @@
         return type(self).__name__
 
 
 class SomeEffect(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should not be zero."""
 
     def apply(self, res: CausalTestResult) -> bool:
-        if res.test_value.type == "ate":
+        if res.test_value.type in {"ate", "coefficient"}:
             return (0 < res.ci_low() < res.ci_high()) or (res.ci_low() < res.ci_high() < 0)
         if res.test_value.type == "risk_ratio":
             return (1 < res.ci_low() < res.ci_high()) or (res.ci_low() < res.ci_high() < 1)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class NoEffect(CausalTestOutcome):
     """An extension of TestOutcome representing that the expected causal effect should be zero."""
 
     def apply(self, res: CausalTestResult) -> bool:
-        if res.test_value.type == "ate":
+        print("RESULT", res)
+        if res.test_value.type in {"ate", "coefficient"}:
             return (res.ci_low() < 0 < res.ci_high()) or (abs(res.test_value.value) < 1e-10)
         if res.test_value.type == "risk_ratio":
             return (res.ci_low() < 1 < res.ci_high()) or np.isclose(res.test_value.value, 1.0, atol=1e-10)
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
 class ExactValue(SomeEffect):
@@ -59,31 +60,31 @@
             return super().apply(res) and np.isclose(res.test_value.value, self.value, atol=self.tolerance)
         return np.isclose(res.test_value.value, self.value, atol=self.tolerance)
 
     def __str__(self):
         return f"ExactValue: {self.value}±{self.tolerance}"
 
 
-class Positive(CausalTestOutcome):
+class Positive(SomeEffect):
     """An extension of TestOutcome representing that the expected causal effect should be positive."""
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.ci_valid() and not super().apply(res):
             return False
-        if res.test_value.type == "ate":
+        if res.test_value.type in {"ate", "coefficient"}:
             return res.test_value.value > 0
         if res.test_value.type == "risk_ratio":
             return res.test_value.value > 1
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
 
 
-class Negative(CausalTestOutcome):
+class Negative(SomeEffect):
     """An extension of TestOutcome representing that the expected causal effect should be negative."""
 
     def apply(self, res: CausalTestResult) -> bool:
         if res.ci_valid() and not super().apply(res):
             return False
-        if res.test_value.type == "ate":
+        if res.test_value.type in {"ate", "coefficient"}:
             return res.test_value.value < 0
         if res.test_value.type == "risk_ratio":
             return res.test_value.value < 1
         raise ValueError(f"Test Value type {res.test_value.type} is not valid for this TestOutcome")
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_result.py` & `causal_testing_framework-4.0.0/causal_testing/testing/causal_test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,18 +40,18 @@
             self.effect_modifier_configuration = effect_modifier_configuration
         else:
             self.effect_modifier_configuration = {}
 
     def __str__(self):
         base_str = (
             f"Causal Test Result\n==============\n"
-            f"Treatment: {self.estimator.treatment[0]}\n"
+            f"Treatment: {self.estimator.treatment}\n"
             f"Control value: {self.estimator.control_value}\n"
             f"Treatment value: {self.estimator.treatment_value}\n"
-            f"Outcome: {self.estimator.outcome[0]}\n"
+            f"Outcome: {self.estimator.outcome}\n"
             f"Adjustment set: {self.adjustment_set}\n"
             f"{self.test_value.type}: {self.test_value.value}\n"
         )
         confidence_str = ""
         if self.confidence_intervals:
             confidence_str += f"Confidence intervals: {self.confidence_intervals}\n"
         return base_str + confidence_str
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/causal_test_suite.py` & `causal_testing_framework-4.0.0/causal_testing/testing/causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/estimators.py` & `causal_testing_framework-4.0.0/causal_testing/testing/estimators.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,22 +69,14 @@
     @abstractmethod
     def add_modelling_assumptions(self):
         """
         Add modelling assumptions to the estimator. This is a list of strings which list the modelling assumptions that
         must hold if the resulting causal inference is to be considered valid.
         """
 
-    @abstractmethod
-    def estimate_ate(self) -> float:
-        """
-        Estimate the unit effect of the treatment on the outcome. That is, the coefficient of the treatment variable
-        in the linear regression equation.
-        :return: The intercept and coefficient of the linear regression equation
-        """
-
     def compute_confidence_intervals(self) -> list[float, float]:
         """
         Estimate the 95% Wald confidence intervals for the effect of changing the treatment from control values to
         treatment values on the outcome.
         :return: 95% Wald confidence intervals.
         """
 
@@ -316,15 +308,15 @@
         if effect_modifiers is None:
             effect_modifiers = []
 
         if formula is not None:
             self.formula = formula
         else:
             terms = [treatment] + sorted(list(adjustment_set)) + sorted(list(effect_modifiers))
-            self.formula = f"{outcome} ~ {'+'.join(((terms)))}"
+            self.formula = f"{outcome} ~ {'+'.join(terms)}"
 
         for term in self.effect_modifiers:
             self.adjustment_set.add(term)
 
     def add_modelling_assumptions(self):
         """
         Add modelling assumptions to the estimator. This is a list of strings which list the modelling assumptions that
@@ -339,18 +331,19 @@
     def estimate_unit_ate(self) -> float:
         """Estimate the unit average treatment effect of the treatment on the outcome. That is, the change in outcome
         caused by a unit change in treatment.
 
         :return: The unit average treatment effect and the 95% Wald confidence intervals.
         """
         model = self._run_linear_regression()
+        assert self.treatment in model.params, f"{self.treatment} not in {model.params}"
         unit_effect = model.params[[self.treatment]].values[0]  # Unit effect is the coefficient of the treatment
         [ci_low, ci_high] = self._get_confidence_intervals(model)
 
-        return unit_effect * self.treatment_value - unit_effect * self.control_value, [ci_low, ci_high]
+        return unit_effect, [ci_low, ci_high]
 
     def estimate_ate(self) -> tuple[float, list[float, float], float]:
         """Estimate the average treatment effect of the treatment on the outcome. That is, the change in outcome caused
         by changing the treatment variable from the control value to the treatment value.
 
         :return: The average treatment effect and the 95% Wald confidence intervals.
         """
@@ -530,29 +523,41 @@
         related linearly in the form Y = aX + b."""
         self.modelling_assumptions += """The three IV conditions must hold
             (i) Instrument is associated with treatment
             (ii) Instrument does not affect outcome except through its potential effect on treatment
             (iii) Instrument and outcome do not share causes
         """
 
-    def estimate_coefficient(self):
+    def estimate_coefficient(self, df):
         """
-        Estimate the linear regression coefficient of the treatment on the outcome.
+        Estimate the linear regression coefficient of the treatment on the
+        outcome.
         """
         # Estimate the total effect of instrument I on outcome Y = abI + c1
-        ab = sm.OLS(self.df[self.outcome], self.df[[self.instrument]]).fit().params[self.instrument]
+        ab = sm.OLS(df[self.outcome], df[[self.instrument]]).fit().params[self.instrument]
 
         # Estimate the direct effect of instrument I on treatment X = aI + c1
-        a = sm.OLS(self.df[self.treatment], self.df[[self.instrument]]).fit().params[self.instrument]
+        a = sm.OLS(df[self.treatment], df[[self.instrument]]).fit().params[self.instrument]
 
         # Estimate the coefficient of I on X by cancelling
         return ab / a
 
-    def estimate_ate(self):
-        return (self.treatment_value - self.control_value) * self.estimate_coefficient(), (None, None)
+    def estimate_unit_ate(self, bootstrap_size=100):
+        """
+        Estimate the unit ate (i.e. coefficient) of the treatment on the
+        outcome.
+        """
+        bootstraps = sorted(
+            [self.estimate_coefficient(self.df.sample(len(self.df), replace=True)) for _ in range(bootstrap_size)]
+        )
+        bound = ceil((bootstrap_size * 0.05) / 2)
+        ci_low = bootstraps[bound]
+        ci_high = bootstraps[bootstrap_size - bound]
+
+        return self.estimate_coefficient(self.df), (ci_low, ci_high)
 
 
 class CausalForestEstimator(Estimator):
     """A causal random forest estimator is a non-parametric estimator which recursively partitions the covariate space
     to learn a low-dimensional representation of treatment effect heterogeneity. This form of estimator is best suited
     to the estimation of heterogeneous treatment effects i.e. the estimated effect for every sample rather than the
     population average.
```

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/intervention.py` & `causal_testing_framework-4.0.0/causal_testing/testing/intervention.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing/testing/validation.py` & `causal_testing_framework-4.0.0/causal_testing/testing/validation.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/causal_testing_framework.egg-info/PKG-INFO` & `causal_testing_framework-4.0.0/causal_testing_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causal-testing-framework
-Version: 3.2.0
+Version: 4.0.0
 Summary: A framework for causal testing using causal directed acyclic graphs.
 Author: The CITCOM team
 License: MIT
 Project-URL: Bug_Tracker, https://github.com/CITCOM-project/CausalTestingFramework/issues
 Project-URL: Documentation, https://causal-testing-framework.readthedocs.io/
 Project-URL: Source, https://github.com/CITCOM-project/CausalTestingFramework
 Keywords: causal inference,verification
```

### Comparing `causal_testing_framework-3.2.0/causal_testing_framework.egg-info/SOURCES.txt` & `causal_testing_framework-4.0.0/causal_testing_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 .github/workflows/lint-format.yaml
 .github/workflows/publish-to-pypi.yaml
 causal_testing/__init__.py
 causal_testing/data_collection/__init__.py
 causal_testing/data_collection/data_collector.py
 causal_testing/generation/__init__.py
 causal_testing/generation/abstract_causal_test_case.py
+causal_testing/generation/enum_gen.py
 causal_testing/json_front/__init__.py
 causal_testing/json_front/json_class.py
 causal_testing/specification/__init__.py
 causal_testing/specification/causal_dag.py
 causal_testing/specification/causal_specification.py
 causal_testing/specification/metamorphic_relation.py
 causal_testing/specification/scenario.py
```

### Comparing `causal_testing_framework-3.2.0/docs/Makefile` & `causal_testing_framework-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/README.md` & `causal_testing_framework-4.0.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/make.bat` & `causal_testing_framework-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/conf.py` & `causal_testing_framework-4.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/description.rst` & `causal_testing_framework-4.0.0/docs/source/description.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/frontends/json_front_end.rst` & `causal_testing_framework-4.0.0/docs/source/frontends/json_front_end.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,36 @@
 4. Meta constraint functions
 5. Mapping JSON distributions, effects, and estimators to python objects
 
 Use case specific information is also declared here such as the paths to the relevant files needed for the tests.
 
 causal_tests.json
 -----------------
-`examples/poisson/causal_tests.json <https://github.com/CITCOM-project/CausalTestingFramework/blob/main/examples/poisson/causal_tests.json>`_ contains python code written by the user to implement scenario specific features
-is the JSON file that allows for the easy specification of multiple causal tests.
+`examples/poisson/causal_tests.json <https://github.c#om/CITCOM-project/CausalTestingFramework/blob/main/examples/poisson/causal_tests.json>`_ contains python code written by the user to implement scenario specific features
+is the JSON file that allows for the easy specification of multiple causal tests. Tests can be specified two ways; firstly by specifying a mutation lke in the example tests with the following structure:
 Each test requires:
-1. Test name
-2. Mutations
-3. Estimator
-4. Estimate_type
-5. Effect modifiers
-6. Expected effects
-7. Skip: boolean that if set true the test won't be executed and will be skipped
 
+#. name
+#. mutations
+#. estimator
+#. estimate_type
+#. effect_modifiers
+#. expected_effects
+#. skip: boolean that if set true the test won't be executed and will be skipped
+
+The second method of specifying a test is to specify the test in a concrete form with the following structure:
+
+#. name
+#. treatment_variable
+#. control_value
+#. treatment_value
+#. estimator
+#. estimate_type
+#. expected_effect
+#. skip
 
 Run Commands
 ------------
 To run the JSON frontend example from the root directory of the project, use::
 
     python examples\poisson\run_causal_tests.py --data_path="examples\poisson\data.csv" --dag_path="examples\poisson\dag.dot" --json_path="examples\poisson\causal_tests.json
```

### Comparing `causal_testing_framework-3.2.0/docs/source/frontends/test_suite.rst` & `causal_testing_framework-4.0.0/docs/source/frontends/test_suite.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/images/workflow.png` & `causal_testing_framework-4.0.0/docs/source/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/index.rst` & `causal_testing_framework-4.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/installation.rst` & `causal_testing_framework-4.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/modules/causal_specification.rst` & `causal_testing_framework-4.0.0/docs/source/modules/causal_specification.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/modules/causal_tests.rst` & `causal_testing_framework-4.0.0/docs/source/modules/causal_tests.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/modules/data_collector.rst` & `causal_testing_framework-4.0.0/docs/source/modules/data_collector.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/docs/source/usage.rst` & `causal_testing_framework-4.0.0/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/README.md` & `causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/dag.png` & `causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv` & `causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/data/10k_observational_data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/doubling_beta/example_beta.py` & `causal_testing_framework-4.0.0/examples/covasim_/doubling_beta/example_beta.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,62 +44,83 @@
 
     :param observational_data_path: Path to csv containing observational data for analysis.
     :param simulate_counterfactuals: Whether to repeat analysis with counterfactuals.
     :param verbose: Whether to print verbose details (causal test results).
     :return results_dict: A nested dictionary containing results (ate and confidence intervals)
                           for association, causation, and counterfactual (if completed).
     """
-    results_dict = {'association': {},
-                    'causation': {}}
+    results_dict = {"association": {}, "causation": {}}
 
     # Read in the observational data, perform identification, and setup the causal_test_engine
     past_execution_df = pd.read_csv(observational_data_path)
     _, causal_test_engine, causal_test_case = engine_setup(observational_data_path)
 
-    linear_regression_estimator = LinearRegressionEstimator('beta', 0.032, 0.016,
-                                                            {'avg_age', 'contacts'},  # We use custom adjustment set
-                                                            'cum_infections',
-                                                            df=past_execution_df,
-                                                            formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts")
+    linear_regression_estimator = LinearRegressionEstimator(
+        "beta",
+        0.032,
+        0.016,
+        {"avg_age", "contacts"},  # We use custom adjustment set
+        "cum_infections",
+        df=past_execution_df,
+        formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
+    )
 
     # Add squared terms for beta, since it has a quadratic relationship with cumulative infections
-    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, 'ate')
+    causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, "ate")
 
     # Repeat for association estimate (no adjustment)
-    no_adjustment_linear_regression_estimator = LinearRegressionEstimator('beta', 0.032, 0.016,
-                                                                          set(),
-                                                                          'cum_infections',
-                                                                          df=past_execution_df,
-                                                                          formula="cum_infections ~ beta + np.power(beta, 2)")
-    association_test_result = causal_test_engine.execute_test(no_adjustment_linear_regression_estimator, causal_test_case, 'ate')
+    no_adjustment_linear_regression_estimator = LinearRegressionEstimator(
+        "beta",
+        0.032,
+        0.016,
+        set(),
+        "cum_infections",
+        df=past_execution_df,
+        formula="cum_infections ~ beta + np.power(beta, 2)",
+    )
+    association_test_result = causal_test_engine.execute_test(
+        no_adjustment_linear_regression_estimator, causal_test_case, "ate"
+    )
 
     # Store results for plotting
-    results_dict['association'] = {'ate': association_test_result.test_value.value,
-                                   'cis': association_test_result.confidence_intervals,
-                                   'df': past_execution_df}
-    results_dict['causation'] = {'ate': causal_test_result.test_value.value,
-                                 'cis': causal_test_result.confidence_intervals,
-                                 'df': past_execution_df}
+    results_dict["association"] = {
+        "ate": association_test_result.test_value.value,
+        "cis": association_test_result.confidence_intervals,
+        "df": past_execution_df,
+    }
+    results_dict["causation"] = {
+        "ate": causal_test_result.test_value.value,
+        "cis": causal_test_result.confidence_intervals,
+        "df": past_execution_df,
+    }
 
     if verbose:
         print(f"Association:\n{association_test_result}")
         print(f"Causation:\n{causal_test_result}")
 
     # Repeat causal inference after deleting all rows with treatment value to obtain counterfactual inferences
     if simulate_counterfactuals:
-        counterfactual_past_execution_df = past_execution_df[past_execution_df['beta'] != 0.032]
-        counterfactual_linear_regression_estimator = LinearRegressionEstimator('beta', 0.032, 0.016,
-                                                                               {'avg_age', 'contacts'},
-                                                                               'cum_infections',
-                                                                               df=counterfactual_past_execution_df,
-                                                                               formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts")
-        counterfactual_causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, 'ate')
-        results_dict['counterfactual'] = {'ate': counterfactual_causal_test_result.test_value.value,
-                                          'cis': counterfactual_causal_test_result.confidence_intervals,
-                                          'df': counterfactual_past_execution_df}
+        counterfactual_past_execution_df = past_execution_df[past_execution_df["beta"] != 0.032]
+        counterfactual_linear_regression_estimator = LinearRegressionEstimator(
+            "beta",
+            0.032,
+            0.016,
+            {"avg_age", "contacts"},
+            "cum_infections",
+            df=counterfactual_past_execution_df,
+            formula="cum_infections ~ beta + np.power(beta, 2) + avg_age + contacts",
+        )
+        counterfactual_causal_test_result = causal_test_engine.execute_test(
+            linear_regression_estimator, causal_test_case, "ate"
+        )
+        results_dict["counterfactual"] = {
+            "ate": counterfactual_causal_test_result.test_value.value,
+            "cis": counterfactual_causal_test_result.confidence_intervals,
+            "df": counterfactual_past_execution_df,
+        }
         if verbose:
             print(f"Counterfactual:\n{counterfactual_causal_test_result}")
 
     return results_dict
 
 
 def doubling_beta_CATEs(observational_data_path: str, simulate_counterfactual: bool = False, verbose: bool = False):
```

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/README.md` & `causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/dag.png` & `causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/covasim_/vaccinating_elderly/example_vaccine.py` & `causal_testing_framework-4.0.0/examples/covasim_/vaccinating_elderly/example_vaccine.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/README.md` & `causal_testing_framework-4.0.0/examples/lr91/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/dag.dot` & `causal_testing_framework-4.0.0/examples/lr91/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/dag.png` & `causal_testing_framework-4.0.0/examples/lr91/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/data/normalised_results.csv` & `causal_testing_framework-4.0.0/examples/lr91/data/normalised_results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/data/results.csv` & `causal_testing_framework-4.0.0/examples/lr91/data/results.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/lr91/example_max_conductances.py` & `causal_testing_framework-4.0.0/examples/lr91/example_max_conductances.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     # 10. Run the causal test and print results
     causal_test_result = causal_test_engine.execute_test(linear_regression_estimator, causal_test_case, "ate")
     logger.info("%s", causal_test_result)
     return causal_test_result.test_value.value, causal_test_result.confidence_intervals
 
 
-def plot_ates_with_cis(results_dict: dict, xs: list, save: bool = True, show: bool = False):
+def plot_ates_with_cis(results_dict: dict, xs: list, save: bool = False, show: bool = False):
     """Plot the average treatment effects for a given treatment against a list of x-values with confidence intervals.
 
     :param results_dict: A dictionary containing results for sensitivity analysis of each input parameter.
     :param xs: Values to be plotted on the x-axis.
     :param save: Whether to save the plot.
     """
     fig, axes = plt.subplots()
```

### Comparing `causal_testing_framework-3.2.0/examples/lr91/example_max_conductances_test_suite.py` & `causal_testing_framework-4.0.0/examples/lr91/example_max_conductances_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson/README.md` & `causal_testing_framework-4.0.0/examples/poisson/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 Here we demonstrate how the same test suite as in `poisson-line-process` can be coded using the JSON front end.
 
 ## How to run
 To run this case study:
 1. Ensure all project dependencies are installed by running `pip install .` in the top level directory
    (instructions are provided in the project README).
 2. Change directory to `causal_testing/examples/poisson`.
-3. Run the command `python test_run_causal_tests.py --data_path data.csv --dag_path dag.dot --json_path causal_tests.json`
+3. Run the command `python example_run_causal_tests.py --data_path data.csv --dag_path dag.dot --json_path causal_tests.json`
 
 This should print a series of causal test results and produce two CSV files. `intensity_num_shapes_results_random_1000.csv` corresponds to table 1, and `width_num_shapes_results_random_1000.csv` relates to our findings regarding the relationship of width and `P_u`.
```

### Comparing `causal_testing_framework-3.2.0/examples/poisson/causal_tests.json` & `causal_testing_framework-4.0.0/examples/poisson/causal_tests.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8743131868131868%*

 * *Differences: {"'tests'": "{0: {'expected_effect': OrderedDict([('num_lines_abs', 'PoissonWidthHeight')]), "*

 * *            "delete: ['expectedEffect']}, 1: {'expected_effect': OrderedDict([('num_shapes_abs', "*

 * *            "'Positive')]), delete: ['expectedEffect']}, 2: {'expected_effect': "*

 * *            "OrderedDict([('num_lines_unit', 'Negative')]), delete: ['expectedEffect']}, 3: "*

 * *            "{'expected_effect': OrderedDict([('num_shapes_unit', 'Negative')]), delete: "*

 * *            "['expectedEffect']}, 4: {'expected_eff […]*

```diff
@@ -3,15 +3,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "height"
             ],
             "estimate_type": "ate",
             "estimator": "WidthHeightEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_abs": "PoissonWidthHeight"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__num_lines_abs",
             "skip": true
@@ -19,15 +19,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "height"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_abs": "Positive"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__num_shapes_abs",
             "skip": true
@@ -35,15 +35,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "height"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "Negative"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__num_lines_unit",
             "skip": true
@@ -51,41 +51,41 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "height"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "Negative"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__num_shapes_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "height": "NoEffect"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__height",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "intensity": "NoEffect"
             },
             "mutations": {
                 "width": "Increase"
             },
             "name": "width__intensity",
             "skip": true
@@ -93,119 +93,119 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "CausalForestEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_abs": "Positive"
             },
             "mutations": {
                 "num_lines_abs": "Increase"
             },
             "name": "num_lines_abs__num_shapes_abs",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "Positive"
             },
             "mutations": {
                 "num_lines_abs": "Increase"
             },
             "name": "num_lines_abs__num_lines_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "NoEffect"
             },
             "mutations": {
                 "num_lines_abs": "Increase"
             },
             "name": "num_lines_abs__num_shapes_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "NoEffect"
             },
             "mutations": {
                 "num_shapes_abs": "Increase"
             },
             "name": "num_shapes_abs__num_lines_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "Positive"
             },
             "mutations": {
                 "num_shapes_abs": "Increase"
             },
             "name": "num_shapes_abs__num_shapes_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_abs": "NoEffect"
             },
             "mutations": {
                 "num_lines_unit": "Increase"
             },
             "name": "num_lines_unit__num_shapes_abs",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "NoEffect"
             },
             "mutations": {
                 "num_lines_unit": "Increase"
             },
             "name": "num_lines_unit__num_shapes_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "NoEffect"
             },
             "mutations": {
                 "num_shapes_unit": "Increase"
             },
             "name": "num_shapes_unit__num_lines_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "width": "NoEffect"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__width",
             "skip": true
@@ -213,15 +213,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "WidthHeightEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_abs": "PoissonWidthHeight"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__num_lines_abs",
             "skip": true
@@ -229,15 +229,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_abs": "Positive"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__num_shapes_abs",
             "skip": true
@@ -245,15 +245,15 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "Negative"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__num_lines_unit",
             "skip": true
@@ -261,41 +261,41 @@
         {
             "effect_modifiers": [
                 "intensity",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "Negative"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__num_shapes_unit",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "intensity": "NoEffect"
             },
             "mutations": {
                 "height": "Increase"
             },
             "name": "height__intensity",
             "skip": true
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "width": "NoEffect"
             },
             "mutations": {
                 "intensity": "Increase"
             },
             "name": "intensity__width",
             "skip": true
@@ -303,15 +303,15 @@
         {
             "effect_modifiers": [
                 "height",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "WidthHeightEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_abs": "PoissonIntensity"
             },
             "mutations": {
                 "intensity": "Increase"
             },
             "name": "intensity__num_lines_abs",
             "skip": true
@@ -319,15 +319,15 @@
         {
             "effect_modifiers": [
                 "height",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_abs": "Positive"
             },
             "mutations": {
                 "intensity": "Increase"
             },
             "name": "intensity__num_shapes_abs",
             "skip": true
@@ -335,40 +335,40 @@
         {
             "effect_modifiers": [
                 "height",
                 "width"
             ],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_lines_unit": "NoEffect"
             },
             "mutations": {
                 "intensity": "Increase"
             },
             "name": "intensity__num_lines_unit",
             "skip": true
         },
         {
             "estimate_type": "risk_ratio",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "num_shapes_unit": "ExactValue4_05"
             },
             "mutations": {
                 "intensity": "ChangeByFactor(2)"
             },
             "name": "intensity__num_shapes_unit",
             "skip": false
         },
         {
             "effect_modifiers": [],
             "estimate_type": "ate",
             "estimator": "LinearRegressionEstimator",
-            "expectedEffect": {
+            "expected_effect": {
                 "height": "NoEffect"
             },
             "mutations": {
                 "intensity": "Increase"
             },
             "name": "intensity__height",
             "skip": true
```

### Comparing `causal_testing_framework-3.2.0/examples/poisson/dag.dot` & `causal_testing_framework-4.0.0/examples/poisson/dag.dot`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson/data.csv` & `causal_testing_framework-4.0.0/examples/poisson/data.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson/example_run_causal_tests.py` & `causal_testing_framework-4.0.0/examples/poisson/example_run_causal_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,46 +145,37 @@
 mutates = {
     "Increase": lambda x: modelling_scenario.treatment_variables[x].z3 > modelling_scenario.variables[x].z3,
     "ChangeByFactor(2)": lambda x: modelling_scenario.treatment_variables[x].z3
     == modelling_scenario.variables[x].z3 * 2,
 }
 
 
-class MyJsonUtility(JsonUtility):
-    """Extension of JsonUtility class to add modelling assumptions to the estimator instance"""
-
-    def add_modelling_assumptions(self, estimation_model: Estimator):
-        # Add squared intensity term as a modelling assumption if intensity is the treatment of the test
-        if "intensity" in estimation_model.treatment[0]:
-            estimation_model.intercept = 0
-
-
 def test_run_causal_tests():
     ROOT = os.path.realpath(os.path.dirname(__file__))
 
     log_path = f"{ROOT}/json_frontend.log"
     json_path = f"{ROOT}/causal_tests.json"
     dag_path = f"{ROOT}/dag.dot"
     data_path = f"{ROOT}/data.csv"
 
-    json_utility = MyJsonUtility(log_path)  # Create an instance of the extended JsonUtility class
+    json_utility = JsonUtility(log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         json_path, dag_path, [data_path]
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
     json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
 
-    json_utility.generate_tests(effects, mutates, estimators, False)
+    json_utility.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
 
 if __name__ == "__main__":
-    args = MyJsonUtility.get_args()
-    json_utility = MyJsonUtility(args.log_path)  # Create an instance of the extended JsonUtility class
+    args = JsonUtility.get_args()
+    json_utility = JsonUtility(args.log_path)  # Create an instance of the extended JsonUtility class
     json_utility.set_paths(
         args.json_path, args.dag_path, args.data_path
     )  # Set the path to the data.csv, dag.dot and causal_tests.json file
 
     # Load the Causal Variables into the JsonUtility class ready to be used in the tests
     json_utility.setup(scenario=modelling_scenario)  # Sets up all the necessary parts of the json_class needed to execute tests
 
-    json_utility.generate_tests(effects, mutates, estimators, args.f)
+    json_utility.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=args.f)
```

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/README.md` & `causal_testing_framework-4.0.0/examples/poisson-line-process/README.md`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/dag.png` & `causal_testing_framework-4.0.0/examples/poisson-line-process/dag.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/random/data_random_1000.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/random/data_random_1000.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh10_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh1_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh2_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh3_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh4_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh5_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh6_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh7_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh8_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv` & `causal_testing_framework-4.0.0/examples/poisson-line-process/data/smt_100/data_smt_wh9_100.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/examples/poisson-line-process/example_poisson_process.py` & `causal_testing_framework-4.0.0/examples/poisson-line-process/example_poisson_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,15 @@
     inverse_terms=[],
     empirical=False,
 ):
     # 6. Create a data collector
     data_collector = ObservationalDataCollector(scenario, pd.read_csv(observational_data_path))
 
     # 7. Create an instance of the causal test engine
-    causal_test_engine = CausalTestEngine(
-        causal_specification, data_collector
-    )
+    causal_test_engine = CausalTestEngine(causal_specification, data_collector)
 
     # 8. Obtain the minimal adjustment set for the causal test case from the causal DAG
     minimal_adjustment_set = causal_dag.identification(causal_test_case.base_test_case)
 
     # 9. Set up an estimator
     data = pd.read_csv(observational_data_path)
 
@@ -117,21 +115,19 @@
             treatment=treatment,
             control_value=causal_test_case.control_value,
             treatment_value=causal_test_case.treatment_value,
             adjustment_set=set(),
             outcome=outcome,
             df=data,
             effect_modifiers=causal_test_case.effect_modifier_configuration,
-            formula=f"{outcome} ~ {treatment} + {'+'.join(square_terms + inverse_terms + list([e for e in causal_test_case.effect_modifier_configuration]))} -1"
+            formula=f"{outcome} ~ {treatment} + {'+'.join(square_terms + inverse_terms + list([e for e in causal_test_case.effect_modifier_configuration]))} -1",
         )
 
     # 10. Execute the test
-    causal_test_result = causal_test_engine.execute_test(
-        estimator, causal_test_case, causal_test_case.estimate_type
-    )
+    causal_test_result = causal_test_engine.execute_test(estimator, causal_test_case, causal_test_case.estimate_type)
 
     return causal_test_result
 
 
 def test_poisson_intensity_num_shapes(save=False):
     intensity_num_shapes_results = []
     for wh in range(1, 11):
```

### Comparing `causal_testing_framework-3.2.0/images/workflow.png` & `causal_testing_framework-4.0.0/images/workflow.png`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/pyproject.toml` & `causal_testing_framework-4.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/data/nhefs.csv` & `causal_testing_framework-4.0.0/tests/data/nhefs.csv`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/data_collection_tests/test_observational_data_collector.py` & `causal_testing_framework-4.0.0/tests/data_collection_tests/test_observational_data_collector.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/generation_tests/test_abstract_test_case.py` & `causal_testing_framework-4.0.0/tests/generation_tests/test_abstract_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import unittest
 import os
 import pandas as pd
 import numpy as np
 from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
+from causal_testing.generation.enum_gen import EnumGen
 from causal_testing.specification.causal_specification import Scenario
 from causal_testing.specification.variable import Input, Output
 from scipy.stats import uniform, rv_discrete
 from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
 from causal_testing.testing.causal_test_outcome import Positive
 from z3 import And
 from enum import Enum
@@ -18,25 +19,14 @@
 
     def __gt__(self, other):
         if self.__class__ is other.__class__:
             return self.value > other.value
         return NotImplemented
 
 
-class CarGen(rv_discrete):
-    cars = dict(enumerate(Car, 1))
-    inverse_cars = {v: k for k, v in cars.items()}
-
-    def ppf(self, q, *args, **kwds):
-        return np.vectorize(self.cars.get)(np.ceil(len(self.cars) * q))
-
-    def cdf(self, q, *args, **kwds):
-        return np.vectorize(self.inverse_cars.get)(q) / len(Car)
-
-
 class TestAbstractTestCase(unittest.TestCase):
     """
     Class to test abstract test cases.
     """
 
     def setUp(self) -> None:
         temp_dir_path = create_temp_dir_if_non_existent()
@@ -49,15 +39,15 @@
         )
         self.observational_df.to_csv(self.observational_df_path)
         self.X1 = Input("X1", float, uniform(1, 4))
         self.X2 = Input("X2", int, rv_discrete(values=([7], [1])))
         self.X3 = Input("X3", float, uniform(10, 40))
         self.X4 = Input("X4", int, rv_discrete(values=([10], [1])))
         self.X5 = Input("X5", bool, rv_discrete(values=(range(2), [0.5, 0.5])))
-        self.Car = Input("Car", Car, CarGen())
+        self.Car = Input("Car", Car, EnumGen(Car))
         self.Y = Output("Y", int)
 
     def test_generate_concrete_test_cases(self):
         scenario = Scenario({self.X1, self.X2, self.X3, self.X4})
         scenario.setup_treatment_variables()
         abstract = AbstractCausalTestCase(
             scenario=scenario,
```

### Comparing `causal_testing_framework-3.2.0/tests/json_front_tests/test_json_class.py` & `causal_testing_framework-4.0.0/tests/json_front_tests/test_json_class.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import unittest
 from pathlib import Path
 from statistics import StatisticsError
 import scipy
-import csv
-import json
+
 
 from causal_testing.testing.estimators import LinearRegressionEstimator
-from causal_testing.testing.causal_test_outcome import NoEffect
-from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
+from causal_testing.testing.causal_test_outcome import NoEffect, Positive
+from tests.test_helpers import remove_temp_dir_if_existent
 from causal_testing.json_front.json_class import JsonUtility, CausalVariables
 from causal_testing.specification.variable import Input, Output, Meta
 from causal_testing.specification.scenario import Scenario
 from causal_testing.specification.causal_specification import CausalSpecification
-from causal_testing.generation.abstract_causal_test_case import AbstractCausalTestCase
 
 
 class TestJsonClass(unittest.TestCase):
     """Test the JSON frontend for the Causal Testing Framework (CTF)
 
     The JSON frontend is an alternative interface for the CTF where tests are specified in JSON format and ingested
     with the frontend. Tests involve testing that this correctly interfaces with the framework with some dummy data
@@ -28,43 +26,47 @@
         data_file_name = "data_with_meta.csv"
         test_data_dir_path = Path("tests/resources/data")
         self.json_path = str(test_data_dir_path / json_file_name)
         self.dag_path = str(test_data_dir_path / dag_file_name)
         self.data_path = [str(test_data_dir_path / data_file_name)]
         self.json_class = JsonUtility("temp_out.txt", True)
         self.example_distribution = scipy.stats.uniform(1, 10)
-        self.input_dict_list = [{"name": "test_input", "datatype": float, "distribution": self.example_distribution}]
+        self.input_dict_list = [
+            {"name": "test_input", "datatype": float, "distribution": self.example_distribution},
+            {"name": "test_input_no_dist", "datatype": float},
+        ]
         self.output_dict_list = [{"name": "test_output", "datatype": float}]
         self.meta_dict_list = [{"name": "test_meta", "datatype": float, "populate": populate_example}]
-        variables = CausalVariables(inputs=self.input_dict_list, outputs=self.output_dict_list,
-                                    metas=self.meta_dict_list)
+        variables = CausalVariables(
+            inputs=self.input_dict_list, outputs=self.output_dict_list, metas=self.meta_dict_list
+        )
         self.scenario = Scenario(variables=variables, constraints=None)
         self.json_class.set_paths(self.json_path, self.dag_path, self.data_path)
         self.json_class.setup(self.scenario)
 
     def test_setting_paths(self):
         self.assertEqual(self.json_class.input_paths.json_path, Path(self.json_path))
         self.assertEqual(self.json_class.input_paths.dag_path, Path(self.dag_path))
         self.assertEqual(self.json_class.input_paths.data_paths, [Path(self.data_path[0])])  # Needs to be list of Paths
 
     def test_set_inputs(self):
         ctf_input = [Input("test_input", float, self.example_distribution)]
-        self.assertEqual(ctf_input[0].name, self.json_class.scenario.variables['test_input'].name)
-        self.assertEqual(ctf_input[0].datatype, self.json_class.scenario.variables['test_input'].datatype)
-        self.assertEqual(ctf_input[0].distribution, self.json_class.scenario.variables['test_input'].distribution)
+        self.assertEqual(ctf_input[0].name, self.json_class.scenario.variables["test_input"].name)
+        self.assertEqual(ctf_input[0].datatype, self.json_class.scenario.variables["test_input"].datatype)
+        self.assertEqual(ctf_input[0].distribution, self.json_class.scenario.variables["test_input"].distribution)
 
     def test_set_outputs(self):
         ctf_output = [Output("test_output", float)]
-        self.assertEqual(ctf_output[0].name, self.json_class.scenario.variables['test_output'].name)
-        self.assertEqual(ctf_output[0].datatype, self.json_class.scenario.variables['test_output'].datatype)
+        self.assertEqual(ctf_output[0].name, self.json_class.scenario.variables["test_output"].name)
+        self.assertEqual(ctf_output[0].datatype, self.json_class.scenario.variables["test_output"].datatype)
 
     def test_set_metas(self):
         ctf_meta = [Meta("test_meta", float, populate_example)]
-        self.assertEqual(ctf_meta[0].name, self.json_class.scenario.variables['test_meta'].name)
-        self.assertEqual(ctf_meta[0].datatype, self.json_class.scenario.variables['test_meta'].datatype)
+        self.assertEqual(ctf_meta[0].name, self.json_class.scenario.variables["test_meta"].name)
+        self.assertEqual(ctf_meta[0].datatype, self.json_class.scenario.variables["test_meta"].datatype)
 
     def test_argparse(self):
         args = self.json_class.get_args(["--data_path=data.csv", "--dag_path=dag.dot", "--json_path=tests.json"])
         self.assertEqual(args.data_path, ["data.csv"])
         self.assertEqual(args.dag_path, "dag.dot")
         self.assertEqual(args.json_path, "tests.json")
 
@@ -79,58 +81,164 @@
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
                     "estimator": "LinearRegressionEstimator",
                     "estimate_type": "ate",
                     "effect_modifiers": [],
-                    "expectedEffect": {"test_output": "NoEffect"},
+                    "expected_effect": {"test_output": "NoEffect"},
                     "skip": False,
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
         with self.assertRaises(StatisticsError):
-            self.json_class.generate_tests(effects, mutates, estimators, True)
+            self.json_class.run_json_tests(effects, estimators, True, mutates)
+
+    def test_generate_coefficient_tests_from_json(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "mutations": ["test_input"],
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "coefficient",
+                    "effect_modifiers": [],
+                    "expected_effect": {"test_output": "NoEffect"},
+                    "skip": False,
+                }
+            ]
+        }
+        self.json_class.test_plan = example_test
+        effects = {"NoEffect": NoEffect()}
+        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+
+        self.json_class.run_json_tests(effects=effects, mutates={}, estimators=estimators, f_flag=False)
+
+        # Test that the final log message prints that failed tests are printed, which is expected behaviour for this scenario
+        with open("temp_out.txt", "r") as reader:
+            temp_out = reader.readlines()
+        self.assertIn("failed", temp_out[-1])
 
-    def test_generate_tests_from_json(self):
+    def test_run_json_tests_from_json(self):
         example_test = {
             "tests": [
                 {
                     "name": "test1",
                     "mutations": {"test_input": "Increase"},
                     "estimator": "LinearRegressionEstimator",
                     "estimate_type": "ate",
                     "effect_modifiers": [],
-                    "expectedEffect": {"test_output": "NoEffect"},
+                    "expected_effect": {"test_output": "NoEffect"},
                     "skip": False,
                 }
             ]
         }
         self.json_class.test_plan = example_test
         effects = {"NoEffect": NoEffect()}
         mutates = {
             "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
-                                  > self.json_class.scenario.variables[x].z3
+            > self.json_class.scenario.variables[x].z3
         }
         estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
 
-        self.json_class.generate_tests(effects, mutates, estimators, False)
+        self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False, mutates=mutates)
+
+        # Test that the final log message prints that failed tests are printed, which is expected behaviour for this
+        # scenario
+        with open("temp_out.txt", "r") as reader:
+            temp_out = reader.readlines()
+        self.assertIn("failed", temp_out[-1])
+
+    def test_generate_tests_from_json_no_dist(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "mutations": {"test_input_no_dist": "Increase"},
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "ate",
+                    "effect_modifiers": [],
+                    "expected_effect": {"test_output": "NoEffect"},
+                    "skip": False,
+                }
+            ]
+        }
+        self.json_class.test_plan = example_test
+        effects = {"NoEffect": NoEffect()}
+        mutates = {
+            "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
+            > self.json_class.scenario.variables[x].z3
+        }
+        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+
+        self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
 
         # Test that the final log message prints that failed tests are printed, which is expected behaviour for this scenario
+        with open("temp_out.txt", "r") as reader:
+            temp_out = reader.readlines()
+        self.assertIn("failed", temp_out[-1])
+
+    def test_formula_in_json_test(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "mutations": {"test_input": "Increase"},
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "ate",
+                    "effect_modifiers": [],
+                    "expected_effect": {"test_output": "Positive"},
+                    "skip": False,
+                    "formula": "test_output ~ test_input",
+                }
+            ]
+        }
+        self.json_class.test_plan = example_test
+        effects = {"Positive": Positive()}
+        mutates = {
+            "Increase": lambda x: self.json_class.scenario.treatment_variables[x].z3
+            > self.json_class.scenario.variables[x].z3
+        }
+        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+
+        self.json_class.run_json_tests(effects=effects, mutates=mutates, estimators=estimators, f_flag=False)
+        with open("temp_out.txt", "r") as reader:
+            temp_out = reader.readlines()
+        self.assertIn("test_output ~ test_input", "".join(temp_out))
+
+    def test_run_concrete_json_testcase(self):
+        example_test = {
+            "tests": [
+                {
+                    "name": "test1",
+                    "treatment_variable": "test_input",
+                    "control_value": 0,
+                    "treatment_value": 1,
+                    "estimator": "LinearRegressionEstimator",
+                    "estimate_type": "ate",
+                    "expected_effect": {"test_output": "NoEffect"},
+                    "skip": False,
+                }
+            ]
+        }
+        self.json_class.test_plan = example_test
+        effects = {"NoEffect": NoEffect()}
+        estimators = {"LinearRegressionEstimator": LinearRegressionEstimator}
+
+        self.json_class.run_json_tests(effects=effects, estimators=estimators, f_flag=False)
         with open("temp_out.txt", 'r') as reader:
             temp_out = reader.readlines()
         self.assertIn("failed", temp_out[-1])
 
     def tearDown(self) -> None:
-        pass
-        # remove_temp_dir_if_existent()
+        remove_temp_dir_if_existent()
 
 
 def populate_example(*args, **kwargs):
     pass
```

### Comparing `causal_testing_framework-3.2.0/tests/specification_tests/test_causal_dag.py` & `causal_testing_framework-4.0.0/tests/specification_tests/test_causal_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     In particular, confirm whether the Causal DAG class creates valid causal directed acyclic graphs (empty and directed
     graphs without cycles) and refuses to create invalid (cycle-containing) graphs.
     """
 
     def setUp(self) -> None:
         temp_dir_path = create_temp_dir_if_non_existent()
         self.dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
-        dag_dot = """digraph G { A -> B; B -> C; D -> A; D -> C}"""
+        dag_dot = """digraph G { A -> B; B -> C; D -> A; D -> C;}"""
         f = open(self.dag_dot_path, "w")
         f.write(dag_dot)
         f.close()
 
     def test_valid_causal_dag(self):
         """Test whether the Causal DAG is valid."""
         causal_dag = CausalDAG(self.dag_dot_path)
@@ -95,14 +95,18 @@
         self.assertRaises(nx.HasACycle, causal_dag.add_edge, "C", "A")
 
     def test_empty_casual_dag(self):
         """Test whether an empty dag can be created."""
         causal_dag = CausalDAG()
         assert list(causal_dag.graph.nodes) == [] and list(causal_dag.graph.edges) == []
 
+    def test_to_dot_string(self):
+        causal_dag = CausalDAG(self.dag_dot_path)
+        self.assertEqual(causal_dag.to_dot_string(), """digraph G {\nA -> B;\nB -> C;\nD -> A;\nD -> C;\n}""")
+
     def tearDown(self) -> None:
         remove_temp_dir_if_existent()
 
 
 class TestCyclicCausalDAG(unittest.TestCase):
     """
     Test the creation of a cyclic causal graph.
```

### Comparing `causal_testing_framework-3.2.0/tests/specification_tests/test_metamorphic_relations.py` & `causal_testing_framework-4.0.0/tests/specification_tests/test_metamorphic_relations.py`

 * *Files 10% similar despite different names*

```diff
@@ -95,24 +95,70 @@
             (u, v) = edge
             adj_set = list(causal_dag.direct_effect_adjustment_sets([u], [v])[0])
             should_cause_MR = ShouldCause(u, v, adj_set, causal_dag)
             should_cause_MR.generate_follow_up(10, -10.0, 10.0, 1)
             test_results = should_cause_MR.execute_tests(self.data_collector)
             should_cause_MR.test_oracle(test_results)
 
+    def test_should_not_cause_json_stub(self):
+        """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program
+        and there is only a single input."""
+        causal_dag = CausalDAG(self.dag_dot_path)
+        self.data_collector = SingleInputProgramUnderTestEDC(
+            self.scenario, self.default_control_input_config, self.default_treatment_input_config
+        )
+        causal_dag.graph.remove_nodes_from(["X2", "X3"])
+        adj_set = list(causal_dag.direct_effect_adjustment_sets(["X1"], ["Z"])[0])
+        should_not_cause_MR = ShouldNotCause("X1", "Z", adj_set, causal_dag)
+        self.assertEqual(
+            should_not_cause_MR.to_json_stub(),
+            {
+                "effect": "direct",
+                "estimate_type": "coefficient",
+                "estimator": "LinearRegressionEstimator",
+                "expected_effect": {"Z": "NoEffect"},
+                "mutations": ["X1"],
+                "name": "X1 _||_ Z",
+                "skip": True,
+            },
+        )
+
+    def test_should_cause_json_stub(self):
+        """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program
+        and there is only a single input."""
+        causal_dag = CausalDAG(self.dag_dot_path)
+        self.data_collector = SingleInputProgramUnderTestEDC(
+            self.scenario, self.default_control_input_config, self.default_treatment_input_config
+        )
+        causal_dag.graph.remove_nodes_from(["X2", "X3"])
+        adj_set = list(causal_dag.direct_effect_adjustment_sets(["X1"], ["Z"])[0])
+        should_cause_MR = ShouldCause("X1", "Z", adj_set, causal_dag)
+        self.assertEqual(
+            should_cause_MR.to_json_stub(),
+            {
+                "effect": "direct",
+                "estimate_type": "coefficient",
+                "estimator": "LinearRegressionEstimator",
+                "expected_effect": {"Z": "SomeEffect"},
+                "mutations": ["X1"],
+                "name": "X1 --> Z",
+                "skip": True,
+            },
+        )
+
     def test_should_cause_metamorphic_relations_correct_spec_one_input(self):
         """Test if the ShouldCause MR passes all metamorphic tests where the DAG perfectly represents the program
         and there is only a single input."""
         causal_dag = CausalDAG(self.dag_dot_path)
         self.data_collector = SingleInputProgramUnderTestEDC(
             self.scenario, self.default_control_input_config, self.default_treatment_input_config
         )
-        causal_dag.graph.remove_nodes_from(['X2', 'X3'])
-        adj_set = list(causal_dag.direct_effect_adjustment_sets(['X1'], ['Z'])[0])
-        should_cause_MR = ShouldCause('X1', 'Z', adj_set, causal_dag)
+        causal_dag.graph.remove_nodes_from(["X2", "X3"])
+        adj_set = list(causal_dag.direct_effect_adjustment_sets(["X1"], ["Z"])[0])
+        should_cause_MR = ShouldCause("X1", "Z", adj_set, causal_dag)
         should_cause_MR.generate_follow_up(10, -10.0, 10.0, 1)
         test_results = should_cause_MR.execute_tests(self.data_collector)
         should_cause_MR.test_oracle(test_results)
 
     def test_should_not_cause_metamorphic_relations_correct_spec(self):
         """Test if the ShouldNotCause MR passes all metamorphic tests where the DAG perfectly represents the program."""
         causal_dag = CausalDAG(self.dag_dot_path)
```

### Comparing `causal_testing_framework-3.2.0/tests/specification_tests/test_variable.py` & `causal_testing_framework-4.0.0/tests/specification_tests/test_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,14 @@
     def test_typestring(self):
         class Var(Variable):
             pass
 
         var = Var("v", int)
         self.assertEqual(var.typestring(), "Var")
 
-
     def test_copy(self):
         ip = Input("ip", float, norm)
         self.assertTrue(ip.copy() is not ip)
         self.assertEqual(ip.copy().name, ip.name)
         self.assertEqual(ip.copy().datatype, ip.datatype)
         self.assertEqual(ip.copy().distribution, ip.distribution)
         self.assertEqual(repr(ip), repr(ip.copy()))
@@ -169,15 +168,15 @@
     def test_ne(self):
         self.assertEqual(str(self.i1 != 5), "i1 != 5")
 
     def test_neg(self):
         self.assertEqual(str(-self.i1), "-i1")
 
     def test_pow(self):
-        self.assertEqual(str(self.i1 ** 5), "i1**5")
+        self.assertEqual(str(self.i1**5), "i1**5")
 
     def test_le(self):
         self.assertEqual(str(self.i1 <= 5), "i1 <= 5")
 
     def test_mul(self):
         self.assertEqual(str(self.i1 * 2), "i1*2")
```

### Comparing `causal_testing_framework-3.2.0/tests/test_helpers.py` & `causal_testing_framework-4.0.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_case.py` & `causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,28 @@
 import unittest
 import os
 from tests.test_helpers import create_temp_dir_if_non_existent, remove_temp_dir_if_existent
-from causal_testing.specification.causal_specification import CausalSpecification, Scenario
 from causal_testing.specification.variable import Input, Output
-from causal_testing.specification.causal_dag import CausalDAG
 from causal_testing.testing.causal_test_case import CausalTestCase
 from causal_testing.testing.causal_test_outcome import ExactValue
 from causal_testing.testing.base_test_case import BaseTestCase
 
 
-class TestCausalTestEngineObservational(unittest.TestCase):
-    """Test the CausalTestEngine workflow using observational data.
+class TestCausalTestCase(unittest.TestCase):
+    """Test the CausalTestCase class.
 
-    The causal test engine (CTE) is the main workflow for the causal testing framework. The CTE takes a causal test case
-    and a causal specification and computes the causal effect of the intervention on the outcome of interest.
+    The base test case is a data class which contains the minimum information
+    necessary to perform identification. The CausalTestCase class represents
+    a causal test case. We here test the basic getter methods.
     """
 
     def setUp(self) -> None:
-        # 1. Create Causal DAG
-        temp_dir_path = create_temp_dir_if_non_existent()
-        dag_dot_path = os.path.join(temp_dir_path, "dag.dot")
-        dag_dot = """digraph G { A -> C; D -> A; D -> C}"""
-        f = open(dag_dot_path, "w")
-        f.write(dag_dot)
-        f.close()
-        self.causal_dag = CausalDAG(dag_dot_path)
-
         # 2. Create Scenario and Causal Specification
         A = Input("A", float)
         C = Output("C", float)
-        D = Output("D", float)
-        self.scenario = Scenario({A, C, D})
-        self.causal_specification = CausalSpecification(scenario=self.scenario, causal_dag=self.causal_dag)
 
         # 3. Create an intervention and causal test case
         self.expected_causal_effect = ExactValue(4)
         self.base_test_case = BaseTestCase(A, C)
         self.causal_test_case = CausalTestCase(
             base_test_case=self.base_test_case,
             expected_causal_effect=self.expected_causal_effect,
```

### Comparing `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_engine.py` & `causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,14 +174,30 @@
             minimal_adjustment_set,
             "C",
             causal_test_engine.scenario_execution_data_df,
         )
         causal_test_result = causal_test_engine.execute_test(estimation_model, causal_test_case)
         self.assertAlmostEqual(causal_test_result.test_value.value, 4, delta=1e-10)
 
+    def test_execute_test_observational_linear_regression_estimator_coefficient(self):
+        """Check that executing the causal test case returns the correct results for dummy data using a linear
+        regression estimator."""
+        estimation_model = LinearRegressionEstimator(
+            "D",
+            self.treatment_value,
+            self.control_value,
+            self.minimal_adjustment_set,
+            "A",
+            self.causal_test_engine.scenario_execution_data_df,
+        )
+        causal_test_result = self.causal_test_engine.execute_test(
+            estimation_model, self.causal_test_case, estimate_type="coefficient"
+        )
+        self.assertEqual(int(causal_test_result.test_value.value), 0)
+
     def test_execute_test_observational_linear_regression_estimator_risk_ratio(self):
         """Check that executing the causal test case returns the correct results for dummy data using a linear
         regression estimator."""
         estimation_model = LinearRegressionEstimator(
             "D",
             self.treatment_value,
             self.control_value,
```

### Comparing `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_outcome.py` & `causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_outcome.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/testing_tests/test_causal_test_suite.py` & `causal_testing_framework-4.0.0/tests/testing_tests/test_causal_test_suite.py`

 * *Files identical despite different names*

### Comparing `causal_testing_framework-3.2.0/tests/testing_tests/test_estimators.py` & `causal_testing_framework-4.0.0/tests/testing_tests/test_estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,23 +162,39 @@
         cls.df = pd.DataFrame({"Z": Z, "X": X, "Y": Y})
 
     def test_estimate_coefficient(self):
         """
         Test we get the correct coefficient.
         """
         iv_estimator = InstrumentalVariableEstimator(
+            df=self.df,
             treatment="X",
             treatment_value=None,
             control_value=None,
             adjustment_set=set(),
             outcome="Y",
             instrument="Z",
+        )
+        self.assertEqual(iv_estimator.estimate_coefficient(self.df), 2)
+
+    def test_estimate_unit_ate(self):
+        """
+        Test we get the correct coefficient.
+        """
+        iv_estimator = InstrumentalVariableEstimator(
             df=self.df,
+            treatment="X",
+            treatment_value=None,
+            control_value=None,
+            adjustment_set=set(),
+            outcome="Y",
+            instrument="Z",
         )
-        self.assertEqual(iv_estimator.estimate_coefficient(), 2)
+        unit_ate, [low, high] = iv_estimator.estimate_unit_ate()
+        self.assertEqual(unit_ate, 2)
 
 
 class TestLinearRegressionEstimator(unittest.TestCase):
     """Test the linear regression estimator against the programming exercises in Section 2 of Hernán and Robins [1].
 
     Reference: Hernán MA, Robins JM (2020). Causal Inference: What If. Boca Raton: Chapman & Hall/CRC.
     Link: https://www.hsph.harvard.edu/miguel-hernan/causal-inference-book/
@@ -188,43 +204,43 @@
     def setUpClass(cls) -> None:
         cls.nhefs_df = load_nhefs_df()
         cls.chapter_11_df = load_chapter_11_df()
 
     def test_program_11_2(self):
         """Test whether our linear regression implementation produces the same results as program 11.2 (p. 141)."""
         df = self.chapter_11_df
-        linear_regression_estimator = LinearRegressionEstimator("treatments", 100, 90, set(), "outcomes", df)
+        linear_regression_estimator = LinearRegressionEstimator("treatments", None, None, set(), "outcomes", df)
         model = linear_regression_estimator._run_linear_regression()
         ate, _ = linear_regression_estimator.estimate_unit_ate()
 
         print(model.summary())
         self.assertEqual(round(model.params["Intercept"] + 90 * model.params["treatments"], 1), 216.9)
 
         # Increasing treatments from 90 to 100 should be the same as 10 times the unit ATE
-        self.assertEqual(round(10 * model.params["treatments"], 1), round(ate, 1))
+        self.assertEqual(round(model.params["treatments"], 1), round(ate, 1))
 
     def test_program_11_3(self):
         """Test whether our linear regression implementation produces the same results as program 11.3 (p. 144)."""
         df = self.chapter_11_df.copy()
         linear_regression_estimator = LinearRegressionEstimator(
-            "treatments", 100, 90, set(), "outcomes", df, formula="outcomes ~ treatments + np.power(treatments, 2)"
+            "treatments", None, None, set(), "outcomes", df, formula="outcomes ~ treatments + np.power(treatments, 2)"
         )
         model = linear_regression_estimator._run_linear_regression()
         ate, _ = linear_regression_estimator.estimate_unit_ate()
         self.assertEqual(
             round(
                 model.params["Intercept"]
                 + 90 * model.params["treatments"]
                 + 90 * 90 * model.params["np.power(treatments, 2)"],
                 1,
             ),
             197.1,
         )
         # Increasing treatments from 90 to 100 should be the same as 10 times the unit ATE
-        self.assertEqual(round(10 * model.params["treatments"], 3), round(ate, 3))
+        self.assertEqual(round(model.params["treatments"], 3), round(ate, 3))
 
     def test_program_15_1A(self):
         """Test whether our linear regression implementation produces the same results as program 15.1 (p. 163, 184)."""
         df = self.nhefs_df
         covariates = {
             "sex",
             "race",
```

