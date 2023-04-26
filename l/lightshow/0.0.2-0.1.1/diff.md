# Comparing `tmp/lightshow-0.0.2.tar.gz` & `tmp/lightshow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightshow-0.0.2.tar", last modified: Fri Sep  9 20:43:08 2022, max compression
+gzip compressed data, was "lightshow-0.1.1.tar", last modified: Wed Apr 26 15:30:02 2023, max compression
```

## Comparing `lightshow-0.0.2.tar` & `lightshow-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,88 @@
--rw-r--r--   0        0        0      135 2022-08-23 20:54:26.781557 lightshow-0.0.2/.coveragerc
--rw-r--r--   0        0        0      288 2022-08-23 20:54:26.781795 lightshow-0.0.2/.flake8
--rw-r--r--   0        0        0     2966 2022-09-09 16:16:58.460235 lightshow-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2106 2022-08-18 15:12:24.554639 lightshow-0.0.2/.gitignore
--rw-r--r--   0        0        0      336 2022-08-23 20:54:26.782279 lightshow-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1099 2022-08-25 01:55:55.613305 lightshow-0.0.2/AUTHORS.rst
--rw-r--r--   0        0        0     3553 2022-08-18 15:13:20.282962 lightshow-0.0.2/LICENSE
--rw-r--r--   0        0        0     2875 2022-09-09 19:41:30.216354 lightshow-0.0.2/README.rst
--rw-r--r--   0        0        0     3660 2022-09-09 20:41:19.329457 lightshow-0.0.2/build.sh
--rw-r--r--   0        0        0      673 2022-08-18 15:12:24.555058 lightshow-0.0.2/docs/Makefile
--rw-r--r--   0        0        0   118686 2022-08-23 20:54:26.783348 lightshow-0.0.2/docs/_static/images/lightshow.jpg
--rw-r--r--   0        0        0      797 2022-08-18 15:12:24.555549 lightshow-0.0.2/docs/make.bat
--rw-r--r--   0        0        0        0 2022-08-18 15:12:24.555630 lightshow-0.0.2/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     6725 2022-09-09 16:21:18.435294 lightshow-0.0.2/docs/source/conf.py
--rw-r--r--   0        0        0      389 2022-09-09 19:42:56.866424 lightshow-0.0.2/docs/source/index.rst
--rw-r--r--   0        0        0      193 2022-08-18 15:13:20.284996 lightshow-0.0.2/docs/source/installation.rst
--rw-r--r--   0        0        0     1053 2022-08-18 15:12:24.555971 lightshow-0.0.2/docs/source/lightshow.parameters.rst
--rw-r--r--   0        0        0      559 2022-08-18 15:12:24.556017 lightshow-0.0.2/docs/source/lightshow.rst
--rw-r--r--   0        0        0       86 2022-08-18 15:13:20.285460 lightshow-0.0.2/docs/source/modules.rst
--rw-r--r--   0        0        0      337 2022-09-09 17:10:18.930245 lightshow-0.0.2/docs/source/project.rst
--rw-r--r--   0        0        0       34 2022-08-25 01:55:55.615722 lightshow-0.0.2/docs/source/project/authors.rst
--rw-r--r--   0        0        0      163 2022-08-25 01:55:55.616397 lightshow-0.0.2/docs/source/project/funding.rst
--rw-r--r--   0        0        0       47 2022-08-25 01:55:55.617028 lightshow-0.0.2/docs/source/project/license.rst
--rw-r--r--   0        0        0    21024 2022-08-25 01:55:55.618168 lightshow-0.0.2/docs/source/quickstart.rst
--rw-r--r--   0        0        0    92531 2022-08-18 15:13:20.286153 lightshow-0.0.2/figures/Lightshow_Workflow_Diagram.jpg
--rw-r--r--   0        0        0    25190 2022-08-18 15:13:20.286392 lightshow-0.0.2/figures/Lightshow_Workflow_Diagram.pdf
--rw-r--r--   0        0        0     1887 2022-09-09 20:43:07.819421 lightshow-0.0.2/lightshow/__init__.py
--rw-r--r--   0        0        0        0 2022-08-18 15:12:24.556837 lightshow-0.0.2/lightshow/_tests/__init__.py
--rw-r--r--   0        0        0     1187 2022-08-23 20:54:26.784971 lightshow-0.0.2/lightshow/_tests/conftest.py
--rw-r--r--   0        0        0       40 2022-08-23 20:54:26.785163 lightshow-0.0.2/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
--rw-r--r--   0        0        0       42 2022-08-23 20:54:26.785326 lightshow-0.0.2/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
--rw-r--r--   0        0        0       34 2022-08-23 20:54:26.785489 lightshow-0.0.2/lightshow/_tests/dummy_chpsp_files/O.fch.upf
--rw-r--r--   0        0        0       35 2022-08-23 20:54:26.785656 lightshow-0.0.2/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
--rw-r--r--   0        0        0      476 2022-08-18 15:12:24.557026 lightshow-0.0.2/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
--rw-r--r--   0        0        0      480 2022-08-18 15:12:24.557125 lightshow-0.0.2/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
--rw-r--r--   0        0        0       24 2022-08-23 20:54:26.785863 lightshow-0.0.2/lightshow/_tests/dummy_psp_files/O.mock.upf
--rw-r--r--   0        0        0       25 2022-08-23 20:54:26.786030 lightshow-0.0.2/lightshow/_tests/dummy_psp_files/Ti.mock.upf
--rw-r--r--   0        0        0      152 2022-08-23 20:54:26.786188 lightshow-0.0.2/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
--rw-r--r--   0        0        0        0 2022-08-23 20:54:26.786225 lightshow-0.0.2/lightshow/_tests/helpers/__init__.py
--rw-r--r--   0        0        0    11407 2022-08-23 20:54:26.786323 lightshow-0.0.2/lightshow/_tests/helpers/geometry.py
--rw-r--r--   0        0        0      376 2022-08-23 20:54:26.786442 lightshow-0.0.2/lightshow/_tests/structure_files/mp-10734/POSCAR
--rw-r--r--   0        0        0      198 2022-08-23 20:54:26.786523 lightshow-0.0.2/lightshow/_tests/structure_files/mp-1215/POSCAR
--rw-r--r--   0        0        0      814 2022-08-23 20:54:26.786601 lightshow-0.0.2/lightshow/_tests/structure_files/mp-1840/POSCAR
--rw-r--r--   0        0        0      284 2022-08-23 20:54:26.786682 lightshow-0.0.2/lightshow/_tests/structure_files/mp-2657/POSCAR
--rw-r--r--   0        0        0      167 2022-08-23 20:54:26.786767 lightshow-0.0.2/lightshow/_tests/structure_files/mp-2664/POSCAR
--rw-r--r--   0        0        0      287 2022-08-23 20:54:26.786867 lightshow-0.0.2/lightshow/_tests/structure_files/mp-390/POSCAR
--rw-r--r--   0        0        0      460 2022-08-23 20:54:26.786954 lightshow-0.0.2/lightshow/_tests/structure_files/mp-430/POSCAR
--rw-r--r--   0        0        0      403 2022-08-23 20:54:26.787032 lightshow-0.0.2/lightshow/_tests/structure_files/mp-458/POSCAR
--rw-r--r--   0        0        0      461 2022-08-23 20:54:26.787117 lightshow-0.0.2/lightshow/_tests/structure_files/mvc-11115/POSCAR
--rw-r--r--   0        0        0     3324 2022-08-23 20:54:26.787433 lightshow-0.0.2/lightshow/_tests/test_database.py
--rw-r--r--   0        0        0    12398 2022-08-23 20:54:26.787684 lightshow-0.0.2/lightshow/_tests/test_exciting.py
--rw-r--r--   0        0        0     1167 2022-08-23 20:54:26.787875 lightshow-0.0.2/lightshow/_tests/test_vasp.py
--rw-r--r--   0        0        0        0 2022-08-18 15:13:20.289584 lightshow-0.0.2/lightshow/common/__init__.py
--rw-r--r--   0        0        0     2517 2022-08-23 20:54:26.788024 lightshow-0.0.2/lightshow/common/kpoints.py
--rw-r--r--   0        0        0     3322 2022-08-23 20:54:26.788270 lightshow-0.0.2/lightshow/common/nbands.py
--rw-r--r--   0        0        0    21936 2022-09-06 17:08:21.403653 lightshow-0.0.2/lightshow/database.py
--rw-r--r--   0        0        0      602 2022-08-18 15:13:20.291074 lightshow-0.0.2/lightshow/defaults.py
--rw-r--r--   0        0        0        0 2022-08-18 15:12:24.559121 lightshow-0.0.2/lightshow/parameters/__init__.py
--rw-r--r--   0        0        0      206 2022-08-18 15:13:20.291409 lightshow-0.0.2/lightshow/parameters/_base.py
--rw-r--r--   0        0        0     9115 2022-08-23 20:54:26.788827 lightshow-0.0.2/lightshow/parameters/exciting.py
--rw-r--r--   0        0        0     7407 2022-08-18 15:13:20.293930 lightshow-0.0.2/lightshow/parameters/feff.py
--rw-r--r--   0        0        0    14221 2022-08-23 20:54:26.789088 lightshow-0.0.2/lightshow/parameters/ocean.py
--rw-r--r--   0        0        0    29415 2022-08-23 20:54:26.789280 lightshow-0.0.2/lightshow/parameters/vasp.py
--rw-r--r--   0        0        0    20109 2022-08-25 01:55:55.620779 lightshow-0.0.2/lightshow/parameters/xspectra.py
--rw-r--r--   0        0        0     2371 2022-08-23 20:54:26.789675 lightshow-0.0.2/lightshow/pymatgen_utils.py
--rw-r--r--   0        0        0   143428 2022-09-06 17:09:31.141086 lightshow-0.0.2/notebooks/00_basic_usage.ipynb
--rw-r--r--   0        0        0     2065 2022-09-09 20:34:42.700762 lightshow-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4587 1970-01-01 00:00:00.000000 lightshow-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-04-26 15:29:52.354047 lightshow-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      221 2023-04-26 15:29:52.354047 lightshow-0.1.1/.flake8
+-rw-r--r--   0        0        0     6310 2023-04-26 15:29:52.354047 lightshow-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2106 2023-04-26 15:29:52.354047 lightshow-0.1.1/.gitignore
+-rw-r--r--   0        0        0      336 2023-04-26 15:29:52.354047 lightshow-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1099 2023-04-26 15:29:52.354047 lightshow-0.1.1/AUTHORS.rst
+-rw-r--r--   0        0        0     1574 2023-04-26 15:29:52.354047 lightshow-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5427 2023-04-26 15:29:52.354047 lightshow-0.1.1/README.md
+-rw-r--r--   0        0        0      673 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/Makefile
+-rw-r--r--   0        0        0    60563 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/_static/images/lightshow.jpg
+-rw-r--r--   0        0        0   118686 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/_static/images/lightshow_old.jpg
+-rw-r--r--   0        0        0      797 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     6725 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     2023 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     1181 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     1053 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/lightshow.parameters.rst
+-rw-r--r--   0        0        0      559 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/lightshow.rst
+-rw-r--r--   0        0        0       86 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/modules.rst
+-rw-r--r--   0        0        0      337 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/project.rst
+-rw-r--r--   0        0        0       34 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/authors.rst
+-rw-r--r--   0        0        0     1720 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/funding.rst
+-rw-r--r--   0        0        0       47 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/license.rst
+-rw-r--r--   0        0        0    21003 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/quickstart.rst
+-rw-r--r--   0        0        0    92531 2023-04-26 15:29:52.358047 lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.jpg
+-rw-r--r--   0        0        0    25190 2023-04-26 15:29:52.358047 lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.pdf
+-rw-r--r--   0        0        0     1887 2023-04-26 15:30:01.814000 lightshow-0.1.1/lightshow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/conftest.py
+-rw-r--r--   0        0        0       40 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
+-rw-r--r--   0        0        0       42 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
+-rw-r--r--   0        0        0       34 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/O.fch.upf
+-rw-r--r--   0        0        0       35 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
+-rw-r--r--   0        0        0      476 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
+-rw-r--r--   0        0        0      480 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
+-rw-r--r--   0        0        0       24 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/O.mock.upf
+-rw-r--r--   0        0        0       25 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/Ti.mock.upf
+-rw-r--r--   0        0        0      152 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/helpers/__init__.py
+-rw-r--r--   0        0        0    11401 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/helpers/geometry.py
+-rw-r--r--   0        0        0       82 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/README.rst
+-rw-r--r--   0        0        0    42630 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/ene_dep_broad.txt
+-rw-r--r--   0        0        0    43441 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/gauss_broad.txt
+-rw-r--r--   0        0        0    43519 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/lorentz_broad.txt
+-rw-r--r--   0        0        0    43398 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/voigt_broad.txt
+-rw-r--r--   0        0        0      376 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-10734/POSCAR
+-rw-r--r--   0        0        0      198 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-1215/POSCAR
+-rw-r--r--   0        0        0      814 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-1840/POSCAR
+-rw-r--r--   0        0        0      284 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-2657/POSCAR
+-rw-r--r--   0        0        0      167 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-2664/POSCAR
+-rw-r--r--   0        0        0      287 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-390/POSCAR
+-rw-r--r--   0        0        0      460 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-430/POSCAR
+-rw-r--r--   0        0        0      403 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-458/POSCAR
+-rw-r--r--   0        0        0      461 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mvc-11115/POSCAR
+-rw-r--r--   0        0        0     1692 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/test_broaden.py
+-rw-r--r--   0        0        0     3372 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/test_database.py
+-rw-r--r--   0        0        0    12398 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/_tests/test_exciting.py
+-rw-r--r--   0        0        0     1166 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/_tests/test_vasp.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/__init__.py
+-rw-r--r--   0        0        0     2558 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/kpoints.py
+-rw-r--r--   0        0        0     3322 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/nbands.py
+-rw-r--r--   0        0        0    21933 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/database.py
+-rw-r--r--   0        0        0      602 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/defaults.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/_base.py
+-rw-r--r--   0        0        0     9115 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/exciting.py
+-rw-r--r--   0        0        0     7407 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/feff.py
+-rw-r--r--   0        0        0    14284 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/ocean.py
+-rw-r--r--   0        0        0    29413 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/vasp.py
+-rw-r--r--   0        0        0    19946 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/xspectra.py
+-rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/postprocess/__init__.py
+-rw-r--r--   0        0        0     8871 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/postprocess/broaden.py
+-rw-r--r--   0        0        0     2371 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/pymatgen_utils.py
+-rw-r--r--   0        0        0    32206 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/00_basic_usage.ipynb
+-rw-r--r--   0        0        0    10013 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/01_Ti_K_anatase_broaden.ipynb
+-rwxr-xr-x   0        0        0    41029 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_exciting.txt
+-rw-r--r--   0        0        0     3816 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_exp.txt
+-rw-r--r--   0        0        0    54210 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_ocean.txt
+-rw-r--r--   0        0        0     5000 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_theory_FEFF.txt
+-rw-r--r--   0        0        0  2000000 2023-04-26 15:29:52.374047 lightshow-0.1.1/notebooks/spectra_files/anatase_theory_VASP.txt
+-rwxr-xr-x   0        0        0    11578 2023-04-26 15:29:52.374047 lightshow-0.1.1/notebooks/spectra_files/anatase_xspectra.txt
+-rw-r--r--   0        0        0     2076 2023-04-26 15:29:52.374047 lightshow-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1204 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/README.rst
+-rw-r--r--   0        0        0      575 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/build_docs.sh
+-rw-r--r--   0        0        0      118 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/build_project.sh
+-rw-r--r--   0        0        0      943 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/install.sh
+-rw-r--r--   0        0        0     1076 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/update_version.sh
+-rw-r--r--   0        0        0     7154 1970-01-01 00:00:00.000000 lightshow-0.1.1/PKG-INFO
```

### Comparing `lightshow-0.0.2/.gitignore` & `lightshow-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/AUTHORS.rst` & `lightshow-0.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/Makefile` & `lightshow-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/_static/images/lightshow.jpg` & `lightshow-0.1.1/docs/_static/images/lightshow_old.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/make.bat` & `lightshow-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/source/conf.py` & `lightshow-0.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/source/lightshow.parameters.rst` & `lightshow-0.1.1/docs/source/lightshow.parameters.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/source/lightshow.rst` & `lightshow-0.1.1/docs/source/lightshow.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/docs/source/quickstart.rst` & `lightshow-0.1.1/docs/source/quickstart.rst`

 * *Files 1% similar despite different names*

```diff
@@ -289,22 +289,22 @@
 
 
 XSpectra
 --------
 
 .. note::
 
