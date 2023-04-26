# Comparing `tmp/lightshow-0.1.1.tar.gz` & `tmp/lightshow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightshow-0.1.1.tar", last modified: Wed Apr 26 15:30:02 2023, max compression
+gzip compressed data, was "lightshow-0.1.2.tar", last modified: Wed Apr 26 16:58:26 2023, max compression
```

## Comparing `lightshow-0.1.1.tar` & `lightshow-0.1.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0      135 2023-04-26 15:29:52.354047 lightshow-0.1.1/.coveragerc
--rw-r--r--   0        0        0      221 2023-04-26 15:29:52.354047 lightshow-0.1.1/.flake8
--rw-r--r--   0        0        0     6310 2023-04-26 15:29:52.354047 lightshow-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2106 2023-04-26 15:29:52.354047 lightshow-0.1.1/.gitignore
--rw-r--r--   0        0        0      336 2023-04-26 15:29:52.354047 lightshow-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1099 2023-04-26 15:29:52.354047 lightshow-0.1.1/AUTHORS.rst
--rw-r--r--   0        0        0     1574 2023-04-26 15:29:52.354047 lightshow-0.1.1/LICENSE
--rw-r--r--   0        0        0     5427 2023-04-26 15:29:52.354047 lightshow-0.1.1/README.md
--rw-r--r--   0        0        0      673 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/Makefile
--rw-r--r--   0        0        0    60563 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/_static/images/lightshow.jpg
--rw-r--r--   0        0        0   118686 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/_static/images/lightshow_old.jpg
--rw-r--r--   0        0        0      797 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/make.bat
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     6725 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/conf.py
--rw-r--r--   0        0        0     2023 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/index.rst
--rw-r--r--   0        0        0     1181 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/installation.rst
--rw-r--r--   0        0        0     1053 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/lightshow.parameters.rst
--rw-r--r--   0        0        0      559 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/lightshow.rst
--rw-r--r--   0        0        0       86 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/modules.rst
--rw-r--r--   0        0        0      337 2023-04-26 15:29:52.354047 lightshow-0.1.1/docs/source/project.rst
--rw-r--r--   0        0        0       34 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/authors.rst
--rw-r--r--   0        0        0     1720 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/funding.rst
--rw-r--r--   0        0        0       47 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/project/license.rst
--rw-r--r--   0        0        0    21003 2023-04-26 15:29:52.358047 lightshow-0.1.1/docs/source/quickstart.rst
--rw-r--r--   0        0        0    92531 2023-04-26 15:29:52.358047 lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.jpg
--rw-r--r--   0        0        0    25190 2023-04-26 15:29:52.358047 lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.pdf
--rw-r--r--   0        0        0     1887 2023-04-26 15:30:01.814000 lightshow-0.1.1/lightshow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/conftest.py
--rw-r--r--   0        0        0       40 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
--rw-r--r--   0        0        0       42 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
--rw-r--r--   0        0        0       34 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/O.fch.upf
--rw-r--r--   0        0        0       35 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
--rw-r--r--   0        0        0      476 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
--rw-r--r--   0        0        0      480 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
--rw-r--r--   0        0        0       24 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/O.mock.upf
--rw-r--r--   0        0        0       25 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/Ti.mock.upf
--rw-r--r--   0        0        0      152 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/helpers/__init__.py
--rw-r--r--   0        0        0    11401 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/helpers/geometry.py
--rw-r--r--   0        0        0       82 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/README.rst
--rw-r--r--   0        0        0    42630 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/ene_dep_broad.txt
--rw-r--r--   0        0        0    43441 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/gauss_broad.txt
--rw-r--r--   0        0        0    43519 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/lorentz_broad.txt
--rw-r--r--   0        0        0    43398 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/sample_files/voigt_broad.txt
--rw-r--r--   0        0        0      376 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-10734/POSCAR
--rw-r--r--   0        0        0      198 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-1215/POSCAR
--rw-r--r--   0        0        0      814 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-1840/POSCAR
--rw-r--r--   0        0        0      284 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-2657/POSCAR
--rw-r--r--   0        0        0      167 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-2664/POSCAR
--rw-r--r--   0        0        0      287 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-390/POSCAR
--rw-r--r--   0        0        0      460 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-430/POSCAR
--rw-r--r--   0        0        0      403 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mp-458/POSCAR
--rw-r--r--   0        0        0      461 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/structure_files/mvc-11115/POSCAR
--rw-r--r--   0        0        0     1692 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/test_broaden.py
--rw-r--r--   0        0        0     3372 2023-04-26 15:29:52.358047 lightshow-0.1.1/lightshow/_tests/test_database.py
--rw-r--r--   0        0        0    12398 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/_tests/test_exciting.py
--rw-r--r--   0        0        0     1166 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/_tests/test_vasp.py
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/__init__.py
--rw-r--r--   0        0        0     2558 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/kpoints.py
--rw-r--r--   0        0        0     3322 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/common/nbands.py
--rw-r--r--   0        0        0    21933 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/database.py
--rw-r--r--   0        0        0      602 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/defaults.py
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/__init__.py
--rw-r--r--   0        0        0      206 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/_base.py
--rw-r--r--   0        0        0     9115 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/exciting.py
--rw-r--r--   0        0        0     7407 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/feff.py
--rw-r--r--   0        0        0    14284 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/ocean.py
--rw-r--r--   0        0        0    29413 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/vasp.py
--rw-r--r--   0        0        0    19946 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/parameters/xspectra.py
--rw-r--r--   0        0        0        0 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/postprocess/__init__.py
--rw-r--r--   0        0        0     8871 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/postprocess/broaden.py
--rw-r--r--   0        0        0     2371 2023-04-26 15:29:52.362047 lightshow-0.1.1/lightshow/pymatgen_utils.py
--rw-r--r--   0        0        0    32206 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/00_basic_usage.ipynb
--rw-r--r--   0        0        0    10013 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/01_Ti_K_anatase_broaden.ipynb
--rwxr-xr-x   0        0        0    41029 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_exciting.txt
--rw-r--r--   0        0        0     3816 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_exp.txt
--rw-r--r--   0        0        0    54210 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_ocean.txt
--rw-r--r--   0        0        0     5000 2023-04-26 15:29:52.362047 lightshow-0.1.1/notebooks/spectra_files/anatase_theory_FEFF.txt
--rw-r--r--   0        0        0  2000000 2023-04-26 15:29:52.374047 lightshow-0.1.1/notebooks/spectra_files/anatase_theory_VASP.txt
--rwxr-xr-x   0        0        0    11578 2023-04-26 15:29:52.374047 lightshow-0.1.1/notebooks/spectra_files/anatase_xspectra.txt
--rw-r--r--   0        0        0     2076 2023-04-26 15:29:52.374047 lightshow-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1204 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/README.rst
--rw-r--r--   0        0        0      575 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/build_docs.sh
--rw-r--r--   0        0        0      118 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/build_project.sh
--rw-r--r--   0        0        0      943 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/install.sh
--rw-r--r--   0        0        0     1076 2023-04-26 15:29:52.374047 lightshow-0.1.1/scripts/update_version.sh
--rw-r--r--   0        0        0     7154 1970-01-01 00:00:00.000000 lightshow-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-04-26 16:58:19.808681 lightshow-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      221 2023-04-26 16:58:19.808681 lightshow-0.1.2/.flake8
+-rw-r--r--   0        0        0     6310 2023-04-26 16:58:19.808681 lightshow-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2106 2023-04-26 16:58:19.808681 lightshow-0.1.2/.gitignore
+-rw-r--r--   0        0        0      336 2023-04-26 16:58:19.808681 lightshow-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1099 2023-04-26 16:58:19.808681 lightshow-0.1.2/AUTHORS.rst
+-rw-r--r--   0        0        0     1574 2023-04-26 16:58:19.808681 lightshow-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5427 2023-04-26 16:58:19.808681 lightshow-0.1.2/README.md
+-rw-r--r--   0        0        0      673 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/Makefile
+-rw-r--r--   0        0        0    60563 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/_static/images/lightshow.jpg
+-rw-r--r--   0        0        0   118686 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/_static/images/lightshow_old.jpg
+-rw-r--r--   0        0        0      797 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     6725 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/conf.py
+-rw-r--r--   0        0        0     2023 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/index.rst
+-rw-r--r--   0        0        0     1181 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/installation.rst
+-rw-r--r--   0        0        0     1053 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/lightshow.parameters.rst
+-rw-r--r--   0        0        0      559 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/lightshow.rst
+-rw-r--r--   0        0        0       86 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/modules.rst
+-rw-r--r--   0        0        0      337 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project.rst
+-rw-r--r--   0        0        0       34 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/authors.rst
+-rw-r--r--   0        0        0     1720 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/funding.rst
+-rw-r--r--   0        0        0       47 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/license.rst
+-rw-r--r--   0        0        0    21003 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/quickstart.rst
+-rw-r--r--   0        0        0    92531 2023-04-26 16:58:19.808681 lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.jpg
+-rw-r--r--   0        0        0    25190 2023-04-26 16:58:19.808681 lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.pdf
+-rw-r--r--   0        0        0     1887 2023-04-26 16:58:26.428712 lightshow-0.1.2/lightshow/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.808681 lightshow-0.1.2/lightshow/_tests/__init__.py
+-rw-r--r--   0        0        0     1540 2023-04-26 16:58:19.808681 lightshow-0.1.2/lightshow/_tests/conftest.py
+-rw-r--r--   0        0        0       40 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
+-rw-r--r--   0        0        0       42 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
+-rw-r--r--   0        0        0       34 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/O.fch.upf
+-rw-r--r--   0        0        0       35 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
+-rw-r--r--   0        0        0      476 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
+-rw-r--r--   0        0        0      480 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
+-rw-r--r--   0        0        0       24 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/O.mock.upf
+-rw-r--r--   0        0        0       25 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/Ti.mock.upf
+-rw-r--r--   0        0        0      152 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/helpers/__init__.py
+-rw-r--r--   0        0        0    11401 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/helpers/geometry.py
+-rw-r--r--   0        0        0       82 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/README.rst
+-rw-r--r--   0        0        0    42630 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/ene_dep_broad.txt
+-rw-r--r--   0        0        0    43441 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/gauss_broad.txt
+-rw-r--r--   0        0        0    43519 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/lorentz_broad.txt
+-rw-r--r--   0        0        0    43398 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/voigt_broad.txt
+-rw-r--r--   0        0        0      376 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-10734/POSCAR
+-rw-r--r--   0        0        0      198 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-1215/POSCAR
+-rw-r--r--   0        0        0      814 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-1840/POSCAR
+-rw-r--r--   0        0        0      284 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-2657/POSCAR
+-rw-r--r--   0        0        0      167 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-2664/POSCAR
+-rw-r--r--   0        0        0      287 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-390/POSCAR
+-rw-r--r--   0        0        0      460 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-430/POSCAR
+-rw-r--r--   0        0        0      403 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-458/POSCAR
+-rw-r--r--   0        0        0      461 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mvc-11115/POSCAR
+-rw-r--r--   0        0        0     1702 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_broaden.py
+-rw-r--r--   0        0        0     3372 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_database.py
+-rw-r--r--   0        0        0    12398 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_exciting.py
+-rw-r--r--   0        0        0     1166 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_vasp.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/__init__.py
+-rw-r--r--   0        0        0     2558 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/kpoints.py
+-rw-r--r--   0        0        0     3322 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/nbands.py
+-rw-r--r--   0        0        0    21933 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/database.py
+-rw-r--r--   0        0        0      602 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/defaults.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/__init__.py
+-rw-r--r--   0        0        0      206 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/_base.py
+-rw-r--r--   0        0        0     9115 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/exciting.py
+-rw-r--r--   0        0        0     7407 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/feff.py
+-rw-r--r--   0        0        0    14284 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/ocean.py
+-rw-r--r--   0        0        0    29413 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/vasp.py
+-rw-r--r--   0        0        0    19946 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/xspectra.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/postprocess/__init__.py
+-rw-r--r--   0        0        0     8977 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/postprocess/broaden.py
+-rw-r--r--   0        0        0     2371 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/pymatgen_utils.py
+-rw-r--r--   0        0        0    32206 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/00_basic_usage.ipynb
+-rw-r--r--   0        0        0    10037 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/01_Ti_K_anatase_broaden.ipynb
+-rwxr-xr-x   0        0        0    41029 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/spectra_files/anatase_exciting.txt
+-rw-r--r--   0        0        0     3816 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/spectra_files/anatase_exp.txt
+-rw-r--r--   0        0        0    54210 2023-04-26 16:58:19.816681 lightshow-0.1.2/notebooks/spectra_files/anatase_ocean.txt
+-rw-r--r--   0        0        0     5000 2023-04-26 16:58:19.816681 lightshow-0.1.2/notebooks/spectra_files/anatase_theory_FEFF.txt
+-rw-r--r--   0        0        0  2000000 2023-04-26 16:58:19.824681 lightshow-0.1.2/notebooks/spectra_files/anatase_theory_VASP.txt
+-rwxr-xr-x   0        0        0    11578 2023-04-26 16:58:19.824681 lightshow-0.1.2/notebooks/spectra_files/anatase_xspectra.txt
+-rw-r--r--   0        0        0     2076 2023-04-26 16:58:19.824681 lightshow-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1204 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/README.rst
+-rw-r--r--   0        0        0      575 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/build_docs.sh
+-rw-r--r--   0        0        0      118 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/build_project.sh
+-rw-r--r--   0        0        0      943 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/install.sh
+-rw-r--r--   0        0        0     1076 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/update_version.sh
+-rw-r--r--   0        0        0     7154 1970-01-01 00:00:00.000000 lightshow-0.1.2/PKG-INFO
```

### Comparing `lightshow-0.1.1/.github/workflows/ci.yml` & `lightshow-0.1.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/.gitignore` & `lightshow-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/AUTHORS.rst` & `lightshow-0.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/LICENSE` & `lightshow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/README.md` & `lightshow-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/Makefile` & `lightshow-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/_static/images/lightshow.jpg` & `lightshow-0.1.2/docs/_static/images/lightshow.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/_static/images/lightshow_old.jpg` & `lightshow-0.1.2/docs/_static/images/lightshow_old.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/make.bat` & `lightshow-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/conf.py` & `lightshow-0.1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/index.rst` & `lightshow-0.1.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/installation.rst` & `lightshow-0.1.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/lightshow.parameters.rst` & `lightshow-0.1.2/docs/source/lightshow.parameters.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/lightshow.rst` & `lightshow-0.1.2/docs/source/lightshow.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/project/funding.rst` & `lightshow-0.1.2/docs/source/project/funding.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/docs/source/quickstart.rst` & `lightshow-0.1.2/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.jpg` & `lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/figures/Lightshow_Workflow_Diagram.pdf` & `lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.pdf`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/__init__.py` & `lightshow-0.1.2/lightshow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import environ
 
 
 # DO NOT CHANGE BELOW ---------------------------------------------------------
 # This is replaced at build time automatically during deployment and
 # installation. Replacing anything will mess that up and crash the entire
 # build.
-__version__ = '0.1.1'
+__version__ = '0.1.2'
 # DO NOT CHANGE ABOVE ---------------------------------------------------------
 
 
 def _get_API_key_from_environ():
     """Checks for an environment variable PMG_API_KEY. If does not exist,
     returns None.
```

