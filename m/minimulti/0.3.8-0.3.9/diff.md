# Comparing `tmp/minimulti-0.3.8.tar.gz` & `tmp/minimulti-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minimulti-0.3.8.tar", last modified: Thu Nov  4 12:19:29 2021, max compression
+gzip compressed data, was "minimulti-0.3.9.tar", last modified: Sat Dec 11 20:14:30 2021, max compression
```

## Comparing `minimulti-0.3.8.tar` & `minimulti-0.3.9.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      413 2021-11-04 12:19:29.927169 minimulti-0.3.8/PKG-INFO
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1087 2021-02-14 09:32:33.000000 minimulti-0.3.8/README.md
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.915169 minimulti-0.3.8/minimulti/
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.915169 minimulti-0.3.8/minimulti/LWF/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-11 14:41:03.000000 minimulti-0.3.8/minimulti/LWF/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       96 2021-07-05 09:37:20.000000 minimulti-0.3.8/minimulti/LWF/lwf.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     6892 2021-07-09 20:01:21.000000 minimulti-0.3.8/minimulti/LWF/lwf_to_atoms_batch.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/__init__.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.915169 minimulti-0.3.8/minimulti/abstract/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       50 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/abstract_coupling.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      878 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/abstract_hamiltonian.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      844 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/abstract_model.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      140 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/abstract_mover.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      876 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/abstract/abstract_potential.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7742 2021-02-24 09:19:55.000000 minimulti-0.3.8/minimulti/abstract/datatype.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      741 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/constants.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.919170 minimulti-0.3.8/minimulti/electron/
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7067 2020-05-05 13:21:25.000000 minimulti-0.3.8/minimulti/electron/COHP.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    17506 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/HF.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    52456 2021-04-19 20:43:12.000000 minimulti-0.3.8/minimulti/electron/Hamiltonian.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    16167 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/Hubbard.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    22312 2021-01-28 10:01:07.000000 minimulti-0.3.8/minimulti/electron/Hubbard_4ind.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    19444 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/Hubbard_old.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    11972 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/Hubbard_old2.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.919170 minimulti-0.3.8/minimulti/electron/TB/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/TB/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    11917 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/TB/myTB.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10537 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/TB/mypythtb.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3137 2021-04-01 13:12:22.000000 minimulti-0.3.8/minimulti/electron/UJfitter.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    20830 2021-04-01 13:12:48.000000 minimulti-0.3.8/minimulti/electron/U_matrix.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     8175 2021-04-18 09:38:40.000000 minimulti-0.3.8/minimulti/electron/basis2.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.919170 minimulti-0.3.8/minimulti/electron/box/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/box/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1028 2021-04-13 20:39:14.000000 minimulti-0.3.8/minimulti/electron/box/dummymixer.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2479 2021-04-19 20:35:49.000000 minimulti-0.3.8/minimulti/electron/box/pulay.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/electron/builder/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       26 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/builder/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2667 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/builder/perovskite.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2811 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/constraint.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     8495 2021-04-19 19:31:38.000000 minimulti-0.3.8/minimulti/electron/density.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    12935 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/epc.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5001 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/from_banddownfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4989 2021-04-15 18:52:00.000000 minimulti-0.3.8/minimulti/electron/hopping.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    10019 2021-04-19 20:49:57.000000 minimulti-0.3.8/minimulti/electron/ijR.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      420 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/ioput.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10629 2021-04-01 13:19:01.000000 minimulti-0.3.8/minimulti/electron/lwf.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3318 2021-04-19 19:41:50.000000 minimulti-0.3.8/minimulti/electron/mixing.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1194 2021-04-03 13:16:13.000000 minimulti-0.3.8/minimulti/electron/modifier.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    10256 2021-04-01 13:19:09.000000 minimulti-0.3.8/minimulti/electron/myNN.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     8922 2021-04-19 19:31:52.000000 minimulti-0.3.8/minimulti/electron/occupations.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     3710 2021-04-19 20:35:17.000000 minimulti-0.3.8/minimulti/electron/pdos.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8437 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/plot.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)   155570 2021-04-19 19:25:21.000000 minimulti-0.3.8/minimulti/electron/pythtb.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     5254 2021-04-19 19:19:15.000000 minimulti-0.3.8/minimulti/electron/spherical_harmonic.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4015 2021-04-03 13:22:05.000000 minimulti-0.3.8/minimulti/electron/susceptibility.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      600 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/test_pert.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2007 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/electron/utils.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    13283 2020-06-11 12:58:20.000000 minimulti-0.3.8/minimulti/electron/wannier90.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/ioput/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       51 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7052 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/base_parser.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)     2794 2021-01-27 15:41:07.000000 minimulti-0.3.8/minimulti/ioput/ifc_netcdf.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    12331 2021-01-27 20:41:13.000000 minimulti-0.3.8/minimulti/ioput/ifc_parser.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)       60 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/spin_nc.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/spin_pot_nc.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/spin_ucl.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7500 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/spin_xml.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)      229 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/ioput/to_hdf.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/lattice/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       23 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/lattice/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    10084 2020-11-08 09:08:47.000000 minimulti-0.3.8/minimulti/lattice/file_io.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      480 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/lattice/latt_obs.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    16301 2021-01-28 08:55:09.000000 minimulti-0.3.8/minimulti/lattice/lattice.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      512 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/lattice/lattice_model.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      310 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/lattice/lattice_mover.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2701 2020-11-08 09:09:15.000000 minimulti-0.3.8/minimulti/lattice/mytb.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/learn/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/learn/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      874 2021-02-15 16:34:42.000000 minimulti-0.3.8/minimulti/learn/polynomial.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/manager/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       32 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/manager/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      753 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/manager/abstract_manager.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      184 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/manager/lattice_manager.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2021-01-28 09:35:17.000000 minimulti-0.3.8/minimulti/manager/spin_lattice_manager.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2331 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/manager/spin_manager.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/math/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       23 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/math/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      575 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/math/geometry.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      300 2020-03-24 09:41:51.000000 minimulti-0.3.8/minimulti/math/linalg.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     5553 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/math/pert.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/model_data/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       34 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/model_data/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1026 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/model_data/model_data.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/mover/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/mover/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)       61 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/mover/lattice_mover.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/plot/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       28 2020-03-23 10:16:06.000000 minimulti-0.3.8/minimulti/plot/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1672 2020-04-17 13:13:02.000000 minimulti-0.3.8/minimulti/plot/plot.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.923169 minimulti-0.3.8/minimulti/scdm/
--rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-04-16 08:15:10.000000 minimulti-0.3.8/minimulti/scdm/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     8068 2020-04-16 08:09:57.000000 minimulti-0.3.8/minimulti/scdm/downfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3566 2020-04-15 15:30:12.000000 minimulti-0.3.8/minimulti/scdm/lwf.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3269 2020-03-11 18:22:18.000000 minimulti-0.3.8/minimulti/scdm/mytb.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1297 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/scdm/rebase.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14391 2020-04-17 17:49:21.000000 minimulti-0.3.8/minimulti/scdm/scdmk.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1968 2020-03-26 14:21:47.000000 minimulti-0.3.8/minimulti/scdm/sisl_downfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2132 2020-04-17 16:43:21.000000 minimulti-0.3.8/minimulti/scdm/test_scdm.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      232 2020-03-20 21:56:34.000000 minimulti-0.3.8/minimulti/scdm/test_svd.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/spin/
--rw-r--r--   0 hexu      (1000) hexu      (1000)      106 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7080 2021-11-04 12:15:01.000000 minimulti-0.3.8/minimulti/spin/builder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    14503 2021-11-04 11:25:45.000000 minimulti-0.3.8/minimulti/spin/hamiltonian.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     9869 2021-11-04 11:04:26.000000 minimulti-0.3.8/minimulti/spin/hamiltonian_terms.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2635 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin/hist_file.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1143 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin/mathcore.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    10108 2021-11-04 11:27:12.000000 minimulti-0.3.8/minimulti/spin/mover.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      403 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin/parameters.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     7049 2021-11-04 10:01:00.000000 minimulti-0.3.8/minimulti/spin/plot.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2176 2021-11-04 09:57:11.000000 minimulti-0.3.8/minimulti/spin/qsolver.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2270 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin/spin_api.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    10911 2021-11-04 10:23:42.000000 minimulti-0.3.8/minimulti/spin/spin_xml.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/spin_lattice_coupling/
--rw-r--r--   0 hexu      (1000) hexu      (1000)       19 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin_lattice_coupling/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    15292 2020-04-17 19:02:57.000000 minimulti-0.3.8/minimulti/spin_lattice_coupling/fit_forces.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1044 2020-04-20 08:08:15.000000 minimulti-0.3.8/minimulti/spin_lattice_coupling/fitting.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)    18876 2020-04-07 13:25:43.000000 minimulti-0.3.8/minimulti/spin_lattice_coupling/slc.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/spin_lattice_model/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin_lattice_model/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3063 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/spin_lattice_model/spin_lattice_model.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/total/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/total/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1084 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/total/model.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/unfolding/
--rw-r--r--   0 hexu      (1000) hexu      (1000)     8267 2021-02-22 21:32:23.000000 minimulti-0.3.8/minimulti/unfolding/DDB_unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)      121 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/unfolding/__init__.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4766 2021-02-22 21:22:09.000000 minimulti-0.3.8/minimulti/unfolding/phonon_unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     3280 2021-02-19 08:49:51.000000 minimulti-0.3.8/minimulti/unfolding/phonopy_unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     2542 2021-02-22 21:21:50.000000 minimulti-0.3.8/minimulti/unfolding/plotphon.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4943 2021-05-28 14:47:22.000000 minimulti-0.3.8/minimulti/unfolding/unfolder.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     5253 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/unfolding/wannier_unfold.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.927169 minimulti-0.3.8/minimulti/utils/
--rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/utils/__init__.py
--rw-rw-r--   0 hexu      (1000) hexu      (1000)    14447 2021-11-04 10:21:18.000000 minimulti-0.3.8/minimulti/utils/supercell.py
--rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1165 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/utils/symbol.py
--rw-r--r--   0 hexu      (1000) hexu      (1000)     1166 2019-12-27 14:10:04.000000 minimulti-0.3.8/minimulti/utils/symbols.py
-drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-11-04 12:19:29.915169 minimulti-0.3.8/minimulti.egg-info/
--rw-r--r--   0 hexu      (1000) hexu      (1000)      413 2021-11-04 12:19:29.000000 minimulti-0.3.8/minimulti.egg-info/PKG-INFO
--rw-r--r--   0 hexu      (1000) hexu      (1000)     4047 2021-11-04 12:19:29.000000 minimulti-0.3.8/minimulti.egg-info/SOURCES.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)        1 2021-11-04 12:19:29.000000 minimulti-0.3.8/minimulti.egg-info/dependency_links.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)       58 2021-11-04 12:19:29.000000 minimulti-0.3.8/minimulti.egg-info/requires.txt
--rw-r--r--   0 hexu      (1000) hexu      (1000)       10 2021-11-04 12:19:29.000000 minimulti-0.3.8/minimulti.egg-info/top_level.txt
--rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2021-11-04 12:19:29.927169 minimulti-0.3.8/setup.cfg
--rw-rw-r--   0 hexu      (1000) hexu      (1000)      848 2021-11-04 12:19:23.000000 minimulti-0.3.8/setup.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.190896 minimulti-0.3.9/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      413 2021-12-11 20:14:30.190896 minimulti-0.3.9/PKG-INFO
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1087 2021-02-14 09:32:33.000000 minimulti-0.3.9/README.md
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.154895 minimulti-0.3.9/minimulti/
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.158896 minimulti-0.3.9/minimulti/LWF/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-07-11 14:41:03.000000 minimulti-0.3.9/minimulti/LWF/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       96 2021-07-05 09:37:20.000000 minimulti-0.3.9/minimulti/LWF/lwf.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     6892 2021-07-09 20:01:21.000000 minimulti-0.3.9/minimulti/LWF/lwf_to_atoms_batch.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/__init__.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.158896 minimulti-0.3.9/minimulti/abstract/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       50 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/abstract_coupling.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      878 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/abstract_hamiltonian.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      844 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/abstract_model.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      140 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/abstract_mover.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      876 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/abstract/abstract_potential.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7742 2021-02-24 09:19:55.000000 minimulti-0.3.9/minimulti/abstract/datatype.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      741 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/constants.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.166895 minimulti-0.3.9/minimulti/electron/
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     7067 2020-05-05 13:21:25.000000 minimulti-0.3.9/minimulti/electron/COHP.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    17506 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/HF.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    52456 2021-04-19 20:43:12.000000 minimulti-0.3.9/minimulti/electron/Hamiltonian.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    16167 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/Hubbard.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    22312 2021-01-28 10:01:07.000000 minimulti-0.3.9/minimulti/electron/Hubbard_4ind.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    19444 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/Hubbard_old.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    11972 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/Hubbard_old2.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.170896 minimulti-0.3.9/minimulti/electron/TB/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/TB/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    11917 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/TB/myTB.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10537 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/TB/mypythtb.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3137 2021-04-01 13:12:22.000000 minimulti-0.3.9/minimulti/electron/UJfitter.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    20830 2021-04-01 13:12:48.000000 minimulti-0.3.9/minimulti/electron/U_matrix.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     8175 2021-04-18 09:38:40.000000 minimulti-0.3.9/minimulti/electron/basis2.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.170896 minimulti-0.3.9/minimulti/electron/box/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/box/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1028 2021-04-13 20:39:14.000000 minimulti-0.3.9/minimulti/electron/box/dummymixer.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2479 2021-04-19 20:35:49.000000 minimulti-0.3.9/minimulti/electron/box/pulay.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.170896 minimulti-0.3.9/minimulti/electron/builder/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       26 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/builder/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2667 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/builder/perovskite.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2811 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/constraint.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     8495 2021-04-19 19:31:38.000000 minimulti-0.3.9/minimulti/electron/density.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    12935 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/epc.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     5001 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/from_banddownfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4989 2021-04-15 18:52:00.000000 minimulti-0.3.9/minimulti/electron/hopping.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    10019 2021-04-19 20:49:57.000000 minimulti-0.3.9/minimulti/electron/ijR.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      420 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/ioput.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10629 2021-04-01 13:19:01.000000 minimulti-0.3.9/minimulti/electron/lwf.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3318 2021-04-19 19:41:50.000000 minimulti-0.3.9/minimulti/electron/mixing.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1194 2021-04-03 13:16:13.000000 minimulti-0.3.9/minimulti/electron/modifier.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    10256 2021-04-01 13:19:09.000000 minimulti-0.3.9/minimulti/electron/myNN.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     8922 2021-04-19 19:31:52.000000 minimulti-0.3.9/minimulti/electron/occupations.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     3710 2021-04-19 20:35:17.000000 minimulti-0.3.9/minimulti/electron/pdos.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     8437 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/plot.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)   155570 2021-04-19 19:25:21.000000 minimulti-0.3.9/minimulti/electron/pythtb.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     5254 2021-04-19 19:19:15.000000 minimulti-0.3.9/minimulti/electron/spherical_harmonic.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4015 2021-04-03 13:22:05.000000 minimulti-0.3.9/minimulti/electron/susceptibility.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      600 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/test_pert.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2007 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/electron/utils.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    13283 2020-06-11 12:58:20.000000 minimulti-0.3.9/minimulti/electron/wannier90.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.174896 minimulti-0.3.9/minimulti/ioput/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       51 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7052 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/base_parser.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)     2794 2021-01-27 15:41:07.000000 minimulti-0.3.9/minimulti/ioput/ifc_netcdf.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    12331 2021-01-27 20:41:13.000000 minimulti-0.3.9/minimulti/ioput/ifc_parser.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       60 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/spin_nc.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/spin_pot_nc.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/spin_ucl.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7500 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/spin_xml.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)      229 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/ioput/to_hdf.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.174896 minimulti-0.3.9/minimulti/lattice/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       23 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/lattice/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    10084 2020-11-08 09:08:47.000000 minimulti-0.3.9/minimulti/lattice/file_io.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      480 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/lattice/latt_obs.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    16301 2021-01-28 08:55:09.000000 minimulti-0.3.9/minimulti/lattice/lattice.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      512 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/lattice/lattice_model.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      310 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/lattice/lattice_mover.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2701 2020-11-08 09:09:15.000000 minimulti-0.3.9/minimulti/lattice/mytb.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.174896 minimulti-0.3.9/minimulti/learn/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/learn/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      874 2021-02-15 16:34:42.000000 minimulti-0.3.9/minimulti/learn/polynomial.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.178896 minimulti-0.3.9/minimulti/manager/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       32 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/manager/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      753 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/manager/abstract_manager.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      184 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/manager/lattice_manager.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2021-01-28 09:35:17.000000 minimulti-0.3.9/minimulti/manager/spin_lattice_manager.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2331 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/manager/spin_manager.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.178896 minimulti-0.3.9/minimulti/math/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       23 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/math/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      575 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/math/geometry.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      300 2020-03-24 09:41:51.000000 minimulti-0.3.9/minimulti/math/linalg.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     5553 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/math/pert.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.178896 minimulti-0.3.9/minimulti/model_data/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       34 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/model_data/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1026 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/model_data/model_data.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.178896 minimulti-0.3.9/minimulti/mover/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/mover/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       61 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/mover/lattice_mover.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.178896 minimulti-0.3.9/minimulti/plot/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       28 2020-03-23 10:16:06.000000 minimulti-0.3.9/minimulti/plot/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1672 2020-04-17 13:13:02.000000 minimulti-0.3.9/minimulti/plot/plot.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.182896 minimulti-0.3.9/minimulti/scdm/
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)        0 2020-04-16 08:15:10.000000 minimulti-0.3.9/minimulti/scdm/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     8068 2020-04-16 08:09:57.000000 minimulti-0.3.9/minimulti/scdm/downfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3566 2020-04-15 15:30:12.000000 minimulti-0.3.9/minimulti/scdm/lwf.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3269 2020-03-11 18:22:18.000000 minimulti-0.3.9/minimulti/scdm/mytb.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1297 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/scdm/rebase.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14391 2020-04-17 17:49:21.000000 minimulti-0.3.9/minimulti/scdm/scdmk.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1968 2020-03-26 14:21:47.000000 minimulti-0.3.9/minimulti/scdm/sisl_downfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2132 2020-04-17 16:43:21.000000 minimulti-0.3.9/minimulti/scdm/test_scdm.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      232 2020-03-20 21:56:34.000000 minimulti-0.3.9/minimulti/scdm/test_svd.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.182896 minimulti-0.3.9/minimulti/spin/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      106 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7080 2021-11-04 12:15:01.000000 minimulti-0.3.9/minimulti/spin/builder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    14503 2021-11-04 11:25:45.000000 minimulti-0.3.9/minimulti/spin/hamiltonian.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     9869 2021-11-04 11:04:26.000000 minimulti-0.3.9/minimulti/spin/hamiltonian_terms.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2635 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin/hist_file.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1143 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin/mathcore.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    10108 2021-11-04 12:29:00.000000 minimulti-0.3.9/minimulti/spin/mover.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      403 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin/parameters.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     7049 2021-11-04 10:01:00.000000 minimulti-0.3.9/minimulti/spin/plot.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2176 2021-11-04 09:57:11.000000 minimulti-0.3.9/minimulti/spin/qsolver.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2270 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin/spin_api.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    10911 2021-11-04 10:23:42.000000 minimulti-0.3.9/minimulti/spin/spin_xml.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.186896 minimulti-0.3.9/minimulti/spin_lattice_coupling/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       19 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin_lattice_coupling/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    15292 2020-04-17 19:02:57.000000 minimulti-0.3.9/minimulti/spin_lattice_coupling/fit_forces.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1044 2020-04-20 08:08:15.000000 minimulti-0.3.9/minimulti/spin_lattice_coupling/fitting.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)    18876 2020-04-07 13:25:43.000000 minimulti-0.3.9/minimulti/spin_lattice_coupling/slc.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.186896 minimulti-0.3.9/minimulti/spin_lattice_model/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin_lattice_model/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3063 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/spin_lattice_model/spin_lattice_model.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.186896 minimulti-0.3.9/minimulti/total/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/total/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1084 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/total/model.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.190896 minimulti-0.3.9/minimulti/unfolding/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     8532 2021-12-11 19:36:40.000000 minimulti-0.3.9/minimulti/unfolding/DDB_unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      121 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/unfolding/__init__.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     5494 2021-12-11 14:15:39.000000 minimulti-0.3.9/minimulti/unfolding/phonon_unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     3280 2021-02-19 08:49:51.000000 minimulti-0.3.9/minimulti/unfolding/phonopy_unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     2542 2021-02-22 21:21:50.000000 minimulti-0.3.9/minimulti/unfolding/plotphon.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4943 2021-05-28 14:47:22.000000 minimulti-0.3.9/minimulti/unfolding/unfolder.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     5253 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/unfolding/wannier_unfold.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.190896 minimulti-0.3.9/minimulti/utils/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        0 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/utils/__init__.py
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)    14447 2021-11-04 10:21:18.000000 minimulti-0.3.9/minimulti/utils/supercell.py
+-rwxr-xr-x   0 hexu      (1000) hexu      (1000)     1165 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/utils/symbol.py
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     1166 2019-12-27 14:10:04.000000 minimulti-0.3.9/minimulti/utils/symbols.py
+drwxrwxr-x   0 hexu      (1000) hexu      (1000)        0 2021-12-11 20:14:30.158896 minimulti-0.3.9/minimulti.egg-info/
+-rw-r--r--   0 hexu      (1000) hexu      (1000)      413 2021-12-11 20:14:29.000000 minimulti-0.3.9/minimulti.egg-info/PKG-INFO
+-rw-r--r--   0 hexu      (1000) hexu      (1000)     4047 2021-12-11 20:14:29.000000 minimulti-0.3.9/minimulti.egg-info/SOURCES.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)        1 2021-12-11 20:14:29.000000 minimulti-0.3.9/minimulti.egg-info/dependency_links.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       58 2021-12-11 20:14:29.000000 minimulti-0.3.9/minimulti.egg-info/requires.txt
+-rw-r--r--   0 hexu      (1000) hexu      (1000)       10 2021-12-11 20:14:29.000000 minimulti-0.3.9/minimulti.egg-info/top_level.txt
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)       38 2021-12-11 20:14:30.190896 minimulti-0.3.9/setup.cfg
+-rw-rw-r--   0 hexu      (1000) hexu      (1000)      848 2021-12-11 20:14:26.000000 minimulti-0.3.9/setup.py
```

### Comparing `minimulti-0.3.8/README.md` & `minimulti-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/LWF/lwf_to_atoms_batch.py` & `minimulti-0.3.9/minimulti/LWF/lwf_to_atoms_batch.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/abstract/abstract_hamiltonian.py` & `minimulti-0.3.9/minimulti/abstract/abstract_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/abstract/abstract_model.py` & `minimulti-0.3.9/minimulti/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/abstract/abstract_potential.py` & `minimulti-0.3.9/minimulti/abstract/abstract_potential.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/abstract/datatype.py` & `minimulti-0.3.9/minimulti/abstract/datatype.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/constants.py` & `minimulti-0.3.9/minimulti/constants.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/COHP.py` & `minimulti-0.3.9/minimulti/electron/COHP.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/HF.py` & `minimulti-0.3.9/minimulti/electron/HF.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/Hamiltonian.py` & `minimulti-0.3.9/minimulti/electron/Hamiltonian.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/Hubbard.py` & `minimulti-0.3.9/minimulti/electron/Hubbard.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/Hubbard_4ind.py` & `minimulti-0.3.9/minimulti/electron/Hubbard_4ind.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/Hubbard_old.py` & `minimulti-0.3.9/minimulti/electron/Hubbard_old.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/Hubbard_old2.py` & `minimulti-0.3.9/minimulti/electron/Hubbard_old2.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/TB/myTB.py` & `minimulti-0.3.9/minimulti/electron/TB/myTB.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/TB/mypythtb.py` & `minimulti-0.3.9/minimulti/electron/TB/mypythtb.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/UJfitter.py` & `minimulti-0.3.9/minimulti/electron/UJfitter.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/U_matrix.py` & `minimulti-0.3.9/minimulti/electron/U_matrix.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/basis2.py` & `minimulti-0.3.9/minimulti/electron/basis2.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/box/dummymixer.py` & `minimulti-0.3.9/minimulti/electron/box/dummymixer.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/box/pulay.py` & `minimulti-0.3.9/minimulti/electron/box/pulay.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/builder/perovskite.py` & `minimulti-0.3.9/minimulti/electron/builder/perovskite.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/constraint.py` & `minimulti-0.3.9/minimulti/electron/constraint.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/density.py` & `minimulti-0.3.9/minimulti/electron/density.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/epc.py` & `minimulti-0.3.9/minimulti/electron/epc.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/from_banddownfolder.py` & `minimulti-0.3.9/minimulti/electron/from_banddownfolder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/hopping.py` & `minimulti-0.3.9/minimulti/electron/hopping.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/ijR.py` & `minimulti-0.3.9/minimulti/electron/ijR.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/lwf.py` & `minimulti-0.3.9/minimulti/electron/lwf.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/mixing.py` & `minimulti-0.3.9/minimulti/electron/mixing.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/modifier.py` & `minimulti-0.3.9/minimulti/electron/modifier.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/myNN.py` & `minimulti-0.3.9/minimulti/electron/myNN.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/occupations.py` & `minimulti-0.3.9/minimulti/electron/occupations.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/pdos.py` & `minimulti-0.3.9/minimulti/electron/pdos.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/plot.py` & `minimulti-0.3.9/minimulti/electron/plot.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/pythtb.py` & `minimulti-0.3.9/minimulti/electron/pythtb.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/spherical_harmonic.py` & `minimulti-0.3.9/minimulti/electron/spherical_harmonic.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/susceptibility.py` & `minimulti-0.3.9/minimulti/electron/susceptibility.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/test_pert.py` & `minimulti-0.3.9/minimulti/electron/test_pert.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/utils.py` & `minimulti-0.3.9/minimulti/electron/utils.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/electron/wannier90.py` & `minimulti-0.3.9/minimulti/electron/wannier90.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/ioput/base_parser.py` & `minimulti-0.3.9/minimulti/ioput/base_parser.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/ioput/ifc_netcdf.py` & `minimulti-0.3.9/minimulti/ioput/ifc_netcdf.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/ioput/ifc_parser.py` & `minimulti-0.3.9/minimulti/ioput/ifc_parser.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/ioput/spin_xml.py` & `minimulti-0.3.9/minimulti/ioput/spin_xml.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/lattice/file_io.py` & `minimulti-0.3.9/minimulti/lattice/file_io.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/lattice/lattice.py` & `minimulti-0.3.9/minimulti/lattice/lattice.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/lattice/lattice_model.py` & `minimulti-0.3.9/minimulti/lattice/lattice_model.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/lattice/mytb.py` & `minimulti-0.3.9/minimulti/lattice/mytb.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/learn/polynomial.py` & `minimulti-0.3.9/minimulti/learn/polynomial.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/manager/abstract_manager.py` & `minimulti-0.3.9/minimulti/manager/abstract_manager.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/manager/spin_manager.py` & `minimulti-0.3.9/minimulti/manager/spin_manager.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/math/geometry.py` & `minimulti-0.3.9/minimulti/math/geometry.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/math/pert.py` & `minimulti-0.3.9/minimulti/math/pert.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/model_data/model_data.py` & `minimulti-0.3.9/minimulti/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/plot/plot.py` & `minimulti-0.3.9/minimulti/plot/plot.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/downfolder.py` & `minimulti-0.3.9/minimulti/scdm/downfolder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/lwf.py` & `minimulti-0.3.9/minimulti/scdm/lwf.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/mytb.py` & `minimulti-0.3.9/minimulti/scdm/mytb.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/rebase.py` & `minimulti-0.3.9/minimulti/scdm/rebase.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/scdmk.py` & `minimulti-0.3.9/minimulti/scdm/scdmk.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/sisl_downfolder.py` & `minimulti-0.3.9/minimulti/scdm/sisl_downfolder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/scdm/test_scdm.py` & `minimulti-0.3.9/minimulti/scdm/test_scdm.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/builder.py` & `minimulti-0.3.9/minimulti/spin/builder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/hamiltonian.py` & `minimulti-0.3.9/minimulti/spin/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/hamiltonian_terms.py` & `minimulti-0.3.9/minimulti/spin/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/hist_file.py` & `minimulti-0.3.9/minimulti/spin/hist_file.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/mathcore.py` & `minimulti-0.3.9/minimulti/spin/mathcore.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/mover.py` & `minimulti-0.3.9/minimulti/spin/mover.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/plot.py` & `minimulti-0.3.9/minimulti/spin/plot.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/qsolver.py` & `minimulti-0.3.9/minimulti/spin/qsolver.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/spin_api.py` & `minimulti-0.3.9/minimulti/spin/spin_api.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin/spin_xml.py` & `minimulti-0.3.9/minimulti/spin/spin_xml.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin_lattice_coupling/fit_forces.py` & `minimulti-0.3.9/minimulti/spin_lattice_coupling/fit_forces.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin_lattice_coupling/fitting.py` & `minimulti-0.3.9/minimulti/spin_lattice_coupling/fitting.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin_lattice_coupling/slc.py` & `minimulti-0.3.9/minimulti/spin_lattice_coupling/slc.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/spin_lattice_model/spin_lattice_model.py` & `minimulti-0.3.9/minimulti/spin_lattice_model/spin_lattice_model.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/total/model.py` & `minimulti-0.3.9/minimulti/total/model.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/unfolding/DDB_unfolder.py` & `minimulti-0.3.9/minimulti/unfolding/DDB_unfolder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 #!/usr/bin/env python
+from .plotphon import plot_band_weight
+from .phonon_unfolder import phonon_unfolder
+import sys
+import matplotlib.pyplot as plt
+from ase.dft.kpoints import get_special_points, bandpath
+from ase.build import bulk
+from ase.io import write
+import numpy as np
 has_abipy = False
 try:
     import abipy.abilab as abilab
     has_abipy = True
 except:
     has_abipy = False
