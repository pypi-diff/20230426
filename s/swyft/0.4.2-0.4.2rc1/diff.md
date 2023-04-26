# Comparing `tmp/swyft-0.4.2.tar.gz` & `tmp/swyft-0.4.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swyft-0.4.2.tar", last modified: Wed Apr 26 21:04:10 2023, max compression
+gzip compressed data, was "swyft-0.4.2rc1.tar", last modified: Thu Jan 12 08:06:39 2023, max compression
```

## Comparing `swyft-0.4.2.tar` & `swyft-0.4.2rc1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.660369 swyft-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-26 21:03:55.000000 swyft-0.4.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.640369 swyft-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.644369 swyft-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-26 21:03:55.000000 swyft-0.4.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 21:03:55.000000 swyft-0.4.2/.github/workflows/syntax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-26 21:03:55.000000 swyft-0.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-26 21:03:55.000000 swyft-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-26 21:03:55.000000 swyft-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-26 21:03:55.000000 swyft-0.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-04-26 21:03:55.000000 swyft-0.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-04-26 21:03:55.000000 swyft-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-26 21:04:10.660369 swyft-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-04-26 21:03:55.000000 swyft-0.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.644369 swyft-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.644369 swyft-0.4.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.640369 swyft-0.4.2/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.648369 swyft-0.4.2/docs/source/_static/img/
--rw-r--r--   0 runner    (1001) docker     (123)  4253636 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/_static/img/SBI-curve.gif
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/_static/img/swyft_logo_wide.png
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/autodoc.rst
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/contributing-link.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.648369 swyft-0.4.2/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)   176838 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/images/20d-1dPos.png
--rw-r--r--   0 runner    (1001) docker     (123)    23873 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/images/quickstart-1d.png
--rw-r--r--   0 runner    (1001) docker     (123)    57354 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/images/quickstart-2d.png
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.652369 swyft-0.4.2/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/bounds.rst~
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/inference.rst~
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/lightning.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/networks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/plot.rst
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/prior.rst~
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/store.rst~
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/utils.rst~
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/module/weightedmarginals.rst~
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.652369 swyft-0.4.2/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0A-SwyftModule.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0B-Simulator.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0C-LogRatioEstimator_Ndim.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0D-Mass.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0E-ZarrStore.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0F-Logging.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0G-Bounds.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/0H-Fast-slow.nblink
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/Swyft in 15 minutes.nblink
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/notebooks/make-nblinks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.652369 swyft-0.4.2/docs/source/old/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/context.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/goals.rst
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/latex_macros.sty
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/theory.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/old/theorytex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/swyft.rst
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/tutorial-notebooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-26 21:03:55.000000 swyft-0.4.2/docs/source/videos.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.652369 swyft-0.4.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/01-Precision through truncation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0A-SwyftModule.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0B-Simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   157710 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0C-LogRatioEstimator_Ndim.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    66954 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0D-Mass.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0E-ZarrStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0F-Logging.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31346 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0G-Bounds.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31489 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0H-Fast-slow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    72381 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/0I-Model comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54358 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/Swyft in 15 minutes.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.656369 swyft-0.4.2/notebooks/deprecated/
--rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/01-minimal-example-Copy1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/01-minimal-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/02-minimal-hparams.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/03-minimal-zarr.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/04-minimal-noise-hook.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    35280 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/05-minimal-example-n-dim.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    82722 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 1. Custom networks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    45697 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 2. Truncation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   116736 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 3. Saving and Loading.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 4. The Store.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 5. External Simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 6. Dask Simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Examples - 7. Composite Priors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   134566 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/Quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.656369 swyft-0.4.2/notebooks/deprecated/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)    50093 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/lightning/Examples - 1. Simple 1-dim parameter fit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    44102 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/lightning/Examples - 2. Rings.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    59369 2023-04-26 21:03:55.000000 swyft-0.4.2/notebooks/deprecated/lightning/Examples - 3. Simple 2-dim posteriors.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-26 21:03:55.000000 swyft-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-26 21:04:10.660369 swyft-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 21:03:55.000000 swyft-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.656369 swyft-0.4.2/swyft/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.656369 swyft-0.4.2/swyft/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/online.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/samples.py~
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/torchstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/lightning/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.660369 swyft-0.4.2/swyft/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/networks/channelized.py
--rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/networks/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/networks/standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.660369 swyft-0.4.2/swyft/plot/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/plot2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/plot/violin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.660369 swyft-0.4.2/swyft/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/utils/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/utils/marginals.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-26 21:03:55.000000 swyft-0.4.2/swyft/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.656369 swyft-0.4.2/swyft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-26 21:04:10.000000 swyft-0.4.2/swyft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 21:04:10.660369 swyft-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 21:03:55.000000 swyft-0.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 21:03:55.000000 swyft-0.4.2/tests/test_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.722318 swyft-0.4.2rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.722318 swyft-0.4.2rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.github/workflows/syntax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.722318 swyft-0.4.2rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.726318 swyft-0.4.2rc1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.722318 swyft-0.4.2rc1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.730318 swyft-0.4.2rc1/docs/source/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)  4253636 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/_static/img/SBI-curve.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/_static/img/swyft_logo_wide.png
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/autodoc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/contributing-link.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.730318 swyft-0.4.2rc1/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   176838 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/images/20d-1dPos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23873 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/images/quickstart-1d.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57354 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/images/quickstart-2d.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.730318 swyft-0.4.2rc1/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/bounds.rst~
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/inference.rst~
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/lightning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/prior.rst~
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/store.rst~
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/utils.rst~
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/module/weightedmarginals.rst~
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.730318 swyft-0.4.2rc1/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0A-SwyftModule.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0B-Simulator.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0C-LogRatioEstimator_Ndim.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0D-Mass.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0E-ZarrStore.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0F-Logging.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0G-Bounds.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/0H-Fast-slow.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/Swyft in 15 minutes.nblink
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/notebooks/make-nblinks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.730318 swyft-0.4.2rc1/docs/source/old/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/goals.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/latex_macros.sty
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15978 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/theory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/old/theorytex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/swyft.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/tutorial-notebooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/docs/source/videos.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.734318 swyft-0.4.2rc1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    48455 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/01-Precision through truncation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28617 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0A-SwyftModule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0B-Simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   157710 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0C-LogRatioEstimator_Ndim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    66954 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0D-Mass.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14059 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0E-ZarrStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0F-Logging.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31346 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0G-Bounds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31489 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0H-Fast-slow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    72381 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/0I-Model comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54358 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/Swyft in 15 minutes.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.734318 swyft-0.4.2rc1/notebooks/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/01-minimal-example-Copy1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18682 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/01-minimal-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    30966 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/02-minimal-hparams.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/03-minimal-zarr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/04-minimal-noise-hook.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    35280 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/05-minimal-example-n-dim.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    82722 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 1. Custom networks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    45697 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 2. Truncation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   116736 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 3. Saving and Loading.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 4. The Store.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11171 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 5. External Simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 6. Dask Simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Examples - 7. Composite Priors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   134566 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/Quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.734318 swyft-0.4.2rc1/notebooks/deprecated/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)    50093 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 1. Simple 1-dim parameter fit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    44102 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 2. Rings.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    59369 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 3. Simple 2-dim posteriors.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-01-12 08:06:39.742318 swyft-0.4.2rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16368 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/online.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/samples.py~
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/torchstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/lightning/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/networks/channelized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8094 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/networks/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/networks/standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/plot2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/plot/violin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/utils/marginals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/swyft/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/swyft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-12 08:06:39.000000 swyft-0.4.2rc1/swyft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:39.738318 swyft-0.4.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-01-12 08:06:25.000000 swyft-0.4.2rc1/tests/test_simulator.py
```

### Comparing `swyft-0.4.2/.github/workflows/pypi-publish.yml` & `swyft-0.4.2rc1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/.github/workflows/syntax.yml` & `swyft-0.4.2rc1/.github/workflows/syntax.yml`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/.github/workflows/tests.yml` & `swyft-0.4.2rc1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/.gitignore` & `swyft-0.4.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/.pre-commit-config.yaml` & `swyft-0.4.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/.readthedocs.yaml` & `swyft-0.4.2rc1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/CONTRIBUTING.md` & `swyft-0.4.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/LICENSE` & `swyft-0.4.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/PKG-INFO` & `swyft-0.4.2rc1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swyft
-Version: 0.4.2
+Version: 0.4.2rc1
 Summary: Universal scalable simulation-based inference with TMNRE (Truncated Marginal Neural Ratio Estimation) and pytorch-lightning.
 Home-page: https://github.com/undark-lab/swyft
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -85,35 +85,14 @@
 * To this end, Swyft estimates likelihood-to-evidence ratios for arbitrary marginal posteriors; they typically require fewer simulations than the corresponding joint.
 * Swyft performs targeted inference by prior truncation, combining simulation efficiency with empirical testability.
 * Swyft is based on stochastic simulators, which map parameters stochastically to observational data. Swyft makes it convenient to define such simulators as graphical models.
 * In scientific settings, a cost-benefit analysis often favors approximating the posterior marginality; *swyft* provides this functionality.
 * The package additionally implements our prior truncation technique, routines to empirically test results by estimating the expected coverage, and a simulator manager with `zarr <https://zarr.readthedocs.io/en/stable/>`_ storage to simplify use with complex simulators.
 
 
