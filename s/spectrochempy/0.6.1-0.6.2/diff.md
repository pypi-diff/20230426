# Comparing `tmp/spectrochempy-0.6.1.tar.gz` & `tmp/spectrochempy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrochempy-0.6.1.tar", last modified: Thu Apr 13 09:17:25 2023, max compression
+gzip compressed data, was "spectrochempy-0.6.2.tar", last modified: Tue Apr 25 16:33:51 2023, max compression
```

## Comparing `spectrochempy-0.6.1.tar` & `spectrochempy-0.6.2.tar`

### file list

```diff
@@ -1,226 +1,227 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.codespellrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/.conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.conda/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/NMRGLUE_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/NNMF_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/PACKAGING_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/PANDAS_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/LICENSES/TRAITTYPES_LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/environment_dev.yml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/requirements/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/scp_data/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.513840 spectrochempy-0.6.1/scp_data/databases/
--rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/databases/isotopes.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scp_data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/Felipa-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/Humor-Sans.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/LICENSE_felipa.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/LICENSE_victormono.txt
--rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Oblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinOblique.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/fonts/comic-sans-ms.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scp_data/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/grayscale.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/notebook.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/paper.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/poster.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/sans.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/scpy.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/serif.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scp_data/stylesheets/talk.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scripts/checkindex.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/scripts/validate_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-13 09:17:25.561840 spectrochempy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.525840 spectrochempy-0.6.1/spectrochempy/
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52625 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/efa.py
--rw-r--r--   0 runner    (1001) docker     (123)    35689 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/iris.py
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/kinetic_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/linearregression.py
--rw-r--r--   0 runner    (1001) docker     (123)    43620 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/mcrals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/nnmf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/analysis/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9988 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    36844 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22702 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21132 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/simplisma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/analysis/svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/application/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43480 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/general_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/metaconfigurable.py
--rw-r--r--   0 runner    (1001) docker     (123)    47047 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/application/plot_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.533840 spectrochempy-0.6.1/spectrochempy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/common/dialogs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndio.py
--rw-r--r--   0 runner    (1001) docker     (123)   120723 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndmath.py
--rw-r--r--   0 runner    (1001) docker     (123)    27693 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/npy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.537840 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    23084 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndcomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)    34168 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/coord.py
--rw-r--r--   0 runner    (1001) docker     (123)    37998 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/coordset.py
--rw-r--r--   0 runner    (1001) docker     (123)    53899 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/dataset/nddataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/plotters/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/multiplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    26279 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plot3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/plotters/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/align.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/apodization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    28435 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/baseline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19449 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/phasing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/processors/zero_filling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.541840 spectrochempy-0.6.1/spectrochempy/core/project/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/abstractproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    18331 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7976 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    26561 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_carroucell.py
--rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_labspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_matlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    50613 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_omnic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_opus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_quadera.py
--rw-r--r--   0 runner    (1001) docker     (123)    14104 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_soc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19509 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_spc.py
--rw-r--r--   0 runner    (1001) docker     (123)    48164 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_topspin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/readers/read_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/script/
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/units/
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/units/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.549840 spectrochempy-0.6.1/spectrochempy/core/writers/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_jcamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/core/writers/write_matlab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.553840 spectrochempy-0.6.1/spectrochempy/extern/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/nmrglue.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/traittypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/extern/traittypes_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.553840 spectrochempy-0.6.1/spectrochempy/ipython/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/ipython/magics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.557840 spectrochempy-0.6.1/spectrochempy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/citation.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/coordrange.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/fake.py
--rw-r--r--   0 runner    (1001) docker     (123)    23056 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/jsonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/orderedset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/packages.py
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/print.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3402 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/print_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (123)    33935 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.557840 spectrochempy-0.6.1/spectrochempy/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/baselinecorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-13 09:17:00.000000 spectrochempy-0.6.1/spectrochempy/widgets/fileselector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 09:17:25.529840 spectrochempy-0.6.1/spectrochempy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-13 09:17:25.000000 spectrochempy-0.6.1/spectrochempy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.codespellrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/.conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.conda/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18144 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    21393 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/NMRGLUE_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/NNMF_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/PACKAGING_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/PANDAS_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/LICENSES/TRAITTYPES_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/environment_dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/requirements/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/scp_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.640977 spectrochempy-0.6.2/scp_data/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)    26810 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/databases/isotopes.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scp_data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    38040 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/Felipa-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    25832 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/Humor-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/LICENSE_felipa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/LICENSE_victormono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   157048 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   197120 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   164392 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150324 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184764 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156852 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188172 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150888 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188268 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157596 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153808 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   194336 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158228 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   151576 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155276 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   193176 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161200 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150284 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188288 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   157184 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinOblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105316 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/fonts/comic-sans-ms.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scp_data/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/grayscale.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/notebook.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/paper.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/poster.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/sans.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/scpy.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/serif.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scp_data/stylesheets/talk.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.648977 spectrochempy-0.6.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scripts/checkindex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/scripts/validate_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71384 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/efa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35136 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45878 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/kinetic_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/linearregression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43542 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/mcrals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/nnmf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/analysis/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9945 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36802 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20966 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/simplisma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/analysis/svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44877 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/general_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/metaconfigurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47043 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/application/plot_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/common/dialogs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.656978 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120597 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndmath.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/npy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74573 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22940 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndcomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34042 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/coord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37871 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/coordset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54110 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/dataset/nddataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/multiplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19702 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26241 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/plotters/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.660978 spectrochempy-0.6.2/spectrochempy/core/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/apodization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8403 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19302 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/phasing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/processors/zero_filling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/project/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/abstractproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18203 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29909 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_carroucell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_labspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_matlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40293 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_omnic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_opus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_quadera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_soc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16937 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_spc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_topspin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/readers/read_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/units/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.664978 spectrochempy-0.6.2/spectrochempy/core/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_jcamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/core/writers/write_matlab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.668978 spectrochempy-0.6.2/spectrochempy/extern/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64415 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/nmrglue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/traittypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/extern/traittypes_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.668978 spectrochempy-0.6.2/spectrochempy/ipython/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/ipython/magics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/spectrochempy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/coordrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14176 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/fake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23395 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/jsonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14888 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/orderedset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/print.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3422 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/print_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33712 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16115 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.672978 spectrochempy-0.6.2/spectrochempy/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14463 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/baselinecorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-25 16:33:30.000000 spectrochempy-0.6.2/spectrochempy/widgets/fileselector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:33:51.652978 spectrochempy-0.6.2/spectrochempy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:33:51.000000 spectrochempy-0.6.2/spectrochempy.egg-info/top_level.txt
```

### Comparing `spectrochempy-0.6.1/.codeclimate.yml` & `spectrochempy-0.6.2/.codeclimate.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/.conda/meta.yaml` & `spectrochempy-0.6.2/.conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/.gitignore` & `spectrochempy-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/.pre-commit-config.yaml` & `spectrochempy-0.6.2/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,21 @@
       - id: create-requirements
         name: create-requirements
         description: Create environment and requirement files according to a template
         entry: python .ci/create_requirements.py
         language: python
         additional_dependencies: [pyyaml, jinja2]
         pass_filenames: false
+      - id: update_version_and_release_notes
+        name: update_version_and_release_notes
+        description: Update version number and udate release notes
+        entry: python .ci/update_version_and_release_notes.py
+        language: python
+        additional_dependencies: [pyyaml, cffconvert, setuptools_scm]
+        pass_filenames: false
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: mixed-line-ending
```

### Comparing `spectrochempy-0.6.1/.pylintrc` & `spectrochempy-0.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/.zenodo.json` & `spectrochempy-0.6.2/.zenodo.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'publication_date'": "'2023-04-25'", "'version'": "'0.6.2'"}*

```diff
@@ -50,12 +50,12 @@
         "raman",
         "raman-spectra",
         "raman-spectroscopy",
         "spectroscopy",
         "uv-vis"
     ],
     "license": "CECILL-B",
-    "publication_date": "2023-04-13",
+    "publication_date": "2023-04-25",
     "title": "SpectroChemPy",
     "upload_type": "software",
-    "version": "0.6.1"
+    "version": "0.6.2"
 }
```

### Comparing `spectrochempy-0.6.1/CITATION.cff` & `spectrochempy-0.6.2/CITATION.cff`

 * *Files 22% similar despite different names*

```diff
@@ -11,20 +11,20 @@
   orcid: https://orcid.org/0000-0002-9579-8910
 - affiliation: "ENSICAEN, Universit\xE9 de Caen, CNRS (Laboratoire Catalyse et Spectrochimie)"
   email: christian.fernandez@ensicaen.fr
   family-names: Fernandez
   given-names: Christian
   orcid: https://orcid.org/0000-0002-5476-3148
 cff-version: 1.2.0
-date-released: '2023-04-13'
+date-released: '2023-04-25'
 identifiers:
 - description: Persistent identifier for all versions of SpectroChemPy
   type: doi
   value: 10.5281/zenodo.3823841
 license: CECILL-B
 message: If you use this software, please cite it using the metadata from this file.
 repository-code: https://github.com/spectrochempy/spectrochempy
 title: SpectroChemPy, a framework for processing, analyzing and modeling spectroscopic
   data for chemistry with Python
 type: software
 url: https://www.spectrochempy.fr
-version: 0.6.1
+version: 0.6.2
```

### Comparing `spectrochempy-0.6.1/Dockerfile` & `spectrochempy-0.6.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSE` & `spectrochempy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSES/NMRGLUE_LICENSE.rst` & `spectrochempy-0.6.2/LICENSES/NMRGLUE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSES/NNMF_LICENSE.rst` & `spectrochempy-0.6.2/LICENSES/NNMF_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSES/PACKAGING_LICENSE.rst` & `spectrochempy-0.6.2/LICENSES/PACKAGING_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSES/PANDAS_LICENSE.rst` & `spectrochempy-0.6.2/LICENSES/PANDAS_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/LICENSES/TRAITTYPES_LICENSE.rst` & `spectrochempy-0.6.2/LICENSES/TRAITTYPES_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/PKG-INFO` & `spectrochempy-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.1/README.md` & `spectrochempy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/environment.yml` & `spectrochempy-0.6.2/environment.yml`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/environment_dev.yml` & `spectrochempy-0.6.2/environment_dev.yml`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     - coverage
     - black
     - pre-commit
     - mamba
     - docrep
     - jupytext
     - sphinx=5.3
-    - sphinx_rtd_theme=1.1
+    - sphinx_rtd_theme=1.2
     - autodocsumm
     - sphinx-gallery
     - nbsphinx
     - jupyter_sphinx
     - json5
     - sphinx-copybutton
     - sphinxcontrib-bibtex
```

### Comparing `spectrochempy-0.6.1/requirements/requirements.txt` & `spectrochempy-0.6.2/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/requirements/requirements_dev.txt` & `spectrochempy-0.6.2/requirements/requirements_dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 coverage
 black
 pre-commit
 mamba
 docrep
 jupytext
 sphinx==5.3
-sphinx_rtd_theme==1.1
+sphinx_rtd_theme==1.2
 autodocsumm
 sphinx-gallery
 nbsphinx
 jupyter_sphinx
 json5
 sphinx-copybutton
 sphinxcontrib-bibtex
```

### Comparing `spectrochempy-0.6.1/scp_data/databases/isotopes.csv` & `spectrochempy-0.6.2/scp_data/databases/isotopes.csv`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/Felipa-Regular.ttf` & `spectrochempy-0.6.2/scp_data/fonts/Felipa-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/Humor-Sans.ttf` & `spectrochempy-0.6.2/scp_data/fonts/Humor-Sans.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/LICENSE_felipa.txt` & `spectrochempy-0.6.2/scp_data/fonts/LICENSE_felipa.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/LICENSE_victormono.txt` & `spectrochempy-0.6.2/scp_data/fonts/LICENSE_victormono.txt`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Bold.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-BoldOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLight.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ExtraLightOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ExtraLightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Italic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Light.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-LightOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-LightOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Medium.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-MediumOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-MediumOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Oblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Regular.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBold.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-SemiBoldOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-SemiBoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-Thin.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinItalic.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/VictorMono-ThinOblique.ttf` & `spectrochempy-0.6.2/scp_data/fonts/VictorMono-ThinOblique.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/fonts/comic-sans-ms.ttf` & `spectrochempy-0.6.2/scp_data/fonts/comic-sans-ms.ttf`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/stylesheets/grayscale.mplstyle` & `spectrochempy-0.6.2/scp_data/stylesheets/grayscale.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/stylesheets/notebook.mplstyle` & `spectrochempy-0.6.2/scp_data/stylesheets/notebook.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/stylesheets/sans.mplstyle` & `spectrochempy-0.6.2/scp_data/stylesheets/sans.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scp_data/stylesheets/scpy.mplstyle` & `spectrochempy-0.6.2/scp_data/stylesheets/scpy.mplstyle`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 figure.constrained_layout.hspace         : 0.02
 figure.constrained_layout.use            : False
 figure.constrained_layout.w_pad          : 0.04167
 figure.constrained_layout.wspace         : 0.02
 figure.dpi                               : 96.0
 figure.edgecolor                         : white
 figure.facecolor                         : white
-figure.figsize                           : 6.8, 4.4
+figure.figsize                           : 5.5, 3.5
 figure.frameon                           : True
 figure.subplot.bottom                    : 0.12
 figure.subplot.hspace                    : 0.0
 figure.subplot.left                      : 0.15
 figure.subplot.right                     : 0.95
 figure.subplot.top                       : 0.98
 figure.subplot.wspace                    : 0.0
```

### Comparing `spectrochempy-0.6.1/scp_data/stylesheets/serif.mplstyle` & `spectrochempy-0.6.2/scp_data/stylesheets/serif.mplstyle`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scripts/checkindex.py` & `spectrochempy-0.6.2/scripts/checkindex.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/scripts/validate_docstrings.py` & `spectrochempy-0.6.2/scripts/validate_docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/setup.cfg` & `spectrochempy-0.6.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [flake8]
 ignore = 
 	E203,
 	E402,
 	E501,
 	E703,
 	E731,
+	E902,
 	F405,
 	W503,
 	W504,
 	W605,
 	
 	N801
 	N802,
```

### Comparing `spectrochempy-0.6.1/setup.py` & `spectrochempy-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/__init__.py` & `spectrochempy-0.6.2/spectrochempy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,12 +76,7 @@
 
 
 def __getattr__(name):
     # NDDataset method accessible from the API
     if hasattr(NDDataset, name):
         return getattr(NDDataset, name)
     raise AttributeError
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/_base.py` & `spectrochempy-0.6.2/spectrochempy/analysis/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import inspect
 import logging
 import warnings
 from copy import copy
 from functools import partial, update_wrapper
 
+import matplotlib.pyplot as plt
 import numpy as np
 import traitlets as tr
 from sklearn import linear_model
 
 from spectrochempy.application.metaconfigurable import MetaConfigurable
 from spectrochempy.core import app, set_loglevel
 from spectrochempy.core.dataset.baseobjects.ndarray import NDArray
@@ -38,15 +39,17 @@
 class NotFittedError(exceptions.SpectroChemPyError):
     """
     Exception raised when an analysis estimator is not fitted
     but one use one of its method.
 
     Parameters
     ----------
-    attr :
+    attr : method, optional
+        The method from which the error was issued. In general it is determined
+        automatically.
     """
 
     def __init__(self, attr=None):
         frame = inspect.currentframe().f_back
         caller = frame.f_code.co_name if attr is None else attr
         model = frame.f_locals["self"].name
         message = (
@@ -54,29 +57,31 @@
             f" should be executed first"
         )
         super().__init__(message)
 
 
 # ======================================================================================
 # A decorator to transform np.ndarray output from models to NDDataset
-# according to the X input
+# according to the X (default) and/or Y input
 # ======================================================================================
 class _set_output(object):
     def __init__(
         self,
         method,
         *args,
+        meta_from="_X",  # the attribute or tuple of attributes from which meta data are taken
         units="keep",
         title="keep",
         typex=None,
         typey=None,
         typesingle=None,
     ):
         self.method = method
         update_wrapper(self, method)
+        self.meta_from = meta_from
         self.units = units
         self.title = title
         self.typex = typex
         self.typey = typey
         self.typesingle = typesingle
 
     @preserve_signature
@@ -92,104 +97,143 @@
         from spectrochempy.core.dataset.nddataset import NDDataset
 
         # HACK to be able to used deprecated alias of the method, without error
         # because if not this modification obj appears two times
         if args and type(args[0]) == type(obj):
             args = args[1:]
 
-        # get the sklearn data output
-        data = self.method(obj, *args, **kwargs)
+        # get the method output - one or two arrays depending on the method and *args
+        output = self.method(obj, *args, **kwargs)
 
         # restore eventually masked rows and columns
         axis = "both"
         if self.typex is not None and self.typex != "features":
             axis = 0
         elif self.typey is not None:
             axis = 1
 
-        # make a new dataset with this data
-        X_transf = NDDataset(data)
-
-        # Now set the NDDataset attributes from the original X
-
-        # determine the input X dataset
-        X = obj._X
-
-        if self.units is not None:
-            if self.units == "keep":
-                X_transf.units = X.units
-            else:
-                X_transf.units = self.units
-        X_transf.name = f"{X.name}_{obj.name}.{self.method.__name__}"
-        X_transf.history = f"Created using method {obj.name}.{self.method.__name__}"
-        if self.title is not None:
-            if self.title == "keep":
-                X_transf.title = X.title
+        # if a single array was returned...
+        if not isinstance(output, tuple):
+            # ... make a tuple of 1 array:
+            data_tuple = (output,)
+            # ... and a tuple of 1 from_meta element:
+            if not isinstance(self.meta_from, tuple):
+                meta_from_tuple = (self.meta_from,)
             else:
-                X_transf.title = self.title
-        # make coordset
-        M, N = X.shape
-        if X_transf.shape == X.shape and self.typex is None and self.typey is None:
-            X_transf.set_coordset(y=X.coord(0), x=X.coord(1))
+                # ensure that the first one
+                meta_from_tuple = (self.meta_from[0],)
         else:
-            if self.typey == "components":
-                X_transf.set_coordset(
-                    y=Coord(
-                        None,
-                        labels=["#%d" % (i + 1) for i in range(X_transf.shape[0])],
-                        title="components",
-                    ),
-                    x=X.coord(-1),
-                )
-            if self.typex == "components":
-                X_transf.set_coordset(
-                    y=X.coord(0),  # cannot use X.y in case of transposed X
-                    x=Coord(
-                        None,
-                        labels=["#%d" % (i + 1) for i in range(X_transf.shape[-1])],
-                        title="components",
-                    ),
-                )
-            if self.typex == "features":
-                X_transf.set_coordset(
-                    y=Coord(
-                        None,
-                        labels=["#%d" % (i + 1) for i in range(X_transf.shape[-1])],
-                        title="components",
-                    ),
-                    x=X.coord(1),
-                )
-            if self.typesingle == "components":
-                # occurs when the data are 1D such as ev_ratio...
-                X_transf.set_coordset(
-                    x=Coord(
-                        None,
-                        labels=["#%d" % (i + 1) for i in range(X_transf.shape[-1])],
-                        title="components",
-                    ),
-                )
+            data_tuple = output
+            meta_from_tuple = self.meta_from
 
-        # eventually restore masks
-        X_transf = obj._restore_masked_data(X_transf, axis=axis)
+        out = []
+        for data, meta_from in zip(data_tuple, meta_from_tuple):
+            X_transf = NDDataset(data)
+
+            # Now set the NDDataset attributes from the original X
+
+            # determine the input X dataset
+            X = getattr(obj, meta_from)
+
+            if self.units is not None:
+                if self.units == "keep":
+                    X_transf.units = X.units
+                else:
+                    X_transf.units = self.units
+            X_transf.name = f"{X.name}_{obj.name}.{self.method.__name__}"
+            X_transf.history = f"Created using method {obj.name}.{self.method.__name__}"
+            if self.title is not None:
+                if self.title == "keep":
+                    X_transf.title = X.title
+                else:
+                    X_transf.title = self.title
+            # make coordset
+            M, N = X.shape
+            if X_transf.shape == X.shape and self.typex is None and self.typey is None:
+                X_transf.set_coordset(y=X.coord(0), x=X.coord(1))
+            else:
+                if self.typey == "components":
+                    X_transf.set_coordset(
+                        y=Coord(
+                            None,
+                            labels=["#%d" % (i) for i in range(X_transf.shape[0])],
+                            title="components",
+                        ),
+                        x=X.coord(-1),
+                    )
+                if self.typex == "components":
+                    X_transf.set_coordset(
+                        y=X.coord(0),  # cannot use X.y in case of transposed X
+                        x=Coord(
+                            None,
+                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
+                            title="components",
+                        ),
+                    )
+                if self.typex == "features":
+                    X_transf.set_coordset(
+                        y=Coord(
+                            None,
+                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
+                            title="components",
+                        ),
+                        x=X.coord(1),
+                    )
+                if self.typesingle == "components":
+                    # occurs when the data are 1D such as ev_ratio...
+                    X_transf.set_coordset(
+                        x=Coord(
+                            None,
+                            labels=["#%d" % (i) for i in range(X_transf.shape[-1])],
+                            title="components",
+                        ),
+                    )
+                if self.typesingle == "targets":
+                    # occurs when the data are 1D such as PLSRegression intercept...
+                    if X.coordset[0].labels is not None:
+                        labels = X.coordset[0].labels
+                    else:
+                        labels = ["#%d" % (i + 1) for i in range(X.shape[-1])]
+                    X_transf.set_coordset(
+                        x=Coord(
+                            None,
+                            labels=labels,
+                            title="targets",
+                        ),
+                    )
+
+            # eventually restore masks
+            X_transf = obj._restore_masked_data(X_transf, axis=axis)
+            out.append(X_transf.squeeze())
 
-        return X_transf.squeeze()
+        if len(out) == 1:
+            return out[0]
+        else:
+            return tuple(out)
 
 
 def _wrap_ndarray_output_to_nddataset(
-    method=None, units="keep", title="keep", typex=None, typey=None, typesingle=None
+    method=None,
+    meta_from="_X",
+    units="keep",
+    title="keep",
+    typex=None,
+    typey=None,
+    typesingle=None,
 ):
     # wrap _set_output to allow for deferred calling
     if method:
         # case of the decorator without argument
         out = _set_output(method)
     else:
         # and with argument
         def wrapper(method):
             return _set_output(
                 method,
+                meta_from=meta_from,
                 units=units,
                 title=title,
                 typex=typex,
                 typey=typey,
                 typesingle=typesingle,
             )
 
