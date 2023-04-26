# Comparing `tmp/stopeight-0.3.24.tar.gz` & `tmp/stopeight-0.3.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopeight-0.3.24.tar", last modified: Wed Apr 26 17:11:40 2023, max compression
+gzip compressed data, was "stopeight-0.3.25.tar", last modified: Wed Apr 26 18:33:58 2023, max compression
```

## Comparing `stopeight-0.3.24.tar` & `stopeight-0.3.25.tar`

### file list

```diff
@@ -1,324 +1,324 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.533066 stopeight-0.3.24/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.493063 stopeight-0.3.24/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.497063 stopeight-0.3.24/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-26 17:10:37.000000 stopeight-0.3.24/.github/workflows/conda-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-26 17:10:37.000000 stopeight-0.3.24/.github/workflows/pypi-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 17:10:37.000000 stopeight-0.3.24/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 17:10:37.000000 stopeight-0.3.24/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 17:10:37.000000 stopeight-0.3.24/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 17:10:37.000000 stopeight-0.3.24/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 17:10:37.000000 stopeight-0.3.24/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 17:11:40.533066 stopeight-0.3.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 17:10:37.000000 stopeight-0.3.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.501063 stopeight-0.3.24/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.501063 stopeight-0.3.24/doc/_extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_extra/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_extra/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.501063 stopeight-0.3.24/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/cliff.svg
--rw-r--r--   0 runner    (1001) docker     (123)   235608 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/crab.png
--rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/crest.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/crest_or_sinusoid.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/extraction_sequence.svg
--rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/function_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/sinus.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/text.svg
--rw-r--r--   0 runner    (1001) docker     (123)   115146 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/vector_construction.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/vector_graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47729 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/vector_graph2.svg
--rw-r--r--   0 runner    (1001) docker     (123)    49772 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_static/vector_graph3.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.505064 stopeight-0.3.24/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/analyzer.txt
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/applications.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/build_latex.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/dev_analyzer.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/dev_build.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/dev_comparator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/dev_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/dev_stroke-analyzer.txt
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/index.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.505064 stopeight-0.3.24/doc/latex/
--rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Antis.tex
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Not_Used.tex
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Simulation.tex
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Spline_Axioms.tex
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Stopeight.bib
--rw-r--r--   0 runner    (1001) docker     (123)    24538 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Stopeight_Analyzer.tex
--rw-r--r--   0 runner    (1001) docker     (123)    34304 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Stopeight_Comparator.tex
--rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/latex/Stopeight_Grapher.tex
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.505064 stopeight-0.3.24/doc/mathematica/
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Representation_Circles.m
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Representation_Parallelogram.m
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline.m
--rw-r--r--   0 runner    (1001) docker     (123)    50428 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_CharacteristicPolynomials.nb
--rw-r--r--   0 runner    (1001) docker     (123)    39988 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_EVConstraint.nb
--rw-r--r--   0 runner    (1001) docker     (123)    50140 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_Eigensystems.nb
--rw-r--r--   0 runner    (1001) docker     (123)    33175 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_Generative.nb
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_Pascal.nb
--rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/Spline_Representation.nb
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/mathematica/SubSpaces.m
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/run_comparator.txt
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/run_editor.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/run_tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/sample-data.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/stopeight.txt
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/theory.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-26 17:10:37.000000 stopeight-0.3.24/doc/vector-graph.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 17:10:37.000000 stopeight-0.3.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 17:10:37.000000 stopeight-0.3.24/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-26 17:10:37.000000 stopeight-0.3.24/setup-dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 17:11:40.533066 stopeight-0.3.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-26 17:10:37.000000 stopeight-0.3.24/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.497063 stopeight-0.3.24/stopeight/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight/comparator/
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/lineMatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/matrixTools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/matrixTools_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/shapeMatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/shapeMatchSubSection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/comparator/vectorTools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight/multiprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/multiprocessing/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight/test/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/test/test_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/test/test_comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/test/test_grapher.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/test/test_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.533066 stopeight-0.3.24/stopeight/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/SVG.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/SVGViewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/TCT_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.533066 stopeight-0.3.24/stopeight/util/editor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/callwindow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.533066 stopeight-0.3.24/stopeight/util/editor/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/file_wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/grapher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/modules/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/scribble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/editor/wave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/tableau_printer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.533066 stopeight-0.3.24/stopeight/util/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight/util/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.505064 stopeight-0.3.24/stopeight-clibs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/Includes.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/Package.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/Versioning.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.505064 stopeight-0.3.24/stopeight-clibs/analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/analyzer/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/analyzer/python/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/analyzer/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/analyzer/python/IFPyAnalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/analyzer/turns.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/analyzer/turns.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git.h
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git_watcher.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/git_watcher.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/hello-world/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/hello-world/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/hello-world/git_watcher.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/grapher/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/algo.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/containers.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/containers.h
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/grapher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/grapher_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/iterators.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/grapher/mac/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/mac/grapher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/mean.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/mean_impl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/grapher/python/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/grapher/python/IFPyGrapher.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.493063 stopeight-0.3.24/stopeight-clibs/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/Matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/algo.h
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/analyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/angle_functions.h
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/grapher.h
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/mean.h
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/preloaderif.h
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/shared_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.509064 stopeight-0.3.24/stopeight-clibs/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.517065 stopeight-0.3.24/stopeight-clibs/legacy/include/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/analyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/areaanalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/areacalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/areanormalizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/calculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cliffs.h
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cliffsanalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cliffscalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cliffsnormalizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/corneranalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cornercalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/cornernormalizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/corners.h
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/dpoint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/editorbase.h
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/editorcliffs.h
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/editorinterface.h
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/editorspirals.h
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/error.h
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/legacy_export.h
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/legacy_global.h
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/listbase.h
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/listcopyable.h
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/listrotator.h
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/listswitchable.h
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/myreal.h
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/render.h
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/spirals.h
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/spiralsanalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/spiralscalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/straightsanalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/straightscalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/straightsnormalizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/turnanalyzer.h
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/turncalculator.h
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/turnnormalizer.h
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/include/turns.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.517065 stopeight-0.3.24/stopeight-clibs/legacy/python/
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyFinders.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyGetters.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyShared.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyShared.h
--rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/interfacepython.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/python/interfacepython.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.521065 stopeight-0.3.24/stopeight-clibs/legacy/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/analyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/areaanalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/areacalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/areanormalizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/calculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cliffs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cliffsanalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cliffscalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cliffsnormalizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/corneranalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cornercalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/cornernormalizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/corners.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/dpoint.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/editorbase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/editorcliffs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/editorspirals.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/listbase.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/listcopyable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/listrotator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/listswitchable.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/myreal.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/render.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/spirals.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/spiralsanalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/spiralscalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/straightsanalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/straightscalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/straightsnormalizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/turnanalyzer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/turncalculator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/turnnormalizer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/legacy/src/turns.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.521065 stopeight-0.3.24/stopeight-clibs/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/matrix/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/matrix/Matrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.521065 stopeight-0.3.24/stopeight-clibs/matrix/python/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/matrix/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-26 17:10:37.000000 stopeight-0.3.24/stopeight-clibs/matrix/python/IFPyMatrix.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.521065 stopeight-0.3.24/stopeight-clibs/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.493063 stopeight-0.3.24/stopeight-clibs/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    65942 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    53288 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    42720 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/typeid.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen/
--rw-r--r--   0 runner    (1001) docker     (123)    31450 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen/matrix.h
--rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen/tensor.h
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    79416 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.525065 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight-clibs/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindPythonLibsNew.cmake
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/JoinPaths.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-26 17:10:39.000000 stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11Tools.cmake
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:11:40.529066 stopeight-0.3.24/stopeight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 17:11:40.000000 stopeight-0.3.24/stopeight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.629744 stopeight-0.3.25/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.569742 stopeight-0.3.25/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.577742 stopeight-0.3.25/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-04-26 18:33:07.000000 stopeight-0.3.25/.github/workflows/conda-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-26 18:33:07.000000 stopeight-0.3.25/.github/workflows/pypi-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 18:33:07.000000 stopeight-0.3.25/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 18:33:07.000000 stopeight-0.3.25/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 18:33:07.000000 stopeight-0.3.25/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15220 2023-04-26 18:33:07.000000 stopeight-0.3.25/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 18:33:07.000000 stopeight-0.3.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 18:33:58.629744 stopeight-0.3.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-26 18:33:07.000000 stopeight-0.3.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.581742 stopeight-0.3.25/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.581742 stopeight-0.3.25/doc/_extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_extra/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_extra/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.585742 stopeight-0.3.25/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/cliff.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   235608 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/crab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13213 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/crest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15246 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/crest_or_sinusoid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/extraction_sequence.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    26892 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/function_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12623 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/sinus.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25550 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/text.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   115146 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/vector_construction.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47143 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/vector_graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47729 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/vector_graph2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    49772 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_static/vector_graph3.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.585742 stopeight-0.3.25/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/analyzer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/applications.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/build_latex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/dev_analyzer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/dev_build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/dev_comparator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/dev_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/dev_stroke-analyzer.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.585742 stopeight-0.3.25/doc/latex/
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Antis.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Not_Used.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Simulation.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Spline_Axioms.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Stopeight.bib
+-rw-r--r--   0 runner    (1001) docker     (123)    24538 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Stopeight_Analyzer.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    34304 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Stopeight_Comparator.tex
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/latex/Stopeight_Grapher.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/doc/mathematica/
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Representation_Circles.m
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Representation_Parallelogram.m
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline.m
+-rw-r--r--   0 runner    (1001) docker     (123)    50428 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_CharacteristicPolynomials.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    39988 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_EVConstraint.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    50140 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_Eigensystems.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    33175 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_Generative.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_Pascal.nb
+-rw-r--r--   0 runner    (1001) docker     (123)    27081 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/Spline_Representation.nb
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/mathematica/SubSpaces.m
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/run_comparator.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/run_editor.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/run_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/sample-data.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/stopeight.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/theory.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-04-26 18:33:07.000000 stopeight-0.3.25/doc/vector-graph.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-26 18:33:07.000000 stopeight-0.3.25/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 18:33:07.000000 stopeight-0.3.25/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-04-26 18:33:07.000000 stopeight-0.3.25/setup-dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-04-26 18:33:58.629744 stopeight-0.3.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-04-26 18:33:07.000000 stopeight-0.3.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.573742 stopeight-0.3.25/stopeight/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight/comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/lineMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/matrixTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/matrixTools_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/shapeMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/shapeMatchSubSection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/comparator/vectorTools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight/multiprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/multiprocessing/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/test/test_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/test/test_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/test/test_grapher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/test/test_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/SVG.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/SVGViewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/TCT_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.629744 stopeight-0.3.25/stopeight/util/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/callwindow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.629744 stopeight-0.3.25/stopeight/util/editor/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/file_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/grapher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/modules/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/scribble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/editor/wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/tableau_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.629744 stopeight-0.3.25/stopeight/util/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 18:33:07.000000 stopeight-0.3.25/stopeight/util/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/Includes.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/Package.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/Versioning.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/analyzer/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/analyzer/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/analyzer/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/analyzer/python/IFPyAnalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/analyzer/turns.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/analyzer/turns.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git_watcher.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/git_watcher.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.589742 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/hello-world/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/hello-world/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/hello-world/git_watcher.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.593742 stopeight-0.3.25/stopeight-clibs/grapher/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/algo.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/containers.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/containers.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/grapher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/grapher_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/iterators.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.593742 stopeight-0.3.25/stopeight-clibs/grapher/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/mac/grapher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/mean.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/mean_impl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.593742 stopeight-0.3.25/stopeight-clibs/grapher/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/grapher/python/IFPyGrapher.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.569742 stopeight-0.3.25/stopeight-clibs/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.597743 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/Matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/algo.h
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/analyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/angle_functions.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/grapher.h
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/mean.h
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/preloaderif.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/shared_types.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.597743 stopeight-0.3.25/stopeight-clibs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.605743 stopeight-0.3.25/stopeight-clibs/legacy/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/analyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/areaanalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/areacalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/areanormalizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/calculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cliffs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cliffsanalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cliffscalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cliffsnormalizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/corneranalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cornercalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/cornernormalizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/corners.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/dpoint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/editorbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/editorcliffs.h
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/editorinterface.h
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/editorspirals.h
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/error.h
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/legacy_export.h
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/legacy_global.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/listbase.h
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/listcopyable.h
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/listrotator.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/listswitchable.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/myreal.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/render.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/spirals.h
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/spiralsanalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/spiralscalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/straightsanalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/straightscalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/straightsnormalizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/turnanalyzer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/turncalculator.h
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/turnnormalizer.h
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/include/turns.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.605743 stopeight-0.3.25/stopeight-clibs/legacy/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyFinders.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyGetters.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyShared.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyShared.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/interfacepython.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/python/interfacepython.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.613743 stopeight-0.3.25/stopeight-clibs/legacy/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/analyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/areaanalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/areacalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/areanormalizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/calculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cliffs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cliffsanalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cliffscalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cliffsnormalizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/corneranalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cornercalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/cornernormalizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/corners.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/dpoint.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/editorbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/editorcliffs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/editorspirals.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/listbase.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/listcopyable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/listrotator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/listswitchable.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/myreal.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/render.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/spirals.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/spiralsanalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/spiralscalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/straightsanalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/straightscalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/straightsnormalizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/turnanalyzer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/turncalculator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/turnnormalizer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/legacy/src/turns.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.613743 stopeight-0.3.25/stopeight-clibs/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/matrix/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/matrix/Matrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.613743 stopeight-0.3.25/stopeight-clibs/matrix/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/matrix/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-04-26 18:33:08.000000 stopeight-0.3.25/stopeight-clibs/matrix/python/IFPyMatrix.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.613743 stopeight-0.3.25/stopeight-clibs/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.573742 stopeight-0.3.25/stopeight-clibs/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    65942 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28518 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    53288 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28076 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    42720 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 runner    (1001) docker     (123)    31450 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    79416 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   126420 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    94641 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15399 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21709 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.617743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.621743 stopeight-0.3.25/stopeight-clibs/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    11190 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindPythonLibsNew.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/JoinPaths.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-04-26 18:33:11.000000 stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11Tools.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:33:58.625743 stopeight-0.3.25/stopeight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 18:33:58.000000 stopeight-0.3.25/stopeight.egg-info/top_level.txt
```

### Comparing `stopeight-0.3.24/.github/workflows/conda-build.yml` & `stopeight-0.3.25/.github/workflows/conda-build.yml`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/.github/workflows/pypi-sdist.yml` & `stopeight-0.3.25/.github/workflows/pypi-sdist.yml`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/CMakeLists.txt` & `stopeight-0.3.25/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/LICENSE.txt` & `stopeight-0.3.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/MANIFEST.in` & `stopeight-0.3.25/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/PKG-INFO` & `stopeight-0.3.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopeight
-Version: 0.3.24
+Version: 0.3.25
 Summary: stopeight: Comparing sequences of points in 2 dimensions
 Home-page: https://github.com/specpose/stopeight
 Author: Fassio Blatter
 Author-email: fassio@specpose.com
 License: GNU General Public License, version 2
 Project-URL: Documentation, https://specpose.github.io/stopeight
 Keywords: signal-analysis time-series pen-stroke
