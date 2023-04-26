# Comparing `tmp/nef_pipelines-0.1.35.tar.gz` & `tmp/nef_pipelines-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.35.tar", last modified: Wed Apr 19 09:39:51 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.36.tar", last modified: Wed Apr 26 21:20:08 2023, max compression
```

## Comparing `nef_pipelines-0.1.35.tar` & `nef_pipelines-0.1.36.tar`

### file list

```diff
@@ -1,341 +1,351 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.540081 nef_pipelines-0.1.35/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.205764 nef_pipelines-0.1.35/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.304113 nef_pipelines-0.1.35/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.35/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.366172 nef_pipelines-0.1.35/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.35/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.35/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.35/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.403982 nef_pipelines-0.1.35/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.35/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.35/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.35/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      404 2023-04-17 20:49:49.000000 nef_pipelines-0.1.35/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.35/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.35/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.35/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3011 2023-04-17 21:10:39.000000 nef_pipelines-0.1.35/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.35/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.35/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-19 09:39:51.540403 nef_pipelines-0.1.35/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.35/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.35/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.35/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.450360 nef_pipelines-0.1.35/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.35/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.35/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.35/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.35/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-04-19 09:39:51.543213 nef_pipelines-0.1.35/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.35/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.206586 nef_pipelines-0.1.35/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.515905 nef_pipelines-0.1.35/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.35/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.637229 nef_pipelines-0.1.35/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.35/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.715176 nef_pipelines-0.1.35/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2782 2023-04-17 20:22:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14630 2023-04-17 20:22:42.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    19514 2023-03-18 23:11:49.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3828 2023-03-19 15:41:24.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8776 2023-02-05 14:12:26.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.717756 nef_pipelines-0.1.35/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.35/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-03-24 21:55:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.720708 nef_pipelines-0.1.35/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.757407 nef_pipelines-0.1.35/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.779415 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.798304 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.804571 nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.842146 nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.848488 nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.859262 nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.893903 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.903457 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.930232 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.955706 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.003287 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.090544 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14354 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.155076 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.492427 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.523169 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.527792 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.534904 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.603557 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.618888 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.623727 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.631148 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.707838 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.785227 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7643 2023-03-18 23:11:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.790965 nef_pipelines-0.1.35/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.847441 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:50.986129 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.017302 nef_pipelines-0.1.35/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.052988 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2592 2022-12-13 19:17:42.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.118733 nef_pipelines-0.1.35/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.140576 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.148247 nef_pipelines-0.1.35/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.164938 nef_pipelines-0.1.35/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7082 2023-04-18 16:38:05.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.187065 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.203802 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.207485 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.210511 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.214041 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.217545 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-01-16 22:41:06.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.222362 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.271064 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.276058 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11481 2023-03-19 00:07:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.288521 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.322185 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3373 2023-02-07 21:14:19.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3019 2023-02-07 21:08:19.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20232 2022-11-27 19:45:21.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.333335 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.345533 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.395139 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2196 2022-11-27 19:45:21.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5647 2023-02-07 23:05:11.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.398068 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.405402 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.407675 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.410729 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.413599 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.444554 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.448480 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.453163 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6315 2023-02-08 23:35:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.456539 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      727 2023-03-20 21:00:52.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.461786 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17136 2023-03-24 20:03:59.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.492044 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14367 2023-03-21 20:30:29.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.495797 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.499113 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.505858 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.516944 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:51.538338 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-19 09:39:49.594331 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    12685 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-04-19 09:39:49.000000 nef_pipelines-0.1.35/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.35/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.912728 nef_pipelines-0.1.36/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.673779 nef_pipelines-0.1.36/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.770862 nef_pipelines-0.1.36/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.36/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.796636 nef_pipelines-0.1.36/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.36/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.36/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.36/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.800645 nef_pipelines-0.1.36/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.36/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.36/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.36/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.36/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.36/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.36/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.36/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     3273 2023-04-26 21:19:20.000000 nef_pipelines-0.1.36/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.36/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.36/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-26 21:20:08.913052 nef_pipelines-0.1.36/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.36/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.36/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.36/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.807401 nef_pipelines-0.1.36/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.36/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.36/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.36/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.36/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-04-26 21:20:08.916120 nef_pipelines-0.1.36/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.36/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.675904 nef_pipelines-0.1.36/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.827436 nef_pipelines-0.1.36/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.36/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.869802 nef_pipelines-0.1.36/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-01-31 10:45:30.000000 nef_pipelines-0.1.36/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.928075 nef_pipelines-0.1.36/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16143 2023-04-15 16:57:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15012 2023-04-26 21:06:25.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    21105 2023-04-24 21:14:52.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4039 2023-04-26 20:02:21.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.931222 nef_pipelines-0.1.36/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22250 2023-04-17 20:19:05.000000 nef_pipelines-0.1.36/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5239 2023-03-24 21:55:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.934737 nef_pipelines-0.1.36/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.952108 nef_pipelines-0.1.36/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.971845 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.976745 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.983851 nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.986508 nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.989524 nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.993532 nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.004660 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.008061 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1123 2023-04-15 16:57:25.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.035603 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.038255 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.075116 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.118288 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.164518 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.218197 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.224823 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.241103 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.243072 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.284147 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.286176 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.292067 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.302660 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.374039 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3706 2023-04-26 21:12:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.423957 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/test_test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.430900 nef_pipelines-0.1.36/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.452161 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.487380 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.541858 nef_pipelines-0.1.36/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.563433 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.571415 nef_pipelines-0.1.36/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.596783 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6996 2023-04-15 16:55:03.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.603378 nef_pipelines-0.1.36/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.608698 nef_pipelines-0.1.36/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7095 2023-04-26 16:43:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.36/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.611215 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.611749 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.619720 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.623649 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.627429 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.645661 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.651884 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.667330 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.671324 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.693966 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.702194 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.709873 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.742799 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.755349 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.757379 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.767506 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10789 2023-01-30 23:23:18.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.769141 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.785138 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.791123 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.794997 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.820840 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.823324 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.825573 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.831964 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17216 2023-04-24 20:34:09.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.854610 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    19475 2023-04-26 21:11:26.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.881092 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.887937 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.895685 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.902093 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:08.911217 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-04-26 21:20:07.845259 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    13321 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-04-26 21:20:07.000000 nef_pipelines-0.1.36/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.36/tox.ini
```

### Comparing `nef_pipelines-0.1.35/.github/workflows/ci.yml` & `nef_pipelines-0.1.36/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.36/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/.pre-commit-config.yaml` & `nef_pipelines-0.1.36/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/CHANGELOG.md` & `nef_pipelines-0.1.36/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -85,36 +85,53 @@
 
 added support for reading MARS shift files
 
 
 ## version 0.1.28
 
 added an about command for information about the project
+
 added support for export xcamshift chemical shift restraint files
+
 added export of mars connected pseudo residue file
 
 ## version 0.1.29
 
 correct error in mars export fragments (mars connected pseudo residue file)
 
 ## version 0.1.30
 
 add support for writing sparky peak lists
 
 ## version 0.1.31
 
 add rudimentary rpf shift list exporter
+
 add a sparky peak list importer [alpha no tests]
 
 ## version 0.1.32
 
 patches to rpf exporter
 
 ##  version 0.1.33
 
 add the ability to rename nef frames
+
 add a verbose option to about [lists os and python versions]
+
 add the ability to suppress assignment height and volume columns in sparky peak export
 
 ## version 0.1.34
 
 shifts make peaks now has test suite
