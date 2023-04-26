# Comparing `tmp/pybdsim-3.1.1.tar.gz` & `tmp/pybdsim-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdsim-3.1.1.tar", last modified: Sat Apr 22 20:48:00 2023, max compression
+gzip compressed data, was "pybdsim-3.2.0.tar", last modified: Wed Apr 26 20:33:29 2023, max compression
```

## Comparing `pybdsim-3.1.1.tar` & `pybdsim-3.2.0.tar`

### file list

```diff
@@ -1,175 +1,176 @@
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884832 pybdsim-3.1.1/
--rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.1.1/.gitignore
--rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.1.1/COPYING.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.1.1/LICENSE.txt
--rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.1.1/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-22 20:48:00.884943 pybdsim-3.1.1/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)      924 2023-03-19 11:28:25.000000 pybdsim-3.1.1/README.md
--rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.1.1/bitbucket-pipelines.yml
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.846835 pybdsim-3.1.1/docs/
--rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/Makefile
--rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/make.bat
--rw-r--r--   0 lnevay     (501) staff       (20)  1187057 2023-04-02 21:26:31.000000 pybdsim-3.1.1/docs/pybdsim.pdf
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.852374 pybdsim-3.1.1/docs/source/
--rw-r--r--   0 lnevay     (501) staff       (20)      291 2023-03-17 15:48:00.000000 pybdsim-3.1.1/docs/source/authorship.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/classes.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.1.1/docs/source/compare.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.1.1/docs/source/conf.py
--rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.1.1/docs/source/convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.1.1/docs/source/data.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.1.1/docs/source/data_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.1.1/docs/source/developer.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.1.1/docs/source/fieldmaps.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.855233 pybdsim-3.1.1/docs/source/figures/
--rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileHistograms.png
--rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileHistogramsWrapped.png
--rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/rebdsimFileMembers.png
--rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/figures/simpleHistogramPlot.png
--rw-r--r--   0 lnevay     (501) staff       (20)      456 2023-03-22 08:08:12.000000 pybdsim-3.1.1/docs/source/index.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2107 2023-03-19 13:20:03.000000 pybdsim-3.1.1/docs/source/installation.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.1.1/docs/source/licence.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.1.1/docs/source/moduledocs.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.1.1/docs/source/support.rst
--rw-r--r--   0 lnevay     (501) staff       (20)    11351 2023-04-22 20:36:34.000000 pybdsim-3.1.1/docs/source/version_history.rst
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.855743 pybdsim-3.1.1/examples/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.856900 pybdsim-3.1.1/examples/1_builder/
--rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_builder.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_testmachine.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/1_builder/1_testmachine.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859498 pybdsim-3.1.1/examples/2_convert/
--rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_convert.rst
--rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_transport2gmad.png
--rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/2_transport2gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/transport_example.dat
--rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/transport_example.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.pdf
--rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.tar.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859721 pybdsim-3.1.1/examples/3_optics/
--rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.1.1/examples/3_optics/optics_validation.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.859986 pybdsim-3.1.1/examples/4_uproot/
--rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.1.1/examples/4_uproot/4_uproot.rst
--rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.1.1/examples/examples.rst
--rw-r--r--   0 lnevay     (501) staff       (20)     1731 2023-04-22 17:03:22.000000 pybdsim-3.1.1/pyproject.toml
--rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-04-22 20:48:00.885220 pybdsim-3.1.1/setup.cfg
--rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.1.1/setup.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843051 pybdsim-3.1.1/src/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.867704 pybdsim-3.1.1/src/pybdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.1.1/src/pybdsim/Beam.py
--rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.1.1/src/pybdsim/Builder.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.872250 pybdsim-3.1.1/src/pybdsim/Compare/
--rw-r--r--   0 lnevay     (501) staff       (20)     8639 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_BdsimBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.1.1/src/pybdsim/Compare/_ElegantBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
--rw-r--r--   0 lnevay     (501) staff       (20)    23116 2022-02-14 12:30:59.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MadxBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MadxMadxComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48472 2022-02-14 12:30:59.000000 pybdsim-3.1.1/src/pybdsim/Compare/_MultipleCodeComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Compare/_SadComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6448 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Compare/_TransportBdsimComparison.py
--rw-r--r--   0 lnevay     (501) staff       (20)      822 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Compare/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.1.1/src/pybdsim/Constants.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.875479 pybdsim-3.1.1/src/pybdsim/Convert/
--rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.1.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.1.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
--rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.1.1/src/pybdsim/Convert/_CPyMad2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_ElegantParamToStrength.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Rebdsim2Numpy.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Convert/_SadFlat2Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     4460 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Convert/_Transport2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-03-28 19:11:54.000000 pybdsim-3.1.1/src/pybdsim/Convert/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Convert/collimator_analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)    78167 2023-04-22 20:33:46.000000 pybdsim-3.1.1/src/pybdsim/Data.py
--rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.1.1/src/pybdsim/DataUproot.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.876345 pybdsim-3.1.1/src/pybdsim/Field/
--rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Field/FieldPlotter.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Field/FieldPlotterVtk.py
--rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.1.1/src/pybdsim/Field/_Field.py
--rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.1.1/src/pybdsim/Field/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.1.1/src/pybdsim/Geant4.py
--rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.1.1/src/pybdsim/Gmad.py
--rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Joinhistograms.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.1.1/src/pybdsim/ModelProcessing.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843335 pybdsim-3.1.1/src/pybdsim/Obsolete/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.878234 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/
--rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
--rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
--rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Event.py
--rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Model.py
--rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Plots.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Processed.py
--rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Root.py
--rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Run.py
--rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.1.1/src/pybdsim/Optics.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.1.1/src/pybdsim/Options.py
--rw-r--r--   0 lnevay     (501) staff       (20)    74729 2023-04-22 20:35:30.000000 pybdsim-3.1.1/src/pybdsim/Plot.py
--rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.1.1/src/pybdsim/Run.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.878907 pybdsim-3.1.1/src/pybdsim/Testing/
--rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Testing/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)    48649 2021-06-15 15:09:13.000000 pybdsim-3.1.1/src/pybdsim/Testing/bdsimMadx.py
--rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.1.1/src/pybdsim/Testing/trackingTester.py
--rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.1.1/src/pybdsim/Visualisation.py
--rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.1.1/src/pybdsim/Writer.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.1.1/src/pybdsim/XSecBias.py
--rw-r--r--   0 lnevay     (501) staff       (20)     3390 2023-03-19 12:59:36.000000 pybdsim-3.1.1/src/pybdsim/_General.py
--rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.1.1/src/pybdsim/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim/_version.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.868444 pybdsim-3.1.1/src/pybdsim.egg-info/
--rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/PKG-INFO
--rw-r--r--   0 lnevay     (501) staff       (20)     5123 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/SOURCES.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/dependency_links.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.1.1/src/pybdsim.egg-info/not-zip-safe
--rw-r--r--   0 lnevay     (501) staff       (20)      245 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/requires.txt
--rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-04-22 20:48:00.000000 pybdsim-3.1.1/src/pybdsim.egg-info/top_level.txt
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.879140 pybdsim-3.1.1/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.1.1/tests/__init__.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.880208 pybdsim-3.1.1/tests/test_input/
--rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
--rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model-aper.tfs.gz
--rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model-collsettings.dat
--rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_input/model-model.tfs.gz
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.880557 pybdsim-3.1.1/tests/test_output/
--rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/test_output/.gitkeep
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.881380 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.882124 pybdsim-3.1.1/tests/test_output/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.843893 pybdsim-3.1.1/tests/test_output2/
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.883024 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/
--rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.883781 pybdsim-3.1.1/tests/test_output2/model-model/
--rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_beam.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_components.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_options.gmad
--rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/test_output2/model-model/model_sequence.gmad
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884578 pybdsim-3.1.1/tests/tests/
--rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.1.1/tests/tests/__init__.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/tests/pybdsim_test_utils.py
--rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.1.1/tests/tests/test_MadxTfs2Gmad.py
--rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.1.1/tests/tests/testratio.py
--rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.1.1/tests/tests/write_test_outputs.py
-drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-22 20:48:00.884710 pybdsim-3.1.1/tests/unit/
--rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.1.1/tests/unit/test_Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946318 pybdsim-3.2.0/
+-rw-r--r--   0 lnevay     (501) staff       (20)      116 2023-03-19 12:01:08.000000 pybdsim-3.2.0/.gitignore
+-rw-r--r--   0 lnevay     (501) staff       (20)    35149 2020-05-18 14:14:31.000000 pybdsim-3.2.0/COPYING.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      615 2023-03-19 11:23:51.000000 pybdsim-3.2.0/LICENSE.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)      565 2023-03-17 15:48:00.000000 pybdsim-3.2.0/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-26 20:33:29.946434 pybdsim-3.2.0/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)      924 2023-03-19 11:28:25.000000 pybdsim-3.2.0/README.md
+-rw-r--r--   0 lnevay     (501) staff       (20)      960 2020-06-08 21:19:17.000000 pybdsim-3.2.0/bitbucket-pipelines.yml
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.911662 pybdsim-3.2.0/docs/
+-rw-r--r--   0 lnevay     (501) staff       (20)      611 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/Makefile
+-rw-r--r--   0 lnevay     (501) staff       (20)      809 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/make.bat
+-rw-r--r--   0 lnevay     (501) staff       (20)  1197598 2023-04-26 20:32:00.000000 pybdsim-3.2.0/docs/pybdsim.pdf
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.914553 pybdsim-3.2.0/docs/source/
+-rw-r--r--   0 lnevay     (501) staff       (20)      291 2023-03-17 15:48:00.000000 pybdsim-3.2.0/docs/source/authorship.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5049 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2784 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/classes.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5251 2022-02-14 12:30:59.000000 pybdsim-3.2.0/docs/source/compare.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     5444 2023-03-19 13:19:27.000000 pybdsim-3.2.0/docs/source/conf.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    20082 2021-06-15 15:09:13.000000 pybdsim-3.2.0/docs/source/convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11964 2023-03-19 11:16:47.000000 pybdsim-3.2.0/docs/source/data.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3032 2023-03-19 12:42:38.000000 pybdsim-3.2.0/docs/source/data_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1448 2023-04-02 20:14:28.000000 pybdsim-3.2.0/docs/source/developer.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    12892 2023-03-29 08:13:29.000000 pybdsim-3.2.0/docs/source/fieldmaps.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.915709 pybdsim-3.2.0/docs/source/figures/
+-rw-r--r--   0 lnevay     (501) staff       (20)   459915 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileHistograms.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   536529 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileHistogramsWrapped.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   287477 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/rebdsimFileMembers.png
+-rw-r--r--   0 lnevay     (501) staff       (20)   196253 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/figures/simpleHistogramPlot.png
+-rw-r--r--   0 lnevay     (501) staff       (20)      468 2023-04-26 11:59:44.000000 pybdsim-3.2.0/docs/source/index.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2107 2023-03-19 13:20:03.000000 pybdsim-3.2.0/docs/source/installation.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      679 2023-03-19 13:16:04.000000 pybdsim-3.2.0/docs/source/licence.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     2827 2023-03-17 15:47:53.000000 pybdsim-3.2.0/docs/source/moduledocs.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     3420 2023-04-26 14:47:31.000000 pybdsim-3.2.0/docs/source/plotting.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      558 2020-05-18 14:14:31.000000 pybdsim-3.2.0/docs/source/support.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)    11854 2023-04-26 14:49:01.000000 pybdsim-3.2.0/docs/source/version_history.rst
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.915939 pybdsim-3.2.0/examples/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.917608 pybdsim-3.2.0/examples/1_builder/
+-rw-r--r--   0 lnevay     (501) staff       (20)      396 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_builder.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   348736 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_testmachine.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      379 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/1_builder/1_testmachine.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.922961 pybdsim-3.2.0/examples/2_convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)    84758 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      165 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1068 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_convert.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)   107428 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_transport2gmad.png
+-rwxr-xr-x   0 lnevay     (501) staff       (20)      184 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/2_transport2gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)   134154 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/transport_example.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)    19220 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/transport_example.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    24970 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.pdf
+-rw-r--r--   0 lnevay     (501) staff       (20)    21778 2020-05-18 14:14:31.000000 pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.tar.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.923160 pybdsim-3.2.0/examples/3_optics/
+-rw-r--r--   0 lnevay     (501) staff       (20)     4703 2023-03-19 12:30:43.000000 pybdsim-3.2.0/examples/3_optics/optics_validation.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.923407 pybdsim-3.2.0/examples/4_uproot/
+-rw-r--r--   0 lnevay     (501) staff       (20)      943 2023-03-19 11:16:47.000000 pybdsim-3.2.0/examples/4_uproot/4_uproot.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)      446 2023-03-19 11:16:47.000000 pybdsim-3.2.0/examples/examples.rst
+-rw-r--r--   0 lnevay     (501) staff       (20)     1731 2023-04-22 17:03:22.000000 pybdsim-3.2.0/pyproject.toml
+-rw-r--r--   0 lnevay     (501) staff       (20)      257 2023-04-26 20:33:29.946752 pybdsim-3.2.0/setup.cfg
+-rw-r--r--   0 lnevay     (501) staff       (20)       38 2023-03-19 11:23:22.000000 pybdsim-3.2.0/setup.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.908655 pybdsim-3.2.0/src/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.927912 pybdsim-3.2.0/src/pybdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)    12864 2023-03-17 15:50:15.000000 pybdsim-3.2.0/src/pybdsim/Beam.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    71670 2023-03-29 08:02:12.000000 pybdsim-3.2.0/src/pybdsim/Builder.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.930554 pybdsim-3.2.0/src/pybdsim/Compare/
+-rw-r--r--   0 lnevay     (501) staff       (20)     8655 2023-04-26 11:56:15.000000 pybdsim-3.2.0/src/pybdsim/Compare/_BdsimBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    10617 2023-03-29 08:03:23.000000 pybdsim-3.2.0/src/pybdsim/Compare/_ElegantBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    14701 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    28319 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    23115 2023-04-26 11:54:49.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MadxBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      294 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MadxMadxComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48470 2023-04-26 11:55:02.000000 pybdsim-3.2.0/src/pybdsim/Compare/_MultipleCodeComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3641 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Compare/_SadComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6448 2023-04-26 11:55:20.000000 pybdsim-3.2.0/src/pybdsim/Compare/_TransportBdsimComparison.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      822 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Compare/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2584 2023-04-22 20:29:56.000000 pybdsim-3.2.0/src/pybdsim/Constants.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.934297 pybdsim-3.2.0/src/pybdsim/Convert/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2801 2023-03-28 19:08:52.000000 pybdsim-3.2.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12960 2023-03-28 19:07:59.000000 pybdsim-3.2.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    24068 2023-03-28 19:16:33.000000 pybdsim-3.2.0/src/pybdsim/Convert/_CPyMad2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3984 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_ElegantParamToStrength.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12045 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    30913 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    34813 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    37650 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     6282 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     1561 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Rebdsim2Numpy.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12293 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Convert/_SadFlat2Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     4460 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Convert/_Transport2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1115 2023-03-28 19:11:54.000000 pybdsim-3.2.0/src/pybdsim/Convert/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1044 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Convert/collimator_analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    78167 2023-04-22 20:33:46.000000 pybdsim-3.2.0/src/pybdsim/Data.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    69562 2023-04-10 18:48:13.000000 pybdsim-3.2.0/src/pybdsim/DataUproot.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.934869 pybdsim-3.2.0/src/pybdsim/Field/
+-rwxr-xr-x   0 lnevay     (501) staff       (20)    19403 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Field/FieldPlotter.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2427 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Field/FieldPlotterVtk.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    16881 2023-04-17 18:48:37.000000 pybdsim-3.2.0/src/pybdsim/Field/_Field.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      981 2023-04-22 17:06:38.000000 pybdsim-3.2.0/src/pybdsim/Field/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2704 2023-03-17 15:47:53.000000 pybdsim-3.2.0/src/pybdsim/Geant4.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    18652 2023-04-17 19:55:26.000000 pybdsim-3.2.0/src/pybdsim/Gmad.py
+-rwxr-xr-x   0 lnevay     (501) staff       (20)     2654 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Joinhistograms.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3648 2023-04-10 22:16:41.000000 pybdsim-3.2.0/src/pybdsim/ModelProcessing.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.908956 pybdsim-3.2.0/src/pybdsim/Obsolete/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.936887 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/
+-rw-r--r--   0 lnevay     (501) staff       (20)     3587 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4482 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      934 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     5562 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Event.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      348 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Model.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      353 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      115 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Plots.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3276 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Processed.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    11554 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Root.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      479 2020-05-18 14:14:31.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Run.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      513 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    15291 2023-03-29 19:06:12.000000 pybdsim-3.2.0/src/pybdsim/Optics.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12066 2023-03-19 13:13:38.000000 pybdsim-3.2.0/src/pybdsim/Options.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    76164 2023-04-26 14:35:42.000000 pybdsim-3.2.0/src/pybdsim/Plot.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     9630 2023-03-19 13:00:55.000000 pybdsim-3.2.0/src/pybdsim/Run.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.937880 pybdsim-3.2.0/src/pybdsim/Testing/
+-rw-r--r--   0 lnevay     (501) staff       (20)       25 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Testing/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    48656 2023-04-26 11:55:44.000000 pybdsim-3.2.0/src/pybdsim/Testing/bdsimMadx.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    12119 2020-05-18 15:11:01.000000 pybdsim-3.2.0/src/pybdsim/Testing/trackingTester.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     2484 2023-03-19 13:02:51.000000 pybdsim-3.2.0/src/pybdsim/Visualisation.py
+-rw-r--r--   0 lnevay     (501) staff       (20)    25579 2023-03-19 13:03:02.000000 pybdsim-3.2.0/src/pybdsim/Writer.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3125 2020-05-18 17:03:47.000000 pybdsim-3.2.0/src/pybdsim/XSecBias.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     3358 2023-04-26 09:53:42.000000 pybdsim-3.2.0/src/pybdsim/_General.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     4658 2023-04-22 20:04:46.000000 pybdsim-3.2.0/src/pybdsim/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      160 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim/_version.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.928662 pybdsim-3.2.0/src/pybdsim.egg-info/
+-rw-r--r--   0 lnevay     (501) staff       (20)     2090 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/PKG-INFO
+-rw-r--r--   0 lnevay     (501) staff       (20)     5148 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/SOURCES.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/dependency_links.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        1 2023-03-19 11:36:13.000000 pybdsim-3.2.0/src/pybdsim.egg-info/not-zip-safe
+-rw-r--r--   0 lnevay     (501) staff       (20)      245 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/requires.txt
+-rw-r--r--   0 lnevay     (501) staff       (20)        8 2023-04-26 20:33:29.000000 pybdsim-3.2.0/src/pybdsim.egg-info/top_level.txt
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.938126 pybdsim-3.2.0/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       13 2020-06-08 21:19:17.000000 pybdsim-3.2.0/tests/__init__.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.939693 pybdsim-3.2.0/tests/test_input/
+-rw-r--r--   0 lnevay     (501) staff       (20)   122327 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)   137539 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model-aper.tfs.gz
+-rw-r--r--   0 lnevay     (501) staff       (20)      459 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model-collsettings.dat
+-rw-r--r--   0 lnevay     (501) staff       (20)   231976 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_input/model-model.tfs.gz
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.940140 pybdsim-3.2.0/tests/test_output/
+-rw-r--r--   0 lnevay     (501) staff       (20)        0 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/test_output/.gitkeep
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.942494 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      281 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27567 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.943291 pybdsim-3.2.0/tests/test_output/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5311 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.909513 pybdsim-3.2.0/tests/test_output2/
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.944144 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/
+-rw-r--r--   0 lnevay     (501) staff       (20)      277 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      424 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    27349 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     9339 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.944947 pybdsim-3.2.0/tests/test_output2/model-model/
+-rw-r--r--   0 lnevay     (501) staff       (20)      269 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      478 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_beam.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)     5281 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_components.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)      112 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_options.gmad
+-rw-r--r--   0 lnevay     (501) staff       (20)    10521 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/test_output2/model-model/model_sequence.gmad
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946029 pybdsim-3.2.0/tests/tests/
+-rw-r--r--   0 lnevay     (501) staff       (20)       31 2023-03-17 15:49:55.000000 pybdsim-3.2.0/tests/tests/__init__.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1359 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/tests/pybdsim_test_utils.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     8239 2020-05-18 17:03:47.000000 pybdsim-3.2.0/tests/tests/test_MadxTfs2Gmad.py
+-rw-r--r--   0 lnevay     (501) staff       (20)      631 2022-02-14 12:30:59.000000 pybdsim-3.2.0/tests/tests/testratio.py
+-rw-r--r--   0 lnevay     (501) staff       (20)     1424 2020-05-18 15:11:01.000000 pybdsim-3.2.0/tests/tests/write_test_outputs.py
+drwxr-xr-x   0 lnevay     (501) staff       (20)        0 2023-04-26 20:33:29.946186 pybdsim-3.2.0/tests/unit/
+-rw-r--r--   0 lnevay     (501) staff       (20)     9948 2020-05-18 14:14:31.000000 pybdsim-3.2.0/tests/unit/test_Builder.py
```

### Comparing `pybdsim-3.1.1/COPYING.txt` & `pybdsim-3.2.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/LICENSE.txt` & `pybdsim-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/Makefile` & `pybdsim-3.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/PKG-INFO` & `pybdsim-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.1.1/README.md` & `pybdsim-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/bitbucket-pipelines.yml` & `pybdsim-3.2.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/Makefile` & `pybdsim-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/make.bat` & `pybdsim-3.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/pybdsim.pdf` & `pybdsim-3.2.0/docs/pybdsim.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 8% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 pybdsim Documentation
-Release 3.1.0
+Release 3.2.0
 
 Royal Holloway
 
-Apr 02, 2023
+Apr 26, 2023
 
 CONTENTS
 
 1
 
 Licence & Disclaimer
 
@@ -113,143 +113,162 @@
 33
 33
 
 i
 
 9
 
-Field Maps
-9.1 Loading . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.2 Writing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.3 Creation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.4 Visualisation and Plotting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.5 Conversion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.6 Sorting Points . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-9.7 Importance of Order . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Plotting
+9.1 BDSIM Optics . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+9.2 Histogram Plotting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+9.3 Energy Deposition . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+9.4 Machine Diagrams For Plots . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 35
 35
 35
-36
-39
-40
-40
-40
-
-10 Utility Classes
-10.1 General Classes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-10.2 Specialised Classes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-41
-41
-42
+37
+37
 
-11 Support
-11.1 Feature Request . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10 Field Maps
+10.1 Loading . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.2 Writing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.3 Creation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.4 Visualisation and Plotting . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.5 Conversion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.6 Sorting Points . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+10.7 Importance of Order . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
+39
+39
+39
+40
 43
-43
+44
+44
+44
 
-12 Version History
-12.1 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.2 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.3 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.4 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.5 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.6 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.7 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.8 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.9 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.10 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.11 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.12 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.13 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.14 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-12.15 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+11 Utility Classes
+11.1 General Classes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+11.2 Specialised Classes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 45
 45
-45
-45
 46
+
+12 Support
+12.1 Feature Request . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
 47
 47
-47
-48
-48
+
+13 Version History
+13.1 V3.2.0 - 2023 / 04 / 26 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.2 V3.1.1 - 2023 / 04 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.3 V3.1.0 - 2023 / 04 / 02 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.4 V3.0.1 - 2023 / 03 / 22 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.5 V3.0.0 - 2023 / 03 / 19 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.6 v2.4.0 - 2021 / 06 / 16 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.7 v2.3.0 - 2020 / 12 / 15 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.8 v2.2.0 - 2020 / 06 / 08 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.9 v2.1 - 2019 / 04 / 20 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.10 v2.0 - 2019 / 02 / 27 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.11 v1.9 - 2018 / 08 / 24 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.12 v1.8 - 2018 / 06 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.13 v1.7 - 2018 / 06 / 30 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.14 v1.6 - 2018 / 05 / 23 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.15 v1.5 - 2018 / 05 / 17 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.16 v1.4 - 2018 / 10 / 04 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+13.17 v1.3 - 2017 / 12 / 05 . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+
+49
 49
 49
 49
 50
 50
 51
-
-13 Module Contents
-13.1 pybdsim.Beam module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.2 pybdsim.Builder module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.3 pybdsim.Compare . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.4 pybdsim.Constants module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.5 pybdsim.Convert . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.6 pybdsim.Data module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.7 pybdsim.Field module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.8 pybdsim.Gmad module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.9 pybdsim.ModelProcessing module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.10 pybdsim.Options module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.11 pybdsim.Plot module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.12 pybdsim.Run module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.13 pybdsim.Visualisation module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.14 pybdsim.Writer module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-13.15 pybdsim.XSecBias module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
+51
+52
+52
+52
 53
 53
 54
-63
-64
-64
-69
-75
-81
-83
-83
-86
-91
-92
-92
-94
+54
+54
+55
+55
 
-14 Developer Documentation
-14.1 Release Checklist . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14 Module Contents
+14.1 pybdsim.Beam module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.2 pybdsim.Builder module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.3 pybdsim.Compare . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.4 pybdsim.Constants module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.5 pybdsim.Convert . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.6 pybdsim.Data module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.7 pybdsim.Field module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.8 pybdsim.Gmad module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.9 pybdsim.ModelProcessing module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.10 pybdsim.Options module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.11 pybdsim.Plot module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.12 pybdsim.Run module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.13 pybdsim.Visualisation module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.14 pybdsim.Writer module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+14.15 pybdsim.XSecBias module . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-97
-97
+57
+57
+58
+67
+68
+68
+73
+79
+85
+87
+87
+90
+95
+96
+96
+99
 
-15 Indices and tables
+15 Developer Documentation
 
-99
+101
+
+ii
+
+15.1 Release Checklist . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 101
+16 Indices and tables
+
+103
 
 Python Module Index
 
-101
+105
 
 Index
 
-103
+107
 
-ii
+iii
+
+iv
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim is a Python package to aid in the preparation, running and validation of BDSIM models.
 
 CONTENTS
 
 1
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 2
 
 CONTENTS
 
 CHAPTER
 
@@ -263,15 +282,15 @@
 pybdsim is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
 Public License for more details.
 You should have received a copy of the GNU General Public License along with pybdsim. If not, see <http:
 //www.gnu.org/licenses/>.
 
 3
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 4
 
 Chapter 1. Licence & Disclaimer
 
 CHAPTER
 
@@ -291,15 +310,15 @@
 • William Shields
 • Jochem Snuverink
 • Robin Tesse
 • Stuart Walker
 
 5
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 6
 
 Chapter 2. Authorship
 
 CHAPTER
 