@@ -199,43 +243,40 @@
 
 # ======================================================================================
 # Base class AnalysisConfigurable
 # ======================================================================================
 class AnalysisConfigurable(MetaConfigurable):
 
     __doc__ = _docstring.dedent(
-        """
+        r"""
     Abstract class to write analysis model estimators.
 
     Analysis model class must subclass this to get a minimal structure
 
     Parameters
     ----------
-    log_level : any of [ ``"INFO"`` , ``"DEBUG"`` , ``"WARNING"`` , ``"ERROR"`` ], optional, default: ``"WARNING"``
+    log_level : any of [``"INFO"``\ , ``"DEBUG"``\ , ``"WARNING"``\ , ``"ERROR"``\ ], optional, default: ``"WARNING"``
         The log level at startup.
-    warm_start : `bool`\ , optional, default:`False`
+    warm_start : `bool`\ , optional, default: `False`
         When fitting repeatedly on the same dataset, but for multiple
         parameter values (such as to find the value maximizing performance),
         it may be possible to reuse previous model learned from the previous parameter
         value, saving time.
 
         When `warm_start` is `True`\ , the existing fitted model attributes is used to
-        initialize the new model in a subsequent call to `fit`.
-    %(copy)s
+        initialize the new model in a subsequent call to `fit`\ .
     """
     )
 
     # Get doc sections for reuse in subclass
     _docstring.get_sections(__doc__, base="AnalysisConfigurable")
 
     # ----------------------------------------------------------------------------------
     # Runtime Parameters
     # ----------------------------------------------------------------------------------
-    _copy = tr.Bool(default_value=True, help="If True, input X data are copied")
-
     _fitted = tr.Bool(False, help="False if the model was not yet fitted")
     _masked_rc = tr.Tuple(allow_none=True, help="List of masked rows and columns")
     _X = NDDatasetType(allow_none=True, help="Data to fit a model")
     _X_mask = Array(allow_none=True, help="Mask information of the input X data")
     _X_preprocessed = Array(help="Preprocessed inital input X data")
     _X_shape = tr.Tuple(
         help="Original shape of the input X data, " "before any transformation"
@@ -261,15 +302,14 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level=logging.WARNING,
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
         """ """
         # An empty __doc__ is placed here, else Configurable.__doc__
         # will appear when there is no __init___.doc in subclass
 
         # Reset default configuration if not warm_start
@@ -306,30 +346,27 @@
         # If warm start we can use the previous fit as starting profiles.
         # so the flag _fitted is not set.
         if not warm_start:
             # We should not be able to use any methods requiring fit results
             # until the fit method has been executed
             self._fitted = False
 
-        # Copy passed data if required (True is the default)
-        self._copy = copy
-
     # ----------------------------------------------------------------------------------
     # Private methods
     # ----------------------------------------------------------------------------------
     def _make_dataset(self, d):
-        # Transform an array-like object to NDDataset (optionally copy data)
+        # Transform an array-like object to NDDataset
         # or a list of array-like to a list of NDQataset
         if d is None:
             return
         if isinstance(d, (tuple, list)):
             d = [self._make_dataset(item) for item in d]
         elif not isinstance(d, NDDataset):
-            d = NDDataset(d, copy=self._copy)
-        elif self._copy:
+            d = NDDataset(d, copy=True)
+        else:
             d = d.copy()
         return d
 
     def _get_masked_rc(self, mask):
         # Get the mask by row and columns.
         # -------------------------------
         # When a single element in the array is
@@ -350,15 +387,15 @@
         # doesn't support numpy masked arrays as input. So we will have to
         # remove the masked values ourselves
 
         # the following however assumes that entire rows or columns are masked,
         # not only some individual data (if this is what you wanted, this
         # will fail)
 
-        if not hasattr(X, "mask"):
+        if not hasattr(X, "mask") or not np.any(X._mask):
             return X
 
         # remove masked rows and columns
         masked_rows, masked_columns = self._get_masked_rc(X._mask)
 
         Xc = X[:, ~masked_columns]
         Xrc = Xc[~masked_rows]
@@ -458,15 +495,14 @@
     def _X_default(self):
         raise NotFittedError
 
     @tr.validate("_X")
     def _X_validate(self, proposal):
         # validation fired when self._X is assigned
         X = proposal.value
-
         # for the following we need X with two dimensions
         # So let's generate the un-squeezed X
         if X.ndim == 1:
             coordset = X.coordset
             X._data = X._data[np.newaxis]
             if np.any(X.mask):
                 X._mask = X._mask[np.newaxis]
@@ -508,24 +544,24 @@
         X = change.new
         # .... preprocessing as scaling, centering, ... must return a ndarray with
         #  same shape a X.data
 
         # Set a X.data by default
         self._X_preprocessed = X.data
 
-    def _fit(self, X, Y=None):
+    def _fit(self, X, Y=None):  # pragma: no cover
         #  Intended to be replaced in the subclasses by user defined function
         #  (with the same name)
         raise NotImplementedError("fit method has not yet been implemented")
 
     # ----------------------------------------------------------------------------------
     # Public methods and property
     # ----------------------------------------------------------------------------------
     def fit(self, X, Y=None):
-        """
+        r"""
         Fit the model with ``X`` as input dataset.
 
         Parameters
         ----------
         X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ )
             Training data.
         Y : any
@@ -541,15 +577,15 @@
         fit_transform :  Fit the model with an input dataset ``X`` and apply the dimensionality reduction on ``X``\ .
         fit_reduce : Alias of `fit_transform` (Deprecated).
         """
         self._fitted = False  # reinit this flag
 
         # fire the X and eventually Y validation and preprocessing.
         # X and Y are expected to be resp. NDDataset and NDDataset or list of NDDataset.
-        self._X = X  # self._make_dataset(X)
+        self._X = X
         if Y is not None:
             self._Y = Y
 
         # _X_preprocessed has been computed when X was set, as well as _Y_preprocessed.
         # At this stage they should be simple ndarrays
         newX = self._X_preprocessed
         newY = self._Y_preprocessed if Y is not None else None
@@ -657,17 +693,15 @@
     # Private validation and default getter methods
     # ----------------------------------------------------------------------------------
     @tr.validate("_Y")
     def _Y_validate(self, proposal):
         # validation of the _Y attribute: fired when self._Y is assigned
         Y = proposal.value
 
-        # we need a dataset or a list of NDDataset with eventually  a copy of the
-        # original data (default being to copy them)
-
+        # we need a dataset or a list of NDDataset
         Y = self._make_dataset(Y)
         return Y
 
     @property
     def _Y_is_missing(self):
         # check wether or not Y has been already defined
         try:
@@ -690,46 +724,46 @@
     def _preprocess_as_Y_changed(self, change):
         # to be optionally replaced by user defined function (with the same name)
         Y = change.new
         # optional preprocessing as scaling, centering, ...
         # return a np.ndarray
         self._Y_preprocessed = Y.data
 
-    def _transform(self, *args, **kwargs):
+    def _transform(self, *args, **kwargs):  # pragma:  no cover
         # to be overriden in subclass such as PCA, MCRALS, ...
         raise NotImplementedError("transform has not yet been implemented")
 
-    def _inverse_transform(self, *args, **kwargs):
+    def _inverse_transform(self, *args, **kwargs):  # pragma:  no cover
         # to be overriden in subclass such as PCA, MCRALS, ...
         raise NotImplementedError("inverse_transform has not yet been implemented")
 
-    def _get_components(self, n_components=None):
+    def _get_components(self, n_components=None):  # pragma:  no cover
         # to be overriden in subclass such as PCA, MCRALS, ...
         raise NotImplementedError("get_components has not yet been implemented")
 
     # ----------------------------------------------------------------------------------
     # Public methods
     # ----------------------------------------------------------------------------------
     @_wrap_ndarray_output_to_nddataset(units=None, title=None, typex="components")
     @_docstring.dedent
     def transform(self, X=None, **kwargs):
-        """
+        r"""
         Apply dimensionality reduction to `X`\ .
 
         Parameters
         ----------
         X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ ), optional
             New data, where :term:`n_observations` is the number of observations
             and :term:`n_features` is the number of features.
             if not provided, the input dataset of the `fit` method will be used.
         %(kwargs)s
 
         Returns
         -------
-        `~spectrochempy.core.dataset.nddataset.NDDataset`
+        `NDDataset`
             Dataset with shape (:term:`n_observations`\ , :term:`n_components`\ ).
 
         Other Parameters
         ----------------
         n_components : `int`, optional
             The number of components to use for the reduction. If not given
             the number of components is eventually the one specified or determined
@@ -768,15 +802,15 @@
         sections=["Parameters", "Other Parameters", "Returns"],
     )
     _docstring.keep_params("analysis_transform.parameters", "X")
 
     @_wrap_ndarray_output_to_nddataset
     @_docstring.dedent
     def inverse_transform(self, X_transform=None, **kwargs):
-        """
+        r"""
         Transform data back to its original space.
 
         In other words, return an input `X_original` whose reduce/transform would
         be `X_transform`.
 
         Parameters
         ----------
@@ -784,15 +818,15 @@
             Reduced `X` data, where `n_observations` is the number of observations
             and `n_components` is the number of components. If `X_transform` is not
             provided, a transform of `X` provided in `fit` is performed first.
         %(kwargs)s
 
         Returns
         -------
-        `~spectrochempy.core.dataset.nddataset.NDDataset`
+        `NDDataset`
             Dataset with shape (:term:`n_observations`\ , :term:`n_features`\ ).
 
         Other Parameters
         ----------------
         %(analysis_transform.other_parameters)s
 
         See Also
@@ -833,15 +867,15 @@
         base="analysis_inverse_transform",
         sections=["Parameters", "Returns"],
     )
     # _docstring.keep_params("analysis_inverse_transform.parameters", "X_transform")
 
     @_docstring.dedent
     def fit_transform(self, X, Y=None, **kwargs):
-        """
+        r"""
         Fit the model with `X` and apply the dimensionality reduction on `X`\ .
 
         Parameters
         ----------
         %(analysis_fit.parameters.X)s
         Y : any
             Depends on the model.
@@ -877,15 +911,15 @@
 
     reconstruct.__doc__ = (
         inverse_transform.__doc__ + "\nNotes\n-----\nDeprecated in version 0.6.\n"
     )
 
     @_wrap_ndarray_output_to_nddataset(units=None, title=None, typey="components")
     def get_components(self, n_components=None):
-        """
+        r"""
         Return the component's dataset: (selected :term:`n_components`\ , :term:`n_features`\ ).
 
         Parameters
         ----------
         n_components : `int`, optional, default: `None`
             The number of components to keep in the output dataset.
             If `None`, all calculated components are returned.
@@ -902,15 +936,15 @@
         components = self._get_components()[:n_components]
 
         return components
 
     @property
     @_wrap_ndarray_output_to_nddataset(units=None, title="keep", typey="components")
     def components(self):
-        """
+        r"""
         `NDDataset` with components in feature space (:term:`n_components`\ , :term:`n_features`\ ).
 
         See Also
         --------
         get_components : Retrieve only the specified number of components.
         """
         return self._get_components()
@@ -926,15 +960,15 @@
             raise NotFittedError("n_components")
 
     # ----------------------------------------------------------------------------------
     # Plot methods
     # ----------------------------------------------------------------------------------
     @_docstring.dedent
     def plotmerit(self, X=None, X_hat=None, **kwargs):
-        """
+        r"""
         Plot the input (:math:`X`\ ), reconstructed (:math:`\hat{X}`\ ) and residuals (:math:`E`\ ) datasets.
 
         :math:`X` and :math:`\hat{X}` can be passed as arguments. If not,
         the `X` attribute is used for :math:`X`\ and :math:`\hat{X}`\ is computed by
         the `inverse_transform` method
 
         Parameters
@@ -1028,26 +1062,467 @@
         ax.yaxis.set_visible(False)
         return ax
 
     _docstring.get_sections(_docstring.dedent(plotmerit.__doc__), base="plotmerit")
 
     @property
     def Y(self):
-        """
+        r"""
         The `Y` input.
         """
         # We use Y property only to show this information to the end-user. Internally
         # we use _Y attribute to refer to the input data
         if self._Y_is_missing:
             raise NotFittedError
         Y = self._Y
         return Y
 
 
 # ======================================================================================
+# Base class CrossDecompositionAnalysis
+# ======================================================================================
+class CrossDecompositionAnalysis(DecompositionAnalysis):
+    """
+    Abstract class to write analysis cross decomposition models such as `PLSRegression`, ...
+
+    Subclass this to get a minimal structure
+
+    See Also
+    --------
+    PLSRegression : Perform a Partial Least Square Regression .
+    """
+
+    # This class is a subclass of DecompositionAnalysis, so we define only additional
+    # attributes and methods necessary for cross decomposition model.
+
+    # Get doc sections for reuse in subclass
+    _docstring.get_sections(
+        _docstring.dedent(__doc__),
+        base="CrossDecompositionAnalysis",
+        sections=["See Also"],
+    )
+
+    # ----------------------------------------------------------------------------------
+    # Private methods that should be most of the time overloaded in subclass
+    # ----------------------------------------------------------------------------------
+    def _predict(self, *args, **kwargs):  # pragma:  no cover
+        # to be overriden in subclass such as PLSRegression, ...
+        raise NotImplementedError("predict has not yet been implemented")
+
+    # ----------------------------------------------------------------------------------
+    # Public methods
+    # ----------------------------------------------------------------------------------
+
+    @_wrap_ndarray_output_to_nddataset(meta_from="_Y", title=None)
+    @_docstring.dedent
+    def predict(self, X=None):
+        """
+        Predict targets of given observations.
+
+        Parameters
+        ----------
+        X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ ), optional
+            New data, where :term:`n_observations` is the number of observations
+            and :term:`n_features` is the number of features.
+            if not provided, the input dataset of the `fit` method will be used.
+
+        Returns
+        -------
+        `NDDataset`
+            Datasets with shape (:term:`n_observations`\ ,) or ( :term:`n_observations`\ , :term:`n_targets`\ ).
+        """
+        if not self._fitted:
+            raise NotFittedError()
+
+        if X is None:
+            X = self._X_preprocessed
+        elif isinstance(X, NDDataset):
+            X = X.data
+
+        return self._predict(X)
+
+    @_docstring.dedent
+    def score(self, X=None, Y=None, sample_weight=None):
+        r"""
+        Return the coefficient of determination of the prediction.
+
+        The coefficient of determination :math:`R^2` is defined as
+        :math:`(1 - \frac{u}{v})` , where :math:`u` is the residual
+        sum of squares ``((y_true - y_pred)** 2).sum()`` and :math:`v`
+        is the total sum of squares ``((y_true - y_true.mean()) ** 2).sum()``\ .
+        The best possible score is ``1.0`` and it can be negative (because the
+        model can be arbitrarily worse). A constant model that always predicts
+        the expected value of `Y`\ , disregarding the input features, would get
+        a :math:`R^2` score of 0.0.
+
+        Parameters
+        ----------
+        X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ ), optional
+            Test samples. If not given, the X attribute is used.
+        Y : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_targets`\ ), optional
+            True values for `X`.
+        sample_weight : `NDDataset` or :term:`array-like` of shape (:term:`n_samples`\ ,), default: `None`
+            Sample weights.
+
+        Returns
+        -------
+        `float`
+            :math:`R^2` of `predict`\ (X) w.r.t `Y`\ .
+        """
+        if not self._fitted:
+            raise NotFittedError()
+
+        if X is None:
+            X = self._X_preprocessed
+        elif isinstance(X, NDDataset):
+            X = X.data
+
+        if Y is None:
+            Y = self._Y_preprocessed
+        elif isinstance(Y, NDDataset):
+            Y = Y.data
+
+        if isinstance(sample_weight, NDDataset):
+            sample_weight = sample_weight.data
+
+        return self._score(X, Y, sample_weight)
+
+    @_wrap_ndarray_output_to_nddataset(
+        units=None, title=None, meta_from=("_X", "_Y"), typex="components"
+    )
+    @_docstring.dedent
+    def transform(self, X=None, Y=None, both=False, **kwargs):
+        r"""
+        Apply dimensionality reduction to `X`\ and `Y`\ .
+
+        Parameters
+        ----------
+        X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ ), optional
+            New data, where :term:`n_observations` is the number of observations
+            and :term:`n_features` is the number of features.
+            if not provided, the input dataset of the `fit` method will be used.
+        Y : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_targets`\ ), optional
+            New data, where :term:`n_targets` is the number of variables to predict.
+            if not provided, the input dataset of the `fit` method will be used.
+        both : `bool`, default: `False`
+            Whether to also apply the dimensionality reduction to Y when neither X nor Y are provided.
+        %(kwargs)s
+
+        Returns
+        -------
+        x_score, y_score: `NDDataset` or tuple of `NDDataset`
+            Datasets with shape (:term:`n_observations`\ , :term:`n_components`\ ).
+
+        """
+        if not self._fitted:
+            raise NotFittedError()
+
+        # Fire the validation and preprocessing
+        self._X = X if X is not None else self.X
+        self._Y = Y if Y is not None else self.Y
+
+        # Get the processed ndarray data
+        newX = self._X_preprocessed
+        newY = self._Y_preprocessed
+
+        if both or (Y is not None):
+            return self._transform(newX, newY)
+        else:
+            return self._transform(newX, None)
+
+    # Get doc sections for reuse in subclass
+    _docstring.get_sections(
+        _docstring.dedent(transform.__doc__),
+        base="cross_decomposition_transform",
+        sections=["Parameters", "Other Parameters", "Returns"],
+    )
+    _docstring.keep_params("cross_decomposition_transform.parameters", "X", "Y", "both")
+
+    @_wrap_ndarray_output_to_nddataset(meta_from=("_X", "_Y"))
+    @_docstring.dedent
+    def inverse_transform(
+        self, X_transform=None, Y_transform=None, both=False, **kwargs
+    ):
+        """
+        Transform data back to its original space.
+
+        In other words, return reconstructed `X` and `Y` whose reduce/transform would
+        be `X_transform` and `Y_transform`.
+
+        Parameters
+        ----------
+        X_transform : array-like of shape (:term:`n_observations`\ , :term:`n_components`\ ), optional
+            Reduced `X` data, where `n_observations` is the number of observations
+            and `n_components` is the number of components. If `X_transform` is not
+            provided, a transform of `X` provided in `fit` is performed first.
+        Y_transform : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , `n_components`\ ), optional
+            New data, where :term:`n_targets` is the number of variables to predict. If `Y_transform` is not
+            provided, a transform of `Y` provided in `fit` is performed first.
+        %(kwargs)s
+
+        Returns
+        -------
+        `NDDataset`
+            Dataset with shape (:term:`n_observations`\ , :term:`n_features`\ ).
+
+        Other Parameters
+        ----------------
+        %(analysis_transform.other_parameters)s
+
+        See Also
+        --------
+        reconstruct : Alias of inverse_transform (Deprecated).
+        """
+        if not self._fitted:
+            raise NotFittedError
+
+        if isinstance(X_transform, NDDataset):
+            X_transform = X_transform.data
+
+        elif X_transform is None:
+            X_transform = self.transform(**kwargs).data
+
+        if isinstance(Y_transform, NDDataset):
+            Y_transform = Y_transform.data
+
+        elif Y_transform is None and both is True:
+            Y_transform = self.transform(**kwargs).data
+
+        if Y_transform is None:
+            X = self._inverse_transform(X_transform)
+            return X
+        else:
+            X, Y = self._inverse_transform(X_transform, X_transform)
+            return X, Y
+
+    _docstring.get_sections(
+        _docstring.dedent(inverse_transform.__doc__),
+        base="analysis_inverse_transform",
+        sections=["Parameters", "Returns"],
+    )
+    # _docstring.keep_params("analysis_inverse_transform.parameters", "X_transform")
+
+    @_docstring.dedent
+    def fit_transform(self, X, Y, both=False):
+        """
+        Fit the model with `X` and `Y` and apply the dimensionality reduction on `X` and optionally on `Y`\ .
+
+        Parameters
+        ----------
+        %(analysis_fit.parameters.X)s
+        Y : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ , :term:`n_features`\ )
+            Training data.
+        both : `bool`\ , optional
+            Whether to apply the dimensionality reduction on `X` and `Y` .
+
+        Returns
+        -------
+        %(analysis_transform.returns)s
+        """
+
+        self.fit(X, Y)
+        if both:
+            return self.transform(X, Y)
+        else:
+            return self.transform(X)
+
+    # ----------------------------------------------------------------------------------
+    # Plot methods
+    # ----------------------------------------------------------------------------------
+    @_docstring.dedent
+    def parityplot(
+        self,
+        Y=None,
+        Y_hat=None,
+        clear=True,
+        **kwargs,
+    ):
+        r"""
+        Plot the predicted (:math:`\hat{Y}`\ ) vs measured (:math:`Y`\ ) values.
+
+        :math:`Y` and :math:`\hat{Y}` can be passed as arguments. If not,
+        the `Y` attribute is used for :math:`Y`\ and :math:`\hat{Y}`\ is computed by
+        the `inverse_transform` method.
+
+        Parameters
+        ----------
+        Y : `NDDataset`\ , optional
+            Measured values. If is not provided (default), the `Y`
+            attribute is used and Y_hat is computed using `inverse_transform`\ .
+        Y_hat : `NDDataset`\ , optional
+            Predicted values. if `Y` is provided, `Y_hat` must also be provided as
+            computed externally.
+        clear : `bool`\ , optional
+            Whether to plot on a new axes. Default is True.
+        %(kwargs)s
+
+        Returns
+        -------
+        `~matplotlib.axes.Axes`
+            Matplotlib subplot axe.
+
+        Other Parameters
+        ----------------
+        s : `float` or :term:`array-like`, shape (n, ), optional
+            The marker size in points**2 (typographic points are 1/72 in.).
+            Default is rcParams['lines.markersize'] ** 2.
+        c : :term:`array-like` or `list` of colors or color, optional
+            The marker colors. Possible values:
+
+            - A scalar or sequence of n numbers to be mapped to colors using cmap
+              and norm.
+            - A 2D array in which the rows are RGB or RGBA.
+            - A sequence of colors of length n.
+            - A single color format string.
+              see `~matplotlib.pyplot.scatter` for details.
+
+        marker : `markerMarkerStyle`, default: rcParams["scatter.marker"] (default: 'o')
+            The marker style. marker can be either an instance of the class or the text
+            shorthand for a particular marker. See `~matplotlib.markers` for more
+            information.
+        cmap : `str` or `Colormap`, default: rcParams["image.cmap"] (default: 'viridis')
+            The Colormap instance or registered colormap name used to map scalar data
+            to colors.
+            This parameter is ignored if c is RGB(A).
+        norm : `str` or Normalize, optional
+            The normalization method used to scale scalar data to the [0, 1] range
+            before mapping
+            to colors using cmap. By default, a linear scaling is used, mapping the
+            lowest value to
+            0 and the highest to 1.
+            If given, this can be one of the following:
+
+            - An instance of Normalize or one of its subclasses
+              (see Colormap Normalization).
+            - A scale name, i.e. one of "linear", "log", "symlog", "logit", etc.
+              For a list of available scales, call
+              matplotlib.scale.get_scale_names(). In that case, a suitable Normalize
+              subclass is dynamically generated
+              and instantiated.
+              This parameter is ignored if c is RGB(A).
+
+        vmin, vmax : `float`\ , optional
+            When using scalar data and no explicit norm, vmin and vmax define the data
+            range that the colormap covers.
+            By default, the colormap covers the complete value range of the supplied
+            data. It is an error to use
+            vmin/vmax when a norm instance is given (but using a str norm name together
+            with vmin/vmax is acceptable).
+            This parameter is ignored if c is RGB(A).
+        alpha : `float`\ , default: 0.5
+            The alpha blending value, between 0 (transparent) and 1 (opaque).
+        linewidths : `float` or array-like, default: rcParams["lines.linewidth"] (default: 1.5)
+            The linewidth of the marker edges. Note: The default edgecolors is 'face'.
+            You may want to change this as well.
+        edgecolors : {'face', 'none', None} or color or sequence of color, default: rcParams["scatter.edgecolors"], (default: 'face')
+            The edge color of the marker. Possible values:
+            'face': The edge color will always be the same as the face color.
+            'none': No patch boundary will be drawn.
+            A color or sequence of colors.
+            For non-filled markers, edgecolors is ignored. Instead, the color is
+            determined like with 'face',
+            i.e. from c, colors, or facecolors.
+        plotnonfinite : `bool`\ , default: False
+            Whether to plot points with nonfinite c (i.e. inf, -inf or nan).
+            If True the points are drawn with the bad
+            colormap color (see Colormap.set_bad).
+        """
+
+        s = kwargs.pop("s", None)
+        c = kwargs.pop("c", None)
+        marker = kwargs.pop("marker", None)
+        cmap = kwargs.pop("cmap", None)
+        norm = kwargs.pop("norm", None)
+        vmin = kwargs.pop("vmin", None)
+        vmax = kwargs.pop("vmax", None)
+        alpha = kwargs.pop("alpha", 0.5)
+        linewidths = kwargs.pop("linewidths", None)
+        edgecolors = kwargs.pop("edgecolors", None)
+        plotnonfinite = kwargs.pop("plotnonfinite", False)
+        data = kwargs.pop("data", None)
+
+        if Y is None:
+            Y = self.Y
+            if Y_hat is None:
+                # compute the inverse transform (this check that the model
+                # is already fitted and handle eventual masking)
+                Y_hat = self.predict(self.X)
+        elif Y_hat is None:
+            raise ValueError(
+                "If Y is provided, An externally computed Y_hat dataset "
+                "must be also provided."
+            )
+
+        if Y._squeeze_ndim == 1:
+            # normally this was done before, but if needed.
+            Y = Y.squeeze()
+            Y_hat = Y_hat.squeeze()
+
+        plt.style.use(["default"])
+        plt.rcParams.update({"font.size": 14})
+        if clear:
+            fig = plt.figure()
+            ax = fig.add_subplot(111)
+        else:
+            ax = plt.gca()
+        if len(Y.shape) == 1:
+            plt.scatter(
+                Y.data,
+                Y_hat.data,
+                s=s,
+                c=c,
+                marker=marker,
+                cmap=cmap,
+                norm=norm,
+                vmin=vmin,
+                vmax=vmax,
+                alpha=alpha,
+                linewidths=linewidths,
+                edgecolors=edgecolors,
+                plotnonfinite=plotnonfinite,
+                data=data,
+                **kwargs,
+            )
+        else:
+            for col in Y.shape[1]:
+                plt.scatter(
+                    Y.data[:, col],
+                    Y_hat.data[:, col],
+                    s=s,
+                    c=c,
+                    marker=marker,
+                    cmap=cmap,
+                    norm=norm,
+                    vmin=vmin,
+                    vmax=vmax,
+                    alpha=alpha,
+                    linewidths=linewidths,
+                    edgecolors=edgecolors,
+                    plotnonfinite=plotnonfinite,
+                    data=data,
+                    **kwargs,
+                )
+        xmin, xmax = ax.get_xlim()
+        ymin, ymax = ax.get_ylim()
+        xymin = min(xmin, ymin)
+        xymax = max(xmax, ymax)
+        ax.set_xlim(xymin, xymax)
+        ax.set_ylim(xymin, xymax)
+        plt.plot([xymin, xymax], [xymin, xymax])
+        plt.legend()
+        plt.xlabel("measured values")
+        plt.ylabel("predicted values")
+        plt.tight_layout()
+
+        return ax
+
+    _docstring.get_sections(_docstring.dedent(parityplot.__doc__), base="parityplot")
+
+
+# ======================================================================================
 # Base class LinearRegressionAnalysis
 # ======================================================================================
 class LinearRegressionAnalysis(AnalysisConfigurable):
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters (mostly defined in subclass
     # as they depend on the model estimator)
@@ -1057,15 +1532,16 @@
         help="Whether to calculate the `intercept` for this model. If set to `False`, "
         "no `intercept` will be used in calculations (*i.e.,* data is expected to be "
         "centered).",
     ).tag(config=True)
 
     positive = tr.Bool(
         default_value=False,
-        help="When set to `True` , forces the coefficients (\ `coef`\ ) to be positive.",
+        help=r"When set to `True` , forces the coefficients (\ `coef`\ ) "
+        r"to be positive.",
     ).tag(config=True)
 
     # ----------------------------------------------------------------------------------
     # Runtime Parameters (in addition to those of AnalysisConfigurable)
     # ----------------------------------------------------------------------------------
     _Y = NDDatasetType()
     _Y_preprocessed = Array(help="preprocessed Y")