-import numpy as np
-from ase.build import bulk
-from ase.dft.kpoints import get_special_points, bandpath
-import matplotlib.pyplot as plt
-import sys
-from .phonon_unfolder import phonon_unfolder
-from .plotphon import plot_band_weight
 
 atomic_masses = np.array([
     1., 1.008, 4.002602, 6.94, 9.0121831, 10.81, 12.011, 14.007, 15.999,
     18.99840316, 20.1797, 22.98976928, 24.305, 26.9815385, 28.085, 30.973762,
     32.06, 35.45, 39.948, 39.0983, 40.078, 44.955908, 47.867, 50.9415, 51.9961,
     54.938044, 55.845, 58.933194, 58.6934, 63.546, 65.38, 69.723, 72.63,
     74.921595, 78.971, 79.904, 83.798, 85.4678, 87.62, 88.90584, 91.224,
@@ -86,125 +87,133 @@
     scaled_positions = struct.frac_coords
 
     cell = struct.lattice_vectors()
     numbers = struct.atomic_numbers
     masses = [atomic_masses[i] for i in numbers]
 
     phbst, phdos = DDB.anaget_phbst_and_phdos_files(
-        nqsmall=2,
+        nqsmall=0,
         asr=1,
         chneut=1,
         dipdip=dipdip,
         verbose=1,
-        ndivsm=40,
+        ngqpt=[1, 1, 1],
+        #ngqpt=[4, 4, 4],
+        ndivsm=10,
         lo_to_splitting=True,
         qptbounds=kpath_bounds,
+        dipquad=0,
+        quadquad=0,
     )
     qpoints = phbst.qpoints.frac_coords
     nqpts = len(qpoints)
     nbranch = 3 * len(numbers)
     evals = np.zeros([nqpts, nbranch])
     evecs = np.zeros([nqpts, nbranch, nbranch], dtype='complex128')
 
     m = np.sqrt(np.kron(masses, [1, 1, 1]))
-    #positions=np.kron(scaled_positions,[1,1,1])
+    # positions=np.kron(scaled_positions,[1,1,1])
 
     for iqpt, qpt in enumerate(qpoints):
         for ibranch in range(nbranch):
             phmode = phbst.get_phmode(qpt, ibranch)
             evals[iqpt, ibranch] = phmode.freq
             evec = displacement_cart_to_evec(phmode.displ_cart,
                                              masses,
                                              scaled_positions,
                                              qpoint=qpt,
                                              add_phase=True)
             evecs[iqpt, :, ibranch] = evec
 
     uf = phonon_unfolder(atoms, sc_mat, evecs, qpoints, phase=False)
+    print("Getting weights")
     weights = uf.get_weights()
+    print("weights got")
     x = np.arange(nqpts)
     freqs = evals
     xpts = []
     for ix, xx in enumerate(x):
         for q in kpath_bounds:
-            if np.sum((np.array(qpoints[ix]) - np.array(q))**
-                      2) < 0.00001 and ix not in xpts:
+            if np.sum((np.array(qpoints[ix]) - np.array(q)) **
+                      2) < 0.00000001 and ix not in xpts:
                 xpts.append(ix)
     if knames is None:
         knames = [str(k) for k in kpath_bounds]
     ax = plot_band_weight([list(x)] * freqs.shape[1],
                           freqs.T * 8065.6,
-                          weights[:, :].T * 0.98 + 0.01,
+                          weights[:, :].T * 0.95 + 0.01,
                           xticks=[knames, xpts],
                           style='alpha')
     return ax
 
 
 def nc_unfolder(fname,
                 sc_mat,
                 kx=None,
                 knames=None,
-                ghost_atoms=None,
+                # ghost_atoms=None,
                 plot_width=False,
                 weight_multiplied_by=None):
     if not has_abipy:
         raise Exception("Please install abipy to use nc_unfolder")
 
     ncfile = abilab.abiopen(fname)
     struct = ncfile.structure
     atoms = ncfile.structure.to_ase_atoms()
     scaled_positions = struct.frac_coords
 
     cell = struct.lattice_vectors()
     numbers = struct.atomic_numbers
     masses = [atomic_masses[i] for i in numbers]
 
-    #print numbers
-    #print cell
-    #print scaled_positions
+    # print numbers
+    # print cell
+    # print scaled_positions
 
-    #print kpath_bounds
+    # print kpath_bounds
 
     phbst = ncfile.phbands
-    #phbst.plot_phbands()
+    # phbst.plot_phbands()
     qpoints = phbst.qpoints.frac_coords
     nqpts = len(qpoints)
     nbranch = 3 * len(numbers)
     evals = np.zeros([nqpts, nbranch])
     evecs = np.zeros([nqpts, nbranch, nbranch], dtype='complex128')
 
     m = np.sqrt(np.kron(masses, [1, 1, 1]))
-    #positions=np.kron(scaled_positions,[1,1,1])
+    # positions=np.kron(scaled_positions,[1,1,1])
     freqs = phbst.phfreqs
     displ_carts = phbst.phdispl_cart
 
     for iqpt, qpt in enumerate(qpoints):
         print(iqpt, qpt)
         for ibranch in range(nbranch):
             #phmode = ncfile.get_phmode(qpt, ibranch)
-            #print(2)
+            # print(2)
             evals[iqpt, ibranch] = freqs[iqpt, ibranch]
             #evec=phmode.displ_cart *m
             #phase = [np.exp(-2j*np.pi*np.dot(pos,qpt)) for pos in scaled_positions]
             #phase = np.kron(phase,[1,1,1])
-            #evec*=phase
+            # evec*=phase
             #evec /= np.linalg.norm(evec)
             evec = displacement_cart_to_evec(displ_carts[iqpt, ibranch, :],
                                              masses,
                                              scaled_positions,
                                              qpoint=qpt,
                                              add_phase=True)
             evecs[iqpt, :, ibranch] = evec
 
     uf = phonon_unfolder(atoms,
                          sc_mat,
                          evecs,
                          qpoints,
                          phase=False,
-                         ghost_atoms=ghost_atoms)
+                         # ghost_atoms=ghost_atoms
+                         )
+    write("atoms.vasp", atoms, vasp5=True, sort=True)
     weights = uf.get_weights()
     if plot_width:
         weights = (weights * (1.0 - weights))**(0.5)
     if weight_multiplied_by is not None:
         weights = weights * weight_multiplied_by
     x = np.arange(nqpts)
     freqs = evals
@@ -220,11 +229,11 @@
     """example of how to use DDB_unfolder
     """
     # supercell matrix
     sc_mat = np.eye(3)*2
     # kpath in primitive cell
     kpoints = np.array([(0, 0, 0), (0, .5, 0), (0.5, 0.5, 0), [.5, .5, .5],
                         [0, 0, 0]])
-    # Note the k.sc_mat should be used instead of k. 
+    # Note the k.sc_mat should be used instead of k.
     DDB_unfolder(DDB_fname='out_DDB',
                  kpath_bounds=[np.dot(k, sc_mat) for k in kpoints],
                  sc_mat=sc_mat, knames=['$\Gamma$', 'X', 'M', 'R', '$\Gamma$'])
```

### Comparing `minimulti-0.3.8/minimulti/unfolding/phonon_unfolder.py` & `minimulti-0.3.9/minimulti/unfolding/phonon_unfolder.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,109 +2,134 @@
 Phonon unfolding: Reciprocal space method. The method is described in
 P. B. Allen et al. Phys Rev B 87, 085322 (2013).
 This method should be also applicable to other bloch waves on discrete grid, eg. electrons wave function in wannier basis set, magnons, etc. Now only phonon istested.
 """
 from ase.build import make_supercell
 from ase.atoms import Atoms
 import numpy as np
+import numba
+
+@numba.njit()
+def close_to_int(x, tol_r):
+    return np.all(np.abs(x - np.rint(x)) < tol_r)
+
+@numba.njit()
+def match(rs, positions, _ndim, tol_r, indices):
+    for i, ri in enumerate(rs):
+        Tpositions = positions + ri
+        for i_atom, pos in enumerate(positions):
+            for j_atom, Tpos in enumerate(Tpositions):
+                dpos = Tpos - pos
+                if close_to_int(dpos, tol_r):
+                    indices[i, j_atom * _ndim:j_atom * _ndim + _ndim] = np.arange(
+                        i_atom * _ndim, i_atom * _ndim + _ndim)
+    return indices
+
+
 
 class phonon_unfolder:
     """ phonon unfolding class"""
 
-    def __init__(self, atoms, supercell_matrix, eigenvectors, qpoints, tol_r=0.04, ndim=3,labels=None,compare=None,phase=True):
+    def __init__(self, atoms, supercell_matrix, eigenvectors, qpoints, tol_r=0.04, ndim=3, labels=None, compare=None, phase=True):
         """
         Params:
         ===================
         atoms: The structure of supercell.
         supercell matrix: The matrix that convert the primitive cell to supercell.
         eigenvectors: The phonon eigenvectors. format np.array() index=[ikpts, ifreq, 3*iatoms+j]. j=0..2
         qpoints: list of q-points, note the q points are in the BZ of the supercell. 
         tol_r: tolerance. If abs(a-b) <r, they are seen as the same atom.
         ndim: number of dimensions. For 3D phonons, use ndim=3. For electrons(no spin), ndim=1. For spinors, use ndim=2 (TODO: spinor not tested. is it correct?).
         labels: labels of the basis. for 3D phonons, ndim can be set to 1 alternately, with labels set to ['x','y','z']*natoms. The labels are used to decide if two basis are identical by translation. (Not used for phonon)
         compare: how to decide the basis are identical (Not used for phonon)
-        
+
         """
         self._atoms = atoms
         self._scmat = supercell_matrix
         self._evecs = eigenvectors
         self._qpts = qpoints
         self._tol_r = tol_r
         self._ndim = ndim
-        self._labels=labels
+        self._labels = labels
         self._trans_rs = None
         self._trans_indices = None
         self._make_translate_maps()
-        self._phase=phase
+        self._phase = phase
         return
 
     def _translate(self, evec, r):
         """
         T(r) psi: r is integer numbers of primitive cell lattice matrix.
         Params:
         =================
         evec: an eigen vector of supercell
         r: The translate vector
-        
+
         Returns:
         ================
          tevec: translated vector.
         """
         pass
 
     def _make_translate_maps(self):
         """
         find the mapping between supercell and translated cell.
         Returns:
         ===============
         A N * (ndim*natoms) array.
         index[i] is the mapping from supercell to translated supercell so that
         T(r_i) psi = psi[indices[i]].
-        
+
         TODO: vacancies/add_atoms not supported. How to do it? For vacancies, a ghost atom can be added. For add_atom, maybe we can just ignore them? Will it change the energy spectrum?
         """
         a1 = Atoms(symbols='H', positions=[(0, 0, 0)], cell=[1, 1, 1])
         sc = make_supercell(a1, self._scmat)
         rs = sc.get_scaled_positions()
         positions = np.array(self._atoms.get_scaled_positions())
-        indices = np.zeros([len(rs), len(positions) * self._ndim], dtype='int32')
-        for i, ri in enumerate(rs):
-            inds = []
-            Tpositions = positions + np.array(ri)
-            close_to_int = lambda x: np.all(np.abs(x - np.round(x)) < self._tol_r)
-            for i_atom, pos in enumerate(positions):
-                for j_atom, Tpos in enumerate(Tpositions):
-                    dpos = Tpos - pos
-                    if close_to_int(dpos):
-                        indices[i, j_atom * self._ndim:j_atom * self._ndim + self._ndim] = np.arange(i_atom * self._ndim, i_atom * self._ndim + self._ndim)
+        indices = np.zeros(
+            [len(rs), len(positions) * self._ndim], dtype='int32')
+
+        print("matching")
+        match(rs, positions, self._ndim, self._tol_r, indices)
+        #for i, ri in enumerate(rs):
+        #    Tpositions = positions + np.array(ri)
+        #    for i_atom, pos in enumerate(positions):
+        #        for j_atom, Tpos in enumerate(Tpositions):
+        #            dpos = Tpos - pos
+        #            if close_to_int(dpos, self._tol_r):
+        #                indices[i, j_atom * self._ndim:j_atom * self._ndim + self._ndim] = np.arange(
+        #                    i_atom * self._ndim, i_atom * self._ndim + self._ndim)
 
         self._trans_rs = rs
         self._trans_indices = indices
-        #print indices
+        # print indices
 
-    def get_weight(self, evec, qpt, G=np.array([0,0,0]) ):
+    def get_weight(self, evec, qpt, G=np.array([0, 0, 0])):
         """
         get the weight of a mode which has the wave vector of qpt and eigenvector of evec.
         W= sum_1^N < evec| T(r_i)exp(-I (K+G) * r_i| evec>, here G=0. T(r_i)exp(-I K r_i)| evec> = evec[indices[i]]
         """
         weight = 0j
         N = len(self._trans_rs)
         for r_i, ind in zip(self._trans_rs, self._trans_indices):
             if self._phase:
-                weight += np.vdot(evec, evec[ind])*np.exp(-1j *2 * np.pi * np.dot(qpt+G,r_i))  /N
+                weight += np.vdot(evec, evec[ind])*np.exp(-1j *
+                                                          2 * np.pi * np.dot(qpt+G, r_i)) / N
             else:
-                weight += np.vdot(evec, evec[ind]) / N*np.exp(-1j *2 * np.pi * np.dot(G,r_i))  
+                weight += np.vdot(evec, evec[ind]) / N * \
+                    np.exp(-1j * 2 * np.pi * np.dot(G, r_i))
 
         return weight.real
 
     def get_weights(self):
         """
         Get the weight for all the modes.
         """
         nqpts, nfreqs = self._evecs.shape[0], self._evecs.shape[1]
         weights = np.zeros([nqpts, nfreqs])
         for iqpt in range(nqpts):
             for ifreq in range(nfreqs):
-                weights[iqpt, ifreq] = self.get_weight(self._evecs[iqpt, :, ifreq], self._qpts[iqpt])
+                weights[iqpt, ifreq] = self.get_weight(
+                    self._evecs[iqpt, :, ifreq], self._qpts[iqpt])
 
         self._weights = weights
         return self._weights
```

### Comparing `minimulti-0.3.8/minimulti/unfolding/phonopy_unfolder.py` & `minimulti-0.3.9/minimulti/unfolding/phonopy_unfolder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/unfolding/plotphon.py` & `minimulti-0.3.9/minimulti/unfolding/plotphon.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/unfolding/unfolder.py` & `minimulti-0.3.9/minimulti/unfolding/unfolder.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/unfolding/wannier_unfold.py` & `minimulti-0.3.9/minimulti/unfolding/wannier_unfold.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/utils/supercell.py` & `minimulti-0.3.9/minimulti/utils/supercell.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/utils/symbol.py` & `minimulti-0.3.9/minimulti/utils/symbol.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti/utils/symbols.py` & `minimulti-0.3.9/minimulti/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/minimulti.egg-info/SOURCES.txt` & `minimulti-0.3.9/minimulti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minimulti-0.3.8/setup.py` & `minimulti-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 long_description = """minimulti is a python framework of effective potentials, including lattice model, electron (tight-binding+Hubbard), magnetic Heisenberg model, etc """
 
 setup(
     name='minimulti',
-    version='0.3.8',
+    version='0.3.9',
     description='Mini Extendable framework of multi Hamiltonian',
     long_description=long_description,
     author='Xu He',
     author_email='mailhexu@gmail.com',
     license='GPLv3',
     packages=find_packages(),
     package_data={},
```