### Comparing `lightshow-0.1.1/lightshow/_tests/conftest.py` & `lightshow-0.1.2/lightshow/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/helpers/geometry.py` & `lightshow-0.1.2/lightshow/_tests/helpers/geometry.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/sample_files/ene_dep_broad.txt` & `lightshow-0.1.2/lightshow/_tests/sample_files/ene_dep_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/sample_files/gauss_broad.txt` & `lightshow-0.1.2/lightshow/_tests/sample_files/gauss_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/sample_files/lorentz_broad.txt` & `lightshow-0.1.2/lightshow/_tests/sample_files/lorentz_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/sample_files/voigt_broad.txt` & `lightshow-0.1.2/lightshow/_tests/sample_files/voigt_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/structure_files/mp-1840/POSCAR` & `lightshow-0.1.2/lightshow/_tests/structure_files/mp-1840/POSCAR`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/test_broaden.py` & `lightshow-0.1.2/lightshow/_tests/test_broaden.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     vasp_spectrum.broaden(x, method="Voigt", sigma=0.5, gamma=0.5)
 
     # ... using energy-dependent Voigt broadening
     vasp_spectrum.broaden(
         x,
         method="energy_dependent_voigt_broaden",
         sigma=0.2,
-        ld=40.0,
-        lt=TiK_core_hole_lifetime,
+        alpha=0.025,
+        lifetime=TiK_core_hole_lifetime,
     )