@@ -1074,31 +1550,28 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
         # initialize sklearn LinearRegression
         self._linear_regression = linear_model.LinearRegression(
             fit_intercept=self.fit_intercept,
-            copy_X=copy,
             n_jobs=None,  # not used for the moment (XXX: should we add this?)
             positive=self.positive,
         )
 
         # unlike decomposition methods, we output ndarray when the input
         # is not a dataset
         self._output_type = "ndarray"
@@ -1107,17 +1580,15 @@
     # Private validation and default getter methods
     # ----------------------------------------------------------------------------------
     @tr.validate("_Y")
     def _Y_validate(self, proposal):
         # validation of the _Y attribute: fired when self._Y is assigned
         Y = proposal.value
 
-        # we need a dataset or a list of NDDataset with eventually  a copy of the
-        # original data (default being to copy them)
-
+        # we need a dataset or a list of NDDataset
         Y = self._make_dataset(Y)
         return Y
 
     @property
     def _Y_is_missing(self):
         # check wether or not Y has been already defined
         try:
@@ -1143,15 +1614,15 @@
         _outfit = self._linear_regression.fit(X, Y, sample_weight=sample_weight)
         return _outfit
 
     # ----------------------------------------------------------------------------------
     # Public methods
     # ----------------------------------------------------------------------------------
     def fit(self, X, Y=None, sample_weight=None):
-        """
+        r"""
         Fit linear model.
 
         Parameters
         ----------
         X : `NDDataset` or :term:`array-like` of shape (:term:`n_observations`\ ,:term:`n_features`\ )
             Training data, where `n_observations` is the number of observations
             and `n_features` is the number of features.
@@ -1229,15 +1700,15 @@
         if self._is_dataset or self._output_type == "NDDataset":
             return Y
         else:
             return np.asarray(Y)
 
     @property
     def coef(self):
-        """
+        r"""
         Estimated coefficients for the linear regression problem.
 
         If multiple targets are passed during the fit (Y 2D), this is a 2D array of
         shape (:term:`n_targets`\ , :term:`n_features`\ ), while if only one target
         is passed, this is a 1D array of length :term:`n_features`\ .
         """
         if self._linear_regression.coef_.size == 1:
@@ -1263,15 +1734,15 @@
                 title=f"{self._Y.title} / {self._X.title}",
                 history="Computed from the LSTSQ model",
             )
         return A
 
     @property
     def intercept(self):
-        """
+        r"""
         Return a float or an array of shape (:term:`n_targets`\ ,).
 
         Independent term in the linear model. Set to ``0.0`` if `fit_intercept` is `False`.
         If `Y` has units, then `intercept` has the same units.
         """
         if self._linear_regression.intercept_.size == 1:
             # A single value, return the associated quantity
@@ -1287,15 +1758,15 @@
                 units=self._Y.units,
                 title=f"{self._Y.title} at origin",
                 history="Computed from the LSTSQ model",
             )
         return B
 
     def predict(self, X=None):
-        """
+        r"""
         Predict features using the linear model.
 
         Parameters
         ----------
         X : `NDDataset` or :term:`array-like` matrix, shape (:term:`n_observations`\ ,:term:`n_features`\ )
             Observations. If `X` is not set, the input `X` for `fit` is used.
 
@@ -1326,19 +1797,19 @@
                 title=self._Y.title,
                 history="Computed from a LSTSQ model",
             )
 
         return predicted
 
     def score(self, X=None, Y=None, sample_weight=None):
-        """
+        r"""
         Return the coefficient of determination of the prediction.
 
         The coefficient of determination :math:`R^2` is defined as
-        :math:`(1 - \\frac{u}{v})` , where :math:`u` is the residual
+        :math:`(1 - \frac{u}{v})` , where :math:`u` is the residual
         sum of squares ``((y_true - y_pred)** 2).sum()`` and :math:`v`
         is the total sum of squares ``((y_true - y_true.mean()) ** 2).sum()`` .
         The best possible score is ``1.0`` and it can be negative (because the
         model can be arbitrarily worse). A constant model that always predicts
         the expected value of `Y`\ , disregarding the input features, would get
         a :math:`R^2` score of 0.0.
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/api.py` & `spectrochempy-0.6.2/spectrochempy/analysis/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/efa.py` & `spectrochempy-0.6.2/spectrochempy/analysis/efa.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 import traitlets as tr
 
 from spectrochempy.analysis._base import (
     DecompositionAnalysis,
     _wrap_ndarray_output_to_nddataset,
 )
 from spectrochempy.core import info_