+
+## version 0.1.35
+
+minor cleanups
+
+## version 0.1.36
+
+initial support for RNA and DNA added (only surfaced in the sparky importers)
+
+sparky sequence import including RNA and DNA
+
+sparky peak import fully supported with all fields shown in the spark manual
```

### Comparing `nef_pipelines-0.1.35/CONTRIBUTING.md` & `nef_pipelines-0.1.36/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/LICENSE.txt` & `nef_pipelines-0.1.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/PKG-INFO` & `nef_pipelines-0.1.36/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nef_pipelines
-Version: 0.1.35
+Name: nef-pipelines
+Version: 0.1.36
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.35/README.md` & `nef_pipelines-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/TODO.md` & `nef_pipelines-0.1.36/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.36/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.36/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/release_to_pypi.sh` & `nef_pipelines-0.1.36/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/setup.cfg` & `nef_pipelines-0.1.36/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/setup.py` & `nef_pipelines-0.1.36/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.36/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 SF_CATEGORY = f"{SF}_category"
 SF_FRAMECODE = f"{SF}_framecode"
 NUM_DIMENSIONS = "num_dimensions"
 CHEMICAL_SHIFT_LIST = "chemical_shift_list"
 EXPERIMENT_TYPE = "experiment_type"
 EXPERIMENT_CLASSIFICATION = "experiment_classification"
+CCPN_COMMENT = "ccpn_comment"
 
 SPECTRUM_FRAME_TAGS = (
     SF_CATEGORY,
     SF_FRAMECODE,
     NUM_DIMENSIONS,
     CHEMICAL_SHIFT_LIST,
     EXPERIMENT_CLASSIFICATION,
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/peak_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from nef_pipelines.lib.isotope_lib import GAMMA_RATIOS, Isotope
 from nef_pipelines.lib.nef_frames_lib import (
     ABSOLUTE_PEAK_POSITIONS,
     ATOM_NAME,
     ATOM_NAME__DIMENSION_INDEX,
     AXIS_CODE,
     AXIS_UNIT,
+    CCPN_COMMENT,
     CHAIN_CODE,
     CHAIN_CODE__DIMENSION_INDEX,
     CHEMICAL_SHIFT_LIST,
     DIMENSION__DIMENSION_INDEX,
     DIMENSION_ID,
     DIMENSION_INDEX,
     DIMENSION_LOOP_TAGS,
@@ -197,14 +198,20 @@
     frame_code = f"{SPECTRUM_FRAME_CATEGORY}_{frame_code}"
 
     frame = Saveframe.from_scratch(frame_code, SPECTRUM_FRAME_CATEGORY)
 
     frame.add_tag(SF_CATEGORY, SPECTRUM_FRAME_CATEGORY)
     frame.add_tag(SF_FRAMECODE, frame_code)
 
+    have_comments = False
+    for peak in peaks:
+        if peak.comment != "":
+            have_comments = True
+            break
+
     peak_dimensions = []
     for peak in peaks:
         peak_dimensions.append(len(peak.shifts))
 
     peak_dimensions.sort()
     peak_dimensions = remove_duplicates_stable(peak_dimensions)
 
@@ -305,14 +312,16 @@
             ]
         )
 
     peak_loop = Loop.from_scratch(SPECTRUM_PEAK_LOOP_CATEGORY)
     frame.add_loop(peak_loop)
 
     peak_loop_tags = _expand_templates(PEAK_LOOP_TAGS, dimension_indices)