```

### Comparing `lightshow-0.1.1/lightshow/_tests/test_database.py` & `lightshow-0.1.2/lightshow/_tests/test_database.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/test_exciting.py` & `lightshow-0.1.2/lightshow/_tests/test_exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/_tests/test_vasp.py` & `lightshow-0.1.2/lightshow/_tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/common/kpoints.py` & `lightshow-0.1.2/lightshow/common/kpoints.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/common/nbands.py` & `lightshow-0.1.2/lightshow/common/nbands.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/database.py` & `lightshow-0.1.2/lightshow/database.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/defaults.py` & `lightshow-0.1.2/lightshow/defaults.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/parameters/exciting.py` & `lightshow-0.1.2/lightshow/parameters/exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/parameters/feff.py` & `lightshow-0.1.2/lightshow/parameters/feff.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/parameters/ocean.py` & `lightshow-0.1.2/lightshow/parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/parameters/vasp.py` & `lightshow-0.1.2/lightshow/parameters/vasp.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/parameters/xspectra.py` & `lightshow-0.1.2/lightshow/parameters/xspectra.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/lightshow/postprocess/broaden.py` & `lightshow-0.1.2/lightshow/postprocess/broaden.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,42 +89,42 @@
     """
 
     x1, x2 = np.meshgrid(x, xin)
     dx = xin[-1] - xin[0]
     return np.dot(voigt(x1 - x2, sigma, gamma / 2.0).T, yin) / len(xin) * dx
 
 
-def energy_dependent_voigt_broaden(x, xin, yin, sigma, ld, lt, ef):
+def energy_dependent_voigt_broaden(x, xin, yin, sigma, alpha, lifetime, efermi):
     """See ``voigt_broaden``. Performs a similar broadening only with an
     energy-dependent Lorentzian gamma term.
 
     Parameters
     ----------
     x : numpy.ndarray
         The output energy grid.
     xin : numpy.ndarray
         The input energy grid.
     yin : numpy.ndarray
         The input spectrum.
     sigma : float
         Voigt broadening sigma.