-from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["EFA"]
 __configurables__ = ["EFA"]
 
 
 @signature_has_configurable_traits
 class EFA(DecompositionAnalysis):
 
     _docstring.delete_params("DecompositionAnalysis.see_also", "EFA")
 
     __doc__ = _docstring.dedent(
-        """
+        r"""
     Evolving Factor Analysis (EFA).
 
-    Evolving factor analysis (`EFA`) is a method that allows model-free resolution of
+    Evolving factor analysis (`EFA`\ ) is a method that allows model-free resolution of
     overlapping peaks into concentration profiles and normalized spectra of components.
 
-    Originally developed for GC and GC-MS experiments (See e.g.,
+    Originally developed for GC and GC-MS experiments (See *e.g.,*
     :cite:t:`maeder:1986` , :cite:t:`roach:1992`\ ), it is also suitable for
     analysis spectra such as those obtained by Operando FTIR for example.
 
     The model used in this class allow to perform a forward and reverse analysis of the
     input `NDDataset` .
 
     Parameters
@@ -54,15 +54,15 @@
     >>> # Init the model
     >>> model = scp.EFA()
     >>> # Read an experimental 2D spectra (N x M )
     >>> X = scp.read("irdata/nh4y-activation.spg")
     >>> # Fit the model
     >>> _ = model.fit(X)
     >>> # Display components spectra (2 x M)
-    >>> model.used_components = 2
+    >>> model.n_components = 2
     >>> _ = model.components.plot(title="Component spectra")
     >>> # Get the abstract concentration profile based on the FIFO EFA analysis
     >>> c = model.transform()
     >>> # Plot the transposed concentration matrix  (2 x N)
     >>> _ = c.T.plot(title="Concentration")
     >>> scp.show()
     """
@@ -72,46 +72,39 @@
     # Configuration parameters (mostly defined in subclass
     # as they depend on the model estimator)
     # ----------------------------------------------------------------------------------
     cutoff = tr.Float(default_value=None, allow_none=True, help="Cut-off value.").tag(
         config=True
     )
 
-    used_components = tr.Int(
+    n_components = tr.Int(
         allow_none=True, default_value=None, help="Number of components to keep."
     ).tag(config=True)
 
     # ----------------------------------------------------------------------------------
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
-        # We have changed the name n_components use in sklearn by
-        # used_components (in order  to avoid conflict with the rest of the program)
-        # warn th user:
-        if "n_components" in kwargs:
-            raise KeyError(
-                "`n_components` is not a valid parameter. Did-you mean "
-                "`used_components`?"
-            )
 
         # Call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
+        if "used_components" in kwargs:
+            deprecated("used_components", replace="n_components", removed="0.6.5")
+            kwargs["n_components"] = kwargs.pop("used_components")
 
     def _fit(self, X, Y=None):
         # X has already been validated and eventually
         # preprocessed. X is now a nd-array with masked elements removed.
         # and this method should return _outfit
         # Y is not used but necessary to fit the superclass
 
@@ -156,16 +149,16 @@
         # Return concentration profile
         return self._get_conc()
 
     def _get_conc(self):
         f, b = self._outfit
         M = f.shape[0]
         K = self._n_components
-        if self.used_components is not None:
-            K = min(K, self.used_components)
+        if self.n_components is not None:
+            K = min(K, self.n_components)
         c = np.zeros((M, K))
         for i in range(M):
             c[i] = np.min((f[i, :K], b[i, :K][::-1]), axis=0)
         return c
 
     def _get_components(self):
         # compute the components from the original dataset and the EFA concentrations
@@ -237,12 +230,7 @@
         """
         Eigenvalues for the backward analysis ( `NDDataset` ).
         """
         b = self._outfit[1]
         if self.cutoff is not None:
             b = np.max((b, np.ones_like(b) * self.cutoff), axis=0)
         return b
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/iris.py` & `spectrochempy-0.6.2/spectrochempy/analysis/iris.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,23 +334,14 @@
     Parameters
     ----------
     %(AnalysisConfigurable.parameters)s
 
     See Also
     --------
     %(DecompositionAnalysis.see_also.no_IRIS)s
-
-    Examples
-    --------
-    >>> X = scp.read("irdata/CO@Mo_Al2O3.SPG")
-    >>> p = [0.003, 0.004, 0.009, 0.014, 0.021, 0.026, 0.036, 0.051, 0.093, 0.150,
-    ...      0.203, 0.300, 0.404, 0.503, 0.602, 0.702, 0.801, 0.905, 1.004]
-    >>> iris = scp.IRIS(X[:,2250.0:1960.0], "langmuir", q = [-8, -1, 10])
-    >>> iris.f
-    NDDataset: [float64] unitless (shape: (z:1, y:10, x:301))
     """
     )
 
     # ----------------------------------------------------------------------------------
     # Runtime Parameters (in addition to those of AnalysisConfigurable)
     # ----------------------------------------------------------------------------------
     _Y = tr.Union(
@@ -385,23 +376,21 @@
     # ----------------------------------------------------------------------------------
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
         # no validation of reg_par triggred when it is None
         # so we need to init self._lambdas manually else itt will not be inited
         if self.reg_par is None:
             self._lambdas = Coord([0], title="lambda")
 
@@ -808,22 +797,22 @@
         Parameters
         ----------
         index : `int`\ , `list` or `tuple` of `int`\ , optional, default: `None`
             Index(es) of the inversions (*i.e.,* of the lambda values) to consider.
             If `None` plots for all indices.
         %(kwargs)s
 
-        Other Parameters
-        ----------------
-        %(plotmerit.other_parameters)s
-
         Returns
         -------
         `list` of `~matplotlib.axes.Axes`
             Subplots.
+
+        Other Parameters
+        ----------------
+        %(plotmerit.other_parameters)s
         """
         X = self.X
         X_hat = self.inverse_transform()
         axeslist = []
         if index is None:
             index = range(len(self._lambdas))
         if type(index) is int:
@@ -984,12 +973,7 @@
     """
 
     try:
         _ = np.linalg.cholesky(B)
         return True
     except np.linalg.LinAlgError:
         return False
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/kinetic_utilities.py` & `spectrochempy-0.6.2/spectrochempy/analysis/kinetic_utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
         This function computes and integrates the set of kinetic differential
         equations given the initial concentration values:
 
         .. math::
             dC / dt =  (B - A).T  K C^A
 
-            C(t0) = C0
+            C(t_0) = C_0
 
         where :math:`A` and :math:`B` are the stoichiometry matrices,
         :math:`K` is the diagonal matrix of rate constants and :math:`C^A` is the
         vector-matrix exponentiation of :math:`C` by :math:`A`\ .
 
         Parameters
         ----------
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/linearregression.py` & `spectrochempy-0.6.2/spectrochempy/analysis/linearregression.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/mcrals.py` & `spectrochempy-0.6.2/spectrochempy/analysis/mcrals.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         0.1,
         help=(
             "Convergence criterion on the change of residuals (percent change of "
             "standard deviation of residuals)."
         ),
     ).tag(config=True)
 
-    max_iter = tr.Integer(50, help="Maximum number of :term:`ALS` iteration").tag(
+    max_iter = tr.Integer(50, help="Maximum number of :term:`ALS` iteration.").tag(
         config=True
     )
 
     maxdiv = tr.Integer(
         5, help="Maximum number of successive non-converging iterations."
     ).tag(config=True)
 
@@ -362,15 +362,14 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *args,
         log_level=logging.WARNING,
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
         if len(args) > 0:
             raise ValueError(
                 "Passing arguments such as MCRALS(X , profile) "
                 "is now deprecated. "
                 "Instead, use MCRAL() followed by MCRALS.fit(X , profile). "
@@ -399,15 +398,14 @@
             deprecated("unimodMod", replace="unimodConcMod", removed="0.6.5")
             kwargs["unimodConcMod"] = kwargs.pop("unimodMod")
 
         # call the super class for initialisation
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
         # deal with the callable that may have been serialized
         if self.getConc is not None and isinstance(self.getConc, str):
             self.getConc = dill.loads(base64.b64decode(self.getConc))
         if self.getSpec is not None and isinstance(self.getSpec, str):
@@ -980,22 +978,22 @@
 
         In other words, return an input `X_original` whose reduce/transform would be X.
 
         Parameters
         ----------
         %(analysis_inverse_transform.parameters)s
 
+        Returns
+        -------
+        `NDDataset`
+            Dataset with shape (:term:`n_observations`\ , :term:`n_features`\ ).
+
         Other Parameters
         ----------------
         %(analysis_transform.other_parameters)s
-
-        Returns
-        -------
-        `~spectrochempy.core.dataset.nddataset.NDDataset`
-            Dataset with shape (:term:`n_observations`\ , :term:`n_features`\ )
         """
         return super().inverse_transform(X_transform, **kwargs)
 
     @property
     def C(self):
         """
         The final concentration profiles.
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/nnmf.py` & `spectrochempy-0.6.2/spectrochempy/analysis/nnmf.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import logging
 
 import traitlets as tr
 from numpy.random import RandomState
 from sklearn import decomposition
 
 from spectrochempy.analysis._base import DecompositionAnalysis
-from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 
 __all__ = ["NMF"]
 __configurables__ = ["NMF"]
 
 
 # ======================================================================================
@@ -59,15 +59,15 @@
         help="The instance of sklearn.decomposition.NMF used in this model",
     )
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # ----------------------------------------------------------------------------------
 
-    used_components = tr.Integer(
+    n_components = tr.Integer(
         default_value=None,
         allow_none=True,
         help="Number of components to use. If None is passed, all are used.",
     ).tag(config=True)
 
     init = tr.Enum(
         ["random", "nndsvd", "nndsvda", "nndsvdar", "custom"],
@@ -168,38 +168,31 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
-        # we have changed the name n_components use in sklearn by
-        # used_components (in order  to avoid conflict with the rest of the program)
-        # warn th user:
-        if "n_components" in kwargs:
-            raise KeyError(
-                "`n_components` is not a valid parameter. Did-you mean "
-                "`used_components`?"
-            )
+        if "used_components" in kwargs:
+            deprecated("used_components", replace="n_components", removed="0.6.5")
+            kwargs["n_components"] = kwargs.pop("used_components")
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
         # initialize sklearn NMF
         self._nmf = decomposition.NMF(
-            n_components=self.used_components,
+            n_components=self.n_components,
             init=self.init,
             beta_loss=self.beta_loss,
             tol=self.tol,
             max_iter=self.max_iter,
             random_state=self.random_state,
             alpha_W=self.alpha_W,
             alpha_H=self.alpha_H,
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/optimize/__init__.py` & `spectrochempy-0.6.2/spectrochempy/analysis/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/optimize/_models.py` & `spectrochempy-0.6.2/spectrochempy/analysis/optimize/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,22 @@
 #          #
 ############
 
 # ======================================================================================
 # PolynomialBaseline
 # ======================================================================================
 class polynomialbaseline(object):
-    """
+    r"""
     Arbitrary-degree polynomial (degree limited to 10, however).
 
     As a linear baseline is automatically calculated, this polynom is always of
     greater or equal to order 2 (parabolic function).
 
     .. math::
-        f(x) = ampl * \\sum_{i=2}^{max} c_i*x^i
+        f(x) = ampl * \sum_{i=2}^{max} c_i*x^i
     """
 
     type = "1D"
     args = ["ampl"]
     args.extend(["c_%d" % i for i in range(2, 11)])
 
     script = """
@@ -136,19 +136,19 @@
         return ampl * np.polyval(np.array(tuple(c))[::-1], x - x[int(x.size / 2)])
 
 
 # #===============================================================================
 # # Gaussian2DModel
 # #===============================================================================
 # class gaussian2dmodel(object):
-#    """
+#    r"""
 #    Two dimensional Gaussian model (*not* normalized - peak value is 1).
 #
 #    .. math::
-#        A e^{\\frac{-(x-\\iso_x)^2}{2 \\gb_x^2}} e^{\\frac{-(y-\\iso_y)^2}{2 \\gb_y^2}}
+#        A e^{\frac{-(x-\iso_x)^2}{2 \gb_x^2}} e^{\frac{-(y-\iso_y)^2}{2 \gb_y^2}}
 #
 #    """
 #    args = ['amp','gbx','gby','posx','posy']
 #    def f(self, xy, amp, gbx, gby, posx, posy, **kargs):
 #        gbx = float(gbx)
 #        gby = float(gby)
 #        x,y = xy
@@ -323,11 +323,7 @@
 
     """
 
     @make_units_compatibility
     def f(self, x, ampl, pos, asym, **kargs):
         w = 1.0 / (1.0 + np.exp(asym * (x - pos) / ampl))
         return ampl * w
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/optimize/_parameters.py` & `spectrochempy-0.6.2/spectrochempy/analysis/optimize/_parameters.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/optimize/optimize.py` & `spectrochempy-0.6.2/spectrochempy/analysis/optimize/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,26 +105,24 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
         """ """
         # An empty __doc__ must be placed here, else Configurable.__doc__ will appear
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
     # ----------------------------------------------------------------------------------
     # Private methods ( overriding abstract methods)
     # ----------------------------------------------------------------------------------
     def _fit(self, X, Y=None):
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/pca.py` & `spectrochempy-0.6.2/spectrochempy/analysis/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sklearn import decomposition
 
 from spectrochempy.analysis._base import (
     DecompositionAnalysis,
     NotFittedError,
     _wrap_ndarray_output_to_nddataset,
 )
-from spectrochempy.utils.decorators import signature_has_configurable_traits
+from spectrochempy.utils.decorators import deprecated, signature_has_configurable_traits
 from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.plots import NBlue, NRed
 
 __all__ = ["PCA"]
 __configurables__ = ["PCA"]
 
 
@@ -63,43 +63,43 @@
 
     # ----------------------------------------------------------------------------------
     # Configuration parameters
     # ----------------------------------------------------------------------------------
     # sklearn PCA is always on centered data
     standardized = tr.Bool(
         default_value=False,
-        help="If True the data are scaled to unit standard deviation: "
-        ":math:`X' = X / \\sigma`",
+        help=r"If True the data are scaled to unit standard deviation: "
+        ":math:`X' = X / \sigma`\ .",
     ).tag(config=True)
 
     scaled = tr.Bool(
         default_value=False,
-        help="If True the data are scaled in the interval ``[0-1]`` : "
-        ":math:`X' = (X - min(X)) / (max(X)-min(X))``",
+        help="If True the data are scaled in the interval ``[0-1]``\ : "
+        ":math:`X' = (X - min(X)) / (max(X)-min(X))`\ .",
     ).tag(config=True)
 
-    used_components = tr.Union(
+    n_components = tr.Union(
         (tr.Enum(["mle"]), tr.Int(), tr.Float()),
         allow_none=True,
         default_value=None,
         help="""Number of components to keep.
-if `used_components` is not set all components are kept::
+if `n_components` is not set all components are kept::
 
-    used_components == min(n_observations, n_features)
+    n_components == min(n_observations, n_features)
 
-If ``used_components == 'mle'`` and ``svd_solver == 'full'`` , Minka's MLE is used to guess
-the dimension. Use of ``used_components == 'mle'`` will interpret `svd_solver == 'auto'`
+If ``n_components == 'mle'`` and ``svd_solver == 'full'`` , Minka's MLE is used to guess
+the dimension. Use of ``n_components == 'mle'`` will interpret `svd_solver == 'auto'`
 as ``svd_solver == 'full'`` .
-If `0 < used_components < 1` and `svd_solver == 'full'` , select the number of
+If `0 < n_components < 1` and `svd_solver == 'full'` , select the number of
 components such that the amount of variance that needs to be explained is greater than
-the percentage specified by used_components.
+the percentage specified by n_components.
 If `svd_solver == 'arpack'` , the number of components must be strictly less than the
 minimum of n_features and n_observations. Hence, the None case results in::
 
-    used_components == min(n_observations, n_features) - 1""",
+    n_components == min(n_observations, n_features) - 1.""",
     ).tag(config=True)
 
     whiten = tr.Bool(
         default_value=False,
         help="""When True (False by default) the `components_` vectors are multiplied
 by the square root of n_observations and then divided by the singular values to ensure
 uncorrelated outputs with unit component-wise variances. Whitening will remove some
@@ -109,24 +109,24 @@
     ).tag(config=True)
 
     svd_solver = tr.Enum(
         ["auto", "full", "arpack", "randomized"],
         default_value="auto",
         help="""If auto :
 The solver is selected by a default policy based on `X.shape`
-and `used_components`: if the input data is larger than 500x500 and the number of
+and `n_components`: if the input data is larger than 500x500 and the number of
 components to extract is lower than 80% of the smallest dimension of the data, then the
 more efficient 'randomized' method is enabled. Otherwise the exact full SVD is computed
 and optionally truncated afterwards.
 If full :
 run exact full SVD calling the standard LAPACK solver via `scipy.linalg.svd` and select
 the components by postprocessing
 If arpack :
-run SVD truncated to used_components calling ARPACK solver via `scipy.sparse.linalg.svds` .
-It requires strictly 0 < used_components < min(X.shape)
+run SVD truncated to n_components calling ARPACK solver via `scipy.sparse.linalg.svds` .
+It requires strictly 0 < n_components < min(X.shape)
 If randomized :
 run randomized SVD by the method of Halko et al.""",
     ).tag(config=True)
 
     tol = tr.Float(
         default_value=0.0,
         help="""Tolerance for singular values computed by svd_solver == 'arpack'.
@@ -167,40 +167,32 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
-        # we have changed the name n_components use in sklearn by
-        # used_components (in order  to avoid conflict with the rest of the program)
-        # warn th user:
-        if "n_components" in kwargs:
-            raise KeyError(
-                "`n_components` is not a valid parameter. Did-you mean "
-                "`used_components`?"
-            )
+        if "used_components" in kwargs:
+            deprecated("used_components", replace="n_components", removed="0.6.5")
+            kwargs["n_components"] = kwargs.pop("used_components")
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
         # initialize sklearn PCA
         self._pca = decomposition.PCA(
-            n_components=self.used_components,
+            n_components=self.n_components,
             whiten=self.whiten,
-            copy=copy,
             svd_solver=self.svd_solver,
             tol=self.tol,
             iterated_power=self.iterated_power,
             n_oversamples=self.n_oversamples,
             power_iteration_normalizer=self.power_iteration_normalizer,
             random_state=self.random_state,
         )
@@ -227,29 +219,29 @@
             self._ampl = X.ptp(dim=0)
             X -= self._min
             X /= self._ampl
             X.name = "scaled %s" % X.name
 
         self._X_preprocessed = X.data
 
-        # final check on the configuration used_components parameter
+        # final check on the configuration n_components parameter
         # (which can be done only when X is defined in fit arguments)
         n_observations, n_features = X.shape
 
-        n_components = self.used_components
+        n_components = self.n_components
         if n_components is None:
             pass
         elif n_components == "mle":
             if n_observations < n_features:
                 raise ValueError(
-                    "used_components='mle' is only supported if n_observations >= n_features"
+                    "n_components='mle' is only supported if n_observations >= n_features"
                 )
         elif not 0 <= n_components <= min(n_observations, n_features):
             raise ValueError(
-                "used_components=%r must be between 0 and "
+                "n_components=%r must be between 0 and "
                 "min(n_observations, n_features)=%r with "
                 "svd_solver='full'" % (n_components, min(n_observations, n_features))
             )
 
     def _fit(self, X, Y=None):
         # this method is called by the abstract class fit.
         # Input X is a np.ndarray
@@ -274,14 +266,15 @@
         # eventually calculated ones: this will simplify further process
         # indeed in sklearn, the value after processing is n_components_
         # with an underscore at the end
 
         self._n_components = int(
             self._pca.n_components_
         )  # cast the returned int64 to int
+        self.n_components = self._n_components
         return _outfit
 
     def _transform(self, X):
         return self._pca.transform(X)
 
     def _inverse_transform(self, X_transform):
         # we need to  set self._pca.components_ to a compatible size but without
@@ -393,15 +386,15 @@
         """
         Print PCA figures of merit.
 
         Prints eigenvalues and explained variance for all or first n_pc PC's.
 
         Parameters
         ----------
-        n_pc : int, optional
+        n_components : int, optional
             The number of components to print.
         """
         if not self._fitted:
             raise NotFittedError(
                 "The fit method must be used " "before using this method"
             )
 
@@ -487,20 +480,20 @@
             used for color mapping.
         show_labels : bool, optional, default: False
             If True each observation will be annotated with its label.
         labels_column : int, optional, default:0
             If several columns of labels are present indicates which column has to be
             used to show labels.
         labels_every : int, optional, default: 1
-        `   Do not label all points, but only every value indicated by this parameter.
+            Do not label all points, but only every value indicated by this parameter.
 
         Returns
         -------
         `~matplotlib.axes.Axes`
-            The axes
+            The matplotlib axes.
         """
         self.prefs = self.X.preferences
 
         # checks args
         if len(args) > 0:
             scores = args[0]
             if hasattr(scores, "_implements") and scores._implements("NDDataset"):
@@ -617,11 +610,7 @@
                 i = labels.index(lab)
                 c = axsc.get_cmap().colors[int(255 / (len(labels) - 1) * i)]
                 leg.append(mpatches.Patch(color=c, label=lab))
 
             ax.legend(handles=leg, loc="best")
 
         return ax
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/peakfinding.py` & `spectrochempy-0.6.2/spectrochempy/analysis/peakfinding.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/readme.rst` & `spectrochempy-0.6.2/spectrochempy/analysis/readme.rst`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/simplisma.py` & `spectrochempy-0.6.2/spectrochempy/analysis/simplisma.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,45 +60,44 @@
     # They will be written in a file from which the default can be modified)
     # Obviously, the parameters can also be modified at runtime as usual by assignment.
     # ----------------------------------------------------------------------------------
     interactive = tr.Bool(
         default_value=False,
         help=(
             "If True, the determination of purest variables is carried out "
-            "interactively"
+            "interactively."
         ),
     ).tag(config=True)
     max_components = tr.Integer(
         default_value=2,
         help=(
             "The maximum number of pure compounds. Used only for non interactive"
-            "analysis"
+            "analysis."
         ),
     ).tag(config=True)
     tol = tr.Float(
         default_value=0.1,
         help="The convergence criterion on the percent of unexplained variance.",
     ).tag(config=True)
     noise = tr.Float(
         default_value=3,
         help=(
             "A correction factor (%) for low intensity variables (0 - no offset, "
-            "15 - large offset"
+            "15 - large offset."
         ),
     ).tag(config=True)
 
     # ----------------------------------------------------------------------------------
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *args,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
         if len(args) > 0:
             raise ValueError(
                 "Passing arguments such as SIMPLISMA(X) is now deprecated. "
                 "Instead, use SIMPLISMA() followed by SIMPLISMA.fit(X). "
                 "See the documentation and exemples"
@@ -117,15 +116,14 @@
             deprecated("n_pc", replace="max_components", removed="0.6.5")
             kwargs["max_components"] = kwargs.pop("n_pc")
 
         # call the super class for initialisation
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
     # ----------------------------------------------------------------------------------
     # Private validation methods and default getter
     # ----------------------------------------------------------------------------------
     @tr.validate("max_components")
@@ -554,12 +552,7 @@
         Standard deviation spectra.
         """
         s = self.St.copy()  # get a container
         s.data = self._outfit[3]
         s.name = "Standard deviation spectra"
         s.description = "Standard deviation spectra matrix from SIMPLISMA:"  # + logs
         return s
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/analysis/svd.py` & `spectrochempy-0.6.2/spectrochempy/analysis/svd.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,20 +60,20 @@
 # class PCA
 # ======================================================================================
 class SVD(DecompositionAnalysis):
 
     _docstring.delete_params("DecompositionAnalysis.see_also", "SVD")
 
     __doc__ = _docstring.dedent(
-        """
+        r"""
     Singular Value Decomposition (SVD).
 
-    The SVD is commonly written as :math:`X = U \\Sigma V^{T}` .
+    The SVD is commonly written as :math:`X = U \Sigma V^{T}`\ .
 
-    This class has the attributes : U, s = diag(S) and VT=V :math:`^T` .
+    This class has the attributes : U, s = diag(S) and VT=V :math:`^T`\ .
 
     If the dataset contains masked values, the corresponding ranges are
     ignored in the calculation.
 
     Parameters
     ----------
     %(AnalysisConfigurable.parameters)s
@@ -83,14 +83,15 @@
     %(DecompositionAnalysis.see_also.no_SVD)s
 
     Examples
     --------
     >>> dataset = scp.read('irdata/nh4y-activation.spg')
     >>> svd = scp.SVD()
     >>> svd.fit(dataset)
+    <svd: U(55, 55), s(55), VT(55, 5549)>
     >>> print(svd.ev.data)
     [1.185e+04      634 ... 0.001089 0.000975]
     >>> print(svd.ev_cum.data)
     [   94.54     99.6 ...      100      100]
     >>> print(svd.ev_ratio.data)
     [   94.54    5.059 ... 8.687e-06 7.779e-06]
     """
@@ -113,24 +114,22 @@
     # Initialization
     # ----------------------------------------------------------------------------------
     def __init__(
         self,
         *,
         log_level="WARNING",
         warm_start=False,
-        copy=True,
         **kwargs,
     ):
 
         # call the super class for initialisation of the configuration parameters
         # to do before anything else!
         super().__init__(
             log_level=log_level,
             warm_start=warm_start,
-            copy=copy,
             **kwargs,
         )
 
     # ----------------------------------------------------------------------------------
     # Private methods (overloading abstract classes)
     # ----------------------------------------------------------------------------------
     def _fit(self, X, Y=None):
@@ -184,15 +183,15 @@
 
     @property
     @_wrap_ndarray_output_to_nddataset(
         units=None, title="Singular values", typesingle="components"
     )
     def singular_values(self):
         """
-        Return a NDDataset containing singular values
+        Return a NDDataset containing singular values.
         """
         s = self._outfit[1]
         return s
 
     sv = singular_values
 
     @property
@@ -257,12 +256,7 @@
 
     @property
     def s(self):
         """
         Return Vector of singular values .
         """
         return self._outfit[1]
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/api.py` & `spectrochempy-0.6.2/spectrochempy/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,11 +133,7 @@
     # set a test file in environment
 
     environ["TEST_FILE"] = str(DATADIR / "irdata" / "nh4y-activation.spg")
     environ["TEST_FOLDER"] = str(DATADIR / "irdata" / "subdir")
     environ["TEST_NMR_FOLDER"] = str(
         DATADIR / "nmrdata" / "bruker" / "tests" / "nmr" / "topspin_2d"
     )
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/application/application.py` & `spectrochempy-0.6.2/spectrochempy/application/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 This module defines the `application` on which the API rely.
 
 It also defines
 the default application preferences and IPython magic functions.
 """
 
 import inspect
+import io
 import json
 import logging
 import pprint
 import subprocess
 import sys
 import threading
 import time
 import traceback
 import warnings
 from datetime import date, timedelta
-from io import StringIO
 from os import environ
 from pathlib import Path
+from zipfile import ZipFile
 
 import matplotlib as mpl
 import numpy as np
 import requests
 import traitlets as tr
 from IPython import get_ipython
 from IPython.core.error import UsageError
@@ -257,16 +258,45 @@
         # root = tk.Tk()
         # root.withdraw()
         # showinfo("New version available", message)
         # root.mainloop()
         return message
 
 
-CHECK_UPDATE = threading.Thread(target=_check_for_updates, args=(1,))
-CHECK_UPDATE.start()
+# --------------------------------------------------------------------------------------
+# Testdata
+# --------------------------------------------------------------------------------------
+def _download_full_testdata_directory(datadir):
+
+    # this process is relatively long, so we do not want to do it several time:
+    downloaded = datadir / "__downloaded__"
+    if downloaded.exists():
+        return
+
+    url = "https://github.com/spectrochempy/spectrochempy_data/archive/refs/heads/master.zip"
+
+    resp = requests.get(url, stream=True, allow_redirects=True)
+    zipfile = ZipFile(io.BytesIO(resp.content))
+    files = [zipfile.open(file_name) for file_name in zipfile.namelist()]
+
+    for file in files:
+        name = file.name
+        if name.endswith("/") or "testdata/" not in name:  # dir
+            continue
+        uncompressed = zipfile.read(name)
+        p = list(pathclean(name).parts)[2:]
+        dst = datadir.joinpath("/".join(p))
+        if not dst.parent.exists():
+            # create the eventually missing subdirectory
+            dst.parent.mkdir(parents=True, exist_ok=True)
+        dst.write_bytes(uncompressed)
+
+    # write the "__downloaded__" file to avoid this process to run several file.
+    downloaded.touch(exist_ok=True)
+
 
 # --------------------------------------------------------------------------------------
 # Other info
 # --------------------------------------------------------------------------------------
 url = "https://www.spectrochempy.fr"
 "URL for the documentation of this package"
 
@@ -700,15 +730,15 @@
                     "maxBytes": 262144,
                     "backupCount": 5,
                 },
                 "string": {
                     "class": "logging.StreamHandler",
                     "formatter": "console",
                     "level": "INFO",
-                    "stream": StringIO(),
+                    "stream": io.StringIO(),
                 },
             },
             "loggers": {
                 "SpectroChemPy": {
                     "level": "DEBUG",
                     "handlers": ["console", "rotatingfile", "string"],
                 },
@@ -961,36 +991,39 @@
         # ---------------------------------------------------------------------
         self._init_all_preferences()
 
         # we catch warnings and error for a lighter display to the end-user.
         # except if we are in debugging mode
 
         # warning handler
-        # --------------------------------------------------------------------
+        # ----------------
         def send_warnings_to_log(message, category):
             self.log.warning(f"{category.__name__} - {message}")
 
         warnings.showwarning = send_warnings_to_log
 
         # Warning handler
         # we catch warnings and error for a lighter display to the end-user.
         # except if we are in debugging mode
 
         warnings.showwarning = self._custom_warning
 
         # exception handler
+        # -----------------
         if ipy is not None:  # pragma: no cover
             ipy.set_custom_exc((Exception,), self._ipython_catch_exceptions)
         else:
-            sys.excepthook = self._catch_exceptions
+            if environ.get("SCPY_TESTING", 0) == 0 and "pytest" not in sys.argv[0]:
+                # catch exception only when pytest is not running
+                sys.excepthook = self._catch_exceptions
 
-            # load our custom magic extensions
-            # --------------------------------------------------------------------
-            if ipy is not None:
-                ipy.register_magics(SpectroChemPyMagics)
+        # load our custom magic extensions
+        # --------------------------------------------------------------------
+        if ipy is not None:
+            ipy.register_magics(SpectroChemPyMagics)
 
     def reset_preferences(self):
         """
         Reset all preferences to default.
         """
         self.reset_config = True
         self._init_all_preferences()
@@ -1184,10 +1217,15 @@
 plot_preferences = app.plot_preferences
 description = app.description
 long_description = app.long_description
 config_manager = app.config_manager
 config_dir = app.config_dir
 reset_preferences = app.reset_preferences
 
-# ======================================================================================
-if __name__ == "__main__":
-    pass
+
+CHECK_UPDATE = threading.Thread(target=_check_for_updates)
+CHECK_UPDATE.start()
+
+DOWNLOAD_TESTDATA = threading.Thread(
+    target=_download_full_testdata_directory, args=(preferences.datadir,)
+)
+DOWNLOAD_TESTDATA.start()
```

### Comparing `spectrochempy-0.6.1/spectrochempy/application/general_preferences.py` & `spectrochempy-0.6.2/spectrochempy/application/general_preferences.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/application/metaconfigurable.py` & `spectrochempy-0.6.2/spectrochempy/application/metaconfigurable.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     A subclass of Configurable that stores configuration changes in a json file.
 
     Saving the configuration changes allows to retrieve them between different
     executions of the main application.
     """
 
-    name = tr.Unicode(allow_none=True)
+    name = tr.Unicode(allow_none=True, help="Object name")
 
     def __init__(self, **kwargs):
         # keep only the current config section
         reset = kwargs.pop("reset", False)
         parent = kwargs.get("parent")
         parent_config = parent.config
         config = Config()
```

### Comparing `spectrochempy-0.6.1/spectrochempy/application/plot_preferences.py` & `spectrochempy-0.6.2/spectrochempy/application/plot_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,15 @@
     )
     figure_titlesize = Float(
         12.0, help=r"""size of the figure title (Figure.suptitle())"""
     ).tag(config=True, kind="")
     figure_titleweight = Unicode("normal", help=r"""weight of the figure title""").tag(
         config=True, kind=""
     )
-    figure_figsize = Tuple((6.8, 4.4), help=r"""figure size in inches""").tag(
+    figure_figsize = Tuple((6, 4), help=r"""figure size in inches""").tag(
         config=True, kind=""
     )
     figure_dpi = Float(96.0, help=r"""figure dots per inch""").tag(config=True, kind="")
     figure_facecolor = Unicode(
         "white", help=r"""figure facecolor; 0.75 is scalar gray"""
     ).tag(config=True, kind="color")
     figure_edgecolor = Unicode("white", help=r"""figure edgecolor""").tag(
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/__init__.py` & `spectrochempy-0.6.2/spectrochempy/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,11 +215,7 @@
         "set_nmr_context",
         "DimensionalityError",
     ]
 
 # START THE app
 with timeit("start app"):
     _started = app.start()
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/common/dialogs.py` & `spectrochempy-0.6.2/spectrochempy/core/common/dialogs.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/api.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/api.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/__init__.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndio.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndio.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,13 +467,7 @@
         self.filename = filename
         self.name = filename.stem
 
         return filename
 
 
 load = NDIO.load  # make plot accessible directly from the scp API
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
-
-# EOF
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndmath.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndmath.py`

 * *Files 0% similar despite different names*

```diff
@@ -3363,11 +3363,7 @@
 
 api_funcs = _update_api_funclist(NDMath)
 # print(api_funcs)
 
 for funcname in api_funcs:
     setattr(thismodule, funcname, getattr(NDMath, funcname))
     thismodule.__all__.append(funcname)
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/ndplot.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/ndplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -815,11 +815,7 @@
         """
         Matplotlib plot divider.
         """
         return self._divider
 
 
 plot = NDPlot.plot  # make plot accessible directly from the scp API
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/arraymixins/npy.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/arraymixins/npy.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,12 +102,7 @@
         new.units = b.units
     elif b.unitless:
         new.units = a.units
     else:
         new.units = a.units * b.units
 
     return new
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/meta.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/meta.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndarray.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndarray.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/baseobjects/ndcomplex.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/baseobjects/ndcomplex.py`

 * *Files 1% similar despite different names*

```diff
@@ -673,14 +673,7 @@
 
     # ----------------------------------------------------------------------------------
     # special methods
     # ----------------------------------------------------------------------------------
     def __setitem__(self, items, value):
 
         super().__setitem__(items, value)
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
-
-# end of module
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/coord.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/coord.py`

 * *Files 0% similar despite different names*

```diff
@@ -1072,11 +1072,7 @@
 
 
 # ======================================================================================
 # Set the operators
 # ======================================================================================
 _set_operators(Coord, priority=50)
 _set_operators(LinearCoord, priority=50)
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/coordset.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/coordset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1104,12 +1104,7 @@
         #   'old': 5, # The old value
         #   'name': "foo", # The name of the changed trait
         #   'type': 'change', # The event type of the notification, usually 'change'
         # }
 
         if change.name == "_updated" and change.new:
             self._updated = False  # reset
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/dataset/nddataset.py` & `spectrochempy-0.6.2/spectrochempy/core/dataset/nddataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module implements the `NDDataset` class.
 """
 
 __all__ = ["NDDataset"]
-
+# import signal
 import sys
 import textwrap
 from datetime import datetime, tzinfo
 
 import numpy as np
 import pytz  # TODO: for py>=3.9, we could use builtin zoneinfo library instead of pyt
 import traitlets as tr
@@ -37,33 +37,34 @@
 
 
 # ======================================================================================
 # NDDataset class definition
 # ======================================================================================
 @tr.signature_has_traits
 class NDDataset(NDMath, NDIO, NDPlot, NDComplexArray):
-    """
+    r"""
     The main N-dimensional dataset class used by  `SpectroChemPy`\ .
 
     The `NDDataset` is the main object use by SpectroChemPy. Like numpy
-    `~numpy.ndarray`\ s, `NDDataset` have the capability to be sliced, sorted and subject to
-    mathematical operations. But, in addition, `NDDataset` may have units,
+    `~numpy.ndarray`\ s, `NDDataset` have the capability to be sliced, sorted and
+    subject to mathematical operations. But, in addition, `NDDataset` may have units,
     can be masked and each dimensions can have coordinates also with units. This make
     `NDDataset` aware of unit compatibility,
     *e.g.,* for binary operation such as additions or subtraction or during the
     application of mathematical operations.
     In addition or in replacement of numerical data for coordinates,
     `NDDataset` can also have labeled coordinates where labels can be different kind of
     objects (`str`\ , `datetime`\ , `~numpy.ndarray` or other `NDDataset`\ 's, etc...).
 
     Parameters
     ----------
     data : :term:`array-like`
         Data array contained in the object. The data can be a list, a tuple,
-        a `~numpy.ndarray`, a subclass of `~numpy.ndarray`, another `NDDataset` or a  `Coord` object.
+        a `~numpy.ndarray`, a subclass of `~numpy.ndarray`, another `NDDataset` or a
+        `Coord` object.
         Any size or shape of data is accepted. If not given, an empty
         `NDDataset` will be inited.
         At the initialisation the provided data will be eventually cast to
         a `~numpy.ndarray`\ .
         If the provided objects is passed which already contains some
         mask, or units, these elements will be used if possible to accordingly set
         those of the created object. If possible, the provided data will not be copied
@@ -399,15 +400,16 @@
                 "__aiter__",
                 "__name__",
                 "__qualname__",
             ]
             or "_validate" in item
             or "_changed" in item
         ):
-            # raise an error so that traits, ipython operation and more ... will be handled correctly
+            # raise an error so that traits, ipython operation and more ...
+            # will be handled correctly
             raise AttributeError
 
         # syntax such as ds.x, ds.y, etc...
 
         if item[0] in self.dims or self._coordset:
 
             # look also properties
@@ -450,14 +452,17 @@
                     )
 
             return None
 
         raise AttributeError
 
     def __setattr__(self, key, value):
+        # TODO: entering this function in debug stepping mode kill the program
+        #    need to investigate further, why!
+
         if key in DEFAULT_DIM_NAME:  # syntax such as ds.x, ds.y, etc...
             # Note the above test is important to avoid errors with traitlets
             # even if it looks redundant with the following
             if key in self.dims:
                 if self._coordset is None:
                     # we need to create a coordset first
                     self.set_coordset(
@@ -484,15 +489,16 @@
                 else:
                     _coordset[idx] = Coord(value, name=key)
                 _coordset = self._valid_coordset(_coordset)
                 self._coordset.set(_coordset)
             else:
                 raise AttributeError(f"Coordinate `{key}` is not used.")
         else:
-            super().__setattr__(key, value)
+            # print(key, value)
+            super(NDDataset, self).__setattr__(key, value)
 
     def __eq__(self, other, attrs=None):
         attrs = self.__dir__()
         for attr in (
             "filename",
             "preferences",
             "name",
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/plotters/multiplot.py` & `spectrochempy-0.6.2/spectrochempy/core/plotters/multiplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,11 +438,7 @@
 
         fig.canvas.mpl_connect("axes_enter_event", _onenter)
         fig.canvas.mpl_connect("axes_leave_event", _onenter)
         fig.canvas.mpl_connect("figure_enter_event", _onenter)
         fig.canvas.mpl_connect("figure_leave_event", _onenter)
 
     return axes
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/plotters/plot1d.py` & `spectrochempy-0.6.2/spectrochempy/core/plotters/plot1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -601,11 +601,7 @@
             zdata.max() + 1,
             where=new.mask,
             facecolor="#FFEEEE",
             alpha=0.3,
         )
 
     return ax
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/plotters/plot2d.py` & `spectrochempy-0.6.2/spectrochempy/core/plotters/plot2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,11 +803,7 @@
     clevel = cl * (maximum - start) / cl.max() + start
     clevelneg = -clevel
     clevelc = clevel
     if negative:
         clevelc = sorted(list(np.concatenate((clevel, clevelneg))))
 
     return clevelc
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/plotters/plot3d.py` & `spectrochempy-0.6.2/spectrochempy/core/plotters/plot3d.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/plotters/plotly.py` & `spectrochempy-0.6.2/spectrochempy/core/plotters/plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,11 +566,7 @@
 #
 #     print(np.count_nonzero(~new.mask), COUNT)
 #     keep = []
 #     for i, b in enumerate(new.mask):
 #         if not b:
 #             keep.append(ds[i])
 #     return keep
-#
-#
-# if __name__ == '__main__':
-#     pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/align.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/align.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/apodization.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/apodization.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/autosub.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/autosub.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/baseline.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/baseline.py`

 * *Files 0% similar despite different names*

```diff
@@ -844,11 +844,7 @@
         poly = np.poly1d(row)
         baseline[i] = poly(w)
 
     if data.ndim == 1:
         baseline = baseline[0]
 
     return baseline
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/concatenate.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/concatenate.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,11 +247,7 @@
 # --------------------
 def _get_copy(datasets):
     # get a copy of datasets from the input
     if isinstance(datasets, tuple):
         if isinstance(datasets[0], (list, tuple)):
             datasets = datasets[0]
     return [ds.copy() for ds in datasets]
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/fft.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/fft.py`

 * *Files 0% similar despite different names*

```diff
@@ -631,12 +631,7 @@
     else:
         for i, vec in enumerate(dataset):
             z[i] = hilbert(vec.real, N)[: dataset.shape[-1]] * fac
 
     # correct the real data as sometimes it changes
     z.real = dataset.real
     return z
-
-
-# ======================================================================================
-if __name__ == "__main__":  # pragma: no cover
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/filter.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/filter.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/integrate.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/integrate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/interpolate.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/interpolate.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/phasing.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/phasing.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/shift.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/shift.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/smooth.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/smooth.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,11 +122,7 @@
         # restore original data order if it was swapped
         if swapped:
             new.swapdims(axis, -1, inplace=True)  # must be done inplace
     else:
         new = data
 
     return new
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/utils.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/processors/zero_filling.py` & `spectrochempy-0.6.2/spectrochempy/core/processors/zero_filling.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/project/abstractproject.py` & `spectrochempy-0.6.2/spectrochempy/core/project/abstractproject.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/project/project.py` & `spectrochempy-0.6.2/spectrochempy/core/project/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         If not None, this list gives the names associated to each
         object passed as args. It MUST be the same length that the
         number of args, or an error will be raised.
         If None, the internal name of each object will be used instead.
     name : str, optional
         The name of the project.  If the name is not provided, it will be
         generated automatically.
-    \**meta : dict
+    **meta : dict
         Any other attributes to describe the project.
 
     See Also
     --------
     NDDataset : The main object containing arrays.
     Script : Executables scripts container.
 
@@ -617,12 +617,7 @@
         def wrapper(*args, **kwargs):
             f = func(*args, **kwargs)
             return f
 
         return wrapper
 
     return decorator
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/download.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,26 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 In this module, methods are provided to download external datasets
 from public database.
 """
-__all__ = ["download_iris", "download_nist_ir", "download"]
+__all__ = ["download_iris", "download_nist_ir"]
 __dataset_methods__ = __all__
 
-import shutil
 from io import StringIO
 from pathlib import Path
 
 import numpy as np
 import requests
 
 from spectrochempy.core import error_, info_
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.core.readers.importer import read
 from spectrochempy.core.readers.read_jcamp import read_jcamp
 from spectrochempy.utils.misc import is_iterable
 from spectrochempy.utils.optional import import_optional_dependency
 
 
 def download_iris():
     """
@@ -214,57 +212,7 @@
                 "Can't read this JCAMP file: please report the issue to Spectrochempy developpers"
             )
 
     if len(out) == 1:
         return out[0]
     else:
         return out
-
-
-def download(url):
-    """
-    Download data from an url
-
-    Parameters
-    ----------
-    url : str
-        url to a readable file
-
-    Returns
-    -------
-    list of NDDataset or NDDataset
-        The dataset(s).
-
-    See Also
-    --------
-    read : Read data from experimental data.
-    """
-
-    # https://stackoverflow.com/questions/16694907/download-large-file-in-python-with-requests
-
-    local_filename = url.split("/")[-1]
-
-    try:
-        response = requests.get(url, stream=True, timeout=10)
-    except OSError:
-        error_("OSError: could not connect")
-        return None
-
-    with response as r:
-        r.raise_for_status()
-        with open(local_filename, "wb") as f:
-            shutil.copyfileobj(r.raw, f)
-            ds = read(local_filename)
-
-            if isinstance(ds, NDDataset):
-                ds.history = f"Downloaded from {url}"
-            elif isinstance(ds, list):
-                for ds_ in ds:
-                    ds_.history = f"Downloaded from {url}"
-
-    Path(local_filename).unlink()
-    return ds
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/importer.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/importer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module define a generic class to import directories, files and contents.
 """
-__all__ = ["read", "read_dir", "read_remote"]
+__all__ = ["read", "read_dir"]  # , "read_remote"]
 __dataset_methods__ = __all__
 
-from io import BytesIO
+import io
+import re
 from warnings import warn
 from zipfile import ZipFile
 
 import requests
 import yaml
 from traitlets import Dict, HasTraits, List, Type, Unicode
 
 from spectrochempy.core import info_, warning_
+from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.exceptions import DimensionsCompatibilityError, ProtocolError
 from spectrochempy.utils.file import (
     check_filename_to_open,
     get_directory_name,
     get_filenames,
     pathclean,
 )
@@ -31,15 +33,16 @@
     ("scp", "SpectroChemPy files (*.scp)"),
     ("omnic", "Nicolet OMNIC files and series (*.spa *.spg *.srs)"),
     ("soc", "Surface Optics Corp. (*.ddr *.hdr *.sdr)"),
     ("labspec", "LABSPEC exported files (*.txt)"),
     ("opus", "Bruker OPUS files (*.[0-9]*)"),
     (
         "topspin",
-        "Bruker TOPSPIN fid or series or processed data files (fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
+        "Bruker TOPSPIN fid or series or processed data files "
+        "(fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
     ),
     ("matlab", "MATLAB files (*.mat)"),
     ("dso", "Data Set Object files (*.dso)"),
     ("jcamp", "JCAMP-DX files (*.jdx *.dx)"),
     ("csv", "CSV files (*.csv)"),
     ("excel", "Microsoft Excel files (*.xls)"),
     ("zip", "Compressed folder of data files (*.zip)"),
@@ -63,15 +66,15 @@
     ("xls", "excel"),
     ("asc", "quadera"),
 ]
 
 
 # --------------------------------------------------------------------------------------
 class Importer(HasTraits):
-    # Private _Importer class
+    # Private Importer class
 
     objtype = Type()
     datasets = List()
     files = Dict()
     default_key = Unicode()
     protocol = Unicode()
 
@@ -93,17 +96,19 @@
 
     def __call__(self, *args, **kwargs):
 
         self.datasets = []
         self.default_key = kwargs.pop("default_key", ".scp")
 
         if "merge" not in kwargs.keys():
-            # if merge is not specified, but the args are provided as a single list, then will are supposed to merge
-            # the datasets. If merge is specified then it has priority.
-            # This is not useful for the 1D datasets, as if they are compatible they are merged automatically
+            # if merge is not specified, but the args are provided as a single list,
+            # then will are supposed to merge the datasets. If merge is specified then
+            # it has priority.
+            # This is not useful for the 1D datasets, as if they are compatible they
+            # are merged automatically
             if args and len(args) == 1 and isinstance(args[0], (list, tuple)):
                 kwargs["merge"] = True
 
         args, kwargs = self._setup_objtype(*args, **kwargs)
         res = check_filename_to_open(*args, **kwargs)
         if res:
             # Normal return
@@ -136,16 +141,16 @@
 
         # now we will reset preference for this newly loaded datasets
         if len(self.datasets) > 0:
 
             if all(self.datasets) is None:
                 return None
 
-            prefs = self.datasets[0].preferences
             try:
+                prefs = self.datasets[0].preferences
                 prefs.reset()
             except (FileNotFoundError, AttributeError):
                 pass
         else:
             return None
 
         if len(self.datasets) == 1:
@@ -194,77 +199,71 @@
 
         protocol = kwargs.get("protocol", None)
         if protocol is not None and protocol != "ALL":
             if not isinstance(protocol, list):
                 protocol = [protocol]
             if key and key[1:] not in protocol and self.alias[key[1:]] not in protocol:
                 return
+
         datasets = []
         for filename in files[key]:
-            if (
-                isinstance(filename, str)
-                and not filename.startswith("http://")
-                and not filename.startswith("https://")
-            ):
-                filename = pathclean(filename)
+
             read_ = getattr(self, f"_read_{key[1:]}")
+
+            dataset = None
             try:
-                res = read_(self.objtype(), filename, **kwargs)
-                # sometimes read_ can return None (e.g. non labspec text file)
-            except FileNotFoundError:
-                # try to get the file from github
-                kwargs["read_method"] = read_
-                try:
-                    res = _read_remote(self.objtype(), filename, **kwargs)
+                # read locally or using url if filename is an url
+                dataset = read_(self.objtype(), filename, **kwargs)
 
-                except OSError as e:
-                    if kwargs.get("remote"):
-                        raise e
-                    else:
-                        raise FileNotFoundError(f"{filename} not found")
+            except (FileNotFoundError, OSError) as exc:
+                # file was not found.
+                # it is an url we raise an error
+                local_only = kwargs.get("local_only", False)
+                if _is_url(filename) or local_only:
+                    raise (FileNotFoundError) from exc
 
-                except IOError as e:
-                    warning_(str(e))
-                    res = None
+                # else, we try on github
+                try:
+                    # Try to get the file from github
+                    kwargs["read_method"] = read_
+                    info_(
+                        "File/directory not found locally: Attempt to download it from "
+                        "the GitHub repository `spectrochempy_data`..."
+                    )
+                    dataset = _read_remote(self.objtype(), filename, **kwargs)
 
-                except NotImplementedError as e:
-                    warning_(str(e))
-                    res = None
+                except (FileNotFoundError) as exc:
+                    raise (FileNotFoundError) from exc
 
                 except Exception as e:
-                    raise e
-
-            except IOError as e:
-                warning_(str(e))
-                res = None
+                    warning_(str(e))
 
-            except NotImplementedError as e:
+            except Exception as e:
                 warning_(str(e))
-                res = None
 
-            if res is not None:
-                if not isinstance(res, list):
-                    datasets.append(res)
+            if dataset is not None:
+                if not isinstance(dataset, list):
+                    datasets.append(dataset)
                 else:
-                    datasets.extend(res)
+                    datasets.extend(dataset)
 
         if len(datasets) > 1:
             datasets = self._do_merge(datasets, **kwargs)
             if kwargs.get("merge", False):
                 datasets[0].name = pathclean(filename).stem
                 datasets[0].filename = pathclean(filename)
 
         self.datasets.extend(datasets)
 
     def _do_merge(self, datasets, **kwargs):
 
         # several datasets returned (only if several files have been passed) and the `merge` keyword argument is False
         merged = kwargs.get("merge", False)
-        shapes = {nd.shape for nd in datasets}
-        if len(shapes) == 1:
+        shapes = {nd.shape if hasattr(nd, "shape") else None for nd in datasets}
+        if len(shapes) == 1 and None not in shapes:
             # homogeneous set of files
             dim0 = shapes.pop()[0]
             if dim0 == 1:
                 merged = kwargs.get("merge", True)  # priority to the keyword setting
         else:
             # not homogeneous
             merged = kwargs.get("merge", False)
@@ -287,142 +286,180 @@
 def _importer_method(func):
     # Decorator to define a given read function as belonging to Importer
     setattr(Importer, func.__name__, staticmethod(func))
     return func
 
 
 # --------------------------------------------------------------------------------------
-# Generic Read function
+# Public Generic Read function
 # --------------------------------------------------------------------------------------
+
+_docstring.get_sections(
+    """
+See Also
+--------
+read : Generic reader inferring protocol from the filename extension.
+read_zip : Read Zip archives (containing spectrochempy readable files)
+read_dir : Read an entire directory.
+read_opus : Read OPUS spectra.
+read_labspec : Read Raman LABSPEC spectra (:file:`.txt`\ ).
+read_omnic : Read Omnic spectra (:file:`.spa`\ , :file:`.spg`\ , :file:`.srs`\ ).
+read_soc : Read Surface Optics Corps. files (:file:`.ddr` , :file:`.hdr` or :file:`.sdr`\ ).
+read_galactic : Read Galactic files (:file:`.spc`\ ).
+read_quadera : Read a Pfeiffer Vacuum's QUADERA mass spectrometer software file.
+read_topspin : Read TopSpin Bruker NMR spectra.
+read_csv : Read CSV files (:file:`.csv`\ ).
+read_jcamp : Read Infrared JCAMP-DX files (:file:`.jdx`\ , :file:`.dx`\ ).
+read_matlab : Read Matlab files (:file:`.mat`\ , :file:`.dso`\ ).
+read_carroucell : Read files in a directory after a carroucell experiment.
+""",
+    sections=["See Also"],
+    base="Importer",
+)
+
+_docstring.delete_params("Importer.see_also", "read")
+
+
+@_docstring.dedent
 def read(*paths, **kwargs):
     """
     Generic read method.
 
     This method is generally able to load experimental files based on extensions.
 
     Parameters
     ----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
+    *paths : `str`, `~pathlib.Path` object objects or valid urls, optional
         The data source(s) can be specified by the name or a list of name for the
         file(s) to be loaded:
 
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
+        * *e.g.,* ( filename1, filename2, ...,  \*\*kwargs )*
 
         If the list of filenames are enclosed into brackets:
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
+        * *e.g.,* ( **[** *filename1, filename2, ...* **]**, \*\*kwargs *)*
 
         The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no
-        `filename` , nor `content` ),
+        except if ``merge`` is set to `False`.
+
+        If a source is not provided (*i.e.,* no ``paths`` , nor ``content``\ ),
         a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    %(kwargs)s
 
     Returns
-    --------
-    read
-        `NDDataset` or list of `NDDataset` .
+    -------
+    object : `NDDataset` or list of `NDDataset`
+        The returned dataset(s).
 
     Other Parameters
     ----------------
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whenever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the
-        default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as
-        arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description : str, optional
+    protocol : `str`\ , optional
+        ``Protocol`` used for reading. It can be one of {``'scp'``\ , ``'omnic'``\ ,
+        ``'opus'``\ , ``'topspin'``\ , ``'matlab'``\ , ``'jcamp'``\ , ``'csv'``\ ,
+        ``'excel'``\ }. If not provided, the correct protocol
+        is inferred (whenever it is possible) from the filename extension.
+    directory : `~pathlib.Path` object objects or valid urls, optional
+        From where to read the files.
+    merge : `bool`\ , optional, default: `False`
+        If `True` and several filenames or a ``directory`` have been provided as
+        arguments, then a single `NDDataset` with merged (stacked along the first
+        dimension) is returned.
+    sortbydate : `bool`, optional, default: `True`
+        Sort multiple filename by acquisition date.
+    description : `str`, optional
         A Custom description.
-    origin : {'omnic', 'tga'}, optional
-        In order to properly interpret CSV file it can be necessary to set the origin
-        of the spectra.
-        Up to now only 'omnic' and 'tga' have been implemented.
-    csv_delimiter : str, optional
+    origin : one of {``'omnic'``\ , ``'tga'``\ }, optional
+        Used when reading with the CSV protocol. In order to properly interpret CSV file
+        it can be necessary to set the origin of the spectra.
+        Up to now only ``'omnic'`` and ``'tga'`` have been implemented.
+    csv_delimiter : `str`\ , optional, default: `~spectrochempy.preferences.csv_delimiter`
         Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy `Preferences` .
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True)
-    recursive : bool, optional
-        Read also in subfolders. (default=False)
+    content : `bytes` object, optional
+        Instead of passing a filename for further reading, a bytes content can be
+        directly provided as bytes objects.
+        The most convenient way is to use a dictionary. This feature is particularly
+        useful for a GUI Dash application to handle drag and drop of files into a
+        Browser.
+    iterdir : `bool`\ , optional, default: `True`
+        If `True` and no filename was provided, all files present in the provided
+        ``directory`` are returned (and merged if ``merge`` is `True`\ .
+        It is assumed that all the files correspond to current reading protocol.
+
+        .. versionchanged:: 0.6.2
+
+            ``iterdir`` replace the deprecated ``listdir`` argument.
+
+    recursive : `bool`, optional, default: `False`
+        Read also in subfolders.
+    replace_existing: `bool`, optional, default: `False`
+        Used only when url are specified. By default, existing files are not replaced
+        so not downloaded.
+    download_only: `bool`, optional, default: `False`
+        Used only when url are specified.  If True, only downloading and saving of the
+        files is performed, with no attempt to read their content.
+    read_only: `bool`, optional, default: `True`
+        Used only when url are specified.  If True, saving of the
+        files is performed in the current directory, or in the directory specified by
+        the directory parameter.
 
     See Also
     --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .spa single spectra.
-    read_spc : Read Galactic .spc files.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    %(Importer.see_also.no_read)s
 
     Examples
     ---------
-    Reading a single OPUS file  (providing a windows type filename relative to the default `Datadir` )
+    Reading a single OPUS file  (providing a windows type filename relative
+    to the default `~spectrochempy.preferences.datadir` )
 
     >>> scp.read('irdata\\\\OPUS\\\\test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-    Reading a single OPUS file  (providing a unix/python type filename relative to the default `Datadir` )
+    Reading a single OPUS file  (providing a unix/python type filename relative
+    to the default ``datadir`` )
     Note that here read_opus is called as a classmethod of the NDDataset class
 
     >>> scp.NDDataset.read('irdata/OPUS/test.0000')
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Single file specified with pathlib.Path object
 
     >>> from pathlib import Path
     >>> folder = Path('irdata/OPUS')
     >>> p = folder / 'test.0000'
     >>> scp.read(p)
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-    Multiple files not merged (return a list of datasets). Note that a directory is specified
+    Multiple files not merged (return a list of datasets).
+    Note that a directory is specified
 
     >>> le = scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
     >>> len(le)
     3
     >>> le[0]
     NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
     Multiple files merged as the `merge` keyword is set to true
 
     >>> scp.read('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
     NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
-    Multiple files to merge : they are passed as a list instead of using the keyword `merge`
+    Multiple files to merge : they are passed as a list instead of using the keyword
+    `merge`
 
     >>> scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
     NDDataset: [float64] a.u. (shape: (y:3, x:2567))
 
     Multiple files not merged : they are passed as a list but `merge` is set to false
 
     >>> le = scp.read(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
     >>> len(le)
     3
 
-    Read without a filename. This has the effect of opening a dialog for file(s) selection
+    Read without a filename. This has the effect of opening a dialog for file(s)
+    selection
 
     >>> nd = scp.read()
 
     Read in a directory (assume that only OPUS files are present in the directory
     (else we must use the generic `read` function instead)
 
     >>> le = scp.read(directory='irdata/OPUS')
@@ -449,201 +486,310 @@
         if default_filter is not None:
             kwargs["default_filter"] = importer.filetypes[default_filter]
     else:
         try:
             kwargs["filetypes"] = [importer.filetypes[protocol]]
         except KeyError:
             raise ProtocolError(protocol, list(importer.protocols.values()))
+        except TypeError as e:
+            print(e)
+
+    # deprecated kwargs
+    listdir = kwargs.pop("listdir", True)
+    if "listdir" in kwargs and "iterdir" not in kwargs:
+        kwargs["iterdir"] = listdir
+        warning_(
+            "argument `listdir` is deprecated, use ìterdir` instead",
+            category=DeprecationWarning,
+        )
 
     return importer(*paths, **kwargs)
 
 
+# for some reasons the doctring.getsection modify the signature of the function
+# when used as a decorator, so we use it as a function
+_docstring.get_sections(
+    read.__doc__,
+    sections=["Parameters", "Other Parameters", "Returns"],
+    base="Importer",
+)
+
+_docstring.delete_params("Importer.see_also", "read_dir")
+
+
+@_docstring.dedent
 def read_dir(directory=None, **kwargs):
     """
     Read an entire directory.
 
-    Open a list of readable files in a and store data/metadata in a dataset or a list of datasets according to the
-    following rules :
+    Open a list of readable files in a and store data/metadata in a dataset or a list of
+    datasets according to the following rules :
 
     * 2D spectroscopic data (e.g. valid .spg files or matlab arrays, etc...) from
-      distinct files are stored in distinct NDdatasets.
-    * 1D spectroscopic data (e.g., .spa files) in a given directory are grouped
-      into single NDDataset, providing their unique dimension are compatible. If not,
-      an error is generated.
+      distinct files are stored in distinct `NDdataset`\ s.
+    * 1D spectroscopic data (e.g., :file:`.spa` files) in a given directory are merged
+      into single `NDDataset`\ , providing their unique dimension are compatible.
+      If not, an error is generated.
     * non-readable files are ignored
 
     Parameters
     ----------
     directory : str or pathlib
         Folder where are located the files to read.
 
     Returns
     --------
-    read_dir
-        `NDDataset` or list of `NDDataset` .
-
-    Depending on the python version, the order of the datasets in the list may change.
+    %(Importer.returns)s
+        Depending on the python version, the order of the datasets in the list
+        may change.
 
     See Also
     --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .Spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    %(Importer.see_also.no_read_dir)s
 
     Examples
     --------
 
     >>> scp.preferences.csv_delimiter = ','
     >>> A = scp.read_dir('irdata')
     >>> len(A)
     4
 
     >>> B = scp.NDDataset.read_dir()
     """
-    kwargs["listdir"] = True
+    kwargs["iterdir"] = True
     importer = Importer()
     return importer(directory, **kwargs)
 
 
-def read_remote(file_or_dir, **kwargs):
-    """
-    Download and read files or an entire directory on github spectrochempy_data
-    repository.
+# _docstring.delete_params("Importer.see_also", "read_remote")
+# @_docstring.dedent
+# def read_remote(file_or_dir, **kwargs):
+#     """
+#     Download and read files or an entire directory from any url
+#
+#     The first usage in spectrochempy is the loading of test files in the
+#     `spectrochempy_data repository <https://github.com/spectrochempy/spectrochempy_data>`__\ .
+#     This is done only if the data are not yet
+#     downloaded and present in the `~spectrochempy.preferences.datadir` directory.
+#
+#     It can also be used to download and read file or directory from any url.
+#
+#     Parameters
+#     ----------
+#     path : `str`, `~pathlib.Path` object or an url.
+#         When a file or folder is specified, it must be written as if it were present
+#         locally exactly as for the `read` function. The correponding file or directory
+#         is downloaded from the ``github spectrochemp_data`` repository.
+#         Otherwise it should be a full and valid url.
+#     %(kwargs)s
+#
+#     Returns
+#     --------
+#     %(Importer.returns)s
+#
+#     Other Parameters
+#     ----------------
+#     %(Importer.other_parameters)s
+#
+#     See Also
+#     --------
+#     %(Importer.see_also.no_read_remote)s
+#
+#     Examples
+#     --------
+#
+#     >>> A = scp.read_remote('irdata/subdir')
+#     """
+#     kwargs["remote"] = True
+#     importer = Importer()
+#     return importer(file_or_dir, **kwargs)
+#
 
-    This is done only if the data are not yet downloaded and present in the DATADIR
-    directory.
+# ======================================================================================
+# Private read functions
+# ======================================================================================
+@_importer_method
+def _read_dir(*args, **kwargs):
+    _, directory = args
+    directory = get_directory_name(directory)
+    files = get_filenames(directory, **kwargs)
+    datasets = []
+    valid_extensions = list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]
+    for key in [key for key in files.keys() if key[1:] in valid_extensions]:
+        if key:
+            importer = Importer()
+            nd = importer(files[key], **kwargs)
+            if nd is not None:
+                if not isinstance(nd, list):
+                    nd = [nd]
+                datasets.extend(nd)
+    return datasets
 
-    Parameters
-    ----------
-    file_or_dir : str or pathlib
-        Folder where are located the files to read
-        (it should be written as if it was locally downloaded already).
-    **kwargs : optional keywords parameters
-        See Other Parameters.
 
-    Other Parameters
-    ----------------
-    merge : bool, optional, default: False
-        By default files read are noot merged
-    replace_existing: bool, optional, default: False
-        By default, existing files are not replaced so not downloaded.
-    download_only: bool, optional, default: False
-        If True, only downloading and saving of the files is performed, with no
-        attempt to read their content.
+@_importer_method
+def _read_scp(*args, **kwargs):
+    dataset, filename = args
+    return dataset.load(filename, **kwargs)
 
-    Returns
-    --------
-    dataset(s)
-        `NDDataset` or list of `NDDataset` .
 
-    See Also
-    --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_spa : Read Omnic \*.spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+@_importer_method
+def _read_(*args, **kwargs):
+    dataset, filename = args
 
-    Examples
-    --------
+    if kwargs.pop("remote", False):
+        return Importer._read_remote(*args, **kwargs)
+    elif not filename or filename.is_dir():
+        return Importer._read_dir(*args, **kwargs)
+    else:
+        raise FileNotFoundError
 
-    >>> A = scp.read_remote('irdata/subdir')
-    """
-    kwargs["remote"] = True
-    if "merge" not in kwargs:
-        kwargs["merge"] = False  # by default, no attempt to merge
-    if "replace_existing" not in kwargs:
-        kwargs["replace_existing"] = False  # by default we download only if needed.
-    importer = Importer()
-    return importer(file_or_dir, **kwargs)
+    # protocol = kwargs.get("protocol", None)
+    # if protocol and ".scp" in protocol:
+    #     return dataset.load(filename, **kwargs)
+    #
+    # elif filename and filename.name in ("fid", "ser", "1r", "2rr", "3rrr"):
+    #     # probably an Topspin NMR file
+    #     return dataset.read_topspin(filename, **kwargs)
+    # elif filename:
+    #     # try scp format
+    #     try:
+    #         return dataset.load(filename, **kwargs)
+    #     except Exception:
+    #         # lets try some common format
+    #         for key in ["omnic", "opus", "topspin", "labspec", "matlab", "jdx"]:
+    #             try:
+    #                 _read = getattr(dataset, f"read_{key}")
+    #                 f = f"{filename}.{key}"
+    #                 return _read(f, **kwargs)
+    #             except Exception:
+    #                 pass
+    #         raise NotImplementedError
+
+
+# ======================================================================================
+# Private functions
+# ======================================================================================
+def _is_url(filename):
+    return (
+        isinstance(filename, str)
+        and re.match(r"http[s]?:[\/]{2}", filename) is not None
+    )
+
+
+def _openfid(filename, mode="rb", **kwargs):
+    # Return a file ID
+
+    # Check if Content has been passed?
+    content = kwargs.get("content", False)
+
+    # default encoding
+    encoding = "utf-8"
+
+    if _is_url(filename):
+        # by default we set the read_only flag to True when reading remote url
+        kwargs["read_only"] = kwargs.get("read_only", True)
+
+        # use request to read the remote content
+        r = requests.get(filename, allow_redirects=True)
+        r.raise_for_status()
+        content = r.content
+        encoding = r.encoding
+
+    else:
+        # Transform filename to a Path object is not yet the case
+        filename = pathclean(filename)
+
+    # Create the file ID
+    if content:
+        # if a content has been passed, then it has priority
+        fid = (
+            io.BytesIO(content)
+            if mode == "rb"
+            else io.StringIO(content.decode(encoding))
+        )
+    else:
+        fid = open(filename, mode=mode)
+
+    return fid, kwargs
 
 
 def _write_downloaded_file(content, dst):
     if not dst.parent.exists():
         # create the eventually missing subdirectory
         dst.parent.mkdir(parents=True, exist_ok=True)
     dst.write_bytes(content)
     info_(f"{dst.name} has been downloaded and written in {dst.parent}")
 
 
-def _get_url_content_and_save(url, dst, replace):
+def _get_url_content_and_save(url, dst, replace, read_only=False):
 
     if not replace and dst.exists():
         return
 
     try:
         r = requests.get(url, allow_redirects=True)
 
-        # write downloaded file
         r.raise_for_status()
-        _write_downloaded_file(r.content, dst)
+
+        # write downloaded file
+        if not read_only:
+            _write_downloaded_file(r.content, dst)
+
+        # in all case return the content
+        return r.content
 
     except OSError:
         raise FileNotFoundError(f"Not found locally or at url:{url}")
 
 
 def _download_full_testdata_directory():
     from spectrochempy.core import preferences as prefs
 
     datadir = prefs.datadir
 
     url = "https://github.com/spectrochempy/spectrochempy_data/archive/refs/heads/master.zip"
 
     resp = requests.get(url)
-    zipfile = ZipFile(BytesIO(resp.content))
+    zipfile = ZipFile(io.BytesIO(resp.content))
     files = [zipfile.open(file_name) for file_name in zipfile.namelist()]
 
     for file in files:
         name = file.name
         if name.endswith("/") or "testdata/" not in name:  # dir
             continue
         uncompressed = zipfile.read(name)
         p = list(pathclean(name).parts)[2:]
         dst = datadir.joinpath("/".join(p))
         _write_downloaded_file(uncompressed, dst)
 
 
-def _download_from_url(url, dst, replace=False):
-    # ##
-    # ##    Do not forget to change the fork in the following url
-    # ##
-    if not str(url).startswith("https://") and not str(url).startswith("http://"):
-        # download on github
-        url = (
-            f"https://github.com/spectrochempy/spectrochempy_data/raw/master/"
-            f"testdata/{url}"
-        )
+def _download_from_github(path, dst, replace=False):
+    # download on github (always save the downloaded files)
+    relative_path = str(pathclean(path).as_posix())
+    path = (
+        f"https://github.com/spectrochempy/spectrochempy_data/raw/master/"
+        f"testdata/{relative_path}"
+    )
 
-        # first determine if it is a directory
-        r = requests.get(url + "/__index__", allow_redirects=True)
-        index = None
-        if r.status_code == 200:
-            index = yaml.load(r.content, Loader=yaml.CLoader)
+    # first determine if it is a directory
+    r = requests.get(path + "/__index__", allow_redirects=True)
+    index = None
+    if r.status_code == 200:
+        index = yaml.load(r.content, Loader=yaml.CLoader)
 
-        if index is None:
-            _get_url_content_and_save(url, dst, replace)
+    if index is None:
+        return _get_url_content_and_save(path, dst, replace)
 
-        else:
-            for filename in index["files"]:
-                _get_url_content_and_save(f"{url}/{filename}", dst / filename, replace)
-            for folder in index["folders"]:
-                _download_from_url(f"{url}/{folder}", dst / folder)
     else:
-        # download url
-        _get_url_content_and_save(url, dst, replace)
+        # download folder
+        for filename in index["files"]:
+            _get_url_content_and_save(f"{path}/{filename}", dst / filename, replace)
+        for folder in index["folders"]:
+            _download_from_github(f"{relative_path}/{folder}", dst / folder)
 
 
 def _is_relative_to(path, base):
     # try to emulate the pathlib is_relative_to method which does not work on python
     # 3.7 (needed for Colab!)
     # TODO: replace as Colab is updated to 3.9
     pparts = path.parts
@@ -668,102 +814,56 @@
 
 
 @_importer_method
 def _read_remote(*args, **kwargs):
     from spectrochempy.core import preferences as prefs
 
     datadir = prefs.datadir
-
     dataset, path = args
-    is_url = str(path).startswith("http://") or str(path).startswith("https://")
-
-    replace = kwargs.pop("replace_existing", False)
-    if not is_url:
-        path = pathclean(path)
-
-        if _is_relative_to(path, datadir):
-            # try to make it relative for remote downloading on github
-            relative_path = _relative_to(path, datadir)
-        else:
-            # assume it is already relative
-            relative_path = path
-
-        # in principle the data came from github. Try to download it
-        dst = datadir / relative_path
-        if dst.name != "testdata":
-            _download_from_url(relative_path, dst, replace)
-        else:
-            # we are going to download the whole testdata directory -> use a faster method
-            _download_full_testdata_directory()
-
+    kwargs["merge"] = kwargs.get("merge", False)  # by default, no attempt to merge
+    read_method = kwargs.pop("read_method", read)
+    download_only = kwargs.pop("download_only", False)
+    replace = kwargs.pop(
+        "replace_existing", False
+    )  # by default we download only if needed.
+
+    # downloaded file
+    # we try to download the github testdata
+    path = pathclean(path)
+
+    # we need to download additional files for topspin
+    topspin = True if "topspin" in read_method.__name__ else False
+    # we have to treat a special case: topspin, where the parent directory need
+    # to be downloaded with the required file
+    if topspin:
+        savedpath = path
+        m = re.match(r"(.*)(\/pdata\/\d+\/\d+[r|i]{1,2}|ser|fid)", str(path))
+        if m is not None:
+            path = pathclean(m[1])
+
+    if _is_relative_to(path, datadir):
+        # try to make it relative for remote downloading on github
+        relative_path = _relative_to(path, datadir)
     else:
-        # download localy
-        dst = pathclean(path.split("/")[-1])
-        _download_from_url(path, dst, replace)
-
-    if not kwargs.pop("download_only", False):
-        read_method = kwargs.pop("read_method", read)
-        return read_method(dataset, dst, **kwargs)
-
-
-# ======================================================================================
-# Private functions
-# ======================================================================================
-@_importer_method
-def _read_dir(*args, **kwargs):
-    _, directory = args
-    directory = get_directory_name(directory)
-    files = get_filenames(directory, **kwargs)
-    datasets = []
-    valid_extensions = list(zip(*FILETYPES))[0] + list(zip(*ALIAS))[0]
-    for key in [key for key in files.keys() if key[1:] in valid_extensions]:
-        if key:
-            importer = Importer()
-            nd = importer(files[key], **kwargs)
-            if nd is not None:
-                if not isinstance(nd, list):
-                    nd = [nd]
-                datasets.extend(nd)
-    return datasets
-
-
-@_importer_method
-def _read_scp(*args, **kwargs):
-    dataset, filename = args
-    return dataset.load(filename, **kwargs)
-
-
-@_importer_method
-def _read_(*args, **kwargs):
-    dataset, filename = args
-
-    if kwargs.pop("remote", False):
-        return Importer._read_remote(*args, **kwargs)
-    elif not filename or filename.is_dir():
-        return Importer._read_dir(*args, **kwargs)
-
-    # protocol = kwargs.get("protocol", None)
-    # if protocol and ".scp" in protocol:
-    #     return dataset.load(filename, **kwargs)
-    #
-    # elif filename and filename.name in ("fid", "ser", "1r", "2rr", "3rrr"):
-    #     # probably an Topspin NMR file
-    #     return dataset.read_topspin(filename, **kwargs)
-    # elif filename:
-    #     # try scp format
-    #     try:
-    #         return dataset.load(filename, **kwargs)
-    #     except Exception:
-    #         # lets try some common format
-    #         for key in ["omnic", "opus", "topspin", "labspec", "matlab", "jdx"]:
-    #             try:
-    #                 _read = getattr(dataset, f"read_{key}")
-    #                 f = f"{filename}.{key}"
-    #                 return _read(f, **kwargs)
-    #             except Exception:
-    #                 pass
-    #         raise NotImplementedError
+        # assume it is already relative
+        relative_path = path
 
+    # Try to download it
+    dst = datadir / relative_path
+    if dst.name == "testdata":
+        # we are going to download the whole testdata directory
+        # -> use a faster method
+        _download_full_testdata_directory()
+        return
+    else:
+        content = _download_from_github(relative_path, dst, replace)
 
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
+    if not download_only:
+        if content is None:
+            if topspin:
+                return read_method(
+                    dataset, dst / _relative_to(savedpath, dst), **kwargs
+                )
+            else:
+                return read_method(dataset, dst, **kwargs)
+        else:
+            return read_method(dataset, dst, content=content, **kwargs)
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_carroucell.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_carroucell.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,69 +17,64 @@
 
 import numpy as np
 import scipy.interpolate
 import xlrd
 
 from spectrochempy.core import info_
 from spectrochempy.core.dataset.coord import Coord
-from spectrochempy.core.dataset.nddataset import NDDataset
 from spectrochempy.core.readers.importer import Importer, _importer_method
+from spectrochempy.core.readers.read_omnic import read_omnic
+from spectrochempy.utils.docstrings import _docstring
 from spectrochempy.utils.file import get_directory_name, get_filenames
 
+_docstring.delete_params("Importer.see_also", "read_carroucell")
 
+
+@_docstring.dedent
 def read_carroucell(directory=None, **kwargs):
     """
-    Open .spa files in a directory after a carroucell experiment.
+    Open :file:`.spa` files in a directory after a :term:`carroucell` experiment.
 
-    The files for a given sample are grouped in NDDatasets (sorted by acquisition date).
-    The NDDatasets are returned in a list sorted by sample number.
+    The files for a given sample are grouped in `NDDataset`\ s (sorted by
+    acquisition date).
+    The `NDDataset`\ s are returned in a list sorted by sample number.
     When the file containing the temperature data is present, the temperature is read
     and assigned as a label to each spectrum.
 
     Parameters
     ----------
-    directory : str, optional
+    directory : `str`, optional
         If not specified, opens a dialog box.
-    **kwargs
-        Optional keyword parameters. See Other Parameters.
+    %(kwargs)s
+
+    Returns
+    -------
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    spectra : arraylike of 2 int (min, max), optional, default=None
+    spectra : :term:`array-like` of 2 `int` (``min`` , ``max`` ), optional, default: `None`
         The first and last spectrum to be loaded as determined by their number.
-         If None all spectra are loaded.
-    discardbg : bool, optional, default=True
-        If True : do not load background (sample #9).
-    delta_clocks : int, optional, default=0
-        Difference in seconds between the clocks used for spectra and temperature acquisition.
-        Defined as t(thermocouple clock) - t(spectrometer clock).
-
-    Returns
-    --------
-    nddataset
-        `NDDataset` or list of `NDDataset` .
+        If `None` all spectra are loaded.
+    discardbg : `bool`, optional, default: `True`
+        If `True` : do not load background (sample #9).
+    delta_clocks : `int`, optional, default:  0
+        Difference in seconds between the clocks used for spectra and temperature
+        acquisition. Defined as ``t(thermocouple clock) - t(spectrometer clock)`` .
 
     See Also
     --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    %(Importer.see_also.no_read_carroucell)s
 
     Notes
     ------
     All files are expected to be present in the same directory and their filenames
-    are expected to be in the format : X_samplename_YYY.spa
-    and for the background files : X_BCKG_YYYBG.spa
-    where X is the sample holder number and YYY the spectrum number.
+    are expected to be in the format : :file:`X_samplename_YYY.spa`
+    and for the background files : :file:`X_BCKG_YYYBG.spa`
+    where ``X`` is the sample holder number and ``YYY`` the spectrum number.
 
     Examples
     --------
 
     >>> scp.read_carroucell("irdata/carroucell_samp")
     no temperature file
     [NDDataset: [float64] a.u. (shape: (y:6, x:11098)), NDDataset: ...
@@ -130,25 +125,23 @@
         spafiles += spafileback
 
     # merge dataset with the same number
     curfilelist = [spafiles[0]]
     curprefix = prefix(spafiles[0])
     for f in spafiles[1:]:
         if prefix(f) != curprefix:
-            ds = NDDataset.read_omnic(
+            ds = read_omnic(
                 curfilelist, sortbydate=True, directory=directory, name=curprefix
             )
             datasets.append(ds)
             curfilelist = [f]
             curprefix = prefix(f)
         else:
             curfilelist.append(f)
-    ds = NDDataset.read_omnic(
-        curfilelist, sortbydate=True, directory=directory, name=curprefix
-    )
+    ds = read_omnic(curfilelist, sortbydate=True, directory=directory, name=curprefix)
     datasets.append(ds)
 
     # Now manage temperature
     Tfile = sorted([f for f in os.listdir(directory) if f[-4:].lower() == ".xls"])
     if len(Tfile) == 0:
         info_("no temperature file")
     elif len(Tfile) > 1:
@@ -197,11 +190,7 @@
                 ds.y = Coord(title=ds.y.title, data=ds.y.data, labels=newlabels)
 
     if len(datasets) == 1:
         return datasets[0]  # a single dataset is returned
 
     # several datasets returned, sorted by sample #
     return sorted(datasets, key=lambda ds: re.split("-|_", ds.name)[0])
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_csv.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_csv.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 __all__ = ["read_csv"]
 __dataset_methods__ = __all__
 
+import csv
+
 # --------------------------------------------------------------------------------------
 # standard and other imports
 # --------------------------------------------------------------------------------------
-import io
 import locale
 import warnings
 from datetime import datetime
 
 import numpy as np
 
 from spectrochempy.core import preferences as prefs
 from spectrochempy.core.dataset.coord import Coord
-from spectrochempy.core.readers.importer import Importer, _importer_method
+from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
+from spectrochempy.utils.docstrings import _docstring
 
 try:
     locale.setlocale(locale.LC_ALL, "en_US")  # to avoid problems with date format
 except Exception:  # pragma: no cover
     try:
         locale.setlocale(
             locale.LC_ALL, "en_US.utf8"
@@ -31,172 +33,132 @@
     except Exception:
         warnings.warn("Could not set locale: en_US or en_US.utf8")
 
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_csv")
+
+
+@_docstring.dedent
 def read_csv(*paths, **kwargs):
     """
-    Open a \*.csv file or a list of \*.csv files.
+    Open a :file:`.csv` file or a list of :file:`.csv` files.
 
     This is limited to 1D array - csv file must have two columns [index, data]
     without header.
 
     Parameters
     ----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_csv
-        `NDDataset` or list of `NDDataset` .
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
-        A Custom description.
-    origin : {'omnic', 'tga'}, optional
-        in order to properly interpret CSV file it can be necessary to set the origin of the spectra.
-        Up to now only 'omnic' and 'tga' have been implemented.
-    csv_delimiter : str, optional
-        Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy `Preferences` .
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    %(Importer.other_parameters)s
 
     See Also
     --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_spa : Read Omnic \*.Spa single spectra.
-    read_srs : Read Omnic series.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
-    read : Generic file reading.
+    %(Importer.see_also.no_read_csv)s
 
     Examples
     ---------
 
     >>> scp.read_csv('agirdata/P350/TGA/tg.csv')
     NDDataset: [float64] unitless (shape: (y:1, x:3247))
 
     Additional information can be stored in the dataset if the origin is given
     (known origin for now : tga or omnic)
     # TODO: define some template to allow adding new origins
 
-    >>> scp.read_csv('agirdata/P350/TGA/tg.csv', origin='tga')
-    NDDataset: [float64] wt.% (shape: (y:1, x:3247))
+    >>> A = scp.read_csv('agirdata/P350/TGA/tg.csv', origin='tga')
 
     Sometimes the delimiteur needs to be adjusted
 
     >>> prefs = scp.preferences
-    >>> scp.read_csv('irdata/IR.CSV', directory=prefs.datadir, origin='omnic', csv_delimiter=',')
-    NDDataset: [float64] a.u. (shape: (y:1, x:3736))
+    >>> B = scp.read_csv('irdata/IR.CSV', origin='omnic', csv_delimiter=',')
     """
     kwargs["filetypes"] = ["CSV files (*.csv)"]
     kwargs["protocol"] = ["csv"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 # ======================================================================================
 # Private functions
 # ======================================================================================
 @_importer_method
 def _read_csv(*args, **kwargs):
     # read csv file
     dataset, filename = args
-    content = kwargs.get("content", None)
     delimiter = kwargs.get("csv_delimiter", prefs.csv_delimiter)
 
-    def _open():
-        if content is not None:
-            f = io.StringIO(content.decode("utf-8"))
-        else:
-            f = open(filename, "r")
-        return f
+    fid, kwargs = _openfid(filename, mode="r", **kwargs)
 
-    try:
-        fid = _open()
-        d = np.loadtxt(fid, unpack=True, delimiter=delimiter)
-        fid.close()
-    except ValueError:
-        # it might be that the delimiter is not correct (default is ','), but
-        # french excel export with the french locale for instance, use ";".
-        _delimiter = ";"
-        try:
-            fid = _open()
-            if fid:
-                fid.close()
-            fid = _open()
-            d = np.loadtxt(fid, unpack=True, delimiter=_delimiter)
-            fid.close()
-
-        except Exception:  # pragma: no cover
-            # in french, very often the decimal '.' is replaced by a
-            # comma:  Let's try to correct this
-            if fid:
-                fid.close()
-            if not isinstance(fid, io.StringIO):
-                with open(fid, "r") as fid_:
-                    txt = fid_.read()
-            else:
-                txt = fid.read()
-            txt = txt.replace(",", ".")
-            fil = io.StringIO(txt)
-            try:
-                d = np.loadtxt(fil, unpack=True, delimiter=delimiter)
-            except Exception:
-                raise IOError(
-                    "{} is not a .csv file or its structure cannot be recognized"
-                )
+    txt = fid.read()
+    fid.close()
+
+    # We assume this csv file contains only numbers # TODO: write a more general reader
+    if ";" in txt:
+        # look like the delimiter is ;
+        # if comma is also present, it could be that french writer was used.
+        txt = txt.replace(",", ".")
+        delimiter = ";"
+
+    d = [row for row in csv.reader(txt.splitlines(), delimiter=delimiter)]
+    d = np.array(d).T
 
     # First column is the x coordinates
     coordx = Coord(d[0])
 
-    # create a second coordinate for dimension y of size 1
+    # Create a second coordinate for dimension y of size 1
     coordy = Coord([0])
 
     # and data is the second column -  we make it a vector
     data = d[1].reshape((1, coordx.size))
 
-    # update the dataset
+    # try:
+    #     d = np.loadtxt(fid, unpack=True, delimiter=delimiter)
+    #     fid.close()
+    #
+    # except ValueError:
+    #     # it might be that the delimiter is not correct (default is ','), but
+    #     # french excel export with the french locale for instance, use ";".
+    #     _delimiter = ";"
+    #     try:
+    #         if fid:
+    #             fid.close()
+    #         fid, kwargs = _openfid(filename, mode="r", **kwargs)
+    #         d = np.loadtxt(fid, unpack=True, delimiter=_delimiter)
+    #         fid.close()
+    #
+    #     except Exception:  # pragma: no cover
+    #         # in french, very often the decimal '.' is replaced by a
+    #         # comma:  Let's try to correct this
+    #         if fid:
+    #             fid.close()
+    #         fid, kwargs = _openfid(filename, mode="r", **kwargs)
+    #         txt = fid.read()
+    #         fid.close()
+    #
+    #         txt = txt.replace(",", ".")
+    #
+    #         fid = io.StringIO(txt)
+    #         try:
+    #             d = np.loadtxt(fid, unpack=True, delimiter=delimiter)
+    #         except Exception:
+    #             raise IOError(
+    #                 "{} is not a .csv file or its structure cannot be recognized"
+    #             )
+
+    # Update the dataset
     dataset.data = data
     dataset.set_coordset(y=coordy, x=coordx)
 
     # set the additional attributes
     name = filename.stem
     dataset.filename = filename
     dataset.name = kwargs.get("name", name)
@@ -280,12 +242,7 @@
     dataset.x.units = "hour"
     dataset.units = "weight_percent"
     dataset.x.title = "time-on-stream"
     dataset.title = "mass change"
     dataset.origin = "tga"
 
     return dataset
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_jcamp.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_jcamp.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,100 +4,56 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 This module to extend NDDataset with the import methods.
 """
 
-__all__ = ["read_jcamp", "read_jdx", "read_dx"]
+__all__ = ["read_jcamp"]
 __dataset_methods__ = __all__
 
 import io
 import re
 from datetime import datetime, timezone
 
 import numpy as np
 
 from spectrochempy.core.dataset.coord import Coord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.utils.decorators import deprecated
-
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_jcamp")
+
+
+@_docstring.dedent
 def read_jcamp(*paths, **kwargs):
     """
-    Open Infrared JCAMP-DX files with extension ` .jdx` or ` .dx` .
+    Open Infrared ``JCAMP-DX`` files with extension :file:`.jdx` or :file:`.dx`\ .
 
-    Limited to AFFN encoding (see R. S. McDonald and Paul A. Wilks,
-    JCAMP-DX: A Standard Form for Exchange of Infrared Spectra in Computer Readable Form,
-    Appl. Spec., 1988, 1, 151–162. doi:10.1366/0003702884428734.)
+    Limited to AFFN encoding (see :cite:t:`mcdonald:1988`\ )
 
     Parameters
     ----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_jcamp
-        `NDDataset` or list of `NDDataset` .
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whnever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    %(Importer.other_parameters)s
 
     See Also
     ---------
-    read : Generic read method.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    %(Importer.see_also.no_read_jcamp)s
     """
     kwargs["filetypes"] = ["JCAMP-DX files (*.jdx *.dx)"]
     kwargs["protocol"] = ["jcamp"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
@@ -384,12 +340,7 @@
             text = ""
         else:  # keyword + text
             keyword, text = line.split("=")
     else:
         keyword = ""
         text = line.strip()
     return keyword, text
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_labspec.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_labspec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,107 +1,58 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-"""
+r"""
 This module extend NDDataset with the import method for Labspec \*.txt generated data files.
 """
 
 __all__ = ["read_labspec"]
 __dataset_methods__ = __all__
 
 import datetime
 
 import numpy as np
 
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.dataset.coord import Coord, LinearCoord
 from spectrochempy.core.readers.importer import Importer, _importer_method
-
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_labspec")
+
+
+@_docstring.dedent
 def read_labspec(*paths, **kwargs):
     """
     Read a single Raman spectrum or a series of Raman spectra.
 
-    Files to open are .txt file created by Labspec software. Non-labspec .txt files
-    are ignored (return None)
+    Files to open are :file:`.txt` file created by ``Labspec`` software.
+    Non-labspec :file:`.txt` files are ignored (return None)
 
     Parameters
     ----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the
-        file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no
-        `filename` , nor `content` ), a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    %(Importer.parameters)s
 
     Returns
     --------
-    read
-        `NDDataset` or list of `NDDataset` or None.
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whnever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the
-        default `datadir` specified in SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as
-        arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False)
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True)
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be
-        directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly
-        useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory`
-        are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol
-        (default=True)
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also.no_read_labspec)s
 
     Examples
     --------
     >>> A = scp.read_labspec('ramandata/Activation.txt')
     """
 
     kwargs["filetypes"] = ["LABSPEC exported files (*.txt)"]
@@ -120,18 +71,15 @@
 def _read_txt(*args, **kwargs):
     # read Labspec *txt files or series
 
     dataset, filename = args
     content = kwargs.get("content", False)
 
     if content:
-        pass
-        # fid = io.StringIO(content)
-        # TODO: get the l list of string
-
+        lines = content.decode("utf-8").splitlines()
     else:
         fid = open(filename, "r", encoding="utf-8")
         try:
             lines = fid.readlines()
         except UnicodeDecodeError:
             fid = open(filename, "r", encoding="latin-1")
             lines = fid.readlines()
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_matlab.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_matlab.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,102 +7,61 @@
 """
 Plugin module to extend NDDataset with the import methods method.
 """
 
 __all__ = ["read_matlab", "read_mat"]
 __dataset_methods__ = __all__
 
-import io
 from datetime import datetime
-from warnings import warn
 
 import numpy as np
 import scipy.io as sio
 
+from spectrochempy.application import info_, warning_
 from spectrochempy.core.dataset.nddataset import Coord, NDDataset
-from spectrochempy.core.readers.importer import Importer, _importer_method
-
+from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_matlab")
+
+
+@_docstring.dedent
 def read_matlab(*paths, **kwargs):
     """
-    Read a matlab file with extension ` .mat` and return its content as a list.
+    Read a matlab file with extension :file:`.mat` and return its content as a list.
 
-    The array of numbers (i.e. matlab matrices) and Eigenvector's DataSet Object (DSO, see
-    `DSO <https://www.eigenvector.com/software/dataset.htm>`_ ) are returned as NDDatasets.  The
-    content not recognized by SpectroChemPy is returned as a tuple (name, object).
+    The array of numbers (*i.e.,* matlab matrices) and Eigenvector's DataSet Object
+    (``DSO``, see `DSO <https://www.eigenvector.com/software/dataset.htm>`__ ) are
+    returned as NDDatasets.  The content not recognized by SpectroChemPy is returned
+    as a tuple (name, object).
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_matlab
-        `NDDataset` or list of `NDDataset` .
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whnever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False)
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the `tests/tests_readers` directory
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol (default=True)
-    recursive : bool, optional
-        Read also in subfolders. (default=False)
+    %(Importer.other_parameters)s
+
+    See Also
+    ---------
+    %(Importer.see_also.no_read_matlab)s
 
     Examples
     ---------
 
     >>> scp.read_matlab('matlabdata/dso.mat')
     NDDataset: [float64] unitless (shape: (y:20, x:426))
-
-    See `read_omnic` for more examples of use
-    See Also
-    --------
-    read : Read generic files.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic .spg grouped spectra.
-    read_spa : Read Omnic .spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
     """
     kwargs["filetypes"] = ["MATLAB files (*.mat *.dso)"]
     kwargs["protocol"] = ["matlab", "mat", "dso"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
@@ -111,20 +70,16 @@
 
 # --------------------------------------------------------------------------------------
 # Private methods
 # --------------------------------------------------------------------------------------
 @_importer_method
 def _read_mat(*args, **kwargs):
     _, filename = args
-    content = kwargs.get("content", False)
 
-    if content:
-        fid = io.BytesIO(content)
-    else:
-        fid = open(filename, "rb")
+    fid, kwargs = _openfid(filename, **kwargs)
 
     dic = sio.loadmat(fid)
 
     datasets = []
     for name, data in dic.items():
 
         dataset = NDDataset()
@@ -153,28 +108,28 @@
             dataset.history = "Imported from .mat file"
             # TODO: reshape from fortran/Matlab order to C opder
             # for 3D or higher datasets ?
             datasets.append(dataset)
 
         elif data.dtype.char == "U":
             # this is an array of string
-            warn(
+            info_(
                 f"The mat file contains an array of strings named '{name}' which will not be converted to NDDataset"
             )
             continue
 
         elif all(
             name_ in data.dtype.names for name_ in ["moddate", "axisscale", "imagesize"]
         ):
             # this is probably a DSO object
             dataset = _read_dso(dataset, name, data)
             datasets.append(dataset)
 
         else:
-            warn(f"unsupported data type : {data.dtype}")
+            warning_(f"unsupported data type : {data.dtype}")
             # TODO: implement DSO reader
             datasets.append([name, data])
 
     return datasets
 
 
 @_importer_method
@@ -279,12 +234,7 @@
             dataset.description += i
 
         for i in data["history"][0][0][0][0]:
             dataset.history = i
 
         dataset.history = "Imported by spectrochempy."
     return dataset
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_omnic.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_omnic.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,110 +17,63 @@
 from datetime import datetime, timedelta, timezone
 
 import numpy as np
 
 from spectrochempy.core import info_
 from spectrochempy.core.dataset.coord import Coord, LinearCoord
 from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.core.readers.importer import Importer, _importer_method
+from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import ur
-
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_omnic")
+
+
+@_docstring.dedent
 def read_omnic(*paths, **kwargs):
     """
     Open a Thermo Nicolet OMNIC file.
 
-    Open Omnic file or a list of files with extension ` .spg` , ` .spa` or
-    ` .srs` and set data/metadata in the current dataset.
+    Open Omnic file or a list of :file:`.spg`\ , :file:`.spa` or
+    :file:`.srs` files and set data/metadata in the current dataset.
 
     The collected metadata are:
     - names of spectra
     - acquisition dates (UTC)
     - units of spectra (absorbance, transmittance, reflectance, Log(1/R),
     Kubelka-Munk, Raman intensity, photoacoustics, volts)
-    - units of xaxis (wavenumbers in cm^-1, wavelengths in nm or micrometer,
-    Raman shift in cm^-1)
+    - units of xaxis (wavenumbers in :math:`cm^{-1}`, wavelengths in nm or micrometer,
+    Raman shift in :math:`cm^{-1}`)
     - spectra history (but only incorporated in the NDDataset if a single
     spa is read)
 
     An error is generated if attempt is made to inconsistent datasets: units
-    of spectra and
-    xaxis, limits and number of points of the xaxis.
+    of spectra and xaxis, limits and number of points of the xaxis.
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name
-        for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    out
-        The dataset or a list of dataset corresponding to a (set of) .spg,
-        .spa or .srs file(s).
+    %(Importer.returns)s
 
     Other Parameters
-    -----------------
-    directory : str, optional
-        From where to read the specified `filename` . If not specified,
-        read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been
-        provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description : str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content
-        can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is
-        particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided
-        `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    ----------------
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_dir : Read a set of data from a directory.
-    read_spg : Read Omnic files .spg.
-    read_spa : Read Omnic files .spa.
-    read_srs : Read Omnic files .srs.
-    read_opus : Read Bruker OPUS files.
-    read_topspin : Read TopSpin NMR files.
-    read_csv : Read .csv.
-    read_matlab : Read MATLAB files .mat.
-    read_zip : Read zipped group of files.
+    ---------
+    read_spg : Read grouped Omnic spectra.
+    read_spa : Read single Omnic spectra.
+    read_srs : Read series Omnic spectra.
+    %(Importer.see_also.no_read_omnic)s
 
     Examples
     ---------
     Reading a single OMNIC file  (providing a windows type filename relative
     to the default `datadir` )
 
     >>> scp.read_omnic('irdata\\\\nh4y-activation.spg')
@@ -209,192 +162,81 @@
 
     kwargs["filetypes"] = ["OMNIC files (*.spa *.spg)", "OMNIC series (*.srs)"]
     kwargs["protocol"] = ["omnic", "spa", "spg", "srs"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
+@_docstring.dedent
 def read_spg(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ` .spg` .
-
-    Open Omnic file or a list of files with extension ` .spg` and set
-    data/metadata in the current dataset.
+    Open a Thermo Nicolet file or a list of files with extension ``.spg``\ .
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name
-        for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_spg
-        The dataset or a list of dataset corresponding to a (set of) .spg
-        file(s).
+    %(Importer.returns)s
 
     Other Parameters
-    -----------------
-    directory : str, optional
-        From where to read the specified `filename` . If not specified,
-        read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been
-        provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description : str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content
-        can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is
-        particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided
-        `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    ----------------
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_dir : Read a set of data from a directory.
-    read_omnnic : Read Omnic files.
-    read_spa : Read Omnic files .spa.
-    read_srs : Read Omnic files .srs.
-    read_opus : Read Bruker OPUS files.
-    read_topspin : Read TopSpin NMR files.
-    read_csv : Read .csv.
-    read_matlab : Read MATLAB files .mat.
-    read_zip : Read zipped group of files.
+    ---------
+    read_spg : Read grouped Omnic spectra.
+    read_spa : Read single Omnic spectra.
+    read_srs : Read series Omnic spectra.
+    %(Importer.see_also.no_read_omnic)s
 
     Notes
     -----
     This method is an alias of `read_omnic`\ , except that the type of file
-    is contrain to *.spg.
+    is contrain to ``.spg``.
 
     Examples
     ---------
 
     >>> scp.read_spg('irdata/nh4y-activation.spg')
     NDDataset: [float64] a.u. (shape: (y:55, x:5549))
     """
 
     kwargs["filetypes"] = ["OMNIC files (*.spg)"]
     kwargs["protocol"] = ["spg", "spa"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
+@_docstring.dedent
 def read_spa(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ` .spa` .
-
-    Open Omnic file or a list of files with extension ` .spa` and set
-    data/metadata in the current dataset.
+    Open a Thermo Nicolet file or a list of files with extension ``.spa``\ .
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name
-        for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_spa
-        The dataset or a list of dataset corresponding to the (set of) .spa
-        file(s).
+    %(Importer.returns)s
 
     Other Parameters
-    -----------------
-    return_ifg : str or None, optional
-        Default value is None. When set to 'sample' returns the sample interferogram
-        of the spa file if present or None if absent. When set to 'backgroung' returns
-        the backgroung interferogram of the spa file if present or None if absent.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified,
-        read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been
-        provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content
-        can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is
-        particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided
-        `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    ----------------
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also)s
 
     Notes
     -----
     This method is an alias of `read_omnic`\ , except that the type of file
-    is contrain to *.spa.
+    is contrain to ``.spa``\ .
 
     Examples
     ---------
 
     >>> scp.read_spa('irdata/subdir/20-50/7_CZ0-100 Pd_21.SPA')
     NDDataset: [float64] a.u. (shape: (y:1, x:5549))
     >>> scp.read_spa(directory='irdata/subdir', merge=True)
@@ -403,96 +245,42 @@
 
     kwargs["filetypes"] = ["OMNIC files (*.spa)"]
     kwargs["protocol"] = ["spa"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
+@_docstring.dedent
 def read_srs(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension `.srs` .
-
-    Open Omnic file or a list of files with extension `.srs` and set
-    data/metadata in the current dataset.
+    Open a Thermo Nicolet file or a list of files with extension ``.srs`` .
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name
-        for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    NDDataset
-        The dataset or a list of dataset corresponding to a (set of) series
-        or backgroun files.
+    %(Importer.returns)s
+        When return_bg is set to 'True', the series background is returned.
 
     Other Parameters
-    -----------------
+    ----------------
     return_bg : bool, optional
         Default value is False. When set to 'True' returns the series background
-    directory : str, optional
-        From where to read the specified `filename` . If not specified,
-        read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been
-        provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content
-        can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is
-        particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided
-        `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol (default=True)
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_spa : Read Omnic \*.Spa single spectra.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also)s
 
     Notes
     -----
     This method is an alias of `read_omnic`\ , except that the type of file
-    is constrained to *.srs.
+    is constrained to ``.srs``\ .
 
     Examples
     ---------
     >>> scp.read_srs('irdata/omnic_series/rapid_scan_reprocessed.srs')
     NDDataset: [float64] a.u. (shape: (y:643, x:3734))
     """
 
@@ -506,26 +294,22 @@
 # Private functions
 # ======================================================================================
 @_importer_method
 def _read_spg(*args, **kwargs):
     # read spg file
 
     dataset, filename = args
-    sortbydate = kwargs.pop("sortbydate", True)
-    content = kwargs.get("content", False)
 
-    if content:
-        fid = io.BytesIO(content)
-    else:
-        fid = open(filename, "rb")
+    fid, kwargs = _openfid(filename, **kwargs)
 
     # Read name:
     # The name starts at position hex 1e = decimal 30. Its max length
     # is 256 bytes. It is the original filename under which the group has been saved: it
-    # won't match with the actual filename if a subsequent renaming has been done in the OS.
+    # won't match with the actual filename if a subsequent renaming has been done in the
+    # OS.
 
     spg_title = _readbtext(fid, 30, 256)
 
     # Count the number of spectra
     # From hex 120 = decimal 304, individual spectra are described
     # by blocks of lines starting with "key values",
     # for instance hex[02 6a 6b 69 1b 03 82] -> dec[02 106  107 105 27 03 130]
@@ -649,15 +433,15 @@
 
     # Read spectra titles and acquisition date
     for i in range(nspec):
         # determines the position of informatioon
         fid.seek(position6B[i] + 2)  # go to line and skip 2 bytes
         spa_title_pos = _fromfile(fid, "uint32", 1)
 
-        # read filename
+        # read omnic filename
         spa_title = _readbtext(fid, spa_title_pos, 256)
         spectitles.append(spa_title)
 
         # and the acquisition date
         fid.seek(spa_title_pos + 256)
         timestamp = _fromfile(fid, dtype="uint32", count=1)
         # since 31/12/1899, 00:00
@@ -728,32 +512,29 @@
     dataset.description = kwargs.get(
         "description", f"Omnic title: {spg_title}\nOmnic " f"filename: {filename}"
     )
 
     dataset._date = datetime.now(timezone.utc)
 
     dataset.history = f"Imported from spg file {filename}."
-    if sortbydate:
+
+    if kwargs.pop("sortbydate", True):
         dataset.sort(dim="y", inplace=True)
         dataset.history = "Sorted by date"
 
     # debug_("end of reading")
 
     return dataset
 
 
 @_importer_method
 def _read_spa(*args, **kwargs):
     dataset, filename = args
-    content = kwargs.get("content", False)
 
-    if content:
-        fid = io.BytesIO(content)
-    else:
-        fid = open(filename, "rb")
+    fid, kwargs = _openfid(filename, **kwargs)
 
     return_ifg = kwargs.get("return_ifg", None)
 
     # Read name:
     # The name  starts at position hex 1e = decimal 30. Its max length
     # is 256 bytes. It is the original filename under which the spectrum has
     # been saved: it won't match with the actual filename if a subsequent
@@ -1431,12 +1212,7 @@
     fid.seek(pos + 6)
     intensity_size = _fromfile(fid, "uint32", 1)
     nintensities = int(intensity_size / 4)
 
     # Read and return spectral intensities
     fid.seek(intensity_pos)
     return _fromfile(fid, "float32", int(nintensities))
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_spc.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_spc.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,103 +6,52 @@
 # ======================================================================================
 """
 This module extend NDDataset with the import method for Thermo galactic (spc) data files.
 """
 __all__ = ["read_spc"]
 __dataset_methods__ = __all__
 
-import io
 import struct
 from datetime import datetime
 from warnings import warn
 
 import numpy as np
 
 from spectrochempy.core.dataset.coord import Coord, LinearCoord
 from spectrochempy.core.dataset.nddataset import NDDataset
-from spectrochempy.core.readers.importer import Importer, _importer_method
+from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
 from spectrochempy.core.units import Quantity
-
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
-# Public function
+# Public functions
 # ======================================================================================
+_docstring.delete_params("Importer.see_also", "read_spc")
+
+
+@_docstring.dedent
 def read_spc(*paths, **kwargs):
     """
-    Open a Thermo Nicolet file or a list of files with extension ` .spg` .
+    Read GRAMS/Thermo Scientific Galactic files or a list of files with extension :file:`.spc`\ .
 
     Parameters
-    -----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name
-        for the file(s) to be loaded:
-
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
-
-        If the list of filenames are enclosed into brackets:
-
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
-
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e.
-        no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_spc
-        The dataset or a list of dataset corresponding to a (set of) .spa
-        file(s).
+    %(Importer.returns)s
 
     Other Parameters
-    -----------------
-    directory : str, optional
-        From where to read the specified `filename` . If not specified,
-        read in the default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been
-        provided as arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: str, optional
-        A Custom description.
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content
-        can be directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is
-        particularly useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided
-        `directory` are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol (default=True).
-    recursive : bool, optional
-        Read also in subfolders. (default=False).
+    ----------------
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read : Generic read method.
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spa : Read Omnic \*.spa spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also.no_read_spc)s
 
     Examples
     ---------
     >>> scp.read_spc("galacticdata/BENZENE.spc")
     NDDataset: [float64] a.u. (shape: (y:1, x:1842))
     """
 
@@ -114,21 +63,18 @@
 
 # ======================================================================================
 # Private functions
 # ======================================================================================
 @_importer_method
 def _read_spc(*args, **kwargs):
     dataset, filename = args
-    content = kwargs.get("content", False)
 
-    if content:
-        fid = io.BytesIO(content)
-    else:
-        fid = open(filename, "rb")
-        content = fid.read()
+    fid, kwargs = _openfid(filename, **kwargs)
+
+    content = fid.read()
 
     # extract version
     _, Fversn = struct.unpack("cc".encode("utf8"), content[:2])
 
     # check spc version
     if Fversn == b"\x4b":
         endian = "little"
@@ -582,12 +528,7 @@
         dataset.x.set_laser_frequency()
         dataset.x._use_time_axis = (
             False  # True to have time, else it will be optical path difference
         )
 
     fid.close()
     return dataset
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_topspin.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_topspin.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
 """
 Bruker file (single dimension FID or multidimensional SER) importers.
 """
 
-__all__ = ["read_topspin", "read_bruker_nmr"]
+__all__ = ["read_topspin"]
 __dataset_methods__ = __all__
 
 import re
 
 import numpy as np
 from quaternion import as_quat_array
 
 from spectrochempy.core import debug_
 from spectrochempy.core.dataset.baseobjects.meta import Meta
 from spectrochempy.core.dataset.coord import LinearCoord
 from spectrochempy.core.readers.importer import Importer, _importer_method
 from spectrochempy.core.units import ur
 from spectrochempy.extern.nmrglue import read_fid, read_pdata
-from spectrochempy.utils.decorators import deprecated
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Constants
 # ======================================================================================
 FnMODE = ["undefined", "QF", "QSEQ", "TPPI", "STATES", "STATES-TPPI", "ECHO-ANTIECHO"]
 AQ_mod = ["QF", "QSIM", "QSEQ", "DQD"]
 
@@ -693,103 +693,55 @@
 #     else:
 #         return scal()
 
 
 # ======================================================================================
 # Bruker topspin import function
 # ======================================================================================
+
+_docstring.delete_params("Importer.see_also", "read_topspin")
+
+
+@_docstring.dedent
 def read_topspin(*paths, **kwargs):
     """
     Open Bruker TOPSPIN (NMR) dataset.
 
     Parameters
     ----------
     *paths : str, optional
         Paths of the Bruker directories to read.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    %(kwargs)s
 
     Returns
     --------
-    read_topspin
-        `NDDataset` or list of `NDDataset` .
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    expno : int, optional
-        experiment number.
-    procno : int
-        processing number.
-    protocol : {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}, optional
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whnever it is possible) from the file name extension.
-    directory : str, optional
-        From where to read the specified `filename` . If not specified, read in the
-        default `datadir` specified in
-        SpectroChemPy Preferences.
-    merge : bool, optional
-        Default value is False. If True, and several filenames have been provided as
-        arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : bool, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description : str, optional
-        A Custom description.
-    origin : {'omnic', 'tga'}, optional
-        In order to properly interpret CSV file it can be necessary to set the origin
-        of the spectra.
-        Up to now only 'omnic' and 'tga' have been implemented.
-    csv_delimiter : str, optional
-        Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy `Preferences` .
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be
-        directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly
-        useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        `tests/tests_readers` directory.
-    listdir : bool, optional
-        If True and filename is None, all files present in the provided `directory` are
-        returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current reading protocol
-        (default=True)
-    recursive : bool, optional
-        Read also in subfolders. (default=False)
+    expno : `int`\ , optional
+        Experiment number.
+    procno : `int`\ , optional
+        Processing number.
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_spa : Read Omnic \*.Spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also.no_read_topspin)s
     """
 
     kwargs["filetypes"] = [
         "Bruker TOPSPIN fid's or processed data files (fid ser 1[r|i] 2[r|i]* 3[r|i]*)",
         "Compressed TOPSPIN data directories (*.zip)",
     ]
     kwargs["protocol"] = ["topspin"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
-@deprecated(replace="read_topspin")
-def read_bruker_nmr(*args, **kwargs):
-    return read_topspin(*args, **kwargs)
-
-
 def _get_files(path, typ="acqu"):
     files = []
     for i in ["", 2, 3]:
         f = path / f"{typ}{i}"
         if f.exists():
             files.append(f)
         f = path / f"{typ}{i}s"
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/readers/read_zip.py` & `spectrochempy-0.6.2/spectrochempy/core/readers/read_opus.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,201 +1,201 @@
 # -*- coding: utf-8 -*-
 # ======================================================================================
 # Copyright (©) 2015-2023 LCS - Laboratoire Catalyse et Spectrochimie, Caen, France.
 # CeCILL-B FREE SOFTWARE LICENSE AGREEMENT
 # See full LICENSE agreement in the root directory.
 # ======================================================================================
-__all__ = ["read_zip"]
+"""
+This module extend NDDataset with the import method for OPUS generated data files.
+"""
+__all__ = ["read_opus"]
 __dataset_methods__ = __all__
 
-import io
+from datetime import datetime, timedelta, timezone
 
-from spectrochempy.core.readers.importer import Importer, _importer_method
+import numpy as np
+from brukeropusreader.opus_parser import parse_data, parse_meta
 
+from spectrochempy.core import debug_
+from spectrochempy.core.dataset.coord import Coord, LinearCoord
+from spectrochempy.core.readers.importer import Importer, _importer_method, _openfid
+from spectrochempy.utils.docstrings import _docstring
 
 # ======================================================================================
 # Public functions
 # ======================================================================================
-def read_zip(*paths, **kwargs):
-    """
-    Open a zipped list of data files.
-
-    Parameters
-    ----------
-    *paths : str, pathlib.Path object, list of str, or list of pathlib.Path objects, optional
-        The data source(s) can be specified by the name or a list of name for the
-        file(s) to be loaded:
+_docstring.delete_params("Importer.see_also", "read_opus")
 
-        *e.g.,( file1, file2, ...,  \*\*kwargs )*
 
-        If the list of filenames are enclosed into brackets:
+@_docstring.dedent
+def read_opus(*paths, **kwargs):
+    """
+    Open Bruker OPUS file(s).
 
-        *e.g.,* ( **[** *file1, file2, ...* **]**, \*\*kwargs *)*
+    Eventually group them in a single dataset. Only Absorbance spectra are
+    extracted ("AB" field). Returns an error if dimensions are incompatibles.
 
-        The returned datasets are merged to form a single dataset,
-        except if `merge` is set to False. If a source is not provided (i.e. no `filename` , nor `content` ),
-        a dialog box will be opened to select files.
-    **kwargs
-        Optional keyword parameters (see Other Parameters).
+    Parameters
+    ----------
+    %(Importer.parameters)s
 
     Returns
     --------
-    read_zip
-        `NDDataset` or list of `NDDataset` .
+    %(Importer.returns)s
 
     Other Parameters
     ----------------
-    protocol : 'str'\ , optional
-        One of {'scp', 'omnic', 'opus', 'topspin', 'matlab', 'jcamp', 'csv', 'excel'}
-        Protocol used for reading. If not provided, the correct protocol
-        is inferred (whenever it is possible) from the file name extension.
-    directory : `str`\ , optional
-        From where to read the specified `filename`\ . If not specified, read in the
-        default ``datadir`` specified in
-        SpectroChemPy Preferences.
-    merge : `bool`, optional
-        Default value is False. If True, and several filenames have been provided as
-        arguments,
-        then a single dataset with merged (stacked along the first
-        dimension) is returned (default=False).
-    sortbydate : `bool`, optional
-        Sort multiple spectra by acquisition date (default=True).
-    description: `str`\ , optional
-        A Custom description.
-    origin : {'omnic', 'tga'}, optional
-        in order to properly interpret CSV file it can be necessary to set the origin
-        of the spectra.
-        Up to now only 'omnic' and 'tga' have been implemented.
-    csv_delimiter : str, optional
-        Set the column delimiter in CSV file.
-        By default it is the one set in SpectroChemPy `Preferences` .
-    content : bytes object, optional
-        Instead of passing a filename for further reading, a bytes content can be
-        directly provided as bytes objects.
-        The most convenient way is to use a dictionary. This feature is particularly
-        useful for a GUI Dash application
-        to handle drag and drop of files into a Browser.
-        For examples on how to use this feature, one can look in the
-        ``tests/tests_readers`` directory.
-    listdir : `bool`, optional, default: `True`
-        If `True` and filename is None, all files present in the provided `directory`
-        are returned (and merged if `merge`
-        is True. It is assumed that all the files correspond to current
-        reading protocol.
-    recursive : bool, optional, default=False
-        Read also in subfolders.
+    %(Importer.other_parameters)s
 
     See Also
-    --------
-    read_topspin : Read TopSpin Bruker NMR spectra.
-    read_omnic : Read Omnic spectra.
-    read_opus : Read OPUS spectra.
-    read_labspec : Read Raman LABSPEC spectra.
-    read_spg : Read Omnic \*.spg grouped spectra.
-    read_spa : Read Omnic \*.Spa single spectra.
-    read_srs : Read Omnic series.
-    read_csv : Read CSV files.
-    read_zip : Read Zip files.
-    read_matlab : Read Matlab files.
+    ---------
+    %(Importer.see_also.no_read_opus)s
 
     Examples
-    --------
+    ---------
+    Reading a single OPUS file  (providing a windows type filename relative to
+    the default `datadir` )
+
+    >>> scp.read_opus('irdata\\\\OPUS\\\\test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+
+    Reading a single OPUS file  (providing a unix/python type filename relative to the
+    default `datadir` )
+    Note that here read_opus is called as a classmethod of the NDDataset class
+
+    >>> scp.NDDataset.read_opus('irdata/OPUS/test.0000')
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+
+    Single file specified with pathlib.Path object
+
+    >>> from pathlib import Path
+    >>> folder = Path('irdata/OPUS')
+    >>> p = folder / 'test.0000'
+    >>> scp.read_opus(p)
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
+
+    Multiple files not merged (return a list of datasets). Note that a directory is
+    specified
+
+    >>> le = scp.read_opus('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS')
+    >>> len(le)
+    3
+    >>> le[0]
+    NDDataset: [float64] a.u. (shape: (y:1, x:2567))
 
-    >>> A = scp.read_zip('agirdata/P350/FTIR/FTIR.zip', only=50, origin='omnic')
-    >>> print(A)
-    NDDataset: [float64]  a.u. (shape: (y:50, x:2843))
+    Multiple files merged as the `merge` keyword is set to true
+
+    >>> scp.read_opus('test.0000', 'test.0001', 'test.0002', directory='irdata/OPUS', merge=True)
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
+
+    Multiple files to merge : they are passed as a list instead of using the keyword `
+    merge`
+
+    >>> scp.read_opus(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS')
+    NDDataset: [float64] a.u. (shape: (y:3, x:2567))
+
+    Multiple files not merged : they are passed as a list but `merge` is set to false
+
+    >>> le = scp.read_opus(['test.0000', 'test.0001', 'test.0002'], directory='irdata/OPUS', merge=False)
+    >>> len(le)
+    3
+
+    Read without a filename. This has the effect of opening a dialog for file(s)
+    selection
+
+    >>> nd = scp.read_opus()
+
+    Read in a directory (assume that only OPUS files are present in the directory
+    (else we must use the generic `read` function instead)
+
+    >>> le = scp.read_opus(directory='irdata/OPUS')
+    >>> len(le)
+    4
+
+    Again we can use merge to stack all 4 spectra if thet have compatible dimensions.
+
+    >>> scp.read_opus(directory='irdata/OPUS', merge=True)
+    NDDataset: [float64] a.u. (shape: (y:4, x:2567))
     """
-    kwargs["filetypes"] = ["Compressed files (*.zip)"]
-    # TODO: allows other type of compressed files
-    kwargs["protocol"] = ["zip"]
+
+    kwargs["filetypes"] = ["Bruker OPUS files (*.[0-9]*)"]
+    kwargs["protocol"] = ["opus"]
     importer = Importer()
     return importer(*paths, **kwargs)
 
 
 # ======================================================================================
-# Private functions
+# Private Functions
 # ======================================================================================
 @_importer_method
-def _read_zip(*args, **kwargs):
-    # Below we assume that files to read are in a unique directory
-    import zipfile
-
-    from spectrochempy.core.dataset.nddataset import NDDataset
-
-    # read zip file
-    _, filename = args
-    content = kwargs.pop("content", None)
-
-    if content:
-        fid = io.BytesIO(content)
-    else:
-        fid = open(filename, "rb")
-
-    with zipfile.ZipFile(fid) as zf:
-
-        filelist = zf.filelist
-        only = kwargs.pop("only", len(filelist))
-
-        datasets = []
-
-        # for file in filelist:
-        #
-        #   # make a pathlib object (but this doesn't work with python 3.7)
-        #     file = zipfile.Path(zf, at=file.filename)      # TODO:
-        #
-        #     if file.name.startswith('__MACOSX'):
-        #         continue  # bypass non-data files
-        #
-        #     # seek the parent directory containing the files to read
-        #     if not file.is_dir():
-        #         continue
-        #
-        #     parent = file
-        #     break
-        #
-        #
-        # for count, children in enumerate(parent.iterdir()):
-        #
-        #     if count == only:
-        #         # limits to only this number of files
-        #         break
-        #
-        #     _ , extension = children.name.split('.')
-        #     if extension == 'DS_Store':
-        #         only += 1
-        #         continue
-        #
-        #     read_ = getattr(NDDataset, f"read_{extension}")
-        #
-        #     datasets.append(read_(children.name, content=children.read_bytes(), **kwargs))
-
-        # 3.7 compatible code
-
-        # seek the parent directory containing the files to read
-        for file in filelist:
-            if not file.filename.startswith("__") and file.is_dir():
-                parent = file.filename
-                break
-
-        count = 0
-        for file in filelist:
-            if (
-                not file.is_dir()
-                and file.filename.startswith(parent)
-                and "DS_Store" not in file.filename
-            ):
-                # read it
-                datasets.append(
-                    NDDataset.read(
-                        {file.filename: zf.read(file.filename)},
-                        origin=kwargs.get("origin", None),
-                    )
-                )
-                count += 1
-                if count == only:
-                    break
-    return datasets
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
+def _read_opus(*args, **kwargs):
+    debug_("Bruker OPUS import")
+
+    dataset, filename = args
+
+    fid, kwargs = _openfid(filename, **kwargs)
+
+    opus_data = _read_data(fid)
+
+    # data
+    try:
+        npt = opus_data["AB Data Parameter"]["NPT"]
+        data = opus_data["AB"][:npt]
+        dataset.data = np.array(data[np.newaxis], dtype="float32")
+    except KeyError:
+        raise KeyError(
+            f"{filename} is not an Absorbance spectrum. It cannot be read with the `read_opus` import method"
+        )
+    # todo: read background
+
+    # xaxis
+    fxv = opus_data["AB Data Parameter"]["FXV"]
+    lxv = opus_data["AB Data Parameter"]["LXV"]
+    # xdata = linspace(fxv, lxv, npt)
+    xaxis = LinearCoord.linspace(fxv, lxv, npt, title="wavenumbers", units="cm^-1")
+
+    # yaxis
+    name = opus_data["Sample"]["SNM"]
+    acqdate = opus_data["AB Data Parameter"]["DAT"]
+    acqtime = opus_data["AB Data Parameter"]["TIM"]
+    gmt_offset_hour = float(acqtime.split("GMT")[1].split(")")[0])
+    if len(acqdate.split("/")[0]) == 2:
+        date_time = datetime.strptime(
+            acqdate + "_" + acqtime.split()[0], "%d/%m/%Y_%H:%M:%S.%f"
+        )
+    elif len(acqdate.split("/")[0]) == 4:
+        date_time = datetime.strptime(
+            acqdate + "_" + acqtime.split()[0], "%Y/%m/%d_%H:%M:%S"
+        )
+    utc_dt = date_time - timedelta(hours=gmt_offset_hour)
+    utc_dt = utc_dt.replace(tzinfo=timezone.utc)
+    timestamp = utc_dt.timestamp()
+
+    yaxis = Coord(
+        [timestamp],
+        title="acquisition timestamp (GMT)",
+        units="s",
+        labels=([utc_dt], [name], [filename]),
+    )
+
+    # set dataset's Coordset
+    dataset.set_coordset(y=yaxis, x=xaxis)
+    dataset.units = "absorbance"
+    dataset.title = "absorbance"
+
+    # Set name, origin, description and history
+    dataset.name = filename.name
+    dataset.origin = "opus"
+    dataset.description = "Dataset from opus files. \n"
+    dataset.history = str(datetime.now(timezone.utc)) + ": import from opus files \n"
+
+    # reset modification date to cretion date
+    dataset._modified = dataset._created
+
+    return dataset
+
+
+def _read_data(fid):
+    data = fid.read()
+    meta_data = parse_meta(data)
+    opus_data = parse_data(data, meta_data)
+    return opus_data
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/script/__init__.py` & `spectrochempy-0.6.2/spectrochempy/core/script/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,11 +236,7 @@
     ----------
     project : project instance
         The project in which the scripts have to be executed
     """
     # TODO: complete this run_all_script function
 
     project
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/units/__init__.py` & `spectrochempy-0.6.2/spectrochempy/core/units/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,12 +424,7 @@
     def new_func(*args, **kwargs):
 
         args = tuple([_remove_units(arg) for arg in args])
         kwargs = {key: _remove_units(val) for key, val in kwargs.items()}
         return func(*args, **kwargs)
 
     return new_func
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/writers/exporter.py` & `spectrochempy-0.6.2/spectrochempy/core/writers/exporter.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,12 +142,7 @@
 
 
 @exportermethod
 def _write_scp(*args, **kwargs):
     dataset, filename = args
     dataset.filename = filename
     return dataset.dump(filename, **kwargs)
-
-
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/writers/write_csv.py` & `spectrochempy-0.6.2/spectrochempy/core/writers/write_csv.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/writers/write_excel.py` & `spectrochempy-0.6.2/spectrochempy/core/writers/write_excel.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/core/writers/write_jcamp.py` & `spectrochempy-0.6.2/spectrochempy/core/writers/write_jcamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 from datetime import datetime, timezone
 
 import numpy as np
 
 from spectrochempy.core.writers.exporter import Exporter, exportermethod
 
-__all__ = ["write_jcamp", "write_jdx"]
+__all__ = ["write_jcamp"]
 __dataset_methods__ = __all__
 
 
 def write_jcamp(*args, **kwargs):
     """
     Write a dataset in JCAMP-DX format.
 
@@ -48,18 +48,14 @@
     """
     exporter = Exporter()
     kwargs["filetypes"] = ["JCAMP-DX files (*.jdx)"]
     kwargs["suffix"] = ".jdx"
     return exporter(*args, **kwargs)
 
 
-write_jdx = write_jcamp
-write_jdx.__doc__ = "This method is an alias of `write_jcamp` ."
-
-
 @exportermethod
 def _write_jcamp(*args, **kwargs):
     # Writes a dataset in JCAMP-DX format
 
     dataset, filename = args
     dataset.filename = filename
```

### Comparing `spectrochempy-0.6.1/spectrochempy/core/writers/write_matlab.py` & `spectrochempy-0.6.2/spectrochempy/core/writers/write_matlab.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/extern/nmrglue.py` & `spectrochempy-0.6.2/spectrochempy/extern/nmrglue.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/extern/traittypes.py` & `spectrochempy-0.6.2/spectrochempy/extern/traittypes.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/extern/traittypes_utils.py` & `spectrochempy-0.6.2/spectrochempy/extern/traittypes_utils.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/ipython/magics.py` & `spectrochempy-0.6.2/spectrochempy/ipython/magics.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/__init__.py` & `spectrochempy-0.6.2/spectrochempy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/citation.py` & `spectrochempy-0.6.2/spectrochempy/utils/citation.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/constants.py` & `spectrochempy-0.6.2/spectrochempy/utils/constants.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/coordrange.py` & `spectrochempy-0.6.2/spectrochempy/utils/coordrange.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,12 +100,7 @@
     Examples
     --------
 
     >>> scp.trim_ranges([1, 4], [7, 5], [6, 10])
     [[1, 4], [5, 10]]
     """
     return _CoordRange(*ranges, reversed=reversed).ranges
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/decorators.py` & `spectrochempy-0.6.2/spectrochempy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/docstrings.py` & `spectrochempy-0.6.2/spectrochempy/utils/docstrings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/exceptions.py` & `spectrochempy-0.6.2/spectrochempy/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/fake.py` & `spectrochempy-0.6.2/spectrochempy/utils/fake.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,12 +90,7 @@
     d = dot(concs.T, specs)
 
     # add some noise
     d.data = np.random.normal(d.data, 0.005 * d.data.max())
 
     # d.plot()
     return d, specs, concs
-
-
-if __name__ == "__main__":
-
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/file.py` & `spectrochempy-0.6.2/spectrochempy/utils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,22 @@
 
 
 # ======================================================================================
 # Utility functions
 # ======================================================================================
 def download_testdata():
     from spectrochempy.core import preferences
-    from spectrochempy.core.readers.importer import read_remote
+    from spectrochempy.core.readers.importer import read
     from spectrochempy.utils.file import pathclean
 
     datadir = pathclean(preferences.datadir)
     # this process is relatively long, so we do not want to do it several time:
     downloaded = datadir / "__downloaded__"
     if not downloaded.exists():
-        read_remote(datadir, download_only=True)
+        read(datadir, download_only=True)
         downloaded.touch(exist_ok=True)
 
 
 def _insensitive_case_glob(pattern):
     def either(c):
         return f"[{c.lower()}{c.upper()}]" if c.isalpha() else c
 
@@ -54,25 +54,25 @@
     """
     Clean a path or a series of path.
 
     The aim is to be compatible with windows and unix-based system.
 
     Parameters
     ----------
-    paths :  str or a list of str
-        Path to clean. It may contain windows or conventional python separators.
+    paths :  `str` or a `list` of `str`
+        Path to clean. It may contain Windows or conventional python separators.
 
     Returns
     -------
     pathlib or list of pathlib
         Cleaned path(s).
 
     Examples
     --------
-    >>> from spectrochempy.utils import pathclean
+    >>> from spectrochempy.utils.file import pathclean
 
     Using unix/mac way to write paths
     >>> filename = pathclean('irdata/nh4y-activation.spg')
     >>> filename.suffix
     '.spg'
     >>> filename.parent.name
     'irdata'
@@ -143,50 +143,51 @@
 
 def check_filenames(*args, **kwargs):
     """
     Return a list or a dictionary of filenames.
 
     Parameters
     ----------
-    \*args
+    *args
         If passed it is a str, a list of str or a dictionary containing filenames or a byte's contents.
     **kwargs
         Optional keywords parameters. See Other parameters
 
     Other Parameters
     ----------------
     filename :
     filetypes :
     content :
     protocol :
     processed :
     expno :
     procno :
-    listdir :
+    iterdir :
     glob :
 
     See Also
     --------
     check_filename_to_open
     check_filename_to_save
 
     Examples
     --------
     """
+    # from spectrochempy.application import info_
     from spectrochempy.core import preferences as prefs
 
     datadir = pathclean(prefs.datadir)
 
     filenames = None
 
     if args:
         if (
             isinstance(args[0], str)
             and (args[0].startswith("http://") or args[0].startswith("https://"))
-            and kwargs.get("remote")
+            # and kwargs.get("remote")
         ):
             # return url
             return args
         elif isinstance(args[0], (str, Path, PosixPath, WindowsPath)):
             # one or several filenames are passed - make Path objects
             filenames = pathclean(args)
         elif isinstance(args[0], bytes):
@@ -201,15 +202,16 @@
         elif isinstance(args[0], list) and isinstance(args[0][0], bytes):
             return {pathclean(f"no_name_{i}"): arg for i, arg in enumerate(args[0])}
         elif isinstance(args[0], dict):
             # return directly the dictionary
             return args[0]
 
     if not filenames:
-        # look into keywords (only the case where a str or pathlib filename is given are accepted)
+        # look into keywords (only the case where a str or pathlib filename is given are
+        # accepted)
         filenames = kwargs.pop("filename", None)
         filenames = [pathclean(filenames)] if pathclean(filenames) is not None else None
 
     # Look for content in kwargs
     content = kwargs.pop("content", None)
     if content:
         if not filenames:
@@ -235,28 +237,30 @@
             if directory and kw_directory and directory != kw_directory:
                 # conflict we do not take into account the kw.
                 warnings.warn(
                     "Two different directory where specified (from args and keywords arg). "
                     "Keyword `directory` will be ignored!"
                 )
             elif not directory and kw_directory:
-                filename = kw_directory / filename
+                filename = pathclean(kw_directory / filename)
 
             # check if the file exists here
             if not directory or str(directory).startswith("."):
                 # search first in the current directory
                 directory = Path.cwd()
 
-            f = directory / filename
+            f = pathclean(directory / filename)
 
             fexist = f if f.exists() else _get_file_for_protocol(f, **kwargs)
-
+            # info_(f"fexist  {fexist}")
             if fexist is None:
-                f = datadir / filename
+                f = pathclean(datadir / filename)
+                # info_(f"f (line 255) {f}")
                 fexist = f if f.exists() else _get_file_for_protocol(f, **kwargs)
+                # info_(f"fexist  {fexist}")
 
             if fexist:
                 filename = fexist
 
             # Particular case for topspin where filename can be provided as a directory only
             # use of expno and procno
             if filename.is_dir() and "topspin" in kwargs.get("protocol", []):
@@ -269,16 +273,15 @@
 
         filenames = filenames_
 
     return filenames
 
 
 def _topspin_check_filename(filename, **kwargs):
-
-    if kwargs.get("listdir", False) or kwargs.get("glob", None) is not None:
+    if kwargs.get("iterdir", False) or kwargs.get("glob", None) is not None:
         # when we list topspin dataset we have to read directories, not directly files
         # we can retrieve them using glob patterns
         glob = kwargs.get("glob", None)
         if glob:
             files_ = list(filename.glob(glob))
         elif not kwargs.get("processed", False):
             files_ = list(filename.glob("**/ser"))
@@ -342,15 +345,15 @@
     directory : `str` or pathlib object, optional.
         The directory where to look at. If not specified, read in
         current directory, or in the datadir if unsuccessful.
     filetypes : `list` , optional, default=['all files, '.*)'].
         File type filter.
     dictionary : `bool` , optional, default=True
         Whether a dictionary or a list should be returned.
-    listdir : bool, default=False
+    iterdir : bool, default=False
         Read all file (possibly limited by `filetypes` in a given `directory` .
     recursive : bool, optional,  default=False.
         Read also subfolders.
 
     Warnings
     --------
     if several filenames are provided in the arguments, they must all reside in the same directory!
@@ -377,15 +380,18 @@
         filenames = filenames[0]
 
     filenames = pathclean(list(filenames))
 
     directory = None
     if len(filenames) == 1:
         # check if it is a directory
-        f = get_directory_name(filenames[0])
+        try:
+            f = get_directory_name(filenames[0])
+        except OSError:
+            f = None
         if f and f.is_dir():
             # this specify a directory not a filename
             directory = f
             filenames = None
             NODIAL = True
     # else:
     #    filenames = pathclean(list(filenames))
@@ -396,15 +402,15 @@
     if directory is None:
         directory = kw_dir
 
     if directory is not None:
         if filenames:
             # prepend to the filename (incompatibility between filename and directory specification
             # will result to a error
-            filenames = [directory / filename for filename in filenames]
+            filenames = [pathclean(directory / filename) for filename in filenames]
         else:
             directory = get_directory_name(directory)
 
     # check the parent directory
     # all filenames must reside in the same directory
     if filenames:
         parents = set()
@@ -424,32 +430,32 @@
     # now proceed with the filenames
     if filenames:
 
         # look if all the filename exists either in the specified directory,
         # else in the current directory, and finally in the default preference data directory
         temp = []
         for i, filename in enumerate(filenames):
-            if not (directory / filename).exists():
+            if not (pathclean(directory / filename)).exists():
                 # the filename provided doesn't exists in the working directory
                 # try in the data directory
                 directory = pathclean(prefs.datadir)
-                if not (directory / filename).exists():
+                if not (pathclean(directory / filename)).exists():
                     raise IOError(f"Can't find  this filename {filename}")
             temp.append(directory / filename)
 
         # now we have checked all the filename with their correct location
         filenames = temp
 
     else:
         # no filenames:
         # open a file dialog
-        # except if a directory is specified or listdir is True.
+        # except if a directory is specified or iterdir is True.
 
         getdir = kwargs.get(
-            "listdir",
+            "iterdir",
             directory is not None or kwargs.get("protocol", None) == ["topspin"]
             # or kwargs.get("protocol", None) == ["carroucell"],
         )
 
         if not getdir:
             # we open a dialogue to select one or several files manually
             if not NODIAL:
@@ -571,29 +577,31 @@
 
     data_dir = pathclean(prefs.datadir)
     working_dir = Path.cwd()
 
     directory = pathclean(directory)
 
     if directory:
+
+        # Search locally
         if directory.is_dir():
             # nothing else to do
             return directory
 
         elif (working_dir / directory).is_dir():
             # if no parent directory: look at current working dir
             return working_dir / directory
 
         elif (data_dir / directory).is_dir():
             return data_dir / directory
 
         else:
-            # raise ValueError(f'"{dirname}" is not a valid directory')
-            warnings.warn(f'"{directory}" is not a valid directory')
-            return None
+            raise OSError(f'"{str(directory)}" is not a valid directory')
+            # warnings.warn(f'"{directory}" is not a valid directory')
+            # return None
 
     else:
         # open a file dialog
         directory = data_dir
         if not NO_DIALOG:  # this is for allowing test to continue in the background
             from spectrochempy.core.common.dialogs import open_dialog
 
@@ -683,10 +691,7 @@
         # args where passed so in this case we have directly byte contents instead of filenames only
         contents = filenames
         return {"frombytes": contents}
 
     else:
         # probably no args (which means that we are coming from a dialog or from a full list of a directory
         return filenames
-
-
-# EOF
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/jsonutils.py` & `spectrochempy-0.6.2/spectrochempy/utils/jsonutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,11 +174,7 @@
         else:
             return {
                 "base64": base64.b64encode(pickle.dumps(byte_obj)).decode(),
                 "__class__": "COMPLEX",
             }
 
     raise ValueError(f"No encoding handler for data type {type(byte_obj)}")
-
-
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/misc.py` & `spectrochempy-0.6.2/spectrochempy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/objects.py` & `spectrochempy-0.6.2/spectrochempy/utils/objects.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/optional.py` & `spectrochempy-0.6.2/spectrochempy/utils/optional.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def import_optional_dependency(
     name: str,
     extra: str = "",
     errors: str = "raise",
     min_version: str | None = None,
 ):
-    """
+    r"""
     Import an optional dependency.
 
     By default, if a dependency is missing an ImportError with a nice
     message will be raised. If a dependency is present, but too old,
     we raise.
 
     Parameters
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/orderedset.py` & `spectrochempy-0.6.2/spectrochempy/utils/orderedset.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/packages.py` & `spectrochempy-0.6.2/spectrochempy/utils/packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,12 +92,7 @@
     path = os.path.dirname(import_item(package).__file__)
     path = os.path.join(path, data_name)
 
     if not os.path.isdir(path):  # pragma: no cover
         return os.path.dirname(path)
 
     return path
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/plots.py` & `spectrochempy-0.6.2/spectrochempy/utils/plots.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/print.py` & `spectrochempy-0.6.2/spectrochempy/utils/print.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/print_versions.py` & `spectrochempy-0.6.2/spectrochempy/utils/print_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,9 +108,9 @@
                 f"{optional.get_module_version(mod) if mod is not None else None}",
                 file=file,
             )
         except ImportError:
             print(f"{dep}: (Can't determine version string)", file=file)
 
 
-if __name__ == "__main__":
+if __name__ == "__main__":  # pragma: no cover
     show_versions()
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/system.py` & `spectrochempy-0.6.2/spectrochempy/utils/system.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/testing.py` & `spectrochempy-0.6.2/spectrochempy/utils/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,14 +982,7 @@
 #                     break
 #
 #             return
 #
 #         return wrapper
 #
 #     return make_image_comparison
-
-
-# --------------------------------------------------------------------------------------
-# main
-# --------------------------------------------------------------------------------------
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/traits.py` & `spectrochempy-0.6.2/spectrochempy/utils/traits.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,12 +94,7 @@
     def __init__(self, default_value=Empty, allow_none=False, dtype=None, **kwargs):
         if "klass" not in kwargs and self.klass is None:
             from spectrochempy.core.dataset.coord import Coord
 
             kwargs["klass"] = Coord
         super().__init__(default_value=default_value, allow_none=allow_none, **kwargs)
         self.metadata.update({"dtype": dtype})
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
```

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/version.py` & `spectrochempy-0.6.2/spectrochempy/utils/version.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/warnings.py` & `spectrochempy-0.6.2/spectrochempy/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/utils/zip.py` & `spectrochempy-0.6.2/spectrochempy/utils/zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,14 +141,7 @@
             return self.zip.read(key)
 
         else:
             raise KeyError("%s is not a file in the archive or is not " "allowed" % key)
 
     def __contains__(self, key):
         return self.files.__contains__(key)
-
-
-# ======================================================================================
-if __name__ == "__main__":
-    pass
-
-# EOF
```

### Comparing `spectrochempy-0.6.1/spectrochempy/widgets/baselinecorrector.py` & `spectrochempy-0.6.2/spectrochempy/widgets/baselinecorrector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy/widgets/fileselector.py` & `spectrochempy-0.6.2/spectrochempy/widgets/fileselector.py`

 * *Files identical despite different names*

### Comparing `spectrochempy-0.6.1/spectrochempy.egg-info/PKG-INFO` & `spectrochempy-0.6.2/spectrochempy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrochempy
-Version: 0.6.1
+Version: 0.6.2
 Summary: Processing, analysis and modelling Spectroscopic data for Chemistry with Python
 Home-page: https://www.spectrochempy.fr
 Author: Arnaud Travert & Christian Fernandez
 Author-email: contact@spectrochempy.fr
 Maintainer: C. Fernandez
 Maintainer-email: christian.fernandez@ensicaen.fr
 License: CECILL-B
```

### Comparing `spectrochempy-0.6.1/spectrochempy.egg-info/SOURCES.txt` & `spectrochempy-0.6.2/spectrochempy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 spectrochempy/analysis/iris.py
 spectrochempy/analysis/kinetic_utilities.py
 spectrochempy/analysis/linearregression.py
 spectrochempy/analysis/mcrals.py
 spectrochempy/analysis/nnmf.py
 spectrochempy/analysis/pca.py
 spectrochempy/analysis/peakfinding.py
+spectrochempy/analysis/pls.py
 spectrochempy/analysis/readme.rst
 spectrochempy/analysis/simplisma.py
 spectrochempy/analysis/svd.py
 spectrochempy/analysis/optimize/__init__.py
 spectrochempy/analysis/optimize/_models.py
 spectrochempy/analysis/optimize/_parameters.py
 spectrochempy/analysis/optimize/optimize.py
```