@@ -333,15 +352,15 @@
 • pymadx
 • pymad8
 • pytransport
 These are all available through pip and will be automatically installed.
 
 7
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 Optional:
 • ROOT Python interface
 
 3.2 Local Installation
 Although on pip, for development purposes you may wish to use pybdsim from a copy of the source code. It is
 possible to clone the git repository and use pip to point at the local set of files, or generally install that set of files
@@ -391,15 +410,15 @@
 File:
 ~/physics/reps/pybdsim/Builder.py
 Type:
 instancemethod
 
 9
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 4.2 Adding Options
 No options are required to run the most basic BDSIM model. However, it is often advantageous to specify at least
 a few options such as the physics list and default aperture. To add options programmatically, there is an options
 class. This is instantiated and then ‘setter’ methods are used to set values of parameters. This options instance can
 then be associated with a machine instance. For example:
 >>> o = pybdsim.Options.Options()
@@ -431,15 +450,15 @@
 >>> a = pybdsim.Builder.Machine()
 >>> a.Write('outputfilename')
 
 10
 
 Chapter 4. Building Models
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 4.5 Units
 The user may supply units as strings that will be written to the gmad syntax as a Python tuple. For example:
 >>> a = pybdsim.Builder.Machine()
 >>> a.AddDrift('d1', (3.2, 'm'))
 This will result in the following gmad syntax:
 >>> print a[0]
@@ -465,15 +484,15 @@
 Anywhere you see a function with the last argument as **kwargs, this feature can be used.
 The arguments included in the function signatures are the minimum arguments required for functionality.
 
 4.5. Units
 
 11
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 12
 
 Chapter 4. Building Models
 
 CHAPTER
 
@@ -507,15 +526,15 @@
 where SEQUENCENAME is the name of the sequence in madx. By not specifying the output columns, a very large
 file is produced containing all possible columns. This is required to successfully convert the lattice. If the tfs file
 contains insufficient information, pybdsim will not be able to convert the model.
 Note: The python utilities require “.tfs” suffix as the file type to work properly.
 
 13
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 5.1.2 Converting the Tfs File
 Once prepared, the Tfs file can be converted. The converter is used as follows:
 >>> pybdsim.Convert.MadxTfs2Gmad('inputfile.tfs', 'latticev1')
 The conversion returns three objects, which are the pybdsim.Builder.Machine instance as converted, a second
 Machine that isn’t split by aperture and a list of any ommitted items by name.
 >>> a,b,c = pybdsim.Convert.MadxTfs2Gmad('inputfile.tfs', 'latticev1')
@@ -526,15 +545,15 @@
 will create a directory test if it doesn’t exist already.
 There are a few options that provide useful functionality for conversion:
 
 14
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -626,15 +645,15 @@
 Do not append an integer to the base file name if it already exists. Instead
 overwrite the files.
 15
 Treat every row in the TFS file/instance as a unique element. This makes
 it easier to edit individual components as they are guaranteed to appear
 only once in the entire resulting GMAD lattice.
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 The user may convert only part of the input model by specifying startname and stopname.
 Generally speaking, extra information can be folded into the conversion via a user supplied dictionary with extra
 parameters for a particular element by name. For a given element, for example ‘drift123’, extra parameters can
 be speficied in a dictionary. This leads to a dictionary of dictionaries being supplied. This is a relatively simple
 structure the user may prepare from their own input format and converters in Python. For example:
 >>> drift123dict = {'aper1':0.03, 'aper2':0.05, 'apertureType':'rectangular'}
@@ -672,15 +691,15 @@
 2. echo variables in the mad8 job log (SIGPT, SIGT)
 3. converting the tape files to gmad using pybdsim
 
 16
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 5.3.1 Running mad8
 The following variables need to be defined in the Mad8 job from a BETA0
 EMITX
 EMITY
 BLENG
 ESPRD
@@ -744,15 +763,15 @@
 pybdsim.Convert.Mad8MakeApertureTemplate(<inputtwissfilename>,<aperturedbfilename>)
 Copy the <collimatordbfilename> to collimator.dat and <aperturedbfilename> to apertures.dat Once prepared, the Tape files can be converted. The converter is used as follows:
 
 5.3. Mad8Twiss2Gmad (using saved TWISS output)
 
 17
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim.Convert.Mad8Twiss2Gmad(<inputtwissfilename>,<outputgamdfilename>)
 
 5.4 pytransport
 https://bitbucket.org/jairhul/pytransport is a separate utility to convert transport models into BDSIM ones.
 
 5.5 BDSIM Primaries To Others
@@ -785,15 +804,15 @@
 The primary BDSIM coordinates are converted to a BDSIM userFile format. The converter is used as follows:
 >>> pybdsim.Convert.BdsimPrimaries2BdsimUserFile('output.root', 'inrays.dat')
 
 18
 
 Chapter 5. Converting Models
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 5.5.4 BdsimSampler2BdsimUserFile
 The BDSIM coordinates from a provided sampler name are converted to a BDSIM userFile format. The converter
 is used as follows:
 >>> pybdsim.Convert.BdsimSampler2BdsimUserFile('output.root', 'inrays.dat','DR1')
 The time coordinate recorded in the input file will be finite if the sampler being converted is not at the start of the
 machine. This function is intended to convert particles into a primary distribution, therefore the time coordinate
@@ -809,15 +828,15 @@
 The primary BDSIM coordinates are converted to mad8 format. The converter is used as follows:
 >>> pybdsim.Convert.BdsimPrimaries2Mad8('output.root', 'inrays.dat')
 
 5.5. BDSIM Primaries To Others
 
 19
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 20
 
 Chapter 5. Converting Models
 
 CHAPTER
 
@@ -850,15 +869,15 @@
 present, these should be set to zero strength but must remain in the lattice. The pybdsim.Convert.MadxTfs2Gmad
 converter for example provides a boolean flag to convert the lattice with only linear optical components. The user
 may of course proceed with non-linear magnetic fields included but it is only useful to compare the sigma in each
 dimension to a similarly similuated distribution and not the Twiss parameters.
 
 21
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 6.1.2 Analysing Optical Data
 The rebdsim tool can be used with an input analysisConfig.txt that specifies CalculateOpticalFunctions to 1 or true
 in the header (see BDSIM manual). Or the specially prepared optics tool rebdsimOptics can be used to achieve the
 same outcome - we recommend this. In the terminal:
 rebdsimOptics bdsimRawOutputFile.root optics.root
 This may take a few minutes to process. This analyses the file from the BDSIM run called ‘bdsimRawOutputFile.root’ and produces another ROOT file called optics.root with a different structure. This output file contains
@@ -887,15 +906,15 @@
 Two BDSIM optics files can also be compared with the following command:
 >>> pybdsim.Compare.BDSIMVsBDSIM('optics1.root', 'optics2.root')
 
 22
 
 Chapter 6. Model Comparison
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 6.5 Comparing to PTC
 BDSIM output can be compared to the PTC output from the PTC_TRACK routine available in MADX. The PTC
 output is written to a file typically named trackone, however it is necessary to convert this into a BDSIM-like ROOT
 output file. This can be easily accomplished with the ptc2bdsim tool, however the particle species and nominal
 momentum is required to correctly convert to the BDSIM coordinate convention. An example terminal command:
 ptc2bdsim trackone ptc.root proton 0.9999
@@ -908,15 +927,15 @@
 With the help of pytransport a TRANSPORT “FOR002” output file that has sigma matrices can be read and compared with BDSIM output:
 >>> pybdsim.Compare.TransportVsBDSIM('FOR002.DAT', 'bdsim_optics.root')
 
 6.5. Comparing to PTC
 
 23
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 24
 
 Chapter 6. Model Comparison
 
 CHAPTER
 
@@ -958,15 +977,15 @@
 'Event/MergedHistograms/PlossHisto': <pybdsim.Data.TH1 at 0x15503aeb0>,
 'Event/MergedHistograms/ElossHisto': <pybdsim.Data.TH1 at 0x15503aee0>,
 'Event/MergedHistograms/PhitsPEHisto': <pybdsim.Data.TH1 at 0x15503af10>,
 (continues on next page)
 
 25
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 (continued from previous page)
 
 'Event/MergedHistograms/PlossPEHisto': <pybdsim.Data.TH1 at 0x15503af40>,
 'Event/MergedHistograms/ElossPEHisto': <pybdsim.Data.TH1 at 0x15503af70>,
 'Event/MergedHistograms/PFirstAIHisto': <pybdsim.Data.TH1 at 0x15503afa0>,
 'Event/MergedHistograms/ElossTunnelHisto': <pybdsim.Data.TH1 at 0x15503afd0>,
@@ -1000,21 +1019,21 @@
 ˓→'])
 Note, the use of d.histogramspy for the wrapped set of histograms and not the raw ROOT histograms.
 
 26
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 7.4. Histogram Plotting
 
 27
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 7.5 ROOT Histogram Operations
 Loaded histograms from a rebdsim file are both wrapped in our pybdsim.Data.THX classes for nice numpy arrays
 for easy plotting, but also we retain the original ROOT objects.
 We can use the original ROOT objects to do many very useful things with the histogram, then wrap it again for
 plotting.
 1) Get the ROOT histogram from the loaded file in pybdsim
@@ -1032,21 +1051,21 @@
 • https://root.cern.ch/doc/master/classTH1.html
 • https://root.cern.ch/doc/master/classTH2D.html
 • https://root.cern.ch/doc/master/classTH3D.html
 28
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 7.5. ROOT Histogram Operations
 
 29
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 TH1 is, perhaps nonintuitively, the base class for 2D and 3D histograms, so many functions are documented there.
 The 2D and 3D ones have some specialised methods.
 Note: The integral and its error are nicely provided as members in pybdsim.Data.THXD. Also, you can use the
 pybdsim.Plot.Histogram. . . functions with a scaling parameter for the data.
 Some useful functions assuming a histogram h of type TH1D or TH2D or TH3D in Python:
 TH1
@@ -1086,15 +1105,15 @@
 ROOT Jargon
 • “Profile” histogram is an average in 1 dimension, not a ‘profile’ as per the real meaning of the word.
 • “Projection” means integral.
 30
 
 Chapter 7. Data Loading
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 7.6 Python Histogram Operations
 Some of the above operations are provided in functions of pybdsim.Data.TH2 and pybdsim.Data.TH3 - the ‘Python’
 versions in pybdsim.
 See pybdsim.Data module and look for each of the classes there, where their functions are listed.
 Some specifically for 3D histograms (i.e. often scoring meshes) are described below.
 
@@ -1134,15 +1153,15 @@
 # now the same as pybdsim.Data.Load("run1.root")
 (continues on next page)
 
 7.6. Python Histogram Operations
 
 31
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 (continued from previous page)
 
 model = pybdsim.Data.GetModelForPlotting(d)
 
 7.9 Sampler Data
 Warning: This is a simplified way of loading sampler data that “flattens” the structure losing all concept of
@@ -1199,15 +1218,15 @@
 >>> import pybdsim
 >>> d = pybdsim.DataUproot.BDSimOutput("output.root")
 >>> samplers = d.event.samplers
 samplers is a dictionary where keys are the name of the samplers and values are an instance of pybdsim.DataUproot.BDSimOutput.Event.Sampler. Data can be easily converted in a pandas.DataFrame using:
 
 33
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 >>> samplers['sampler_name'].df
 The primary beam can be extracted using the same procedure:
 >>> primary_beam = d.event.primary
 
 8.1.3 Optics Files
 After loading the file using pybdsim.DataUproot.ReBDSimOpticsOutput, the optics of the line can be accessed
@@ -1237,46 +1256,143 @@
 
 Chapter 8. Data Loading Using Uproot
 
 CHAPTER
 
 NINE
 
+PLOTTING
+
+pybdsim includes functions for common plots useful for BDSIM.
+
+9.1 BDSIM Optics
+With a model, use sample, all; in the input GMAD to give a sampler behind every element. Then calculate the
+optics and plot just those on their own.
+bdsim --file=mymodel.gmad --outfile=o1 --batch --ngenerate=5000
+rebdsimOptics o1.root
+ls
+o1.root
+o1_optics.root
+>>> pybdsim.Plot.BDSIMOptics("o1_optics.root")
+
+9.2 Histogram Plotting
+9.2.1 1D Histogram
+Loaded histograms that are wrapped in our pybdsim.Data.THX classes can be plotted:
+>>> pybdsim.Plot.Histogram1D(d.histogramspy['Event/PerEntryHistograms/EnergyLossManual
+˓→'])
+Note, the use of d.histogramspy for the wrapped set of histograms and not the raw ROOT histograms.
+
+9.2.2 2D Histogram
+See pybdsim.Plot.Histogram2D
+
+35
+
+pybdsim Documentation, Release 3.2.0
+
+36
+
+Chapter 9. Plotting
+
+pybdsim Documentation, Release 3.2.0
+
+9.2.3 Spectra
+>>> d = pybdsim.Data.Load("ana1.root")
+>>> d.spectra
+defaultdict(pybdsim.Data.Spectra,
+{'t10_0': <pybdsim.Data.Spectra at 0x28eaf3cd0>,
+'tax_0': <pybdsim.Data.Spectra at 0x290ed6f90>,
+'col1_0': <pybdsim.Data.Spectra at 0x290ed78d0>,
+'col2_0': <pybdsim.Data.Spectra at 0x290edc150>,
+'col3_0': <pybdsim.Data.Spectra at 0x290edca10>,
+'interface_0': <pybdsim.Data.Spectra at 0x290edd090>,
+'interface_1': <pybdsim.Data.Spectra at 0x290eddad0>})
+>>> pybdsim.Plot.Spectra(d.spectra["t10_0"])
+
+9.3 Energy Deposition
+bdsim --file=mymodel.gmad --outfile=run1 --batch --ngenerate=1000
+rebdsimHistoMerge run1.root
+>>> pybdsim.Plot.EnergyDeposition("run1_histos.root")
+
+9.4 Machine Diagrams For Plots
+For a plot or histogram that follows the accelerator along its axis (e.g. S coordinate), it is common to draw a small
+schematic of the various elements in the accelerator above the plot. pybdsim provides functionality to make such
+diagrams using information from a BDSIM output file or from a MADX Twiss output in a TFS file.
+Information is accepted from the following sources:
+• BDSIM raw output file (from bdsim, bdskim, bdsimCombine)
+• REBDSIM output file (from rebdsim or rebdsimCombine)
+• MADX Twiss output in a TFS file
+• BDSIM survey text output
+Each can be supplied as either a string giving the file name or as an already loaded object in python.
+The main function of interest is pybdsim.Plot.AddMachineLatticeFromSurveyToFigure.
+
+9.4.1 REBDSIM Output
+>>> import pybdsim
+>>> d = pybdsim.Data.Load("ana1.root") # a rebdsim output file
+>>> f = pybdsim.Plot.Histogram1D(d.histogramspy["Event/MergedHistograms/ElossHisto"])
+>>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, d.model)
+or
+>>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, d)
+or
+
+9.3. Energy Deposition
+
+37
+
+pybdsim Documentation, Release 3.2.0
+
+>>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, "ana1.root")
+
+9.4.2 BDSIM Survey
+bdsim --file=mymodel.gmad --output=none --batch --ngenerate=1 --survey=survey1
+This produces the file survey1.dat for example, for some input model mymodel.gmad.
+>>> import pybdsim
+>>> d = pybdsim.Data.Load("ana1.root") # a rebdsim output file
+>>> f = pybdsim.Plot.Histogram1D(d.histogramspy["Event/MergedHistograms/ElossHisto"])
+>>> pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(f, "survey.dat")
+
+38
+
+Chapter 9. Plotting
+
+CHAPTER
+
+TEN
+
 FIELD MAPS
 
 The pybdsim.Field module has several functions and classes to help create, convert, and visualise BDSIM-format
 field maps easier. Various useful workflows are described below, but every function and class is documented in:
 pybdsim.Field module.
 
-9.1 Loading
+10.1 Loading
 Existing BDSIM-format field maps can be loaded with:
 fm = pybdsim.Field.Load("nameOfFieldMap.dat")
 This will automatically detect the number of dimensions in the field map and load it into a numpy array inside a
 pybdsim class. The class is one of:
 • pybdsim.Field.Field1D
 • pybdsim.Field.Field2D
 • pybdsim.Field.Field3D
 • pybdsim.Field.Field4D
 These all have member variables such as:
 • data - the numpy array of the field map data
 • columns - a list of column names
 • header - a dictionary of all information in the header
 
-9.2 Writing
+10.2 Writing
 Al of the pybdsim classes described in Loading (e.g. Field3D) have a method called Write. This will write out
 the instance of that class (i.e. that particular field map data) to a BDSIM-format field map file.
 Therefore, these classes represent a a very good route for creation and conversion of field maps. The recommended
 strategy is to get the information into one of those classes then it can be written out to file, loaded, plotted with
 ease.
 