```

### Comparing `stopeight-0.3.24/doc/Makefile` & `stopeight-0.3.25/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/cliff.svg` & `stopeight-0.3.25/doc/_static/cliff.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/crab.png` & `stopeight-0.3.25/doc/_static/crab.png`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/crest.svg` & `stopeight-0.3.25/doc/_static/crest.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/crest_or_sinusoid.svg` & `stopeight-0.3.25/doc/_static/crest_or_sinusoid.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/extraction_sequence.svg` & `stopeight-0.3.25/doc/_static/extraction_sequence.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/function_graph.svg` & `stopeight-0.3.25/doc/_static/function_graph.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/sinus.svg` & `stopeight-0.3.25/doc/_static/sinus.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/text.svg` & `stopeight-0.3.25/doc/_static/text.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/vector_construction.svg` & `stopeight-0.3.25/doc/_static/vector_construction.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/vector_graph.svg` & `stopeight-0.3.25/doc/_static/vector_graph.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/vector_graph2.svg` & `stopeight-0.3.25/doc/_static/vector_graph2.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/_static/vector_graph3.svg` & `stopeight-0.3.25/doc/_static/vector_graph3.svg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/analyzer.txt` & `stopeight-0.3.25/doc/analyzer.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/applications.txt` & `stopeight-0.3.25/doc/applications.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/build_latex.txt` & `stopeight-0.3.25/doc/build_latex.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/conf.py` & `stopeight-0.3.25/doc/conf.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/dev_analyzer.txt` & `stopeight-0.3.25/doc/dev_analyzer.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/dev_build.txt` & `stopeight-0.3.25/doc/dev_build.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/dev_comparator.txt` & `stopeight-0.3.25/doc/dev_comparator.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/dev_doc.txt` & `stopeight-0.3.25/doc/dev_doc.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/index.txt` & `stopeight-0.3.25/doc/index.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Antis.tex` & `stopeight-0.3.25/doc/latex/Antis.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Not_Used.tex` & `stopeight-0.3.25/doc/latex/Not_Used.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Simulation.tex` & `stopeight-0.3.25/doc/latex/Simulation.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Spline_Axioms.tex` & `stopeight-0.3.25/doc/latex/Spline_Axioms.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Stopeight.bib` & `stopeight-0.3.25/doc/latex/Stopeight.bib`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Stopeight_Analyzer.tex` & `stopeight-0.3.25/doc/latex/Stopeight_Analyzer.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Stopeight_Comparator.tex` & `stopeight-0.3.25/doc/latex/Stopeight_Comparator.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/latex/Stopeight_Grapher.tex` & `stopeight-0.3.25/doc/latex/Stopeight_Grapher.tex`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/make.bat` & `stopeight-0.3.25/doc/make.bat`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Representation_Circles.m` & `stopeight-0.3.25/doc/mathematica/Representation_Circles.m`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Representation_Parallelogram.m` & `stopeight-0.3.25/doc/mathematica/Representation_Parallelogram.m`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline.m` & `stopeight-0.3.25/doc/mathematica/Spline.m`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_CharacteristicPolynomials.nb` & `stopeight-0.3.25/doc/mathematica/Spline_CharacteristicPolynomials.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_EVConstraint.nb` & `stopeight-0.3.25/doc/mathematica/Spline_EVConstraint.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_Eigensystems.nb` & `stopeight-0.3.25/doc/mathematica/Spline_Eigensystems.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_Generative.nb` & `stopeight-0.3.25/doc/mathematica/Spline_Generative.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_Pascal.nb` & `stopeight-0.3.25/doc/mathematica/Spline_Pascal.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/Spline_Representation.nb` & `stopeight-0.3.25/doc/mathematica/Spline_Representation.nb`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/mathematica/SubSpaces.m` & `stopeight-0.3.25/doc/mathematica/SubSpaces.m`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/run_comparator.txt` & `stopeight-0.3.25/doc/run_comparator.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/sample-data.txt` & `stopeight-0.3.25/doc/sample-data.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/stopeight.txt` & `stopeight-0.3.25/doc/stopeight.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/theory.txt` & `stopeight-0.3.25/doc/theory.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/doc/vector-graph.txt` & `stopeight-0.3.25/doc/vector-graph.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/setup-dev.py` & `stopeight-0.3.25/setup-dev.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/setup.cfg` & `stopeight-0.3.25/setup.cfg`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/setup.py` & `stopeight-0.3.25/setup.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/lineMatch.py` & `stopeight-0.3.25/stopeight/comparator/lineMatch.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/matrix.py` & `stopeight-0.3.25/stopeight/comparator/matrix.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/matrixTools.py` & `stopeight-0.3.25/stopeight/comparator/matrixTools.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/matrixTools_new.py` & `stopeight-0.3.25/stopeight/comparator/matrixTools_new.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/shapeMatch.py` & `stopeight-0.3.25/stopeight/comparator/shapeMatch.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/shapeMatchSubSection.py` & `stopeight-0.3.25/stopeight/comparator/shapeMatchSubSection.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/comparator/vectorTools.py` & `stopeight-0.3.25/stopeight/comparator/vectorTools.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/logging/__init__.py` & `stopeight-0.3.25/stopeight/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/multiprocessing/pooling.py` & `stopeight-0.3.25/stopeight/multiprocessing/pooling.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/test/test_comparator.py` & `stopeight-0.3.25/stopeight/test/test_comparator.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/test/test_grapher.py` & `stopeight-0.3.25/stopeight/test/test_grapher.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/test/test_legacy.py` & `stopeight-0.3.25/stopeight/test/test_legacy.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/SVG.py` & `stopeight-0.3.25/stopeight/util/SVG.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/TCT_printer.py` & `stopeight-0.3.25/stopeight/util/TCT_printer.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/callwindow.py` & `stopeight-0.3.25/stopeight/util/editor/callwindow.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/command.py` & `stopeight-0.3.25/stopeight/util/editor/command.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/data.py` & `stopeight-0.3.25/stopeight/util/editor/data.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/dispatch.py` & `stopeight-0.3.25/stopeight/util/editor/dispatch.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/modules/file.py` & `stopeight-0.3.25/stopeight/util/editor/modules/file.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/modules/file_wave.py` & `stopeight-0.3.25/stopeight/util/editor/modules/file_wave.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/modules/grapher.py` & `stopeight-0.3.25/stopeight/util/editor/modules/grapher.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/modules/legacy.py` & `stopeight-0.3.25/stopeight/util/editor/modules/legacy.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/runnable.py` & `stopeight-0.3.25/stopeight/util/editor/runnable.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/scribble.py` & `stopeight-0.3.25/stopeight/util/editor/scribble.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/editor/wave.py` & `stopeight-0.3.25/stopeight/util/editor/wave.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/parser.py` & `stopeight-0.3.25/stopeight/util/parser.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/singleton.py` & `stopeight-0.3.25/stopeight/util/singleton.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/tableau_printer.py` & `stopeight-0.3.25/stopeight/util/tableau_printer.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight/util/test/test_util.py` & `stopeight-0.3.25/stopeight/util/test/test_util.py`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/Versioning.cmake` & `stopeight-0.3.25/stopeight-clibs/Versioning.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/analyzer/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/analyzer/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/analyzer/python/IFPyAnalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/analyzer/python/IFPyAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/analyzer/turns.h` & `stopeight-0.3.25/stopeight-clibs/analyzer/turns.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git.cc.in` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git.cc.in`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git.h` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/better-example/git_watcher.cmake` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/better-example/git_watcher.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/git_watcher.cmake` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/git_watcher.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/hello-world/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/hello-world/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/cmake-git-version-tracking/hello-world/git_watcher.cmake` & `stopeight-0.3.25/stopeight-clibs/cmake-git-version-tracking/hello-world/git_watcher.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/grapher/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/algo.cpp` & `stopeight-0.3.25/stopeight-clibs/grapher/algo.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/containers.cpp` & `stopeight-0.3.25/stopeight-clibs/grapher/containers.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/containers.h` & `stopeight-0.3.25/stopeight-clibs/grapher/containers.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/grapher.cpp` & `stopeight-0.3.25/stopeight-clibs/grapher/grapher.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/grapher_impl.h` & `stopeight-0.3.25/stopeight-clibs/grapher/grapher_impl.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/iterators.h` & `stopeight-0.3.25/stopeight-clibs/grapher/iterators.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/mean.cpp` & `stopeight-0.3.25/stopeight-clibs/grapher/mean.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/python/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/grapher/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/grapher/python/IFPyGrapher.cpp` & `stopeight-0.3.25/stopeight-clibs/grapher/python/IFPyGrapher.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/Matrix.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/Matrix.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/algo.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/algo.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/analyzer.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/analyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/angle_functions.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/angle_functions.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/grapher.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/grapher.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/mean.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/mean.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/preloaderif.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/preloaderif.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/include/stopeight-clibs/shared_types.h` & `stopeight-0.3.25/stopeight-clibs/include/stopeight-clibs/shared_types.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/legacy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/analyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/analyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/areaanalyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/areaanalyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/areacalculator.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/areacalculator.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/areanormalizer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/areanormalizer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/cliffs.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/cliffs.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/cliffsanalyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/cliffsanalyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/cliffsnormalizer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/cliffsnormalizer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/corneranalyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/corneranalyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/cornernormalizer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/cornernormalizer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/corners.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/corners.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/dpoint.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/dpoint.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/editorbase.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/editorbase.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/editorcliffs.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/editorcliffs.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/editorinterface.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/editorinterface.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/editorspirals.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/editorspirals.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/error.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/error.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/legacy_global.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/legacy_global.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/listbase.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/listbase.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/listcopyable.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/listcopyable.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/listrotator.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/listrotator.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/listswitchable.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/listswitchable.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/myreal.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/myreal.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/render.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/render.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/spirals.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/spirals.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/spiralsanalyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/spiralsanalyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/turnanalyzer.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/turnanalyzer.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/include/turncalculator.h` & `stopeight-0.3.25/stopeight-clibs/legacy/include/turncalculator.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/legacy/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyFinders.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyFinders.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyGetters.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyGetters.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyShared.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyShared.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/IFPyShared.h` & `stopeight-0.3.25/stopeight-clibs/legacy/python/IFPyShared.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/interfacepython.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/python/interfacepython.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/python/interfacepython.h` & `stopeight-0.3.25/stopeight-clibs/legacy/python/interfacepython.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/analyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/analyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/areaanalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/areaanalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/areacalculator.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/areacalculator.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/areanormalizer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/areanormalizer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/cliffs.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/cliffs.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/cliffsanalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/cliffsanalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/cliffscalculator.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/cliffscalculator.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/cliffsnormalizer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/cliffsnormalizer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/corneranalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/corneranalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/cornernormalizer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/cornernormalizer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/corners.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/corners.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/dpoint.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/dpoint.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/editorbase.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/editorbase.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/editorcliffs.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/editorcliffs.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/editorspirals.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/editorspirals.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/listbase.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/listbase.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/listcopyable.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/listcopyable.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/listrotator.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/listrotator.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/listswitchable.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/listswitchable.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/render.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/render.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/spirals.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/spirals.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/spiralsanalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/spiralsanalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/straightsanalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/straightsanalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/straightscalculator.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/straightscalculator.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/turnanalyzer.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/turnanalyzer.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/turncalculator.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/turncalculator.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/legacy/src/turns.cpp` & `stopeight-0.3.25/stopeight-clibs/legacy/src/turns.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/matrix/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/matrix/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/matrix/Matrix.cpp` & `stopeight-0.3.25/stopeight-clibs/matrix/Matrix.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/matrix/python/IFPyMatrix.cpp` & `stopeight-0.3.25/stopeight-clibs/matrix/python/IFPyMatrix.cpp`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/attr.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/buffer_info.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/cast.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/chrono.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/complex.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/class.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/common.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/descr.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/init.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/internals.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/type_caster_base.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/detail/typeid.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen/matrix.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen/matrix.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eigen/tensor.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eigen/tensor.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/embed.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/eval.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/functional.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/gil.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/iostream.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/numpy.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/operators.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/options.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/pybind11.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/pytypes.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl/filesystem.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/include/pybind11/stl_bind.h` & `stopeight-0.3.25/stopeight-clibs/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tests/test_embed/CMakeLists.txt` & `stopeight-0.3.25/stopeight-clibs/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindCatch.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindEigen3.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/FindPythonLibsNew.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/JoinPaths.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/JoinPaths.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11Common.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11NewTools.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight-clibs/pybind11/tools/pybind11Tools.cmake` & `stopeight-0.3.25/stopeight-clibs/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `stopeight-0.3.24/stopeight.egg-info/PKG-INFO` & `stopeight-0.3.25/stopeight.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopeight
-Version: 0.3.24
+Version: 0.3.25
 Summary: stopeight: Comparing sequences of points in 2 dimensions
 Home-page: https://github.com/specpose/stopeight
 Author: Fassio Blatter
 Author-email: fassio@specpose.com
 License: GNU General Public License, version 2
 Project-URL: Documentation, https://specpose.github.io/stopeight
 Keywords: signal-analysis time-series pen-stroke
```

### Comparing `stopeight-0.3.24/stopeight.egg-info/SOURCES.txt` & `stopeight-0.3.25/stopeight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