-Papers using Swyft/TMNRE
-------------------------
-
-2021
-
-- “Fast and Credible Likelihood-Free Cosmology with Truncated Marginal Neural Ratio Estimation“ Cole+ https://arxiv.org/abs/2111.08030
-
-2022
-
-- “Estimating the warm dark matter mass from strong lensing images with truncated marginal neural ratio estimation” Anau Montel+, https://arxiv.org/abs/2205.09126
-- “SICRET: Supernova Ia Cosmology with truncated marginal neural Ratio EsTimation” Karchev+ https://arxiv.org/abs/2209.06733
-- “One never walks alone: the effect of the perturber population on subhalo measurements in strong gravitational lenses” Coogan+ https://arxiv.org/abs/2209.09918
-- “Detection is truncation: studying source populations with truncated marginal neural ratio estimation” Anau Montel+ https://arxiv.org/abs/2211.04291
-
-2023
-
-- “Debiasing Standard Siren Inference of the Hubble Constant with Marginal Neural Ratio Estimation” Gagnon-Hartman+ https://arxiv.org/abs/2301.05241
-- “Constraining the X-ray heating and reionization using 21-cm power spectra with Marginal Neural Ratio Estimation” Saxena+ https://arxiv.org/abs/2303.07339
-- “Peregrine: Sequential simulation-based inference for gravitational wave signals”, Bhardwaj+ https://arxiv.org/abs/2304.02035
-- “Albatross: A scalable simulation-based inference pipeline for analysing stellar streams in the Milky Way”, Alvey+ https://arxiv.org/abs/2304.02032
-
 
 Further information
 -------------------
 
 * **Documentation & installation**: https://swyft.readthedocs.io/
 * **Example usage**: https://swyft.readthedocs.io/en/latest/tutorial-notebooks.html
 * **Source code**: https://github.com/undark-lab/swyft
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swyft-0.4.2/README.rst` & `swyft-0.4.2rc1/swyft.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: swyft
+Version: 0.4.2rc1
+Summary: Universal scalable simulation-based inference with TMNRE (Truncated Marginal Neural Ratio Estimation) and pytorch-lightning.
+Home-page: https://github.com/undark-lab/swyft
+License: MIT License
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Environment :: GPU
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+Provides-Extra: docs
+License-File: LICENSE
+
 Swyft v0.4
 ==========
 
 .. image:: https://badge.fury.io/py/swyft.svg
    :target: https://badge.fury.io/py/swyft
    :alt: PyPI version
 
