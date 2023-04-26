# Comparing `tmp/biosimulators_test_suite-0.1.87.tar.gz` & `tmp/biosimulators_test_suite-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biosimulators_test_suite-0.1.87.tar", last modified: Wed Apr 26 00:30:58 2023, max compression
+gzip compressed data, was "dist/biosimulators_test_suite-0.1.9.tar", last modified: Sat Jan  2 23:29:07 2021, max compression
```

## Comparing `biosimulators_test_suite-0.1.87.tar` & `biosimulators_test_suite-0.1.9.tar`

### file list

```diff
@@ -1,52 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.779111 biosimulators_test_suite-0.1.87/
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/LICENSE-DATA
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4993 2023-04-26 00:30:58.779111 biosimulators_test_suite-0.1.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3723 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     4173 2023-04-26 00:30:51.000000 biosimulators_test_suite-0.1.87/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.771111 biosimulators_test_suite-0.1.87/biosimulators_test_suite/
--rw-r--r--   0 runner    (1001) docker     (122)       70 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    13734 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6048 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/exec_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    22250 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/exec_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    30815 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/exec_gh_action.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.775111 biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      946 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/io.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.779111 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8789 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     9481 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/combine_archive.py
--rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/docker_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     7798 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/log.py
--rw-r--r--   0 runner    (1001) docker     (122)    61057 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/published_project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4405 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/results_report.py
--rw-r--r--   0 runner    (1001) docker     (122)    98444 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/sedml.py
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      878 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.775111 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4993 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1532 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-04-26 00:30:58.000000 biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/requirements.optional.txt
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-04-26 00:30:58.779111 biosimulators_test_suite-0.1.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1964 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 00:30:58.779111 biosimulators_test_suite-0.1.87/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4505 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_data_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     8454 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (122)     8708 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_exec_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)    15604 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_exec_core.py
--rw-r--r--   0 runner    (1001) docker     (122)    63248 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_exec_gh_action.py
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-04-26 00:28:57.000000 biosimulators_test_suite-0.1.87/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      135 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     5697 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4160 2021-01-02 23:29:03.000000 biosimulators_test_suite-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/
+-rw-r--r--   0 runner    (1001) docker     (116)       70 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       22 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)      395 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4498 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)      783 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4150 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/exec_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14928 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/exec_core.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19675 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/exec_gh_action.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4496 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (116)      670 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/io.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7123 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3389 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/combine_archive.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5941 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4485 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/exec_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (116)    46032 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/published_project.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3329 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/results_report.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29668 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/sedml.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1539 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      876 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     5697 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1303 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      131 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/requirements.optional.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      109 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2021-01-02 23:29:07.000000 biosimulators_test_suite-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1964 2021-01-02 23:27:51.000000 biosimulators_test_suite-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `biosimulators_test_suite-0.1.87/LICENSE` & `biosimulators_test_suite-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `biosimulators_test_suite-0.1.87/PKG-INFO` & `biosimulators_test_suite-0.1.9/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,74 @@
-Metadata-Version: 2.1
-Name: biosimulators_test_suite
-Version: 0.1.87
-Summary: Tools for validating that biosimulation tools are consistent with the BioSimulators standards
-Home-page: https://github.com/biosimulators/Biosimulators_test_suite
-Download-URL: https://github.com/biosimulators/Biosimulators_test_suite
-Author: Center for Reproducible Biomedical Modeling
-Author-email: info@biosimulators.org
-License: MIT
-Keywords: systems biology modeling simulation BioSimulators
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides-Extra: logging
-Provides-Extra: tests
-Provides-Extra: docs
-Provides-Extra: all
-License-File: LICENSE
-License-File: LICENSE-DATA
-
-|Latest release| |PyPI| |CI status| |Test coverage| |All Contributors|
+|Latest release| |PyPI| |CI status| |Test coverage|
 
 BioSimulators test suite
 ========================
 
 The BioSimulators test suite is a tool for validating that biosimulation
-software tools implement the `BioSimulators conventions for
-biosimulation
-tools <https://docs.biosimulations.org/concepts/conventions/>`__.
+software tools implement the `BioSimulators standards for biosimulation
+tools <https://biosimulators.org/standards>`__.
 
 The test suite is composed of two parts:
 
--  `A collection of example modeling projects <examples>`__. Each
-   project is represented by a single `COMBINE/OMEX
+-  A collection of example modeling projects. Each project is
+   represented by a single `COMBINE/OMEX
    archive <https://combinearchive.org/>`__ that contains one or more
    simulation experiments described using the `Simulation Experiment
    Description Markup Language (SED-ML) <https://sed-ml.org>`__ and one
    or more models described using a format such as the `BioNetGen
    Language (BNGL) <https://bionetgen.org>`__ or the `Systems Biology
    Markup Language (SBML) <http://sbml.org>`__.
 
 -  Software for checking that biosimulation tools execute these projects
-   according to the BioSimulators conventions.
+   according to the BioSimulators standards.
 
    -  Simulation tools support the `BioSimulators standard command-line
-      arguments <https://docs.biosimulations.org/concepts/conventions/simulator-interfaces/>`__.
+      arguments <https://biosimulators.org/standards/simulator-interfaces>`__.
    -  Simulation tools support the `BioSimulators conventions for Docker
-      images <https://docs.biosimulations.org/concepts/conventions/simulator-images/>`__.
+      images <https://biosimulators.org/standards/simulator-images>`__.
    -  Simulation tools follow the `BioSimulators conventions for
       executing simulations described by SED-ML files in COMBINE/OMEX
-      archives <https://docs.biosimulations.org/concepts/conventions/simulation-experiments/>`__.
+      archives <https://biosimulators.org/standards/simulation-experiments>`__.
    -  Simulation tools support the `BioSimulators conventions for the
       outputs of SED-ML files in COMBINE/OMEX
-      archives <https://docs.biosimulations.org/concepts/conventions/simulation-run-reports/>`__.
+      archives <https://biosimulators.org/standards/simulation-reports>`__.
+
+Contents
+--------
+
+-  `Installation instructions, tutorial, and API
+   documentation <#installation-instructions,-tutorial,-and-API-documentation>`__
+-  `License <#license>`__
+-  `Development team <#development-team>`__
+-  `Contributing to the test suite <#contributing-to-the-test-suite>`__
+-  `Acknowledgements <#acknowledgements>`__
+-  `Questions and comments <#questions-and-comments>`__
 
 Installation instructions, tutorial, and API documentation
 ----------------------------------------------------------
 
 Installation instructions, tutorial, and API documentation are available
-`here <https://docs.biosimulators.org/Biosimulators_test_suite/>`__.
+`here <https://biosimulators.github.io/Biosimulators_test_suite/>`__.
 
 License
 -------
 
 The software in this package is released under the `MIT
 License <LICENSE>`__. The modeling projects in this package are released
 under the `Creative Commons 1.0 Universal (CC0)
 license <LICENSE-DATA>`__.
 
 Development team
 ----------------
 
 This package was developed by the `Karr Lab <https://www.karrlab.org>`__
 at the Icahn School of Medicine at Mount Sinai in New York, the
-`https://health.uconn.edu/cell-analysis-modeling/ <https://health.uconn.edu/cell-analysis-modeling/>`__
-at the University of Connecticut, and the `Center for Reproducible
-Biomedical Modeling <http://reproduciblebiomodels.org>`__ with
-assistance from the contributors listed `here <CONTRIBUTORS.md>`__.
+https://health.uconn.edu/cell-analysis-modeling/ at the University of
+Connecticut, and the `Center for Reproducible Biomedical
+Modeling <http://reproduciblebiomodels.org>`__.
 
 Contributing to the test suite
 ------------------------------
 
 We enthusiastically welcome contributions to the test suite! Please see
 the `guide to contributing <CONTRIBUTING.md>`__ and the `developer's
 code of conduct <CODE_OF_CONDUCT.md>`__.
@@ -101,9 +89,7 @@
    :target: https://github.com/biosimulators/Biosimulators_test_suite/releases
 .. |PyPI| image:: https://img.shields.io/pypi/v/Biosimulators-test-suite
    :target: https://pypi.org/project/Biosimulators-test-suite/
 .. |CI status| image:: https://github.com/biosimulators/Biosimulators_test_suite/workflows/Continuous%20integration/badge.svg
    :target: https://github.com/biosimulators/Biosimulators_test_suite/actions?query=workflow%3A%22Continuous+integration%22
 .. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_test_suite/branch/dev/graph/badge.svg
    :target: https://codecov.io/gh/biosimulators/Biosimulators_test_suite
-.. |All Contributors| image:: https://img.shields.io/github/all-contributors/biosimulators/Biosimulators_test_suite/HEAD
-   :target: #contributors-
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/data_model.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/data_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,24 +2,23 @@
 
 :Author: Jonathan Karr <karr@mssm.edu>
 :Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
-from .config import Config
 from .exceptions import SkippedTestCaseException  # noqa: F401
 from biosimulators_utils.image import get_docker_image
 import abc
 import docker
 import enum
 
 __all__ = [
     'OutputMedium',
-    'TestCase', 'SedTaskRequirements', 'ExpectedSedReport', 'ExpectedSedDataSet', 'ExpectedSedPlot',
+    'TestCase', 'SedTaskRequirements', 'ExpectedSedReport', 'ExpectedSedPlot',
     'AlertType',
 ]
 
 
 class OutputMedium(str, enum.Enum):
     """ Output medium """
     console = 'console'
@@ -46,113 +45,82 @@
         """
         self.id = id
         self.name = name
         self.description = description
         self.output_medium = output_medium
 
     @abc.abstractmethod
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`, optional): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`SkippedTestCaseException`: if the test case is not applicable to the simulator
             :obj:`Exception`: if the simulator did not pass the test case
         """
         pass  # pragma: no cover
 
-    def get_simulator_docker_image(self, specifications, pull=None):
+    def get_simulator_docker_image(self, specifications, pull=True):
         """ Get the Docker image for a simulator, pulling if necessary
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
 
         Returns:
             :obj:`docker.models.images.Image`: Docker image
         """
         docker_client = docker.from_env()
         image_url = specifications['image']['url']
-        if pull is None:
-            pull = Config().pull_docker_image
         return get_docker_image(docker_client, image_url, pull=pull)
 
 
 class SedTaskRequirements(object):
     """ Required model format for simulation algorithm for each task in a SED document
 
     Attributes:
         model_format (:obj:`str`): EDAM id for the format of the model involved in the task
-        model_format_features (:obj:`set` of :obj:`str`): model format features required to execute the task
-                such as SBML packages
         simulation_algorithm (:obj:`str`): KiSAO id for the simulation algorithm involved in the task
     """
 
-    def __init__(self, model_format=None, model_format_features=None, simulation_algorithm=None):
+    def __init__(self, model_format=None, simulation_algorithm=None):
         """
         Args:
             model_format (:obj:`str`, optional): EDAM id for the format of the model involved in the task
-            model_format_features (:obj:`set` of :obj:`str`, optional): model format features required to execute the task
-                such as SBML packages
             simulation_algorithm (:obj:`str`, optional): KiSAO id for the simulation algorithm involved in the task
         """
         self.model_format = model_format
-        self.model_format_features = model_format_features or set()
         self.simulation_algorithm = simulation_algorithm
 
 
 class ExpectedSedReport(object):
     """ An expected SED report
 
     Attributes
         id (:obj:`str`): id
-        data_sets (:obj:`list` of :obj:`ExpectedSedDataSet`): labels of expected data sets
+        data_sets (:obj:`list` of :obj:`str`): ids of expected datasets
         points (:obj:`tuple` of :obj:`int`): number of expected points of
-        values (:obj:`dict` of :obj:`str` to :obj:`dict` of :obj:`list`): expected values of data sets or elements of data sets
+        values (:obj:`dict` of :obj:`str` to :obj:`dict` of :obj:`list`): expected values of datasets or elements of datasets
     """
 
     def __init__(self, id=None, data_sets=None, points=None, values=None):
         """
         Args:
             id (:obj:`str`, optional): id
-            data_sets (:obj:`set` of :obj:`ExpectedSedDataSet`, optional): labels of expected data sets
+            data_sets (:obj:`set` of :obj:`str`, optional): ids of expected datasets
             points (:obj:`tuple` of :obj:`int`, optional): number of expected points of
-            values (:obj:`dict` of :obj:`str` to :obj:`dict` of :obj:`list`, optional): expected values of data sets or elements of data sets
+            values (:obj:`dict` of :obj:`str` to :obj:`dict` of :obj:`list`, optional): expected values of datasets or elements of datasets
         """
         self.id = id
         self.data_sets = data_sets or set()
         self.points = points
         self.values = values
 
 
-class ExpectedSedDataSet(object):
-    """ An expected SED report
-
-    Attributes
-        id (:obj:`str`): id
-        label (:obj:`str`): label
-    """
-
-    def __init__(self, id=None, label=None):
-        """
-        Args:
-            id (:obj:`str`): id
-            label (:obj:`str`): label
-        """
-        self.id = id
-        self.label = label
-
-
 class ExpectedSedPlot(object):
     """ An expected SED report
 
     Attributes
         id (:obj:`str`): id
     """
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/exceptions.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/warnings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-""" Common exceptions for test cases
+""" Common warnings for test cases
 
 :Author: Jonathan Karr <karr@mssm.edu>
 :Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
 __all__ = [
-    'TestCaseException',
-    'InvalidOutputsException',
-    'SkippedTestCaseException',
-    'TimeoutException',
+    'TestCaseWarning',
+    'IgnoredTestCaseWarning',
+    'SimulatorRuntimeErrorWarning',
+    'InvalidOuputsWarning',
 ]
 
 
-class TestCaseException(Exception):
-    """ Exception raised when outputs of execution of COMBINE/OMEX archive are not as expected """
-    pass  # pragma: no cover
+class TestCaseWarning(UserWarning):
+    """ Base class for warnings collected from test cases """
+    pass
 
 
-class InvalidOutputsException(TestCaseException):
-    """ Exception raised when outputs of execution of COMBINE/OMEX archive are not as expected """
-    pass  # pragma: no cover
+class SimulatorRuntimeErrorWarning(TestCaseWarning, RuntimeWarning):
+    """ Warning that the execution of a test case failed """
+    pass  # pragma: no co
 
 
-class SkippedTestCaseException(TestCaseException):
-    """ Exception raised that indicates that a test case should be skipped """
+class IgnoredTestCaseWarning(TestCaseWarning):
+    """ Warning that a test case was ignored """
     pass  # pragma: no cover
 
 
-class TimeoutException(TestCaseException):
-    """ Exception raised that indicates that a test case timed out """
+class InvalidOuputsWarning(TestCaseWarning):
+    """ Warning that the outputs of the execution of a COMBINE/OMEX archive were not as expected """
     pass  # pragma: no cover
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/exec_core.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/exec_core.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,98 +2,68 @@
 
 :Author: Jonathan Karr <karr@mssm.edu>
 :Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
-from .config import Config
+from .config import TERMINAL_COLORS
 from .data_model import TestCase, OutputMedium
-from .exceptions import SkippedTestCaseException, TimeoutException
+from .exceptions import SkippedTestCaseException
 from .results.data_model import TestCaseResult, TestCaseResultType
 from .test_case import cli
 from .test_case import combine_archive
 from .test_case import docker_image
-from .test_case import log
+from .test_case import exec_status_report
 from .test_case import published_project
 from .test_case import results_report
 from .test_case import sedml
 from .warnings import TestCaseWarning, IgnoredTestCaseWarning
-from biosimulators_utils.config import Colors
-from biosimulators_utils.log.utils import StandardOutputErrorCapturer
 import biosimulators_utils.simulator.io
+import capturer
 import collections
-import contextlib
 import datetime
 import inspect
-import os
-import shutil
-import signal
 import sys
-import tempfile
 import termcolor
-import traceback
 import warnings
 
 __all__ = ['SimulatorValidator']
 
 
 class SimulatorValidator(object):
     """ Validate that a Docker image for a simulator implements the BioSimulations simulator interface by
     checking that the image produces the correct outputs for one of more test cases (e.g., COMBINE archive)
 
     Attributes:
         specifications (:obj:`str` or :obj:`dict`): path or URL to the specifications of the simulator, or the specifications of the simulator
         cases (:obj:`collections.OrderedDict` of :obj:`types.ModuleType` to :obj:`TestCase`): groups of test cases
         verbose (:obj:`bool`): if :obj:`True`, display stdout/stderr from executing cases in real time
-        synthetic_archives_dir (:obj:`str`): Directory to save the synthetic COMBINE/OMEX archives generated by the test cases
         output_medium (:obj:`OutputMedium`): environment where outputs will be sent
-        log_std_out_err (:obj:`bool`): whether to log the standard output and error generated by each test case
-        working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-        dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-        cli (:obj:`str`): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-            archives rather than a Docker image
     """
 
-    def __init__(self, specifications, case_ids=None, verbose=False, synthetic_archives_dir=None, output_medium=OutputMedium.console,
-                 log_std_out_err=True, working_dirname=None, dry_run=False, cli=None, validate_specs=True):
+    def __init__(self, specifications, case_ids=None, verbose=False, output_medium=OutputMedium.console):
         """
         Args:
             specifications (:obj:`str` or :obj:`dict`): path or URL to the specifications of the simulator, or the specifications of the simulator
             case_ids (:obj:`list` of :obj:`str`, optional): List of ids of test cases to verify. If :obj:`ids`
                 is none, all test cases are verified.
             verbose (:obj:`bool`, optional): if :obj:`True`, display stdout/stderr from executing cases in real time
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives generated by the test cases
             output_medium (:obj:`OutputMedium`, optional): environment where outputs will be sent
-            log_std_out_err (:obj:`bool`, optional): whether to log the standard output and error generated by each test case
-            working_dirname (:obj:`str`, optional): directory for temporary files for evaluating test case
-            dry_run (:obj:`bool`, optional): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
-            validate_specs (:obj:`bool`, optional): whether to validate specifications
         """
         # if necessary, get and validate specifications of simulator
         if isinstance(specifications, str):
-            specifications = biosimulators_utils.simulator.io.read_simulator_specs(specifications, validate=validate_specs)
+            specifications = biosimulators_utils.simulator.io.read_simulator_specs(specifications)
 
         self.specifications = specifications
         self.verbose = verbose
-        if synthetic_archives_dir and not os.path.isdir(synthetic_archives_dir):
-            os.makedirs(synthetic_archives_dir)
-        self.synthetic_archives_dir = synthetic_archives_dir
         self.output_medium = output_medium
-        self.log_std_out_err = log_std_out_err
-        self.working_dirname = working_dirname
-        self.dry_run = dry_run
-        self.cli = cli
 
         self.cases = self.find_cases(ids=case_ids)
 
-        self.test_case_timeout = Config().test_case_timeout
-
     def find_cases(self, ids=None):
         """ Find test cases
 
         Args:
             ids (:obj:`list` of :obj:`str`, optional): List of ids of test cases to verify. If :obj:`ids`
                 is none, all test cases are verified.
 
@@ -123,28 +93,23 @@
         cases[suite_name] = self.find_cases_in_module(sedml, compatible_published_projects_test_cases, ids=ids)
 
         # get cases for reports of simulation results
         suite_name = results_report.__name__.replace('biosimulators_test_suite.test_case.', '')
         cases[suite_name] = self.find_cases_in_module(results_report, compatible_published_projects_test_cases, ids=ids)
 
         # get cases for reporting status of the execution of modeling projects
-        suite_name = log.__name__.replace('biosimulators_test_suite.test_case.', '')
-        cases[suite_name] = self.find_cases_in_module(log, compatible_published_projects_test_cases, ids=ids)
+        suite_name = exec_status_report.__name__.replace('biosimulators_test_suite.test_case.', '')
+        cases[suite_name] = self.find_cases_in_module(exec_status_report, compatible_published_projects_test_cases, ids=ids)
 
         # add cases involving published COMBINE/OMEX archives
         suite_name = published_project.__name__.replace('biosimulators_test_suite.test_case.', '')
         cases[suite_name] = []
         for case in all_published_projects_test_cases:
-            if ids is None:
+            if ids is None or case.id in ids:
                 cases[suite_name].append(case)
-            else:
-                for id in ids:
-                    if id in case.id:
-                        cases[suite_name].append(case)
-                        break
 
         # warn if desired cases weren't found
         if ids is not None:
             found_case_ids = set()
             for suite_cases in cases.values():
                 for case in suite_cases:
                     found_case_ids.add(case.id)
@@ -170,56 +135,38 @@
             :obj:`list` of :obj:`TestCase`: test cases
         """
         cases = []
         ignored_ids = []
         module_name = module.__name__.replace('biosimulators_test_suite.test_case.', '')
         for child_name in dir(module):
             child = getattr(module, child_name)