-35
+39
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-9.3 Creation
+10.3 Creation
 A field map can be created from scratch in Python from knowledge of a field, such as an equation. A numpy array
 of the right shape should be created, then an instance of pybdsim.Field.Field[N]D created (where N is one of
 (1,2,3,4).
 Creating the array is entirely up to the user as this depends on how they get the information. However, a small
 example script is shown below here (in Python language):
 import numpy as np
 import pybdsim
@@ -1312,36 +1428,36 @@
 object with the same contents as the original Field2D instance.
 The array should be structured to contain the coordinates and field components at each point. So for a 2D field
 map, this would be: (𝑥, 𝑦, 𝐹𝑥 , 𝐹𝑦 , 𝐹𝑧 ). The array would then have 2 dimensions representing its structure. So if
 the field map had 10 points in x and 20 in y, it would ultimately be a numpy array with the shape (10,20,5).
 Generally, the numpy.shape(array) would look like:
 • 1D: (N_x, 4)
 
-36
+40
 
-Chapter 9. Field Maps
+Chapter 10. Field Maps
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • 2D: (N_x, N_y, 5)
 • 3D: (N_x, N_y, N_z, 6)
 • 4D: (N_x, N_y, N_z, N_t, 7)
 Warning: A key check is looking at the field map, the higher dimension coordinates (e.g. Y, not X) should
 change first. So for a given X value we should see the Y values cycle through a range, then the X should
 increment then the Y values cycle again. If this is not the case, then the loop order of dimensions is backwards.
 You can use “loopOrder” in the header or rewrite the field map correctly.
 
-9.3.1 Alternative Dimensions
+10.3.1 Alternative Dimensions
 In the case of alternative dimension (e.g. a 2D field map with x and z dimensions but no y), the construction is the
 same but we can label the dimensions differently. The dimensions must be in order (e.g. x, y, z, then t for whichever
 ones are used).
 Example:
 fm = pybdsim.Field.Field2D(arrayData, firstColumn='X', secondColumn='Z')
 
-9.3.2 Alternative Loop Order
+10.3.2 Alternative Loop Order
 It is possible for BDSIM to read a file where the right-most coordinate column varies first. However, for each value,
 the coordinate columns must still be in x,y,z,t order left to right. Below is an example similar to above but writing
 out the file the other way (note the write function). This will also write the line loopOrder> tzyx in the header
 so BDSIM can load the field map equivalently.
 import numpy as np
 import pybdsim
 fx, fy, fz = 0.0, 1.0, 0.0
@@ -1363,19 +1479,19 @@
 # this will be written out in the BDSIM conventional looping order
 f = pybdsim.Field.Field2D(data, flip=True)
 f.Write("box-field-map.dat')
 Below is a script included with bdsim (bdsim/examples/features/maps_bdsim/Generate2DLoopOrder.
 py) that shows 4 ways to write a field map with the same information. Ultimately, they convey the exact same field
 map to BDSIM although the file contents differ (2 sets of possible contents).
 
-9.3. Creation
+10.3. Creation
 
-37
+41
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 import numpy as _np
 import pybdsim
 B = 2.0
 # LOOP METHOD 1
 data = []
 # loop over and build up 3d lists of lists of lists
@@ -1411,21 +1527,21 @@
 # around, so we use flip=True when constructing the field instance
 g = pybdsim.Field.Field2D(data2, flip=True, secondColumn='Z')
 # this will write out a file identical to the very first one
 g.Write('2dexample_loopOrder_for_zx.dat')
 # this will write out a file identical to the second one
 g.Write('2dexample_loopOrder_for_zx_tzyx.dat', writeLoopOrderReversed=True)
 
-38
+42
 
-Chapter 9. Field Maps
+Chapter 10. Field Maps
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-9.4 Visualisation and Plotting
+10.4 Visualisation and Plotting
 To visualise a field map, it is possible to do so in BDSIM / Geant4. See the BDSIM manual for this information.
 This draws a selection of arrows in the 3D model and gives a rough indication that the field map is as intended.
 An alternative way is to load the data in pybdsim in Python and plot it, either fully or in slices (for 3D or 4D maps).
 Any library desired can be used in Python and the classes described above in Loading provide an excellent way to
 get a numpy array, that is ubiquitous in Python programming and libraries.
 pybdsim provides a variety of small plotting functions mostly for 1D and 2D field maps using Matplotlib. These
 functions are inside the pybdsim.Field module and all start with Plot. A list is:
@@ -1454,21 +1570,21 @@
 Plot a bdsim field map file using the X,Y plane.
 :param filename: name of field map file or object
 :type filename: str, pybdsim.Field._Field.Field2D instance
 :param scale: numerical scaling for quiver plot arrow lengths.
 :type scale: float
 >>>
 
-9.4. Visualisation and Plotting
+10.4. Visualisation and Plotting
 
-39
+43
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-9.5 Conversion
+10.5 Conversion
 your data -> numpy array -> pybdsim.Field.FieldND(data) class
 To convert a field map, you should first write a loader from your own format to the field map into a numpy array
 with a structure described in Creation. Then, this array can be wrapped in an instance of one of the pybdsim Field
 classes. This class can then be used to write out the field map in BDSIM’s format. This would look something
 like:
 def LoadMyFormatFieldMap(filename):
 # ... some implementation...
@@ -1481,47 +1597,47 @@
 bd.Write(outputfilename)
 The source of a field map data should represent an equally spaced grid of points and provided in order, such that it
 can be converted easily to BDSIM’s format with the various classes.
 Note: See Importance of Order. Make sure to validate the order with plots before using in a simulation in BDSIM.
 You can also visualise the fields in BDSIM to check. It is recommended to do this with a single component before
 using in a bigger model.
 
-9.6 Sorting Points
+10.6 Sorting Points
 If the data points for the field map correspond to a rectilinear grid but are not provided in order (sometimes
 can happen from finite-element programs), you should ideally try to get a field map in order. Failing that,
 you can try to sort the data into an ordered array. An example implementation is given in pybdsim.Field.
 SortUnorderedFieldMap2D. Although, this is provided there is no guarantee the implementation will work depending on the numerical precision of the coordinates. It is still recommended to go back to the origin field program
 and get a correct grid of points.
 
-9.7 Importance of Order
+10.7 Importance of Order
 In a BDSIM field map file, the coordinates at each point are written but BDSIM itself does not use these. BDSIM
 reads the header information and loops over the data assuming the number of points specified in the header. Therefore if the data is provided in the wrong order the field map will appear scrambled in BDSIM. This can happen
 with hand-preparation and editing of files.
 It is recommended to use the pybdsim.Field classes as these are guaranteed to write the data out correctly.
 Plots that use arrows or stream plots do not depend on the order of the points so they cannot be relied upon to tell
 if the field map being prepared is in the correct order. Use Plot2DXYMagnitude or Plot2DXYConnectionOrder to
 verify the order of the points.
 
-40
+44
 
-Chapter 9. Field Maps
+Chapter 10. Field Maps
 
 CHAPTER
 
-TEN
+ELEVEN
 
 UTILITY CLASSES
 
 Various classes are provided for the construction of BDSIM input definitions. There are classes defined in
 pybdsim.Builder that allow writing of an object without any checks. Also, there are some specialised classes
 listed here that exist in pybdsim that include some checking and utility functions.
 Once a class is constructed, converting to a string in Python will produce a string in BDSIM input syntax that can
 be written to a file.
 
-10.1 General Classes
+11.1 General Classes
 • pybdsim.Builder.Aperture
 • pybdsim.Builder.Atom
 • pybdsim.Builder.BLM
 • pybdsim.Builder.CavityModel
 • pybdsim.Builder.Crystal
 • pybdsim.Builder.Field
 • pybdsim.Builder.Material
@@ -1537,107 +1653,123 @@
 >>> a = pybdsim.Builder.Aperture('aperDef1', aper1=3, aper2=(2.5,'cm'))
 >>> str(a)
 'aperDef1: aperture, aper1=3, aper2=2.5*cm;\n'
 Acceptable types are int, float, str, list, tuple(number, str). In the case of a tuple (e.g. ()), it should contain 2 items
 and the second is the units string.
 An example with a list:
 
-41
+45
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 >>> sp = pybdsim.Builder.SamplerPlacement('z350mL',
 z=(350,'m'),
 shape="rectangular",
 aper1=(5,'m'),
 aper2=(5,'m'),
 partID=[13,-13])
 >>> str(sp)
 'z350mL: samplerplacement, shape="rectangular", partID={13,-13}, aper1=5.0*m,␣
 ˓→z=350.0*m, aper2=5.0*m;\n'
 
 Note: The keyword arguments are not checked. One could write “bananas=5” and it would be used, but ultimately
 would have no meaning to BDSIM.
 
-10.2 Specialised Classes
-10.2.1 Beam.Beam
+11.2 Specialised Classes
+11.2.1 Beam.Beam
 This beam class represents a beam definition in gmad syntax. The class has ‘setter’ functions that are added
 dynamically based on the distribution type selected.:
 >>> b = pybdsim.Beam.Beam()
 >>> b.SetParicleType("proton")
 >>> b.SetDistributionType("reference")
 
-10.2.2 Options.Options
+11.2.2 Options.Options
 This class provides the set of options for BDSIM. Please see pybdsim.Options module for more details.
 
-10.2.3 XSecBias.XSecBias
+11.2.3 XSecBias.XSecBias
 This class provides the definition process biasing in BDSIM. Please see pybdsim.XSecBias module for more details.
 
-42
+46
 
-Chapter 10. Utility Classes
+Chapter 11. Utility Classes
 
 CHAPTER
 
-ELEVEN
+TWELVE
 
 SUPPORT
 
 All support issues can be submitted to our issue tracker
 
-11.1 Feature Request
+12.1 Feature Request
 Feature requests or proposals can be submitted to the issue tracker - select the issue type as proposal or enhancement..
 Please have a look at the existing list of proposals before submitting a new one.
 
-43
+47
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-44
+48
 
-Chapter 11. Support
+Chapter 12. Support
 
 CHAPTER
 
-TWELVE
+THIRTEEN
 
 VERSION HISTORY
 
-12.1 V3.1.0 - 2023 / 04 / 02
+13.1 V3.2.0 - 2023 / 04 / 26
+• Remove the function pybdsim.Plot.AddMachineLatticeToFigure(). This was just a forward to
+pymadx.Plot.AddMachineLatticeToFigure() and this should be used explicitly for machine diagram
+plotting for TFS files. Otherwise, pybdsim.Plot.AddMachineLatticeFromSurveyToFigure should be
+used.
+• Better documentation about plotting.
+• Increase the visibility of light grey elements in the machine diagram from alpha 0.1 to 0.4.
+
+13.2 V3.1.1 - 2023 / 04 / 23
+• Fixed spectra loading and plotting for when the ‘p’ and ‘s’ prefixes are used in the rebdsim Spectra command
+to denote primary and secondary particles.
+• Fixed error with default log scale in Plot.Histogram2D when no vmin was specified.
+• Fix pybdsim._version_tuple which should be pybdsim.__version_tuple__.
+• Fix import without awkward array which is only required for the [uproot] feature of pybdsim.
+• pybdsim.Plot.Spectra() now makes more than one plot if more than 8 particles are specified.
+• Recognised PDG ID 0 as “total” from BDSIM.
+
+13.3 V3.1.0 - 2023 / 04 / 02
 • Add the writing and reading of comment lines in field maps.
 • Reduce print out when loading a field map.
 • Clean imports in cpymad interface as well as in Convert functions.
 
-12.2 V3.0.1 - 2023 / 03 / 22
+49
+
+pybdsim Documentation, Release 3.2.0
+
+13.4 V3.0.1 - 2023 / 03 / 22
 • Fix import for pybdsim when ROOT is present but librebdsim etc. are not available through environmental
 variables, or findable. Would cause induce a classic ROOT segfault when importing pybdsim.
 • Fix wrong exception being raised.
 • Always write a comment string at the start of a BDSIM field map file to specify the units of the file.
 
-12.3 V3.0.0 - 2023 / 03 / 19
+13.5 V3.0.0 - 2023 / 03 / 19
 • Restructure package into a declarative Python package where all source files are now in src/pybdsim/.
 • The package now has a feature called uproot for the optional dependencies of uproot, pandas, and pint
 packages.
 • Field classes no longer have flip=True as the default - it is now False. Please check any field maps created
 by scripts using these classes.
 
-12.3.1 New Features
+13.5.1 New Features
 • Add a module to load BDSIM output file, included rebdsim files with uproot.
 • Create a nice Python copy of the header information from any (re)bdsim file when loading with pybdsim
 using only Python types.
 • New integration for 2D histograms along each axis to 1D histograms.
 • New slices for 3D histograms as well as integrating along a dimension (‘projection’). See 3D Scoring Histograms.
 • New ratio plot for 2x 1D histograms. See pybdsim.Plot.Histogram1DRatio.
 • New loading and handling of 4D histograms (from BDSIM with Boost). They can now be loaded and handled
 similarly to 1,2,3D histograms. They are loaded automatically when loading a rebdsim file.
-
-45
-
-pybdsim Documentation, Release 3.1.0
-
 • pybdsim.Data.TH1,2,3 now have xrange, yrange, and zrange members where appropriate with a convenient tuple of the range in each dimension. They also have the member integral and integralError
 taken from their ROOT objects.
 • Field plotting functions now tolerate Field class objects as well as filenames to make it easier to check field
 objects as you’re making them.
 • New field plotting for 2D field maps showing each component.
 • New field reflection utility function pybdsim.Field.MirrorDipoleQuadrant1 for 2D fields.
 • New field plotting function pybdsim.Field.Plot2DXYConnectionOrder to see the order an array is written in.
@@ -1645,222 +1777,222 @@
 • New field plotting function pybdsim.Field.Plot1DFxFyFz to see field components in 1D.
 • Field loading automatically works for dimensions such as X, Z for 2D instead of X, Y now.
 • Ability to load a rebdsim output file and only load the ROOT histograms without loading the BDSIM and
 rebdsim shared libraries, so it can be used on a separate computer with just ROOT.
 • Added classes to Builder for all GMAD objects. New ones include aperture, atom, blm, cavitymodel, crystal,
 field, material, newcolour, query, region, samplerplacement, scorer, tunnel, xsecbias.
 
-12.3.2 Bug Fixes
+50
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.2.0
+
+13.5.2 Bug Fixes
 • pybdsim would throw an exception that librebdsim and libbdsimRootEvent could not be loaded and stop if the
 libraries had been already loaded separately outside pybdsim. This has been fixed by fixing the interpretation
 of the error codes from ROOT.
 • Fix warning about “nonposy” in matplotlib version for log scales.
 • Fix check in Run of if it’s a ROOT file or not. Simplify it to use file extension.
 • Tolerate no pytransport installation.
 • Fix loading of aperture data from a BDSIM output file.
 • Fix loading of model data.
 • Fix aperture plots from a BDSIM output file.
 
-12.3.3 General
+13.5.3 General
 • The Beam class now takes distrType and not distrtype so as to match BDSIM syntax and be less confusing.
 • Updated out of date documentation.
 • Better automatic ranges for Histogram1DMultiple plots by default.
 • Better field loading in pybdsim.Field.Load. Returns the same Field object from pybdsim as you would write.
 
-12.4 v2.4.0 - 2021 / 06 / 16
-12.4.1 New Features
+13.6 v2.4.0 - 2021 / 06 / 16
+13.6.1 New Features
 • Transform3D function in a Machine.
 • Crystal, ScorerMesh and Placement also can be added to a Machine.
 • Ability to insert and replace an element in a machine.
 
-46
-
-Chapter 12. Version History
-
-pybdsim Documentation, Release 3.1.0
-
-12.4.2 Bug Fixes
+13.6.2 Bug Fixes
 • Python 3.8+ warnings fixed.
 • Add ROOT_INCLUDE_PATH to ROOT as newer versions don’t do this automatically.
 • Fixed vmin for 2D histogram plot.
 
-12.5 v2.3.0 - 2020 / 12 / 15
-12.5.1 New Features
+13.7 v2.3.0 - 2020 / 12 / 15
+13.7.1 New Features
 • Convenience functions for pickling and un-pickling data in the Data module with optional compression.
 • Generic loss map plot.
 
-12.6 v2.2.0 - 2020 / 06 / 08
-12.6.1 New Features
+13.6. v2.4.0 - 2021 / 06 / 16
+
+51
+
+pybdsim Documentation, Release 3.2.0
+
+13.8 v2.2.0 - 2020 / 06 / 08
+13.8.1 New Features
 • Support for Python3.
 
-12.7 v2.1 - 2019 / 04 / 20
-12.7.1 New Featuers
+13.9 v2.1 - 2019 / 04 / 20
+13.9.1 New Featuers
 • Optional flag of whether to write out the converted model with pybdsim.Convert.MadxTfs2Gmad.
 • Machine builder now supports new bdsim jcol element.
 • Machine diagram drawing can now start from any arbitrary S location.
 • For loaded histograms (using pybdsim.Data.TH1, TH2, TH3 classes, there are now functions ErrorsToSTD()
 and ErrorsToErrorOnMean() to easily convert between the different types of error - the default is error on
 the mean.
 • New plotting function pybdsim.Plot.Histogram2DErrors to visualise 2D histogram errors.
 
-12.7.2 General
+13.9.2 General
 • Return arguments of pybdsim.Convert.MadxTfs2Gmad is now just 2 items - machine and omitted items.
 Previously 3.
 
-12.7.3 Bug Fixes
+13.9.3 Bug Fixes
 • Fix loading of Model tree from ROOT output given some recent collimation variables may have a different
 structure or type from the existing ones.
 • In pybdsim.Plot.Histogram2D, the y log scale argument was “ylocscale” and is fixed to “yLogScale”.
 
-12.5. v2.3.0 - 2020 / 12 / 15
-
-47
-
-pybdsim Documentation, Release 3.1.0
-
-12.8 v2.0 - 2019 / 02 / 27
-12.8.1 New Features
+13.10 v2.0 - 2019 / 02 / 27
+13.10.1 New Features
 • Machine diagram plotting automatically from BDSIM output. Compatible with newer BDSIM output format.
 • Support for thin R matrix, parallel transporter and thick R matrix in builder.
 • Generate transfer matrix from tracking data from BDSIM for a single element.
 • Control over legend location in standard energy deposition and loss plots.
 • Utility function to write sampler data from BDSIM output to a user input file.
 • Support for energy variation in the beam line in MAD8 conversion.
 
-12.8.2 General
+52
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.2.0
+
+13.10.2 General
 • Remove dependency of root_numpy. pybdsim now uses only standard ROOT interfaces.
 • Update physics lists.
 
-12.8.3 Bug Fixes
+13.10.3 Bug Fixes
 • Fix bug where calling pybdsim.Plot.PrimaryPhaseSpace with an output file name would result in an error as
 this argument was wrongly supplied to the number of bins argument.
 • Fix for hidden scientific notation when using machine diagram.
 • Fix TH1 TH2 TH3 histogram x,y,z highedge variables in histogram loading. These were the lowedge duplicated, which was wrong.
 • Add missing variables from sampler data given changes in BDSIM.
 
-12.9 v1.9 - 2018 / 08 / 24
-12.9.1 General
+13.11 v1.9 - 2018 / 08 / 24
+13.11.1 General
 • Significant new tests.
 • Trajectory loading from BDSIM ROOT output.
 • Plot trajectories.
 • New padding function for 1D histogram to ensure lines in plots.
 • New value replacement function for histograms to ensure continuous line in log plots.
 • Control over aspect ration in default 2D histogram plots.
 • New classes for each element in the Builder.
 • Refactor of MadxTfs2Gmad to use new classes in Builder.
 
-48
-
-Chapter 12. Version History
-
-pybdsim Documentation, Release 3.1.0
-
-12.9.2 Bug Fixes
+13.11.2 Bug Fixes
 • Fix orientation of 2D histograms in plotting.
 • Fix header information labels when writing field maps with reversed order.
 
-12.10 v1.8 - 2018 / 06 / 23
-12.10.1 General
+13.12 v1.8 - 2018 / 06 / 23
+13.12.1 General
 • Setup requires pytest-runner.
 • Introduction of testing.
 • Removed line wrapping written to GMAD files in Builder.
 • “PlotBdsimOptics” is now “BDSIMOptics” in the Plot module.
 • New comparison plots for arbitrary inputs from different tracking codes.
 • Prepare PTC coordinates from any BDSIM sampler.
 
-12.10.2 Bug Fixes
+13.11. v1.9 - 2018 / 08 / 24
+
+53
+
+pybdsim Documentation, Release 3.2.0
+
+13.12.2 Bug Fixes
 • Fixes for “Optics” vs “optics” naming change in ROOT files.
 
-12.11 v1.7 - 2018 / 06 / 30
-12.11.1 General
+13.13 v1.7 - 2018 / 06 / 30
+13.13.1 General
 • Can specify which dimension in Field class construction (i.e. ‘x’:’z’ instead of default ‘x’:’y’).
 
-12.11.2 Bug Fixes
+13.13.2 Bug Fixes
 • ‘nx’ and ‘ny’ were written the wrong way around from a 2D field map in pybdsim.
 
-12.12 v1.6 - 2018 / 05 / 23
-12.12.1 Bug Fixes
+13.14 v1.6 - 2018 / 05 / 23
+13.14.1 Bug Fixes
 • Fix machine diagram plotting from BDSIM survey.
 • Fix machine diagram searching with right-click in plots.
 
-12.10. v1.8 - 2018 / 06 / 23
-
-49
-
-pybdsim Documentation, Release 3.1.0
-
-12.13 v1.5 - 2018 / 05 / 17
-12.13.1 New Features
+13.15 v1.5 - 2018 / 05 / 17
+13.15.1 New Features
 • Function now public to create beam from Madx TFS file.
 • Improved searching for BDSAsciiData class.
 • Ability to easily write out beam class.
 • Plot phase space from any sampler in a BDSIM output file.
 • __version__ information in package.
 • Get a column from data irrespective of case.
 • Coded energy deposition plot. Use for example for labelling cyrogenic, warm and collimator losses.
 • Improved Transport BDSIM comparison.
 • Function to convert a line from a TFS file into a beam definition file.
 
-12.13.2 Bug Fixes
+13.15.2 Bug Fixes
 • Fix library loading given changes to capitalisation in BDSIM.
 • Beam class now supports all BDSIM beam definitions.
 • Support all aperture shapes in Builder.
 • Fixes for loading optics given changes to capitalisation and BDSAsciiData class usage.
 • Fixes for collimator conversion from MADX.
 
-12.14 v1.4 - 2018 / 10 / 04
-12.14.1 New Features
+54
+
+Chapter 13. Version History
+
+pybdsim Documentation, Release 3.2.0
+
+13.16 v1.4 - 2018 / 10 / 04
+13.16.1 New Features
 • Full support for loading BDSIM output formats through ROOT.
 • Extraction of data from ROOT histograms to numpy arrays.
 • Simple histogram plotting from ROOT files.
 • Loading of sampler data and simple extraction of phase space data.
 • Line wrapping for elements with very long definitions.
 • Comparison plots standardised.
 • New BDSIM BDSIM comparison.
 • New BDSIM Mad8 comparison.
 • Support for changes to BDSIM data format variable renaming in V1.0
 
-50
-
-Chapter 12. Version History
-
-pybdsim Documentation, Release 3.1.0
-
-12.14.2 Bug Fixes
+13.16.2 Bug Fixes
 • Correct conversion of all dispersion component for Beam.
 • Don’t write all multipole components if not needed.
 • Fixed histogram plotting.
 • Fixed conversion of coordinates in BDSIM2PtcInrays for subrelativistic particles.
 • Fixed behaviour of fringe field fint and fintx behaviour from MADX.
 • Fixed pole face angles given MADX writes out wrong angles.
 • Fixed conversion of multipoles and other components for ‘linear’ flag in MadxTfs2Gmad.
 • Fixed axis labels in field map plotting utilities.
 • MADX BDSIM testing suite now works with subrelativistic particles.
 • Many small fixes to conversion.
 
-12.15 v1.3 - 2017 / 12 / 05
-12.15.1 New Features
+13.17 v1.3 - 2017 / 12 / 05
+13.17.1 New Features
 • GPL3 licence introduced.
 • Compatibility with PIP install system.
 • Manual.
 • Testing suite.
 
-12.15. v1.3 - 2017 / 12 / 05
+13.16. v1.4 - 2018 / 10 / 04
 
-51
+55
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-52
+56
 
-Chapter 12. Version History
+Chapter 13. Version History
 
 CHAPTER
 
-THIRTEEN
+FOURTEEN
 
 MODULE CONTENTS
 
 This documentation is automatically generated by scanning all the source code. Parts may be incomplete.
 pybdsim - python tool for BDSIM.
 Copyright Royal Holloway, University of London 2023.
 Module
@@ -1883,59 +2015,59 @@
 
 Description
 Create generic accelerators for BDSIM.
 Comparison of optics between different codes.
 Constants.
 Convert other formats into gmad.
 Read the bdsim output formats.
-Data loading with uproot instead of pyroot.
+Data loading with uproot instead of pyroot. (optional)
 Read and write BDSIM field format files.
 Dictionary that contains process and subprocess IDs
 Create bdsim input files - lattices & options.
 Tools to process existing BDSIM models and generate other versions of them.
-Optical calculation in development.
+Optical calculation in development. (optional)
 Methods to generate bdsim options.
 Some nice plots for data.
 Run BDSIM programatically.
 Help locate objects in the BDSIM visualisation, requires a BDSIM survey file.
 Write various objects from Builder.
 
 Class
 Beam
 XSecBias
 
 Description
 A beam options dictionary with methods.
 A cross-section biasing object.
 
-13.1 pybdsim.Beam module
+14.1 pybdsim.Beam module
 Module containing a similarly named Beam class for creating a BDSIM beam distribution programmatically.
 class pybdsim.Beam.Beam(particleType='e-', energy=1.0, distrType='reference', *args, **kwargs)
 Bases: dict
 ReturnBeamString()
 SetDistributionType(distrType='reference')
 SetE0(e0=1, unitsstring='GeV')
 SetEnergy(energy=1.0, unitsstring='GeV')
 
-53
+57
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 SetParticleType(particleType='e-')
 SetS0(s0=0, unitsstring='m')
 SetT0(t0=0.0, unitsstring='s')
 SetX0(x0=0.0, unitsstring='m')
 SetXP0(xp0=0.0)
 SetY0(y0=0.0, unitsstring='m')
 SetYP0(yp0=0.0)
 SetZ0(z0=0.0, unitsstring='m')
 SetZP0(zp0=0.0)
 WriteToFile(filename)
 
-13.2 pybdsim.Builder module
+14.2 pybdsim.Builder module
 Builder
 Build generic machines for bdsim. You can create a lattice using one of the predefined simple lattices or by adding
 many pieces together of your own design. Finally, output the gmad files required.
 Classes: Element - beam line element that always has name,type and length Machine - a list of elements
 class pybdsim.Builder.Aperture(name, **kwargs)
 Bases: GmadObject
 A crystal definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
@@ -1951,19 +2083,19 @@
 Bases: GmadObject
 A blmplacement definition. Any kwargs will be written as parameter=value. parameter=(value,unit) ->
 parameter=value*unit
 class pybdsim.Builder.CavityModel(name, **kwargs)
 Bases: GmadObject
 A cavitymodel definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 
-54
+58
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim.Builder.CreateDipoleDriftRing(filename, ncells=60, circumference=100.0, driftfraction=0.1,
 samplers='first')
 Create a ring composed of dipoles and drifts filename ncells - number of cells, each containing 1 dipole and
 a drift circumference - in metres driftfraction - the fraction of drift in each cell (0.0 < driftfraction < 1.0)
 samplers - ‘first’, ‘last’ or ‘all’
 pybdsim.Builder.CreateDipoleFodoRing(filename, ncells=60, circumference=200.0,
@@ -2003,19 +2135,19 @@
 advantage that built in printing or string conversion provides BDSIM syntax.
 Element(name,type,**kwargs)
 >>> a = Element("d1", "drift", l=1.3)
 >>> b = Element("qx1f", "quadrupole", l=(0.4,'m'), k1=0.2, aper1=(0.223,'m'))
 >>> print(b)
 (continues on next page)
 
-13.2. pybdsim.Builder module
+14.2. pybdsim.Builder module
 
-55
+59
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 (continued from previous page)
 
 qx1f: quadrupole, k1=0.2, l=0.4*m, aper1=0.223*m;
 >>> str(c)
 qx1f: quadrupole, k1=0.2, l=0.4*m, aper1=0.223*m\n;
 A beam line element must ALWAYs have a name, and type. The keyword arguments are specific to the type
@@ -2052,19 +2184,19 @@
 This results in the quadrupole strength k1 in this example being changed to 0.0245.
 class pybdsim.Builder.ExternalGeometry(name, l, outerDiameter, geometryFile, **kwargs)
 Bases: Element
 class pybdsim.Builder.Field(name, **kwargs)
 Bases: GmadObject
 A field definition. Any kwargs will be written as parameter=value. parameteter=(value,unit) -> parameter=value*unit
 
-56
+60
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Builder.Gap(name, l, **kwargs)
 Bases: Element
 pybdsim.Builder.GenerateSamplersFromBDSIMSurvey(surveyfile, outputfilename,
 excludesamplers=True)
 Create a gmad file with samplers for all the elements in a beamline as described by the survey outline from
 bdsim
@@ -2101,19 +2233,19 @@
 Return a string that contains the lines required to define each element in the Line.
 Example using predefined Elements name ‘d1’ and ‘q1’:
 >>> l = Line([d1,q1])
 >>> f = open("file.txt", "w")
 >>> f.write(l.DefineConsituentElements())
 >>> f.close()
 
-13.2. pybdsim.Builder module
+14.2. pybdsim.Builder module
 
-57
+61
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Builder.Machine(verbose=False, sr=False, energy0=0.0, charge=-1.0)
 Bases: object
 A class represents an accelerator lattice as a sequence of components. Member functions allow various lattice
 components to be append to the sequence of the machine. This class allows the user to programatically create
 a lattice and write the BDSIM gmad representation of it.
 Example:
@@ -2150,19 +2282,19 @@
 AddElement(name='el', length=0.1, outerDiameter=1, geometryFile='geometry.gdml', **kwargs)
 AddFodoCell(basename, magnetlength, driftlength, kabs, **kwargs)
 basename - the basename for the fodo cell beam line elements magnetlength - length of magnets in
 metres driftlength - length of drift segment in metres kabs - the absolute value of the quadrupole strength
 - alternates between magnets
 kwargs are other parameters for bdsim - ie material=’Fe’
 
-58
+62
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 AddFodoCellMultiple(basename='fodo', magnetlength=1.0, driftlength=4.0, kabs=0.2, ncells=2,
 **kwargs)
 AddFodoCellSplitDrift(basename, magnetlength, driftlength, kabs, nsplits, **kwargs)
 basename - the basename for the fodo cell beam line elements magnetlength - length of magnets in
 metres driftlength - length of drift segment in metres kabs - the absolute value of the quadrupole strength
 - alternates between magnets nsplits - number of segments drift length is split into
@@ -2197,19 +2329,19 @@
 AddOctupole(name='oc', length=0.1, k3=0.0, **kwargs)
 AddOptions(options=None)
 Assign an options instance to this machine.
 AddPlacement(name, **kwargs)
 AddQuadrupole(name='qd', length=0.1, k1=0.0, **kwargs)
 AddRBend(name='rb', length=0.1, angle=None, b=None, **kwargs)
 
-13.2. pybdsim.Builder module
+14.2. pybdsim.Builder module
 
-59
+63
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 AddRCol(name='rc', length=0.1, xsize=0.1, ysize=0.1, **kwargs)
 AddRFCavity(name='arreff', length=0.1, gradient=10, **kwargs)
 AddRmat(name='rmat', length=0.1, r11=1.0, r12=0, r13=0, r14=0, r21=0, r22=1.0, r23=0, r24=0,
 r31=0, r32=0, r33=1.0, r34=0, r41=0, r42=0, r43=0, r44=1.0, **kwargs)
 AddSBend(name='sb', length=0.1, angle=None, b=None, **kwargs)
 AddSampler(names)
@@ -2242,19 +2374,19 @@
 Change category of all elements of a given category. All parameters of the element being changed will
 be preserved, please update with the UpdateCategoryParameter function.
 ReplaceWithElement(name, newelement, warnAboutLengthDifference=True)
 Replace an element in the machine with a new element object (one of the individual element pybdsim.Builder classes that inherit the Element class).
 SynchrotronRadiationRescale()
 Rescale all component strengths for SR
 
-60
+64
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 UpdateCategoryParameter(category, parameter, value)
 Update parameter for all elements of a given category.
 UpdateElement(name, parameter, value)
 Update a parameter for a specified element name. Modifying element length will produce a warning.
 If a value for that parameter already exists, the value will be overwritten.
 UpdateElements(names, parameter, value, namelocation='all')
@@ -2288,19 +2420,19 @@
 class pybdsim.Builder.Placement(name, **kwargs)
 Bases: GmadObject
 A placement definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 pybdsim.Builder.PrepareApertureModel(rowDictionary, default='circular', warningName='')
 class pybdsim.Builder.Quadrupole(name, l, k1, **kwargs)
 Bases: Element
 
-13.2. pybdsim.Builder module
+14.2. pybdsim.Builder module
 
-61
+65
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Builder.Query(name, **kwargs)
 Bases: GmadObject
 A query definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 class pybdsim.Builder.RBend(name, l, angle=None, B=None, **kwargs)
 Bases: _Dipole
 class pybdsim.Builder.RCol(name, l, xsize, ysize, **kwargs)
@@ -2332,19 +2464,19 @@
 class pybdsim.Builder.Sextupole(name, l, k2, **kwargs)
 Bases: Element
 class pybdsim.Builder.Shield(name, l, **kwargs)
 Bases: Element
 class pybdsim.Builder.Solenoid(name, l, ks, **kwargs)
 Bases: Element
 
-62
+66
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim.Builder.SuggestFodoK(magnetlength, driftlength)
 returns k1 (float) value for matching into next quad in a FODO cell. f = 1/(k1 * magnetlength) = driftlength
 -> solve for k1
 Note the convention in pybdsim.Builder is that the quadrupoles in the fodo cell are split in two. So this is in
 fact half the integrated k you need. This matches with the other functions in Builder.
 class pybdsim.Builder.TKicker(name, hkick, vkick, **kwargs)
@@ -2368,24 +2500,24 @@
 strengths, etc, which is left to derived classes where appropriate.
 class pybdsim.Builder.WireScanner(name, l, wireDiameter, wireLength, material, **kwargs)
 Bases: Element
 class pybdsim.Builder.XSecBias(name, **kwargs)
 Bases: GmadObject
 A xsecbias definition. Any kwargs will be written as parameter=value. parameter=(value,unit) -> parameter=value*unit
 
-13.3 pybdsim.Compare
+14.3 pybdsim.Compare
 pybdsim.Compare.MadxVsBDSIM(tfs, bdsim, survey=None, functions=None, postfunctions=None, figsize=(10,
 5), saveAll=True, outputFileName=None)
 Compares MadX and BDSIM optics variables. User must provide a tfsoptIn file or Tfsinstance and a BDSAscii file or instance.
 
-13.3. pybdsim.Compare
+14.3. pybdsim.Compare
 
-63
+67
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 Parameters
 tfs
 bdsim
 survey
 functions
 figsize
@@ -2406,38 +2538,38 @@
 pybdsim.Compare.BDSIMVsBDSIM(first, second, first_name=None, second_name=None, survey=None,
 saveAll=True, outputFileName=None, **kwargs)
 Display all the optical function plots for the two input optics files.
 pybdsim.Compare.TransportVsBDSIM(first, second, first_name=None, second_name=None, survey=None,
 saveAll=True, outputFileName=None, **kwargs)
 Display all the optical function plots for the two input optics files.
 
-13.4 pybdsim.Constants module
+14.4 pybdsim.Constants module
 pybdsim.Constants.GetPDGInd(particlename)
 pybdsim.Constants.GetPDGName(particleid)
 
-13.5 pybdsim.Convert
+14.5 pybdsim.Convert
 Module for various conversions.
 pybdsim.Convert.BdsimPrimaries2Mad8(inputfile, outfile, start=0, ninrays=-1)
 Takes .root file generated from a BDSIM run an an input and creates a MAD8 inrays file from the primary
 particle tree.
 Parameters
 • inputfile (str) – root format output from BDSIM run
 • outfile (str) – filename for the inrays file
 • start (int) – starting primary particle index
 • ninrays (int) – total number of inrays to generate
 pybdsim.Convert.BdsimPrimaries2Madx(inputfile, outfile, start=0, ninrays=-1)
 Takes .root file generated from a BDSIM run an an input and creates a MADX inrays file from the primary
 particle tree.
 Parameters
 
-64
+68
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • inputfile (str) – root format output from BDSIM run
 • outfile (str) – filename for the inrays file
 • start (int) – starting primary particle index
 • ninrays (int) – total number of inrays to generate, default is all available
 pybdsim.Convert.BdsimPrimaries2Ptc(inputfile, outfile=None, start=0, ninrays=-1)
 Takes .root file generated from a BDSIM run an an input and creates a PTC inrays file from the primary
@@ -2457,19 +2589,19 @@
 MadxTfs2Gmad convert a madx twiss output file (.tfs) into a gmad tfs file for bdsim
 Example:
 >>> a,b = pybdsim.Convert.MadxTfs2Gmad('twiss.tfs', 'mymachine')
 returns Machine, [omittedItems]
 Returns two pybdsim.Builder.Machine instances. The first desired full conversion. The second is the raw
 conversion that’s not split by aperture. Thirdly, a list of the names of the omitted items is returned.
 
-13.5. pybdsim.Convert
+14.5. pybdsim.Convert
 
-65
+69
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -2482,15 +2614,15 @@
 
 aperlocalpositions
 
 collimatordict
 
 userdict
 
-66
+70
 
 partnamedict
 
 path to the input tfs file or pymadx.Data.Tfs instance
 requested output file
 the name (exact string match) of the lattice element
 to start the machine at this can also be an integer
@@ -2536,21 +2668,21 @@
 width in metres
 A python dictionary the user can supply with any
 additional information for that particular element.
 The dictionary should have keys matching the exact
 element name inChapter
 the Tfs file
 containContents
-a dictio13.and
+a dictio14.and
 Module
 nary itself with key, value pairs of parameters and
 values to be added to that particular element.
 A python dictionary of dictionaries. The key is a
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim.Convert.MadxTfs2GmadStrength(input, outputfilename, existingmachine=None, verbose=False,
 flipmagnets=False, linear=False, allNamesUnique=False,
 ignoreZeroLengthItems=True)
 Use a MADX Tfs file containing full twiss information to generate a strength (only) BDSIM GMAD file to
 be used with an existing lattice.
 existingmachine
@@ -2574,19 +2706,19 @@
 MadxTfs2Gmad convert a madx twiss output file (.tfs) into a gmad tfs file for bdsim
 Example:
 >>> a,b = pybdsim.Convert.MadxTfs2Gmad('twiss.tfs', 'mymachine')
 returns Machine, [omittedItems]
 Returns two pybdsim.Builder.Machine instances. The first desired full conversion. The second is the raw
 conversion that’s not split by aperture. Thirdly, a list of the names of the omitted items is returned.
 
-13.5. pybdsim.Convert
+14.5. pybdsim.Convert
 
-67
+71
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 tfs
 outputfilename
 startname
 
 stopname
 
@@ -2599,15 +2731,15 @@
 
 aperlocalpositions
 
 collimatordict
 
 userdict
 
-68
+72
 
 partnamedict
 
 path to the input tfs file or pymadx.Data.Tfs instance
 requested output file
 the name (exact string match) of the lattice element
 to start the machine at this can also be an integer
@@ -2653,32 +2785,32 @@
 width in metres
 A python dictionary the user can supply with any
 additional information for that particular element.
 The dictionary should have keys matching the exact
 element name inChapter
 the Tfs file
 containContents
-a dictio13.and
+a dictio14.and
 Module
 nary itself with key, value pairs of parameters and
 values to be added to that particular element.
 A python dictionary of dictionaries. The key is a
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 pybdsim.Convert._MadxTfs2Gmad.MadxTfs2GmadBeam(tfs, startname=None, verbose=False,
 extraParamsDict={})
 Takes a pymadx.Data.Tfs instance and extracts information from first line to create a BDSIM beam definition
 in a pybdsim.Beam object. Note that if kwarg startname is used, the optics are retrieved at the start of the
 element, i.e. you do not need to get the optics of the previous element, this function does that automatically.
 Works for e+, e- and proton. Default emittance is 1e-9mrad if 1 in tfs file.
 pybdsim.Convert._MadxTfs2Gmad.ZeroMissingRequiredColumns(tfsinstance)
 Sets any missing required columns to zero. Warns user when doing so.
 
-13.6 pybdsim.Data module
+14.6 pybdsim.Data module
 Output loading
 Read bdsim output
 Classes: Data - read various output files
 class pybdsim.Data.ApertureInfo(apertureType, aper1, aper2=0, aper3=0, aper4=0, offsetX=0,
 offsetY=0)
 Bases: object
 Simple class to hold aperture parameters and extents.
@@ -2703,19 +2835,19 @@
 This is used to filter the instance of the class based on matching a parameter withing a certain tolerance.
 >>> a = pybdsim.Data.Load("myfile.txt")
 >>> a.MatchValue("S",0.3,0.0004)
 this will match the “S” variable in instance “a” to the value of 0.3 within +- 0.0004.
 You can therefore used to match any parameter.
 Return type is BDSAsciiData
 
-13.6. pybdsim.Data module
+14.6. pybdsim.Data module
 
-69
+73
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 NameFromNearestS(S)
 ToDF()
 Get this BDSAsciiData instance as a pandas.DataFrame instance.
 class pybdsim.Data.BDSBH4D(hist, extractData=True)
 Bases: object
 Wrapper for a BDSBH instance. Converts to numpy data.
@@ -2750,19 +2882,19 @@
 Utility function to extract the number of events in a file quickly without fully loading it. Uses only ROOT to
 inspect the tree. Will raise an IOError exception if no Event tree is found. No check if it’s a BDSIM format
 file or not.
 class pybdsim.Data.Header(**kwargs)
 Bases: object
 A simple Python version of a header in a (RE)BDSIM file for easy access to the data.
 
-70
+74
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Data.Histogram1DSet(name=None)
 Bases: object
 Basic histogram for a categorical axis with a dict / map as the storage.
 This is completely agnostic of the type of the value used as the axis.
 It is ultimately a python dict[key] = (value, sumWeightsSq) where ‘key’ is the ‘x’ used to file the histogram.
 The bin errors can be accessed by calling Result() to return a dictionary of key : (value, error)
@@ -2798,19 +2930,19 @@
 class pybdsim.Data.ModelData(data)
 Bases: object
 A python versio of the data held in a Model tree in BDSIM output.
 d = pybdsim.Data.Load(“output.root”) md = pybdsim.Data.ModelData(d)
 Extracts this from a bdsim output file.
 classmethod FromROOTFile(path)
 
-13.6. pybdsim.Data module
+14.6. pybdsim.Data module
 
-71
+75
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 GetApertureData(removeZeroLength=False, removeZeroApertures=True, lengthTolerance=1e-06)
 return a list of aperture instances along with coordinates: l,s,x,y,apertures l - length of element s curvilinear S coordinate at the end of the element x - horizontal extent y - vertical extent apertures =
 [ApertureInfo]
 PrepareAxisAngleRotations()
 class pybdsim.Data.OptionsData(data)
 Bases: object
@@ -2846,19 +2978,19 @@
 class pybdsim.Data.RebdsimFile(filename, convert=True, histogramsOnly=False)
 Bases: object
 Class to represent data in rebdsim output file.
 Parameters
 • filename (str) – File to load
 • convert (bool) – Whether to ROOT histograms to pybdsim ones as well
 
-72
+76
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • histogramsOnly (bool) – If true, then don’t load rebdsim libraries and only load histograms.
 Contains histograms as root objects. Conversion function converts to pybdsim.Rebdsim.THX classes holding
 numpy data.
 If optics data is present, this is loaded into self.Optics which is BDSAsciiData instance.
 If convert=True (default), root histograms are automatically converted to classes provided here with numpy
 data.
@@ -2891,21 +3023,21 @@
 including the primaries (ie +1 on the index in data.GetSamplerNames()). Examples:
 >>> f = pybdsim.Data.Load("file.root")
 >>> primaries = pybdsim.Data.SamplerData(f)
 >>> samplerfd45 = pybdsim.Data.SamplerData(f, "samplerfd45")
 >>> thirdAfterPrimaries = pybdsim.Data.SamplerData(f, 3)
 class pybdsim.Data.Spectra(nameIn=None)
 Bases: object
-append(pdgid, hist, path, nameIn=None)
+append(pdgid, hist, path, nameIn=None, flag=None)
 
-13.6. pybdsim.Data module
+14.6. pybdsim.Data module
 
-73
+77
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Data.TH1(hist, extractData=True)
 Bases: ROOTHist
 Wrapper for a ROOT TH1 instance. Converts to numpy data.
 >>> h = file.Get("histogramName")
 >>> hpy = TH1(h)
 Rebin(nBins)
@@ -2940,19 +3072,19 @@
 resultDimension (str) – ‘x’, ‘y’ or ‘z’ dimension to produce 1D histogram along.
 returns pybdsim.Data.TH1 instance.
 Slice2DXY(index)
 Extract a single 2D histogram from an index along the Z dimension.
 Parameters
 index (int) – index in z array of bins to extract, e.g. 0 -> nbinsz-1
 
-74
+78
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 Slice2DXZ(index)
 Extract a single 2D histogram from an index along the Y dimension.
 Parameters
 index (int) – index in y array of bins to extract, e.g. 0 -> nbinsy-1
 Slice2DZY(index)
 Extract a single 2D histogram from an index along the X dimension.
@@ -2971,33 +3103,33 @@
 pybdsim.Data.WriteROOTHistogramsToDirectory(tfile, directoryName, histograms)
 Parameters
 • tfile (ROOT.TFile.) – TFile object to write to.
 • directoryName (str (e.g. "Event/PerEntryHistograms" )) – Full path of directory you wish to write the histograms to.
 • histograms ([ROOT.TH1,..]) – List of ROOT histograms to write.
 Write a list of histograms (ROOT.TH*) to a directory (str) in a ROOT.TFile instance.
 
-13.7 pybdsim.Field module
+14.7 pybdsim.Field module
 Utilities to convert and prepare field maps.
 Most of the plots assume magnetic fields for the labels, but they work equally well for electric fields.
 class pybdsim.Field._Field.Field(array=array([], dtype=float64), columns=[], flip=False,
 doublePrecision=False)
 Bases: object
 Base class used for common writing procedures for BDSIM field format.
 This does not support arbitrary loop ordering - only the originally intended xyzt.
 AddComment(commentString)
 Add a string that will be put on a comment line at the beginning of the file.
 Write(fileName, writeLoopOrderReversed=False, overrideLoopOrder=None)
 Parameters
 • writeLoopOrderReversed (bool) – Write this field map with the other loop order.
 
-13.7. pybdsim.Field module
+14.7. pybdsim.Field module
 
-75
+79
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • overrideLoopOrder (str) – string to write irrespective of internal data as the loop
 order.
 gzip - if the file ends with “.gz” the file will be compressed automatically.
 For overrideLoopOrder it should be only ‘xyzt’ or ‘tzyx’. This option is provided in case a field is
 prepared in the other order somehow and you want to control the writing of this header variable independently.
 WriteFLUKA2DFormat1(fileName)
@@ -3033,19 +3165,19 @@
 [x,y,z,fx,fy,fz]. So a 100x50x30 (x,y,z) grid would have np.shape of (100,50,30,6).
 Example:
 >>> a = Field3D(data) # data is a prepared array
 >>> a.Write('outputFileName.dat')
 The ‘flip’ boolean allows an array with (z,y,x,value) dimension order to be written as (x,y,z,value). Values
 must still be (x,y,fx,fy,fz).
 
-76
+80
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 The ‘doublePrecision’ boolean controls whether the field and spatial values are written to 16 s.f. (True) or 8
 s.f. (False - default).
 class pybdsim.Field._Field.Field4D(data, flip=False, doublePrecision=False)
 Bases: Field
 Utility class to write a 4D field map array to BDSIM field format.
 The array supplied should be 5 dimensional. Dimensions are: (t,y,z,x,value) where value has 7 elements
@@ -3070,33 +3202,33 @@
 
 1
 4
 
 Parameters
 field2D (pybdsim.Field._Field.Field2D instance) – field object
 returns an instance of the same type.
-For a 2D field (i.e. function of x,y but can include Bx,By,Bz), for the quadrant #1, mirror it and generate a
-bigger field for all four quadrants.
+For a 2D field (i.e. function of x,y but can include Bx,By,Bz), for the quadrant number 1, mirror it and
+generate a bigger field for all four quadrants.
 1. original data
 2. data mirrored in x, (x,Bx) *= -1
 3. data mirrored in x,y, (x,y,By) *= -1
 4. data mirrored in y, (y,Bx) *= -1
 This is based on a dipole field.
 pybdsim.Field._Field.SortUnorderedFieldMap2D(field)
 Rearrange the data in a 2D field map to be in a linearly progressing loop of (x,y). In future this could be
 generalised to more dimensions and also any two dimensions, not just x,y.
 Parameters
 field (pybdsim.Field.Field2D) – Incoming jumbled field map
 Returns a new Field2D object
 
-13.7. pybdsim.Field module
+14.7. pybdsim.Field module
 
-77
+81
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Field.FieldPlotter.FourDData(filename, xind=0, yind=1, zind=2, tind=3)
 Class purely to simplify plotting of fields. Not for general use.
 class pybdsim.Field.FieldPlotter.OneDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 pybdsim.Field.FieldPlotter.Plot1DFxFyFz(filename)
 Plot a bdsim 1D field map file.
@@ -3134,19 +3266,19 @@
 pybdsim.Field.FieldPlotter.Plot2DXYBx(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
 • filename (str, pybdsim.Field._Field.Field2D instance) – name of field
 map file or object
 • scale (float) – numerical scaling for quiver plot arrow lengths.
-78
+82
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • title (str) – title for plot
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 pybdsim.Field.FieldPlotter.Plot2DXYBy(filename, scale=None, title=None, flipX=False,
 aspect='equal')
 Plot a bdsim field map file use the X,Y plane, but plotting By component.
 Parameters
@@ -3184,19 +3316,19 @@
 Plot Fx,Fy,Fz components of a field separately as a function of X,Y.
 Parameters
 • filename (str, pybdsim.Field._Field.Field1D instance) – name of field
 map file or object
 • title (None, str) – optional title for plot
 • aspect (str) – aspect ratio for matplotlib imshow
 
-13.7. pybdsim.Field module
+14.7. pybdsim.Field module
 
-79
+83
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 • extent (list,tuple) – list or tuple of (xmin,xmax,ymin,ymax) for each plot (optional)
 pybdsim.Field.FieldPlotter.Plot2DXYMagnitude(filename, title=None, flipX=False,
 firstDimension='X', secondDimension='Y',
 aspect='equal', zlabel='|$B_{x,y}$| (T)', figsize=(6,
 5))
 Plot a the magnitude of a 2D bdsim field map file using any two planes.
@@ -3233,26 +3365,26 @@
 • aspect (str) – Matplotlib axes aspect (e.g. ‘auto’ or ‘equal’)
 Note, matplotlibs streamplot may raise an exception if the field is entriely 0 valued.
 pybdsim.Field.FieldPlotter.Plot3DXY(filename, scale=None)
 Plots (B_x,B_y) as a function of x and y.
 pybdsim.Field.FieldPlotter.Plot3DXZ(filename, scale=None)
 Plots (B_x,B_z) as a function of x and z.
 
-80
+84
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 class pybdsim.Field.FieldPlotter.ThreeDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 class pybdsim.Field.FieldPlotter.TwoDData(filename)
 Class purely to simplify plotting of fields. Not for general use.
 
-13.8 pybdsim.Gmad module
+14.8 pybdsim.Gmad module
 Survey() - survey a gmad lattice, plot element coords
 Loader() - load a gmad file using the compiled bdsim parser
 GmadFile() - modify a text based gmad file
 
 class pybdsim.Gmad.GmadFile(fileName)
 Bases: object
 Class to determine parameters and gmad include structure
@@ -3281,19 +3413,19 @@
 Class to load a gmad options file to a buffer and modify the contents
 class pybdsim.Gmad.Lattice(filename=None)
 Bases: object
 BDSIM Gmad parser lattice.
 Use this class to load a bdsim input file using the BDSIM parser (GMAD) and then interrogate it. You can
 use this to regenerate a lattice with less information for example
 
-13.8. pybdsim.Gmad module
+14.8. pybdsim.Gmad module
 
-81
+85
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 >>> a = Lattice("filename.gmad")
 or
 >>> a = Lattice()
 >>> a.Load("filename.gmad")
 >>> a # this will tell you some basic details
 >>> print(a) # this will print out the full lattice
@@ -3323,63 +3455,63 @@
 Print elements with zero length with s location
 next()
 class pybdsim.Gmad.Survey(filename=None)
 Bases: object
 Survey - load a gmad lattice and have a look
 Example:
 
-82
+86
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 >>> a = Survey()
 >>> a.Load('mylattice.gmad')
 >>> a.Plot()
 CompareMadX(fileName)
 FinalDiff()
 FindClosestElement(coord)
 Load(filename)
 Plot()
 Step(angle, length)
 
-13.9 pybdsim.ModelProcessing module
+14.9 pybdsim.ModelProcessing module
 ModelProcessing
 Tools to process existing BDSIM models and generate other versions of them.
 pybdsim.ModelProcessing.GenerateFullListOfSamplers(inputfile, outputfile)
 inputfile - path to main gmad input file
 This will parse the input using the compiled BDSIM parser (GMAD), iterate over all the beamline elements
-and generate a sampler for every elements. Ignores samplers, but may include already defined ones in your
+and generate a sampler for every element. Ignores samplers, but may include already defined ones in your
 own input.
 pybdsim.ModelProcessing.GetAxisAlignedBoundingBoxOfCollimator(modelData, collimatorName)
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.GetMaterialIDOfCollimator(modelData, collimatorName)
 Inspect pybdsim.Data.ModelData assuming collimator info was stored to give an axis aligned bounding box
 set of ranges in global coordinates.
 pybdsim.ModelProcessing.WrapLatticeAboutItem(maingmadfile, itemname, outputfilename)
 
-13.10 pybdsim.Options module
+14.10 pybdsim.Options module
 See Options class inside this module.
 pybdsim.Options.ElectronColliderOptions()
 class pybdsim.Options.Options(*args, **kwargs)
 Bases: dict
 Inherits a dict. Converting to a string or using ReturnOptionsString() will give a suitable GMAD string to
 write out to a file.
 o = pybdsim.Options.Options() o[“trajectoryConnect”] = 1 o[“aper1”] = (5, ‘m’) str(o) ‘option, trajectoryConnect=1,
 aper1=5*m;’
 There is no checking on the option if using []. A tuple of (value, unitsString) can be used too resulting in
 value*unitsString.
 
-13.9. pybdsim.ModelProcessing module
+14.9. pybdsim.ModelProcessing module
 
-83
+87
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 ReturnOptionsString()
 SetBLMLength(length=50.0, unitsstring='cm')
 SetBLMRadius(radius=5.0, unitsstring='cm')
 SetBeamPipeRadius(beampiperadius=5.0, unitsstring='cm')
 SetBeamPipeThickness(bpt, unitsstring='mm')
 SetBeamlineS(beamlineS=0, unitsstring='m')
@@ -3407,19 +3539,19 @@
 SetLengthSafety(ls=10.0, unitsstring='um')
 SetMagnetGeometryType(magnetGeometryType='"none"')
 SetMaximumEpsilonStep(mes=1.0, unitsstring='m')
 SetMaximumStepLength(msl=20.0, unitsstring='m')
 SetMaximumTrackingTime(mtt=-1.0, unitsstring='s')
 SetMinimumEpsilonStep(mes=10.0, unitsstring='nm')
 
-84
+88
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 SetNGenerate(nparticles=10)
 SetNLinesIgnore(nlines=0)
 SetNPerFile(nperfile=100)
 SetOuterDiameter(outerdiameter=2.0, unitsstring='m')
 SetPhysicsList(physicslist='')
 SetPipeMaterial(bpm)
@@ -3447,37 +3579,45 @@
 SetTrajectoryCutLTR(ltr=10.0, unitsstring='m')
 SetTunnelFloorOffset(offset=1.0, unitsstring='m')
 SetTunnelMaterial(tm)
 SetTunnelOffsetX(offset=0.0, unitsstring='m')
 SetTunnelOffsetY(offset=0.0, unitsstring='m')
 SetTunnelRadius(tunnelradius=2.0, unitsstring='m')
 
-13.10. pybdsim.Options module
+14.10. pybdsim.Options module
 
-85
+89
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 SetTunnelThickness(tt=1.0, unitsstring='m')
 SetVacuumMaterial(vm)
 SetVacuumPressure(vp)
 Vacuum pressure in bar
 SetWritePrimaries(on=True)
 pybdsim.Options.ProtonColliderOptions()
 
-13.11 pybdsim.Plot module
+14.11 pybdsim.Plot module
 Useful plots for bdsim output
 pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(figure, surveyfile, tightLayout=True,
 sOffset=0.0, fraction=0.9)
-Add a machine diagram to the top of the plot in a current figure sOffset offsets survey along s fraction controls
-fraction of the figure for the plot, the remainder being used for the survey
+Add a machine diagram to the top of the plot in a current figure.
+Parameters
+• figure (matplotlib.figure.Figure) – the matplotlib figure to add the plot to.
+• surveyfile
+(str, pybdsim.Data.RebdsimFile, pybdsim.Data.
+BDSAsciiData, cppyy.gbl.DataLoader) – BDSIM file or REBDSIM file
+(with Model tree filled) or BDSIM survey output or path to any of these.
+• tightLayout (bool) – whether to call matplotlib’s tight layout after adding the axes.
+• sOffset (float) – add this number to the S coordinate of all elements in the machine
+diagram.
+• fraction (float) – controls fraction of the figure for the plot, the remainder being
+used for the survey.
 pybdsim.Plot.AddMachineLatticeFromSurveyToFigureMultiple(figure, machines, tightLayout=True)
 Similar to AddMachineLatticeFromSurveyToFigure() but accepts multiple machines.
-pybdsim.Plot.AddMachineLatticeToFigure(figure, tfsfile, tightLayout=True)
-A forward to the pymadx.Plot.AddMachineLatticeToFigure function.
 pybdsim.Plot.Aperture(rootFileName, filterThin=False, surveyFileName=None)
 pybdsim.Plot.BDSIMAperture(data, machineDiagram=True, plot='xy', plotApertureType=True,
 removeZeroLength=False, removeZeroApertures=True)
 Plot the aperture from a BDSIM DataLoader instance. By default it’s colour coded and excludes any 0
 aperture elements. Zero length elements are included.
 pybdsim.Plot.BDSIMApertureFromFile(filename, machineDiagram=True, plot='xy',
 plotApertureType=True, removeZeroLength=False,
@@ -3485,28 +3625,37 @@
 Plot the aperture from a BDSIM output file. By default it’s colour coded and excludes any 0s.
 pybdsim.Plot.BDSIMOptics(rebdsimOpticsOutput, outputfilename=None, saveall=True, survey=None,
 **kwargs)
 Display all the optical function plots for a rebdsim optics root file. By default, this saves all optical functions
 into a single (outputfilename) pdf, to save the optical functions separately, supply an outputfilename with
 saveall=false.
 pybdsim.Plot.DrawMachineLattice(axesinstance, bdsasciidataobject, sOffset=0.0)
+The low-level version of drawing a machine diagram. Draws into an axes instance given using loaded model
+data in the form of a pybdsim.Data.BDSAsciiData instance.
+Parameters
+
+90
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.2.0
+
+• axesinstance (matplotlib.axes.Axes) – the plotting axis to draw the machine diagram into.
+• sOffset (float) – add this value to the S of all machine elements in the diagram.
+Param
+bdsasciidataobject The model data.
+The main interface is AddMachineLatticeFromSurveyToFigure, but this function may be useful for more
+granular plotting, e.g. with custom subfigures / axes.
 pybdsim.Plot.EnergyDeposition(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
 Plot the energy deposition from a REBDSIM output file - uses premade merged histograms.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot. If both are provided, the machine diagram is plotted from the MADX survey.
 pybdsim.Plot.EnergyDepositionCoded(filename, outputfilename=None, tfssurvey=None,
 bdsimsurvey=None, warmaperinfo=None, **kwargs)
 Plot the energy deposition from a REBDSIM output file - uses premade merged histograms.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot. If both are provided, the machine diagram is plotted from the MADX survey.
-
-86
-
-Chapter 13. Module Contents
-
-pybdsim Documentation, Release 3.1.0
-
 If a BDSIM survey is provided, collimator positions and dimensions can be taken and used to split losses
 into categories: collimator, warm and cold based on warm aperture infomation provided. To enable this, the
 “warmaperinfo” option must be set according to the prescription below.
 The user can supply a list of upper and lower edges of warm regions or give the path to a coulmn-formated
 data file with this information via the “warmaperinfo” option. Set warmaperinfo=1 to treat all non-collimator
 losses as warm or set warmaperinfo=-1 to treat them as cold. Default is not perform the loss classification.
 If no warm aperture information is provided, the plotting falls back to the standard simple plotting provided
@@ -3529,14 +3678,21 @@
 xScalingFactor=1.0, figsize=(6.4, 4.8), log=False, **errorbarKwargs)
 Plot a pybdsim.Data.TH1 instance.
 Parameters
 • xlabel – x axis label
 • ylabel – y axis label
 • title – plot title
 • scalingFactor – multiplier for values
+
+14.11. pybdsim.Plot module
+
+91
+
+pybdsim Documentation, Release 3.2.0
+
 • xScalingFactor – multiplier for x axis coordinates
 • log – whether to automatically plot on a vertical log scale
 return figure instance
 pybdsim.Plot.Histogram1DMultiple(histograms, labels, log=False, xlog=False, xlabel=None,
 ylabel=None, title=None, scalingFactors=None,
 xScalingFactors=None, figsize=(10, 5), legendKwargs={},
 **errorbarKwargs)
@@ -3544,24 +3700,14 @@
 pybdsim.Data.TH1 objects and strings.
 return figure instance
 xScalingFactors may be a float, int or list
 Example:
 Histogram1DMultiple([h1,h2,h3],
 ['Photons', 'Electrons', 'Positrons'],
 xlabel=r'$\mu$m',
-(continues on next page)
-
-13.11. pybdsim.Plot module
-
-87
-
-pybdsim Documentation, Release 3.1.0
-
-(continued from previous page)
-
 ylabel='Fraction',
 scalingFactors=[1,100,100],
 xScalingFactors=1e6,
 log=True)
 pybdsim.Plot.Histogram1DRatio(histogram1, histogram2, label1='', label2='', xLogScale=False,
 yLogScale=False, xlabel=None, ylabel=None, title=None,
 scalingFactor=1.0, xScalingFactor=1.0, figsize=(6.4, 4.8), ratio=3,
@@ -3587,56 +3733,70 @@
 data vmin - explicitly control the vmin for the colour normalisation vmax - explicitly control the vmax for
 the colour normalisation
 return figure instance
 pybdsim.Plot.Histogram2DErrors(histogram, logNorm=False, xLogScale=False, yLogScale=False,
 xlabel='', ylabel='', zlabel='', title='', aspect='auto', scalingFactor=1.0,
 xScalingFactor=1.0, yScalingFactor=1.0, figsize=(6, 5), vmin=None,
 autovmin=False, vmax=None, **imshowKwargs)
+92
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.2.0
+
 Similar to Histogram2D() but plot the errors from the histogram instead of the contents. See pybdsim.Plot.Histogram2D for documentation of arguments.
 pybdsim.Plot.Histogram3D(th3)
 Plot a pybdsim.Data.TH3 instance - TBC
 pybdsim.Plot.LossAndEnergyDeposition(filename, outputfilename=None, tfssurvey=None,
 bdsimsurvey=None, hitslegendloc='upper left',
 elosslegendloc='upper right', perelement=False,
 elossylim=None, phitsylim=None)
 Load a REBDSIM output file and plot the merged histograms automatically generated by BDSIM.
 Optional either Twiss table for MADX or BDSIM Survey to add machine diagram to plot.
 pybdsim.Plot.LossMap(ax, xcentres, y, ylow=None, **kwargs)
 Plot a loss map in such a way that works well for very large loss maps. xcentres, xwidth and y are all provided
 by TH1 python histograms (see pybdsim.Data.TH1).
-
-88
-
-Chapter 13. Module Contents
-
-pybdsim Documentation, Release 3.1.0
-
 Parameters
 • ax – Matplotlib axes instance to draw to
 • xcentres – centres of bins
 • y – loss map signal data, same length as xcentres.
 • ylow – small non-zero value to fill between to ensure works with log scales.
 kwargs: * passed to calls to plot and fill_between.
 pybdsim.Plot.MadxTfsBeta(tfsfile, title='', outputfilename=None)
 A forward to the pymadx.Plot.PlotTfsBeta function.
 pybdsim.Plot.ModelBDSIMXZ(model, ax=None)
+The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey done in BDSIM.
+The results can be found in the BDSIM output file in the Model tree. The functions can plot the start and
+end positions of each element in the sequence.
 pybdsim.Plot.ModelBDSIMYZ(model, ax=None)
+The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey done in BDSIM.
+The results can be found in the BDSIM output file in the Model tree. The functions can plot the start and
+end positions of each element in the sequence.
 pybdsim.Plot.ModelElegantXZ(model, ax=None, transpose=False)
+Plot a model madx from elegant. In development.
 pybdsim.Plot.ModelElegantYZ(model, ax=None, transpose=False)
+Plot a model madx from elegant. In development.
 pybdsim.Plot.PhaseSpace(data, nbins=None, outputfilename=None, extension='.pdf')
 Make two figures for coordinates and correlations.
 Number of bins chosen depending on number of samples.
 ‘outputfilename’ should be without an extension - any extension will be stripped off.
 Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g.
 extension=’.png’.
 pybdsim.Plot.PhaseSpaceFromFile(filename, samplerIndexOrName=0, nbins=None,
 outputfilename=None, extension='.pdf')
 Load a BDSIM output file and plot the phase space of a sampler (default the primaries). Only accepts raw
 BDSIM output.
 Number of bins chosen depending on number of samples.
+
+14.11. pybdsim.Plot module
+
+93
+
+pybdsim Documentation, Release 3.2.0
+
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PhaseSpaceSeparateAxes(filename, samplerIndexOrName=0, outputfilename=None,
 extension='.pdf', nbins=None, energy='total', offsetTime=True,
 includeSecondaries=False, coordsTitle=None,
 correlationTitle=None, scalefactors={}, labels={},
 log1daxes=False, log2daxes=False, includeColorbar=True)
 Plot the coordinates and correlations of both the transverse and longitudinal phase space in separate plots
@@ -3646,21 +3806,14 @@
 Energy can be binned as either kinetic or total (default), supply either energy=’total’ or energy=’kinetic’.
 offSetTime centers the time distribution about the nominal time for the specified sampler rather than the
 absolute time. Default = True.
 Secondaries can be included in the distributions with includeSecondaries. Default = False.
 Plot titles can be supplied as strings with coordsTitle and correlationTitle.
 Parameter scale factors should be supplied in a dictionary in the format {parameter: scalefactor}, e.g scalefactors={‘x’: 1000, ‘y’:1000}. Acceptable parameters are ‘x’,’y’,’xp’,’yp’, ‘T’,’kinetic’, and ‘energy’ for total
 energy.
-
-13.11. pybdsim.Plot module
-
-89
-
-pybdsim Documentation, Release 3.1.0
-
 Axis labels for parameters should be supplied as a dictionary in the format {parameter: label}, e.g labels={‘x’: “X (mm)”, ‘energy’: “Energy (MeV)”}. Acceptable parameters are ‘x’,’y’,’xp’,’yp’, ‘T’,’kinetic’,
 and ‘energy’ for total energy.
 log1daxes & log2daxes plots the 1D and 2D phase space on logarithmic scales respectively. Defaults = False.
 includeColorbar adds a colorbar to the correlation plots. The colorbar is normalised for all plot subfigures.
 Default = True.
 pybdsim.Plot.PlotAlpha(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PlotBeta(bds, outputfilename=None, survey=None, **kwargs)
@@ -3672,38 +3825,44 @@
 pybdsim.Plot.PlotSigmaP(bds, outputfilename=None, survey=None, **kwargs)
 pybdsim.Plot.PrimaryPhaseSpace(filename, outputfilename=None, extension='.pdf')
 Load a BDSIM output file and plot primary phase space. Only accepts raw BDSIM output.
 ‘outputfilename’ should be without an extension - any extension will be stripped off. Plots are saves automatically as pdf, the file extension can be changed with the ‘extension’ kwarg, e.g. extension=’.png’.
 pybdsim.Plot.PrimarySurvival(filename, outputfilename=None, tfssurvey=None, bdsimsurvey=None)
 pybdsim.Plot.PrimaryTrajectoryAndProcess(rootData, eventNumber)
 pybdsim.Plot.ProvideWrappedS(sArray, index)
+
+94
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.2.0
+
 pybdsim.Plot.Spectra(spectra, log=False, xlog=False, xlabel=None, ylabel=None, title=None,
 scalingFactors=None, xScalingFactors=None, figsize=(10, 5), legendKwargs={},
 **errorbarKwargs)
+Plot a Spectra object loaded from data that represents a set of histograms.
+returns a list of figure objects.
 pybdsim.Plot.SubplotsWithDrawnMachineLattice(survey, nrows=2, machine_plot_gap=0.01,
 gridspec_kw=None, subplots_kw=None, **fig_kw)
 Create a figure with a single column of axes, sharing the x-axis by default, with the machine drawn from the
 provided survey on the top row axes. nrows gives the number of axes, the first is always the machine lattice.
 by default 2 are drawn, the first for the machine, and the second for any data to be plotted to afterwards.
-Parameters: survey : BSDIM survey which is used to draw the machine lattice on the top axes. machine_plot_gap : vertical space between the top of the first axes and the bottom of the machine axes. By
+Parameters
+survey (str, pybdsim.Data.BDSAsciiData) – BDSIM survey which is used to draw
+the machine lattice on the top axes.
+machine_plot_gap : vertical space between the top of the first axes and the bottom of the machine axes. By
 default this is small.
 Returns (figure, machine_axes, (axes1, axes2, . . . ))
 figure : Figure instance. machine_axes : Axes instance with the machine drawn on it. Can be used to further
 edit axes : iterable of axes, in order from the first below the machine, downwards.
 pybdsim.Plot.Trajectory3D(rootFileName, eventNumber=0, bottomLeft=None, topRight=None)
 Plot e-, e+ and photons only as r,g,b respectively for a given event from a BDSIM output file.
 bottomLeft and topRight are optional [xlow,xhigh] limits for plots.
 
-90
-
-Chapter 13. Module Contents
-
-pybdsim Documentation, Release 3.1.0
-
-13.12 pybdsim.Run module
+14.12 pybdsim.Run module
 Utilities for running BDSIM and other tools from Python.
 pybdsim.Run.Bdsim(gmadpath, outfile, ngenerate=10000, batch=True, silent=False, errorSilent=False,
 options=None, bdsimExecutable=None)
 Runs bdsim with gmadpath as inputfile and outfile as outfile. Runs in batch mode by default, with 10,000
 particles. Any extra options should be provided as a string or iterable of strings of the form “–vis_debug” or
 “–vis_mac=vis.mac”, etc.
 class pybdsim.Run.ExecOptions(*args, **kwargs)
@@ -3716,14 +3875,21 @@
 class pybdsim.Run.GmadModifier(rootgmadfilename)
 Bases: object
 CheckExtensions()
 DetermineIncludes(filename)
 ReplaceTokens(tokenDict)
 pybdsim.Run.Rebdsim(rootpath, inpath, outpath, silent=False, rebdsimExecutable=None)
 Run rebdsim with rootpath as analysisConfig file, inpath as bdsim file, and outpath as output analysis file.
+
+14.12. pybdsim.Run module
+
+95
+
+pybdsim Documentation, Release 3.2.0
+
 pybdsim.Run.RebdsimCombine(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimCombine
 pybdsim.Run.RebdsimHistoMerge(rootpath, outpath, silent=False, rebdsimHistoExecutable=None)
 Run rebdsimHistoMerge
 pybdsim.Run.RebdsimOptics(rootpath, outpath, silent=False)
 Run rebdsimOptics
 pybdsim.Run.RebdsimOrbit(rootpath, outpath, index='1', silent=False, rebdsimHistoExecutable=None)
@@ -3733,62 +3899,56 @@
 A holder for multiple runs.
 GetInfo(index=-1)
 Get info about a particular run.
 Run(inputfile='optics.gmad', output='rootevent', outfile='output', ngenerate=1,
 bdsimcommand='bdsim-devel', **kwargs)
 RunExecOptions(execoptions, debug=False)
 
-13.12. pybdsim.Run module
-
-91
-
-pybdsim Documentation, Release 3.1.0
-
-13.13 pybdsim.Visualisation module
+14.13 pybdsim.Visualisation module
 Work in progress.
 class pybdsim.Visualisation.Helper(surveyFileName)
 Bases: object
 To help locate objects in the BDSIM visualisation, requires a BDSIM survey file
 draw()
 Quick survey drawing for diagnostic reasons.
 findComponentCoords(componentName)
 Returns the XYZ coordinates of a component relative to the centre
 getWorldCentre(type='linear')
 Returns the center in world coordinates of the centre of the visualisation space
 
-13.14 pybdsim.Writer module
+14.14 pybdsim.Writer module
 Writer
 Write files for a pybdsim.Builder.Machine instance. Each section of the written output (e.g. components, sequence,
 beam etc.) can be written in the main gmad file, written in its own separate file, or called from an external, preexisting file.
 Classes: File - A class that represents each section of the written output - contains booleans and strings. Writer A class that writes the data to disk.
 class pybdsim.Writer.FileSection(willContain='')
 Bases: object
 A class that represents a section of a gmad file. The sections that this class can represent are:
 • Components
+
+96
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.2.0
+
 • Sequence
 • Samplers
 • Beam
 • Options
 • Bias
 • Material
 The class contains booleans and strings relating to the location of that sections data. The section can set to
 be:
 • Written in its own separate file (default)
 • Written in the main gmad file
 • Called from an external file
 These classes are instantiated in the writer class for each section. An optional string passed in upon class instantiation is purely for the representation of the object which will state where the data will be written/called.
 This string should be one of the section names listed above.
 Example:
-
-92
-
-Chapter 13. Module Contents
-
-pybdsim Documentation, Release 3.1.0
-
 >>> beam = FileSection('beam')
 >>> beam.CallExternalFile('../myBeam.gmad')
 >>> beam
 pybdsim.Writer.File instance
 File data will be called from the external file:
 ../myBeam.gmad
 CallExternalFile(filepath='')
@@ -3808,14 +3968,24 @@
 otherwise the main file will have no reference to these sections.
 Examples:
 Writing the Builder.Machine instance myMachine to separate files:
 >>> a = Writer()
 >>> a.WriteMachine(myMachine,'lattice.gmad')
 Lattice written to:
 lattice_components.gmad
+(continues on next page)
+
+14.14. pybdsim.Writer module
+
+97
+
+pybdsim Documentation, Release 3.2.0
+
+(continued from previous page)
+
 lattice_sequence.gmad
 lattice_beam.gmad
 lattice.gmad
 All included in main file:
 lattice.gmad
 Writing the Builder.Machine instance myMachine into a single file:
 >>> a = Writer()
@@ -3825,21 +3995,14 @@
 All included in main file:
 lattice.gmad
 WriteBeam(machine, filename='')
 Write a machines beam to disk: filename.gmad
 Machine can be either a pybdsim.Builder.Machine instance or a pybdsim.Beam.Beam instance.
 WriteBias(machine, filename='')
 Write the machines bias to disk: filename.gmad
-
-13.14. pybdsim.Writer module
-
-93
-
-pybdsim Documentation, Release 3.1.0
-
 WriteComponents(machine, filename='')
 Write the machines components to disk: filename.gmad
 WriteMachine(machine(machine), filename(string), singlefile(bool), verbose(bool))
 Write a machine to disk. By default, the machine will be written into the following individual files:
 filename_components.gmad
 filename_sequence.gmad
 filename_samplers.gmad
@@ -3876,62 +4039,62 @@
 machine
 (components,sequence,beam,options,samplers,bias,material) must be written BEFORE this function is
 called.
 WriteMaterial(machine, filename='')
 Write the machines material to disk: filename.gmad
 WriteObjects(machine, filename='')
 Write the machines objects (e.g. crystals) to disk: filename.gmad
+
+98
+
+Chapter 14. Module Contents
+
+pybdsim Documentation, Release 3.2.0
+
 WriteOptions(machine, filename='')
 Write a machines options to disk: filename.gmad
 Machine can be either a pybdsim.Builder.Machine instance or a pybdsim.Options.Options instance.
 WriteSamplers(machine, filename='')
 Write the machines samplers to disk: filename.gmad
 WriteSequence(machine, filename='')
 Write the machines sequence to disk: filename.gmad
 
-13.15 pybdsim.XSecBias module
+14.15 pybdsim.XSecBias module
 class pybdsim.XSecBias.XSecBias(name, particle, processes, xsecfactors, flags)
 Bases: object
 A class for containing all information regarding cross section definitions.
 CheckBiasedProcesses()
 SetFlags(flags)
 Set flags. flags should be a space-delimited string of integers, 1-3, in the same order as the processes,
-
-94
-
-Chapter 13. Module Contents
-
-pybdsim Documentation, Release 3.1.0
-
 SetName(name)
 Set the bias name. Cannot be any upper/lowercase variant of reserved keyword “xsecBias”.
 SetParticle(particle)
 Set the particle for bias to be associated with.
 SetProcesses(processes)
 Set the list of processes to be biased. processes hould be a space-delimited string of processes.
 SetXSecFactors(xsecs)
 Set cross section factors. xsecs should be a space-delimited string of floats, e.g. “1.0 1e13 1234.9”
 
-13.15. pybdsim.XSecBias module
+14.15. pybdsim.XSecBias module
 
-95
+99
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-96
+100
 
-Chapter 13. Module Contents
+Chapter 14. Module Contents
 
 CHAPTER
 
-FOURTEEN
+FIFTEEN
 
 DEVELOPER DOCUMENTATION
 
-14.1 Release Checklist
+15.1 Release Checklist
 The procedure is as follows because the version number is read from the git tag.
 1) Update version history
 2) Make sure you’re in a new venv or uninstall pybdsim from your current venv / pip.
 3) Locally tag the new version number on the last commit but don’t push the tag.
 4) Locally pip install pybdsim so if you were to import pybdsim you’d find this latest tag.
 5) Generate html manual and stash for later upload (cd docs; make html; tar -czf html.tar.gz
 html).
@@ -3944,985 +4107,984 @@
 You can now uninstall pybdsim through pip again and download it from testpypi:
 pip install --index-url https://test.pypi.org/simple/ pybdsim
 Then you can test by importing it and using it. Afterwards, remove it.
 1) twine upload --repository pypi dist/*
 Warning: Once a tag is pushed to pypi, it can never be deleted or replaced. Similarly for testpypi. Consider
 using v1.2.3-rc or v1.2.3-rc1, which will be recognised as a release candidate by pypi.
 
-97
+101
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-98
+102
 
-Chapter 14. Developer Documentation
+Chapter 15. Developer Documentation
 
 CHAPTER
 
-FIFTEEN
+SIXTEEN
 
 INDICES AND TABLES
 
 • genindex
 • modindex
 • search
 
-99
+103
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-100
+104
 
-Chapter 15. Indices and tables
+Chapter 16. Indices and tables
 
 PYTHON MODULE INDEX
 
 p
-pybdsim, 53
-pybdsim.Beam, 53
-pybdsim.Builder, 54
-pybdsim.Compare, 63
-pybdsim.Constants, 64
-pybdsim.Convert, 64
-pybdsim.Convert._MadxTfs2Gmad, 67
-pybdsim.Data, 69
-pybdsim.Field, 75
-pybdsim.Field._Field, 75
-pybdsim.Field.FieldPlotter, 77
-pybdsim.Gmad, 81
-pybdsim.ModelProcessing, 83
-pybdsim.Options, 83
-pybdsim.Plot, 86
-pybdsim.Run, 91
-pybdsim.Visualisation, 92
-pybdsim.Writer, 92
-pybdsim.XSecBias, 94
+pybdsim, 57
+pybdsim.Beam, 57
+pybdsim.Builder, 58
+pybdsim.Compare, 67
+pybdsim.Constants, 68
+pybdsim.Convert, 68
+pybdsim.Convert._MadxTfs2Gmad, 71
+pybdsim.Data, 73
+pybdsim.Field, 79
+pybdsim.Field._Field, 79
+pybdsim.Field.FieldPlotter, 81
+pybdsim.Gmad, 85
+pybdsim.ModelProcessing, 87
+pybdsim.Options, 87
+pybdsim.Plot, 90
+pybdsim.Run, 95
+pybdsim.Visualisation, 96
+pybdsim.Writer, 96
+pybdsim.XSecBias, 99
 
-101
+105
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-102
+106
 
 Python Module Index
 
 INDEX
 
 A
 
-59
-AddMuSpoiler()
-(pybdsim.Builder.Machine method),
-AddBeam() (pybdsim.Builder.Machine method), 58
-59
-AddBias() (pybdsim.Builder.Machine method), 58
-AddObject() (pybdsim.Builder.Machine method), 59
-AddBLM() (pybdsim.Builder.Machine method), 58
-AddComment() (pybdsim.Field._Field.Field method), AddOctupole() (pybdsim.Builder.Machine method),
-59
-75
-AddOptions()
-(pybdsim.Builder.Machine method), 59
-AddCrystal() (pybdsim.Builder.Machine method), 58
-AddPlacement()
+63
+AddObject()
+(pybdsim.Builder.Machine method), 63
+AddBeam() (pybdsim.Builder.Machine method), 62
+AddOctupole()
 (pybdsim.Builder.Machine method),
-AddCrystalCol()
-(pybdsim.Builder.Machine
-59
-method), 58
+AddBias() (pybdsim.Builder.Machine method), 62
+63
+AddBLM() (pybdsim.Builder.Machine method), 62
+AddComment() (pybdsim.Field._Field.Field method), AddOptions() (pybdsim.Builder.Machine method), 63
+AddPlacement() (pybdsim.Builder.Machine method),
+79
+63
+AddCrystal() (pybdsim.Builder.Machine method), 62
 AddQuadrupole()
 (pybdsim.Builder.Machine
-AddCT() (pybdsim.Builder.Machine method), 58
+AddCrystalCol()
+(pybdsim.Builder.Machine
 method),
-59
-AddDecapole() (pybdsim.Builder.Machine method),
-AddRBend() (pybdsim.Builder.Machine method), 59
-58
-AddDegrader() (pybdsim.Builder.Machine method), AddRCol() (pybdsim.Builder.Machine method), 59
+63
+method), 62
+AddRBend() (pybdsim.Builder.Machine method), 63
+AddCT() (pybdsim.Builder.Machine method), 62
+AddDecapole() (pybdsim.Builder.Machine method), AddRCol() (pybdsim.Builder.Machine method), 63
 AddRFCavity() (pybdsim.Builder.Machine method),
-58
-60
-AddDipole() (pybdsim.Builder.Machine method), 58
+62
+64
+AddDegrader() (pybdsim.Builder.Machine method),
 AddRmat()
-(pybdsim.Builder.Machine method), 60
-AddDrift() (pybdsim.Builder.Machine method), 58
+(pybdsim.Builder.Machine method), 64
+62
 AddSampler()
-(pybdsim.Builder.Machine method), 60
-AddDump() (pybdsim.Builder.Machine method), 58
+(pybdsim.Builder.Machine method), 64
+AddDipole() (pybdsim.Builder.Machine method), 62
 AddSBend()
 (pybdsim.Builder.Machine
-method), 60
-AddECol() (pybdsim.Builder.Machine method), 58
+method), 64
+AddDrift() (pybdsim.Builder.Machine method), 62
 AddScorerMesh()
 (pybdsim.Builder.Machine
-AddElement() (pybdsim.Builder.Machine method), 58
-method), 60
-AddFodoCell() (pybdsim.Builder.Machine method),
+AddDump() (pybdsim.Builder.Machine method), 62
+method), 64
+AddECol() (pybdsim.Builder.Machine method), 62
 AddSextupole()
 (pybdsim.Builder.Machine method),
-58
-60
-AddFodoCellMultiple() (pybdsim.Builder.Machine
-AddShield() (pybdsim.Builder.Machine method), 60
-method), 58
-AddFodoCellSplitDrift()
-(pybd- AddSolenoid() (pybdsim.Builder.Machine method),
-60
-sim.Builder.Machine method), 59
+AddElement() (pybdsim.Builder.Machine method), 62
+64
+AddFodoCell() (pybdsim.Builder.Machine method),
+AddShield() (pybdsim.Builder.Machine method), 64
+62
+AddFodoCellMultiple() (pybdsim.Builder.Machine AddSolenoid() (pybdsim.Builder.Machine method),
+64
+method), 62
 AddTarget()
-(pybdsim.Builder.Machine method), 60
-AddFodoCellSplitDriftMultiple()
+(pybdsim.Builder.Machine method), 64
+AddFodoCellSplitDrift()
 (pybdAddThinMultipole()
 (pybdsim.Builder.Machine
-sim.Builder.Machine method), 59
+sim.Builder.Machine method), 63
 method),
-60
-AddGap() (pybdsim.Builder.Machine method), 59
-AddHKicker() (pybdsim.Builder.Machine method), 59 AddThinRmat() (pybdsim.Builder.Machine method),
-60
-AddIncludePost()
-(pybdsim.Builder.Machine
+64
+AddFodoCellSplitDriftMultiple()
+(pybdAddThinRmat() (pybdsim.Builder.Machine method),
+sim.Builder.Machine method), 63
+64
+AddGap() (pybdsim.Builder.Machine method), 63
 AddTKicker()
-(pybdsim.Builder.Machine method), 60
-method), 59
+(pybdsim.Builder.Machine method), 64
+AddHKicker() (pybdsim.Builder.Machine method), 63
 AddTransform3D()
 (pybdsim.Builder.Machine
-AddIncludePre()
+AddIncludePost()
 (pybdsim.Builder.Machine
-method), 60
-method), 59
-AddUndulator() (pybdsim.Builder.Machine method),
-AddJCol() (pybdsim.Builder.Machine method), 59
-60
-AddKicker() (pybdsim.Builder.Machine method), 59
-AddVKicker() (pybdsim.Builder.Machine method), 60
-AddLaser() (pybdsim.Builder.Machine method), 59
+method),
+64
+method), 63
+AddIncludePre()
+(pybdsim.Builder.Machine AddUndulator() (pybdsim.Builder.Machine method),
+64
+method), 63
+AddVKicker() (pybdsim.Builder.Machine method), 64
+AddJCol() (pybdsim.Builder.Machine method), 63
+AddWireScanner()
 (pybdsim.Builder.Machine
+AddKicker() (pybdsim.Builder.Machine method), 63
+method), 64
+AddLaser() (pybdsim.Builder.Machine method), 63
 AddMachineLatticeFromSurveyToFigure()
-(in AddWireScanner()
-method), 60
-module pybdsim.Plot), 86
-AddMachineLatticeFromSurveyToFigureMultiple()Aperture (class in pybdsim.Builder), 54
-Aperture() (in module pybdsim.Plot), 86
-(in module pybdsim.Plot), 86
-AddMachineLatticeToFigure() (in module pybd- ApertureInfo (class in pybdsim.Data), 69
-ApertureModel (class in pybdsim.Builder), 54
-sim.Plot), 86
-Append() (pybdsim.Builder.Machine method), 60
-AddMarker() (pybdsim.Builder.Machine method), 59
-AddMaterial() (pybdsim.Builder.Machine method), append() (pybdsim.Data.Spectra method), 73
-Atom (class in pybdsim.Builder), 54
-59
+(in Aperture (class in pybdsim.Builder), 58
+Aperture() (in module pybdsim.Plot), 90
+module pybdsim.Plot), 90
+AddMachineLatticeFromSurveyToFigureMultiple()ApertureInfo (class in pybdsim.Data), 73
+ApertureModel (class in pybdsim.Builder), 58
+(in module pybdsim.Plot), 90
+Append() (pybdsim.Builder.Machine method), 64
+AddMarker() (pybdsim.Builder.Machine method), 63
+AddMaterial() (pybdsim.Builder.Machine method), append() (pybdsim.Data.Spectra method), 77
+Atom (class in pybdsim.Builder), 58
+63
 AddMultipole() (pybdsim.Builder.Machine method),
+63
+AddMuSpoiler() (pybdsim.Builder.Machine method),
 
-103
+B
+BDSAsciiData (class in pybdsim.Data), 73
 
-pybdsim Documentation, Release 3.1.0
+107
 
-B
-BDSAsciiData (class in pybdsim.Data), 69
-BDSBH4D (class in pybdsim.Data), 70
-Bdsim() (in module pybdsim.Run), 91
-BDSIMAperture() (in module pybdsim.Plot), 86
-BDSIMApertureFromFile() (in module pybdsim.Plot), 86
-BDSIMOptics() (in module pybdsim.Plot), 86
+pybdsim Documentation, Release 3.2.0
+
+BDSBH4D (class in pybdsim.Data), 74
+Bdsim() (in module pybdsim.Run), 95
+BDSIMAperture() (in module pybdsim.Plot), 90
+BDSIMApertureFromFile() (in module pybdsim.Plot), 90
+BDSIMOptics() (in module pybdsim.Plot), 90
 BdsimPrimaries2Mad8()
 (in
 module
-pybdsim.Convert), 64
+pybdsim.Convert), 68
 BdsimPrimaries2Madx()
 (in
 module
-pybdsim.Convert), 64
+pybdsim.Convert), 68
 BdsimPrimaries2Ptc()
 (in
 module
-pybdsim.Convert), 65
-BDSIMVsBDSIM() (in module pybdsim.Compare), 64
-Beam (class in pybdsim.Beam), 53
-BeamData (class in pybdsim.Data), 70
-BLM (class in pybdsim.Builder), 54
-
-Dump (class in pybdsim.Builder), 55
+pybdsim.Convert), 69
+BDSIMVsBDSIM() (in module pybdsim.Compare), 68
+Beam (class in pybdsim.Beam), 57
+BeamData (class in pybdsim.Data), 74
+BLM (class in pybdsim.Builder), 58
 
 E
 
-ECol (class in pybdsim.Builder), 55
-ElectronColliderOptions() (in module pybdsim.Options), 83
-Element (class in pybdsim.Builder), 55
-ElementBase (class in pybdsim.Builder), 56
-ElementModifier (class in pybdsim.Builder), 56
+ECol (class in pybdsim.Builder), 59
+ElectronColliderOptions() (in module pybdsim.Options), 87
+Element (class in pybdsim.Builder), 59
+ElementBase (class in pybdsim.Builder), 60
+ElementModifier (class in pybdsim.Builder), 60
 elementNames()
 (pybdsim.Gmad.GmadFileComponents method),
-81
-EnergyDeposition() (in module pybdsim.Plot), 86
-EnergyDepositionCoded() (in module pybdsim.Plot), 86
+85
+EnergyDeposition() (in module pybdsim.Plot), 91
+EnergyDepositionCoded() (in module pybdsim.Plot), 91
 ErrorsToErrorOnMean() (pybdsim.Data.BDSBH4D
-method), 70
+method), 74
 ErrorsToErrorOnMean() (pybdsim.Data.ROOTHist
-method), 72
+method), 76
 C
 ErrorsToSTD() (pybdsim.Data.BDSBH4D method),
-70
 CallExternalFile()
 (pybdsim.Writer.FileSection
-ErrorsToSTD()
-(pybdsim.Data.ROOTHist method),
-method), 93
-72
-CavityInfo (class in pybdsim.Data), 70
-EventInfoData (class in pybdsim.Data), 70
-CavityModel (class in pybdsim.Builder), 54
+74
+method), 97
+ErrorsToSTD() (pybdsim.Data.ROOTHist method),
+CavityInfo (class in pybdsim.Data), 74
+76
+CavityModel (class in pybdsim.Builder), 58
+EventInfoData (class in pybdsim.Data), 74
 change()
-(pybdsim.Gmad.GmadFileComponents EventSummaryData (class in pybdsim.Data), 70
-ExecOptions (class in pybdsim.Run), 91
-method), 81
+(pybdsim.Gmad.GmadFileComponents EventSummaryData (class in pybdsim.Data), 74
+method), 85
+ExecOptions (class in pybdsim.Run), 95
 CheckBiasedProcesses()
-(pybd- ExternalGeometry (class in pybdsim.Builder), 56
-sim.XSecBias.XSecBias method), 94
+(pybd- ExternalGeometry (class in pybdsim.Builder), 60
+sim.XSecBias.XSecBias method), 99
 CheckExtensions()
 (pybdsim.Run.GmadModifier F
-method), 91
-Field (class in pybdsim.Builder), 56
-CollimatorInfo (class in pybdsim.Data), 70
-Field (class in pybdsim.Field._Field), 75
-CompareMadX() (pybdsim.Gmad.Survey method), 83
-Field1D (class in pybdsim.Field._Field), 76
+method), 95
+Field (class in pybdsim.Builder), 60
+CollimatorInfo (class in pybdsim.Data), 74
+Field (class in pybdsim.Field._Field), 79
+CompareMadX() (pybdsim.Gmad.Survey method), 87
+Field1D (class in pybdsim.Field._Field), 80
 ConcatenateMachine()
-(pybd- Field2D (class in pybdsim.Field._Field), 76
-sim.Data.BDSAsciiData method), 69
-Field3D (class in pybdsim.Field._Field), 76
+(pybd- Field2D (class in pybdsim.Field._Field), 80
+sim.Data.BDSAsciiData method), 73
+Field3D (class in pybdsim.Field._Field), 80
 ConvertToPybdsimHistograms()
-(pybd- Field4D (class in pybdsim.Field._Field), 77
-sim.Data.RebdsimFile method), 73
-FileSection (class in pybdsim.Writer), 92
-CreateDipoleDriftRing() (in module pybd- Fill() (pybdsim.Data.Histogram1DSet method), 71
-sim.Builder), 54
-Filter() (pybdsim.Data.BDSAsciiData method), 69
-CreateDipoleFodoRing() (in module pybd- FinalDiff() (pybdsim.Gmad.Survey method), 83
-sim.Builder), 55
+(pybd- Field4D (class in pybdsim.Field._Field), 81
+sim.Data.RebdsimFile method), 77
+FileSection (class in pybdsim.Writer), 96
+CreateDipoleDriftRing() (in module pybd- Fill() (pybdsim.Data.Histogram1DSet method), 75
+sim.Builder), 58
+Filter() (pybdsim.Data.BDSAsciiData method), 73
+CreateDipoleFodoRing() (in module pybd- FinalDiff() (pybdsim.Gmad.Survey method), 87
+sim.Builder), 59
 FindClosestElement()
 (pybdsim.Gmad.Survey
 CreateDipoleRing() (in module pybdsim.Builder),
-method), 83
-55
+method), 87
+59
 findComponentCoords()
-(pybdCreateEmptyRebdsimFile() (in module pybdsim.Visualisation.Helper method), 92
-sim.Data), 70
+(pybdCreateEmptyRebdsimFile() (in module pybdsim.Visualisation.Helper method), 96
+sim.Data), 74
 findElement()
-(pybdCreateFodoLine() (in module pybdsim.Builder), 55
+(pybdCreateFodoLine() (in module pybdsim.Builder), 59
 sim.Gmad.GmadFileComponents method),
-Crystal (class in pybdsim.Builder), 55
-81
-CrystalCol (class in pybdsim.Builder), 55
-Flush() (pybdsim.Data.Histogram1DSet method), 71
-FourDData (class in pybdsim.Field.FieldPlotter), 77
-D
+Crystal (class in pybdsim.Builder), 59
+85
+CrystalCol (class in pybdsim.Builder), 59
+Flush() (pybdsim.Data.Histogram1DSet method), 75
+
+FourDData (class in pybdsim.Field.FieldPlotter), 81
 from_element() (pybdsim.Builder.Element class
-method), 56
-Decapole (class in pybdsim.Builder), 55
+Decapole (class in pybdsim.Builder), 59
+method), 60
 DefineConstituentElements()
 (pybd- FromROOTFile() (pybdsim.Data.BeamData class
-method), 70
-sim.Builder.Line method), 57
+sim.Builder.Line method), 61
+method), 74
+Degrader (class in pybdsim.Builder), 59
 FromROOTFile() (pybdsim.Data.EventInfoData class
-Degrader (class in pybdsim.Builder), 55
-method), 70
 DetermineIncludes() (pybdsim.Run.GmadModifier
+method), 74
+method), 95
 FromROOTFile() (pybdsim.Data.ModelData class
-method), 91
-method), 71
-draw() (pybdsim.Visualisation.Helper method), 92
-DrawMachineLattice() (in module pybdsim.Plot), 86 FromROOTFile() (pybdsim.Data.OptionsData class
-method), 72
-Drift (class in pybdsim.Builder), 55
+draw() (pybdsim.Visualisation.Helper method), 96
+method), 75
+DrawMachineLattice() (in module pybdsim.Plot), 90 FromROOTFile() (pybdsim.Data.OptionsData class
+Drift (class in pybdsim.Builder), 59
+method), 76
+Dump (class in pybdsim.Builder), 59
 
-104
+D
+
+108
 
 Index
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 G
-Gap (class in pybdsim.Builder), 56
-GenerateFullListOfSamplers() (in module pybdsim.ModelProcessing), 83
+Gap (class in pybdsim.Builder), 60
+GenerateFullListOfSamplers() (in module pybdsim.ModelProcessing), 87
 GenerateSamplersFromBDSIMSurvey() (in module
-pybdsim.Builder), 57
-GetAllNames() (pybdsim.Gmad.Lattice method), 82
-GetAngle() (pybdsim.Gmad.Lattice method), 82
-GetAper1() (pybdsim.Gmad.Lattice method), 82
-GetAper2() (pybdsim.Gmad.Lattice method), 82
-GetAper3() (pybdsim.Gmad.Lattice method), 82
-GetAper4() (pybdsim.Gmad.Lattice method), 82
+pybdsim.Builder), 61
+GetAllNames() (pybdsim.Gmad.Lattice method), 86
+GetAngle() (pybdsim.Gmad.Lattice method), 86
+GetAper1() (pybdsim.Gmad.Lattice method), 86
+GetAper2() (pybdsim.Gmad.Lattice method), 86
+GetAper3() (pybdsim.Gmad.Lattice method), 86
+GetAper4() (pybdsim.Gmad.Lattice method), 86
 GetApertureData()
 (pybdsim.Data.ModelData
-method), 71
-GetApertureExtent() (in module pybdsim.Data), 70
+method), 75
+GetApertureExtent() (in module pybdsim.Data), 74
 GetApertureExtents()
 (pybdsim.Gmad.Lattice
-method), 82
+method), 86
 GetApertureType()
 (pybdsim.Gmad.Lattice
-method), 82
+method), 86
 GetAxisAlignedBoundingBoxOfCollimator() (in
-module pybdsim.ModelProcessing), 83
+module pybdsim.ModelProcessing), 87
 GetColumn() (pybdsim.Data.BDSAsciiData method),
-69
-GetColumn() (pybdsim.Gmad.Lattice method), 82
-GetElement() (pybdsim.Gmad.Lattice method), 82
+73
+GetColumn() (pybdsim.Gmad.Lattice method), 86
+GetElement() (pybdsim.Gmad.Lattice method), 86
 GetExecArgs() (pybdsim.Run.ExecOptions method),
-91
+95
 GetExecFlags() (pybdsim.Run.ExecOptions method),
-91
+95
 GetIndexOfElementNamed()
-(pybdsim.Gmad.Lattice method), 82
-GetInfo() (pybdsim.Run.Study method), 91
+(pybdsim.Gmad.Lattice method), 86
+GetInfo() (pybdsim.Run.Study method), 96
 GetIntegratedAngle() (pybdsim.Builder.Machine
-method), 60
+method), 64
 GetIntegratedLength() (pybdsim.Builder.Machine
-method), 60
+method), 64
 GetItemTuple()
 (pybdsim.Data.BDSAsciiData
-method), 69
-GetKs() (pybdsim.Gmad.Lattice method), 82
-GetLength() (pybdsim.Gmad.Lattice method), 82
-GetMaterialIDOfCollimator() (in module pybdsim.ModelProcessing), 83
-GetModel() (pybdsim.Data.RebdsimFile method), 73
+method), 73
+GetKs() (pybdsim.Gmad.Lattice method), 86
+GetLength() (pybdsim.Gmad.Lattice method), 86
+GetMaterialIDOfCollimator() (in module pybdsim.ModelProcessing), 87
+GetModel() (pybdsim.Data.RebdsimFile method), 77
 GetModelForPlotting() (in module pybdsim.Data),
-70
+74
 GetModelTree()
 (pybdsim.Data.RebdsimFile
-method), 73
-GetName() (pybdsim.Gmad.Lattice method), 82
+method), 77
+GetName() (pybdsim.Gmad.Lattice method), 86
 GetNamesOfType()
 (pybdsim.Builder.Machine
-method), 60
-GetNEventsInBDSIMFile() (in module pybdsim.Data), 70
-GetOpticsFromGMAD() (in module pybdsim.Run), 91
+method), 64
+GetNEventsInBDSIMFile() (in module pybdsim.Data), 74
+GetOpticsFromGMAD() (in module pybdsim.Run), 95
 getParameter()
 (pybdsim.Gmad.GmadFileComponents method),
-81
-GetPDGInd() (in module pybdsim.Constants), 64
-GetPDGName() (in module pybdsim.Constants), 64
+85
+GetPDGInd() (in module pybdsim.Constants), 68
+GetPDGName() (in module pybdsim.Constants), 68
 Index
 
 getType()
 (pybdsim.Gmad.GmadFileComponents
-method), 81
-GetType() (pybdsim.Gmad.Lattice method), 82
+method), 85
+GetType() (pybdsim.Gmad.Lattice method), 86
 getWorldCentre()
 (pybdsim.Visualisation.Helper
-method), 92
-GmadFile (class in pybdsim.Gmad), 81
-GmadFileBeam (class in pybdsim.Gmad), 81
-GmadFileComponents (class in pybdsim.Gmad), 81
-GmadFileOptions (class in pybdsim.Gmad), 81
-GmadModifier (class in pybdsim.Run), 91
-GmadObject (class in pybdsim.Builder), 57
+method), 96
+GmadFile (class in pybdsim.Gmad), 85
+GmadFileBeam (class in pybdsim.Gmad), 85
+GmadFileComponents (class in pybdsim.Gmad), 85
+GmadFileOptions (class in pybdsim.Gmad), 85
+GmadModifier (class in pybdsim.Run), 95
+GmadObject (class in pybdsim.Builder), 61
 
 H
-Header (class in pybdsim.Data), 70
-Helper (class in pybdsim.Visualisation), 92
-Histogram1D() (in module pybdsim.Plot), 87
+Header (class in pybdsim.Data), 74
+Helper (class in pybdsim.Visualisation), 96
+Histogram1D() (in module pybdsim.Plot), 91
 Histogram1DMultiple() (in module pybdsim.Plot),
-87
-Histogram1DRatio() (in module pybdsim.Plot), 88
-Histogram1DSet (class in pybdsim.Data), 70
-Histogram2D() (in module pybdsim.Plot), 88
-Histogram2DErrors() (in module pybdsim.Plot), 88
-Histogram3D() (in module pybdsim.Plot), 88
-HKicker (class in pybdsim.Builder), 57
+92
+Histogram1DRatio() (in module pybdsim.Plot), 92
+Histogram1DSet (class in pybdsim.Data), 74
+Histogram2D() (in module pybdsim.Plot), 92
+Histogram2DErrors() (in module pybdsim.Plot), 92
+Histogram3D() (in module pybdsim.Plot), 93
+HKicker (class in pybdsim.Builder), 61
 
 I
 IndexFromNearestS() (pybdsim.Data.BDSAsciiData
-method), 69
+method), 73
 IndexFromNearestS()
 (pybdsim.Gmad.Lattice
-method), 82
+method), 86
 InsertAndReplace()
 (pybdsim.Builder.Machine
-method), 60
+method), 64
 IntegateAlong1Dimension() (pybdsim.Data.TH3
-method), 74
+method), 78
 IntegateAlong2Dimensions() (pybdsim.Data.TH3
-method), 74
-IntegrateAlongX() (pybdsim.Data.TH2 method), 74
-IntegrateAlongY() (pybdsim.Data.TH2 method), 74
+method), 78
+IntegrateAlongX() (pybdsim.Data.TH2 method), 78
+IntegrateAlongY() (pybdsim.Data.TH2 method), 78
 
 J
-JCol (class in pybdsim.Builder), 57
+JCol (class in pybdsim.Builder), 61
 
 K
 keysextra() (pybdsim.Builder.ElementBase method),
-56
+60
 keysextra() (pybdsim.Builder.GmadObject method),
-57
-Kicker (class in pybdsim.Builder), 57
+61
+Kicker (class in pybdsim.Builder), 61
 
 L
-Laser (class in pybdsim.Builder), 57
-Lattice (class in pybdsim.Gmad), 81
-Line (class in pybdsim.Builder), 57
+Laser (class in pybdsim.Builder), 61
+Lattice (class in pybdsim.Gmad), 85
+Line (class in pybdsim.Builder), 61
 ListOfDirectories() (pybdsim.Data.RebdsimFile
-method), 73
+method), 77
 ListOfLeavesInTree() (pybdsim.Data.RebdsimFile
-method), 73
-105
+method), 77
+109
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 ListOfTrees() (pybdsim.Data.RebdsimFile method),
-73
-Load() (in module pybdsim.Data), 71
-Load() (in module pybdsim.Field._Field), 77
-Load() (pybdsim.Gmad.Lattice method), 82
-Load() (pybdsim.Gmad.Survey method), 83
-LoadPickledObject() (in module pybdsim.Data), 71
-LoadROOTLibraries() (in module pybdsim.Data), 71
-LoadSDDSColumnsToDict() (in module pybdsim.Data), 71
-LossAndEnergyDeposition() (in module pybdsim.Plot), 88
-LossMap() (in module pybdsim.Plot), 88
+77
+Load() (in module pybdsim.Data), 75
+Load() (in module pybdsim.Field._Field), 81
+Load() (pybdsim.Gmad.Lattice method), 86
+Load() (pybdsim.Gmad.Survey method), 87
+LoadPickledObject() (in module pybdsim.Data), 75
+LoadROOTLibraries() (in module pybdsim.Data), 75
+LoadSDDSColumnsToDict() (in module pybdsim.Data), 75
+LossAndEnergyDeposition() (in module pybdsim.Plot), 93
+LossMap() (in module pybdsim.Plot), 93
 
 M
-Machine (class in pybdsim.Builder), 57
-MadxTfs2Gmad() (in module pybdsim.Convert), 65
+Machine (class in pybdsim.Builder), 61
+MadxTfs2Gmad() (in module pybdsim.Convert), 69
 MadxTfs2Gmad()
 (in
 module
-pybdsim.Convert._MadxTfs2Gmad), 67
+pybdsim.Convert._MadxTfs2Gmad), 71
 MadxTfs2GmadBeam()
 (in
 module
-pybdsim.Convert._MadxTfs2Gmad), 69
-MadxTfs2GmadStrength() (in module pybdsim.Convert), 67
-MadxTfsBeta() (in module pybdsim.Plot), 89
-MadxVsBDSIM() (in module pybdsim.Compare), 63
+pybdsim.Convert._MadxTfs2Gmad), 73
+MadxTfs2GmadStrength() (in module pybdsim.Convert), 71
+MadxTfsBeta() (in module pybdsim.Plot), 93
+MadxVsBDSIM() (in module pybdsim.Compare), 67
 MadxVsBDSIMOrbit() (in module pybdsim.Compare),
-64
-Marker (class in pybdsim.Builder), 61
+68
+Marker (class in pybdsim.Builder), 65
 MatchValue()
 (pybdsim.Data.BDSAsciiData
-method), 69
-Material (class in pybdsim.Builder), 61
-MirrorDipoleQuadrant1() (in module pybdsim.Field._Field), 77
-ModelBDSIMXZ() (in module pybdsim.Plot), 89
-ModelBDSIMYZ() (in module pybdsim.Plot), 89
-ModelData (class in pybdsim.Data), 71
-ModelElegantXZ() (in module pybdsim.Plot), 89
-ModelElegantYZ() (in module pybdsim.Plot), 89
+method), 73
+Material (class in pybdsim.Builder), 65
+MirrorDipoleQuadrant1() (in module pybdsim.Field._Field), 81
+ModelBDSIMXZ() (in module pybdsim.Plot), 93
+ModelBDSIMYZ() (in module pybdsim.Plot), 93
+ModelData (class in pybdsim.Data), 75
+ModelElegantXZ() (in module pybdsim.Plot), 93
+ModelElegantYZ() (in module pybdsim.Plot), 93
 module
-pybdsim, 53
-pybdsim.Beam, 53
-pybdsim.Builder, 54
-pybdsim.Compare, 63
-pybdsim.Constants, 64
-pybdsim.Convert, 64
-pybdsim.Convert._MadxTfs2Gmad, 67
-pybdsim.Data, 69
-pybdsim.Field, 75
-pybdsim.Field._Field, 75
-pybdsim.Field.FieldPlotter, 77
-pybdsim.Gmad, 81
-pybdsim.ModelProcessing, 83
-pybdsim.Options, 83
-pybdsim.Plot, 86
-pybdsim.Run, 91
-pybdsim.Visualisation, 92
-pybdsim.Writer, 92
-pybdsim.XSecBias, 94
-106
+pybdsim, 57
+pybdsim.Beam, 57
+pybdsim.Builder, 58
+pybdsim.Compare, 67
+pybdsim.Constants, 68
+pybdsim.Convert, 68
+pybdsim.Convert._MadxTfs2Gmad, 71
+pybdsim.Data, 73
+pybdsim.Field, 79
+pybdsim.Field._Field, 79
+pybdsim.Field.FieldPlotter, 81
+pybdsim.Gmad, 85
+pybdsim.ModelProcessing, 87
+pybdsim.Options, 87
+pybdsim.Plot, 90
+pybdsim.Run, 95
+pybdsim.Visualisation, 96
+pybdsim.Writer, 96
+pybdsim.XSecBias, 99
+110
 
-Multipole (class in pybdsim.Builder), 61
-MuSpoiler (class in pybdsim.Builder), 61
+Multipole (class in pybdsim.Builder), 65
+MuSpoiler (class in pybdsim.Builder), 65
 
 N
 NameFromNearestS() (pybdsim.Data.BDSAsciiData
-method), 69
-NewColour (class in pybdsim.Builder), 61
-next() (pybdsim.Builder.Machine method), 61
-next() (pybdsim.Data.TrajectoryData method), 75
-next() (pybdsim.Gmad.Lattice method), 82
+method), 73
+NewColour (class in pybdsim.Builder), 65
+next() (pybdsim.Builder.Machine method), 65
+next() (pybdsim.Data.TrajectoryData method), 79
+next() (pybdsim.Gmad.Lattice method), 86
 
 O
-Octupole (class in pybdsim.Builder), 61
-OneDData (class in pybdsim.Field.FieldPlotter), 78
-Options (class in pybdsim.Options), 83
-OptionsData (class in pybdsim.Data), 72
+Octupole (class in pybdsim.Builder), 65
+OneDData (class in pybdsim.Field.FieldPlotter), 82
+Options (class in pybdsim.Options), 87
+OptionsData (class in pybdsim.Data), 76
 
 P
-PadHistogram1D() (in module pybdsim.Data), 72
+PadHistogram1D() (in module pybdsim.Data), 76
 parseElement()
 (pybdsim.Gmad.GmadFileComponents method),
-81
-ParseLattice() (pybdsim.Gmad.Lattice method), 82
-ParseSpectraName() (in module pybdsim.Data), 72
-PhaseSpace() (in module pybdsim.Plot), 89
-PhaseSpaceData (class in pybdsim.Data), 72
-PhaseSpaceFromFile() (in module pybdsim.Plot), 89
-PhaseSpaceSeparateAxes() (in module pybdsim.Plot), 89
-PickleObject() (in module pybdsim.Data), 72
-Placement (class in pybdsim.Builder), 61
-Plot() (pybdsim.Gmad.Survey method), 83
+85
+ParseLattice() (pybdsim.Gmad.Lattice method), 86
+ParseSpectraName() (in module pybdsim.Data), 76
+PhaseSpace() (in module pybdsim.Plot), 93
+PhaseSpaceData (class in pybdsim.Data), 76
+PhaseSpaceFromFile() (in module pybdsim.Plot), 93
+PhaseSpaceSeparateAxes() (in module pybdsim.Plot), 94
+PickleObject() (in module pybdsim.Data), 76
+Placement (class in pybdsim.Builder), 65
+Plot() (pybdsim.Gmad.Survey method), 87
 Plot1DFxFyFz()
 (in
 module
-pybdsim.Field.FieldPlotter), 78
-Plot2D() (in module pybdsim.Field.FieldPlotter), 78
+pybdsim.Field.FieldPlotter), 82
+Plot2D() (in module pybdsim.Field.FieldPlotter), 82
 Plot2DXY() (in module pybdsim.Field.FieldPlotter),
-78
+82
 Plot2DXYBx()
 (in
 module
-pybdsim.Field.FieldPlotter), 78
+pybdsim.Field.FieldPlotter), 82
 Plot2DXYBy()
 (in
 module
-pybdsim.Field.FieldPlotter), 79
+pybdsim.Field.FieldPlotter), 83
 Plot2DXYBz()
 (in
 module
-pybdsim.Field.FieldPlotter), 79
+pybdsim.Field.FieldPlotter), 83
 Plot2DXYComponent()
 (in
 module
-pybdsim.Field.FieldPlotter), 79
-Plot2DXYConnectionOrder() (in module pybdsim.Field.FieldPlotter), 79
+pybdsim.Field.FieldPlotter), 83
+Plot2DXYConnectionOrder() (in module pybdsim.Field.FieldPlotter), 83
 Plot2DXYFxFyFz()
 (in
 module
-pybdsim.Field.FieldPlotter), 79
+pybdsim.Field.FieldPlotter), 83
 Plot2DXYMagnitude()
 (in
 module
-pybdsim.Field.FieldPlotter), 80
+pybdsim.Field.FieldPlotter), 84
 Plot2DXYStream()
 (in
 module
-pybdsim.Field.FieldPlotter), 80
+pybdsim.Field.FieldPlotter), 84
 Plot2DXZStream()
 (in
 module
-pybdsim.Field.FieldPlotter), 80
+pybdsim.Field.FieldPlotter), 84
 Plot3DXY() (in module pybdsim.Field.FieldPlotter),
-80
+84
 
 Index
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 Plot3DXZ() (in module pybdsim.Field.FieldPlotter),
-80
-PlotAlpha() (in module pybdsim.Plot), 90
-PlotBeta() (in module pybdsim.Plot), 90
-PlotDisp() (in module pybdsim.Plot), 90
-PlotDispP() (in module pybdsim.Plot), 90
-PlotMean() (in module pybdsim.Plot), 90
-PlotNPart() (in module pybdsim.Plot), 90
-PlotSigma() (in module pybdsim.Plot), 90
-PlotSigmaP() (in module pybdsim.Plot), 90
-PrepareApertureModel() (in module pybdsim.Builder), 61
+84
+PlotAlpha() (in module pybdsim.Plot), 94
+PlotBeta() (in module pybdsim.Plot), 94
+PlotDisp() (in module pybdsim.Plot), 94
+PlotDispP() (in module pybdsim.Plot), 94
+PlotMean() (in module pybdsim.Plot), 94
+PlotNPart() (in module pybdsim.Plot), 94
+PlotSigma() (in module pybdsim.Plot), 94
+PlotSigmaP() (in module pybdsim.Plot), 94
+PrepareApertureModel() (in module pybdsim.Builder), 65
 PrepareAxisAngleRotations()
-(pybdsim.Data.ModelData method), 72
-PrimaryPhaseSpace() (in module pybdsim.Plot), 90
-PrimarySurvival() (in module pybdsim.Plot), 90
-PrimaryTrajectoryAndProcess() (in module pybdsim.Plot), 90
-Print() (pybdsim.Gmad.Lattice method), 82
+(pybdsim.Data.ModelData method), 76
+PrimaryPhaseSpace() (in module pybdsim.Plot), 94
+PrimarySurvival() (in module pybdsim.Plot), 94
+PrimaryTrajectoryAndProcess() (in module pybdsim.Plot), 94
+Print() (pybdsim.Gmad.Lattice method), 86
 PrintZeroLength()
 (pybdsim.Gmad.Lattice
-method), 82
-ProtonColliderOptions() (in module pybdsim.Options), 86
-ProvideWrappedS() (in module pybdsim.Plot), 90
+method), 86
+ProtonColliderOptions() (in module pybdsim.Options), 90
+ProvideWrappedS() (in module pybdsim.Plot), 94
 pybdsim
-module, 53
+module, 57
 pybdsim.Beam
-module, 53
+module, 57
 pybdsim.Builder
-module, 54
+module, 58
 pybdsim.Compare
-module, 63
+module, 67
 pybdsim.Constants
-module, 64
+module, 68
 pybdsim.Convert
-module, 64
+module, 68
 pybdsim.Convert._MadxTfs2Gmad
-module, 67
+module, 71
 pybdsim.Data
-module, 69
+module, 73
 pybdsim.Field
-module, 75
+module, 79
 pybdsim.Field._Field
-module, 75
+module, 79
 pybdsim.Field.FieldPlotter
-module, 77
-pybdsim.Gmad
 module, 81
+pybdsim.Gmad
+module, 85
 pybdsim.ModelProcessing
-module, 83
+module, 87
 pybdsim.Options
-module, 83
+module, 87
 pybdsim.Plot
-module, 86
+module, 90
 pybdsim.Run
-module, 91
+module, 95
 pybdsim.Visualisation
-module, 92
+module, 96
 
 Index
 
 pybdsim.Writer
-module, 92
+module, 96
 pybdsim.XSecBias
-module, 94
+module, 99
 
 Q
-Quadrupole (class in pybdsim.Builder), 61
-Query (class in pybdsim.Builder), 61
+Quadrupole (class in pybdsim.Builder), 65
+Query (class in pybdsim.Builder), 65
 
 R
-RBend (class in pybdsim.Builder), 62
-RCol (class in pybdsim.Builder), 62
-Rebdsim() (in module pybdsim.Run), 91
-RebdsimCombine() (in module pybdsim.Run), 91
-RebdsimFile (class in pybdsim.Data), 72
-RebdsimHistoMerge() (in module pybdsim.Run), 91
-RebdsimOptics() (in module pybdsim.Run), 91
-RebdsimOrbit() (in module pybdsim.Run), 91
-Rebin() (pybdsim.Data.TH1 method), 74
-Rebin() (pybdsim.Data.TH2 method), 74
+RBend (class in pybdsim.Builder), 66
+RCol (class in pybdsim.Builder), 66
+Rebdsim() (in module pybdsim.Run), 95
+RebdsimCombine() (in module pybdsim.Run), 95
+RebdsimFile (class in pybdsim.Data), 76
+RebdsimHistoMerge() (in module pybdsim.Run), 96
+RebdsimOptics() (in module pybdsim.Run), 96
+RebdsimOrbit() (in module pybdsim.Run), 96
+Rebin() (pybdsim.Data.TH1 method), 78
+Rebin() (pybdsim.Data.TH2 method), 78
 RegenerateLenInt()
 (pybdsim.Builder.Machine
-method), 60
-Region (class in pybdsim.Builder), 62
+method), 64
+Region (class in pybdsim.Builder), 66
 ReplaceElementCategory()
-(pybdsim.Builder.Machine method), 60
+(pybdsim.Builder.Machine method), 64
 ReplaceTokens()
 (pybdsim.Run.GmadModifier
-method), 91
+method), 95
 ReplaceWithElement() (pybdsim.Builder.Machine
-method), 60
-ReplaceZeroWithMinimum() (in module pybdsim.Data), 73
-Result() (pybdsim.Data.Histogram1DSet method), 71
+method), 64
+ReplaceZeroWithMinimum() (in module pybdsim.Data), 77
+Result() (pybdsim.Data.Histogram1DSet method), 75
 ResultMean()
 (pybdsim.Data.Histogram1DSet
-method), 71
+method), 75
 ReturnBeamString() (pybdsim.Beam.Beam method),
-53
+57
 ReturnOptionsString() (pybdsim.Options.Options
-method), 83
-RFCavity (class in pybdsim.Builder), 62
-Rmat (class in pybdsim.Builder), 62
-ROOTHist (class in pybdsim.Data), 72
-Run() (pybdsim.Run.Study method), 91
-RunExecOptions() (pybdsim.Run.Study method), 91
+method), 87
+RFCavity (class in pybdsim.Builder), 66
+Rmat (class in pybdsim.Builder), 66
+ROOTHist (class in pybdsim.Data), 76
+Run() (pybdsim.Run.Study method), 96
+RunExecOptions() (pybdsim.Run.Study method), 96
 
 S
-Sampler (class in pybdsim.Builder), 62
-SamplerData (class in pybdsim.Data), 73
-SamplerPlacement (class in pybdsim.Builder), 62
-SBend (class in pybdsim.Builder), 62
-Scorer (class in pybdsim.Builder), 62
-ScorerMesh (class in pybdsim.Builder), 62
-SDDSBuildParameterDicts() (in module pybdsim.Data), 73
+Sampler (class in pybdsim.Builder), 66
+SamplerData (class in pybdsim.Data), 77
+SamplerPlacement (class in pybdsim.Builder), 66
+SBend (class in pybdsim.Builder), 66
+Scorer (class in pybdsim.Builder), 66
+ScorerMesh (class in pybdsim.Builder), 66
+SDDSBuildParameterDicts() (in module pybdsim.Data), 77
 SetBeamlineS() (pybdsim.Options.Options method),
-84
+88
 SetBeamPipeRadius()
 (pybdsim.Options.Options
-method), 84
+method), 88
 
-107
+111
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 SetBeamPipeThickness()
-(pybdsim.Options.Options method), 84
-sim.Options.Options method), 84
+(pybdsim.Options.Options method), 88
+sim.Options.Options method), 88
 SetMaximumStepLength()
 (pybdSetBLMLength() (pybdsim.Options.Options method),
-sim.Options.Options method), 84
-84
+sim.Options.Options method), 88
+88
 SetMaximumTrackingTime()
 (pybdSetBLMRadius() (pybdsim.Options.Options method),
-sim.Options.Options method), 84
-84
+sim.Options.Options method), 88
+88
 SetMinimumEpsilonStep()
 (pybdSetBuildTunnel()
 (pybdsim.Options.Options
-sim.Options.Options method), 84
-method), 84
-SetName() (pybdsim.XSecBias.XSecBias method), 94
+sim.Options.Options method), 88
+method), 88
+SetName() (pybdsim.XSecBias.XSecBias method), 99
 SetBuildTunnelFloor() (pybdsim.Options.Options SetNGenerate() (pybdsim.Options.Options method),
-method), 84
-84
+method), 88
+88
 SetCherenkovOn()
 (pybdsim.Options.Options SetNLinesIgnore()
 (pybdsim.Options.Options
-method), 84
-method), 85
+method), 88
+method), 89
 SetChordStepMinimum() (pybdsim.Options.Options SetNPerFile() (pybdsim.Options.Options method),
-method), 84
-85
+method), 88
+89
 SetDefaultBiasMaterial()
 (pybd- SetOuterDiameter()
 (pybdsim.Options.Options
-sim.Options.Options method), 84
-method), 85
+sim.Options.Options method), 88
+method), 89
 SetDefaultBiasVaccum()
 (pybd- SetParticle()
 (pybdsim.XSecBias.XSecBias
-sim.Options.Options method), 84
-method), 95
+sim.Options.Options method), 88
+method), 99
 SetDefaultRangeCut() (pybdsim.Options.Options SetParticleType() (pybdsim.Beam.Beam method),
-method), 84
-53
+method), 88
+57
 SetDeltaChord()
 (pybdsim.Options.Options SetPhysicsList()
 (pybdsim.Options.Options
-method), 84
-method), 85
+method), 88
+method), 89
 SetDeltaIntersection()
 (pybd- SetPipeMaterial()
 (pybdsim.Options.Options
-sim.Options.Options method), 84
-method), 85
+sim.Options.Options method), 88
+method), 89
 SetDeltaOneStep()
 (pybdsim.Options.Options SetPrintModuloFraction()
-(pybdmethod), 84
-sim.Options.Options method), 85
+(pybdmethod), 88
+sim.Options.Options method), 89
 SetDistributionType()
 (pybdsim.Beam.Beam SetProcesses()
 (pybdsim.XSecBias.XSecBias
-method), 53
-method), 95
+method), 57
+method), 99
 SetDontSplitSBends() (pybdsim.Options.Options SetProductionCutElectrons()
-(pybdmethod), 84
-sim.Options.Options method), 85
-SetE0() (pybdsim.Beam.Beam method), 53
+(pybdmethod), 88
+sim.Options.Options method), 89
+SetE0() (pybdsim.Beam.Beam method), 57
 SetProductionCutPhotons()
 (pybdSetELossHistBinWidth()
-(pybdsim.Options.Options method), 85
-sim.Options.Options method), 84
+(pybdsim.Options.Options method), 89
+sim.Options.Options method), 88
 SetProductionCutPositrons()
 (pybdSetEMLeadParticleBiasing()
-(pybdsim.Options.Options method), 85
-sim.Options.Options method), 84
+(pybdsim.Options.Options method), 89
+sim.Options.Options method), 88
 SetRandomSeed()
 (pybdsim.Options.Options
-SetEnergy() (pybdsim.Beam.Beam method), 53
-method), 85
-SetEPAnnihilation2HadronEnhancementFactor() SetS0() (pybdsim.Beam.Beam method), 54
-(pybdsim.Options.Options method), 84
+SetEnergy() (pybdsim.Beam.Beam method), 57
+method), 89
+SetEPAnnihilation2HadronEnhancementFactor() SetS0() (pybdsim.Beam.Beam method), 58
+(pybdsim.Options.Options method), 88
 SetSamplerDiameter() (pybdsim.Options.Options
 SetEPAnnihilation2MuonEnhancementFactor()
-method), 85
-(pybdsim.Options.Options method), 84
+method), 89
+(pybdsim.Options.Options method), 88
 SetSensitiveBeamlineComponents()
-(pybdSetFlags() (pybdsim.XSecBias.XSecBias method), 94
-sim.Options.Options method), 85
+(pybdSetFlags() (pybdsim.XSecBias.XSecBias method), 99
+sim.Options.Options method), 89
 SetGamma2MuonEnahncementFactor()
 (pybd- SetSensitiveBeamPipe()
-(pybdsim.Options.Options method), 84
-sim.Options.Options method), 85
+(pybdsim.Options.Options method), 88
+sim.Options.Options method), 89
 SetGeneralOption()
 (pybdsim.Options.Options SetSenssitiveBLMs()
 (pybdsim.Options.Options
-method), 84
-method), 85
+method), 88
+method), 89
 SetIncludeFringeFields()
 (pybd- SetSoilMaterial()
 (pybdsim.Options.Options
-sim.Options.Options method), 84
-method), 85
+sim.Options.Options method), 88
+method), 89
 SetIncludeIronMagField()
 (pybd- SetSoilThickness()
 (pybdsim.Options.Options
-sim.Options.Options method), 84
-method), 85
+sim.Options.Options method), 88
+method), 89
 SetIntegratorSet()
-(pybdsim.Options.Options SetSRLowX() (pybdsim.Options.Options method), 85
-method), 84
+(pybdsim.Options.Options SetSRLowX() (pybdsim.Options.Options method), 89
+method), 88
 SetSRMultiplicity()
 (pybdsim.Options.Options
 SetLengthSafety()
 (pybdsim.Options.Options
-method), 85
-method), 84
+method), 89
+method), 88
 SetStopSecondaries() (pybdsim.Options.Options
 SetLPBFraction()
 (pybdsim.Options.Options
-method), 85
-method), 84
+method), 89
+method), 88
 SetStoreTrajectory() (pybdsim.Options.Options
 SetMagnetGeometryType()
-(pybdmethod), 85
-sim.Options.Options method), 84
+(pybdmethod), 89
+sim.Options.Options method), 88
 SetStoreTrajectoryParticle()
 (pybdSetMaximumEpsilonStep()
-(pybdsim.Options.Options method), 85
+(pybdsim.Options.Options method), 89
 
-108
+112
 
 Index
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
 SetSynchRadiationOn() (pybdsim.Options.Options
-method), 85
-SetT0() (pybdsim.Beam.Beam method), 54
+method), 89
+SetT0() (pybdsim.Beam.Beam method), 58
 SetThresholdCutCharged()
-(pybdsim.Options.Options method), 85
+(pybdsim.Options.Options method), 89
 SetThresholdCutPhotons()
-(pybdsim.Options.Options method), 85
+(pybdsim.Options.Options method), 89
 SetTrackSRPhotons()
 (pybdsim.Options.Options
-method), 85
+method), 89
 SetTrajectoryCutGTZ() (pybdsim.Options.Options
-method), 85
+method), 89
 SetTrajectoryCutLTR() (pybdsim.Options.Options
-method), 85
+method), 89
 SetTunnelFloorOffset()
-(pybdsim.Options.Options method), 85
+(pybdsim.Options.Options method), 89
 SetTunnelMaterial()
 (pybdsim.Options.Options
-method), 85
+method), 89
 SetTunnelOffsetX()
 (pybdsim.Options.Options
-method), 85
+method), 89
 SetTunnelOffsetY()
 (pybdsim.Options.Options
-method), 85
+method), 89
 SetTunnelRadius()
 (pybdsim.Options.Options
-method), 85
+method), 89
 SetTunnelThickness() (pybdsim.Options.Options
-method), 85
+method), 89
 SetVacuumMaterial()
 (pybdsim.Options.Options
-method), 86
+method), 90
 SetVacuumPressure()
 (pybdsim.Options.Options
-method), 86
+method), 90
 SetWritePrimaries()
 (pybdsim.Options.Options
-method), 86
-SetX0() (pybdsim.Beam.Beam method), 54
-SetXP0() (pybdsim.Beam.Beam method), 54
+method), 90
+SetX0() (pybdsim.Beam.Beam method), 58
+SetXP0() (pybdsim.Beam.Beam method), 58
 SetXSecFactors()
 (pybdsim.XSecBias.XSecBias
-method), 95
-SetY0() (pybdsim.Beam.Beam method), 54
-SetYP0() (pybdsim.Beam.Beam method), 54
-SetZ0() (pybdsim.Beam.Beam method), 54
-SetZP0() (pybdsim.Beam.Beam method), 54
-Sextupole (class in pybdsim.Builder), 62
-Shield (class in pybdsim.Builder), 62
-Slice2DXY() (pybdsim.Data.TH3 method), 74
-Slice2DXZ() (pybdsim.Data.TH3 method), 74
-Slice2DZY() (pybdsim.Data.TH3 method), 75
-Solenoid (class in pybdsim.Builder), 62
+method), 99
+SetY0() (pybdsim.Beam.Beam method), 58
+SetYP0() (pybdsim.Beam.Beam method), 58
+SetZ0() (pybdsim.Beam.Beam method), 58
+SetZP0() (pybdsim.Beam.Beam method), 58
+Sextupole (class in pybdsim.Builder), 66
+Shield (class in pybdsim.Builder), 66
+Slice2DXY() (pybdsim.Data.TH3 method), 78
+Slice2DXZ() (pybdsim.Data.TH3 method), 78
+Slice2DZY() (pybdsim.Data.TH3 method), 79
+Solenoid (class in pybdsim.Builder), 66
 SortByBin()
 (pybdsim.Data.Histogram1DSet
-method), 71
-SortUnorderedFieldMap2D() (in module pybdsim.Field._Field), 77
-Spectra (class in pybdsim.Data), 73
-Spectra() (in module pybdsim.Plot), 90
-split() (pybdsim.Builder.Element method), 56
-split() (pybdsim.Builder.HKicker method), 57
-split() (pybdsim.Builder.Kicker method), 57
-split() (pybdsim.Builder.Multipole method), 61
-split() (pybdsim.Builder.TKicker method), 63
-split() (pybdsim.Builder.VKicker method), 63
-Step() (pybdsim.Gmad.Survey method), 83
+method), 75
+SortUnorderedFieldMap2D() (in module pybdsim.Field._Field), 81
+Spectra (class in pybdsim.Data), 77
+Spectra() (in module pybdsim.Plot), 94
+split() (pybdsim.Builder.Element method), 60
+split() (pybdsim.Builder.HKicker method), 61
+split() (pybdsim.Builder.Kicker method), 61
+split() (pybdsim.Builder.Multipole method), 65
+split() (pybdsim.Builder.TKicker method), 67
+split() (pybdsim.Builder.VKicker method), 67
+Step() (pybdsim.Gmad.Survey method), 87
 
 Index
 
-Study (class in pybdsim.Run), 91
+Study (class in pybdsim.Run), 96
 SubplotsWithDrawnMachineLattice() (in module
-pybdsim.Plot), 90
-SuggestFodoK() (in module pybdsim.Builder), 62
-Survey (class in pybdsim.Gmad), 82
-SwapAxes() (pybdsim.Data.TH2 method), 74
+pybdsim.Plot), 95
+SuggestFodoK() (in module pybdsim.Builder), 66
+Survey (class in pybdsim.Gmad), 86
+SwapAxes() (pybdsim.Data.TH2 method), 78
 SynchrotronRadiationRescale()
-(pybdsim.Builder.Machine method), 60
+(pybdsim.Builder.Machine method), 64
 
 T
-TH1 (class in pybdsim.Data), 73
-TH2 (class in pybdsim.Data), 74
-TH3 (class in pybdsim.Data), 74
-ThinMultipole (class in pybdsim.Builder), 63
-ThreeDData (class in pybdsim.Field.FieldPlotter), 80
-TKicker (class in pybdsim.Builder), 63
-ToDF() (pybdsim.Data.BDSAsciiData method), 70
-Trajectory3D() (in module pybdsim.Plot), 90
-TrajectoryData (class in pybdsim.Data), 75
-Transform3D (class in pybdsim.Builder), 63
+TH1 (class in pybdsim.Data), 77
+TH2 (class in pybdsim.Data), 78
+TH3 (class in pybdsim.Data), 78
+ThinMultipole (class in pybdsim.Builder), 67
+ThreeDData (class in pybdsim.Field.FieldPlotter), 84
+TKicker (class in pybdsim.Builder), 67
+ToDF() (pybdsim.Data.BDSAsciiData method), 74
+Trajectory3D() (in module pybdsim.Plot), 95
+TrajectoryData (class in pybdsim.Data), 79
+Transform3D (class in pybdsim.Builder), 67
 TransportVsBDSIM() (in module pybdsim.Compare),
-64
-TRotationToAxisAngle() (in module pybdsim.Data), 75
-Tunnel (class in pybdsim.Builder), 63
-TwoDData (class in pybdsim.Field.FieldPlotter), 81
+68
+TRotationToAxisAngle() (in module pybdsim.Data), 79
+Tunnel (class in pybdsim.Builder), 67
+TwoDData (class in pybdsim.Field.FieldPlotter), 85
 
 U
-Undulator (class in pybdsim.Builder), 63
+Undulator (class in pybdsim.Builder), 67
 UpdateCategoryParameter()
-(pybdsim.Builder.Machine method), 60
+(pybdsim.Builder.Machine method), 64
 UpdateElement()
 (pybdsim.Builder.Machine
-method), 61
+method), 65
 UpdateElements()
 (pybdsim.Builder.Machine
-method), 61
+method), 65
 UpdateGlobalParameter()
-(pybdsim.Builder.Machine method), 61
+(pybdsim.Builder.Machine method), 65
 
 V
-VKicker (class in pybdsim.Builder), 63
+VKicker (class in pybdsim.Builder), 67
 
 W
-WireScanner (class in pybdsim.Builder), 63
-WrapLatticeAboutItem() (in module pybdsim.ModelProcessing), 83
-Write() (pybdsim.Builder.Machine method), 61
-Write() (pybdsim.Field._Field.Field method), 75
+WireScanner (class in pybdsim.Builder), 67
+WrapLatticeAboutItem() (in module pybdsim.ModelProcessing), 87
+Write() (pybdsim.Builder.Machine method), 65
+Write() (pybdsim.Field._Field.Field method), 79
 write()
 (pybdsim.Gmad.GmadFileComponents
-method), 81
-WriteBeam() (pybdsim.Writer.Writer method), 93
-WriteBias() (pybdsim.Writer.Writer method), 93
+method), 85
+WriteBeam() (pybdsim.Writer.Writer method), 98
+WriteBias() (pybdsim.Writer.Writer method), 98
 WriteComponents() (pybdsim.Writer.Writer method),
-93
+98
 WriteFLUKA2DFormat1()
-(pybdsim.Field._Field.Field method), 76
+(pybdsim.Field._Field.Field method), 80
 WriteInMain() (pybdsim.Writer.FileSection method),
-93
-WriteMachine() (pybdsim.Writer.Writer method), 94
-109
+97
+WriteMachine() (pybdsim.Writer.Writer method), 98
+113
 
-pybdsim Documentation, Release 3.1.0
+pybdsim Documentation, Release 3.2.0
 
-WriteMain() (pybdsim.Writer.Writer method), 94
+WriteMain() (pybdsim.Writer.Writer method), 98
 WriteMaterial() (pybdsim.Writer.Writer method),
-94
-WriteObjects() (pybdsim.Writer.Writer method), 94
-WriteOptions() (pybdsim.Writer.Writer method), 94
-Writer (class in pybdsim.Writer), 93
+98
+WriteObjects() (pybdsim.Writer.Writer method), 98
+WriteOptions() (pybdsim.Writer.Writer method), 98
+Writer (class in pybdsim.Writer), 97
 WriteROOTHistogramsToDirectory() (in module
-pybdsim.Data), 75
+pybdsim.Data), 79
 WriteSamplers() (pybdsim.Writer.Writer method),
-94
+99
 WriteSeparately()
 (pybdsim.Writer.FileSection
-method), 93
+method), 97
 WriteSequence() (pybdsim.Writer.Writer method),
-94
-WriteToFile() (pybdsim.Beam.Beam method), 54
+99
+WriteToFile() (pybdsim.Beam.Beam method), 58
 
 X
-XSecBias (class in pybdsim.Builder), 63
-XSecBias (class in pybdsim.XSecBias), 94
+XSecBias (class in pybdsim.Builder), 67
+XSecBias (class in pybdsim.XSecBias), 99
 
 Z
-ZeroMissingRequiredColumns() (in module pybdsim.Convert._MadxTfs2Gmad), 69
+ZeroMissingRequiredColumns() (in module pybdsim.Convert._MadxTfs2Gmad), 73
 
-110
+114
 
 Index
```

### Comparing `pybdsim-3.1.1/docs/source/builder.rst` & `pybdsim-3.2.0/docs/source/builder.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/classes.rst` & `pybdsim-3.2.0/docs/source/classes.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/compare.rst` & `pybdsim-3.2.0/docs/source/compare.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/conf.py` & `pybdsim-3.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/convert.rst` & `pybdsim-3.2.0/docs/source/convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/data.rst` & `pybdsim-3.2.0/docs/source/data.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/data_uproot.rst` & `pybdsim-3.2.0/docs/source/data_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/developer.rst` & `pybdsim-3.2.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/fieldmaps.rst` & `pybdsim-3.2.0/docs/source/fieldmaps.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/figures/rebdsimFileHistograms.png` & `pybdsim-3.2.0/docs/source/figures/rebdsimFileHistograms.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/figures/rebdsimFileHistogramsWrapped.png` & `pybdsim-3.2.0/docs/source/figures/rebdsimFileHistogramsWrapped.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/figures/rebdsimFileMembers.png` & `pybdsim-3.2.0/docs/source/figures/rebdsimFileMembers.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/figures/simpleHistogramPlot.png` & `pybdsim-3.2.0/docs/source/figures/simpleHistogramPlot.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/installation.rst` & `pybdsim-3.2.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/licence.rst` & `pybdsim-3.2.0/docs/source/licence.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/moduledocs.rst` & `pybdsim-3.2.0/docs/source/moduledocs.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/support.rst` & `pybdsim-3.2.0/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/docs/source/version_history.rst` & `pybdsim-3.2.0/docs/source/version_history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 ===============
 Version History
 ===============
 
+V3.2.0 - 2023 / 04 / 26
+=======================
+
+* Remove the function :code:`pybdsim.Plot.AddMachineLatticeToFigure()`. This was just a forward to
+  :code:`pymadx.Plot.AddMachineLatticeToFigure()` and this should be used explicitly for
+  machine diagram plotting for TFS files. Otherwise, :code:`pybdsim.Plot.AddMachineLatticeFromSurveyToFigure`
+  should be used.
+* Better documentation about plotting.
+* Increase the visibility of light grey elements in the machine diagram from alpha 0.1 to 0.4.
+  
+
 V3.1.1 - 2023 / 04 / 23
 =======================
 
 * Fixed spectra loading and plotting for when the 'p' and 's' prefixes are used
   in the rebdsim Spectra command to denote primary and secondary particles.
 * Fixed error with default log scale in `Plot.Histogram2D` when no `vmin` was specified.
 * Fix :code:`pybdsim._version_tuple` which should be :code:`pybdsim.__version_tuple__`.
```

### Comparing `pybdsim-3.1.1/examples/1_builder/1_testmachine.png` & `pybdsim-3.2.0/examples/1_builder/1_testmachine.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/1_madxtfs2gmad.png` & `pybdsim-3.2.0/examples/2_convert/1_madxtfs2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/2_convert.rst` & `pybdsim-3.2.0/examples/2_convert/2_convert.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/2_transport2gmad.png` & `pybdsim-3.2.0/examples/2_convert/2_transport2gmad.png`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/transport_example.dat` & `pybdsim-3.2.0/examples/2_convert/transport_example.dat`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/transport_example.pdf` & `pybdsim-3.2.0/examples/2_convert/transport_example.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.pdf` & `pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.pdf`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/2_convert/twiss35tevb1_short.tar.gz` & `pybdsim-3.2.0/examples/2_convert/twiss35tevb1_short.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/3_optics/optics_validation.py` & `pybdsim-3.2.0/examples/3_optics/optics_validation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/examples/4_uproot/4_uproot.rst` & `pybdsim-3.2.0/examples/4_uproot/4_uproot.rst`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/pyproject.toml` & `pybdsim-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Beam.py` & `pybdsim-3.2.0/src/pybdsim/Beam.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Builder.py` & `pybdsim-3.2.0/src/pybdsim/Builder.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_BdsimBdsimComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_BdsimBdsimComparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 """
 
 import datetime as _datetime
 import matplotlib.pyplot as _plt
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 import os.path as _path
 
-import pybdsim.Data
-import pybdsim.Plot
+import pybdsim.Data as _Data
+import pybdsim.Plot as _Plot
+
+import pymadx as _pymadx
 
 # Predefined lists of tuples for making the standard plots,
 # format = (optical_var_name, optical_var_error_name, legend_name)
 
 _BETA = [("Beta_x", "Sigma_Beta_x", r'$\beta_{x}$'),
          ("Beta_y", "Sigma_Beta_y", r'$\beta_{y}$')]
 
@@ -44,24 +46,24 @@
    be a path to a BDSIM root output file, rebdsimOptics output file,
    or a BDSAsciiData instance, and in either case, generate a
    name if None is provided, and return that as well."""
    if isinstance(bdsim_in, str):
        if not _path.isfile(bdsim_in):
            raise IOError("file \"{}\" not found!".format(bdsim_in))
        name = (_path.splitext(_path.basename(bdsim_in))[0] if name is None else name)
-       data = pybdsim.Data.Load(bdsim_in)
+       data = _Data.Load(bdsim_in)
        if hasattr(data, 'optics'):
            data = data.optics
        elif hasattr(data, 'Optics'):
            data = data.Optics
        else:
            raise AttributeError("No optics found for BDSIM file: {}".format(bdsim_in))
        return data, name
    try:
-       if isinstance(bdsim_in, pybdsim.Data.RebdsimFile):
+       if isinstance(bdsim_in, _Data.RebdsimFile):
            if hasattr(bdsim_in, 'optics'):
                bdsim_in = bdsim_in.optics
            elif hasattr(bdsim_in,'Optics'):
                bdsim_in = bdsim_in.Optics
            else:
                raise AttributeError("No optics found in rebdsim file.")
        name = bdsim_in.filename if name is None else name
@@ -112,17 +114,17 @@
         axes = _plt.gcf().gca()
         axes.set_ylabel(y_label)
         axes.set_xlabel(x_label)
         axes.legend(loc='best')
 
         if survey is not None:
             try:
-                pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
+                _Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
             except IOError:
-                pybdsim.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
+                _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
         _plt.show(block=False)
         return plot
    return f_out
 
 PlotBeta   = _make_plotter(_BETA,    "S / m", r"$\beta_{x,y}$ / m",      "Beta")
 PlotAlpha  = _make_plotter(_ALPHA,   "S / m", r"$\alpha_{x,y}$ / m",     "Alpha")
 PlotDisp   = _make_plotter(_DISP,    "S / m", r"$D_{x,y} / m$",          "Dispersion")
@@ -150,17 +152,17 @@
     axes = _plt.gcf().gca()
     axes.set_ylabel(r'N Particles')
     axes.set_xlabel('S / m')
     axes.legend(loc='best')
 
     if survey is not None:
         try:
-            pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
+            _Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
         except IOError:
-            pybdsim.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
+            _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
     _plt.show(block=False)
 
     return plot
 
 
 def BDSIMVsBDSIM(first, second, first_name=None,
                  second_name=None, survey=None, saveAll=True,
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_ElegantBdsimComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_ElegantBdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_Mad8BdsimComparisonOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_MadxBdsimComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_MadxBdsimComparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,15 +581,15 @@
     if survey is None:
         return
     if isinstance(survey, str): # If BDSIM ASCII survey file
         if survey.split(".")[-1] == 'dat':
             _pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(figure,survey)
     # If BDSIM ASCII survey instance
     elif isinstance(survey, _pybdsim.Data.BDSAsciiData):
-        _pybdsim.Plot.AddMachineLatticeToFigure(figure,survey)
+        _pymadx.Plot.AddMachineLatticeToFigure(figure,survey)
     elif isinstance(survey, _pymadx.Data.Tfs): # If TFS
         _pymadx.Plot.AddMachineLatticeToFigure(figure,survey)
     # if a (BDSIM) ROOT file
     elif _pybdsim._General.IsROOTFile(survey):
         pass
 
 def _ProcessInput(tfsOptics, bdsimOptics):
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_MultipleCodeComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_MultipleCodeComparison.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
         axes.set_xlabel(x_label)
         axes.legend(loc='best')
 
         if survey is not None:
             try:
                 _pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
             except IOError:
-                _pybdsim.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
+                _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
         _plt.show(block=False)
 
         if saveFig:
             _plt.savefig(title+".pdf")
 
         return plot
     return f_out
@@ -990,14 +990,14 @@
     axes.set_xlabel('S / m')
     axes.legend(loc='best')
 
     if survey is not None:
         try:
             _pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
         except IOError:
-            _pybdsim.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
+            _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
     _plt.show(block=False)
 
     if saveFig:
         _plt.savefig("NPart" + ".pdf")
 
     return npartPlot
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_SadComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_SadComparison.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/_TransportBdsimComparison.py` & `pybdsim-3.2.0/src/pybdsim/Compare/_TransportBdsimComparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         axes.set_xlabel(x_label)
         axes.legend(loc='best')
 
         if survey is not None:
            try:
                pybdsim.Plot.AddMachineLatticeFromSurveyToFigure(_plt.gcf(), survey)
            except IOError:
-               pybdsim.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
+               _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(), survey)
         _plt.show(block=False)
         return plot
     return f_out
 
 PlotBeta   = _make_plotter(_BETA,    "S / m", r"$\beta_{x,y}$ / m",      "Beta")
 PlotAlpha  = _make_plotter(_ALPHA,   "S / m", r"$\alpha_{x,y}$ / m",     "Alpha")
 PlotDisp   = _make_plotter(_DISP,    "S / m", r"$D_{x,y} / m$",          "Dispersion")
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Compare/__init__.py` & `pybdsim-3.2.0/src/pybdsim/Compare/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Constants.py` & `pybdsim-3.2.0/src/pybdsim/Constants.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_BdsimElement2TransferMatrix.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_BdsimPrimaries2Inrays.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_CPyMad2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_CPyMad2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_ElegantParamToStrength.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_ElegantParamToStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Saveline2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Saveline2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_Mad8Twiss2GmadOld.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_MadxTfs2GmadStrength.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_MadxTfs2GmadStrength.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_Rebdsim2Numpy.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_Rebdsim2Numpy.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_SadFlat2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_SadFlat2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/_Transport2Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Convert/_Transport2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/__init__.py` & `pybdsim-3.2.0/src/pybdsim/Convert/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Convert/collimator_analysis.py` & `pybdsim-3.2.0/src/pybdsim/Convert/collimator_analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Data.py` & `pybdsim-3.2.0/src/pybdsim/Data.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/DataUproot.py` & `pybdsim-3.2.0/src/pybdsim/DataUproot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Field/FieldPlotter.py` & `pybdsim-3.2.0/src/pybdsim/Field/FieldPlotter.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Field/FieldPlotterVtk.py` & `pybdsim-3.2.0/src/pybdsim/Field/FieldPlotterVtk.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Field/_Field.py` & `pybdsim-3.2.0/src/pybdsim/Field/_Field.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Field/__init__.py` & `pybdsim-3.2.0/src/pybdsim/Field/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Geant4.py` & `pybdsim-3.2.0/src/pybdsim/Geant4.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Gmad.py` & `pybdsim-3.2.0/src/pybdsim/Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Joinhistograms.py` & `pybdsim-3.2.0/src/pybdsim/Joinhistograms.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/ModelProcessing.py` & `pybdsim-3.2.0/src/pybdsim/ModelProcessing.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Analysis.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Analysis.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRoot.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/AnalysisRootOptics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Event.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Event.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Processed.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Processed.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/Root.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/Root.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Obsolete/Rebdsim/__init__.py` & `pybdsim-3.2.0/src/pybdsim/Obsolete/Rebdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Optics.py` & `pybdsim-3.2.0/src/pybdsim/Optics.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Options.py` & `pybdsim-3.2.0/src/pybdsim/Options.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Plot.py` & `pybdsim-3.2.0/src/pybdsim/Plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 import pymadx as _pymadx
 
 import copy as _copy
 import matplotlib as _matplotlib
 from matplotlib.colors import LogNorm as _LogNorm
 import matplotlib.pyplot as _plt
 import matplotlib.patches as _patches
-import matplotlib.ticker as _ticker
 import numpy as _np
-import string as _string
 import datetime as _datetime
 from matplotlib.backends.backend_pdf import PdfPages as _PdfPages
 from scipy import constants as _con
 import os.path as _ospath
 
 from ._General import CheckItsBDSAsciiData as _CheckItsBDSAsciiData
 from ._General import CheckBdsimDataHasSurveyModel as _CheckBdsimDataHasSurveyModel
@@ -38,20 +36,14 @@
 
 def MadxTfsBeta(tfsfile, title='', outputfilename=None):
     """
     A forward to the pymadx.Plot.PlotTfsBeta function.
     """
     _pymadx.Plot.Beta(tfsfile,title,outputfilename)
 
-def AddMachineLatticeToFigure(figure, tfsfile, tightLayout=True):
-    """
-    A forward to the pymadx.Plot.AddMachineLatticeToFigure function.
-    """
-    _pymadx.Plot.AddMachineLatticeToFigure(figure, tfsfile, tightLayout)
-
 def ProvideWrappedS(sArray, index):
     s = sArray #shortcut
     smax = s[-1]
     sind = s[index]
     snewa = s[index:]
     snewa = snewa - sind
     snewb = s[:index]
@@ -98,26 +90,37 @@
     """
     d = _CheckItsBDSAsciiData(machines[0])
     if len(machines) > 1:
         for machine in machines[1:]:
             d.ConcatenateMachine(machine)
     return d
 
-def AddMachineLatticeFromSurveyToFigure(figure, surveyfile,
-                                        tightLayout=True, sOffset=0., fraction=0.9):
+def AddMachineLatticeFromSurveyToFigure(figure, surveyfile, tightLayout=True, sOffset=0., fraction=0.9):
     """
-    Add a machine diagram to the top of the plot in a current figure
-    sOffset offsets survey along s
-    fraction controls fraction of the figure for the plot, the remainder being used for the survey
+    Add a machine diagram to the top of the plot in a current figure.
+
+    :param figure: the matplotlib figure to add the plot to.
+    :type figure: matplotlib.figure.Figure
+    :param surveyfile: BDSIM file or REBDSIM file (with Model tree filled) or BDSIM survey output or path to any of these.
+    :type surveyfile: str, pybdsim.Data.RebdsimFile, pybdsim.Data.BDSAsciiData, cppyy.gbl.DataLoader
+    :param tightLayout: whether to call matplotlib's tight layout after adding the axes.
+    :type tightLayout: bool
+    :param sOffset: add this number to the S coordinate of all elements in the machine diagram.
+    :type sOffset: float
+    :param fraction: controls fraction of the figure for the plot, the remainder being used for the survey.
+    :type fraction: float
     """
     from . import Data as _Data
     if isinstance(surveyfile, str) and not _ospath.isfile(surveyfile):
         raise IOError("Survey not found: ", surveyfile)
     if _CheckBdsimDataHasSurveyModel(surveyfile):
-        sf = _Data.Load(surveyfile).model
+        if hasattr(surveyfile, "model"):
+            sf = surveyfile.model
+        else:
+            sf = _Data.Load(surveyfile).model
     else:
         sf = _CheckItsBDSAsciiData(surveyfile)
 
     # we don't need to check this has the required columns because we control a
     # BDSIM survey contents.
 
     axoptics  = figure.get_axes()
@@ -142,14 +145,28 @@
 
     MachineXlim(axmachine)
     axmachine.callbacks.connect('xlim_changed', MachineXlim)
     figure.canvas.mpl_connect('button_press_event', Click)
 
 
 def DrawMachineLattice(axesinstance, bdsasciidataobject, sOffset=0.0):
+    """
+    The low-level version of drawing a machine diagram. Draws into an axes instance
+    given using loaded model data in the form of a pybdsim.Data.BDSAsciiData instance.
+
+    :param axesinstance: the plotting axis to draw the machine diagram into.
+    :type axesinstance: matplotlib.axes.Axes
+    :param: bdsasciidataobject The model data.
+    :type bdsasciidataobject: pybdsim.Data.BDSAsciiData
+    :param sOffset: add this value to the S of all machine elements in the diagram.
+    :type sOffset: float
+
+    The main interface is AddMachineLatticeFromSurveyToFigure, but this function
+    may be useful for more granular plotting, e.g. with custom subfigures / axes.
+    """
     ax  = axesinstance #handy shortcut
     bds = bdsasciidataobject
 
     def DrawBend(start,length,color='b',alpha=1.0):
         br = _patches.Rectangle((start,-0.1),length,0.2,color=color,alpha=alpha)
         ax.add_patch(br)
     def DrawQuad(start,length,k1,color='r',alpha=1.0):
@@ -215,39 +232,37 @@
         elif kw == 'shield':
             DrawRect(starts[i],lengths[i], u'#808080') #dark grey
         elif kw == 'rf' or kw == 'rfcavity' or kw == 'cavity_pillbox':
             DrawRect(starts[i],lengths[i], u'#768799') #srf grey
         else:
             #unknown so make light in alpha
             if lengths[i] > 1e-1:
-                DrawRect(starts[i],lengths[i],'#cccccc',alpha=0.1) #light grey
+                DrawRect(starts[i],lengths[i],'#cccccc',alpha=0.4) #light grey
             else:
                 #relatively short element - just draw a line
-                DrawLine(starts[i],'#cccccc',alpha=0.1)
+                DrawLine(starts[i],'#cccccc',alpha=0.4)
 
     # plot beam line
     smax = bds.SEnd()[-1] + sOffset
     ax.plot([sOffset, smax],[0,0],'k-',lw=1)
     ax.set_ylim(-0.2,0.2)
     ax.set_xlim(sOffset, smax)
 
-def SubplotsWithDrawnMachineLattice(survey, nrows=2,
-                                    machine_plot_gap=0.01,
-                                    gridspec_kw=None,
-                                    subplots_kw=None, **fig_kw):
+def SubplotsWithDrawnMachineLattice(survey, nrows=2, machine_plot_gap=0.01, gridspec_kw=None, subplots_kw=None, **fig_kw):
     """
     Create a figure with a single column of axes, sharing the
     x-axis by default, with the machine drawn from the provided survey
     on the top row axes.  nrows gives the number of axes, the first is
     always the machine lattice.  by default 2 are drawn, the first for
     the machine, and the second for any data to be plotted to
     afterwards.
 
-    Parameters:
-    survey : BSDIM survey which is used to draw the machine lattice on the top axes.
+    :param survey: BDSIM survey which is used to draw the machine lattice on the top axes.
+    :type survey: str, pybdsim.Data.BDSAsciiData
+
     machine_plot_gap : vertical space between the top of the first axes and the 
     bottom of the machine axes. By default this is small.
 
     Returns (figure, machine_axes, (axes1, axes2, ...))
 
     figure : Figure instance.
     machine_axes : Axes instance with the machine drawn on it.  Can be used to further edit
@@ -1301,15 +1316,15 @@
     ylabel = r"Energy Deposition / Event (GeV / {} m)".format(round(xwidth,2))
     f = Histogram1D(eloss, xlabel='S (m)', ylabel=ylabel)
 
     ax = f.get_axes()[0]
     ax.set_yscale('log')
 
     if tfssurvey:
-        AddMachineLatticeToFigure(f, tfssurvey)
+        _pymadx.Plot.AddMachineLatticeToFigure(f, tfssurvey)
     elif bdsimsurvey:
         AddMachineLatticeFromSurveyToFigure(f, bdsimsurvey)
     elif hasattr(d, "model"):
         AddMachineLatticeFromSurveyToFigure(f, d.model)
 
     if outputfilename is not None:
         _plt.savefig(outputfilename)
@@ -1466,15 +1481,15 @@
     ax.set_xlabel(xlabel)
     ax.set_ylabel(ylabel)
     ax.yaxis.set_major_locator(_plt.LogLocator(subs=(1.0,))) #TODO: Find a way to disable auto ticks and always display all int powers
     ax.yaxis.grid(which="major", linestyle='--')
     _plt.legend(fontsize="small", framealpha=1)# bbox_to_anchor=(0.85, 1), loc=2, borderaxespad=0., framealpha=1)
 
     if tfssurvey:
-        AddMachineLatticeToFigure(f, tfssurvey)
+        _pymadx.Plot.AddMachineLatticeToFigure(f, tfssurvey)
     elif bdsimsurvey and not skipMachineLattice:
         #AddMachineLatticeFromSurveyToFigure(f, bdsimsurvey) #TODO: Fix this, currenly gives an error
         print("not working like this")
     elif hasattr(d, "model"):
         AddMachineLatticeFromSurveyToFigure(f, d.model)
 
     if outputfilename is not None:
@@ -1495,15 +1510,15 @@
     ax1.set_ylabel('Fraction of Beam Surviving')
 
     survival = 1.0 - _np.cumsum(ploss.contents)
     ax1.plot(ploss.xcentres, survival)
     ax1.set_xlabel('S (m)')
 
     if tfssurvey:
-        AddMachineLatticeToFigure(fig, tfssurvey)
+        _pymadx.Plot.AddMachineLatticeToFigure(fig, tfssurvey)
     elif bdsimsurvey:
         AddMachineLatticeFromSurveyToFigure(fig, bdsimsurvey)
     elif hasattr(d, "model"):
         AddMachineLatticeFromSurveyToFigure(fig, d.model)
 
     if outputfilename is not None:
         _plt.savefig(outputfilename)
@@ -1562,15 +1577,15 @@
 
     ax1.legend(loc=hitslegendloc)
     ax2.legend(loc=elosslegendloc)
 
     ax1.set_xlabel('S (m)')
 
     if tfssurvey:
-        AddMachineLatticeToFigure(fig, tfssurvey)
+        _pymadx.Plot.AddMachineLatticeToFigure(fig, tfssurvey)
     elif bdsimsurvey:
         AddMachineLatticeFromSurveyToFigure(fig, bdsimsurvey)
     elif hasattr(d, "model"):
         AddMachineLatticeFromSurveyToFigure(fig, d.model)
 
     if outputfilename is not None:
         _plt.savefig(outputfilename)
@@ -1868,22 +1883,21 @@
     line, = ax.plot(xcentres, y, drawstyle='steps-mid', **kwargs)
     kwargs.pop("label", None) # Only attach label to the line plot.
     kwargs.pop("color", None) # Duplicate kwargs is an error, it is set below.
     ax.fill_between(xcentres, low, y, step='mid',
                     color=line.get_color(),
                     **kwargs)
 
-"""
-The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey
-done in BDSIM. The results can be found in the BDSIM output file in the Model tree.
-The functions can plot the start and end positions of each element in the sequence.
-"""
 
 def ModelBDSIMXZ(model, ax=None):
-
+    """
+    The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey
+    done in BDSIM. The results can be found in the BDSIM output file in the Model tree.
+    The functions can plot the start and end positions of each element in the sequence.
+    """
     staPos = model.staRefPos
     endPos = model.endRefPos
 
     typ = model.componentType
 
     #xr = (_np.min([_np.min(staPos[:,0]), _np.min(endPos[:,0])]), _np.max([_np.max(staPos[:,0]), _np.max(endPos[:,0])]))
     #zr = (_np.min([_np.min(staPos[:,2]), _np.min(endPos[:,2])]), _np.max([_np.max(staPos[:,2]), _np.max(endPos[:,2])]))
@@ -1898,14 +1912,19 @@
         ax.plot([s[2],e[2]],[s[0],e[0]],'k-')
 
     _plt.xlabel('Z (m)')
     _plt.ylabel('X (m)')
     _plt.tight_layout()
 
 def ModelBDSIMYZ(model, ax=None):
+    """
+    The ModelBDSIMXZ and ModelBDSIMYZ functions add the possibility to plot a survey
+    done in BDSIM. The results can be found in the BDSIM output file in the Model tree.
+    The functions can plot the start and end positions of each element in the sequence.
+    """
 
     staPos = model.staRefPos
     endPos = model.endRefPos
 
     typ = model.componentType
 
     #xr = (_np.min([_np.min(staPos[:,0]), _np.min(endPos[:,0])]), _np.max([_np.max(staPos[:,0]), _np.max(endPos[:,0])]))
@@ -1921,15 +1940,17 @@
         ax.plot([s[2],e[2]],[s[1],e[1]],'k-')
 
     _plt.xlabel('Z (m)')
     _plt.ylabel('Y (m)')
     _plt.tight_layout()
 
 def ModelElegantXZ(model, ax=None, transpose=False):
-
+    """
+    Plot a model madx from elegant. In development.
+    """
     X = model['X']
     Z = model['Z']
     if transpose:
         xi = X
         X = Z
         Z = xi
     XZ = _np.stack([X,Z],axis=1)
@@ -1951,15 +1972,17 @@
         _plt.ylabel('Z (m)')
     else:
         _plt.xlabel('Z (m)')
         _plt.ylabel('X (m)')
     _plt.tight_layout()
 
 def ModelElegantYZ(model, ax=None, transpose=False):
-
+    """
+    Plot a model madx from elegant. In development.
+    """
     Y = model['Y']
     Z = model['Z']
     if transpose:
         yi = Y
         Y = Z
         Z = yi
     YZ = _np.stack([Y,Z],axis=1)
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Run.py` & `pybdsim-3.2.0/src/pybdsim/Run.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Testing/bdsimMadx.py` & `pybdsim-3.2.0/src/pybdsim/Testing/bdsimMadx.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
             _plt.errorbar(B_s,B_optfn_y, yerr=B_opterr_y,fmt='o',color='b',label=r'$'+fn_name+fn_subsc[1]+r'$BDS')
             #_plt.plot([], [], color='r', linewidth=10,alpha=0.3,label=r'$'+fn_name+fn_subsc[0]+r'$PTC')
             #_plt.plot([], [], color='b', linewidth=10,alpha=0.3,label=r'$'+fn_name+fn_subsc[1]+r'$PTC')
             _plt.xlabel(r'$S (m)$')
             _plt.ylabel(r'$'+fn_name+fn_units+r'$')
             _plt.legend(numpoints=1,loc=10,fancybox=True, framealpha=1.0,prop={'size':15})
             _plt.grid(True)
-            _Plot.AddMachineLatticeToFigure(_plt.gcf(),madx)
+            _pymadx.Plot.AddMachineLatticeToFigure(_plt.gcf(),madx)
             #_plt.subplots_adjust(left=0.1,right=0.9,top=0.96, bottom=0.15, wspace=0.15, hspace=0.2)
 
         if showResiduals:
             #optical function residuals
             """
             if(in_Tfs):
                 res_optfn_x = M_optfn_x-B_optfn_x
```

### Comparing `pybdsim-3.1.1/src/pybdsim/Testing/trackingTester.py` & `pybdsim-3.2.0/src/pybdsim/Testing/trackingTester.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Visualisation.py` & `pybdsim-3.2.0/src/pybdsim/Visualisation.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/Writer.py` & `pybdsim-3.2.0/src/pybdsim/Writer.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/XSecBias.py` & `pybdsim-3.2.0/src/pybdsim/XSecBias.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim/_General.py` & `pybdsim-3.2.0/src/pybdsim/_General.py`

 * *Files 11% similar despite different names*

```diff
@@ -86,27 +86,25 @@
     elif type(bfile) == _Data.RebdsimFile:
         data = CheckOptics(bfile, requireOptics)
     else:
         raise IOError("Not pybdsim.Data.BDSAsciiData file type: "+str(bfile))
     return data
 
 def CheckBdsimDataHasSurveyModel(bfile):
+    data = None
     if isinstance(bfile, str):
         data = _Data.Load(bfile)
     elif type(bfile) == _Data.BDSAsciiData:
         data = bfile
     elif type(bfile) == _Data.RebdsimFile:
         data = bfile
     else:
-        return False
+        data = bfile
 
-    if hasattr(data,"model"):
-        return True
-    else:
-        return False
+    return hasattr(data,"model")
 
 def PrepareReducedName(elementname):
     """
     Only allow alphanumeric characters and '_'
     """
     rname = _re.sub('[^a-zA-Z0-9_]+','',elementname)
     return rname
```

### Comparing `pybdsim-3.1.1/src/pybdsim/__init__.py` & `pybdsim-3.2.0/src/pybdsim/__init__.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/src/pybdsim.egg-info/PKG-INFO` & `pybdsim-3.2.0/src/pybdsim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybdsim
-Version: 3.1.1
+Version: 3.2.0
 Summary: Python utilities for the Monte Carlo Particle accelerator code BDSIM.
 Author-email: "JAI@RHUL" <laurie.nevay@cern.ch>
 Maintainer-email: Laurie Nevay <laurie.nevay@cern.ch>
 Project-URL: homepage, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: documentation, http://www.pp.rhul.ac.uk/bdsim/pybdsim
 Project-URL: repository, https://bitbucket.org/jairhul/pybdsim
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pybdsim-3.1.1/src/pybdsim.egg-info/SOURCES.txt` & `pybdsim-3.2.0/src/pybdsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/source/data_uproot.rst
 docs/source/developer.rst
 docs/source/fieldmaps.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/licence.rst
 docs/source/moduledocs.rst
+docs/source/plotting.rst
 docs/source/support.rst
 docs/source/version_history.rst
 docs/source/figures/rebdsimFileHistograms.png
 docs/source/figures/rebdsimFileHistogramsWrapped.png
 docs/source/figures/rebdsimFileMembers.png
 docs/source/figures/simpleHistogramPlot.png
 examples/examples.rst
```

### Comparing `pybdsim-3.1.1/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz` & `pybdsim-3.2.0/tests/test_input/atf2-nominal-twiss-v5.2.tfs.tar.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_input/model-model-aper.tfs.gz` & `pybdsim-3.2.0/tests/test_input/model-model-aper.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_input/model-model.tfs.gz` & `pybdsim-3.2.0/tests/test_input/model-model.tfs.gz`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.2.0/tests/test_output/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output/model-model/model_components.gmad` & `pybdsim-3.2.0/tests/test_output/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output/model-model/model_sequence.gmad` & `pybdsim-3.2.0/tests/test_output/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad` & `pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad` & `pybdsim-3.2.0/tests/test_output2/atf2-nominal-twiss-v5.2/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output2/model-model/model_components.gmad` & `pybdsim-3.2.0/tests/test_output2/model-model/model_components.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/test_output2/model-model/model_sequence.gmad` & `pybdsim-3.2.0/tests/test_output2/model-model/model_sequence.gmad`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/tests/pybdsim_test_utils.py` & `pybdsim-3.2.0/tests/tests/pybdsim_test_utils.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/tests/test_MadxTfs2Gmad.py` & `pybdsim-3.2.0/tests/tests/test_MadxTfs2Gmad.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/tests/testratio.py` & `pybdsim-3.2.0/tests/tests/testratio.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/tests/write_test_outputs.py` & `pybdsim-3.2.0/tests/tests/write_test_outputs.py`

 * *Files identical despite different names*

### Comparing `pybdsim-3.1.1/tests/unit/test_Builder.py` & `pybdsim-3.2.0/tests/unit/test_Builder.py`

 * *Files identical despite different names*