-    See `here <https://www.quantum-espresso.org/Doc/INPUT_XSpectra.txt>`__ for the OCEAN documentation.
+    See `here <https://www.quantum-espresso.org/Doc/INPUT_XSpectra.txt>`__ for the XSpectra documentation.
 
 The required primary arguments for the ``XSpectraParameters`` object are the ``cards`` and ``edge``. For example, the general ``XSpectraParameter`` object structure looks something like this:
  
 .. code-block:: python
 
     xspectra_params = XSpectraParameters(
-         cards={'QE': {'control': {'restart_mode': 'from_scratch', 'wf_collect': '.true.'},
+         cards={'QE': {'control': {'restart_mode': 'from_scratch'},
                        'electrons': {'conv_thr': 1e-08, 'mixing_beta': 0.4},
                        'system': {'degauss': 0.002, 'ecutrho': 320, 'ecutwfc': 40,
                                   'nspin': 1, 'occupations': 'smearing', 'smearing': 'gauss'}
                },
                 'XS': {'cut_occ': {'cut_desmooth': 0.3},
                        'input_xspectra': {'outdir': '../',
                        'prefix': 'pwscf',
```

### Comparing `lightshow-0.0.2/figures/Lightshow_Workflow_Diagram.jpg` & `lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/figures/Lightshow_Workflow_Diagram.pdf` & `lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.pdf`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/__init__.py` & `lightshow-0.1.1/lightshow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import environ
 
 
 # DO NOT CHANGE BELOW ---------------------------------------------------------
 # This is replaced at build time automatically during deployment and
 # installation. Replacing anything will mess that up and crash the entire
 # build.
-__version__ = '0.0.2'
+__version__ = '0.1.1'
 # DO NOT CHANGE ABOVE ---------------------------------------------------------
 
 
 def _get_API_key_from_environ():
     """Checks for an environment variable PMG_API_KEY. If does not exist,
     returns None.
```

### Comparing `lightshow-0.0.2/lightshow/_tests/conftest.py` & `lightshow-0.1.1/lightshow/_tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,20 @@
 from pathlib import Path
 import pytest
 
 from pymatgen.core.structure import Structure
 
 from lightshow import Database
 
-STRUCTURE_FILES_PATH = (
-    Path.cwd() / Path("lightshow") / Path("_tests") / Path("structure_files")
+STRUCTURE_FILES_PATH = Path(__file__).parent / Path("structure_files")
+
+SPECTRA_FILES_PATH = Path.cwd() / Path("notebooks") / Path("spectra_files")
+
+SAMPLE_FILES_PATH = (
+    Path.cwd() / Path("lightshow") / Path("_tests") / Path("sample_files")
 )
 
 
 @pytest.fixture
 def test_structure_names():
     return [
         "mp-390",
@@ -24,14 +28,15 @@
         "mp-458",
         "mp-10734",
     ]
 
 
 @pytest.fixture
 def database_from_file():
+    print("structure-files-path", STRUCTURE_FILES_PATH)
     dat = Database.from_files(
         STRUCTURE_FILES_PATH, filename="POSCAR", cleanup_paths=True
     )
     return deepcopy(dat)
 
 
 @pytest.fixture
@@ -50,7 +55,17 @@
 
 
 @pytest.fixture
 def mp_Structure_mp390():
     return Structure.from_file(
         STRUCTURE_FILES_PATH / Path("mp-390") / Path("POSCAR")
     )
+
+
+@pytest.fixture
+def spectra_file_directory():
+    return SPECTRA_FILES_PATH
+
+
+@pytest.fixture
+def sample_file_directory():
+    return SAMPLE_FILES_PATH
```

### Comparing `lightshow-0.0.2/lightshow/_tests/helpers/geometry.py` & `lightshow-0.1.1/lightshow/_tests/helpers/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,14 @@
     "Og": 118,
     "Uue": 119,
 }
 ATOMIC_NUMBERS = {value: key for key, value in ATOMIC_NUMBERS.items()}
 
 
 def read_FEFF_geometry(path, rounding=4):
-
     path = Path(path) / "feff.inp"
 
     with open(path, "r") as f:
         feff_lines = f.readlines()
     where_atoms = [
         ii for ii, xx in enumerate(feff_lines) if xx.startswith("ATOMS")
     ]
@@ -146,15 +145,14 @@
     atoms = [xx[4] for xx in feff_lines]
     distances = np.round([float(xx[5]) for xx in feff_lines], rounding)
 
     return {"atoms": atoms[1:], "distances": distances[1:]}
 
 
 def read_VASP_geometry(path, neighbor_radius=10.0, rounding=4):
-
     path = Path(path) / "POSCAR"
 
     # VASP POSCAR files are easy, only need data after line 8
     structure = IStructure.from_file(path)
     # vasp_coordinates = np.array([site.frac_coords for site in vasp_structure])
     # vasp_atoms = [site.specie.symbol for site in vasp_structure]
 
@@ -165,15 +163,14 @@
     return {
         "atoms": [xx[1] for xx in tmp],
         "distances": np.round([xx[0] for xx in tmp], rounding),
     }
 
 
 def read_OCEAN_geometry(path, neighbor_radius=10.0, rounding=4):
-
     path = Path(path) / "ocean.in"
 
     absorber = str(path.parts[-2])
 
     with open(path, "r") as f:
         ocean_lines = f.readlines()
     ocean_lines = [xx.strip() for xx in ocean_lines]
@@ -225,15 +222,14 @@
                 "distances": np.round([xx[0] for xx in tmp], rounding),
             }
         )
     return return_list
 
 
 def read_XSpectra_geometry(path, neighbor_radius=10.0, rounding=4):
-
     path = Path(path) / "es.in"
 
     with open(path, "r") as f:
         xspectra_lines = f.readlines()
     xspectra_lines = [xx.strip() for xx in xspectra_lines]
 
     # Parse the Xspectra lines... also a pain, just like OCEAN
@@ -285,15 +281,14 @@
     return {
         "atoms": [xx[1] for xx in tmp],
         "distances": np.round([xx[0] for xx in tmp], rounding),
     }
 
 
 def read_EXCITING_geometry(path, neighbor_radius=10.0, rounding=4):
-
     path = Path(path) / "input.xml"
     structure = ExcitingInput.from_file(path).structure
 
     # Get the absorbing index
     with open(path, "r") as f:
         exciting_lines = f.readlines()
     exciting_lines = [xx.strip() for xx in exciting_lines]
@@ -392,15 +387,14 @@
 
         all_data_OCEAN = _read_OCEAN_geometry(
             path_OCEAN, neighbor_radius=neighbor_radius, rounding=rounding
         )
 
         ocean_checks = []
         for data_OCEAN in all_data_OCEAN:
-
             if not (
                 data_OCEAN["atoms"][:first_n_distances]
                 == data_VASP["atoms"][:first_n_distances]
             ):
                 ocean_checks.append(False)
             else:
                 ocean_checks.append(True)
```

### Comparing `lightshow-0.0.2/lightshow/_tests/structure_files/mp-1840/POSCAR` & `lightshow-0.1.1/lightshow/_tests/structure_files/mp-1840/POSCAR`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/_tests/test_database.py` & `lightshow-0.1.1/lightshow/_tests/test_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     XSpectraParameters,
     EXCITINGParameters,
 )
 from lightshow.defaults import VASP_INCAR_DEFAULT_COREHOLE_POTENTIAL
 
 # Helper testing files
 sys.path.append(str(Path(__file__).parent.resolve() / Path("helpers")))
-from geometry import consistency_check  # noqa
+from geometry import consistency_check  # noqa  # type: ignore
 
 
 def test_database_from_disk(database_from_file, test_structure_names):
     dat = database_from_file
     dat.initialize_supercells(9.0)
     dat.initialize_inequivalent_sites()
     assert set(dat.structures.keys()) == set(test_structure_names)
@@ -57,19 +57,19 @@
     mpid,
     dummy_potcar_file_directory,
     dummy_psp_file_directory,
     dummy_chpsp_file_directory,
     database_from_file,
     tmp_path,
 ):
-
     # Load it all in
     dat = database_from_file
     dat.initialize_supercells(9.0)
     dat.initialize_inequivalent_sites()
+    print(dat.structures.keys())
     dat._supercells = {mpid: dat.supercells[mpid]}
     dat._structures = {mpid: dat.structures[mpid]}
     dat._metadata = {mpid: dat.metadata[mpid]}
 
     target = Path(tmp_path) / Path("iama") / Path("destination")
     target.mkdir(exist_ok=True, parents=True)
```

### Comparing `lightshow-0.0.2/lightshow/_tests/test_exciting.py` & `lightshow-0.1.1/lightshow/_tests/test_exciting.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         "gmaxvr",
         "lmaxmat",
         "lmaxvr",
         "lmaxapw",
     }, "Excpected groundstate keys differ from found keys."
     assert groundstate_xml.get("rgkmax") == "9.0"
     assert groundstate_xml.get("do") == "fromscratch"
-    assert groundstate_xml.get("ngridk") == "5 5 6"
+    assert groundstate_xml.get("ngridk") == "3 3 4"
     assert groundstate_xml.get("xctype") == "GGA_PBE"
     assert groundstate_xml.get("nempty") == "200"
     assert groundstate_xml.get("gmaxvr") == "25"
     assert groundstate_xml.get("lmaxmat") == "10"
     assert groundstate_xml.get("lmaxvr") == "10"
     assert groundstate_xml.get("lmaxapw") == "10"
 
@@ -139,22 +139,22 @@
         "gqmax",
         "vkloff",
         "tevout",
         "tappinfo",
         "ngridq",
     }, "Excpected xs keys differ from found keys."
     assert xs_xml.get("broad") == "0.0327069"
-    assert xs_xml.get("ngridk") == "5 5 6"
+    assert xs_xml.get("ngridk") == "3 3 4"
     assert xs_xml.get("xstype") == "BSE"
     assert xs_xml.get("nempty") == "150"
     assert xs_xml.get("gqmax") == "4.0"
     assert xs_xml.get("vkloff") == "0.05 0.03 0.13"
     assert xs_xml.get("tevout") == "true"
     assert xs_xml.get("tappinfo") == "true"
-    assert xs_xml.get("ngridq") == "5 5 6"
+    assert xs_xml.get("ngridq") == "3 3 4"
 
     xs_subelements = list(xs_xml)
     assert len(xs_subelements) == 5, "Expect xs tree to have 5 sub-elements"
 
     energywindow_xml = xs_subelements[0]
     assert (
         energywindow_xml.tag == "energywindow"
@@ -283,32 +283,32 @@
     assert (
         len(groundstate_xml.keys()) == 2
     ), "Excpect groundstate to have 2 attributes."
     assert set(groundstate_xml.keys()) == {
         "ngridk",
         "nempty",
     }, "Excpected groundstate keys differ from found keys."
-    assert groundstate_xml.get("ngridk") == "5 5 6"
+    assert groundstate_xml.get("ngridk") == "3 3 4"
     assert groundstate_xml.get("nempty") == "42"
 
     xs_xml = subelements[3]
     assert xs_xml.tag == "xs"
     assert len(xs_xml.keys()) == 5, "Excpect xs to have 4 attributes."
     assert set(xs_xml.keys()) == {
         "ngridk",
         "nempty",
         "ngridq",
         "xstype",
         "gqmax",
     }, "Excpected xs keys differ from found keys."
     assert xs_xml.get("gqmax") == "4.0"
-    assert xs_xml.get("ngridk") == "5 5 6"
+    assert xs_xml.get("ngridk") == "3 3 4"
     assert xs_xml.get("xstype") == "BSE"
     assert xs_xml.get("nempty") == "43"
-    assert xs_xml.get("ngridq") == "5 5 6"
+    assert xs_xml.get("ngridq") == "3 3 4"
 
     xs_subelements = list(xs_xml)
     assert len(xs_subelements) == 3, "Expect xs tree to have 3 sub-elements"
 
     energywindow_xml = xs_subelements[0]
     assert (
         energywindow_xml.tag == "energywindow"
```

### Comparing `lightshow-0.0.2/lightshow/_tests/test_vasp.py` & `lightshow-0.1.1/lightshow/_tests/test_vasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
 @pytest.mark.parametrize(
     "mpid",
     ["mp-390", "mvc-11115"],
 )
 def test_write(mpid, dummy_potcar_file_directory, database_from_file, tmp_path):
-
     # Load it all in
     dat = database_from_file
     dat.initialize_supercells(9.0)
     dat.initialize_inequivalent_sites()
     dat._supercells = {mpid: dat.supercells[mpid]}
     dat._structures = {mpid: dat.structures[mpid]}
     dat._metadata = {mpid: dat.metadata[mpid]}
```

### Comparing `lightshow-0.0.2/lightshow/common/kpoints.py` & `lightshow-0.1.1/lightshow/common/kpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+from ase.units import Bohr
 
 from monty.json import MSONable
 import numpy as np
 
 
 class _BaseKpointsMethod(ABC):
     @abstractmethod
@@ -48,17 +49,17 @@
         table for the effective radius (controlled by max_radii). The kmesh
         with radius right above the cutoff will be chosen. Default is 32
         Angstroms (60 Bohr).
     max_radii : float, optional
         Maximum radius used for constructing the lookup table.
     """
 
-    def __init__(self, cutoff=32.0, max_radii=50.0):
-        self._cutoff = cutoff
-        self._max_radii = max_radii
+    def __init__(self, cutoff=60.0, max_radii=80.0):
+        self._cutoff = cutoff * Bohr
+        self._max_radii = max_radii * Bohr
 
     def __call__(self, structure):
         klist = dict()
         rlatt = np.array(structure.lattice.reciprocal_lattice.abc)
 
         # TODO: why 10, 0.2?
         for xx in np.arange(0, 10, 0.2):
```

### Comparing `lightshow-0.0.2/lightshow/common/nbands.py` & `lightshow-0.1.1/lightshow/common/nbands.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/database.py` & `lightshow-0.1.1/lightshow/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from tqdm import tqdm
 
 from lightshow import _get_API_key_from_environ
 from lightshow import pymatgen_utils
 
 
 def _delete_common_strings(old_list_of_strings):
-
     list_of_strings = [str(Path(xx).parent) for xx in old_list_of_strings]
     list_of_names = [str(Path(xx).name) for xx in old_list_of_strings]
 
     commonprefix = os.path.commonprefix(list_of_strings)
     new_p = [x[len(commonprefix) :] for x in list_of_strings]
 
     # Reverse every string in the list then do it again
@@ -549,17 +548,15 @@
         }
 
         root = Path(root)
         root.mkdir(exist_ok=True, parents=True)
         writer_metadata_path = root / Path("writer_metadata.json")
 
         for key, supercell in tqdm(self._supercells.items(), disable=not pbar):
-
             for absorbing_atom in absorbing_atoms:
-
                 primitive_info = self._metadata[key]["primitive"]
                 supercell_info = self._metadata[key]["supercell"]
 
                 # If inequiv is None, that means that the absorbing_atom was not
                 # specified (absorbing_atom is None)
                 inequiv = self._get_site_indexes_matching_atom(
                     primitive_info, absorbing_atom
```

### Comparing `lightshow-0.0.2/lightshow/defaults.py` & `lightshow-0.1.1/lightshow/defaults.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/parameters/exciting.py` & `lightshow-0.1.1/lightshow/parameters/exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/parameters/feff.py` & `lightshow-0.1.1/lightshow/parameters/feff.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/lightshow/parameters/ocean.py` & `lightshow-0.1.1/lightshow/parameters/ocean.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
         nbands=UnitCellVolumeEstimate(e_range=30.0),
         bandgap=None,
         diel=None,
         defaultConvPerAtom=1e-10,
         edge="K",
         name="OCEAN",
     ):
-
         # Default cards for ocean
         self._cards = cards
 
         # User modified cards
         self._bandgap = bandgap
         self._diel = diel
 
@@ -308,14 +307,15 @@
 
             # ocean use a negative value to represent the number of
             # conduction bands
             cards["nbands"] = -1 * self._nbands(structure)
 
             # Standardized methods for getting the kpoints
             kmesh = self._kpoints(structure)
+            cards["nkpt"] = f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
             cards["ngkpt"] = f"{kmesh[0]} {kmesh[1]} {kmesh[2]}"
 
             # Determine the diemac
             if self._bandgap is not None or self._diel is not None:
                 if self._diel is not None:
                     cards["diemac"] = self._diel
                 elif self._bandgap is not None:
```

### Comparing `lightshow-0.0.2/lightshow/parameters/vasp.py` & `lightshow-0.1.1/lightshow/parameters/vasp.py`

 * *Files 0% similar despite different names*

```diff
@@ -511,15 +511,14 @@
             )
             return dont_exist
 
         return None
 
     @lru_cache(256)
     def _get_element_lines(self, element):
-
         # Get the element directory using the element as a key
         assert isinstance(element, str)
         element_dir = self._element_mapping[element]
 
         # Construct the path
         path = Path(self._root) / Path(element_dir) / Path("POTCAR")
 
@@ -769,15 +768,14 @@
         kpoints=GenericEstimatorKpoints(cutoff=32.0, max_radii=50.0),
         nbands=UnitCellVolumeEstimate(e_range=40.0),
         potcar_element_mapping=dict(),
         max_bands=-1,
         force_spin_unpolarized=False,
         name="VASP",
     ):
-
         if "NBANDS" in incar.keys():
             if incar["NBANDS"] is None and nbands is None:
                 raise ValueError(
                     "One of incar['NBANDS'] or the nbands argument must be "
                     "provided"
                 )
```

### Comparing `lightshow-0.0.2/lightshow/parameters/xspectra.py` & `lightshow-0.1.1/lightshow/parameters/xspectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from pathlib import Path
 import json
 import bz2
 import base64
 import shutil
 from warnings import warn
-from collections import OrderedDict
 
 from monty.json import MSONable
 from pymatgen.io.pwscf import PWInput
 
 from lightshow.parameters._base import _BaseParameters
 from lightshow.common.kpoints import GenericEstimatorKpoints
 from lightshow import (
     _get_CHPSP_DIRECTORY_from_environ,
     _get_PSP_DIRECTORY_from_environ,
 )
 
 XSPECTRA_DEFAULT_CARDS = {
     "QE": {
-        "control": {"restart_mode": "from_scratch", "wf_collect": ".true."},
+        "control": {"restart_mode": "from_scratch"},
         "electrons": {"conv_thr": 1e-08, "mixing_beta": 0.4},
         "system": {
             "degauss": 0.002,
             "ecutrho": 320,
             "ecutwfc": 40,
             "nspin": 1,
             "occupations": "smearing",
@@ -63,15 +62,14 @@
 
         .. code-block:: python
 
            cards = {
                     "QE": {
                         "control": {
                             "restart_mode": "from_scratch",
-                            "wf_collect": ".true."
                         },
                         "electrons": {"conv_thr": 1e-08, "mixing_beta": 0.4},
                         "system": {
                             "degauss": 0.002,
                             "ecutrho": 320,
                             "ecutwfc": 40,
                             "nspin": 1,
@@ -300,17 +298,15 @@
             "    calculation = 'xanes_%s'" % mode,
             "    edge = '" + XSparams["input_xspectra"]["edge"] + "'",
             "    prefix = 'pwscf'",
             "    outdir = '../'",
             "    xniter = " + str(XSparams["input_xspectra"]["xniter"]),
             "    xiabs = %d" % iabs,
             "    xerror = " + str(XSparams["input_xspectra"]["xerror"]),
-            "    xcoordcrys = '"
-            + XSparams["input_xspectra"]["xcoordcrys"]
-            + "'",
+            "    xcoordcrys = " + XSparams["input_xspectra"]["xcoordcrys"],
             "    xcheck_conv = "
             + str(XSparams["input_xspectra"]["xcheck_conv"]),
             "    xepsilon(1) = %d" % dirs[0],
             "    xepsilon(2) = %d" % dirs[1],
             "    xepsilon(3) = %d" % dirs[2],
         ]
 
@@ -462,29 +458,28 @@
 
         psp[f"{element}+"] = f"{element}.fch.upf"  # psp2[i]
         # copy core-hole potential and core wfn to target folder
         if self._chpsp_directory is not None:
             try:
                 shutil.copyfile(
                     self._chpsp_directory + f"/{element}.fch.upf",
-                    target_directory / Path("{element}.fch.upf"),
+                    target_directory / Path(f"{element}.fch.upf"),
                 )
                 shutil.copyfile(
                     self._chpsp_directory + f"/Core_{element}.wfc",
-                    target_directory / Path("Core_{element}.wfc"),
+                    target_directory / Path(f"Core_{element}.wfc"),
                 )
             except FileNotFoundError:
                 warn(
                     f"{element}.fch.upf or Core_{element}.wfc not found "
                     f"in {self._chpsp_directory}"
                 )
 
         # Determine iabs
-        psp = OrderedDict(psp)
-        for i, j in enumerate(psp.keys()):
+        for i, j in enumerate(sorted(psp.keys())):
             if j == symTarg + "+":
                 iabs = i + 1
         for site, specie in zip(sites, species):
             path = target_directory / Path(f"{site:03}_{specie}")
             path.mkdir(exist_ok=True, parents=True)
 
             structure[index_mapping[site]] = element + "+"
```

### Comparing `lightshow-0.0.2/lightshow/pymatgen_utils.py` & `lightshow-0.1.1/lightshow/pymatgen_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.0.2/pyproject.toml` & `lightshow-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     {"name" = "Christian Vorwerk"}
 ]
 maintainers = [
     {"name" = "Matthew R. Carbone", "email" = "mcarbone@bnl.gov"},
     {"name" = "Fanchen Meng", "email" = "fmeng1@bnl.gov"}
 ]
 description = "A one-stop-shop for writing computational spectroscopy input files"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.7"
 license = {"file" = "LICENSE"}
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Natural Language :: English",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
@@ -36,44 +36,44 @@
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
 ]
 dependencies = [
     "numpy",
     "tqdm",
     "monty",
-    "pymatgen",
+    "pymatgen<=2022.7.8",
     "ase"
 ]
 
 # Dynamic version reads __version__ directly from my_package.__init__
 dynamic = ["version"]
 
 # [tool.flit.sdist]
 # exclude = [
 #     "lightshow/_tests",
 #     "docs"
 # ]
 
 [project.optional-dependencies]
 test = [
-    "codecov",
     "coverage",
     "flake8",
     "pytest",
     "pytest-cov",
     "black",
     "nbstripout",
     "pre-commit",
 ]
 doc = [
     "sphinx",
     "numpydoc",
     "sphinx-copybutton",
     "sphinx_rtd_theme",
     "ipython",
+    "matplotlib"
 ]
 
 [tool.setuptools]
 packages = ["lightshow"]
 
 [tool.black]
 line-length = 80
```