-            if (
-                getattr(child, '__module__', None) == module.__name__
-                and isinstance(child, type)
-                and issubclass(child, TestCase)
-                and not inspect.isabstract(child)
-            ):
-                case_id = module_name + '.' + child_name
-
-                if ids is None:
-                    use_case = True
-                else:
-                    use_case = False
-                    for id in ids:
-                        if id in case_id:
-                            use_case = True
-                            break
-
-                if use_case:
+            if isinstance(child, type) and issubclass(child, TestCase) and not inspect.isabstract(child):
+                id = module_name + '.' + child_name
+                if ids is None or id in ids:
                     description = child.__doc__ or None
                     if description:
                         description_lines = (description
                                              .replace('\r', '')
                                              .replace('\n    ', '\n')
                                              .partition('\n\n')[0]
                                              .strip()
                                              .split('\n'))
                         description = ' '.join(line.strip() for line in description_lines) or None
                     if issubclass(child, published_project.SyntheticCombineArchiveTestCase):
-                        case = child(id=case_id, description=description, output_medium=self.output_medium,
+                        case = child(id=id, description=description, output_medium=self.output_medium,
                                      published_projects_test_cases=published_projects_test_cases)
                     else:
-                        case = child(id=case_id, description=description, output_medium=self.output_medium)
+                        case = child(id=id, description=description, output_medium=self.output_medium)
                     cases.append(case)
-
                 else:
-                    ignored_ids.append(case_id)
+                    ignored_ids.append(id)
 
         if ignored_ids:
             warnings.warn('Some test case(s) were ignored:\n  {}'.format('\n  '.join(sorted(ignored_ids))), IgnoredTestCaseWarning)
 
-        cases.sort(key=lambda case: case.id)
-
         return cases
 
     def run(self):
         """ Validate that a Docker image for a simulator implements the BioSimulations simulator interface by
         checking that the image produces the correct outputs for test cases (e.g., COMBINE archive)
 
         Returns:
@@ -232,265 +179,157 @@
         print('Collected {} test cases.'.format(n_cases))
 
         # get start time
         start = datetime.datetime.now()
 
         # execute test cases and collect results
         results = []
-        working_dirname = self.working_dirname or tempfile.mkdtemp()
         for suite_name, suite_cases in self.cases.items():
             print('\nExecuting {} {} tests ... {}'.format(len(suite_cases), suite_name, 'done' if not suite_cases else ''))
             for i_case, case in enumerate(suite_cases):
                 print('  {}: {} ... '.format(i_case + 1, case.id), end='')
                 sys.stdout.flush()
 
-                result = self.eval_case(case, os.path.join(working_dirname, suite_name, case.id))
+                result = self.eval_case(case)
                 results.append(result)
 
-                print(termcolor.colored(result.type.value, Colors[result.type.value].value), end='')
+                print(termcolor.colored(result.type.value, TERMINAL_COLORS[result.type.value]), end='')
                 print(' (', end='')
                 if result.warnings:
-                    print(termcolor.colored(str(len(result.warnings)) + ' warnings, ', Colors.warned.value), end='')
+                    print(termcolor.colored(str(len(result.warnings)) + ' warnings, ', TERMINAL_COLORS['warned']), end='')
                 print('{:.1f} s'.format(result.duration), end='')
                 print(').')
 
-        if self.working_dirname is None:
-            shutil.rmtree(working_dirname)
-
         # get total duration
         duration = (datetime.datetime.now() - start).total_seconds()
 
         # print completion message
         print('\n{} tests completed in {:.1f} s'.format(n_cases, duration))
 
         # return results
         return results
 
-    def eval_case(self, case, working_dirname):
+    def eval_case(self, case):
         """ Evaluate a test case for a simulator
 
         Args:
             case (:obj:`TestCase`): test case
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
 
         Returns:
             :obj:`TestCaseResult`: test case result
         """
         start_time = datetime.datetime.now()
 
-        with StandardOutputErrorCapturer(relay=self.verbose, disabled=not self.log_std_out_err) as captured:
+        with capturer.CaptureOutput(merged=True, relay=self.verbose) as captured:
             with warnings.catch_warnings(record=True) as caught_warnings:
                 warnings.simplefilter("ignore")
                 warnings.simplefilter("always", TestCaseWarning)
 
                 try:
-
-                    with time_limit(seconds=self.test_case_timeout):
-                        case.eval(self.specifications,
-                                  working_dirname,
-                                  synthetic_archives_dir=self.synthetic_archives_dir,
-                                  dry_run=self.dry_run,
-                                  cli=self.cli)
+                    case.eval(self.specifications)
                     type = TestCaseResultType.passed
                     exception = None
-                    exception_traceback = None
                     skip_reason = None
 
                 except SkippedTestCaseException as caught_exception:
                     type = TestCaseResultType.skipped
                     exception = None
-                    exception_traceback = None
                     skip_reason = caught_exception
 
                 except Exception as caught_exception:
                     type = TestCaseResultType.failed
                     exception = caught_exception
-                    exception_traceback = sys.exc_info()[2]
                     skip_reason = None
 
                 duration = (datetime.datetime.now() - start_time).total_seconds()
 
                 return TestCaseResult(
                     case=case,
                     type=type,
                     duration=duration,
                     exception=exception,
-                    exception_traceback=exception_traceback,
                     warnings=caught_warnings,
                     skip_reason=skip_reason,
                     log=captured.get_text())
 
     @staticmethod
-    def summarize_results(results, debug=False, output_medium=OutputMedium.console):
+    def summarize_results(results):
         """ Get a summary of the results of a set of test cases
 
         Args:
             results (:obj:`list` :obj:`TestCaseResult`): results of executing test cases
-            debug (:obj:`bool`, optional): whether to display traceback information about each error with
-                additional information for debugging
-            output_medium (:obj:`OutputMedium`, optional): environment where outputs will be sent
 
         Returns:
             :obj:`tuple`
 
                 * :obj:`str`: summary of results of test cases
                 * :obj:`list` of :obj:`str`: details of failures
                 * :obj:`list` of :obj:`str`: details of warnings
-                * :obj:`list` of :obj:`str`: details of skips
         """
         passed = []
         failed = []
         skipped = []
         warning_details = []
         failure_details = []
-        skipped_details = []
         for result in sorted(results, key=lambda result: result.case.id):
             if result.type == TestCaseResultType.passed:
                 result_str = '  * `{}`\n'.format(result.case.id)
                 passed.append(result_str)
 
             elif result.type == TestCaseResultType.failed:
                 result_str = '  * `{}`\n'.format(result.case.id)
                 failed.append(result_str)
 
                 detail = ''
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '<details><summary><b><code>{}</code> ({:.1f} s)</b></summary>\n<br/>\n'.format(result.case.id, result.duration)
-                else:
-                    detail += '`{}` ({:.1f} s)\n'.format(result.case.id, result.duration)
+                detail += '`{}` ({:.1f} s)\n'.format(result.case.id, result.duration)
                 detail += '\n'
                 if result.case.description:
                     detail += '  {}\n'.format(result.case.description.replace('\n', '\n  '))
                     detail += '\n'
-
                 detail += '  Exception:\n'
                 detail += '\n'
                 detail += '  ```\n'
                 detail += '  {}\n'.format(str(result.exception).replace('\n', '\n  '))
-                if debug and result.exception_traceback:
-                    detail += '\n'
-                    detail += '  {}\n'.format('\n'.join(traceback.format_tb(result.exception_traceback)).replace('\n', '\n  '))
                 detail += '  ```\n'
                 detail += '\n'
-
-                if result.log:
-                    detail += '  Log:\n'
-                    detail += '\n'
-                    detail += '  ```\n'
-                    detail += '  {}\n'.format(result.log.replace('\n', '\n  '))
-                    detail += '  ```'
-                else:
-                    detail += '  Log: None'
-
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '\n</details>'
-
+                detail += '  Log:\n'
+                detail += '\n'
+                detail += '  ```\n'
+                detail += '  {}\n'.format(result.log.replace('\n', '\n  ') if result.log else '')
+                detail += '  ```'
                 failure_details.append(detail)
 
             elif result.type == TestCaseResultType.skipped:
                 result_str = '  * `{}`\n'.format(result.case.id)
                 skipped.append(result_str)
 
-                detail = ''
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '<details><summary><b><code>{}</code> ({:.1f} s)</b></summary>\n<br/>\n'.format(result.case.id, result.duration)
-                else:
-                    detail += '`{}` ({:.1f} s)\n'.format(result.case.id, result.duration)
-                detail += '\n'
-                if result.case.description:
-                    detail += '  {}\n'.format(result.case.description.replace('\n', '\n  '))
-                    detail += '\n'
-
-                detail += '  Reason for skip:\n'
-                detail += '\n'
-                detail += '  ```\n'
-                detail += '  {}\n'.format(str(result.skip_reason).replace('\n', '\n  '))
-                detail += '  ```\n'
-                detail += '\n'
-
-                if result.warnings:
-                    detail += '  Warnings:\n'
-                    for warning in result.warnings:
-                        detail += '\n'
-                        detail += '  ```\n'
-                        detail += '  {}\n'.format(str(warning.message).replace('\n', '\n  '))
-                        detail += '  ```\n'
-                    detail += '\n'
-
-                if result.log:
-                    detail += '  Log:\n'
-                    detail += '\n'
-                    detail += '  ```\n'
-                    detail += '  {}\n'.format(result.log.replace('\n', '\n  '))
-                    detail += '  ```'
-                else:
-                    detail += '  Log: None\n'
-
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '\n</details>'
-
-                skipped_details.append(detail)
-
             if result.warnings:
                 detail = ''
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '<details><summary><b><code>{}</code> ({:.1f} s)</b></summary>\n<br/>\n'.format(result.case.id, result.duration)
-                else:
-                    detail += '`{}` ({:.1f} s)\n'.format(result.case.id, result.duration)
+                detail += '`{}` ({:.1f} s)\n'.format(result.case.id, result.duration)
                 detail += '\n'
                 if result.case.description:
                     detail += '  {}\n'.format(result.case.description.replace('\n', '\n  '))
                     detail += '\n'
-
                 detail += '  Warnings:\n'
                 for warning in result.warnings:
                     detail += '\n'
                     detail += '  ```\n'
                     detail += '  {}\n'.format(str(warning.message).replace('\n', '\n  '))
                     detail += '  ```\n'
                 detail += '\n'
-
-                if result.log:
-                    detail += '  Log:\n'
-                    detail += '\n'
-                    detail += '  ```\n'
-                    detail += '  {}\n'.format(result.log.replace('\n', '\n  '))
-                    detail += '  ```'
-                else:
-                    detail += '  Log: None'
-
-                if output_medium == OutputMedium.gh_issue:
-                    detail += '\n</details>'
-
+                detail += '  Log:\n'
+                detail += '\n'
+                detail += '  ```\n'
+                detail += '  {}\n'.format(result.log.replace('\n', '\n  ') if result.log else '')
+                detail += '  ```'
                 warning_details.append(detail)
 
         return (
             '\n'.join([
                 '* Executed {} test cases\n'.format(len(results)),
                 '* Passed {} test cases{}\n{}'.format(len(passed), ':' if passed else '', ''.join(passed)),
                 '* Failed {} test cases{}\n{}'.format(len(failed), ':' if failed else '', ''.join(failed)),
                 '* Skipped {} test cases{}\n{}'.format(len(skipped), ':' if skipped else '', ''.join(skipped)),
             ]).strip(),
             failure_details,
             warning_details,
-            skipped_details,
         )
-
-
-@contextlib.contextmanager
-def time_limit(seconds):
-    """ Context manager for timing out long operations
-
-    Args:
-        seconds (:obj:`int`): length in seconds before time out
-
-    Raises:
-        :obj:`TimeoutException`: if the operation timed out
-    """
-    def signal_handler(signum, frame):
-        raise TimeoutException("Operation did not complete within {} seconds".format(seconds))
-    signal.signal(signal.SIGALRM, signal_handler)
-    signal.alarm(int(seconds))
-    try:
-        yield
-    finally:
-        signal.alarm(0)
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/exec_gh_action.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/sedml.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,605 +1,680 @@
-""" Methods for processing submissions to the BioSimulators registry
-(CI workflows for reviewing and committing simulators to the registry)
+""" Methods for testing that simulators support the features of SED-ML
 
 :Author: Jonathan Karr <karr@mssm.edu>
-:Date: 2020-12-06
+:Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
-
-from .config import Config
-from .data_model import OutputMedium
-from .exec_core import SimulatorValidator
-from .results.data_model import TestCaseResult, TestCaseResultType, TestResultsReport  # noqa: F401
-from .results.io import write_test_results
-from .utils import get_singularity_image_filename
-from biosimulators_utils.biosimulations.utils import validate_biosimulations_api_response
-from biosimulators_utils.config import Colors, Config as BioSimulatorsUtilsConfig
-from biosimulators_utils.gh_action.data_model import Comment, GitHubActionCaughtError  # noqa: F401
-from biosimulators_utils.gh_action.core import GitHubAction, GitHubActionErrorHandling
-from biosimulators_utils.image import get_docker_image
-from biosimulators_utils.simulator_registry.data_model import SimulatorSubmission, IssueLabel  # noqa: F401
-from biosimulators_utils.simulator_registry.process_submission import get_simulator_submission_from_gh_issue_body
-from biosimulators_utils.simulator_registry.query import get_simulator_version_specs
-from natsort import natsort_keygen
-import biosimulators_utils.image
-import biosimulators_utils.simulator.io
-import requests
-import requests.exceptions
-import termcolor
-
+from ..exceptions import InvalidOuputsException
+from ..warnings import InvalidOuputsWarning
+from .published_project import SingleMasterSedDocumentCombineArchiveTestCase, UniformTimeCourseTestCase
+from biosimulators_utils.combine.data_model import CombineArchive  # noqa: F401
+from biosimulators_utils.archive.io import ArchiveReader
+from biosimulators_utils.config import get_config
+from biosimulators_utils.report.io import ReportReader
+from biosimulators_utils.sedml.data_model import (SedDocument, Output, Report, Plot2D, Plot3D,  DataGenerator,  # noqa: F401
+                                                  DataGeneratorVariable, UniformTimeCourseSimulation,
+                                                  DataSet, Curve, Surface, AxisScale,
+                                                  Model, ModelAttributeChange, AlgorithmParameterChange)
+import abc
+import copy
+import numpy
+import os
+import PyPDF2
+import shutil
+import tempfile
+import warnings
 
 __all__ = [
-    'ValidateCommitSimulatorGitHubAction',
+    'SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports',
+    'SimulatorSupportsModelAttributeChanges',
+    'SimulatorSupportsAlgorithmParameters',
+    'SimulatorProducesReportsWithCuratedNumberOfDimensions',
+    'SimulatorSupportsMultipleTasksPerSedDocument',
+    'SimulatorSupportsMultipleReportsPerSedDocument',
+    'SimulatorSupportsUniformTimeCoursesWithNonZeroOutputStartTimes',
+    'SimulatorSupportsUniformTimeCoursesWithNonZeroInitialTimes',
+    'SimulatorProducesLinear2DPlots',
+    'SimulatorProducesLogarithmic2DPlots',
+    'SimulatorProducesLinear3DPlots',
+    'SimulatorProducesLogarithmic3DPlots',
+    'SimulatorProducesMultiplePlots',
 ]
 
 
-def get_uncaught_exception_msg(exception):
-    """ Create an error message to display to users for all exceptions not caught during the
-    exception of the :obj:`run` method (exceptions of all types except :obj:`GitHubActionCaughtError`)
+class SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports(SingleMasterSedDocumentCombineArchiveTestCase):
+    """ Test that a simulator supports the core elements of SED: models, simulations, tasks, data generators for
+    individual variables, and reports
+    """
 
-    Args:
-        exception (:obj:`Exception`): a failure encountered during the exception of the :obj:`run` method
+    def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
+        """ Test that the expected outputs were created for the synthetic archive
 
-    Returns:
-        :obj:`str`: error message to display to users
-    """
-    gh_action_run_url = GitHubAction.get_gh_action_run_url()
-    return [
-        Comment(text='The validation/submission of your simulator failed.'),
-        Comment(text=str(exception), error=True),
-        Comment(text=('The complete log of your validation/submission job, including further information about the failure, '
-                      + 'is available for 90 days [here]({}).'.format(gh_action_run_url))),
-        Comment(text=('If you chose to validate your Docker image, the results of the validation of your image will be '
-                      'available shortly as a JSON file. A link to this file will be available for 90 days from the "Artifacts" '
-                      'section at the bottom of [this page]({}).'.format(gh_action_run_url))),
-        Comment(text='Once you have fixed the problem, edit the first block of this issue to re-initiate this validation.'),
-        Comment(text=('The BioSimulators Team is happy to help. '
-                      'Questions and feedback can be directed to the BioSimulators Team by posting comments to this issues that '
-                      'reference the GitHub team `@biosimulators/biosimulators` (without the backticks).')),
-    ]
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
+            synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
+                document in the synthetic archive to the document
+            outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
+
+        Returns:
+            :obj:`bool`: :obj:`True`, if succeeded without warnings
+        """
+        has_warnings = False
 
+        # reports
+        try:
+            report_ids = ReportReader().get_ids(outputs_dir)
+        except Exception:
+            report_ids = []
+
+        expected_report_ids = set()
+        for doc_location, doc in synthetic_sed_docs.items():
+            doc_id = os.path.relpath(doc_location, './')
+            for output in doc.outputs:
+                if isinstance(output, Report):
+                    expected_report_ids.add(os.path.join(doc_id, output.id))
+
+        missing_report_ids = expected_report_ids.difference(set(report_ids))
+        extra_report_ids = set(report_ids).difference(expected_report_ids)
+
+        if missing_report_ids:
+            raise InvalidOuputsException('Simulator did not produce the following reports:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in missing_report_ids))
+            ))
+
+        if extra_report_ids:
+            msg = 'Simulator produced extra reports:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in extra_report_ids)))
+            warnings.warn(msg, InvalidOuputsWarning)
+            has_warnings = True
+
+        # data sets
+        expected_data_set_labels = set()
+        data_set_labels = set()
+        for doc_location, doc in synthetic_sed_docs.items():
+            doc_id = os.path.relpath(doc_location, './')
+            for output in doc.outputs:
+                if isinstance(output, Report):
+                    for data_set in output.data_sets:
+                        expected_data_set_labels.add(os.path.join(doc_id, output.id, data_set.label))
+
+                    results = ReportReader().run(outputs_dir, os.path.join(doc_id, output.id))
+                    data_set_labels.update(set(os.path.join(doc_id, output.id, label) for label in results.index))
+
+        missing_data_set_labels = expected_data_set_labels.difference(set(data_set_labels))
+        extra_data_set_labels = set(data_set_labels).difference(expected_data_set_labels)
+
+        if missing_data_set_labels:
+            raise InvalidOuputsException('Simulator did not produce the following data sets:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + label + '`' for label in missing_data_set_labels))
+            ))
+
+        if extra_data_set_labels:
+            msg = 'Simulator produced extra data sets:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + label + '`' for label in extra_data_set_labels)))
+            warnings.warn(msg, InvalidOuputsWarning)
+            has_warnings = True
 
-class ValidateCommitSimulatorGitHubAction(GitHubAction):
-    """ Action to validate a containerized simulator
+        return not has_warnings
 
-    Attributes:
-        issue_number (:obj:`str`): number of GitHub issue which triggered the action
+
+class SimulatorSupportsModelAttributeChanges(SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports):
+    """ Test that a simulator supports changes to the attributes of model elements
     """
 
-    def __init__(self):
-        super(ValidateCommitSimulatorGitHubAction, self).__init__()
-        self.config = Config()
-        self.issue_number = self.get_issue_number()
-
-    @GitHubActionErrorHandling.catch_errors(uncaught_exception_msg_func=get_uncaught_exception_msg,
-                                            caught_error_labels=[IssueLabel.invalid],
-                                            uncaught_error_labels=[IssueLabel.invalid])
-    def run(self):
-        """ Validate and commit a simulator."""
-
-        # Get properties of submission
-        issue_props = self.get_issue(self.issue_number)
-        submission = get_simulator_submission_from_gh_issue_body(issue_props['body'])
-        submitter = issue_props['user']['login']
-
-        # Send message that validation is starting
-        self.add_comment_to_issue(self.issue_number, self.get_initial_message(submission, submitter))
-
-        # reset labels except approved
-        self.reset_issue_labels(self.issue_number, [IssueLabel.validated.value, IssueLabel.invalid.value, IssueLabel.action_error.value])
-
-        # get specifications of simulator and validate simulator
-        specifications, test_results = self.exec_core(submission, submitter)
-
-        # label issue as validated
-        self.add_labels_to_issue(self.issue_number, [IssueLabel.validated.value])
-
-        # get specifications of other versions of simulator
-        config = BioSimulatorsUtilsConfig()
-        existing_version_specifications = get_simulator_version_specs(specifications['id'], config)
-
-        # determine if simulator is approved: issue is a revision of an existing version of a validated simulator,
-        # a new version of a validated simulator, or the issue has been manually approved by the BioSimulators Team
-        approved = self.is_simulator_approved(specifications, existing_version_specifications)
-
-        # if approved, label the issue as approved
-        if approved and IssueLabel.approved.value not in self.get_labels_for_issue(self.issue_number):
-            self.add_labels_to_issue(self.issue_number, [IssueLabel.approved.value])
-
-        # commit simulator or indicate that further review is required
-        if submission.commit_simulator:
-            if approved:
-                self.commit_simulator(submission, specifications, existing_version_specifications, test_results)
-
-                # post success message
-                self.add_comment_to_issue(
-                    self.issue_number,
-                    ''.join([
-                        'Your submission was committed to the BioSimulators registry. Thank you!\n',
-                        '\n',
-                        'Future submissions of subsequent versions of {} to the BioSimulators registry '.format(specifications['id']),
-                        'will be automatically validated. These submissions will not require manual review by the BioSimulators Team.',
-                    ])
-                )
+    def __init__(self, *args, **kwargs):
+        super(SimulatorSupportsModelAttributeChanges, self).__init__(*args, **kwargs)
+        self._types_of_model_changes_to_keep = (ModelAttributeChange,)
 
-                # close issue
-                self.close_issue(self.issue_number)
-            else:
-                assigned = set([assignee['login'] for assignee in issue_props['assignees']])
-                new_assignees = set(self.config.biosimulators_curator_gh_ids).difference(assigned)
-                if new_assignees:
-                    self.assign_issue(self.issue_number,  list(new_assignees))
-                self.add_comment_to_issue(
-                    self.issue_number,
-                    ('A member of the BioSimulators team will review your submission and '
-                     'publish your image before final committment to the registry.'))
-
-    def get_initial_message(self, submission, submitter):
-        """ Peport message that validation is starting
-
-        Args:
-            submission (:obj:`SimulatorSubmission`): simulator submission
-            submitter (:obj:`str`): GitHub user name of person who executed the submission
-        """
-        actions = []
-        not_actions = []
-
-        actions.append('validating the specifications of your simulator')
-        if submission.validate_image:
-            actions.append('validating your Docker image')
-            test_results_msg = (
-                ' The results of the validation of your tool will also be saved as a JSON file. '
-                'A link to this file will be available for 90 days from the "Artifacts" section at the bottom of this page.'
-            )
-        else:
-            not_actions.append('You have chosen not to have the Docker image for your simulator validated.')
-            test_results_msg = ''
-        if submission.commit_simulator:
-            job_type = 'submission'
-            actions.append('committing your simulator to the BioSimulators registry')
-        else:
-            job_type = 'validation'
-            not_actions.append('You have chosen not to submit your simulator to the BioSimulators registry.')
+    def is_curated_sed_model_suitable_for_building_synthetic_archive(self, specifications, model):
+        """ Determine if a SED model is suitable for testing
 
-        if len(actions) == 1:
-            actions = actions[0]
-        else:
-            actions = ', '.join(actions[0:-1]) + ', and ' + actions[-1]
-        not_actions = ' '.join(action.strip() for action in not_actions)
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            model (:obj:`Model`): SED task in curated archive
+
+        Returns:
+            :obj:`bool`: whether the model is suitable for testing
+        """
+        return next((True for change in model.changes if isinstance(change, ModelAttributeChange)), False)
 
-        return ('Thank you @{} for your submission to the BioSimulators simulator validation/submission system!\n\n'
-                'The BioSimulators validator bot is {}. {}\n\n'
-                'We will discuss any concerns with your submission in this issue.\n\n'
-                'A complete log of your simulator {} job will be available for 90 days [here]({}).{}\n\n'
-                ).format(submitter, actions, not_actions, job_type, self.get_gh_action_run_url(), test_results_msg)
 
-    def exec_core(self, submission, submitter):
-        """ Validate simulator
+class SimulatorSupportsAlgorithmParameters(SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports):
+    """ Test that a simulator supports setting the values of parameters of algorithms """
 
-        * Validate specifications
-        * Validate image
+    def is_curated_sed_algorithm_suitable_for_building_synthetic_archive(self, specifications, algorithm):
+        """ Determine if a SED algorithm is suitable for testing
 
         Args:
-            submission (:obj:`SimulatorSubmission`): simulator submission
-            submitter (:obj:`str`): GitHub id of the submitter
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            algorithm (:obj:`Algorithm`): SED algorithm in curated archive
 
         Returns:
-            :obj:`tuple`:
-
-                * :obj:`dict`: specifications of a simulation tool
-                * :obj:`list` of :obj:`TestCaseResults`: results of test cases
+            :obj:`bool`: whether the algorithm is suitable for testing
         """
-        # validate specifications
-        specifications = biosimulators_utils.simulator.io.read_simulator_specs(
-            submission.specifications_url, submission.specifications_patch,
-            validate=True)
-
-        # check permissions
-        self.validate_permissions(specifications['id'], specifications['name'], submitter)
-
-        # indicate that specifications are valid
-        self.add_comment_to_issue(self.issue_number, 'The specifications of your simulator is valid!')
-
-        # validate image
-        if submission.validate_image:
-            test_results = self.validate_image(specifications)
-            self.add_comment_to_issue(self.issue_number, 'The image for your simulator is valid!')
-        else:
-            test_results = None
+        for alg_specs in specifications['algorithms']:
+            if alg_specs['kisaoId']['id'] == algorithm.kisao_id:
+                for param_spec in alg_specs['parameters']:
+                    if param_spec['value'] is not None:
+                        return True
 
-        # return specifications
-        return specifications, test_results
+        return False
 
-    def validate_permissions(self, simulator_id, simulator_name, submitter):
-        """ Validate that the submitter has permissions to submit or update the simulator
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+        """ Generate a synthetic archive with a copy of each task and each report
 
         Args:
-            simulator_id (:obj:`str`): simulator id
-            simulator_name (:obj:`str`): simulator name
-            submitter (:obj:`str`): GitHub id of the submitter
-        """
-        # check if team exists
-        response = requests.get(
-            'https://api.github.com/orgs/biosimulators/teams/' + simulator_id,
-            auth=self.get_gh_auth())
-        try:
-            response.raise_for_status()
-            has_team = True
-        except requests.exceptions.HTTPError:
-            if response.status_code == 404:
-                has_team = False
-            else:
-                raise
-
-        # create team if none exists and add submitter as a maintainer of the team
-        if not has_team:
-            # get parent team
-            response = requests.get(
-                'https://api.github.com/orgs/biosimulators/teams/simulator-developers',
-                auth=self.get_gh_auth())
-            response.raise_for_status()
-            base_team_id = response.json()['id']
-
-            # create team
-            response = requests.post(
-                'https://api.github.com/orgs/biosimulators/teams',
-                auth=self.get_gh_auth(), json={
-                    'name': simulator_id,
-                    'description': 'Developers of ' + simulator_name,
-                    'parent_team_id': base_team_id,
-                    'maintainers': [submitter],
-                })
-            response.raise_for_status()
-
-            # tell user a group was created
-            msg = (
-                'We created the GitHub group @biosimulators/{} to manage permissions to change the specifications of {} '
-                'and added you (@{}) to this group. You can manage permissions to change the specifications of {} at '
-                'https://github.com/orgs/biosimulators/teams/{}/members.'
-            ).format(simulator_id, simulator_name, submitter, simulator_name, simulator_id)
-            self.add_comment_to_issue(self.issue_number, msg)
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
+            curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
+            curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
+                SED documents in curated archive
 
-        # check submitter has permissions to team
-        else:
-            response = requests.get(
-                'https://api.github.com/orgs/biosimulators/teams/{}/memberships/{}'.format(simulator_id, submitter),
-                auth=self.get_gh_auth())
-            try:
-                response.raise_for_status()
-                has_permissions = True
-            except requests.exceptions.HTTPError:
-                if response.status_code == 404:
-                    has_permissions = False
-                else:
-                    raise
-
-            if not has_permissions:
-                msg = (
-                    'You (@{}) do not have permissions to update the specifications of {}. Only the members of @biosimulators/{} '
-                    'can update the specifications of {}. Please contact the members of this group to request permissions to update {}.'
-                ).format(submitter, simulator_name, simulator_id, simulator_name, simulator_name)
-                self.add_error_comment_to_issue(self.issue_number, [Comment(text=msg, error=True)])
-
-    def validate_image(self, specifications):
-        """ Validate a Docker image for simulation tool
-
-        Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-
-        Returns:
-            :obj:`list` of :obj:`TestCaseResults`: results of test cases
-        """
-        docker_client = biosimulators_utils.image.login_to_docker_registry(
-            'docker.io', self.config.docker_hub_username, self.config.docker_hub_token)
-
-        # validate that container (Docker image) exists
-        image_url = specifications['image']['url']
-        get_docker_image(docker_client, image_url, pull=True)
-
-        # validate that Docker image can be converted to a Singularity image
-        biosimulators_utils.image.convert_docker_image_to_singularity(
-            image_url,
-            singularity_filename=get_singularity_image_filename(image_url))
-
-        # validate that image is consistent with the BioSimulators standards
-        validator = SimulatorValidator(specifications, output_medium=OutputMedium.gh_issue)
-        case_results = validator.run()
-        write_test_results(case_results, '.biosimulators-test-suite-results.json',
-                           gh_issue=int(self.issue_number), gh_action_run=int(self.get_gh_action_run_id()))
-        summary, failure_details, warning_details, skipped_details = validator.summarize_results(
-            case_results, output_medium=OutputMedium.gh_issue)
-
-        # print summary to console
-        print('')
-        print('=============== SUMMARY ===============')
-        print('')
-        print(summary + '\n\n')
-        if failure_details:
-            color = Colors.failure.value
-            print(termcolor.colored('=============== FAILURES ===============', color))
-            print(termcolor.colored('', color))
-            print(termcolor.colored('* ' + '\n\n* '.join(failure_details), color))
-            print('')
-        if warning_details:
-            color = Colors.warning.value
-            print(termcolor.colored('=============== WARNINGS ===============', color))
-            print(termcolor.colored('', color))
-            print(termcolor.colored('* ' + '\n\n* '.join(warning_details), color))
-            print('')
-        if skipped_details:
-            color = Colors.skipped.value
-            print(termcolor.colored('================ SKIPS =================', color))
-            print(termcolor.colored('', color))
-            print(termcolor.colored('* ' + '\n\n* '.join(skipped_details), color))
-            print('')
-
-        # push summary to comments on GitHub issue
-        unable_to_post_results_msg = (
-            'The summary of the tests of your Docker image could not be posted to this GitHub issue. '
-            'The most likely reason is that the summary is too long to post to a comment on a GitHub issue. '
-            'Please use the [console log]({}) of the associated GitHub Action to see the summary of the tests of your '
-            'Docker image.'
-        ).format(self.get_gh_action_run_url())
-
-        msg = '## Summary of tests\n\n{}\n\n'.format(summary)
-        self.add_comment_to_issue(self.issue_number, msg, alternative_comment=unable_to_post_results_msg)
-
-        if failure_details:
-            msg = '\n## Failures\n\n{}\n\n'.format('\n\n'.join(failure_details))
-            self.add_comment_to_issue(self.issue_number, msg, alternative_comment=unable_to_post_results_msg)
-
-        if warning_details:
-            msg = '\n## Warnings\n\n{}\n\n'.format('\n\n'.join(warning_details))
-            self.add_comment_to_issue(self.issue_number, msg, alternative_comment=unable_to_post_results_msg)
-
-        if skipped_details:
-            msg = '\n## Skips\n\n{}\n\n'.format('\n\n'.join(skipped_details))
-            self.add_comment_to_issue(self.issue_number, msg, alternative_comment=unable_to_post_results_msg)
-
-        invalid_cases = [case_result for case_result in case_results if case_result.type == TestCaseResultType.failed]
-        if invalid_cases:
-            gh_action_run_url = self.get_gh_action_run_url()
-            error_msg = (
-                'After correcting your simulator, please edit the first block of this issue to re-initiate this validation.\n\n'
-                'The complete log of your validation/submission job, including further information about the failure, '
-                'is available for 90 days [here]({}). The results of the validation of your image will also be '
-                'available shortly as a JSON file. A link to this file will be available from the "Artifacts" '
-                'section at the bottom of [this page]({}).'
-            ).format(gh_action_run_url, gh_action_run_url)
-
-            self.add_error_comment_to_issue(self.issue_number, [Comment(text=error_msg, error=True)])
-
-        valid_cases = [case_result for case_result in case_results
-                       if case_result.type == TestCaseResultType.passed and case_result.case.id.startswith('sedml.')]
-        if not valid_cases:
-            self.add_error_comment_to_issue(self.issue_number, [Comment(text=(
-                'No test cases are applicable to your simulator. '
-                'Please use this issue to share appropriate test COMBINE/OMEX files. '
-                'The BioSimulators Team will add these files to this validation program and then re-review your simulator.'
-            ))])
-
-        return case_results
-
-    def is_simulator_approved(self, specifications, existing_version_specifications):
-        """ Determine whether a simulation tool has already been approved
-
-        Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
-
-        Returns:
-            :obj:`bool`: :obj:`True`, if the simulation tool has already been approved
-        """
-        return (self.does_submission_have_approved_label()
-                or self.is_other_version_of_simulator_validated(specifications, existing_version_specifications))
+        Returns:
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
+        """
+        curated_archive, curated_sed_docs = super(SimulatorSupportsAlgorithmParameters, self).build_synthetic_archive(
+            specifications, curated_archive, curated_archive_dir, curated_sed_docs)
+
+        # set algorithm parameters
+        doc = list(curated_sed_docs.values())[0]
+
+        algorithm = doc.simulations[0].algorithm
+
+        for alg_specs in specifications['algorithms']:
+            if alg_specs['kisaoId']['id'] == algorithm.kisao_id:
+                if alg_specs['parameters']:
+                    break
+
+        algorithm.changes = []
+        for param_spec in alg_specs['parameters']:
+            if param_spec['value'] is not None:
+                algorithm.changes.append(
+                    AlgorithmParameterChange(
+                        kisao_id=param_spec['kisaoId']['id'],
+                        new_value=param_spec['value'],
+                    )
+                )
 
-    def does_submission_have_approved_label(self):
-        """ Determine whether an issue for submitting a simulator already has the approved label
+        return (curated_archive, curated_sed_docs)
+
+
+class SimulatorProducesReportsWithCuratedNumberOfDimensions(SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports):
+    """ Test that that the curated number of output dimensions matches the actual number of output dimensions
+    """
+
+    def is_curated_sed_algorithm_suitable_for_building_synthetic_archive(self, specifications, algorithm):
+        """ Determine if a SED algorithm is suitable for testing
+
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            algorithm (:obj:`Algorithm`): SED algorithm in curated archive
 
         Returns:
-            :obj:`bool`: :obj:`True`, if the issue for the submission already has the approved label
+            :obj:`bool`: whether the algorithm is suitable for testing
         """
-        if IssueLabel.approved.value in self.get_labels_for_issue(self.issue_number):
+        if not (super(SimulatorProducesReportsWithCuratedNumberOfDimensions, self).
+                is_curated_sed_algorithm_suitable_for_building_synthetic_archive(specifications, algorithm)):
+            return False
+
+        for alg_specs in specifications['algorithms']:
+            if alg_specs['kisaoId']['id'] == algorithm.kisao_id:
+                if alg_specs.get('dependentDimensions', None) is not None:
+                    return True
+
+        return False
+
+    def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
+        """ Test that the expected outputs were created for the synthetic archive
+
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
+            synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
+                document in the synthetic archive to the document
+            outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
+        """
+        doc = list(synthetic_sed_docs.values())[0]
+        doc_location = list(synthetic_sed_docs.keys())[0]
+        doc_id = os.path.relpath(doc_location, './')
+
+        report = doc.outputs[0]
+        data = ReportReader().run(outputs_dir, os.path.join(doc_id, report.id))
+
+        for alg_specs in specifications['algorithms']:
+            if alg_specs['kisaoId']['id'] == doc.simulations[0].algorithm.kisao_id:
+                break
+
+        expected_dims = alg_specs['dependentDimensions']
+
+        if numpy.squeeze(data).ndim != 1 + len(expected_dims):
+            msg = ('The specifications for the number of dimensions of each data set of algorithm `{}` differs '
+                   'from the actual number of dimensions, {} != {}.').format(
+                doc.simulations[0].algorithm.kisao_id, data.ndim - 1, len(expected_dims))
+            warnings.warn(msg, InvalidOuputsWarning)
+            return False
+        else:
             return True
 
-    def is_other_version_of_simulator_validated(self, specifications, existing_version_specifications):
-        """ Determine whether another version of the simulation tool has already been approved
+
+class SimulatorSupportsMultipleTasksPerSedDocument(SingleMasterSedDocumentCombineArchiveTestCase):
+    """ Test that a simulator supports multiple tasks per SED document
+
+    Attributes:
+        _expected_reports (:obj:`list` of :obj:`tuple` of :obj:`str`): list of pairs of
+            original reports and their expected duplicates
+    """
+
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+        """ Generate a synthetic archive with a copy of each task and each report
 
         Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
+            curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
+            curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
+                SED documents in curated archive
 
         Returns:
-            :obj:`bool`: :obj:`True`, if the simulation tool has already been approved
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
+        """
+        curated_archive, curated_sed_docs = super(SimulatorSupportsMultipleTasksPerSedDocument, self).build_synthetic_archive(
+            specifications, curated_archive, curated_archive_dir, curated_sed_docs)
+
+        # get a suitable SED document to modify
+        location = list(curated_sed_docs.keys())[0]
+        doc_id = os.path.relpath(location, './')
+        sed_doc = curated_sed_docs[location]
+
+        # duplicate tasks and reports
+        copy_tasks = {}
+        for task in list(sed_doc.tasks):
+            copy_task = copy.copy(task)
+            copy_task.id += '__test_suite_copy'
+            sed_doc.tasks.append(copy_task)
+            copy_tasks[task.id] = copy_task
+
+        self._expected_reports = []
+        copy_data_gens = {}
+        for output in list(sed_doc.outputs):
+            if isinstance(output, Report):
+                copy_output = Report(id=output.id + '__test_suite_copy')
+                sed_doc.outputs.append(copy_output)
+
+                self._expected_reports.append((
+                    os.path.join(doc_id, output.id),
+                    os.path.join(doc_id, copy_output.id)))
+
+                for data_set in output.data_sets:
+                    copy_data_set = DataSet(id=data_set.id + '__test_suite_copy', label=data_set.label)
+                    copy_output.data_sets.append(copy_data_set)
+
+                    data_gen = data_set.data_generator
+                    copy_data_gen_id = data_gen.id + '__test_suite_copy'
+                    copy_data_gen = copy_data_gens.get(copy_data_gen_id, None)
+                    if not copy_data_gen:
+                        copy_data_gen = DataGenerator(id=copy_data_gen_id, parameters=data_gen.parameters, math=data_gen.math)
+                        sed_doc.data_generators.append(copy_data_gen)
+
+                        for var in data_set.data_generator.variables:
+                            copy_var = DataGeneratorVariable(id=var.id, target=var.target, symbol=var.symbol, model=var.model)
+                            copy_var.task = copy_tasks[var.task.id]
+                            copy_data_gen.variables.append(copy_var)
+                    copy_data_set.data_generator = copy_data_gen
+
+        # return modified SED document
+        return (curated_archive, curated_sed_docs)
+
+    def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
+        """ Test that the expected outputs were created for the synthetic archive
+
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
+            synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
+                document in the synthetic archive to the document
+            outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
         """
-        for version_spec in existing_version_specifications:
-            if version_spec.get('biosimulators', {}).get('validated', False):
-                return True
-        return False
+        try:
+            report_ids = ReportReader().get_ids(outputs_dir)
+        except Exception:
+            report_ids = []
+
+        missing_reports = []
+        for report_loc, copy_report_loc in self._expected_reports:
+            if report_loc not in report_ids:
+                missing_reports.append(report_loc)
+            if copy_report_loc not in report_ids:
+                missing_reports.append(copy_report_loc)
+
+        if missing_reports:
+            raise ValueError('Reports for duplicate tasks were not generated:\n  {}'.format(
+                '\n  '.join(sorted(missing_reports))))
+
+
+class SimulatorSupportsMultipleReportsPerSedDocument(SingleMasterSedDocumentCombineArchiveTestCase):
+    """ Test that a simulator supports multiple reports per SED document """
+
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+        """ Generate a synthetic archive with a copy of each task and each report
+
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
+            curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
+            curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
+                SED documents in curated archive
+
+        Returns:
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
+        """
+        curated_archive, curated_sed_docs = super(SimulatorSupportsMultipleReportsPerSedDocument, self).build_synthetic_archive(
+            specifications, curated_archive, curated_archive_dir, curated_sed_docs)
+
+        # get a suitable SED document to modify
+        sed_doc = list(curated_sed_docs.values())[0]
+
+        # divide data sets between two reports
+        original_data_sets = sed_doc.outputs[0].data_sets
+        sed_doc.outputs = [
+            Report(id='report_1'),
+            Report(id='report_2'),
+        ]
+
+        for i_dataset, data_set in enumerate(original_data_sets):
+            sed_doc.outputs[i_dataset % 2].data_sets.append(data_set)
+
+        # to ensure that each report has at least one data set, including when there's only 1 data set total
+        sed_doc.outputs[1].data_sets.append(original_data_sets[0])
+
+        # return modified SED document
+        return (curated_archive, curated_sed_docs)
 
-    def commit_simulator(self, submission, specifications, existing_version_specifications, test_results):
-        """ Commit simulator to the BioSimulators registry
+    def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
+        """ Test that the expected outputs were created for the synthetic archive
 
         Args:
-            submission (:obj:`SimulatorSubmission`): simulator submission
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
-            test_results (:obj:`list` of :obj:`TestCaseResults`): results of test cases
-        """
-        # commit image
-        if submission.validate_image:
-            # copy image to BioSimulators namespace of Docker registry (GitHub Container Registry)
-            self.push_image(specifications, existing_version_specifications)
-
-        # commit submission to BioSimulators database
-        if 'biosimulators' not in specifications:
-            specifications['biosimulators'] = {}
-
-        if submission.validate_image:
-            specifications['biosimulators']['validated'] = True
-            specifications['biosimulators']['validationTests'] = TestResultsReport(
-                results=test_results, gh_issue=int(self.issue_number), gh_action_run=int(self.get_gh_action_run_id()),
-            ).to_dict(max_log_len=2**16)
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
+            synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
+                document in the synthetic archive to the document
+            outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
+        """
+        has_warnings = False
 
-        else:
-            specifications['biosimulators']['validated'] = False
-            specifications['biosimulators']['validationTests'] = None
+        try:
+            report_ids = ReportReader().get_ids(outputs_dir)
+        except Exception:
+            report_ids = []
+
+        doc_location = os.path.relpath(list(synthetic_sed_docs.keys())[0], './')
+        expected_report_ids = set([os.path.join(doc_location, 'report_1'), os.path.join(doc_location, 'report_2')])
 
-        config = BioSimulatorsUtilsConfig(BIOSIMULATORS_API_ENDPOINT=self.config.biosimulators_prod_api_endpoint)
-        self.post_entry_to_biosimulators_api(specifications, existing_version_specifications, self.config.biosimulators_prod_api_endpoint)
+        missing_report_ids = expected_report_ids.difference(set(report_ids))
+        extra_report_ids = set(report_ids).difference(expected_report_ids)
 
-        config = BioSimulatorsUtilsConfig(BIOSIMULATORS_API_ENDPOINT=self.config.biosimulators_dev_api_endpoint)
-        existing_version_specifications = get_simulator_version_specs(specifications['id'], config)
-        self.post_entry_to_biosimulators_api(specifications, existing_version_specifications, self.config.biosimulators_dev_api_endpoint)
+        if missing_report_ids:
+            raise InvalidOuputsException('Simulator did not produce the following reports:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in missing_report_ids))
+            ))
 
-        # commit image
-        if submission.validate_image:
-            # instruct runBioSimulations to generate a Singularity image for the Docker image
-            self.trigger_conversion_of_docker_image_to_singularity(specifications)
+        if extra_report_ids:
+            msg = 'Simulator produced extra reports:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in extra_report_ids)))
+            warnings.warn(msg, InvalidOuputsWarning)
+            has_warnings = True
 
-    def push_image(self, specifications, existing_version_specifications):
-        """ Push the image for a simulation tool to the GitHub Container Registry
+        return not has_warnings
+
+
+class SimulatorSupportsUniformTimeCoursesWithNonZeroOutputStartTimes(UniformTimeCourseTestCase):
+    """ Test that a simulator supports time courses with non-zero output start times """
+
+    def modify_simulation(self, simulation):
+        """ Modify a simulation
 
         Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
+            simulation (:obj:`UniformTimeCourseSimulation`): simulation
         """
-        # get image, pulling if necessary
-        original_image_url = specifications['image']['url']
-        docker_client = biosimulators_utils.image.login_to_docker_registry(
-            'docker.io', self.config.docker_hub_username, self.config.docker_hub_token)
-        image = get_docker_image(docker_client, original_image_url, pull=True)
+        simulation.output_start_time = simulation.output_end_time / 2
+        simulation.number_of_points = int(simulation.number_of_points / 2)
+
 
-        # push image to BioSimulators namespace of Docker registry
-        biosimulators_utils.image.login_to_docker_registry(
-            self.config.biosimulators_docker_registry_url,
-            self.config.biosimulators_docker_registry_username,
-            self.config.biosimulators_docker_registry_token)
+class SimulatorSupportsUniformTimeCoursesWithNonZeroInitialTimes(UniformTimeCourseTestCase):
+    """ Test that a simulator supports multiple time courses with non-zero initial times """
 
-        copy_image_url = self.config.biosimulators_docker_image_url_pattern \
-            .format(specifications['id'], specifications['version']) \
-            .lower()
-        biosimulators_utils.image.tag_and_push_docker_image(docker_client, image, copy_image_url)
-        specifications['image']['url'] = copy_image_url
+    def modify_simulation(self, simulation):
+        """ Modify a simulation
 
-        image = get_docker_image(docker_client, copy_image_url, pull=False)
-        specifications['image']['digest'] = image.attrs['RepoDigests'][0].partition('@')[2]
+        Args:
+            simulation (:obj:`UniformTimeCourseSimulation`): simulation
+        """
+        simulation.initial_time = simulation.output_end_time / 2
+        simulation.output_start_time = simulation.output_end_time / 2
+        simulation.number_of_points = int(simulation.number_of_points / 2)
 
-        is_latest = self.is_submission_latest_version_of_simulator(specifications, existing_version_specifications)
 
-        if is_latest:
-            latest_copy_image_url = self.config.biosimulators_docker_image_url_pattern \
-                .format(specifications['id'], 'latest') \
-                .lower()
-            biosimulators_utils.image.tag_and_push_docker_image(docker_client, image, latest_copy_image_url)
+class SimulatorProducesPlotsTestCase(SingleMasterSedDocumentCombineArchiveTestCase):
+    """ Test that a simulator produces plots """
 
-        # make image public -- must be done manually; cannot be done via API as of 2020-11-11
+    @property
+    def _num_plots(self):
+        return 1
 
-    def is_submission_latest_version_of_simulator(self, specifications, existing_version_specifications):
-        """ Determine whether the submitted version the latest version of the simulator (greatest tag)
+    @property
+    @abc.abstractmethod
+    def _axis_scale(self):
+        pass  # pragma: no cover
+
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+        """ Generate a synthetic archive with a copy of each task and each report
 
         Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
+            curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
+            curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
+                SED documents in curated archive
 
         Returns:
-            :obj:`bool`: :obj:`True` if the submitted version if the latest version of the simulator
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
         """
-        version_comparison_func = natsort_keygen()
-        for existing_version_spec in existing_version_specifications:
-            if (
-                existing_version_spec.get('image', None)
-                and existing_version_spec.get('biosimulators', {}).get('validated', False)
-                and version_comparison_func(existing_version_spec['version']) > version_comparison_func(specifications['version'])
-            ):
-                return False
-        return True
+        curated_archive, curated_sed_docs = super(SimulatorProducesPlotsTestCase, self).build_synthetic_archive(
+            specifications, curated_archive, curated_archive_dir, curated_sed_docs)
+
+        # get a suitable SED document to modify
+        doc = list(curated_sed_docs.values())[0]
+
+        # replace report with plot(s)
+        doc.outputs = self.build_plots(doc.data_generators)
+
+        # return modified SED document
+        return (curated_archive, curated_sed_docs)
 
-    def trigger_conversion_of_docker_image_to_singularity(self, specifications):
-        """ Post the simulation to the BioSimulators database
+    @abc.abstractmethod
+    def build_plots(self, data_generators):
+        """ Build plots from the defined data generators
 
         Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
+            data_generators (:obj:`list` of :obj:`DataGenerator`): data generators
+
+        Returns:
+            :obj:`list` of :obj:`Output`: plots
+        """
+        pass  # pragma: no cover
+
+    def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
+        """ Test that the expected outputs were created for the synthetic archive
+
+        Args:
+            specifications (:obj:`dict`): specifications of the simulator to validate
+            synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
+            synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
+                document in the synthetic archive to the document
+            outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
         """
-        auth_headers = self.get_auth_headers_for_biosimulations_api(
-            self.config.runbiosimulations_auth_endpoint, self.config.runbiosimulations_audience,
-            self.config.runbiosimulations_api_client_id, self.config.runbiosimulations_api_client_secret)
+        plots_path = os.path.join(outputs_dir, get_config().PLOTS_PATH)
+        if not os.path.isfile(plots_path):
+            warnings.warn('Simulator did not produce plots', InvalidOuputsWarning)
+            return
+
+        tempdir = tempfile.mkdtemp()
+        try:
+            archive = ArchiveReader().run(plots_path, tempdir)
+        except Exception:
+            shutil.rmtree(tempdir)
+            raise InvalidOuputsException('Simulator produced an invalid zip archive of plots')
+
+        for file in archive.files:
+            with open(file.local_path, 'rb') as file:
+                try:
+                    PyPDF2.PdfFileReader(file)
+                except Exception:
+                    shutil.rmtree(tempdir)
+                    raise InvalidOuputsException('Simulator produced an invalid PDF plot')
+
+        doc = list(synthetic_sed_docs.values())[0]
+        doc_location = list(synthetic_sed_docs.keys())[0]
+        doc_id = os.path.relpath(doc_location, './')
+
+        expected_plot_ids = set(os.path.join(doc_id, output.id + '.pdf') for output in doc.outputs)
+        plot_ids = set(os.path.relpath(file.archive_path, './') for file in archive.files)
+
+        missing_plot_ids = expected_plot_ids.difference(plot_ids)
+        extra_plot_ids = plot_ids.difference(expected_plot_ids)
+
+        if missing_plot_ids:
+            shutil.rmtree(tempdir)
+            raise InvalidOuputsException('Simulator did not produce the following plots:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in missing_plot_ids))
+            ))
+
+        if extra_plot_ids:
+            msg = 'Simulator produced extra plots:\n  - {}'.format(
+                '\n  - '.join(sorted('`' + id + '`' for id in extra_plot_ids)))
+            warnings.warn(msg, InvalidOuputsWarning)
+
+        shutil.rmtree(tempdir)
 