@@ -63,35 +85,14 @@
 * To this end, Swyft estimates likelihood-to-evidence ratios for arbitrary marginal posteriors; they typically require fewer simulations than the corresponding joint.
 * Swyft performs targeted inference by prior truncation, combining simulation efficiency with empirical testability.
 * Swyft is based on stochastic simulators, which map parameters stochastically to observational data. Swyft makes it convenient to define such simulators as graphical models.
 * In scientific settings, a cost-benefit analysis often favors approximating the posterior marginality; *swyft* provides this functionality.
 * The package additionally implements our prior truncation technique, routines to empirically test results by estimating the expected coverage, and a simulator manager with `zarr <https://zarr.readthedocs.io/en/stable/>`_ storage to simplify use with complex simulators.
 
 
-Papers using Swyft/TMNRE
-------------------------
-
-2021
-
-- “Fast and Credible Likelihood-Free Cosmology with Truncated Marginal Neural Ratio Estimation“ Cole+ https://arxiv.org/abs/2111.08030
-
-2022
-
-- “Estimating the warm dark matter mass from strong lensing images with truncated marginal neural ratio estimation” Anau Montel+, https://arxiv.org/abs/2205.09126
-- “SICRET: Supernova Ia Cosmology with truncated marginal neural Ratio EsTimation” Karchev+ https://arxiv.org/abs/2209.06733
-- “One never walks alone: the effect of the perturber population on subhalo measurements in strong gravitational lenses” Coogan+ https://arxiv.org/abs/2209.09918
-- “Detection is truncation: studying source populations with truncated marginal neural ratio estimation” Anau Montel+ https://arxiv.org/abs/2211.04291
-
-2023
-
-- “Debiasing Standard Siren Inference of the Hubble Constant with Marginal Neural Ratio Estimation” Gagnon-Hartman+ https://arxiv.org/abs/2301.05241
-- “Constraining the X-ray heating and reionization using 21-cm power spectra with Marginal Neural Ratio Estimation” Saxena+ https://arxiv.org/abs/2303.07339
-- “Peregrine: Sequential simulation-based inference for gravitational wave signals”, Bhardwaj+ https://arxiv.org/abs/2304.02035
-- “Albatross: A scalable simulation-based inference pipeline for analysing stellar streams in the Milky Way”, Alvey+ https://arxiv.org/abs/2304.02032
-
 
 Further information
 -------------------
 
 * **Documentation & installation**: https://swyft.readthedocs.io/
 * **Example usage**: https://swyft.readthedocs.io/en/latest/tutorial-notebooks.html
 * **Source code**: https://github.com/undark-lab/swyft
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swyft-0.4.2/docs/Makefile` & `swyft-0.4.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/make.bat` & `swyft-0.4.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/_static/img/SBI-curve.gif` & `swyft-0.4.2rc1/docs/source/_static/img/SBI-curve.gif`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/_static/img/swyft_logo_wide.png` & `swyft-0.4.2rc1/docs/source/_static/img/swyft_logo_wide.png`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/autodoc.rst` & `swyft-0.4.2rc1/docs/source/autodoc.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/citation.rst` & `swyft-0.4.2rc1/docs/source/citation.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/conf.py` & `swyft-0.4.2rc1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/images/20d-1dPos.png` & `swyft-0.4.2rc1/docs/source/images/20d-1dPos.png`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/images/quickstart-1d.png` & `swyft-0.4.2rc1/docs/source/images/quickstart-1d.png`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/images/quickstart-2d.png` & `swyft-0.4.2rc1/docs/source/images/quickstart-2d.png`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/index.rst` & `swyft-0.4.2rc1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/install.rst` & `swyft-0.4.2rc1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/notebooks/make-nblinks.py` & `swyft-0.4.2rc1/docs/source/notebooks/make-nblinks.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/old/context.rst` & `swyft-0.4.2rc1/docs/source/old/context.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/old/goals.rst` & `swyft-0.4.2rc1/docs/source/old/goals.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/old/quickstart.rst` & `swyft-0.4.2rc1/docs/source/old/quickstart.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/old/theory.rst` & `swyft-0.4.2rc1/docs/source/old/theory.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/old/theorytex.rst` & `swyft-0.4.2rc1/docs/source/old/theorytex.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/refs.bib` & `swyft-0.4.2rc1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/swyft.rst` & `swyft-0.4.2rc1/docs/source/swyft.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/docs/source/videos.rst` & `swyft-0.4.2rc1/docs/source/videos.rst`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/01-Precision through truncation.ipynb` & `swyft-0.4.2rc1/notebooks/01-Precision through truncation.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0A-SwyftModule.ipynb` & `swyft-0.4.2rc1/notebooks/0A-SwyftModule.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0B-Simulator.ipynb` & `swyft-0.4.2rc1/notebooks/0B-Simulator.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0C-LogRatioEstimator_Ndim.ipynb` & `swyft-0.4.2rc1/notebooks/0C-LogRatioEstimator_Ndim.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0D-Mass.ipynb` & `swyft-0.4.2rc1/notebooks/0D-Mass.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0E-ZarrStore.ipynb` & `swyft-0.4.2rc1/notebooks/0E-ZarrStore.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0F-Logging.ipynb` & `swyft-0.4.2rc1/notebooks/0F-Logging.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0G-Bounds.ipynb` & `swyft-0.4.2rc1/notebooks/0G-Bounds.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0H-Fast-slow.ipynb` & `swyft-0.4.2rc1/notebooks/0H-Fast-slow.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/0I-Model comparison.ipynb` & `swyft-0.4.2rc1/notebooks/0I-Model comparison.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/Swyft in 15 minutes.ipynb` & `swyft-0.4.2rc1/notebooks/Swyft in 15 minutes.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/01-minimal-example-Copy1.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/01-minimal-example-Copy1.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/01-minimal-example.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/01-minimal-example.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/02-minimal-hparams.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/02-minimal-hparams.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/03-minimal-zarr.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/03-minimal-zarr.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/04-minimal-noise-hook.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/04-minimal-noise-hook.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/05-minimal-example-n-dim.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/05-minimal-example-n-dim.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 1. Custom networks.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 1. Custom networks.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 2. Truncation.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 2. Truncation.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 3. Saving and Loading.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 3. Saving and Loading.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 4. The Store.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 4. The Store.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 5. External Simulator.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 5. External Simulator.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 6. Dask Simulator.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 6. Dask Simulator.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Examples - 7. Composite Priors.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Examples - 7. Composite Priors.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/Quickstart.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/lightning/Examples - 1. Simple 1-dim parameter fit.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 1. Simple 1-dim parameter fit.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/lightning/Examples - 2. Rings.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 2. Rings.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/notebooks/deprecated/lightning/Examples - 3. Simple 2-dim posteriors.ipynb` & `swyft-0.4.2rc1/notebooks/deprecated/lightning/Examples - 3. Simple 2-dim posteriors.ipynb`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/setup.cfg` & `swyft-0.4.2rc1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 packages = find:
 zip_safe = False
 python_requires = >=3.7
 install_requires = 
 	toolz>=0.10.0
 	numpy>=1.18.1
 	torch>=1.10.2
-	pytorch_lightning>=1.5.10, <=1.9.0
+	pytorch_lightning>=1.5.10
 	zarr>=2.5.0
 	matplotlib>=3.1.3
 	scipy>=1.4.1
 	torchist>=0.1.7
 	fasteners>=0.17
 
 [options.extras_require]
```