-    ld : TYPE
-        Description
-    lt : TYPE
-        Description
-    ef : TYPE
-        Description
+    alpha : float
+        Parameter alpha in the energy dependent broadening function
+    lifetime : float
+        Core-hole lifetime
+    efermi : float
+        Fermi energy
 
     Returns
     -------
     numpy.ndarray
     """
 
     x1, x2 = np.meshgrid(x, xin)
-    gamma = lt + np.heaviside(x2 - ef, 1) * (x2 - ef) / ld
+    gamma = lifetime + np.heaviside(x2 - efermi, 1) * (x2 - efermi) * alpha
     dx = xin[-1] - xin[0]
     return np.dot(voigt(x1 - x2, sigma, gamma / 2.0).T, yin) / len(xin) * dx
 
 
 def get_shift_by_maxima(exp, theory):
     exp_x = exp[:, 0].copy()
     exp_y = exp[:, 1].copy()
@@ -261,15 +261,15 @@
             )
         elif method == "energy_dependent_voigt_broaden":
             res = energy_dependent_voigt_broaden(
                 xout,
                 xin,
                 yin,
                 *broadening_args,
-                ef=self._e_fermi,
+                efermi=self._e_fermi,
                 **broadening_kwargs,
             )
         else:
             raise ValueError(f"Uknown method {method}")
         self._broadening_kwargs = broadening_kwargs
         return res
```

### Comparing `lightshow-0.1.1/lightshow/pymatgen_utils.py` & `lightshow-0.1.2/lightshow/pymatgen_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/00_basic_usage.ipynb` & `lightshow-0.1.2/notebooks/00_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/01_Ti_K_anatase_broaden.ipynb` & `lightshow-0.1.2/notebooks/01_Ti_K_anatase_broaden.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973876191324108%*

 * *Differences: {"'cells'": "{21: {'source': {insert: [(21, '    alpha=0.025,\\n'), (22, '    "*

 * *            "lifetime=TiK_core_hole_lifetime\\n')], delete: [22, 21]}}, 22: {'source': {insert: "*

 * *            '[(0, \'fig, ax = plt.subplots(1, 1, figsize=(4, 2))\\n\'), (7, "ax.plot(x, '*

 * *            "vasp_spectrum_EDV_broadened, label=r'VASP (EDV; "*

 * *            '$\\\\sigma=0.2;\\\\alpha=0.025$)\')\\n")], delete: [7, 0]}}, 23: {\'source\': '*

 * *            "{insert: [(0, '#### There are some issues here:\\n')], delete: [0]}}}",*

 * * "' […]*

```diff
@@ -261,36 +261,36 @@
                 "vasp_spectrum_V_broadened = vasp_spectrum.broaden(x, method=\"Voigt\", sigma=0.5, gamma=0.5)\n",
                 "\n",
                 "# ... using energy-dependent Voigt broadening\n",
                 "vasp_spectrum_EDV_broadened = vasp_spectrum.broaden(\n",
                 "    x,\n",
                 "    method=\"energy_dependent_voigt_broaden\",\n",
                 "    sigma=0.2,\n",
-                "    ld=40.0,\n",
-                "    lt=TiK_core_hole_lifetime\n",
+                "    alpha=0.025,\n",
+                "    lifetime=TiK_core_hole_lifetime\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "130c3950-9677-4c34-a2a7-9ee95f95b066",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "fig, ax = plt.subplots(1, 1, figsize=(2, 1))\n",
+                "fig, ax = plt.subplots(1, 1, figsize=(4, 2))\n",
                 "\n",
                 "ax.plot(experimental_spectrum[:, 0], experimental_spectrum[:, 1], label='Experiment')\n",
                 "ax.plot(vasp_spectrum.spectrum[:, 0], vasp_spectrum.spectrum[:, 1], label='VASP')\n",
                 "ax.plot(x, vasp_spectrum_G_broadened, label=r'VASP (G; $\\sigma=1$)')\n",
                 "ax.plot(x, vasp_spectrum_L_broadened, label=r'VASP (L; $\\gamma=1$)')\n",
                 "ax.plot(x, vasp_spectrum_V_broadened, label=r'VASP (V; $\\gamma=\\sigma=0.5$)')\n",
-                "ax.plot(x, vasp_spectrum_EDV_broadened, label=r'VASP (EDV; $\\sigma=0.2;...$)')\n",
+                "ax.plot(x, vasp_spectrum_EDV_broadened, label=r'VASP (EDV; $\\sigma=0.2;\\alpha=0.025$)')\n",
                 "\n",
                 "\n",
                 "ax.legend(frameon=False, bbox_to_anchor=(1, 0.5), loc=\"center left\", fontsize=6)\n",
                 "ax.set_ylabel(\"$\\mu(E)$ (a.u.)\")\n",
                 "ax.set_xlabel(\"$E$ (eV)\")\n",
                 "ax.set_xlim(4960, 5010)\n",
                 "\n",
@@ -298,15 +298,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "9a385279-ed73-4641-995d-7185eecbd36b",
             "metadata": {},
             "source": [
-                "There are some issues here:\n",
+                "#### There are some issues here:\n",
                 "1. The broadening parameter is not necessarily correct.\n",
                 "2. Even after doing the align-by-maxima procedure, the spectra are clearly not aligned (look at the edge locations).\n",
                 "\n",
                 "We will address these problems in the future!"
             ]
         }
     ],
@@ -322,13 +322,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.16"
+            "version": "3.8.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_exciting.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_exciting.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_exp.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_exp.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_ocean.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_ocean.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_theory_FEFF.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_theory_FEFF.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_theory_VASP.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_theory_VASP.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/notebooks/spectra_files/anatase_xspectra.txt` & `lightshow-0.1.2/notebooks/spectra_files/anatase_xspectra.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/pyproject.toml` & `lightshow-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/scripts/README.rst` & `lightshow-0.1.2/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/scripts/build_docs.sh` & `lightshow-0.1.2/scripts/build_docs.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/scripts/install.sh` & `lightshow-0.1.2/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/scripts/update_version.sh` & `lightshow-0.1.2/scripts/update_version.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.1/PKG-INFO` & `lightshow-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightshow
-Version: 0.1.1
+Version: 0.1.2
 Summary: A one-stop-shop for writing computational spectroscopy input files
 Author: Benedikt Maurer, Fabien Peschel, Eli Stavitski, Xiaohui Qu, John T. Vinson, Christian Vorwerk
 Author-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>, Deyu Lu <dlu@bnl.gov>
 Maintainer-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
```