-        response = requests.post(self.config.runbiosimulations_api_endpoint + 'images/refresh',
-                                 headers=auth_headers,
-                                 json={
-                                     'simulator': specifications['id'],
-                                     'version': specifications['version'],
-                                 })
-        validate_biosimulations_api_response(response, 'A Singularity image could not be generated for the Docker image')
 
-    def post_entry_to_biosimulators_api(self, specifications, existing_version_specifications, biosimulators_api_endpoint):
-        """ Post the simulation to the BioSimulators database
+class SimulatorProduces2DPlotsTestCase(SimulatorProducesPlotsTestCase):
+    """ Test that a simulator produces 2D plots """
+
+    def build_plots(self, data_generators):
+        """ Build plots from the defined data generators
 
         Args:
-            specifications (:obj:`dict`): specifications of a simulation tool
-            existing_version_specifications (:obj:`list` of :obj:`dict`): specifications of other versions of simulation tool
-            biosimulators_api_endpoint (:obj:`str`): endpoint for the BioSimulators API (e.g., ``https://api.biosimulators.org``)
+            data_generators (:obj:`list` of :obj:`DataGenerator`): data generators
+
+        Returns:
+            :obj:`list` of :obj:`Output`: plots
         """
-        auth_headers = self.get_auth_headers_for_biosimulations_api(
-            self.config.biosimulators_auth_endpoint, self.config.biosimulators_audience,
-            self.config.biosimulators_api_client_id, self.config.biosimulators_api_client_secret)
+        plots = []
+        for i in range(self._num_plots):
+            plots.append(Plot2D(id='plot_' + str(i)))
+
+        for i_data_generator, data_generator in enumerate(data_generators):
+            plots[i_data_generator % self._num_plots].curves.append(
+                Curve(
+                    id='curve_' + str(i_data_generator),
+                    x_data_generator=data_generator,
+                    y_data_generator=data_generator,
+                    x_scale=self._axis_scale,
+                    y_scale=self._axis_scale,
+                ),
+            )
 
-        existing_versions = [existing_version_spec['version'] for existing_version_spec in existing_version_specifications]
-        update_simulator = specifications['version'] in existing_versions
-        if update_simulator:
-            endpoint = '{}simulators/{}/{}'.format(biosimulators_api_endpoint, specifications['id'], specifications['version'])
-            requests_method = requests.put
-            method = 'updated'
-        else:
-            endpoint = '{}simulators'.format(biosimulators_api_endpoint)
-            requests_method = requests.post
-            method = 'added'
-        response = requests_method(endpoint, headers=auth_headers, json=specifications)
-        validate_biosimulations_api_response(response, 'Simulation tool `{}` could not be {} to the BioSimulators registry.'.format(
-            specifications['id'], method))
-
-    def get_auth_headers_for_biosimulations_api(self, endpoint, audience, client_id, client_secret):
-        """ Get authorization headers for using one of the BioSimulations REST APIs
-        (BioSimulators, runBioSimulations, etc.).
-
-        Args:
-            endpoint (:obj:`str`): URL for getting an authentication token
-            audience (:obj:`str`): API audience
-            client_id (:obj:`str`): id for this client
-            client_secret (:obj:`str`): secret for this client
-
-        Returns:
-            :obj:`dict`: authorization headers
-        """
-        response = requests.post(endpoint, json={
-            'client_id': client_id,
-            'client_secret': client_secret,
-            'audience': audience,
-            "grant_type": "client_credentials",
-        })
-        response.raise_for_status()
-        response_data = response.json()
-        return {'Authorization': response_data['token_type'] + ' ' + response_data['access_token']}
-
-    @classmethod
-    def add_comment_to_issue(cls, issue_number, comment, alternative_comment=None, max_len=65536):
-        """ Post a comment to the GitHub issue
-
-        Args:
-            issue_number (:obj:`str`): issue number
-            comment (:obj:`str`): comment
-            alternative_comment (:obj:`str`, optional): optional alternative comment to try posting to the GitHub issue
-            max_len (:obj:`int`, optional): maximum comment length accepted by GitHub
+        return plots
+
+
+class SimulatorProduces3DPlotsTestCase(SimulatorProducesPlotsTestCase):
+    """ Test that a simulator produces 3D plots """
+
+    def build_plots(self, data_generators):
+        """ Build plots from the defined data generators
+
+        Args:
+            data_generators (:obj:`list` of :obj:`DataGenerator`): data generators
+
+        Returns:
+            :obj:`list` of :obj:`Output`: plots
         """
-        try:
-            if len(comment) > max_len:
-                comment = comment[0:max_len - 4] + ' ...'
-            super(ValidateCommitSimulatorGitHubAction, cls).add_comment_to_issue(issue_number, comment)
-
-        except (requests.exceptions.RequestException, requests.exceptions.ProxyError, requests.exceptions.SSLError):
-            if alternative_comment:
-                super(ValidateCommitSimulatorGitHubAction, cls).add_comment_to_issue(issue_number, alternative_comment)
-            else:
-                raise
+        plots = []
+        for i in range(self._num_plots):
+            plots.append(Plot3D(id='plot_' + str(i)))
+
+        for i_data_generator, data_generator in enumerate(data_generators):
+            plots[i_data_generator % self._num_plots].surfaces.append(
+                Surface(
+                    id='surface_' + str(i_data_generator),
+                    x_data_generator=data_generator,
+                    y_data_generator=data_generator,
+                    z_data_generator=data_generator,
+                    x_scale=self._axis_scale,
+                    y_scale=self._axis_scale,
+                    z_scale=self._axis_scale,
+                ),
+            )
+
+        return plots
+
+
+class SimulatorProducesLinear2DPlots(SimulatorProduces2DPlotsTestCase):
+    """ Test that a simulator produces linear 2D plots """
+
+    @property
+    def _axis_scale(self):
+        return AxisScale.linear
+
+
+class SimulatorProducesLogarithmic2DPlots(SimulatorProduces2DPlotsTestCase):
+    """ Test that a simulator produces logarithmic 2D plots """
+
+    @property
+    def _axis_scale(self):
+        return AxisScale.log
+
+
+class SimulatorProducesLinear3DPlots(SimulatorProduces3DPlotsTestCase):
+    """ Test that a simulator produces linear 3D plots """
+
+    @property
+    def _axis_scale(self):
+        return AxisScale.linear
+
+
+class SimulatorProducesLogarithmic3DPlots(SimulatorProduces3DPlotsTestCase):
+    """ Test that a simulator produces logarithmic 3D plots """
+
+    @property
+    def _axis_scale(self):
+        return AxisScale.log
+
+
+class SimulatorProducesMultiplePlots(SimulatorProduces2DPlotsTestCase):
+    """ Test that a simulator produces multiple plots """
+
+    @property
+    def _num_plots(self):
+        return 2
+
+    @property
+    def _axis_scale(self):
+        return AxisScale.linear
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/data_model.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/data_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 :Copyright: 2021, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
 from .._version import __version__
 from ..warnings import TestCaseWarning  # noqa: F401
 import enum
-import traceback
 
 __all__ = [
     'TestCaseResultType',
     'TestCaseResult',
     'TestResultsReport',
 ]
 
@@ -29,75 +28,62 @@
     """ A result of executing a test case
 
     Attributes:
         case (:obj:`TestCase`): test case
         type (:obj:`obj:`TestCaseResultType`): type
         duration (:obj:`float`): execution duration in seconds
         exception (:obj:`Exception`): exception
-        exception_traceback (:obj:`str`): traceback
         warnings (:obj:`list` of :obj:`TestCaseWarning`): warnings
         skip_reason (:obj:`Exception`): Exception which explains reason for skip
         log (:obj:`str`): log of execution
     """
 
-    def __init__(self, case=None, type=None, duration=None, exception=None, exception_traceback=None, warnings=None, skip_reason=None, log=None):
+    def __init__(self, case=None, type=None, duration=None, exception=None, warnings=None, skip_reason=None, log=None):
         """
         Args:
             case (:obj:`TestCase`, optional): test case
             type (:obj:`obj:`TestCaseResultType`, optional): type
             duration (:obj:`float`, optional): execution duration in seconds
             exception (:obj:`Exception`, optional): exception
-            exception_traceback (:obj:`str`, optional): traceback
             warnings (:obj:`list` of :obj:`TestCaseWarning`, optional): warnings
             skip_reason (:obj:`Exception`, optional): Exception which explains reason for skip
             log (:obj:`str`, optional): log of execution
         """
         self.case = case
         self.type = type
         self.duration = duration
         self.exception = exception
-        self.exception_traceback = exception_traceback
         self.warnings = warnings or []
         self.skip_reason = skip_reason
         self.log = log
 
-    def to_dict(self, max_log_len=None, debug=True):
+    def to_dict(self):
         """ Generate a dictionary representation e.g., for export to JSON
 
-        Args:
-            max_log_len (:obj:`int`, optional): maximum log length
-            debug (:obj:`bool`, optional): whether to display traceback information about each error
-                with additional information for debugging
-
         Returns:
             :obj:`dict`: dictionary representation
         """
-        log = self.log
-        if max_log_len is not None and log and len(log) > max_log_len:
-            log = log[0:max_log_len - 1] + ' ...'
-
         return {
             'case': {
                 'id': self.case.id,
                 'description': self.case.description,
             },
             'resultType': self.type.value,
             'duration': self.duration,
             'exception': {
                 'category': self.exception.__class__.__name__,
                 'message': str(self.exception),
-                'traceback': traceback.format_tb(self.exception_traceback) if self.exception_traceback else None,
             } if self.exception else None,
             'warnings': [{'category': warning.category.__name__, 'message': str(warning.message)}
                          for warning in self.warnings],
             'skipReason': {
                 'category': self.skip_reason.__class__.__name__,
                 'message': str(self.skip_reason),
             } if self.skip_reason else None,
-            'log': log,
+            'log': self.log,
         }
 
 
 class TestResultsReport(object):
     """ A report of the results of executing the test suite with a simulation tool
 
     Attributes:
@@ -116,22 +102,19 @@
             gh_action_run (:obj:`int`, optional): GitHub action run in which the test suite was executed
         """
         self.test_suite_version = test_suite_version
         self.results = results or []
         self.gh_issue = gh_issue
         self.gh_action_run = gh_action_run
 
-    def to_dict(self, max_log_len=None):
+    def to_dict(self):
         """ Generate a dictionary representation e.g., for export to JSON
 
-        Args:
-            max_log_len (:obj:`int`, optional): maximum log length
-
         Returns:
             :obj:`dict`: dictionary representation
         """
         return {
             'testSuiteVersion': self.test_suite_version,
-            'results': [result.to_dict(max_log_len=max_log_len) for result in self.results],
+            'results': [result.to_dict() for result in self.results],
             'ghIssue': self.gh_issue,
             'ghActionRun': self.gh_action_run,
         }
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/results/io.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/results/io.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,17 @@
 
 from .data_model import TestCaseResult, TestResultsReport  # noqa: F401
 import json
 
 __all__ = ['write_test_results']
 
 
-def write_test_results(results, filename, gh_issue=None, gh_action_run=None):
+def write_test_results(results, filename):
     """ Write the results of test cases to a JSON file
 
     Args:
         results (:obj:`list` of :obj:`TestCaseResult`): results of test cases
         filename (:obj:`str`): path to save results
-        gh_issue (:obj:`int`, optional): GitHub issue for which the test suite was executed
-        gh_action_run (:obj:`int`, optional): GitHub action run in which the test suite was executed
     """
-    report = TestResultsReport(results=results, gh_issue=gh_issue, gh_action_run=gh_action_run)
+    report = TestResultsReport(results=results)
     with open(filename, 'w') as file:
         json.dump(report.to_dict(), file)
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/cli.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,62 +19,57 @@
     'CliDisplaysVersionInformationInline',
 ]
 
 
 class CliDisplaysHelpInline(TestCase):
     """ Test that a command-line interface provides inline help. """
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         self.get_simulator_docker_image(specifications)
         image_url = specifications['image']['url']
 