### Comparing `swyft-0.4.2/swyft/lightning/__init__.py` & `swyft-0.4.2rc1/swyft/lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/bounds.py` & `swyft-0.4.2rc1/swyft/lightning/bounds.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/core.py` & `swyft-0.4.2rc1/swyft/lightning/core.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/data.py` & `swyft-0.4.2rc1/swyft/lightning/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,17 @@
         if isinstance(self.data, Samples):
             dataset = self.data.get_dataset(
                 on_after_load_sample=self.on_after_load_sample
             )
             splits = torch.utils.data.random_split(dataset, self.lengths)
             self.dataset_train, self.dataset_val, self.dataset_test = splits
         elif isinstance(self.data, swyft.ZarrStore):
-            idxr1 = (0, self.lengths[0])
-            idxr2 = (self.lengths[0], self.lengths[0] + self.lengths[1])
-            idxr3 = (self.lengths[0] + self.lengths[1], len(self.data))
+            idxr1 = (0, self.lengths[1])
+            idxr2 = (self.lengths[1], self.lengths[1] + self.lengths[2])
+            idxr3 = (self.lengths[1] + self.lengths[2], len(self.data))
             self.dataset_train = self.data.get_dataset(
                 idx_range=idxr1, on_after_load_sample=self.on_after_load_sample
             )
             self.dataset_val = self.data.get_dataset(
                 idx_range=idxr2, on_after_load_sample=None
             )
             self.dataset_test = self.data.get_dataset(
```

### Comparing `swyft-0.4.2/swyft/lightning/estimators.py` & `swyft-0.4.2rc1/swyft/lightning/estimators.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/online.py` & `swyft-0.4.2rc1/swyft/lightning/online.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/samples.py~` & `swyft-0.4.2rc1/swyft/lightning/samples.py~`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/simulator.py` & `swyft-0.4.2rc1/swyft/lightning/simulator.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/torchstore.py` & `swyft-0.4.2rc1/swyft/lightning/torchstore.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/lightning/utils.py` & `swyft-0.4.2rc1/swyft/lightning/utils.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/networks/__init__.py` & `swyft-0.4.2rc1/swyft/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/networks/channelized.py` & `swyft-0.4.2rc1/swyft/networks/channelized.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/networks/classifier.py` & `swyft-0.4.2rc1/swyft/networks/classifier.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/networks/standardization.py` & `swyft-0.4.2rc1/swyft/networks/standardization.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/__init__.py` & `swyft-0.4.2rc1/swyft/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/constraint.py` & `swyft-0.4.2rc1/swyft/plot/constraint.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/histogram.py` & `swyft-0.4.2rc1/swyft/plot/histogram.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/mass.py` & `swyft-0.4.2rc1/swyft/plot/mass.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/plot.py` & `swyft-0.4.2rc1/swyft/plot/plot.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/plot2.py` & `swyft-0.4.2rc1/swyft/plot/plot2.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/plot/violin.py` & `swyft-0.4.2rc1/swyft/plot/violin.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/types.py` & `swyft-0.4.2rc1/swyft/types.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/utils/__init__.py` & `swyft-0.4.2rc1/swyft/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/utils/array.py` & `swyft-0.4.2rc1/swyft/utils/array.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/utils/marginals.py` & `swyft-0.4.2rc1/swyft/utils/marginals.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft/utils/misc.py` & `swyft-0.4.2rc1/swyft/utils/misc.py`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/swyft.egg-info/PKG-INFO` & `swyft-0.4.2rc1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: swyft
-Version: 0.4.2
-Summary: Universal scalable simulation-based inference with TMNRE (Truncated Marginal Neural Ratio Estimation) and pytorch-lightning.
-Home-page: https://github.com/undark-lab/swyft
-License: MIT License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Environment :: GPU
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-Provides-Extra: docs
-License-File: LICENSE
-
 Swyft v0.4
 ==========
 
 .. image:: https://badge.fury.io/py/swyft.svg
    :target: https://badge.fury.io/py/swyft
    :alt: PyPI version
 
@@ -85,35 +63,14 @@
 * To this end, Swyft estimates likelihood-to-evidence ratios for arbitrary marginal posteriors; they typically require fewer simulations than the corresponding joint.
 * Swyft performs targeted inference by prior truncation, combining simulation efficiency with empirical testability.
 * Swyft is based on stochastic simulators, which map parameters stochastically to observational data. Swyft makes it convenient to define such simulators as graphical models.
 * In scientific settings, a cost-benefit analysis often favors approximating the posterior marginality; *swyft* provides this functionality.
 * The package additionally implements our prior truncation technique, routines to empirically test results by estimating the expected coverage, and a simulator manager with `zarr <https://zarr.readthedocs.io/en/stable/>`_ storage to simplify use with complex simulators.
 
 
-Papers using Swyft/TMNRE
-------------------------
-
-2021
-
-- “Fast and Credible Likelihood-Free Cosmology with Truncated Marginal Neural Ratio Estimation“ Cole+ https://arxiv.org/abs/2111.08030
-
-2022
-
-- “Estimating the warm dark matter mass from strong lensing images with truncated marginal neural ratio estimation” Anau Montel+, https://arxiv.org/abs/2205.09126
-- “SICRET: Supernova Ia Cosmology with truncated marginal neural Ratio EsTimation” Karchev+ https://arxiv.org/abs/2209.06733
-- “One never walks alone: the effect of the perturber population on subhalo measurements in strong gravitational lenses” Coogan+ https://arxiv.org/abs/2209.09918
-- “Detection is truncation: studying source populations with truncated marginal neural ratio estimation” Anau Montel+ https://arxiv.org/abs/2211.04291
-
-2023
-
-- “Debiasing Standard Siren Inference of the Hubble Constant with Marginal Neural Ratio Estimation” Gagnon-Hartman+ https://arxiv.org/abs/2301.05241
-- “Constraining the X-ray heating and reionization using 21-cm power spectra with Marginal Neural Ratio Estimation” Saxena+ https://arxiv.org/abs/2303.07339
-- “Peregrine: Sequential simulation-based inference for gravitational wave signals”, Bhardwaj+ https://arxiv.org/abs/2304.02035
-- “Albatross: A scalable simulation-based inference pipeline for analysing stellar streams in the Milky Way”, Alvey+ https://arxiv.org/abs/2304.02032
-
 
 Further information
 -------------------
 
 * **Documentation & installation**: https://swyft.readthedocs.io/
 * **Example usage**: https://swyft.readthedocs.io/en/latest/tutorial-notebooks.html
 * **Source code**: https://github.com/undark-lab/swyft
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `swyft-0.4.2/swyft.egg-info/SOURCES.txt` & `swyft-0.4.2rc1/swyft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swyft-0.4.2/tests/test_simulator.py` & `swyft-0.4.2rc1/tests/test_simulator.py`

 * *Files identical despite different names*