+    if have_comments:
+        peak_loop_tags.append(CCPN_COMMENT)
 
     peak_loop.add_tag(peak_loop_tags)
 
     for index, peak in enumerate(peaks):
         peak_data = {
             INDEX: index,
             PEAK_ID: index,
@@ -339,14 +348,19 @@
             peak_data[
                 POSITION__DIMENSION_INDEX.format(dimension_index=dim_index)
             ] = shift.value
             peak_data[
                 POSITION_UNCERTAINTY__DIMENSION_INDEX.format(dimension_index=dim_index)
             ] = shift.value_uncertainty
 
+            if have_comments:
+                peak_data[CCPN_COMMENT] = (
+                    peak.comment if peak.comment is not None else UNUSED
+                )
+
         peak_loop.add_data(
             [
                 peak_data,
             ]
         )
 
     return frame
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/sequence_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 import string
 from collections import Counter
 from dataclasses import replace
+from enum import auto
 from pathlib import Path
 from textwrap import dedent
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 from ordered_set import OrderedSet
 from pynmrstar import Entry, Loop, Saveframe
+from strenum import LowercaseStrEnum
 
 from nef_pipelines.lib.constants import NEF_UNKNOWN
 from nef_pipelines.lib.nef_lib import UNUSED, loop_row_namespace_iter
 
 # from nef_pipelines.lib.nef_lib import loop_to_dataframe
 from nef_pipelines.lib.structures import AtomLabel, Linking, SequenceResidue
 from nef_pipelines.lib.util import (
     chunks,
     exit_error,
     get_display_file_name,
     is_int,
     read_from_file_or_exit,
 )
 
+
+class MoleculeType(LowercaseStrEnum):
+    PROTEIN = auto()
+    RNA = auto()
+    DNA = auto()
+    CARBOH = auto()
+
+
 NEF_CHAIN_CODE = "chain_code"
 ANY_CHAIN = "_"
 
 
 def chain_code_iter(
-    user_chain_codes: Union[str, List[str]] = "", exclude: Union[str, List[str]] = ()
+    user_chain_codes: List[str] = "", exclude: List[str] = ()
 ) -> Iterable[str]:
     """
-    split input string into chain codes separated by .s, and yield them.
-    Then yield any remaining letters of the upper case alphabet till they run out
+    Yield chain codes in user chain codes and once exhausted yield any remaining letters of the upper case alphabet
+    till they run out. A list of chain codes to not use can be provided...
 
     Args:
-        user_chain_codes (str):  string of dot separated chain codes
+        user_chain_codes (str):  string of dot separated chain codes or a list of chain codes
         exclude: chain codes to not include in the iteration
 
     Returns:
         Iterable[str] single codes
     """
 
     ascii_uppercase = list(string.ascii_uppercase)
 
-    if isinstance(user_chain_codes, str):
-        if "." in user_chain_codes:
-            user_chain_codes = user_chain_codes.split(".")
-
-    if isinstance(exclude, str):
-        if "." in exclude:
-            exclude = exclude.split(".")
-
-    chain_codes = user_chain_codes if user_chain_codes else ascii_uppercase
-
     seen_codes = set()
 
-    for chain_code in chain_codes:
+    for chain_code in user_chain_codes:
         seen_codes.add(chain_code)
         if chain_code not in exclude:
             yield chain_code
 
     for chain_code in ascii_uppercase:
         if chain_code not in seen_codes and chain_code not in exclude:
             yield chain_code
@@ -156,15 +156,30 @@
         nef_loop.add_data_by_tag("linking", linking)
         nef_loop.add_data_by_tag("residue_variant", NEF_UNKNOWN)
         nef_loop.add_data_by_tag("cis_peptide", NEF_UNKNOWN)
 
     return nef_frame
 
 
-TRANSLATIONS_3_1 = {
+class MoleculeTypes(LowercaseStrEnum):
+    PROTEIN = auto()
+    DNA = auto()
+    RNA = auto()
+    CARBOH = auto()
+    LIGAND = auto()
+    OTHER = auto()
+
+
+TRANSLATIONS_3_1_DNA = {"DG": "G", "DC": "C", "DT": "T", "DA": "A"}
+TRANSLATIONS_1_3_DNA = {value: key for (key, value) in TRANSLATIONS_3_1_DNA.items()}
+
+TRANSLATIONS_3_1_RNA = {"G": "G", "C": "C", "A": "A", "U": "U", "I": "I"}
+TRANSLATIONS_1_3_RNA = {value: key for (key, value) in TRANSLATIONS_3_1_RNA.items()}
+
+TRANSLATIONS_3_1_PROTEIN = {
     "ALA": "A",
     "ARG": "R",
     "ASN": "N",
     "ASP": "D",
     "CYS": "C",
     "GLU": "E",
     "GLN": "Q",
@@ -178,45 +193,68 @@
     "PRO": "P",
     "SER": "S",
     "THR": "T",
     "TRP": "W",
     "TYR": "Y",
     "VAL": "V",
 }
-TRANSLATIONS_1_3 = {value: key for (key, value) in TRANSLATIONS_3_1.items()}
+TRANSLATIONS_1_3_PROTEIN = {
+    value: key for (key, value) in TRANSLATIONS_3_1_PROTEIN.items()
+}
+
+TRANSLATIONS_1_3 = {
+    MoleculeTypes.PROTEIN: TRANSLATIONS_1_3_PROTEIN,
+    MoleculeTypes.DNA: TRANSLATIONS_1_3_DNA,
+    MoleculeTypes.RNA: TRANSLATIONS_1_3_RNA,
+    MoleculeTypes.CARBOH: None,
+    MoleculeTypes.OTHER: None,
+    MoleculeTypes.LIGAND: None,
+}
+TRANSLATIONS_3_1 = {
+    MoleculeTypes.PROTEIN: TRANSLATIONS_3_1_PROTEIN,
+    MoleculeTypes.DNA: TRANSLATIONS_3_1_DNA,
+    MoleculeTypes.RNA: TRANSLATIONS_3_1_RNA,
+    MoleculeTypes.CARBOH: None,
+    MoleculeTypes.OTHER: None,
+    MoleculeTypes.LIGAND: None,
+}
 
 
 class BadResidue(Exception):
     """
     Bad residue found in a sequence
     """
 
     pass
 
 
 def translate_1_to_3(
-    sequence: str,
-    translations: Dict[str, str] = TRANSLATIONS_1_3,
-    unknown: Optional[str] = None,
+    sequence: str, molecule_type=MoleculeTypes.PROTEIN, unknown: Optional[str] = None
 ) -> List[str]:
     """
     Translate a 1 letter sequence to a 3 letter sequence
     Args:
         sequence (str): 1 letter sequence
-        translations (Dict[str, str]): a list of translations for single amino acid codes to 3 letter residue names
+        molecule_type (MoleculeTypes): type of molecule to translate residue types
         unknown (Optional[str]): optional name for residues if they are unknown, if set no error is raised if a
                                  1 letter residue name is not recognised
     Returns List[str]:
         a list of 3 residue codes
+        :param type:
 
     """
+
+    translations = TRANSLATIONS_1_3[molecule_type]
+
     result = []
     for i, residue_name_1let in enumerate(sequence):
         residue_name_1let = residue_name_1let.upper()
-        if residue_name_1let in translations:
+        if translations is None:
+            result.append(residue_name_1let)
+        elif residue_name_1let in translations:
             result.append(translations[residue_name_1let])
         else:
             if unknown:
                 result.append(unknown)
             else:
                 msg = f"""\
                      unknown residue {residue_name_1let} at residue {i+1}
@@ -226,37 +264,50 @@
                 msg = dedent(msg)
                 raise BadResidue(msg)
 
     return result
 
 
 def translate_3_to_1(
-    sequence: List[str], translations: Dict[str, str] = TRANSLATIONS_3_1
+    sequence: List[str], molecule_type=MoleculeTypes.PROTEIN
 ) -> List[str]:
     """
 
     Translate a 3 letter sequence to a 1 letter sequence
     Args:
         sequence (str): 3 letter sequence
-        translations (Dict[str, str]): a list of translations for single amino acid codes to 3 letter residue names
+        molecule_type (MoleculeTypes): type of molecule to translate residue types
 
     Returns List[str]:
         a list of 1 residue codes
 
     :param sequence:
     :return:
     """
+
+    translations = TRANSLATIONS_3_1[molecule_type]
+
     result = []
-    for i, resn in enumerate(sequence, start=1):
-        resn = resn.upper()
-        if resn in translations:
-            result.append(translations[resn])
+    for i, residue_name in enumerate(sequence, start=1):
+        residue_name = residue_name.upper()
+        if translations is None:
+            if len(residue_name) == 1:
+                result.append(residue_name)
+            else:
+                msg = f"""
+                    it isn't possible to translate the residue name {residue_name} to a 1 letter code
+                    the molecule type {molecule_type} doesn't have one letter codes and the residue name: {residue_name}
+                    is longer than one letter and so can't be passed through
+                """
+                exit_error(msg)
+        if residue_name in translations:
+            result.append(translations[residue_name])
         else:
             msg = f"""
-            unknown residue {resn}
+            unknown residue {residue_name}
             in sequence {chunks(' '.join(sequence), 10)}
             at residue number {i}
             """
             exit_error(msg)
 
     return result
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/structures.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from enum import auto
 from typing import Dict, List, Optional, Union
 
-from strenum import StrEnum
+from strenum import LowercaseStrEnum, StrEnum
 
 
 class Linking(StrEnum):
     START = (auto(),)
     MIDDLE = auto()
     END = auto()
 
@@ -157,23 +157,31 @@
     atom_1: AtomLabel
     atom_2: AtomLabel
     value: float
     value_uncertainty: float
     weight: Optional[float] = None
 
 
+class PeakFitMethod(LowercaseStrEnum):
+    GAUSSIAN = auto()
+    LORENTZIAN = auto()
+    SPLINE = auto()
+
+
 @dataclass(frozen=True, order=True)
 class NewPeak:
 
     shifts: List[ShiftData]
 
     id: Optional[int] = None
     height: Optional[float] = None
     height_uncertainty: Optional[float] = None
     volume: Optional[float] = None
     volume_uncertainty: Optional[float] = None
+    peak_fit_method: Optional[Union[str, PeakFitMethod]] = None
+    comment: str = ""
 
 
 @dataclass
 class DimensionInfo:
     axis_code: str  # this is the isotope code for us...
     axis_unit: Optional[str] = "ppm"
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/test_lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -149,29 +149,71 @@
 
             print(f"exp|{i}|  |{expected_line_stripped}|")
             print(f"rep|{i}|  |{reported_line_stripped}|")
 
         assert reported_line_stripped == expected_line_stripped
 
 
-def isolate_frame(target: str, name: str) -> Optional[str]:
+def isolate_frame(target: str, frame_name: str) -> Optional[str]:
     """
     Extract one frame from a NEF file by name as a string
     Args:
         target (Entry): target NEF entry
-        name (str): name of the save frame
+        frame_name (str): name of the save frame
 
     Returns:
         Optional[str]: the entry or a None if not found
     """
 
     entry = Entry.from_string(target)
-    entry = str(entry.get_saveframe_by_name(name))
+    try:
+        frame = entry.get_saveframe_by_name(frame_name)
+    except KeyError as e:
+        msg = f"""
+             the save frame {frame_name} wasn't found in the entry {entry.entry_id} the
+             available_frame names are {','.join([frame.name for frame in entry.frame_list])}'
+         """
+        raise KeyError(msg) from e
 
-    return entry
+    return str(frame)
+
+
+def isolate_loop(target: str, frame_name: str, loop_category: str) -> Optional[str]:
+    """
+    Extract one frame from a NEF file by name as a string
+    Args:
+        target (Entry): target NEF entry
+        frame_name (str): name of the save frame
+        loop_category (str): the name of the loop
+
+    Returns:
+        Optional[str]: the frame as a string or None if it is not found
+    """
+
+    entry = Entry.from_string(target)
+
+    try:
+        frame = entry.get_saveframe_by_name(frame_name)
+    except KeyError as e:
+        msg = f"""
+            the save frame {frame_name} wasn't found in the entry {entry.entry_id} the
+            available_frame names are {','.join([frame.name for frame in entry.frame_list])}'
+        """
+        raise KeyError(msg) from e
+
+    try:
+        loop = str(frame.get_loop(loop_category))
+    except KeyError as e:
+        msg = f"""
+            the loop  {loop_category} wasn't found in the frame {frame.name} in entry {entry.entry_id} the
+            available_loop categories are {','.join([loop.category for loop in frame.loops])}'
+        """
+        raise KeyError(msg) from e
+
+    return str(loop)
 
 
 def path_in_parent_directory(root: str, target: str) -> str:
     """
     given a root and a relative path find the relative file path
 
     Args:
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.36/src/nef_pipelines/lib/util.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/main.py` & `nef_pipelines-0.1.36/src/nef_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,19 +437,19 @@
     assert values == [2, "GLN", "N", 2, "GLN", "HN", -15.524, 1.000, 1.000]
 
     # assert False
 
 
 def test_sequence():
 
-    SEQUENCE = f"DATA {dedent(ABC_SEQUENCE_1LET)}"
+    SEQUENCE = f"DATA SEQUENCE {dedent(ABC_SEQUENCE_1LET)}"
 
     gdb_stream = io.StringIO(SEQUENCE)
 
     records = read_db_file_records(gdb_stream)
     sequence = gdb_to_3let_sequence(records)
 
-    sequence == ABC_SEQUENCE_3LET
+    assert sorted(sequence) == sorted(list(ABC_SEQUENCE_3LET))
 
 
 if __name__ == "__main__":
     pytest.main([__file__, "-vv"])
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,23 +226,23 @@
 
     EXPECTED = list("ABC")
 
     assert EXPECTED == result
 
 
 def test_chain_code_iter_with_user():
-    result = [chain_code for chain_code in islice(chain_code_iter("D.E"), 3)]
+    result = [chain_code for chain_code in islice(chain_code_iter("DE"), 3)]
 
     EXPECTED = list("DEA")
 
     assert EXPECTED == result
 
 
 def test_chain_code_iter_with_exclude():
-    result = [chain_code for chain_code in islice(chain_code_iter(exclude="B.C"), 3)]
+    result = [chain_code for chain_code in islice(chain_code_iter(exclude="BC"), 3)]
 
     EXPECTED = list("ADE")
 
     assert EXPECTED == result
 
 
 def test_sequence_from_frame():
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/clone.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def clone(
     target: str = Argument("A", help="chain to clone"),
     count: int = Argument(1, help="how many copys to make"),
     chain_codes: List[str] = Option(
         None,
         "-c",
         "--chains",
-        help="new chain codes to add otherwise defaults to next available ascii uper case letter,"
+        help="new chain codes to add otherwise defaults to next available ascii upper case letter,"
         " can be called mutiple times or be a comma separated list",
     ),
 ):
     """- duplicate chains one or more times"""
 
     if not count > 0:
         exit_error(f"clone count must be > 0 i got: {count}")
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         STDIN,
         "--in",
         "-i",
         metavar="|INPUT|",
         help="input to read NEF data from [stdin = -]",
     ),
 ):