-        cli = [cli] if cli else ['docker', 'run', '--tty', '--rm', image_url]
-
-        result = subprocess.run(cli, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
         supported = (
             '-i' in log
             and '-o' in log
         )
         if not supported:
             warnings.warn(('Command-line interfaces should display basic help when no arguments are provided.\n\n'
                            'The command-line interface displayed the following when no argument was provided:\n\n  {}'
                            ).format(log.replace('\n', '\n  ')),
                           TestCaseWarning)
 
-        result = subprocess.run(cli + ['-h'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url, '-h'],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
         supported = (
             'arguments' in log
             and '-i' in log
             and '--archive' in log
             and '-o' in log
             and '--out-dir' in log
         )
         if not supported:
             warnings.warn(('Command-line interface should support the `-h` option for displaying help inline.\n\n'
                            'The command-line interface displayed the following when executed with `-h`:\n\n  {}'
                            ).format(log.replace('\n', '\n  ')),
                           TestCaseWarning)
 
-        result = subprocess.run(cli + ['--help'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url, '--help'],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
         supported = (
             'arguments' in log
             and '-i' in log
             and '--archive' in log
             and '-o' in log
             and '--out-dir' in log
@@ -87,34 +82,28 @@
 
 
 class CliDescribesSupportedEnvironmentVariablesInline(TestCase):
     """ Test that the inline help for a command-line interface describes the environment variables that the
     simulator supports.
     """
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         self.get_simulator_docker_image(specifications)
         image_url = specifications['image']['url']
 
-        cli = [cli] if cli else ['docker', 'run', '--tty', '--rm', image_url]
-        result = subprocess.run(cli + ['-h'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url, '-h'],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
 
         potentially_missing_env_vars = []
         for var in ENVIRONMENT_VARIABLES.values():
             if var.name not in log:
                 potentially_missing_env_vars.append(var.name)
 
@@ -130,44 +119,38 @@
                    ).format('\n  - '.join("'" + var + "'" for var in sorted(potentially_missing_env_vars)))
             warnings.warn(msg, TestCaseWarning)
 
 
 class CliDisplaysVersionInformationInline(TestCase):
     """ Test that a command-line interface provides version information inline. """
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         self.get_simulator_docker_image(specifications)
         image_url = specifications['image']['url']
 
-        cli = [cli] if cli else ['docker', 'run', '--tty', '--rm', image_url]
-
-        result = subprocess.run(cli + ['-v'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url, '-v'],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
-        supported = re.search(r'\d+\.\d+', log)
+        supported = re.match(r'\d+\.\d+', log)
         if not supported:
             warnings.warn(('Command-line interface should support the `-v` option for displaying version information inline.\n\n'
                            'The command-line interface displayed the following when executed with `-v`:\n\n  {}'
                            ).format(log.replace('\n', '\n  ')),
                           TestCaseWarning)
 
-        result = subprocess.run(cli + ['--version'], stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+        result = subprocess.run(['docker', 'run', '--tty', '--rm', image_url, '--version'],
+                                stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
         log = result.stdout.decode() if result.stdout else ''
-        supported = re.search(r'\d+\.\d+', log)
+        supported = re.match(r'\d+\.\d+', log)
         if not supported:
             warnings.warn(('Command-line interface should support the `--version` option for displaying version information inline.\n\n'
                            'The command-line interface displayed the following when executed with `--version`:\n\n  {}'
                            ).format(log.replace('\n', '\n  ')),
                           TestCaseWarning)
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/docker_image.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/docker_image.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,74 +4,60 @@
 :Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
 from ..data_model import TestCase
 from ..warnings import TestCaseWarning
-from .sedml import SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports
 from biosimulators_utils.simulator.environ import ENVIRONMENT_VARIABLES
 import warnings
 
 __all__ = [
     'DefaultUserIsRoot',
     'DeclaresSupportedEnvironmentVariables',
     'HasOciLabels',
     'HasBioContainersLabels',
-    'SingularityImageExecutesSimulationsSuccessfully',
 ]
 
 
 class DefaultUserIsRoot(TestCase):
     """ Test that the default user of a Docker image is root """
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None, expected_user=(None, '', '0')):
+    def eval(self, specifications, expected_user=(None, '', '0')):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
             expected_user (:obj:`tuple`, optional): expected user
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         image = self.get_simulator_docker_image(specifications)
         user = image.attrs['Config']['User']
         if user not in expected_user:
             msg = ("The default user for the Docker image is `{}`. For compatability with Singularity, "
                    "Docker images for simulators should not declare default users (`USER`) other than root. "
                    "Compatability with Singularity is important for using the image on HPC systems, including "
                    "the infrastructure used by runBioSimulations and BioSimulations.\n\n"
                    "More information:\n"
-                   "  https://docs.biosimulations.org/concepts/conventions/simulator-images/\n"
+                   "  https://biosimulators.org/standards/simulator-images\n"
                    "  https://sylabs.io/guides/3.7/user-guide/singularity_and_docker.html#best-practices"
                    ).format(user)
             warnings.warn(msg, TestCaseWarning)
 
 
 class DeclaresSupportedEnvironmentVariables(TestCase):
     """ Test if a Docker image declares the environment variables that is supports """
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         image = self.get_simulator_docker_image(specifications)
         expected_env_vars = set(var.name for var in ENVIRONMENT_VARIABLES.values())
         env_vars = set(key_val.partition('=')[0] for key_val in image.attrs['Config']['Env'])
@@ -102,33 +88,27 @@
         'org.opencontainers.image.title',
         'org.opencontainers.image.url',
         'org.opencontainers.image.vendor',
         'org.opencontainers.image.version',
         'org.opencontainers.image.created',
     ]
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         image = self.get_simulator_docker_image(specifications)
         missing_labels = set(self.EXPECTED_LABELS).difference(set(image.labels.keys()))
         if missing_labels:
-            warnings.warn('Docker images are encouraged to have the following Open Container Initiative (OCI) labels:\n  {}'.format(
+            warnings.warn('The Docker image should have the following Open Container Initiative (OCI) labels:\n  {}'.format(
                 '\n  '.join(sorted(missing_labels))), TestCaseWarning)
 
 
 class HasBioContainersLabels(TestCase):
     """ Test that a Docker image has BioContainers labels with metadata
     about the image
     """
@@ -143,33 +123,21 @@
         "extra.identifiers.biotools",
         "maintainer",
         "software",
         "software.version",
         "version",
     ]
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
         image = self.get_simulator_docker_image(specifications)
         missing_labels = set(self.EXPECTED_LABELS).difference(set(image.labels.keys()))
         if missing_labels:
-            warnings.warn('Docker images are encouraged to have the following BioContainers labels:\n  {}'.format(
+            warnings.warn('The Docker image should have the following BioContainers labels:\n  {}'.format(
                 '\n  '.join(sorted(missing_labels))), TestCaseWarning)
-
-
-class SingularityImageExecutesSimulationsSuccessfully(SimulatorSupportsModelsSimulationsTasksDataGeneratorsAndReports):
-    """ Test that the Singularity version of a Docker image can sucessfully execute COMBINE archives """
-
-    EXEC_WITH_SINGULARITY = True
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/published_project.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/published_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,55 +2,52 @@
 
 :Author: Jonathan Karr <karr@mssm.edu>
 :Date: 2020-12-21
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
-from ..config import Config
-from ..data_model import (TestCase, SedTaskRequirements, ExpectedSedReport, ExpectedSedDataSet, ExpectedSedPlot,
+from ..data_model import (TestCase, SedTaskRequirements, ExpectedSedReport, ExpectedSedPlot,
                           AlertType, OutputMedium)
-from ..exceptions import InvalidOutputsException, SkippedTestCaseException, TimeoutException, TestCaseException
-from ..utils import get_singularity_image_filename, simulation_results_isnan
-from ..warnings import IgnoredTestCaseWarning, SimulatorRuntimeErrorWarning, InvalidOutputsWarning
+from ..exceptions import InvalidOuputsException, SkippedTestCaseException
+from ..warnings import IgnoredTestCaseWarning, SimulatorRuntimeErrorWarning, InvalidOuputsWarning
 from .utils import are_array_shapes_equivalent
 from biosimulators_utils.combine.data_model import CombineArchive, CombineArchiveContentFormatPattern  # noqa: F401
 from biosimulators_utils.combine.io import CombineArchiveReader, CombineArchiveWriter
 from biosimulators_utils.config import get_config
-from biosimulators_utils.image import convert_docker_image_to_singularity
 from biosimulators_utils.report.data_model import ReportFormat
 from biosimulators_utils.report.io import ReportReader
 from biosimulators_utils.sedml.data_model import (  # noqa: F401
-    Output, Report, Task, UniformTimeCourseSimulation,
-    DataGenerator, Variable, Symbol, DataSet,
-    Model, ModelLanguagePattern, Simulation, Algorithm)
+    Report, Task, UniformTimeCourseSimulation,
+    DataGenerator, DataGeneratorVariable, DataGeneratorVariableSymbol, DataSet,
+    Model, Simulation, Algorithm)
 from biosimulators_utils.sedml.io import SedmlSimulationReader, SedmlSimulationWriter
 from biosimulators_utils.sedml.utils import (remove_algorithm_parameter_changes,
                                              replace_complex_data_generators_with_generators_for_individual_variables,
                                              remove_plots)
 import biosimulators_utils.archive.io
 import biosimulators_utils.simulator.exec
 import biosimulators_utils.report.io
 import abc
+import copy
+import datetime
+import dateutil.tz
 import glob
 import json
 import numpy
 import numpy.testing
 import os
 import re
 import shutil
-import subprocess
-import types  # noqa: F401
+import tempfile
 import warnings
 
 __all__ = [
     'SimulatorCanExecutePublishedProject',
     'SyntheticCombineArchiveTestCase',
-    'ExpectedResultOfSyntheticArchive',
-    'find_cases',
     'ConfigurableMasterCombineArchiveTestCase',
     'SingleMasterSedDocumentCombineArchiveTestCase',
     'UniformTimeCourseTestCase',
 ]
 
 EXAMPLES_DIR = os.path.join(os.path.dirname(__file__), '..', '..', 'examples')
 
@@ -60,72 +57,63 @@
 
     Attributes:
         id (:obj:`str`): id
         name (:obj:`str`): name
         filename (:obj:`str`): path to archive
         task_requirements (:obj:`list` of :obj:`SedTaskRequirements`): list of the required model format and simulation algorithm
             for each task in the COMBINE/OMEX archive
-        skipped_simulators (:obj:`list` of :obj:`str`): list of simulation tools to not test the COMBINE archive with
         expected_reports (:obj:`list` of :obj:`ExpectedSedReport`): list of reports expected to be produced by algorithm
         expected_plots (:obj:`list` of :obj:`ExpectedSedPlot`): list of plots expected to be produced by algorithm
         runtime_failure_alert_type (:obj:`AlertType`): whether a run-time failure should be raised as an error or warning
         assert_no_extra_reports (:obj:`bool`): if :obj:`True`, raise an exception if the simulator produces unexpected reports
         assert_no_extra_datasets (:obj:`bool`): if :obj:`True`, raise an exception if the simulator produces unexpected datasets
         assert_no_missing_plots (:obj:`bool`): if :obj:`True`, raise an exception if the simulator doesn't produce the expected plots
         assert_no_extra_plots (:obj:`bool`): if :obj:`True`, raise an exception if the simulator produces unexpected plots
         r_tol (:obj:`float`): relative tolerence
         a_tol (:obj:`float`): absolute tolerence
-        minimum_number_of_synthetic_uniform_time_steps (:obj:`int`): minimum number of steps to use for derived simulation experiments
     """
 
-    def __init__(self, id=None, name=None, filename=None,
-                 task_requirements=None, skipped_simulators=None,
-                 expected_reports=None, expected_plots=None,
+    def __init__(self, id=None, name=None, filename=None, task_requirements=None, expected_reports=None, expected_plots=None,
                  runtime_failure_alert_type=AlertType.exception,
-                 assert_no_extra_reports=False, assert_no_extra_datasets=False,
-                 assert_no_missing_plots=False, assert_no_extra_plots=False,
-                 r_tol=1e-4, a_tol=0., minimum_number_of_synthetic_uniform_time_steps=10,
+                 assert_no_extra_reports=False, assert_no_extra_datasets=False, assert_no_missing_plots=False, assert_no_extra_plots=False,
+                 r_tol=1e-4, a_tol=0.,
                  output_medium=OutputMedium.console):
         """
         Args:
             id (:obj:`str`, optional): id
             name (:obj:`str`, optional): name
             filename (:obj:`str`, optional): path to archive
             task_requirements (:obj:`list` of :obj:`SedTaskRequirements`, optional): list of the required model format and simulation algorithm
                 for each task in the COMBINE/OMEX archive
-            skipped_simulators (:obj:`list` of :obj:`str`, optional): list of simulation tools to not test the COMBINE archive with
             expected_reports (:obj:`list` of :obj:`ExpectedSedReport`, optional): list of reports expected to be produced by algorithm
             expected_plots (:obj:`list` of :obj:`ExpectedSedPlot`, optional): list of plots expected to be produced by algorithm
             runtime_failure_alert_type (:obj:`AlertType`, optional): whether a run-time failure should be raised as an error or warning
             assert_no_extra_reports (:obj:`bool`, optional): if :obj:`True`, raise an exception if the simulator produces unexpected reports
             assert_no_extra_datasets (:obj:`bool`, optional): if :obj:`True`, raise an exception if the simulator produces unexpected datasets
             assert_no_missing_plots (:obj:`bool`, optional): if :obj:`True`, raise an exception if the simulator doesn't produce the expected plots
             assert_no_extra_plots (:obj:`bool`, optional): if :obj:`True`, raise an exception if the simulator produces unexpected plots
             r_tol (:obj:`float`, optional): relative tolerence
             a_tol (:obj:`float`, optional): absolute tolerence
-            minimum_number_of_synthetic_uniform_time_steps (:obj:`int`, optional): minimum number of steps to use for derived simulation experiments
             output_medium (:obj:`OutputMedium`, optional): medium the description should be formatted for
         """
         super(SimulatorCanExecutePublishedProject, self).__init__(id, name, output_medium=output_medium)
         self.filename = filename
         self.task_requirements = task_requirements or []
-        self.skipped_simulators = skipped_simulators or []
         self.expected_reports = expected_reports or []
         self.expected_plots = expected_plots or []
 
         self.description = self.get_description()
 
         self.runtime_failure_alert_type = runtime_failure_alert_type
         self.assert_no_extra_reports = assert_no_extra_reports
         self.assert_no_extra_datasets = assert_no_extra_datasets
         self.assert_no_missing_plots = assert_no_missing_plots
         self.assert_no_extra_plots = assert_no_extra_plots
         self.r_tol = r_tol
         self.a_tol = a_tol
-        self.minimum_number_of_synthetic_uniform_time_steps = minimum_number_of_synthetic_uniform_time_steps
 
     def get_description(self):
         """ Get a description of the case
 
         Returns:
             :obj:`str`: description of the case
         """
@@ -164,20 +152,17 @@
 
         Returns:
             :obj:`SimulatorCanExecutePublishedProject`: this object
         """
         with open(os.path.join(base_path, filename), 'r') as file:
             data = json.load(file)
 
-        id = filename.replace(os.sep + 'expected-results.json', '')
-        self.id = 'published_project.SimulatorCanExecutePublishedProject' + ':' + id
+        self.id = 'published_project.SimulatorCanExecutePublishedProject' + ':' + os.path.splitext(filename)[0]
         self.name = data['name']
-        self.filename = os.path.join(
-            base_path,
-            os.path.relpath(os.path.join(os.path.dirname(filename), '..', data['filename']), '.'))
+        self.filename = os.path.join(os.path.dirname(os.path.join(base_path, filename)), data['filename'])
 
         return self.from_dict(data)
 
     def from_dict(self, data):
         """ Read test case from dictionary
 
         Args:
@@ -186,65 +171,58 @@
         Returns:
             :obj:`SimulatorCanExecutePublishedProject`: this object
         """
         self.task_requirements = []
         for task_req_def in data['taskRequirements']:
             self.task_requirements.append(SedTaskRequirements(
                 model_format=task_req_def['modelFormat'],
-                model_format_features=set(task_req_def.get('modelFormatFeatures', [])),
                 simulation_algorithm=task_req_def['simulationAlgorithm'],
             ))
 
-        self.skipped_simulators = [simulator['id'] for simulator in data['skippedSimulators']]
-
         self.expected_reports = []
         for exp_report_def in data.get('expectedReports', []):
             id = exp_report_def['id']
 
-            data_sets = [ExpectedSedDataSet(id=data_set.get('id', None), label=data_set.get('label', None))
-                         for data_set in exp_report_def.get('dataSets', [])]
-            data_set_ids = [data_set.id for data_set in data_sets]
+            data_set_labels = set(exp_report_def.get('dataSets', []))
             points = tuple(exp_report_def['points'])
 
             values = {}
-            for labelVal in exp_report_def.get('values', []):
-                data_set_id = labelVal['id']
-                val = labelVal['value']
+            for key, val in exp_report_def.get('values', {}).items():
                 if isinstance(val, dict):
-                    values[data_set_id] = {}
+                    values[key] = {}
                     for k, v in val.items():
                         multi_index = tuple(int(index) for index in k.split(","))
                         try:
                             numpy.ravel_multi_index([multi_index], points)[0]
                         except ValueError:
                             raise ValueError((
                                 "Key `{}` of the expected values of report `{}` of published project test case `{}` is invalid. "
                                 "Key must be less than or equal to `{}`."
                             ).format(
                                 multi_index,
                                 self.id,
                                 self.id.replace('published_project.SimulatorCanExecutePublishedProject:', ''),
                                 tuple(p - 1 for p in points),
                             ))
-                        values[data_set_id][multi_index] = v
+                        values[key][multi_index] = v
                 else:
-                    values[data_set_id] = numpy.array(val)
+                    values[key] = numpy.array(val)
 
-            invalid_dataset_ids = set(values.keys()).difference(set(data_set_ids))
+            invalid_dataset_ids = set(values.keys()).difference(set(data_set_labels))
             if invalid_dataset_ids:
                 raise ValueError((
-                    "The `id` fields of the expected values of report `{}` of published project test case `{}` "
+                    "The keys of the expected values of report `{}` of published project test case `{}` "
                     "should be defined in the 'dataSets' property. "
                     "The following keys were not in the 'dataSets' property:\n  - {}").format(
                     id, self.id.replace('published_project.SimulatorCanExecutePublishedProject:', ''),
                     '\n  - '.join(sorted(invalid_dataset_ids))))
 
             self.expected_reports.append(ExpectedSedReport(
                 id=id,
-                data_sets=data_sets,
+                data_sets=data_set_labels,
                 points=points,
                 values=values,
             ))
 
         self.expected_plots = []
         for exp_plot_def in data.get('expectedPlots', []):
             self.expected_plots.append(ExpectedSedPlot(
@@ -254,467 +232,273 @@
         self.runtime_failure_alert_type = AlertType(data.get('runtimeFailureAlertType', 'exception'))
         self.assert_no_extra_reports = data.get('assertNoExtraReports', False)
         self.assert_no_extra_datasets = data.get('assertNoExtraDatasets', False)
         self.assert_no_missing_plots = data.get('assertNoMissingPlots', False)
         self.assert_no_extra_plots = data.get('assertNoExtraPlots', False)
         self.r_tol = data.get('r_tol', 1e-4)
         self.a_tol = data.get('a_tol', 0.)
-        self.minimum_number_of_synthetic_uniform_time_steps = data.get('minimumNumberOfSyntheticUniformTimeSteps', 10)
 
         self.description = self.get_description()
 
         return self
 
     def compatible_with_specifications(self, specifications):
         # determine if case is applicable to simulator
-        if specifications.get('id', None) in self.skipped_simulators:
-            return False
-
         for task_reqs in self.task_requirements:
             reqs_satisfied = False
             for alg_specs in specifications['algorithms']:
-                format_reqs_satisfied = False
-                for format in alg_specs['modelFormats']:
-                    if (
-                        task_reqs.model_format == format['id']
-                        and task_reqs.model_format_features == set(format.get('supportedFeatures', []) or [])
-                    ):
-                        format_reqs_satisfied = True
-                        break
-                if not format_reqs_satisfied:
-                    break
-
-                if task_reqs.simulation_algorithm == alg_specs['kisaoId']['id']:
+                if (task_reqs.model_format in set(format['id'] for format in alg_specs['modelFormats'])
+                        and task_reqs.simulation_algorithm == alg_specs['kisaoId']['id']):
                     reqs_satisfied = True
                     break
 
             if not reqs_satisfied:
                 return False
 
         return True
 
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Raises:
             :obj:`SkippedTestCaseException`: if the test case is not applicable to the simulator
             :obj:`Exception`: if the simulator did not pass the test case
         """
         if not self.compatible_with_specifications(specifications):
             model_formats = set()
             simulation_algorithms = set()
             for task_req in self.task_requirements:
                 model_formats.add(task_req.model_format)
                 simulation_algorithms.add(task_req.simulation_algorithm)
             raise SkippedTestCaseException('Case requires model formats {} and simulation algorithms {}'.format(
                 ', '.join(sorted(model_formats)), ', '.join(sorted(simulation_algorithms))))
 
-        if dry_run:
-            return
+        # create output directory for case
+        out_dir = tempfile.mkdtemp()
 
         # pull image and execute COMBINE/OMEX archive for case
         try:
-            self.exec_sedml_docs_in_archive(specifications, working_dirname, cli=cli)
+            biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_containerized_simulator(
+                self.filename, out_dir, specifications['image']['url'], pull_docker_image=True)
 
         except Exception as exception:
-            if os.path.isdir(working_dirname) and os.getenv('CI', 'false').lower() in ['1', 'true']:
-                subprocess.run(['sudo', 'chown', '{}:{}'.format(os.getuid(), os.getgid()), '-R', working_dirname], check=True)
-
+            shutil.rmtree(out_dir)
             if self.runtime_failure_alert_type == AlertType.exception:
                 raise
             else:
                 warnings.warn(str(exception), SimulatorRuntimeErrorWarning)
                 return
 
         # check expected outputs created
         errors = []
 
         # check expected outputs created: reports
-        if not os.path.isfile(os.path.join(working_dirname, get_config().H5_REPORTS_PATH)):
+        if not os.path.isfile(os.path.join(out_dir, get_config().H5_REPORTS_PATH)):
             errors.append('No reports were generated')
 
         else:
             report_reader = biosimulators_utils.report.io.ReportReader()
             for expected_report in self.expected_reports:
-                report = Report()
-                for data_set in expected_report.data_sets:
-                    report.data_sets.append(DataSet(id=data_set.id, label=data_set.label))
                 try:
-                    report_results = report_reader.run(report, working_dirname, expected_report.id, format=ReportFormat.h5)
+                    report = report_reader.run(out_dir, expected_report.id, format=ReportFormat.h5)
                 except Exception:
                     errors.append('Report {} could not be read'.format(expected_report.id))
                     continue
 
-                missing_data_sets = set([data_set.id for data_set in expected_report.data_sets]).difference(set(report_results.keys()))
+                missing_data_sets = set(expected_report.data_sets).difference(set(report.index))
                 if missing_data_sets:
                     errors.append(('Report {} does not contain expected data sets:\n  {}\n\n'
                                    'Report contained these data sets:\n  {}').format(
                         expected_report.id,
                         '\n  '.join(sorted(missing_data_sets)),
-                        '\n  '.join(sorted(report_results.keys())),
+                        '\n  '.join(sorted(report.index)),
                     ))
                     continue
 
-                points = report_results[report.data_sets[0].id].shape
-                if not are_array_shapes_equivalent(points, expected_report.points):
+                extra_data_sets = set(report.index).difference(set(expected_report.data_sets))
+                if extra_data_sets:
+                    if self.assert_no_extra_datasets:
+                        errors.append('Report {} contains unexpected data sets:\n  {}'.format(
+                            expected_report.id, '\n  '.join(sorted(extra_data_sets))))
+                        continue
+                    else:
+                        warnings.warn('Report {} contains unexpected data sets:\n  {}'.format(
+                            expected_report.id, '\n  '.join(sorted(extra_data_sets))), InvalidOuputsWarning)
+
+                if not are_array_shapes_equivalent(report.shape[1:], expected_report.points):
                     errors.append('Report {} contains incorrect number of points: {} != {}'.format(
-                                  expected_report.id, points, expected_report.points))
+                                  expected_report.id, report.shape[1:], expected_report.points))
                     continue
 
-                for data_set_id, expected_value in expected_report.values.items():
+                for data_set_label, expected_value in expected_report.values.items():
                     if isinstance(expected_value, dict):
-                        value = report_results[data_set_id]
+                        value = report.loc[data_set_label, :]
                         for el_id, expected_el_value in expected_value.items():
                             el_index = numpy.ravel_multi_index([el_id], value.shape)[0]
                             actual_el_value = value[el_index]
                             try:
                                 numpy.testing.assert_allclose(
                                     actual_el_value,
                                     expected_el_value,
                                     rtol=self.r_tol,
                                     atol=self.a_tol,
                                 )
                             except AssertionError:
                                 errors.append('Data set {} of report {} does not have expected value at {}: {} != {}'.format(
-                                    data_set_id, expected_report.id, el_id, actual_el_value, expected_el_value))
+                                    data_set_label, expected_report.id, el_id, actual_el_value, expected_el_value))
                     else:
                         try:
                             numpy.testing.assert_allclose(
-                                report_results[data_set_id],
+                                report.loc[data_set_label, :],
                                 expected_value,
                                 rtol=self.r_tol,
                                 atol=self.a_tol,
                             )
                         except AssertionError:
                             errors.append('Data set {} of report {} does not have expected values'.format(
-                                data_set_id, expected_report.id))
+                                data_set_label, expected_report.id))
 
-            report_ids = set(report_reader.get_ids(working_dirname, type=Report))
+            report_ids = report_reader.get_ids(out_dir)
             expected_report_ids = set(report.id for report in self.expected_reports)
             extra_report_ids = report_ids.difference(expected_report_ids)
             if extra_report_ids:
                 if self.assert_no_extra_reports:
                     errors.append('Unexpected reports were produced:\n  {}'.format(
                         '\n  '.join(sorted(extra_report_ids))))
                 else:
                     warnings.warn('Unexpected reports were produced:\n  {}'.format(
-                        '\n  '.join(sorted(extra_report_ids))), InvalidOutputsWarning)
-
-            plot_ids = set(report_reader.get_ids(working_dirname, type=Output)).difference(report_ids)
-            expected_plot_ids = set(plot.id for plot in self.expected_plots)
-            extra_plot_ids = plot_ids.difference(expected_plot_ids)
-            if extra_plot_ids:
-                if self.assert_no_extra_plots:
-                    errors.append('Unexpected reports for data for plots were produced:\n  {}'.format(
-                        '\n  '.join(sorted(extra_plot_ids))))
-                else:
-                    warnings.warn('Unexpected reports for data for plots were produced:\n  {}'.format(
-                        '\n  '.join(sorted(extra_plot_ids))), InvalidOutputsWarning)
+                        '\n  '.join(sorted(extra_report_ids))), InvalidOuputsWarning)
 
         # check expected outputs created: plots
-        if os.path.isfile(os.path.join(working_dirname, get_config().PLOTS_PATH)):
-            archive = biosimulators_utils.archive.io.ArchiveReader().run(os.path.join(working_dirname, 'plots.zip'))
-            plot_ids = set(os.path.splitext(file.archive_path)[0] for file in archive.files)
+        if os.path.isfile(os.path.join(out_dir, get_config().PLOTS_PATH)):
+            archive = biosimulators_utils.archive.io.ArchiveReader().run(os.path.join(out_dir, 'plots.zip'))
+            plot_ids = set(file.archive_path for file in archive.files)
         else:
             plot_ids = set()
 
         expected_plot_ids = set(plot.id for plot in self.expected_plots)
 
         missing_plot_ids = expected_plot_ids.difference(plot_ids)
         extra_plot_ids = plot_ids.difference(expected_plot_ids)
 
         if missing_plot_ids:
             if self.assert_no_missing_plots:
                 errors.append('Plots were not produced:\n  {}'.format(
                     '\n  '.join(sorted(missing_plot_ids))))
             else:
                 warnings.warn('Plots were not produced:\n  {}'.format(
-                    '\n  '.join(sorted(missing_plot_ids))), InvalidOutputsWarning)
+                    '\n  '.join(sorted(missing_plot_ids))), InvalidOuputsWarning)
 
         if extra_plot_ids:
             if self.assert_no_extra_plots:
-                errors.append('Extra plots were produced:\n  {}'.format(
+                errors.append('Extra plots were not produced:\n  {}'.format(
                     '\n  '.join(sorted(extra_plot_ids))))
             else:
-                warnings.warn('Extra plots were produced:\n  {}'.format(
-                    '\n  '.join(sorted(extra_plot_ids))), InvalidOutputsWarning)
+                warnings.warn('Extra plots were not produced:\n  {}'.format(
+                    '\n  '.join(sorted(extra_plot_ids))), InvalidOuputsWarning)
+
+        # cleanup outputs
+        shutil.rmtree(out_dir)
 
         # raise errors
         if errors:
-            raise InvalidOutputsException('\n\n'.join(errors))
-
-    def exec_sedml_docs_in_archive(self, specifications, out_dir, cli=None):
-        """
-        Args:
-            specifications (:obj:`dict`): specifications of the simulator to validate
-            out_dir (:obj:`str`): path to save simulation results
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
-        """
-        config = Config()
-        pull_docker_image = config.pull_docker_image
-        user_to_exec_within_container = config.user_to_exec_in_simulator_containers
-        if os.getenv('CI', 'false').lower() in ['1', 'true']:
-            user_to_exec_within_container = '_SUDO_'
-
-        if cli:
-            biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_simulator_cli(
-                self.filename, out_dir, cli)
-
-        else:
-            biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_containerized_simulator(
-                self.filename, out_dir, specifications['image']['url'], pull_docker_image=pull_docker_image,
-                user_to_exec_within_container=user_to_exec_within_container)
-
-            if os.path.isdir(out_dir) and os.getenv('CI', 'false').lower() in ['1', 'true']:
-                subprocess.run(['sudo', 'chown', '{}:{}'.format(os.getuid(), os.getgid()), '-R', out_dir], check=True)
+            raise InvalidOuputsException('\n\n'.join(errors))
 
 
 class SyntheticCombineArchiveTestCase(TestCase):
     """ Test that involves a computationally-generated COMBINE/OMEX archive
 
     Attributes:
         id (:obj:`str`): id
         name (:obj:`str`): name
         description (:obj:`str`): description
         output_medium (:obj:`OutputMedium`): medium the description should be formatted for
         published_projects_test_cases (:obj:`list` of :obj:`SimulatorCanExecutePublishedProject`):
             curated COMBINE/OMEX archives that can be used to generate example archives for testing
-        _published_projects_test_case (:obj:`SimulatorCanExecutePublishedProject`): COMBINE/OMEX archive
-            that is used to generate example archives for testing
     """
 
-    EXEC_WITH_SINGULARITY = False
-    REPORT_ERROR_AS_SKIP = False
-
     def __init__(self, id=None, name=None, description=None, output_medium=OutputMedium.console, published_projects_test_cases=None):
         """
         Args:
             id (:obj:`str`, optional): id
             name (:obj:`str`, optional): name
             description (:obj:`str`): description
             output_medium (:obj:`OutputMedium`, optional): medium the description should be formatted for
             published_projects_test_cases (:obj:`list` of :obj:`SimulatorCanExecutePublishedProject`, optional):
                 curated COMBINE/OMEX archives that can be used to generate example archives for testing
         """
         super(SyntheticCombineArchiveTestCase, self).__init__(id=id, name=name, description=description, output_medium=output_medium)
         self.published_projects_test_cases = published_projects_test_cases or []
-        self._published_projects_test_case = None
-
-    def eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
-        """ Evaluate a simulator's performance on a test case
-
-        Args:
-            specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
-
-        Returns:
-            :obj:`bool`: whether there were no warnings about the outputs
-
-        Raises:
-            :obj:`Exception`: if the simulator did not pass the test case
-        """
-        try:
-            return_value = self._eval(specifications, working_dirname,
-                                      synthetic_archives_dir=synthetic_archives_dir, dry_run=dry_run, cli=cli)
-        except Exception as exception:
-            if not isinstance(exception, TimeoutException) and self.REPORT_ERROR_AS_SKIP:
-                raise SkippedTestCaseException(str(exception))
-            else:
-                raise
 
-        return return_value
-
-    def _eval(self, specifications, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
+    def eval(self, specifications):
         """ Evaluate a simulator's performance on a test case
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
-            working_dirname (:obj:`str`): directory for temporary files for evaluating test case
-            synthetic_archives_dir (:obj:`str`, optional): Directory to save the synthetic COMBINE/OMEX archives
-                generated by the test cases
-            dry_run (:obj:`bool`): if :obj:`True`, do not use the simulator to execute COMBINE/OMEX archives.
-            cli (:obj:`str`, optional): command-line interface to use to execute the tests involving the simulation of COMBINE/OMEX
-                archives rather than a Docker image
 
         Returns:
-            :obj:`bool`: whether there were no warnings about the outputs
+            :obj:`object`: data returned by :obj:`eval_outputs`
 
         Raises:
             :obj:`Exception`: if the simulator did not pass the test case
         """
-        if not os.path.isdir(working_dirname):
-            os.makedirs(working_dirname)
+        temp_dir = tempfile.mkdtemp()
 
         # read curated archives and find one that is suitable for testing
         suitable_curated_archive = False
-        for published_projects_test_case in self.published_projects_test_cases:
-            self._published_projects_test_case = published_projects_test_case
-
+        for curated_combine_archive_test_case in self.published_projects_test_cases:
             # read archive
-            curated_archive_filename = published_projects_test_case.filename
-            shared_archive_dir = os.path.join(working_dirname, 'archive')
-            if not os.path.isdir(shared_archive_dir):
-                os.makedirs(shared_archive_dir)
+            curated_archive_filename = curated_combine_archive_test_case.filename
+            shared_archive_dir = os.path.join(temp_dir, 'archive')
+            os.mkdir(shared_archive_dir)
 
             curated_archive = CombineArchiveReader().run(curated_archive_filename, shared_archive_dir)
             curated_sed_docs = {}
             sedml_reader = SedmlSimulationReader()
-            for content in list(curated_archive.contents):
-                if content.format and re.match(CombineArchiveContentFormatPattern.SED_ML, content.format):
+            for content in curated_archive.contents:
+                if re.match(CombineArchiveContentFormatPattern.SED_ML, content.format):
                     sed_doc = sedml_reader.run(os.path.join(shared_archive_dir, content.location))
                     curated_sed_docs[content.location] = sed_doc
 
-                # remove manifest from contents because libSED-ML occassionally has trouble with this
-                elif (
-                    content.location in ['manifest.xml', './manifest.xml']
-                    and content.format == 'http://identifiers.org/combine.specifications/omex-manifest'
-                ):
-                    curated_archive.contents.remove(content)
-                    os.remove(os.path.join(shared_archive_dir, content.location))
-
             # see if archive is suitable for testing
             if self.is_curated_archive_suitable_for_building_synthetic_archive(specifications, curated_archive, curated_sed_docs):
                 suitable_curated_archive = True
                 break
 
             # cleanup
             shutil.rmtree(shared_archive_dir)
 
         if not suitable_curated_archive:
-            raise SkippedTestCaseException('No curated COMBINE/OMEX archives are available to generate archives for testing')
+            warnings.warn('No curated COMBINE/OMEX archives are available to generate archives for testing',
+                          IgnoredTestCaseWarning)
+            shutil.rmtree(temp_dir)
+            return False
 
-        expected_results_of_synthetic_archives = self.build_synthetic_archives(
+        synthetic_archive_filename = os.path.join(temp_dir, 'archive.omex')
+        synthetic_archive, synthetic_sed_docs = self.build_synthetic_archive(
             specifications, curated_archive, shared_archive_dir, curated_sed_docs)
-        has_warnings = False
-        for i_archive, expected_results_of_synthetic_archive in enumerate(expected_results_of_synthetic_archives):
-            if self._eval_synthetic_archive(specifications, expected_results_of_synthetic_archive, shared_archive_dir,
-                                            i_archive, os.path.join(working_dirname, str(i_archive + 1)),
-                                            synthetic_archives_dir=synthetic_archives_dir, dry_run=dry_run,
-                                            cli=cli):
-                has_warnings = True
-        return not has_warnings
-
-    def _eval_synthetic_archive(self, specifications, expected_results_of_synthetic_archive, shared_archive_dir,
-                                i_synthetic_archive, working_dirname, synthetic_archives_dir=None, dry_run=False, cli=None):
-        synthetic_archive = expected_results_of_synthetic_archive.archive
-        synthetic_sed_docs = expected_results_of_synthetic_archive.sed_documents
-        is_success_expected = expected_results_of_synthetic_archive.is_success_expected
-        environment = expected_results_of_synthetic_archive.environment
-
-        if not os.path.isdir(working_dirname):
-            os.makedirs(working_dirname)
-
         sedml_writer = SedmlSimulationWriter()
-        synthetic_archive_filename = os.path.join(working_dirname, 'archive.omex')
         for location, sed_doc in synthetic_sed_docs.items():
             sedml_writer.run(sed_doc, os.path.join(shared_archive_dir, location))
         CombineArchiveWriter().run(synthetic_archive, shared_archive_dir, synthetic_archive_filename)
 
-        if synthetic_archives_dir:
-            cls = self.__class__
-            module = cls.__module__.partition('biosimulators_test_suite.test_case.')[2]
-            export_synthetic_archive_dirname = os.path.join(synthetic_archives_dir, module, cls.__name__)
-            if not os.path.isdir(export_synthetic_archive_dirname):
-                os.makedirs(export_synthetic_archive_dirname)
-            export_synthetic_archive_filename = os.path.join(export_synthetic_archive_dirname,
-                                                             '{}.{}.omex'.format(
-                                                                 str(i_synthetic_archive + 1),
-                                                                 'execution-should-succeed'
-                                                                 if is_success_expected else
-                                                                 'execute-should-fail'))
-            shutil.copy(synthetic_archive_filename, export_synthetic_archive_filename)
-
-        if dry_run:
-            return False
-
         # use synthetic archive to test simulator
-        outputs_dir = os.path.join(working_dirname, 'outputs')
-        config = Config()
-        pull_docker_image = config.pull_docker_image
-        user_to_exec_within_container = config.user_to_exec_in_simulator_containers
-        has_warnings = False
+        outputs_dir = os.path.join(temp_dir, 'outputs')
+        succeeded = False
         try:
-            if os.getenv('CI', 'false').lower() in ['1', 'true']:
-                user_to_exec_within_container = '_SUDO_'
-
-            if cli:
-                biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_simulator_cli(
-                    synthetic_archive_filename, outputs_dir, cli, environment=environment)
-
-            elif self.EXEC_WITH_SINGULARITY:
-                docker_image_url = specifications['image']['url']
-
-                # get path for Singularity image
-                singularity_filename = get_singularity_image_filename(docker_image_url)
-
-                # convert image to Singularity format
-                convert_docker_image_to_singularity(docker_image_url, singularity_filename=singularity_filename)
-
-                # run a simulation with the Singularity image
-                if not os.path.isdir(outputs_dir):
-                    os.makedirs(outputs_dir)
-                temp_filename = os.path.join(outputs_dir, os.path.basename(synthetic_archive_filename))
-                shutil.copyfile(synthetic_archive_filename, temp_filename)
-
-                cmd = [
-                    'singularity', 'run',
-                    '-B', outputs_dir + ':/root',
-                    singularity_filename,
-                    '-i', '/root/' + os.path.basename(synthetic_archive_filename),
-                    '-o', '/root',
-                ]
-                result = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, check=False)
-                os.remove(temp_filename)
-                if result.returncode != 0:
-                    msg = 'The Docker image could not be successfully executed as a Singularity image:\n  {}'.format(
-                        result.stderr.decode().replace('\n', '\n  '))
-                    raise TestCaseException(msg)
-
-            else:
-                biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_containerized_simulator(
-                    synthetic_archive_filename, outputs_dir, specifications['image']['url'], pull_docker_image=pull_docker_image,
-                    environment=environment,
-                    user_to_exec_within_container=user_to_exec_within_container)
-
-            if os.path.isdir(outputs_dir) and os.getenv('CI', 'false').lower() in ['1', 'true']:
-                subprocess.run(['sudo', 'chown', '{}:{}'.format(os.getuid(), os.getgid()), '-R', outputs_dir], check=True)
-
-            if not self.eval_outputs(specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
-                has_warnings = True
-
-            succeeded = True
-
-        except Exception:
-            if os.path.isdir(outputs_dir) and os.getenv('CI', 'false').lower() in ['1', 'true']:
-                subprocess.run(['sudo', 'chown', '{}:{}'.format(os.getuid(), os.getgid()), '-R', outputs_dir], check=True)
-
-            succeeded = False
-            if is_success_expected:
-                raise
-
-        if succeeded and not is_success_expected:
-            msg = 'The execution of the COMBINE/OMEX archive did not fail as expected'
-            raise ValueError(msg)
+            biosimulators_utils.simulator.exec.exec_sedml_docs_in_archive_with_containerized_simulator(
+                synthetic_archive_filename, outputs_dir, specifications['image']['url'], pull_docker_image=True)
 
-        return has_warnings
+            succeeded = self.eval_outputs(specifications, synthetic_archive, synthetic_sed_docs, outputs_dir)
+        finally:
+            shutil.rmtree(temp_dir)
+        return succeeded
 
     def is_curated_archive_suitable_for_building_synthetic_archive(self, specifications, archive, sed_docs):
         """ Find an archive with at least one report
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
@@ -722,47 +506,40 @@
                 SED documents in curated archive
 
         Returns:
             :obj:`bool`: :obj:`True`, if the curated archive is suitable for generating a synthetic
                 archive for testing
         """
         for location, sed_doc in sed_docs.items():
-            if self.is_curated_sed_doc_suitable_for_building_synthetic_archive(specifications, sed_doc, location):
+            if self.is_curated_sed_doc_suitable_for_building_synthetic_archive(specifications, sed_doc):
                 return True
         return False
 
-    def is_curated_sed_doc_suitable_for_building_synthetic_archive(self, specifications, sed_doc, sed_doc_location):
+    def is_curated_sed_doc_suitable_for_building_synthetic_archive(self, specifications, sed_doc):
         """ Determine if a SED document is suitable for testing
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             sed_doc (:obj:`SedDocument`): SED document in curated archive
-            sed_doc_location (:obj:`str`): location of the SED document within its parent COMBINE/OMEX archive
 
         Returns:
             :obj:`bool`: whether the SED document is suitable for testing
         """
-        split_sed_doc_location = os.path.split(os.path.relpath(sed_doc_location, '.'))
-        if split_sed_doc_location[0] or len(split_sed_doc_location) > 2:
-            return False
-
         for output in sed_doc.outputs:
-            if isinstance(output, Report) and self.is_curated_sed_report_suitable_for_building_synthetic_archive(
-                    specifications, output, sed_doc_location):
+            if isinstance(output, Report) and self.is_curated_sed_report_suitable_for_building_synthetic_archive(specifications, output):
                 return True
 
         return False
 
-    def is_curated_sed_report_suitable_for_building_synthetic_archive(self, specifications, report, sed_doc_location):
+    def is_curated_sed_report_suitable_for_building_synthetic_archive(self, specifications, report):
         """ Determine if a SED report is suitable for testing
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             report (:obj:`Report`): SED report in curated archive
-            sed_doc_location (:obj:`str`): location of the SED document within its parent COMBINE/OMEX archive
 
         Returns:
             :obj:`bool`: whether the report is suitable for testing
         """
         task_variables = {}
         for data_set in report.data_sets:
             for variable in data_set.data_generator.variables:
@@ -803,23 +580,15 @@
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             model (:obj:`Model`): SED model in curated archive
 
         Returns:
             :obj:`bool`: whether the model is suitable for testing
         """
-        if not model or not model.source:
-            return False
-        source = model.source.lower()
-        return not (
-            source.startswith('#')
-            or source.startswith('http://')
-            or source.startswith('https://')
-            or source.startswith('urn:')
-        )
+        return True
 
     def is_curated_sed_simulation_suitable_for_building_synthetic_archive(self, specifications, simulation):
         """ Determine if a SED simulation is suitable for testing
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             simulation (:obj:`Simulation`): SED simulation in curated archive
@@ -827,15 +596,15 @@
         Returns:
             :obj:`bool`: whether the simulation is suitable for testing
         """
         if isinstance(simulation, UniformTimeCourseSimulation):
             if (
                 simulation.initial_time != 0
                 or simulation.output_start_time != 0
-                or simulation.number_of_points < 1
+                or simulation.number_of_points <= 0
                 or int(simulation.number_of_points / 2) != simulation.number_of_points / 2
             ):
                 return False
         return self.is_curated_sed_algorithm_suitable_for_building_synthetic_archive(specifications, simulation.algorithm)
 
     def is_curated_sed_algorithm_suitable_for_building_synthetic_archive(self, specifications, algorithm):
         """ Determine if a SED algorithm is suitable for testing
@@ -845,64 +614,63 @@
             algorithm (:obj:`Algorithm`): SED algorithm in curated archive
 
         Returns:
             :obj:`bool`: whether the algorithm is suitable for testing
         """
         return True
 
-    def build_synthetic_archives(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
         """ Generate a synthetic archive for testing
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
             curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
             curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
                 SED documents in curated archive
 
         Returns:
-            :obj:`list` of :obj:`ExpectedResultOfSyntheticArchive`
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
+        """
+
+        # set updated times because libCOMBINE requires this
+        now = self.get_current_time_utc()
+        curated_archive.updated = now
+        for content in curated_archive.contents:
+            content.updated = now
+
+        return (curated_archive, curated_sed_docs)
+
+    def get_current_time_utc(self):
+        """ Get the current time in UTC
+
+        Returns:
+            :obj:`datetime.datetime`: current time in UTC
         """
-        return [ExpectedResultOfSyntheticArchive(curated_archive, curated_sed_docs, True)]
+        now = datetime.datetime.now()
+        return datetime.datetime(now.year, now.month, now.day, now.hour, now.minute, now.second, tzinfo=dateutil.tz.tzutc())
 
     @abc.abstractmethod
     def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
         """ Test that the expected outputs were created for the synthetic archive
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
             synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
                 document in the synthetic archive to the document
             outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
-
-        Returns:
-            :obj:`bool`: whether there were no warnings about the outputs
         """
         pass  # pragma: no cover
 
 
-class ExpectedResultOfSyntheticArchive(object):
-    """ An expected result of executing a synthetic COMBINE/OMEX archive
-
-    Attributes:
-        archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
-        sed_documents (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
-          SED documents in synthetic archive
-        is_success_expected (:obj:`bool`, optional): whether the execution of the archive is expected to succeed
-        environment (:obj:`dict`, optional): environment variables that the archive should be executed with
-    """
-
-    def __init__(self, archive, sed_documents, is_success_expected=True, environment=None):
-        self.archive = archive
-        self.sed_documents = sed_documents
-        self.is_success_expected = is_success_expected
-        self.environment = environment or {}
-
-
 def find_cases(specifications, dir_name=None, output_medium=OutputMedium.console):
     """ Collect test cases
 
     Args:
         specifications (:obj:`dict`): specifications of the simulator to validate
         dir_name (:obj:`str`, optional): path to find example COMBINE/OMEX archives
         output_medium (:obj:`OutputMedium`, optional): medium the description should be formatted for
@@ -913,36 +681,33 @@
     if dir_name is None:
         dir_name = EXAMPLES_DIR
     if not os.path.isdir(dir_name):
         warnings.warn('Directory of example COMBINE/OMEX archives is not available', IgnoredTestCaseWarning)
 
     all_cases = []
     compatible_cases = []
-    for example_filename in glob.glob(os.path.join(dir_name, '**/*.omex'), recursive=True):
-        md_filename = os.path.join(example_filename[0:-5], 'expected-results.json')
+    for md_filename in glob.glob(os.path.join(dir_name, '**/*.json'), recursive=True):
         rel_filename = os.path.relpath(md_filename, dir_name)
         case = SimulatorCanExecutePublishedProject(output_medium=output_medium).from_json(dir_name, rel_filename)
         all_cases.append(case)
         if case.compatible_with_specifications(specifications):
             compatible_cases.append(case)
 
-    all_cases.sort(key=lambda case: case.filename)
-    compatible_cases.sort(key=lambda case: case.filename)
-
     # return cases
     return (all_cases, compatible_cases)
 
 
 class ConfigurableMasterCombineArchiveTestCase(SyntheticCombineArchiveTestCase):
     """ Class for generating synthetic archives with a single master SED-ML file or two non-master
     copies of the same file
 
     Attributes:
         _archive_has_master (:obj:`bool`): whether the synthetic archive should have a master file
-        _model_change_filter (:obj:`types.FunctionType`): filter for model changes to keep
+        _include_non_master (:obj:`bool`): whether the synthetic archive should also have a non-master file
+        _types_of_model_changes_to_keep (:obj:`list` of :obj:`type`): types of model changes to keep
         _remove_algorithm_parameter_changes (:obj:`bool`): if :obj:`True`, remove instructions to change
             the values of the parameters of algorithms
         _use_single_variable_data_generators (:obj:`bool`): if :obj:`True`, replace data generators that
             involve multiple variables or parameters (and data sets, curves, and surfaces) with multiple
             data generators for each variable
         _remove_plots (:obj:`bool`): if :obj:`True`, remove plots
         _keep_one_task_one_report (:obj:`bool`): if :obj:`True`, keep only 1 task and only 1 report
@@ -950,41 +715,50 @@
     """
 
     @property
     @abc.abstractmethod
     def _archive_has_master(self):
         pass  # pragma: no cover
 
+    @property
+    @abc.abstractmethod
+    def _include_non_master(self):
+        pass  # pragma: no cover
+
     def __init__(self, *args, **kwargs):
         super(ConfigurableMasterCombineArchiveTestCase, self).__init__(*args, **kwargs)
-        self._model_change_filter = lambda change: False
+        self._types_of_model_changes_to_keep = ()
         self._remove_algorithm_parameter_changes = True
         self._use_single_variable_data_generators = True
         self._remove_plots = True
         self._keep_one_task_one_report = True
 
-    def build_synthetic_archives(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
         """ Generate a synthetic archive with master and non-master SED documents
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
             curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
             curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
                 SED documents in curated archive
 
         Returns:
-            :obj:`list` of :obj:`ExpectedResultOfSyntheticArchive`
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
         """
-        super(ConfigurableMasterCombineArchiveTestCase, self).build_synthetic_archives(
+        super(ConfigurableMasterCombineArchiveTestCase, self).build_synthetic_archive(
             specifications, curated_archive, curated_archive_dir, curated_sed_docs)
 
         # get a suitable SED document to modify
         for doc_location, doc in curated_sed_docs.items():
-            if self.is_curated_sed_doc_suitable_for_building_synthetic_archive(specifications, doc, doc_location):
+            if self.is_curated_sed_doc_suitable_for_building_synthetic_archive(specifications, doc):
                 break
         doc_content = next(content for content in curated_archive.contents if content.location == doc_location)
 
         # remove all other SED documents from archive
         original_contents = curated_archive.contents
         curated_archive.contents = []
         for content in original_contents:
@@ -996,15 +770,15 @@
             content.master = False
 
         # make document master
         doc_content.master = self._archive_has_master
 
         # retain some model changes
         for model in doc.models:
-            model.changes = list(filter(self._model_change_filter, model.changes))
+            model.changes = [change for change in model.changes if isinstance(change, self._types_of_model_changes_to_keep)]
 
         # remove algorithm parameter changes
         if self._remove_algorithm_parameter_changes:
             remove_algorithm_parameter_changes(doc)
 
         # replace data generator that involve mathematical expressions with multiple data generators for each individual variable
         if self._use_single_variable_data_generators:
@@ -1015,78 +789,77 @@
             remove_plots(doc)
 
         # keep only single task and single report
         if self._keep_one_task_one_report and self._use_single_variable_data_generators and self._remove_plots:
             key_report = None
             key_task = None
             for report in doc.outputs:
-                if self.is_curated_sed_report_suitable_for_building_synthetic_archive(specifications, report, doc_location):
+                if self.is_curated_sed_report_suitable_for_building_synthetic_archive(specifications, report):
                     for data_set in report.data_sets:
                         task = data_set.data_generator.variables[0].task
                         if self.is_curated_sed_task_suitable_for_building_synthetic_archive(specifications, task):
                             key_report = report
                             key_task = task
                             break
                     if key_report:
                         break
 
-            key_sim = key_task.simulation
-            if isinstance(key_sim, UniformTimeCourseSimulation):
-                key_sim.output_end_time = (
-                    key_sim.output_start_time
-                    + (
-                        min(self._published_projects_test_case.minimum_number_of_synthetic_uniform_time_steps, key_sim.number_of_points)
-                        / key_sim.number_of_points * (key_sim.output_end_time - key_sim.output_start_time)
-                      )
-                )
-                key_sim.number_of_points = min(self._published_projects_test_case.minimum_number_of_synthetic_uniform_time_steps,
-                                               key_sim.number_of_points)
-
             doc.models = [key_task.model]
             doc.simulations = [key_task.simulation]
             doc.tasks = [key_task]
             doc.data_generators = [data_gen for data_gen in doc.data_generators if data_gen.variables[0].task == key_task]
             doc.outputs = [key_report]
             key_report.data_sets = [data_set for data_set in key_report.data_sets if data_set.data_generator in doc.data_generators]
 
-            # limit number of data set
-            max_data_sets = 10
-            key_report.data_sets = key_report.data_sets[0:max_data_sets]
-            doc.data_generators = [data_set.data_generator for data_set in key_report.data_sets]
-
         curated_sed_docs = {
             doc_content.location: doc,
         }
 
+        # duplicate document
+        if self._include_non_master:
+            doc_content_copy = copy.deepcopy(doc_content)
+            doc_content_copy.master = False
+            doc_content_copy.location = os.path.join(
+                os.path.dirname(doc_content_copy.location),
+                '__copy__' + os.path.basename(doc_content_copy.location))
+            curated_archive.contents.append(doc_content_copy)
+
+            curated_sed_docs[doc_content_copy.location] = copy.deepcopy(doc)
+
         self._expected_report_ids = []
         for output in doc.outputs:
             if isinstance(output, Report):
                 self._expected_report_ids.append(os.path.join(os.path.relpath(doc_content.location, './'), output.id))
+                if not self._archive_has_master and self._include_non_master:
+                    self._expected_report_ids.append(os.path.join(os.path.relpath(doc_content_copy.location, './'), output.id))
 
         # return modified SED document
-        return [ExpectedResultOfSyntheticArchive(curated_archive, curated_sed_docs, True)]
+        return (curated_archive, curated_sed_docs)
 
 
 class SingleMasterSedDocumentCombineArchiveTestCase(ConfigurableMasterCombineArchiveTestCase):
     """ Class for generating synthetic COMBINE/OMEX archives with a single master SED-ML file
 
     Attributes:
         _archive_has_master (:obj:`bool`): whether the synthetic archive should  have a master file
+        _include_non_master (:obj:`bool`): whether the synthetic archive should also have a non-master file
     """
 
     @property
     def _archive_has_master(self):
         return True
 
+    @property
+    def _include_non_master(self):
+        return False
+
 
 class UniformTimeCourseTestCase(SingleMasterSedDocumentCombineArchiveTestCase):
     """ Test that a simulator supports multiple reports per SED document """
 
-    TEST_TIME = True
-
     def is_curated_sed_task_suitable_for_building_synthetic_archive(self, specifications, task):
         """ Determine if a SED task is suitable for testing
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             task (:obj:`Task`): SED task in curated archive
 
@@ -1101,102 +874,78 @@
         return (
             isinstance(sim, UniformTimeCourseSimulation)
             and sim.initial_time == 0
             and sim.output_start_time == 0
             and int(sim.number_of_points / 2) == sim.number_of_points / 2
         )
 
-    def build_synthetic_archives(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
+    def build_synthetic_archive(self, specifications, curated_archive, curated_archive_dir, curated_sed_docs):
         """ Generate a synthetic archive with a copy of each task and each report
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             curated_archive (:obj:`CombineArchive`): curated COMBINE/OMEX archive
             curated_archive_dir (:obj:`str`): directory with the contents of the curated COMBINE/OMEX archive
             curated_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from locations to
                 SED documents in curated archive
 
         Returns:
-            :obj:`list` of :obj:`ExpectedResultOfSyntheticArchive`
+            :obj:`tuple`:
+
+                * :obj:`CombineArchive`: synthetic COMBINE/OMEX archive for testing the simulator
+                * :obj:`dict` of :obj:`str` to :obj:`SedDocument`: map from locations to
+                  SED documents in synthetic archive
         """
-        expected_results_of_synthetic_archives = super(UniformTimeCourseTestCase, self).build_synthetic_archives(
+        curated_archive, curated_sed_docs = super(UniformTimeCourseTestCase, self).build_synthetic_archive(
             specifications, curated_archive, curated_archive_dir, curated_sed_docs)
 
-        for expected_results_of_synthetic_archive in expected_results_of_synthetic_archives:
-            curated_archive = expected_results_of_synthetic_archive.archive
-            curated_sed_docs = expected_results_of_synthetic_archive.sed_documents
-
-            # get a suitable SED document to modify
-            doc = list(curated_sed_docs.values())[0]
-            task = doc.tasks[0]
-            sim = task.simulation
-            self.modify_simulation(sim)
-            report = doc.outputs[0]
-
-            if self.TEST_TIME:
-                self.add_time_data_set(doc, task, report)
-
-            expected_results_of_synthetic_archive.archive = curated_archive
-            expected_results_of_synthetic_archive.sed_documents = curated_sed_docs
-
-        # return modified SED document
-        return expected_results_of_synthetic_archives
-
-    def add_time_data_set(self, doc, task, report):
-        """ Rename or add a time data set to a SED report
+        # get a suitable SED document to modify
+        doc = list(curated_sed_docs.values())[0]
+        task = doc.tasks[0]
+        sim = task.simulation
+        self.modify_simulation(sim)
+        report = doc.outputs[0]
 
-        Args:
-            doc (:obj:`SedDocument`): SED document
-            task (:obj:`task`): SED task
-            report (:obj:`Report`): SED report
-        """
-        time_data_gen = None
+        time_data_set = False
         for data_gen in doc.data_generators:
             var = data_gen.variables[0]
-            if var.task == task and var.symbol == Symbol.time:
-                time_data_gen = data_gen
-                break
-
-        if not time_data_gen:
-            if re.match(ModelLanguagePattern.CellML.value, task.model.language):
-                msg = (
-                    'This test case requires a model language which supports the time symbol ({}). '
-                    '{} does not support the time symbol.'
-                ).format(Symbol.time.value, ModelLanguagePattern.CellML.name)
-                raise SkippedTestCaseException(msg)
-
-            time_data_gen = DataGenerator(
-                id='__data_generator_time__',
-                variables=[
-                    Variable(
-                        id='__variable_time__',
-                        task=task,
-                        symbol=Symbol.time,
-                    ),
-                ],
-                math='__variable_time__',
-            )
-            doc.data_generators.append(time_data_gen)
-
-        time_data_set = None
-        for data_set in report.data_sets:
-            if data_set.data_generator == time_data_gen:
-                time_data_set = data_set
-                data_set.id = '__data_set_time__'
+            if var.symbol == DataGeneratorVariableSymbol.time:
+                for data_set in report.data_sets:
+                    if data_set.data_generator == data_gen:
+                        time_data_set = True
+                        data_set.label = '__data_set_time__'
+                        break
+            if time_data_set:
                 break
 
         if not time_data_set:
+            doc.data_generators.append(
+                DataGenerator(
+                    id='__data_generator_time__',
+                    variables=[
+                        DataGeneratorVariable(
+                            id='__variable_time__',
+                            task=task,
+                            symbol=DataGeneratorVariableSymbol.time,
+                        ),
+                    ],
+                    math='__variable_time__',
+                ),
+            )
             report.data_sets.append(
                 DataSet(
                     id='__data_set_time__',
                     label='__data_set_time__',
-                    data_generator=time_data_gen,
+                    data_generator=doc.data_generators[-1],
                 )
             )
 
+        # return modified SED document
+        return (curated_archive, curated_sed_docs)
+
     @abc.abstractmethod
     def modify_simulation(self, simulation):
         """ Modify a simulation
 
         Args:
             simulation (:obj:`UniformTimeCourseSimulation`): simulation
         """
@@ -1207,39 +956,33 @@
 
         Args:
             specifications (:obj:`dict`): specifications of the simulator to validate
             synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
             synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
                 document in the synthetic archive to the document
             outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
-
-        Returns:
-            :obj:`bool`: whether there were no warnings about the outputs
         """
         has_warnings = False
 
         doc_location = list(synthetic_sed_docs.keys())[0]
         doc_id = os.path.relpath(doc_location, './')
         doc = list(synthetic_sed_docs.values())[0]
         sim = doc.simulations[0]
         report = doc.outputs[0]
 
-        data = ReportReader().run(report, outputs_dir, os.path.join(doc_id, report.id))
+        data = ReportReader().run(outputs_dir, os.path.join(doc_id, report.id))
 
-        for data_set_data in data.values():
-            if numpy.any(simulation_results_isnan(data_set_data)):
-                warnings.warn('The results produced by the simulator include `NaN`.', InvalidOutputsWarning)
-                has_warnings = True
-                break
+        if numpy.any(numpy.isnan(data)):
+            warnings.warn('The results produced by the simulator include `NaN`.', InvalidOuputsWarning)
+            has_warnings = True
 
-        if self.TEST_TIME:
-            try:
-                numpy.testing.assert_allclose(
-                    data['__data_set_time__'],
-                    numpy.linspace(sim.output_start_time, sim.output_end_time, sim.number_of_points + 1),
-                    rtol=1e-4,
-                )
-            except Exception as exception:
-                raise ValueError('Simulator did not produce the expected time course:\n\n  {}'.format(
-                    str(exception).replace('\n', '\n  ')))
+        try:
+            numpy.testing.assert_allclose(
+                data.loc['__data_set_time__', :],
+                numpy.linspace(sim.output_start_time, sim.output_end_time, sim.number_of_points + 1),
+                rtol=1e-4,
+            )
+        except Exception as exception:
+            raise ValueError('Simulator did not produce the expected time course:\n\n  {}'.format(
+                str(exception).replace('\n', '\n  ')))
 
         return not has_warnings
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/results_report.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/exec_status_report.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-""" Methods for checking support for reports of simulation results
+""" Methods for checking support for reports of the execution status of modeling projects
 
 :Author: Jonathan Karr <karr@mssm.edu>
 :Date: 2020-12-29
 :Copyright: 2020, Center for Reproducible Biomedical Modeling
 :License: MIT
 """
 
-from ..utils import simulation_results_isnan
 from ..warnings import TestCaseWarning
 from .published_project import SingleMasterSedDocumentCombineArchiveTestCase
 from biosimulators_utils.combine.data_model import CombineArchive  # noqa: F401
-from biosimulators_utils.report.data_model import ReportFormat
-from biosimulators_utils.report.io import ReportReader
+from biosimulators_utils.config import get_config
+from biosimulators_utils.exec_status.data_model import ExecutionStatus
 from biosimulators_utils.sedml.data_model import SedDocument, Report  # noqa: F401
-import h5py
 import os
-import numpy
 import warnings
+import yaml
 
 __all__ = [
-    'SimulatorGeneratesReportsOfSimulationResults',
+    'SimulatorReportsTheStatusOfTheExecutionOfCombineArchives',
 ]
 
 
-class SimulatorGeneratesReportsOfSimulationResults(SingleMasterSedDocumentCombineArchiveTestCase):
+class SimulatorReportsTheStatusOfTheExecutionOfCombineArchives(SingleMasterSedDocumentCombineArchiveTestCase):
     """ Test that when a COMBINE/OMEX archive defines a (single) master file, the simulator only
     executes this file.
     """
 
     def eval_outputs(self, specifications, synthetic_archive, synthetic_sed_docs, outputs_dir):
         """ Test that the expected outputs were created for the synthetic archive
 
@@ -35,57 +33,74 @@
             specifications (:obj:`dict`): specifications of the simulator to validate
             synthetic_archive (:obj:`CombineArchive`): synthetic COMBINE/OMEX archive for testing the simulator
             synthetic_sed_docs (:obj:`dict` of :obj:`str` to :obj:`SedDocument`): map from the location of each SED
                 document in the synthetic archive to the document
             outputs_dir (:obj:`str`): directory that contains the outputs produced from the execution of the synthetic archive
 
         Returns:
-            :obj:`bool`: whether there were no warnings about the outputs
+            :obj:`bool`: :obj:`True`, if simulator passes the test
         """
-        try:
-            ReportReader().get_ids(outputs_dir)
-        except Exception:
-            raise ValueError('Simulator must generate reports of simulation results')
+        exec_status_path = os.path.join(outputs_dir, get_config().EXEC_STATUS_PATH)
 
         has_warning = False
-        for doc_location, sed_doc in synthetic_sed_docs.items():
-            doc_id = os.path.relpath(doc_location, '.')
-            for output in sed_doc.outputs:
-                if isinstance(output, Report):
-                    uri = os.path.join(doc_id, output.id)
-                    uri_parts = uri.split(os.path.sep)
-                    uri = '/'.join(uri_parts)
-                    report_data = ReportReader().run(output, outputs_dir, uri, format=ReportFormat.h5)
-
-                    expected_data_sets = set(data_set.id for data_set in output.data_sets)
-                    data_sets = set(report_data.keys())
-
-                    missing_data_sets = expected_data_sets.difference(data_sets)
-                    # extra_data_sets = data_sets.difference(expected_data_sets)
-
-                    if missing_data_sets:
-                        raise ValueError('Simulator did not produce the following data sets:\n  - {}'.format(
-                            '\n  - '.join(sorted(missing_data_sets))))
-
-                    for data_set_data in report_data.values():
-                        if numpy.any(simulation_results_isnan(data_set_data)):
-                            warnings.warn('The results produced by the simulator include `NaN`.', TestCaseWarning)
-                            has_warning = True
-
-                    with h5py.File(os.path.join(outputs_dir, 'reports.h5'), 'r') as file:
-
-                        temp = file[uri].attrs.get('uri', None)
-                        if temp != uri:
-                            raise ValueError('`uri` of HDF5 data set `{}` must be `{}`, not `{}`.'.format(uri, uri, temp))
-
-                        for i_group in range(len(uri_parts) - 1):
-                            group_uri = '/'.join(uri_parts[0:i_group + 1])
-                            temp = file[group_uri].attrs.get('uri', None)
-                            if temp != group_uri:
-                                raise ValueError('`uri` of HDF5 group `{}` must be `{}`, not `{}`.'.format(group_uri, group_uri, temp))
-
-                            temp = file[group_uri].attrs.get('combineArchiveLocation', None)
-                            if temp != group_uri:
-                                raise ValueError('`combineArchiveLocation` of HDF5 group `{}` must be `{}`, not `{}`.'.format(
-                                    group_uri, group_uri, temp))
+
+        if not os.path.isfile(exec_status_path):
+            msg = (
+                'The simulator did not export information about the status of its execution. '
+                'Simulators are encouraged to stream information about their execution status.\n\n'
+                'More information: https://biosimulators.org/standards/status'
+            )
+            warnings.warn(msg, TestCaseWarning)
+            has_warning = True
+
+        try:
+            with open(exec_status_path, 'r') as file:
+                status = yaml.load(file)
+        except Exception as exception:
+            warnings.warn('The execution status report produced by the simulator is not valid:\n\n  {}'.format(
+                str(exception).replace('\n', '\n  ')), TestCaseWarning)
+            has_warning = True
+
+        self._status_valid = True
+
+        def is_status_valid(status, self=self):
+            if status not in [
+                ExecutionStatus.SUCCEEDED.value,
+                ExecutionStatus.SKIPPED.value,
+                ExecutionStatus.FAILED.value,
+            ]:
+                self._status_valid = False
+
+        try:
+            is_status_valid(status['status'])
+
+            for doc in status['sedDocuments'].values():
+                is_status_valid(doc['status'])
+
+                for task in doc['tasks'].values():
+                    is_status_valid(task['status'])
+
+                for output in doc['outputs'].values():
+                    is_status_valid(output['status'])
+
+                    els = output.get('dataSets', output.get('curves', output.get('surfaces', None)))
+                    if els is None:
+                        raise KeyError('Outputs must have one of the keys `dataSets`, `curves` or `surfaces`')
+                    for status in els.values():
+                        is_status_valid(status)
+
+        except Exception as exception:
+            warnings.warn('The execution status report produced by the simulator is not valid:\n\n  {}'.format(
+                str(exception).replace('\n', '\n  ')), TestCaseWarning)
+            has_warning = True
+
+        if not self._status_valid:
+            msg = (
+                'The execution status report produced by the simulator is not valid. '
+                'By the end of the execution of a COMBINE/OMEX archive, the status of '
+                'the archive, each SED document, and each SED element should be '
+                '`SUCCEEDED`, `SKIPPED`, or `FAILED`.'
+            )
+            warnings.warn(msg, TestCaseWarning)
+            has_warning = True
 
         return not has_warning
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite/test_case/utils.py` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite/test_case/utils.py`

 * *Files identical despite different names*

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/PKG-INFO` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,114 @@
 Metadata-Version: 2.1
 Name: biosimulators-test-suite
-Version: 0.1.87
+Version: 0.1.9
 Summary: Tools for validating that biosimulation tools are consistent with the BioSimulators standards
 Home-page: https://github.com/biosimulators/Biosimulators_test_suite
-Download-URL: https://github.com/biosimulators/Biosimulators_test_suite
 Author: Center for Reproducible Biomedical Modeling
 Author-email: info@biosimulators.org
 License: MIT
+Download-URL: https://github.com/biosimulators/Biosimulators_test_suite
+Description: |Latest release| |PyPI| |CI status| |Test coverage|
+        
+        BioSimulators test suite
+        ========================
+        
+        The BioSimulators test suite is a tool for validating that biosimulation
+        software tools implement the `BioSimulators standards for biosimulation
+        tools <https://biosimulators.org/standards>`__.
+        
+        The test suite is composed of two parts:
+        
+        -  A collection of example modeling projects. Each project is
+           represented by a single `COMBINE/OMEX
+           archive <https://combinearchive.org/>`__ that contains one or more
+           simulation experiments described using the `Simulation Experiment
+           Description Markup Language (SED-ML) <https://sed-ml.org>`__ and one
+           or more models described using a format such as the `BioNetGen
+           Language (BNGL) <https://bionetgen.org>`__ or the `Systems Biology
+           Markup Language (SBML) <http://sbml.org>`__.
+        
+        -  Software for checking that biosimulation tools execute these projects
+           according to the BioSimulators standards.
+        
+           -  Simulation tools support the `BioSimulators standard command-line
+              arguments <https://biosimulators.org/standards/simulator-interfaces>`__.
+           -  Simulation tools support the `BioSimulators conventions for Docker
+              images <https://biosimulators.org/standards/simulator-images>`__.
+           -  Simulation tools follow the `BioSimulators conventions for
+              executing simulations described by SED-ML files in COMBINE/OMEX
+              archives <https://biosimulators.org/standards/simulation-experiments>`__.
+           -  Simulation tools support the `BioSimulators conventions for the
+              outputs of SED-ML files in COMBINE/OMEX
+              archives <https://biosimulators.org/standards/simulation-reports>`__.
+        
+        Contents
+        --------
+        
+        -  `Installation instructions, tutorial, and API
+           documentation <#installation-instructions,-tutorial,-and-API-documentation>`__
+        -  `License <#license>`__
+        -  `Development team <#development-team>`__
+        -  `Contributing to the test suite <#contributing-to-the-test-suite>`__
+        -  `Acknowledgements <#acknowledgements>`__
+        -  `Questions and comments <#questions-and-comments>`__
+        
+        Installation instructions, tutorial, and API documentation
+        ----------------------------------------------------------
+        
+        Installation instructions, tutorial, and API documentation are available
+        `here <https://biosimulators.github.io/Biosimulators_test_suite/>`__.
+        
+        License
+        -------
+        
+        The software in this package is released under the `MIT
+        License <LICENSE>`__. The modeling projects in this package are released
+        under the `Creative Commons 1.0 Universal (CC0)
+        license <LICENSE-DATA>`__.
+        
+        Development team
+        ----------------
+        
+        This package was developed by the `Karr Lab <https://www.karrlab.org>`__
+        at the Icahn School of Medicine at Mount Sinai in New York, the
+        https://health.uconn.edu/cell-analysis-modeling/ at the University of
+        Connecticut, and the `Center for Reproducible Biomedical
+        Modeling <http://reproduciblebiomodels.org>`__.
+        
+        Contributing to the test suite
+        ------------------------------
+        
+        We enthusiastically welcome contributions to the test suite! Please see
+        the `guide to contributing <CONTRIBUTING.md>`__ and the `developer's
+        code of conduct <CODE_OF_CONDUCT.md>`__.
+        
+        Acknowledgements
+        ----------------
+        
+        This work was supported by National Institutes of Health award
+        P41EB023912.
+        
+        Questions and comments
+        ----------------------
+        
+        Please contact the `BioSimulators
+        Team <mailto:info@biosimulators.org>`__ with any questions or comments.
+        
+        .. |Latest release| image:: https://img.shields.io/github/v/release/biosimulators/Biosimulators_test_suite
+           :target: https://github.com/biosimulators/Biosimulators_test_suite/releases
+        .. |PyPI| image:: https://img.shields.io/pypi/v/Biosimulators-test-suite
+           :target: https://pypi.org/project/Biosimulators-test-suite/
+        .. |CI status| image:: https://github.com/biosimulators/Biosimulators_test_suite/workflows/Continuous%20integration/badge.svg
+           :target: https://github.com/biosimulators/Biosimulators_test_suite/actions?query=workflow%3A%22Continuous+integration%22
+        .. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_test_suite/branch/dev/graph/badge.svg
+           :target: https://codecov.io/gh/biosimulators/Biosimulators_test_suite
+        
 Keywords: systems biology modeling simulation BioSimulators
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Provides-Extra: logging
 Provides-Extra: tests
 Provides-Extra: docs
 Provides-Extra: all
-License-File: LICENSE
-License-File: LICENSE-DATA
-
-|Latest release| |PyPI| |CI status| |Test coverage| |All Contributors|
-
-BioSimulators test suite
-========================
-
-The BioSimulators test suite is a tool for validating that biosimulation
-software tools implement the `BioSimulators conventions for
-biosimulation
-tools <https://docs.biosimulations.org/concepts/conventions/>`__.
-
-The test suite is composed of two parts:
-
--  `A collection of example modeling projects <examples>`__. Each
-   project is represented by a single `COMBINE/OMEX
-   archive <https://combinearchive.org/>`__ that contains one or more
-   simulation experiments described using the `Simulation Experiment
-   Description Markup Language (SED-ML) <https://sed-ml.org>`__ and one
-   or more models described using a format such as the `BioNetGen
-   Language (BNGL) <https://bionetgen.org>`__ or the `Systems Biology
-   Markup Language (SBML) <http://sbml.org>`__.
-
--  Software for checking that biosimulation tools execute these projects
-   according to the BioSimulators conventions.
-
-   -  Simulation tools support the `BioSimulators standard command-line
-      arguments <https://docs.biosimulations.org/concepts/conventions/simulator-interfaces/>`__.
-   -  Simulation tools support the `BioSimulators conventions for Docker
-      images <https://docs.biosimulations.org/concepts/conventions/simulator-images/>`__.
-   -  Simulation tools follow the `BioSimulators conventions for
-      executing simulations described by SED-ML files in COMBINE/OMEX
-      archives <https://docs.biosimulations.org/concepts/conventions/simulation-experiments/>`__.
-   -  Simulation tools support the `BioSimulators conventions for the
-      outputs of SED-ML files in COMBINE/OMEX
-      archives <https://docs.biosimulations.org/concepts/conventions/simulation-run-reports/>`__.
-
-Installation instructions, tutorial, and API documentation
-----------------------------------------------------------
-
-Installation instructions, tutorial, and API documentation are available
-`here <https://docs.biosimulators.org/Biosimulators_test_suite/>`__.
-
-License
--------
-
-The software in this package is released under the `MIT
-License <LICENSE>`__. The modeling projects in this package are released
-under the `Creative Commons 1.0 Universal (CC0)
-license <LICENSE-DATA>`__.
-
-Development team
-----------------
-
-This package was developed by the `Karr Lab <https://www.karrlab.org>`__
-at the Icahn School of Medicine at Mount Sinai in New York, the
-`https://health.uconn.edu/cell-analysis-modeling/ <https://health.uconn.edu/cell-analysis-modeling/>`__
-at the University of Connecticut, and the `Center for Reproducible
-Biomedical Modeling <http://reproduciblebiomodels.org>`__ with
-assistance from the contributors listed `here <CONTRIBUTORS.md>`__.
-
-Contributing to the test suite
-------------------------------
-
-We enthusiastically welcome contributions to the test suite! Please see
-the `guide to contributing <CONTRIBUTING.md>`__ and the `developer's
-code of conduct <CODE_OF_CONDUCT.md>`__.
-
-Acknowledgements
-----------------
-
-This work was supported by National Institutes of Health award
-P41EB023912.
-
-Questions and comments
-----------------------
-
-Please contact the `BioSimulators
-Team <mailto:info@biosimulators.org>`__ with any questions or comments.
-
-.. |Latest release| image:: https://img.shields.io/github/v/release/biosimulators/Biosimulators_test_suite
-   :target: https://github.com/biosimulators/Biosimulators_test_suite/releases
-.. |PyPI| image:: https://img.shields.io/pypi/v/Biosimulators-test-suite
-   :target: https://pypi.org/project/Biosimulators-test-suite/
-.. |CI status| image:: https://github.com/biosimulators/Biosimulators_test_suite/workflows/Continuous%20integration/badge.svg
-   :target: https://github.com/biosimulators/Biosimulators_test_suite/actions?query=workflow%3A%22Continuous+integration%22
-.. |Test coverage| image:: https://codecov.io/gh/biosimulators/Biosimulators_test_suite/branch/dev/graph/badge.svg
-   :target: https://codecov.io/gh/biosimulators/Biosimulators_test_suite
-.. |All Contributors| image:: https://img.shields.io/github/all-contributors/biosimulators/Biosimulators_test_suite/HEAD
-   :target: #contributors-
```

### Comparing `biosimulators_test_suite-0.1.87/biosimulators_test_suite.egg-info/SOURCES.txt` & `biosimulators_test_suite-0.1.9/biosimulators_test_suite.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,34 @@
 LICENSE
-LICENSE-DATA
 MANIFEST.in
-README.md
 README.rst
 requirements.optional.txt
 requirements.txt
 setup.cfg
 setup.py
 biosimulators_test_suite/__init__.py
 biosimulators_test_suite/_version.py
 biosimulators_test_suite/config.py
 biosimulators_test_suite/data_model.py
 biosimulators_test_suite/exceptions.py
 biosimulators_test_suite/exec_cli.py
 biosimulators_test_suite/exec_core.py
 biosimulators_test_suite/exec_gh_action.py
-biosimulators_test_suite/utils.py
 biosimulators_test_suite/warnings.py
 biosimulators_test_suite.egg-info/PKG-INFO
 biosimulators_test_suite.egg-info/SOURCES.txt
 biosimulators_test_suite.egg-info/dependency_links.txt
 biosimulators_test_suite.egg-info/entry_points.txt
 biosimulators_test_suite.egg-info/requires.txt
 biosimulators_test_suite.egg-info/top_level.txt
 biosimulators_test_suite/results/__init__.py
 biosimulators_test_suite/results/data_model.py
 biosimulators_test_suite/results/io.py
 biosimulators_test_suite/test_case/__init__.py
 biosimulators_test_suite/test_case/cli.py
 biosimulators_test_suite/test_case/combine_archive.py
 biosimulators_test_suite/test_case/docker_image.py
-biosimulators_test_suite/test_case/log.py
+biosimulators_test_suite/test_case/exec_status_report.py
 biosimulators_test_suite/test_case/published_project.py
 biosimulators_test_suite/test_case/results_report.py
 biosimulators_test_suite/test_case/sedml.py
-biosimulators_test_suite/test_case/utils.py
-tests/test_config.py
-tests/test_data_model.py
-tests/test_examples.py
-tests/test_exec_cli.py
-tests/test_exec_core.py
-tests/test_exec_gh_action.py
-tests/test_utils.py
-tests/test_version.py
+biosimulators_test_suite/test_case/utils.py
```

### Comparing `biosimulators_test_suite-0.1.87/setup.py` & `biosimulators_test_suite-0.1.9/setup.py`

 * *Files identical despite different names*