-    """-  make a set of peaks for an hsqc or triple resonance spectrum from a list of shifts"""
+    """-  make a set of peaks for an hsqc or triple resonance spectrum from a list of shiftsdbxcli put rh"""
 
     shift_frames = parse_comma_separated_options(shift_frame_selectors)
 
     spectra = set(parse_comma_separated_options(spectra))
 
     spectra = _update_spectra_with_groups(spectra)
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.36/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 # todo add comment to other sequences etc
 @import_app.command()
 def sequence(
     chain_codes: List[str] = typer.Option(
         [],
         "--chains",
-        help="chain codes to use for the exported chains, can be a a comma sepatared list or can be called "
+        help="chain codes to use for the imported chains, can be a a comma separated list or can be called "
         "multiple times",
         metavar="<CHAIN-CODES>",
     ),
     starts: List[str] = typer.Option(
         [],
         "--starts",
         help="first residue number of sequences can be a comma separated list or ",
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     add_frames_to_entry,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.sequence_lib import (
-    TRANSLATIONS_3_1,
+    TRANSLATIONS_3_1_PROTEIN,
     BadResidue,
     chain_code_iter,
     get_residue_name_from_lookup,
     translate_1_to_3,
 )
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import (
@@ -26,14 +26,15 @@
 )
 from nef_pipelines.lib.util import (
     STDIN,
     cached_file_stream,
     exit_error,
     is_float,
     is_int,
+    parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.mars import import_app
 
 DEFAULT_PSEUDO_RESIDUE_PREFIX = "PR_"
 
 PSEUDO_RESIDUE = "PSEUDO_RESIDUE"
 
@@ -67,18 +68,18 @@
     currently if multiple residue codes are detected they are all ignored (with a warning)
 """
 
 
 # noinspection PyUnusedLocal
 @import_app.command(no_args_is_help=True)
 def shifts(
-    chain_code: str = typer.Option(
+    chain_codes: str = typer.Option(
         "-",
         "--chain",
-        help="chain codes [default -]",
+        help="chain codes [default -] can be a comma separated list or can be called mutiple times",
         metavar="<CHAIN-CODE>",
     ),
     entry_name: str = typer.Option(
         "mars", "-e", "--entry-name", help="a name for the entry"
     ),
     frame_name: str = typer.Option(
         "mars", "-f", "--frame-name", help="a name for the frame"
@@ -105,15 +106,17 @@
         ..., help="input files of type mars shifts.tab", metavar="<MARS-shifts>.tab"
     ),
 ):
     """convert MARS shift file <mars-shifts>.txt to NEF"""
 
     entry = read_or_create_entry_exit_error_on_bad_file(input, entry_name)
 
-    pipe(entry, chain_code, frame_name, file_names, prefix_to_strip, parse_residues)
+    chain_codes = parse_comma_separated_options(chain_codes)
+
+    pipe(entry, chain_codes, frame_name, file_names, prefix_to_strip, parse_residues)
 
 
 def pipe(
     entry,
     chain_codes,
     frame_name,
     file_names,
@@ -222,15 +225,15 @@
     return heading_indices
 
 
 def _get_residues_from_string(string):
 
     result = []
     string = string.upper()
-    for residue_name in TRANSLATIONS_3_1:
+    for residue_name in TRANSLATIONS_3_1_PROTEIN:
         if residue_name in string:
             result.append(residue_name)
     return result
 
 
 def _parse_line(
     line_info, heading_indices, chain_code, prefix_to_strip, parse_residues
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     sequence_to_nef_frame,
 )
 from nef_pipelines.lib.structures import SequenceResidue
 from nef_pipelines.lib.typer_utils import get_args
 from nef_pipelines.lib.util import (
     cached_file_stream,
     exit_error,
+    parse_comma_separated_options,
     process_stream_and_add_frames,
 )
 from nef_pipelines.transcoders.nmrpipe import import_app
 from nef_pipelines.transcoders.nmrpipe.nmrpipe_lib import (
     gdb_to_3let_sequence,
     read_db_file_records,
 )
@@ -30,15 +31,15 @@
 
 # noinspection PyUnusedLocal
 @import_app.command()
 def sequence(
     chain_codes: List[str] = typer.Option(
         None,
         "--chains",
-        help="chain codes as a list of names separated by dots",
+        help="chain codes can be called multiple times and / or  be a comma separated list",
         metavar="<CHAIN-CODES>",
     ),
     no_chain_start: bool = typer.Option(
         False,
         "--no-chain-start/",
         help="don't include a start of chain link type for the first residue",
     ),
@@ -69,14 +70,16 @@
         exit_error(f"reading sequence failed because {e}", e)
 
 
 def process_sequence(args: Namespace):
     nmrpipe_frames = []
 
     chain_codes = args.chain_codes
+
+    chain_codes = parse_comma_separated_options(chain_codes)
     if not chain_codes:
         chain_codes = ["A"]
     for file_name, chain_code in zip(args.file_names, chain_code_iter(chain_codes)):
         # cached_file_stream
         with cached_file_stream(file_name) as lines:
 
             nmrpipe_sequence = read_sequence(
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     add_frames_to_entry,
     read_file_or_exit,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.sequence_lib import chain_code_iter, translate_1_to_3
 from nef_pipelines.lib.shift_lib import shifts_to_nef_frame
 from nef_pipelines.lib.structures import ShiftList
-from nef_pipelines.lib.util import STDIN
+from nef_pipelines.lib.util import STDIN, parse_comma_separated_options
 from nef_pipelines.transcoders.nmrpipe import import_app
 from nef_pipelines.transcoders.nmrpipe.nmrpipe_lib import (
     read_db_file_records,
     read_shift_file,
 )
 
 app = typer.Typer()
@@ -24,15 +24,15 @@
 
 # noinspection PyUnusedLocal
 @import_app.command()
 def shifts(
     chain_codes: List[str] = typer.Option(
         None,
         "--chains",
-        help="chain codes as a list of names spearated by dots",
+        help="chain codes, can be called multiple times and or be a comma separated list [no spaces!]",
         metavar="<CHAIN-CODES>",
     ),
     entry_name: str = typer.Option("nmrpipe", help="a name for the entry"),
     frame_name: str = typer.Option("nmrpipe", help="a name for the frame"),
     input: Path = typer.Option(
         STDIN,
         "-i",
@@ -44,14 +44,16 @@
         ..., help="input files of type nmrpipe.tab", metavar="<TAB-FILE>"
     ),
 ):
     """convert nmrpipe shift file <nmrpipe>.tab files to NEF"""
 
     entry = read_or_create_entry_exit_error_on_bad_file(input, entry_name)
 
+    chain_codes = parse_comma_separated_options(chain_codes)
+
     if not chain_codes:
         chain_codes = ["A"]
 
     pipe(entry, chain_codes, file_names, frame_name)
 
 
 def pipe(entry, chain_codes, file_names, frame_name):
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import functools
 import operator
 import re
 from collections import Counter
 from dataclasses import dataclass, field
 from enum import IntEnum
 from textwrap import dedent
-from typing import Callable, Dict, List, Optional, TextIO, Tuple, Union
+from typing import Callable, List, Optional, TextIO, Tuple, Union
 
 from tabulate import tabulate
 
 from nef_pipelines.lib.sequence_lib import (
-    TRANSLATIONS_1_3,
+    MoleculeTypes,
     make_chunked_sequence_1let,
     translate_1_to_3,
 )
 from nef_pipelines.lib.structures import (
     AtomLabel,
     LineInfo,
     PeakAxis,
@@ -351,36 +351,36 @@
     result = [record for record in gdb.records if record.type == record_type]
     if predicate:
         result = [record for record in result if predicate(record)]
     return result
 
 
 def gdb_to_3let_sequence(
-    gdb: DbFile, translations: Dict[str, str] = TRANSLATIONS_1_3
+    gdb: DbFile, molecule_type: MoleculeTypes = MoleculeTypes.PROTEIN
 ) -> List[SequenceResidue]:
     """
     read sequence records from a gdb file and convert them to a list of sequence residues
     it is assumed that residues start from 1 and are in chain A
     Args:
         gdb (DbFile): the source db/tab file records
-        translations (Dict[str, str]): a translation table for 1 letter codes to 3 letter codes
+        molecule_type (MoleculeTypes): the type of the molecule to translate
 
     Returns List[SequenceResidue]:
         a list of sequence residues
     """
     sequence_records = select_records(
         gdb, "DATA", predicate=lambda rec: rec.values[0] == "SEQUENCE"
     )
 
     sequence = [record.values[1:] for record in sequence_records]
 
     flattened_sequence = functools.reduce(operator.iconcat, sequence, [])
     sequence_string = "".join(flattened_sequence)
 
-    return translate_1_to_3(sequence_string, translations)
+    return translate_1_to_3(sequence_string, molecule_type=molecule_type)
 
 
 def _assignments_to_atom_labels(assignments, dimensions, chain_code="A"):
     result = []
 
     for assignment in assignments:
         chain_code = chain_code
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 from pathlib import Path
 from typing import List
 
 import typer
 
 from nef_pipelines.lib.sequence_lib import chain_code_iter, sequence_to_nef_frame
 from nef_pipelines.lib.typer_utils import get_args
-from nef_pipelines.lib.util import exit_error, process_stream_and_add_frames
+from nef_pipelines.lib.util import (
+    exit_error,
+    parse_comma_separated_options,
+    process_stream_and_add_frames,
+)
 from nef_pipelines.transcoders.nmrview import import_app
 from nef_pipelines.transcoders.nmrview.nmrview_lib import read_sequence
 
 app = typer.Typer()
 
 
 # noinspection PyUnusedLocal
 @import_app.command(no_args_is_help=True)
 def sequence(
     chain_codes: str = typer.Option(
         "A",
         "--chains",
-        help="chain codes as a list of names separated by dots",
+        help="chain codes, can be called multiple times and or be a comma separated list [no spaces!]",
         metavar="<CHAIN-CODES>",
     ),
     no_chain_start: bool = typer.Option(
         False,
         "--no-chain-start/",
         help="don't include a start of chain link type for the first residue",
     ),
@@ -50,17 +54,16 @@
     except Exception as e:
         exit_error(f"reading sequence failed because {e}")
 
 
 def process_sequence(args: Namespace):
     nmrview_frames = []
 
-    for file_name, chain_code in zip(
-        args.file_names, chain_code_iter(args.chain_codes)
-    ):
+    chain_codes = parse_comma_separated_options(args.chain_codes)
+    for file_name, chain_code in zip(args.file_names, chain_code_iter(chain_codes)):
         with open(file_name, "r") as lines:
             nmrview_sequence = read_sequence(lines, chain_code=chain_code)
 
             frame = sequence_to_nef_frame(nmrview_sequence, args.entry_name)
 
             nmrview_frames.append(frame)
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from nef_pipelines.lib.util import (
     STDIN,
     cached_file_stream,
     exit_error,
     fixup_metadata,
     get_pipe_file_text_or_exit,
     get_version,
+    parse_comma_separated_options,
     script_name,
 )
 from nef_pipelines.transcoders.nmrview import import_app
 from nef_pipelines.transcoders.nmrview.nmrview_lib import parse_shifts, read_sequence
 
 app = typer.Typer()
 
@@ -28,15 +29,15 @@
 
 # noinspection PyUnusedLocal
 @import_app.command(no_args_is_help=True)
 def shifts(
     chain_codes: str = typer.Option(
         "A",
         "--chains",
-        help="chain codes as a list of names separated by dots",
+        help="chain codes, can be called multiple times and or be a comma separated list [no spaces!]",
         metavar="<CHAIN-CODES>",
     ),
     frame_name: str = typer.Option(
         "nmrview", "-f", "--frame-name", help="a name for the frame"
     ),
     input: Path = typer.Option(
         STDIN,
@@ -50,14 +51,16 @@
     ),
 ):
     """convert nmrview shift file <nmrview-shifts>.out to NEF"""
 
     try:
         entry = read_entry_from_file_or_stdin_or_exit_error(input)
 
+        chain_codes = parse_comma_separated_options(chain_codes)
+
         sequence = sequence_from_entry_or_exit(entry)
 
         pipe(entry, chain_codes, sequence, frame_name, file_names)
 
     except Exception as e:
         exit_error(f"reading sequence failed because {e}", e)
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pynmrstar import Entry, Saveframe
 from tabulate import tabulate
 
 from nef_pipelines.lib.nef_lib import (
     read_entry_from_stdin_or_exit,
     select_frames_by_name,
 )
-from nef_pipelines.lib.sequence_lib import TRANSLATIONS_3_1
+from nef_pipelines.lib.sequence_lib import TRANSLATIONS_3_1_PROTEIN
 from nef_pipelines.lib.shift_lib import nef_frames_to_shifts
 from nef_pipelines.lib.structures import ShiftData
 from nef_pipelines.lib.util import STDOUT, exit_error, flatten, is_int
 from nef_pipelines.transcoders.shifty import export_app
 
 OUTPUT_FILE_SHORTCUTS = """\
     for stdout use -, ! will use the name of the nef entry in the
@@ -110,28 +110,28 @@
         sequence_code = shift.atom.residue.sequence_code
         atom_name = shift.atom.atom_name
         residue_name = shift.atom.residue.residue_name
 
         if _is_pseudo_residue(chain_code, sequence_code):
             continue
 
-        if residue_name.upper() not in TRANSLATIONS_3_1:
+        if residue_name.upper() not in TRANSLATIONS_3_1_PROTEIN:
             continue
 
         if atom_name not in SHIFTY_LOOKUP_ATOMS:
             continue
 
         if chain_code != selected_chain_code:
             continue
 
         if not is_int(sequence_code):
             continue
 
         sequence_code = int(sequence_code)
-        residue_name_1let = TRANSLATIONS_3_1[residue_name]
+        residue_name_1let = TRANSLATIONS_3_1_PROTEIN[residue_name]
         value = shift.value
 
         key = sequence_code, residue_name_1let
         lines.setdefault(key, {})[atom_name] = value
 
     table = [[*SHIFTY_EXTRA_HEADINGS, *SHIFTY_ATOMS]]
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 
     app.add_typer(import_app, name="import", help="-  import sparky [shifts]")
     app.add_typer(export_app, name="export", help="-  export sparky [peaks]")
 
     # import of specific importers must be after app creation to avoid circular imports
     import nef_pipelines.transcoders.sparky.exporters.peaks  # noqa: F401
     import nef_pipelines.transcoders.sparky.importers.peaks  # noqa: F401
+    import nef_pipelines.transcoders.sparky.importers.sequence  # noqa: F401
     import nef_pipelines.transcoders.sparky.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     read_entry_from_file_or_stdin_or_exit_error,
     select_frames_by_name,
 )
 from nef_pipelines.lib.peak_lib import frame_to_peaks
-from nef_pipelines.lib.sequence_lib import TRANSLATIONS_3_1
+from nef_pipelines.lib.sequence_lib import TRANSLATIONS_3_1_PROTEIN
 from nef_pipelines.lib.structures import NewPeak
 from nef_pipelines.lib.util import (
     STDIN,
     STDOUT,
     exit_error,
     is_float,
     parse_comma_separated_options,
@@ -64,14 +64,15 @@
 # peak note. Peaks for 3-D or 4-D spectra can be read.
 #
 # what does sparky do with multiple chains?
 #
 # what does ga mean in the sparky output after a volume
 #
 # why does sparky sometime have ga after a volume I presume it's a gausiann peak fit?
+# comment gst 19/04/2023 is ga for a gaussian peak fit?
 #
 #  Assignment       w1      w2      Volume     lw1 (hz)   lw2 (hz)
 #
 #    G16H3'-H8    4.905   8.010   7.15e+06 ga    28.6       20.0
 #    G16H4'-H8    4.439   8.013   5.42e+06 ga    35.3       16.9
 #  T17H6-G16H8    7.205   8.004   1.68e+06
 #  T17H7-G16H8    1.459   8.008   2.09e+07 ga    27.5       24.1
@@ -471,16 +472,16 @@
 
                         if sequence_code.startswith("@"):
                             sequence_code = f"PR_{sequence_code[1:]}"
                         # if chain_code.startswith('PC_'):
                         #     sequence_code = f'{chain_code}:{sequence_code}'
                         #     chain_sequence_separator = ''
 
-                        if residue_name in TRANSLATIONS_3_1:
-                            residue_name = TRANSLATIONS_3_1[residue_name]
+                        if residue_name in TRANSLATIONS_3_1_PROTEIN:
+                            residue_name = TRANSLATIONS_3_1_PROTEIN[residue_name]
 
                         if not residue_name:
                             residue_name = ""
 
                         group = f"{chain_code}{current_chain_sequence_separator}{residue_name}{sequence_code}"
 
                         assignment = f"{group}{atom_name}"
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,141 +1,217 @@
 import string
 import sys
+from itertools import zip_longest
 from pathlib import Path
 from textwrap import dedent
 from typing import Dict, List
 
 import typer
+from fyeah import f
 
 from nef_pipelines.lib.isotope_lib import ATOM_TO_ISOTOPE
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     add_frames_to_entry,
     read_or_create_entry_exit_error_on_bad_file,
 )
 from nef_pipelines.lib.peak_lib import peaks_to_frame
-from nef_pipelines.lib.sequence_lib import TRANSLATIONS_1_3
+from nef_pipelines.lib.sequence_lib import (
+    TRANSLATIONS_1_3,
+    MoleculeTypes,
+    chain_code_iter,
+    residues_to_residue_name_lookup,
+    sequence_from_entry,
+)
 from nef_pipelines.lib.structures import (
     AtomLabel,
     LineInfo,
     NewPeak,
+    PeakFitMethod,
     Residue,
+    SequenceResidue,
     ShiftData,
 )
 from nef_pipelines.lib.util import (
     STDIN,
     exit_error,
     is_float,
     parse_comma_separated_options,
 )
 from nef_pipelines.transcoders.sparky import import_app
+from nef_pipelines.transcoders.sparky.importers.shifts import (
+    _exit_if_chain_codes_and_file_name_dont_match,
+)
 
 
 # TODO: this needs to be moved to a library
 class SparkyPeakListException(Exception):
     pass
 
 
 class IncompatibleDimensionTypesException(SparkyPeakListException):
     pass
 
 
 app = typer.Typer()
 
 DEFAULT_NUCLEI_HELP = (
-    "nuclei to use for each dimension if not defined they are guessed from the assigments"
+    "nuclei to use for each dimension, if not defined they are guessed from the assignments"
     "or an error is reported"
 )
 
 
 # noinspection PyUnusedLocal
 @import_app.command(no_args_is_help=True)
 def peaks(
-    # chain_codes: List[str] = typer.Option(
-    #     None,
-    #     "--chains",
-    #     help="chain codes as a list of names separated by commas, repeated calls will add further chains [default A]",
-    #     metavar="<CHAIN-CODES>",
-    # ),
+    chain_codes: List[str] = typer.Option(
+        None,
+        "--chains",
+        help="chain codes as a list of names separated by commas, repeated calls will add further chains [default A]",
+        metavar="<CHAIN-CODES>",
+    ),
     frame_name: str = typer.Option(
-        "sparky", "-f", "--frame-name", help="a name for the frame"
+        "sparky_{file_name}",
+        "-f",
+        "--frame-name",
+        help="a templated name for the frame {file_name} will be replaced by input filename",
     ),
     input: Path = typer.Option(
         STDIN,
         "-i",
-        "--input",
+        "--in",
         metavar="|PIPE|",
         help="input to read NEF data from [- is stdin]",
     ),
     file_names: List[Path] = typer.Argument(
         ..., help="input files of type peaks.txt", metavar="<SPARKY-peaks>.txt"
     ),
     nuclei: List[str] = typer.Option([], help=DEFAULT_NUCLEI_HELP),
     default_chain_code: str = typer.Option(
         "A",
         "-c",
         "--chain-code",
         help="default chain code to use if none is provided in the file",
     ),
+    molecule_type: MoleculeTypes = typer.Option(
+        MoleculeTypes.PROTEIN, help="the type of molecule"
+    ),
+    no_validate: bool = typer.Option(
+        False,
+        help="if set don't validate the peaks agains the inpuy sequence if provided",
+    ),
     spectrometer_frequency: float = typer.Option(
         600.123456789, help="spectrometer frequency in MHz"
     ),
 ):
-    """convert sparky peaks file <SPARKY-peaks>.txt to NEF [alpha]"""
+    """convert sparky peaks file <SPARKY-PEAKS>.txt to NEF [alpha]"""
 
-    print(
-        "*** WARNING *** this command [sparky peaks] is only lightly tested use at your own risk!",
-        file=sys.stderr,
-    )
+    chain_codes = parse_comma_separated_options(chain_codes)
 
-    # chain_codes = parse_comma_separated_options(chain_codes)
-    #
-    # if not chain_codes:
-    #     chain_codes = ["A"]
+    if not chain_codes:
+        chain_codes = ["A"]
 
-    # _exit_if_chain_codes_and_file_name_dont_match(chain_codes, file_names)
+    # make this a library function
+    _exit_if_chain_codes_and_file_name_dont_match(chain_codes, file_names)
 
     entry = read_or_create_entry_exit_error_on_bad_file(input)
 
-    # sequence = sequence_from_entry_or_exit(entry)
+    sequence = sequence_from_entry(entry) if not no_validate else None
 
     nuclei = parse_comma_separated_options(nuclei)
 
-    pipe(
+    entry = pipe(
         entry,
         frame_name,
         file_names,
+        chain_codes,
+        sequence,
         input_dimensions=nuclei,
         spectrometer_frequency=spectrometer_frequency,
+        molecule_type=molecule_type,
     )
 
+    print(entry)
+
+
+def pipe(
+    entry,
+    frame_name,
+    file_names,
+    chain_codes,
+    sequence,
+    input_dimensions,
+    spectrometer_frequency,
+    molecule_type=MoleculeTypes.PROTEIN,
+):
+
+    sparky_frames = []
+
+    for file_name, chain_code in zip(file_names, chain_code_iter(chain_codes)):
+
+        try:
+            with open(file_name, "r") as fp:
+                lines = fp.readlines()
+        except IOError as e:
+            msg = f"""
+                    while reading sparky peaks file {file_name} there was an error reading the file
+                    the error was: {e}
+                """
+            exit_error(msg, e)
+
+        sparky_peaks = _parse_peaks(
+            lines,
+            file_name=file_name,
+            molecule_type=molecule_type,
+            chain_code=chain_code,
+            sequence=sequence,
+        )
+
+        dimensions = _guess_dimensions_if_not_defined_or_throw(
+            sparky_peaks, input_dimensions
+        )
+
+        dimensions = [{"axis_code": dimension} for dimension in dimensions]
+
+        frame = peaks_to_frame(sparky_peaks, dimensions, spectrometer_frequency)
+
+        file_name = Path(file_name).stem  # used in f method...
+
+        frame.name = f(frame_name)
+
+        sparky_frames.append(frame)
+
+    return add_frames_to_entry(entry, sparky_frames)
+
 
 def parse_header_to_columns(header_line: str, file_name) -> Dict[str, int]:
     headings_to_columns = {}
     headings = header_line.split()
 
     if "Data" in headings:
         headings.remove("Data")
 
-    while ("hz") in headings:
-        headings.remove("hz")
+    while ("(hz)") in headings:
+        headings.remove("(hz)")
 
     for i, heading in enumerate(headings):
         if heading in "Assignment Height Volume".split():
             headings_to_columns[heading] = i
             continue
 
         if heading.startswith("w") or heading.startswith("lw"):
             headings_to_columns[heading] = i
             continue
 
+        # TODO add a warning function in the library
         msg = f"""
             WARNING: unexpected heading {heading} in the file {file_name}...
                      this heading will be ignored, please send the heading and first
-                     few lines of this file to the developers of NEF-Pipelines
+                     few lines of this file to the developers of NEF-Pipelines if you
+                     believe this is a valid sparky peaks file
         """
 
         print(msg, file=sys.stderr)
 
     assignment_column = headings_to_columns["Assignment"]
     if assignment_column != 0:
         msg = f"""
@@ -149,34 +225,36 @@
     return headings_to_columns
 
 
 def _exit_error_if_shift_not_float(shifts, line_info):
     for i, shift in enumerate(shifts, start=1):
         if not is_float(shift):
             msg = f"""
-                file {line_info.file_name} does not look like a spark file
-                for shift w{i} at line {line_info.line_no} the value {shift} couldn't be converted to a float
-                the full line was
+                file {line_info.file_name} does not look like a sparky file
+                for shift w{i} at line {line_info.line_no} with the value {shift} couldn't be converted to a float
+                the full line was:
                 {line_info.line}
             """
             exit_error(msg)
 
 
-def _parse_peaks(lines, file_name):
+def _parse_peaks(lines, file_name, molecule_type, chain_code, sequence):
 
     peaks = []
 
     in_data = False
 
     dimension_count = None
 
     for line_number, line in enumerate(lines, start=1):
 
-        line_info = LineInfo(file_name, line_number, line)
         line = line.strip()
+
+        line_info = LineInfo(file_name, line_number, line)
+
         if len(line) == 0:
             continue
 
         if line.startswith("#"):
             continue
 
         if line.strip()[: len("Assignment")] == "Assignment":
@@ -193,43 +271,105 @@
 
             continue
         else:
             if not in_data:
                 _exit_error_data_but_no_header(line_info)
 
             fields = line.split()
+
+            column_count = len(fields)
+            if column_count < (dimension_count + 1):
+                _exit_error_not_enough_columns_in_data_row(
+                    dimension_count, column_count, line_info
+                )
             values = {}
             for column, index in column_headers_to_indices.items():
                 if index < len(fields):
                     values[column] = fields[index]
                 else:
-                    _exit_error_not_enough_columns_in_data_row(
-                        column_headers_to_indices, column, line_info
-                    )
+                    values[column] = UNUSED
 
             assignmnents_column = column_headers_to_indices["Assignment"]
             raw_assignment = fields[assignmnents_column]
 
-            assignments = _process_assignments(raw_assignment)
+            assignments = _process_assignments(
+                raw_assignment, chain_code, sequence, molecule_type, line_info
+            )
 
             shifts = [
                 fields[column_headers_to_indices[f"w{index}"]]
                 for index in range(1, dimension_count + 1)
             ]
 
-            shifts = [float(shift) for shift in shifts if is_float(shift)]
+            converted_shifts = []
+            for shift in shifts:
+                shift = float(shift) if is_float(shift) else shift
+                converted_shifts.append(shift)
 
             _exit_error_if_shift_not_float(shifts, line_info)
 
+            shifts = converted_shifts
+
+            peak_fit_method = None
+            volume = None
+            if "Volume" in column_headers_to_indices:
+
+                volume_index = column_headers_to_indices["Volume"]
+
+                volume = float(fields[volume_index])
+
+                line_fit_index = volume_index + 1
+                if line_fit_index < len(fields):
+                    if fields[line_fit_index] == "ga":
+                        peak_fit_method = PeakFitMethod.GAUSSIAN
+                        fields.remove("ga")
+
+            height = (
+                float(fields[column_headers_to_indices["Height"]])
+                if "Height" in column_headers_to_indices
+                else None
+            )
+
+            comment_fields = []
+            line_widths = []
+            for dimension in range(1, dimension_count + 1):
+                line_width_column = f"lw{dimension}"
+                if line_width_column in column_headers_to_indices:
+                    line_width_column_index = column_headers_to_indices[
+                        line_width_column
+                    ]
+                    if line_width_column_index < len(fields):
+                        possible_line_width = fields[line_width_column_index]
+                        if is_float(possible_line_width):
+                            line_widths.append(float(possible_line_width))
+                        else:
+                            comment_fields.append(possible_line_width)
+                            line_widths.append(None)
+                    else:
+                        line_widths.append(None)
+
             shift_data = [
-                ShiftData(atom=atom, value=value)
-                for atom, value in zip(assignments, shifts)
+                ShiftData(atom=atom, value=value, line_width=line_width)
+                for atom, value, line_width in zip_longest(
+                    assignments, shifts, line_widths, fillvalue=None
+                )
             ]
+
+            max_column = max(column_headers_to_indices.values())
+            if len(fields) > max_column:
+                comment_fields = [*comment_fields, *fields[max_column + 1 :]]
+
+            comment = " ".join(comment_fields)
+
             peak = NewPeak(
                 shifts=shift_data,
+                peak_fit_method=peak_fit_method,
+                height=height,
+                volume=volume,
+                comment=comment,
             )
 
             peaks.append(peak)
 
     return peaks
 
 
@@ -241,22 +381,23 @@
                     the current line data is
                     {line_info.line}
                 """
     exit_error(msg)
 
 
 def _exit_error_not_enough_columns_in_data_row(
-    column_headers_to_indices, column, line_info
+    dimension_count, column_count, line_info
 ):
     msg = f"""
-                        In sparky peaks file {line_info.file_name} at line {line_info.line_number} for column {column}
-                        there were was not enough data [expected {len(column_headers_to_indices)} columns]
-                        the line was:
-                        {line_info.line}
-                    """
+            In sparky peaks file {line_info.file_name} at line {line_info.line_no}
+            there were was not enough data [expected {1+ dimension_count} columns
+            (Assignment + shifts * {dimension_count})]
+            the line was:
+            {line_info.line}
+        """
     exit_error(msg)
 
 
 def _exit_error_no_dimensions(dimension_count, line_info):
     if dimension_count < 1:
         msg = f"""
                     sparky peak file {line_info.file_name} doesn't appear to have enough columns [minimum 1]
@@ -284,109 +425,113 @@
         the line was:
         {line_info.line}
                 """
     exit_error(msg)
 
 
 # TODO this doesn't cope with abbreviated names
-def _process_assignments(assignments, chain_code="A"):
+def _process_assignments(
+    assignments, chain_code, sequence: List[SequenceResidue], molecule_type, line_info
+):
+
+    residue_name_lookup = residues_to_residue_name_lookup(sequence)
+
+    residue_name_translations = TRANSLATIONS_1_3[molecule_type]
 
     fields = assignments.split("-")
 
     assignments = []
+    last_sequence_code = None
+    last_residue_name = None
     for field in fields:
 
         if len(field) == 1 and field == "?":
             assignment = AtomLabel(
                 atom_name=UNUSED, residue=Residue("@-", UNUSED, UNUSED)
             )
             assignments.append(assignment)
         else:
 
             without_first_letters = field.lstrip(string.ascii_letters)
+
             first_letters = field[: -len(without_first_letters)]
+
             if len(first_letters) == 0 and without_first_letters[0] == "?":
                 first_letters = "?"
                 without_first_letters = without_first_letters[1:]
 
             without_numbers = without_first_letters.lstrip(string.digits)
+            without_numbers = without_numbers.lstrip("\"'")
+
             numbers = without_first_letters[: -len(without_numbers)]
 
-            if len(numbers) == 0 and without_numbers[0] == "?":
+            if (
+                without_numbers != ""
+                and len(numbers) == 0
+                and without_numbers[0] == "?"
+            ):
                 numbers = "?"
                 without_numbers = without_numbers[1:]
 
-            if len(first_letters) == 0 or first_letters == "?":
+            if without_numbers == "":
+                residue_name = last_residue_name
+            elif len(first_letters) == 0 or first_letters == "?":
                 residue_name = UNUSED
             else:
                 residue_name = first_letters
 
-            if len(numbers) == 0 or numbers == "?":
+            if without_numbers == "":
+                sequence_code = last_sequence_code
+            elif len(numbers) == 0 or numbers == "?":
                 sequence_code = UNUSED
             else:
                 sequence_code = numbers
 
-            if len(without_numbers) == 0 or without_numbers == "?":
+            if without_numbers == "":
+                atom_name = f"{first_letters}{without_first_letters}"
+            elif len(without_numbers) == 0 or without_numbers == "?":
                 atom_name = UNUSED
             else:
                 atom_name = without_numbers
 
-            if residue_name in TRANSLATIONS_1_3:
-                residue_name = TRANSLATIONS_1_3[residue_name]
-
-            assignment = AtomLabel(
-                atom_name=atom_name,
-                residue=Residue(chain_code, sequence_code, residue_name),
-            )
-            assignments.append(assignment)
-
-    return assignments
-
-
-def pipe(
-    entry, frame_name, file_names, input_dimensions, spectrometer_frequency
-):  # , sequence, chain_codes,
+            if residue_name_translations is not None:
+                if residue_name in residue_name_translations:
+                    translated_residue_name = residue_name_translations[residue_name]
+                else:
+                    msg = f"""
+                        The residue name {residue_name} is not defined for the molecule type {molecule_type} for the
+                        assignment {assignment} at line {line_info.line_no} in file {line_info.file_name} the line was
+                        {line_info.line}
+                    """
+                    exit_error(msg)
 
-    sparky_frames = []
+            if sequence and ((chain_code, sequence_code) not in residue_name_lookup):
+                msg = f"""
+                    the chain code {chain_code} and sequence_code {sequence} from
+                    line {line_info.line_no} in file {line_info.file_name} were not found
+                    in the input sequence, the full line was
 
-    for (
-        file_name
-    ) in file_names:  # , chain_code in zip(file_names, chain_code_iter(chain_codes)):
-
-        # with cached_file_stream(file_name) as lines:
-        #
-        #     chain_seqid_to_type = sequence_to_residue_type_lookup(sequence)
+                    {line_info.line}
 
-        try:
-            with open(file_name, "r") as fp:
-                lines = fp.readlines()
-        except IOError as e:
-            msg = f"""
-                    while reading sparky peaks file {file_name} there was an error reading the file
-                    the error was: {e}
+                    if you wish to input the peaks without validating against the input sequence use the
+                    --no-validate option of sparky import peaks
                 """
-            exit_error(msg, e)
-
-        sparky_peaks = _parse_peaks(
-            lines, file_name=file_name  # chain_seqid_to_type, chain_code=chain_code,
-        )
+                exit_error(msg)
 
-        dimensions = _guess_dimensions_if_not_defined_or_throw(
-            sparky_peaks, input_dimensions
-        )
-
-        dimensions = [{"axis_code": dimension} for dimension in dimensions]
+            assignment = AtomLabel(
+                atom_name=atom_name,
+                residue=Residue(chain_code, sequence_code, translated_residue_name),
+            )
 
-        frame = peaks_to_frame(sparky_peaks, dimensions, spectrometer_frequency)
+            assignments.append(assignment)
 
-        sparky_frames.append(frame)
-    #
-    entry = add_frames_to_entry(entry, sparky_frames)
+        last_sequence_code = sequence_code
+        last_residue_name = residue_name
 
-    print(entry)
+    return assignments
 
 
 # TODO: this needs to be moved to a library
 def _guess_dimensions_if_not_defined_or_throw(
     peaks: List[NewPeak], input_dimensions: List[str]
 ) -> List[str]:
     results_by_dimension = {
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.36/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nef-pipelines
-Version: 0.1.35
+Name: nef_pipelines
+Version: 0.1.36
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.35/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.36/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -134,18 +134,27 @@
 src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
 src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
 src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
 src/nef_pipelines/tests/shifts/__init__.py
 src/nef_pipelines/tests/shifts/test_make_peaks.py
 src/nef_pipelines/tests/shifty/__init__.py
 src/nef_pipelines/tests/shifty/test_export_shifts.py
+src/nef_pipelines/tests/sparky/__init__.py
 src/nef_pipelines/tests/sparky/test_export_peaks.py
+src/nef_pipelines/tests/sparky/test_import_peaks.py
+src/nef_pipelines/tests/sparky/test_import_sequence.py
 src/nef_pipelines/tests/sparky/test_import_shifts.py
 src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
 src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
 src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
 src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
 src/nef_pipelines/tests/test_data/3a_ab.neff
@@ -245,14 +254,15 @@
 src/nef_pipelines/transcoders/shifty/exporters/__init__.py
 src/nef_pipelines/transcoders/shifty/exporters/shifts.py
 src/nef_pipelines/transcoders/sparky/__init__.py
 src/nef_pipelines/transcoders/sparky/exporters/__init__.py
 src/nef_pipelines/transcoders/sparky/exporters/peaks.py
 src/nef_pipelines/transcoders/sparky/importers/__init__.py
 src/nef_pipelines/transcoders/sparky/importers/peaks.py
+src/nef_pipelines/transcoders/sparky/importers/sequence.py
 src/nef_pipelines/transcoders/sparky/importers/shifts.py
 src/nef_pipelines/transcoders/xcamshift/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
 src/nef_pipelines/transcoders/xplor/__init__.py
 src/nef_pipelines/transcoders/xplor/psf_lib.py
 src/nef_pipelines/transcoders/xplor/xplor_lib.py
```

### Comparing `nef_pipelines-0.1.35/tox.ini` & `nef_pipelines-0.1.36/tox.ini`

 * *Files identical despite different names*

