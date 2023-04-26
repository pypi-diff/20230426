# Comparing `tmp/featurebox-0.0.9998.tar.gz` & `tmp/featurebox-0.0.9999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebox-0.0.9998.tar", last modified: Sun Feb 26 06:38:22 2023, max compression
+gzip compressed data, was "featurebox-0.0.9999.tar", last modified: Wed Apr 26 13:47:46 2023, max compression
```

## Comparing `featurebox-0.0.9998.tar` & `featurebox-0.0.9999.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.055762 featurebox-0.0.9998/
--rw-rw-rw-   0        0        0     7797 2021-12-17 11:27:06.000000 featurebox-0.0.9998/LICENSE
--rw-rw-rw-   0        0        0      129 2021-12-17 11:27:06.000000 featurebox-0.0.9998/MANIFEST.in
--rw-rw-rw-   0        0        0     2553 2023-02-26 06:38:22.054815 featurebox-0.0.9998/PKG-INFO
--rw-rw-rw-   0        0        0     1372 2022-01-04 11:52:43.000000 featurebox-0.0.9998/README.md
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:21.985816 featurebox-0.0.9998/featurebox/
--rw-rw-rw-   0        0        0       64 2022-08-08 06:09:08.000000 featurebox-0.0.9998/featurebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.003817 featurebox-0.0.9998/featurebox/cli/
--rw-rw-rw-   0        0        0      747 2022-10-15 08:34:40.000000 featurebox-0.0.9998/featurebox/cli/__init__.py
--rw-rw-rw-   0        0        0    13414 2023-02-17 07:06:06.000000 featurebox-0.0.9998/featurebox/cli/_basepathout.py
--rw-rw-rw-   0        0        0     6745 2023-02-22 15:08:51.000000 featurebox-0.0.9998/featurebox/cli/main.py
--rw-rw-rw-   0        0        0      320 2022-10-15 08:34:40.000000 featurebox-0.0.9998/featurebox/cli/template.py
--rw-rw-rw-   0        0        0    10232 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/cli/vasp_bader.py
--rw-rw-rw-   0        0        0    11807 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/cli/vasp_bgp.py
--rw-rw-rw-   0        0        0      913 2022-08-06 15:06:02.000000 featurebox-0.0.9998/featurebox/cli/vasp_chg_diff.py
--rw-rw-rw-   0        0        0    10397 2022-10-15 08:46:16.000000 featurebox-0.0.9998/featurebox/cli/vasp_cohp.py
--rw-rw-rw-   0        0        0     5435 2023-02-21 09:35:25.000000 featurebox-0.0.9998/featurebox/cli/vasp_converge.py
--rw-rw-rw-   0        0        0    37796 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/cli/vasp_dbc.py
--rw-rw-rw-   0        0        0    25116 2022-08-12 08:59:00.000000 featurebox-0.0.9998/featurebox/cli/vasp_dos.py
--rw-rw-rw-   0        0        0     4942 2023-02-17 07:12:55.000000 featurebox-0.0.9998/featurebox/cli/vasp_empty.py
--rw-rw-rw-   0        0        0     7019 2023-02-21 09:34:22.000000 featurebox-0.0.9998/featurebox/cli/vasp_general_diff.py
--rw-rw-rw-   0        0        0     7809 2023-02-19 16:30:44.000000 featurebox-0.0.9998/featurebox/cli/vasp_general_single.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.012800 featurebox-0.0.9998/featurebox/data/
--rw-rw-rw-   0        0        0      167 2022-08-01 08:22:20.000000 featurebox-0.0.9998/featurebox/data/__init__.py
--rw-rw-rw-   0        0        0     6491 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/data/check_data.py
--rw-rw-rw-   0        0        0    10393 2022-10-15 08:47:37.000000 featurebox-0.0.9998/featurebox/data/data_sep.py
--rw-rw-rw-   0        0        0    38626 2021-12-27 15:28:19.000000 featurebox-0.0.9998/featurebox/data/ele_megnet.json
--rw-rw-rw-   0        0        0    37806 2021-12-27 15:28:19.000000 featurebox-0.0.9998/featurebox/data/ele_table.csv
--rw-rw-rw-   0        0        0    47340 2021-12-27 15:28:19.000000 featurebox-0.0.9998/featurebox/data/ele_table_norm.csv
--rw-rw-rw-   0        0        0     2917 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/data/ie.json
--rw-rw-rw-   0        0        0     6763 2022-10-15 08:50:02.000000 featurebox-0.0.9998/featurebox/data/mp_access.py
--rw-rw-rw-   0        0        0     8745 2023-02-19 10:31:47.000000 featurebox-0.0.9998/featurebox/data/name_split.py
--rw-rw-rw-   0        0        0      476 2023-02-05 08:28:56.000000 featurebox-0.0.9998/featurebox/data/namesplit.py
--rw-rw-rw-   0        0        0     7822 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/data/oe.csv
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.014811 featurebox-0.0.9998/featurebox/featurizers/
--rw-rw-rw-   0        0        0       84 2022-10-12 08:15:47.000000 featurebox-0.0.9998/featurebox/featurizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.016816 featurebox-0.0.9998/featurebox/featurizers/atom/
--rw-rw-rw-   0        0        0       22 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/atom/__init__.py
--rw-rw-rw-   0        0        0    27629 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/atom/mapper.py
--rw-rw-rw-   0        0        0    17825 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/featurizers/base_feature.py
--rw-rw-rw-   0        0        0     4086 2022-08-12 09:00:19.000000 featurebox-0.0.9998/featurebox/featurizers/batch_feature.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.020818 featurebox-0.0.9998/featurebox/featurizers/envir/
--rw-rw-rw-   0        0        0      145 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/__init__.py
--rw-rw-rw-   0        0        0     3078 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/featurizers/envir/_get_radius_in_spheres.py
--rw-rw-rw-   0        0        0     6732 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/featurizers/envir/_get_xyz_in_spheres.py
--rw-rw-rw-   0        0        0     2861 2022-11-04 08:32:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/desc_env.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.033762 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/
--rw-rw-rw-   0        0        0    46046 2022-10-15 09:17:09.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/ACSF.py
--rw-rw-rw-   0        0        0    17182 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/EAD.py
--rw-rw-rw-   0        0        0    16250 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/EAMD.py
--rw-rw-rw-   0        0        0    45331 2022-10-15 09:17:09.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SO3.py
--rw-rw-rw-   0        0        0    62762 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SO4.py
--rw-rw-rw-   0        0        0    33591 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SOAP.py
--rw-rw-rw-   0        0        0      271 2022-10-12 08:15:47.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/__init__.py
--rw-rw-rw-   0        0        0      904 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/_generate_coefs.py
--rw-rw-rw-   0        0        0    16420 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/angular_momentum.py
--rw-rw-rw-   0        0        0    43536 2022-10-15 09:17:09.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/behlerparrinello.py
--rw-rw-rw-   0        0        0    50664 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/bispectrum.py
--rw-rw-rw-   0        0        0     4877 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/cutoff.py
--rw-rw-rw-   0        0        0     9684 2022-10-15 09:17:09.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/lbispectrum.py
--rw-rw-rw-   0        0        0      999 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/utils.py
--rw-rw-rw-   0        0        0    34379 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/wACSF.py
--rw-rw-rw-   0        0        0    16373 2022-11-04 08:32:06.000000 featurebox-0.0.9998/featurebox/featurizers/envir/environment.py
--rw-rw-rw-   0        0        0     7980 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/envir/local_env.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.038798 featurebox-0.0.9998/featurebox/featurizers/state/
--rw-rw-rw-   0        0        0       65 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/state/__init__.py
--rw-rw-rw-   0        0        0    12441 2022-10-15 09:31:37.000000 featurebox-0.0.9998/featurebox/featurizers/state/extrastats.py
--rw-rw-rw-   0        0        0      954 2021-12-17 11:27:06.000000 featurebox-0.0.9998/featurebox/featurizers/state/state_mapper.py
--rw-rw-rw-   0        0        0    10989 2022-10-20 14:50:35.000000 featurebox-0.0.9998/featurebox/featurizers/state/statistics.py
--rw-rw-rw-   0        0        0     8329 2022-03-06 10:25:09.000000 featurebox-0.0.9998/featurebox/featurizers/state/union.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.046807 featurebox-0.0.9998/featurebox/pbs/
--rw-rw-rw-   0        0        0      157 2023-02-19 17:25:28.000000 featurebox-0.0.9998/featurebox/pbs/__init__.py
--rw-rw-rw-   0        0        0     3519 2023-02-10 07:49:23.000000 featurebox-0.0.9998/featurebox/pbs/cli.py
--rw-rw-rw-   0        0        0     1683 2023-02-19 17:25:28.000000 featurebox-0.0.9998/featurebox/pbs/jmk.py
--rw-rw-rw-   0        0        0    10498 2023-02-19 17:25:28.000000 featurebox-0.0.9998/featurebox/pbs/job_manager.py
--rw-rw-rw-   0        0        0     4877 2022-12-07 01:59:25.000000 featurebox-0.0.9998/featurebox/pbs/misc.py
--rw-rw-rw-   0        0        0    12164 2023-02-22 04:00:03.000000 featurebox-0.0.9998/featurebox/pbs/misc_slurm.py
--rw-rw-rw-   0        0        0     7827 2023-02-18 07:12:20.000000 featurebox-0.0.9998/featurebox/pbs/misc_torque.py
--rw-rw-rw-   0        0        0     9286 2023-02-19 18:13:40.000000 featurebox-0.0.9998/featurebox/pbs/misc_unischeduler.py
--rw-rw-rw-   0        0        0     2922 2023-02-19 16:42:40.000000 featurebox-0.0.9998/featurebox/pbs/pbs_conf.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.051813 featurebox-0.0.9998/featurebox/selection/
--rw-rw-rw-   0        0        0       68 2022-08-24 14:23:26.000000 featurebox-0.0.9998/featurebox/selection/__init__.py
--rw-rw-rw-   0        0        0    25336 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/selection/backforward.py
--rw-rw-rw-   0        0        0    10591 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/selection/corr.py
--rw-rw-rw-   0        0        0    12244 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/selection/exhaustion.py
--rw-rw-rw-   0        0        0    14579 2022-12-07 05:24:08.000000 featurebox-0.0.9998/featurebox/selection/ga.py
--rw-rw-rw-   0        0        0     5650 2022-08-24 14:25:13.000000 featurebox-0.0.9998/featurebox/selection/multibase.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:22.053819 featurebox-0.0.9998/featurebox/utils/
--rw-rw-rw-   0        0        0       48 2022-10-15 09:08:29.000000 featurebox-0.0.9998/featurebox/utils/__init__.py
--rw-rw-rw-   0        0        0       95 2022-01-04 13:19:58.000000 featurebox-0.0.9998/featurebox/utils/general.py
--rw-rw-rw-   0        0        0      221 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/utils/predefined_typing.py
--rw-rw-rw-   0        0        0    19519 2022-11-25 11:15:33.000000 featurebox-0.0.9998/featurebox/utils/quickmethod.py
-drwxrwxrwx   0        0        0        0 2023-02-26 06:38:21.990815 featurebox-0.0.9998/featurebox.egg-info/
--rw-rw-rw-   0        0        0     2553 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3047 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      146 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      130 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-26 06:38:21.000000 featurebox-0.0.9998/featurebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      245 2022-08-01 10:04:12.000000 featurebox-0.0.9998/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-26 06:38:22.055762 featurebox-0.0.9998/setup.cfg
--rw-rw-rw-   0        0        0     2534 2023-02-26 06:38:20.000000 featurebox-0.0.9998/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.031925 featurebox-0.0.9999/
+-rw-rw-rw-   0        0        0     7797 2021-12-17 11:27:06.000000 featurebox-0.0.9999/LICENSE
+-rw-rw-rw-   0        0        0      129 2021-12-17 11:27:06.000000 featurebox-0.0.9999/MANIFEST.in
+-rw-rw-rw-   0        0        0     2553 2023-04-26 13:47:46.031925 featurebox-0.0.9999/PKG-INFO
+-rw-rw-rw-   0        0        0     1372 2022-01-04 11:52:43.000000 featurebox-0.0.9999/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.961898 featurebox-0.0.9999/featurebox/
+-rw-rw-rw-   0        0        0       64 2022-08-08 06:09:08.000000 featurebox-0.0.9999/featurebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.977716 featurebox-0.0.9999/featurebox/cli/
+-rw-rw-rw-   0        0        0      747 2022-10-15 08:34:40.000000 featurebox-0.0.9999/featurebox/cli/__init__.py
+-rw-rw-rw-   0        0        0    13414 2023-02-17 07:06:06.000000 featurebox-0.0.9999/featurebox/cli/_basepathout.py
+-rw-rw-rw-   0        0        0     6745 2023-02-22 15:08:51.000000 featurebox-0.0.9999/featurebox/cli/main.py
+-rw-rw-rw-   0        0        0      320 2022-10-15 08:34:40.000000 featurebox-0.0.9999/featurebox/cli/template.py
+-rw-rw-rw-   0        0        0    10232 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_bader.py
+-rw-rw-rw-   0        0        0    11807 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_bgp.py
+-rw-rw-rw-   0        0        0      913 2022-08-06 15:06:02.000000 featurebox-0.0.9999/featurebox/cli/vasp_chg_diff.py
+-rw-rw-rw-   0        0        0    10397 2022-10-15 08:46:16.000000 featurebox-0.0.9999/featurebox/cli/vasp_cohp.py
+-rw-rw-rw-   0        0        0     5435 2023-02-21 09:35:25.000000 featurebox-0.0.9999/featurebox/cli/vasp_converge.py
+-rw-rw-rw-   0        0        0    37796 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/cli/vasp_dbc.py
+-rw-rw-rw-   0        0        0    25116 2022-08-12 08:59:00.000000 featurebox-0.0.9999/featurebox/cli/vasp_dos.py
+-rw-rw-rw-   0        0        0     4942 2023-02-17 07:12:55.000000 featurebox-0.0.9999/featurebox/cli/vasp_empty.py
+-rw-rw-rw-   0        0        0     7019 2023-02-21 09:34:22.000000 featurebox-0.0.9999/featurebox/cli/vasp_general_diff.py
+-rw-rw-rw-   0        0        0     7809 2023-02-19 16:30:44.000000 featurebox-0.0.9999/featurebox/cli/vasp_general_single.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.987716 featurebox-0.0.9999/featurebox/data/
+-rw-rw-rw-   0        0        0      167 2022-08-01 08:22:20.000000 featurebox-0.0.9999/featurebox/data/__init__.py
+-rw-rw-rw-   0        0        0     6491 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/data/check_data.py
+-rw-rw-rw-   0        0        0    10393 2022-10-15 08:47:37.000000 featurebox-0.0.9999/featurebox/data/data_sep.py
+-rw-rw-rw-   0        0        0    38626 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_megnet.json
+-rw-rw-rw-   0        0        0    37806 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_table.csv
+-rw-rw-rw-   0        0        0    47340 2021-12-27 15:28:19.000000 featurebox-0.0.9999/featurebox/data/ele_table_norm.csv
+-rw-rw-rw-   0        0        0     2917 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/data/ie.json
+-rw-rw-rw-   0        0        0     6763 2022-10-15 08:50:02.000000 featurebox-0.0.9999/featurebox/data/mp_access.py
+-rw-rw-rw-   0        0        0     8745 2023-02-19 10:31:47.000000 featurebox-0.0.9999/featurebox/data/name_split.py
+-rw-rw-rw-   0        0        0      476 2023-02-05 08:28:56.000000 featurebox-0.0.9999/featurebox/data/namesplit.py
+-rw-rw-rw-   0        0        0     7822 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/data/oe.csv
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.990716 featurebox-0.0.9999/featurebox/featurizers/
+-rw-rw-rw-   0        0        0       84 2022-10-12 08:15:47.000000 featurebox-0.0.9999/featurebox/featurizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.992716 featurebox-0.0.9999/featurebox/featurizers/atom/
+-rw-rw-rw-   0        0        0       22 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/atom/__init__.py
+-rw-rw-rw-   0        0        0    27629 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/atom/mapper.py
+-rw-rw-rw-   0        0        0    17825 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/base_feature.py
+-rw-rw-rw-   0        0        0     4086 2022-08-12 09:00:19.000000 featurebox-0.0.9999/featurebox/featurizers/batch_feature.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.997677 featurebox-0.0.9999/featurebox/featurizers/envir/
+-rw-rw-rw-   0        0        0      145 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/__init__.py
+-rw-rw-rw-   0        0        0     3078 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/featurizers/envir/_get_radius_in_spheres.py
+-rw-rw-rw-   0        0        0     6732 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/envir/_get_xyz_in_spheres.py
+-rw-rw-rw-   0        0        0     2861 2022-11-04 08:32:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/desc_env.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.010625 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/
+-rw-rw-rw-   0        0        0    46046 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/ACSF.py
+-rw-rw-rw-   0        0        0    17182 2022-12-07 05:24:08.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAD.py
+-rw-rw-rw-   0        0        0    16250 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAMD.py
+-rw-rw-rw-   0        0        0    45331 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO3.py
+-rw-rw-rw-   0        0        0    62762 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO4.py
+-rw-rw-rw-   0        0        0    33591 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SOAP.py
+-rw-rw-rw-   0        0        0      271 2022-10-12 08:15:47.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/__init__.py
+-rw-rw-rw-   0        0        0      904 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/_generate_coefs.py
+-rw-rw-rw-   0        0        0    16420 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/angular_momentum.py
+-rw-rw-rw-   0        0        0    43536 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/behlerparrinello.py
+-rw-rw-rw-   0        0        0    50664 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/bispectrum.py
+-rw-rw-rw-   0        0        0     4877 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/cutoff.py
+-rw-rw-rw-   0        0        0     9684 2022-10-15 09:17:09.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/lbispectrum.py
+-rw-rw-rw-   0        0        0      999 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/utils.py
+-rw-rw-rw-   0        0        0    34379 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/wACSF.py
+-rw-rw-rw-   0        0        0    16373 2022-11-04 08:32:06.000000 featurebox-0.0.9999/featurebox/featurizers/envir/environment.py
+-rw-rw-rw-   0        0        0     7980 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/envir/local_env.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.014369 featurebox-0.0.9999/featurebox/featurizers/state/
+-rw-rw-rw-   0        0        0       65 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/state/__init__.py
+-rw-rw-rw-   0        0        0    12441 2022-10-15 09:31:37.000000 featurebox-0.0.9999/featurebox/featurizers/state/extrastats.py
+-rw-rw-rw-   0        0        0      954 2021-12-17 11:27:06.000000 featurebox-0.0.9999/featurebox/featurizers/state/state_mapper.py
+-rw-rw-rw-   0        0        0    10989 2022-10-20 14:50:35.000000 featurebox-0.0.9999/featurebox/featurizers/state/statistics.py
+-rw-rw-rw-   0        0        0     8329 2022-03-06 10:25:09.000000 featurebox-0.0.9999/featurebox/featurizers/state/union.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.021371 featurebox-0.0.9999/featurebox/pbs/
+-rw-rw-rw-   0        0        0      157 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/__init__.py
+-rw-rw-rw-   0        0        0     3519 2023-02-10 07:49:23.000000 featurebox-0.0.9999/featurebox/pbs/cli.py
+-rw-rw-rw-   0        0        0     1683 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/jmk.py
+-rw-rw-rw-   0        0        0    10498 2023-02-19 17:25:28.000000 featurebox-0.0.9999/featurebox/pbs/job_manager.py
+-rw-rw-rw-   0        0        0     4877 2022-12-07 01:59:25.000000 featurebox-0.0.9999/featurebox/pbs/misc.py
+-rw-rw-rw-   0        0        0    12164 2023-02-22 04:00:03.000000 featurebox-0.0.9999/featurebox/pbs/misc_slurm.py
+-rw-rw-rw-   0        0        0     7827 2023-02-18 07:12:20.000000 featurebox-0.0.9999/featurebox/pbs/misc_torque.py
+-rw-rw-rw-   0        0        0     9286 2023-02-19 18:13:40.000000 featurebox-0.0.9999/featurebox/pbs/misc_unischeduler.py
+-rw-rw-rw-   0        0        0     2922 2023-02-19 16:42:40.000000 featurebox-0.0.9999/featurebox/pbs/pbs_conf.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.027371 featurebox-0.0.9999/featurebox/selection/
+-rw-rw-rw-   0        0        0       68 2022-08-24 14:23:26.000000 featurebox-0.0.9999/featurebox/selection/__init__.py
+-rw-rw-rw-   0        0        0    26778 2023-04-26 10:02:44.000000 featurebox-0.0.9999/featurebox/selection/backforward.py
+-rw-rw-rw-   0        0        0     9201 2023-04-26 10:03:21.000000 featurebox-0.0.9999/featurebox/selection/corr.py
+-rw-rw-rw-   0        0        0    12564 2023-04-26 09:52:37.000000 featurebox-0.0.9999/featurebox/selection/exhaustion.py
+-rw-rw-rw-   0        0        0    15219 2023-04-26 10:46:56.000000 featurebox-0.0.9999/featurebox/selection/ga.py
+-rw-rw-rw-   0        0        0     6230 2023-04-25 13:59:08.000000 featurebox-0.0.9999/featurebox/selection/multibase.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:46.030919 featurebox-0.0.9999/featurebox/utils/
+-rw-rw-rw-   0        0        0       48 2022-10-15 09:08:29.000000 featurebox-0.0.9999/featurebox/utils/__init__.py
+-rw-rw-rw-   0        0        0       95 2022-01-04 13:19:58.000000 featurebox-0.0.9999/featurebox/utils/general.py
+-rw-rw-rw-   0        0        0      221 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/utils/predefined_typing.py
+-rw-rw-rw-   0        0        0    19519 2022-11-25 11:15:33.000000 featurebox-0.0.9999/featurebox/utils/quickmethod.py
+drwxrwxrwx   0        0        0        0 2023-04-26 13:47:45.966716 featurebox-0.0.9999/featurebox.egg-info/
+-rw-rw-rw-   0        0        0     2553 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3047 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      146 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 13:47:45.000000 featurebox-0.0.9999/featurebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      245 2022-08-01 10:04:12.000000 featurebox-0.0.9999/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 13:47:46.031925 featurebox-0.0.9999/setup.cfg
+-rw-rw-rw-   0        0        0     2534 2023-04-26 13:47:25.000000 featurebox-0.0.9999/setup.py
```

### Comparing `featurebox-0.0.9998/LICENSE` & `featurebox-0.0.9999/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/PKG-INFO` & `featurebox-0.0.9999/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurebox
-Version: 0.0.9998
+Version: 0.0.9999
 Summary: This is an box contains tools for machine learning.Some of code are non-originality, just copy for use. All the referenced code are marked,details can be shown in their sources
 Home-page: https://github.com/boliqq07/featurebox
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
 License: UNKNOWN
 Keywords: features,combination,selection
```

### Comparing `featurebox-0.0.9998/README.md` & `featurebox-0.0.9999/README.md`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/__init__.py` & `featurebox-0.0.9999/featurebox/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/_basepathout.py` & `featurebox-0.0.9999/featurebox/cli/_basepathout.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/main.py` & `featurebox-0.0.9999/featurebox/cli/main.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_bader.py` & `featurebox-0.0.9999/featurebox/cli/vasp_bader.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_bgp.py` & `featurebox-0.0.9999/featurebox/cli/vasp_bgp.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_chg_diff.py` & `featurebox-0.0.9999/featurebox/cli/vasp_chg_diff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_cohp.py` & `featurebox-0.0.9999/featurebox/cli/vasp_cohp.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_converge.py` & `featurebox-0.0.9999/featurebox/cli/vasp_converge.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_dbc.py` & `featurebox-0.0.9999/featurebox/cli/vasp_dbc.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_dos.py` & `featurebox-0.0.9999/featurebox/cli/vasp_dos.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_empty.py` & `featurebox-0.0.9999/featurebox/cli/vasp_empty.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_general_diff.py` & `featurebox-0.0.9999/featurebox/cli/vasp_general_diff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/cli/vasp_general_single.py` & `featurebox-0.0.9999/featurebox/cli/vasp_general_single.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/check_data.py` & `featurebox-0.0.9999/featurebox/data/check_data.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/data_sep.py` & `featurebox-0.0.9999/featurebox/data/data_sep.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/ele_megnet.json` & `featurebox-0.0.9999/featurebox/data/ele_megnet.json`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/ele_table.csv` & `featurebox-0.0.9999/featurebox/data/ele_table.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/ele_table_norm.csv` & `featurebox-0.0.9999/featurebox/data/ele_table_norm.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/ie.json` & `featurebox-0.0.9999/featurebox/data/ie.json`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/mp_access.py` & `featurebox-0.0.9999/featurebox/data/mp_access.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/name_split.py` & `featurebox-0.0.9999/featurebox/data/name_split.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/data/oe.csv` & `featurebox-0.0.9999/featurebox/data/oe.csv`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/atom/mapper.py` & `featurebox-0.0.9999/featurebox/featurizers/atom/mapper.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/base_feature.py` & `featurebox-0.0.9999/featurebox/featurizers/base_feature.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/batch_feature.py` & `featurebox-0.0.9999/featurebox/featurizers/batch_feature.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/_get_radius_in_spheres.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/_get_radius_in_spheres.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/_get_xyz_in_spheres.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/_get_xyz_in_spheres.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/desc_env.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/desc_env.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/ACSF.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/ACSF.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/EAD.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAD.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/EAMD.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/EAMD.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SO3.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO3.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SO4.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SO4.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/SOAP.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/SOAP.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/_generate_coefs.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/_generate_coefs.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/angular_momentum.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/angular_momentum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/behlerparrinello.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/behlerparrinello.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/bispectrum.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/bispectrum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/cutoff.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/cutoff.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/lbispectrum.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/lbispectrum.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/utils.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/utils.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/descriptors/wACSF.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/descriptors/wACSF.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/environment.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/environment.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/envir/local_env.py` & `featurebox-0.0.9999/featurebox/featurizers/envir/local_env.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/state/extrastats.py` & `featurebox-0.0.9999/featurebox/featurizers/state/extrastats.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/state/state_mapper.py` & `featurebox-0.0.9999/featurebox/featurizers/state/state_mapper.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/state/statistics.py` & `featurebox-0.0.9999/featurebox/featurizers/state/statistics.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/featurizers/state/union.py` & `featurebox-0.0.9999/featurebox/featurizers/state/union.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/cli.py` & `featurebox-0.0.9999/featurebox/pbs/cli.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/jmk.py` & `featurebox-0.0.9999/featurebox/pbs/jmk.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/job_manager.py` & `featurebox-0.0.9999/featurebox/pbs/job_manager.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/misc.py` & `featurebox-0.0.9999/featurebox/pbs/misc.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/misc_slurm.py` & `featurebox-0.0.9999/featurebox/pbs/misc_slurm.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/misc_torque.py` & `featurebox-0.0.9999/featurebox/pbs/misc_torque.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/misc_unischeduler.py` & `featurebox-0.0.9999/featurebox/pbs/misc_unischeduler.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/pbs/pbs_conf.py` & `featurebox-0.0.9999/featurebox/pbs/pbs_conf.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox/selection/backforward.py` & `featurebox-0.0.9999/featurebox/selection/backforward.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,66 +52,77 @@
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
     >>> svr= SVR()
-    >>> bf = BackForward(svr,primary_feature=4, random_state=1)
+    >>> bf = BackForward(svr,primary_feature=4, random_state=1,verbose=0,note=False)
     >>> new_x = bf.fit_transform(X,y)
     >>> bf.support_
     array([False,  True,  True, False, False, False, False,  True])
 
     Examples
     --------
-    If ``score`` and ``predict`` is used, the ``refit`` should be set True,
-    the refit used all data in ``fit`` function, that is, it is not test score/predict.
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> from sklearn.model_selection import cross_val_score
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
+    >>> X_train,y_train,X_test,y_test = X[:50],y[:50],X[-50:],y[-50:]
+
     >>> svr= SVR()
-    >>> bf = BackForward(svr,primary_feature=4, random_state=1, refit=True,cv=5)
-    >>> bf = bf.fit(X[:50],y[:50])
+    >>> bf = BackForward(svr, primary_feature=4, random_state=1, refit=True, cv=5,verbose=0,note=False)
+    >>> bf = bf.fit(X_train,y_train)
     >>> bf.best_score_         # cv score
     -3.0552830696940037
-    >>> train_score = bf.score(X[:50],y[:50])  # train score
-    >>> test_score = bf.score(X[-50:],y[-50:]) # test score in more data.
-    >>> np.mean(cross_val_score(bf.estimator_,X[:50,bf.support_],y[:50],cv=5)) # re cv_score in manually.
+    >>> train_score = bf.score(X_train,y_train)  # train score
+    >>> test_score = bf.score(X_test,y_test) # test score in more data.
+    >>> np.mean(cross_val_score(bf.estimator_,X_train[:,bf.support_],y_train,cv=5)) # get cv_score manually.
     -3.0552830696940037
 
+    Notes
+        If ``score`` and ``predict`` is used, the ``refit`` should be set True,
+        the refit used all data in ``fit`` function, that is, it is not test score/predict.
+
     Examples
     --------
     If GridSearchCV, the refit should be set True and return the cv score.
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> from sklearn import model_selection
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
+    >>> X_train,y_train,X_test,y_test = X[:50],y[:50],X[-50:],y[-50:]
+
     >>> svr= SVR()
     >>> gd = model_selection.GridSearchCV(svr,param_grid={"C":[1,10]},n_jobs=1)  # keep n_jobs=1 there.
-    >>> bf = BackForward(gd,primary_feature=4, random_state=1, refit=True,scoring="neg_root_mean_squared_error",cv=5)
-    >>> bf = bf.fit(X[:50],y[:50])
+    >>> bf = BackForward(gd,primary_feature=4, random_state=1, refit=True,
+    ... scoring="neg_root_mean_squared_error",cv=5,verbose=0, note=False)
+    Uniform parameter in SearchCV and Exhaustion:
+    (scoring=neg_root_mean_squared_error, cv=5, refit=True)
+    >>> bf = bf.fit(X_train,y_train)
     >>> bf.best_score_         # cv score
     -0.5919173121895709
-    >>> train_score = bf.score(X[:50],y[:50])  # train score
-    >>> test_score = bf.score(X[-50:],y[-50:]) # test score in more data.
+
+    >>> train_score = bf.score(X_train,y_train)  # train score
+    >>> test_score = bf.score(X_test,y_test) # test score in more data.
+    >>> # bf.estimator_ is the gd object (GridSearchCV)
     >>> bf.estimator_.best_score_ # re cv_score in manually.
     -0.5919173121895709
     """
 
     def __init__(self, estimator: BaseEstimator, n_type_feature_to_select: int = None, primary_feature: int = None,
-                 multi_grade: int = 2, multi_index: List = None, refit=False, cv=5, min_type_feature_to_select: int = 3,
+                 multi_grade: int = 2, multi_index: List = None, refit=True, cv=5, min_type_feature_to_select: int = 3,
                  must_index: List = None, tolerant: float = 0.01, verbose: int = 1, random_state: int = None,
-                 scoring: str = None):
+                 scoring: str = None, note=True):
         """
 
         Parameters
         ----------
         estimator : estimator object
             This is assumed to implement the scikit-learn estimator interface.
             A supervised sklearn learning estimator with ``fit`` method.
@@ -133,58 +144,71 @@
             print or not.
         random_state:int
             random_state.
         refit:bool
             refit or not. if refit, the model would use all data.
         scoring:None,str
             scoring method name.
+        note:bool
+            print note or not.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         if any((hasattr(estimator, "max_features") and refit,
                 isinstance(estimator, BaseSearchCV) and hasattr(estimator.estimator, "max_features") and refit)):
-            print("For estimator with 'max_features' attribute, the 'max_features' would changed with each sub-data. \n"
-                  "Please change and define 'max_features' by manual testing after Backforward!\n")
-        if refit:
+            warnings.warn("For estimator with 'max_features' attribute, \n"
+                          "the 'max_features' would changed with each sub-data. \n"
+                          "Please change and define 'max_features' by manual testing \n"
+                          "after Backforward!\n", UserWarning)
+        if refit and note:
             if isinstance(estimator, BaseSearchCV) and estimator.refit is True:
-                warnings.warn(
-                    "\nThe self.estimator_ :{} would used all the X, y data if refit! \n"
-                    "Please be careful with the 'score' and 'predict' if use, "
-                    "which are 'train' score/predict if inputs not changed!!!\n"
-                    "Check 'self.estomator_.cv_result' to get CV result,"
-                    " such as 'self.estomator_.best_score_' for evaluation instead.".format(
-                        estimator.__class__.__name__), UserWarning)
+                print(
+f"""Note:
+    If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
+    1. Be careful with the 'score' and 'predict' functions,
+    Those are **training** score/predict if data in ``predict`` function not changed!
+    Those are **testing** score/predict if data in ``predict`` function changed!
+    2. To get CV result for evaluation:
+    self.estimator_ is the SearchCV object, check 'self.estimator_.cv_result' to get CV result.
+    Using 'self.best_score_' or 'self.estimator_.best_score_' for evaluation,
+    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
             else:
-                warnings.warn(
-                    "\nThe self.estimator_ :{} would used all the X, y data with refit! \n"
-                    "Please be careful with the 'score' and 'predict' functions."
-                    "if inputs not changed, the 'score' and 'predict' are training!!!\n"
-                    "Thus:\n"
-                    "Use 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation instead,\n"
-                    "Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plot instead."
-                    "".format(
-                        estimator.__class__.__name__), UserWarning)
+                print(
+f"""Note:
+    If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
+    1. Be careful with the 'score' and 'predict' functions:
+    Those are **training** score/predict, if data in ``predict`` function not changed!
+    Those are **testing** score/predict, if data in ``predict`` function changed!
+    2. To get CV result for evaluation:
+    Use 'self.best_score_' or 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation,
+    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
 
         assert cv >= 3
 
         if isinstance(estimator, BaseSearchCV):
-            print(f"Using scoring:{scoring},and cv:{cv}")
+            print(f"Uniform parameter in SearchCV and Exhaustion:\n"
+                  f"(scoring={scoring}, cv={cv}, refit={refit})")
             estimator.scoring = scoring
             estimator.cv = cv
+            estimator.refit = refit
+            estimator.n_jobs = 1
+
         self.scoring = scoring
         self.estimator = estimator
+        self.estimator_ = clone(self.estimator)
 
         self.n_type_feature_to_select = n_type_feature_to_select
         self.primary_feature = primary_feature
         self.verbose = verbose
         self.score_ = []
         self.random_state = random_state
         self.tolerant = tolerant
         self.refit = refit
         self.min_type_feature_to_select = min_type_feature_to_select
         self.cv = cv
+        self.note = note
         if isinstance(n_type_feature_to_select, int):
             assert n_type_feature_to_select >= min_type_feature_to_select, "Max numbers should be large than Min numbers."
 
     @property
     def _estimator_type(self):
         return self.estimator._estimator_type
 
@@ -327,25 +351,27 @@
 
         slice1, best = add_slice(slice1, slice2)
         if isinstance(self.n_type_feature_to_select, int) and len(slice1) > self.n_type_feature_to_select:
             slice1, best = sub_slice_force(slice1)
 
         slice1.sort()
         select_feature = np.array(self.feature_unfold(slice1))
-        sup = np.zeros(x.shape[1], dtype=np.bool)
-        sup[select_feature] = 1
+        sup = np.full(x.shape[1], fill_value=False, dtype=bool)
+        sup[select_feature] = True
         self.best_score_ = best
         self.support_ = sup
         self.estimator_ = clone(self.estimator)
 
         if self.refit:
             if hasattr(self.estimator, "max_features"):
                 self.estimator_.max_features = select_feature.shape[0]
             elif isinstance(self.estimator, BaseSearchCV) and hasattr(self.estimator.estimator, "max_features"):
+                self.estimator_.refit = self.refit
                 self.estimator_.estimator.max_features = select_feature.shape[0]
+
             self.estimator_.fit(x[:, select_feature], y)
         self.n_feature_ = len(select_feature)
 
         return self
 
     @if_delegate_has_method(delegate='estimator_')
     def predict(self, X):
@@ -442,15 +468,15 @@
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
     >>> svr= SVR()
-    >>> bf = BackForwardStable(svr,primary_feature=3,  random_state=1)
+    >>> bf = BackForwardStable(svr,primary_feature=3, random_state=1,verbose=0,note=False)
     >>> new_x = bf.fit_transform(X,y)
     >>> bf.support_
     array([False,  True, False, False, False,  True,  True, False])
     >>> bf.best_score_
     -0.09122826477472024
 
     If score and predict is used, the refit could be set True and make sure the data is splited, due to the refit
@@ -458,41 +484,43 @@
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
     >>> svr= SVR()
-    >>> bf = BackForwardStable(svr,primary_feature=4, random_state=1, refit=True)
+    >>> bf = BackForwardStable(svr,primary_feature=4, random_state=1, refit=True,verbose=0,note=False)
     >>> new_x = bf.fit_transform(X[:50],y[:50])
     >>> train_score = bf.score(X[50:],y[50:])
     >>> cv_score = bf.best_score_
     ...
 
     If GridSearchCV, the refit could be set True and return the cv score.
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> from sklearn import model_selection
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
     >>> svr= SVR()
-    >>> gd = model_selection.GridSearchCV(svr,param_grid={"C":[1,10]},n_jobs=1,cv=5)
-    >>> bf = BackForward(gd,primary_feature=4, random_state=1, refit=True)
+    >>> gd = model_selection.GridSearchCV(svr,param_grid={"C":[1,10]})
+    >>> bf = BackForward(gd,primary_feature=4, random_state=1, refit=True, cv=5,verbose=0,note=False)
+    Uniform parameter in SearchCV and Exhaustion:
+    (scoring=None, cv=5, refit=True)
     >>> new_x = bf.fit_transform(X,y)
     ...
     """
 
     def __init__(self, estimator: BaseEstimator, n_type_feature_to_select: int = None,
                  min_type_feature_to_select: int = 3,
                  primary_feature: int = None, multi_grade: int = 2, multi_index: List = None,
                  must_index: List = None, verbose: int = 0, random_state: int = None,
                  tolerant: float = 0.001, cv: int = 5,
-                 times: int = 5, scoring: str = None, n_jobs: int = None, refit=False):
+                 times: int = 5, scoring: str = None, n_jobs: int = None, refit=False, note=True):
         """
 
         Parameters
         ----------
         estimator : estimator object
             This is assumed to implement the scikit-learn estimator interface.
             A supervised sklearn learning estimator with ``fit`` method.
@@ -517,14 +545,16 @@
         refit:bool
             refit or not. if refit, the model would use all data.
         n_jobs : int or None
             Number of cores to run in parallel while fitting across folds.
             ``None`` means 1 and ``-1`` means using all processors.
         scoring: None,str
             scoring method.
+        note:bool
+            print note or not.
 
         """
         if isinstance(estimator, BaseSearchCV):
             warnings.warn("The 'estimator' of BackForwardStable not suggested BaseSearchCV, "
                           "because the BackForwardStable is one BaseSearchCV itself.")
 
         self.estimator = estimator
@@ -539,14 +569,16 @@
         self.multi_index = multi_index
         self.must_index = must_index
         self.score_ = []
         self.random_state = random_state
         self.refit = refit
         self.tolerant = tolerant
         self.cv = cv
+        self.note = note
+
 
     def fit(self, X, y, groups=None):
         """Fit the baf model and automatically tune the number of selected feature.
 
         Parameters
         ----------
         X : {array-like, sparse matrix}, shape = [n_samples, n_feature]
@@ -559,24 +591,25 @@
 
         groups : array-like, shape = [n_samples], optional
             cal_group labels for the samples used while splitting the dataset into
             train/test set.
         """
         X, y = check_X_y(X, y, "csr")
         # Initialization
-        estimator = clone(self.estimator)
-        scorer = check_scoring(estimator, scoring=self.scoring)
+        scorer = check_scoring(self.estimator, scoring=self.scoring)
         ran = check_random_state(self.random_state)
 
-        baf = BackForward(estimator=estimator,
+        baf = BackForward(estimator=self.estimator,
                           n_type_feature_to_select=self.n_type_feature_to_select,
                           min_type_feature_to_select=self.min_type_feature_to_select,
                           verbose=self.verbose, primary_feature=self.primary_feature,
                           multi_grade=self.multi_grade, multi_index=self.multi_index, cv=self.cv,
-                          must_index=self.must_index, random_state=ran, tolerant=self.tolerant)
+                          must_index=self.must_index, random_state=ran, tolerant=self.tolerant,
+                          note=self.note
+                          )
         rans = ran.randint(0, 1000, self.times)
 
         func = partial(_multi_time_fit, baf=baf, X=X, y=y, scorer=scorer)
 
         scores = parallelize(n_jobs=self.n_jobs, func=func, iterable=rans, respective=False)
 
         support, scores, score_step = zip(*scores)
@@ -585,14 +618,15 @@
         # Re-execute an elimination with best_k over the whole set
 
         # Set final attributes
         self.support_step = score_step
         self.support_ = best_support
         self.best_score_ = best_score
         self.estimator_ = clone(self.estimator)
+
         if self.refit:
             if hasattr(self.estimator_, "max_features"):
                 self.estimator_.max_features = np.sum(self.support_)
             self.estimator_.fit(X[:, self.support_], y)
         self.n_feature_ = np.count_nonzero(support)
         return self
 
@@ -611,25 +645,27 @@
         y : array of shape [n_samples]
             The predicted target values.
         """
         check_is_fitted(self, 'estimator_')
         return self.estimator_.predict(self.transform(X))
 
     @if_delegate_has_method(delegate='estimator_')
-    def score(self, X, y):
+    def score(self, X, y, scoring=None):
         """Reduce X to the selected feature and then return the score of the underlying estimator, only with refit.
         Only available ``refit=True``.
 
         Parameters
         ----------
         X : array of shape [n_samples, n_feature]
             The input0 samples.
 
         y : array of shape [n_samples]
             The target values.
         """
         check_is_fitted(self, 'estimator_')
-        return self.estimator_.score(self.transform(X), y)
+        scoring = scoring if scoring is not None else self.scoring
+        scorer = check_scoring(self.estimator_, scoring=scoring, allow_none=False)
+        return scorer(self.estimator_, self.transform(X), y)
 
     def _get_support_mask(self):
         check_is_fitted(self, 'support_')
         return self.support_
```

### Comparing `featurebox-0.0.9998/featurebox/selection/corr.py` & `featurebox-0.0.9999/featurebox/selection/corr.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @Software: PyCharm
 # @License: BSD 3-Clause
 
 """
 Calculate the correction of columns.
 """
 import copy
+import warnings
 from typing import List
 
 import numpy as np
 from mgetool.tool import name_to_name
 from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.feature_selection import SelectorMixin
 from sklearn.utils import check_random_state
@@ -22,25 +23,28 @@
 from featurebox.selection.multibase import MultiBase
 
 
 class Corr(BaseEstimator, MetaEstimatorMixin, SelectorMixin, MultiBase):
     """
     Calculate correlation. (Where the result are changed with random state.)
 
+    **1. Used for filter automatically by machine**
+
     Examples
     ---------
     >>> from sklearn.datasets import fetch_california_housing
     >>> from featurebox.selection.corr import Corr
     >>> x, y = fetch_california_housing(return_X_y=True)
     >>> x = x[:100]
     >>> y = y[:100]
     >>> co = Corr(threshold=0.5)
-    >>> nx = co.fit_transform(x)
+    >>> new_x = co.fit_transform(x)
+    >>> select_feature = co.support_
 
-    **1. Used for get group exceeding the threshold**
+    **1. Used for get group exceeding the threshold by setp**
 
     Examples
     ---------
 
     >>> from sklearn.datasets import fetch_california_housing
     >>> from featurebox.selection.corr import Corr
     >>> x, y = fetch_california_housing(return_X_y=True)
@@ -48,59 +52,38 @@
     >>> y = y[:100]
     >>> co = Corr(threshold=0.5)
     >>> groups = co.count_cof(np.corrcoef(x[:,:7], rowvar=False))
     >>> groups[1]
     [[0, 6], [1], [2], [3], [4], [5], [0, 6]]
     >>> groups[0]
     [[1.0, 0.554], [1.0], [1.0], [1.0], [1.0], [1.0], [0.554, 1.0]]
-
-    Where the (0,6) are with correlation more than 0.7.
-
-    **2. Used for filter automatically by machine**
-
-    Examples
-    -----------
-    >>> from sklearn.datasets import fetch_california_housing
-    >>> from featurebox.selection.corr import Corr
-    >>> x, y = fetch_california_housing(return_X_y=True)
-    >>> x = x[:100]
-    >>> y = y[:100]
-    >>> co = Corr(threshold=0.5)
-    >>> co.fit(x)
-    Corr(threshold=0.5)
-    >>> group = co.count_cof()
-    >>> group[1]
-    [[0, 6, 7], [1], [2], [3], [4], [5], [0, 6, 7], [0, 6, 7]]
-    >>> co.remove_coef(group[1]) # Filter automatically by machine.
+    >>> co.remove_coef(groups[1]) # Filter automatically by machine.
     [0, 1, 2, 3, 4, 5]
 
     Where the remove_coef are changed with random state.
 
+    Where the (0,6) are with correlation more than 0.7.
+
     **3. Used for binding correlation**
 
     Examples
     -----------
     >>> from sklearn.datasets import fetch_california_housing
     >>> from featurebox.selection.corr import Corr
     >>> x, y = fetch_california_housing(return_X_y=True)
     >>> x = x[:100]
     >>> y = y[:100]
     >>> co = Corr(threshold=0.3,multi_index=[0,8],multi_grade=2)
     >>> # in range [0,8], the features are binding in to 2 sized: [[0,1],[2,3],[4,5],[6,7]]
     >>> co.fit(x)
-    Corr(multi_index=[0, 8], threshold=0.3)
-    >>> group = co.count_cof()
-    >>> group[1]
-    [[0, 1, 3], [0, 1, 3], [2], [0, 1, 3]]
-    >>> co.remove_coef(group[1]) # Filter automatically by machine.
-    [0, 2]
+    Corr(multi_index=(0, 8), threshold=0.3)
     """
 
-    def __init__(self, threshold: float = 0.85, multi_grade: int = 2, multi_index: List = None, must_index: List = None,
-                 random_state: int = 0):
+    def __init__(self, threshold: float = 0.85, multi_grade: int = 2, multi_index: List = None,
+                 must_index: List = None, random_state: int = 0):
         """
 
         Parameters
         ----------
         threshold:float
             ranking threshold.
         multi_grade:
@@ -117,39 +100,39 @@
         self.cov = None
         self.cov_shrink = None
         self.shrink_list = []
         self.random_state = random_state
         self.nan_index_mark = None
 
     def fit(self, data, pre_cal=None, method="mean"):
+        assert method in ["mean" or "max"]
         if pre_cal is None:
-
-            cov = np.corrcoef(data, rowvar=False, )
+            cov = np.corrcoef(data, rowvar=False)
 
         elif isinstance(pre_cal, np.ndarray) and pre_cal.shape[0] == data.shape[1]:
             cov = pre_cal
         else:
             raise TypeError("pre_cal is None or coef of data_cluster with shape(data_cluster[0],data_cluster[0])")
 
         # for nan
         self.nan_index_mark = ~np.array([np.all(np.isnan(cov[i])) for i in range(cov.shape[0])])
         if not np.all(self.nan_index_mark):
-            print("There are some NAN values in correlation coefficient matrix, which could be constant features.\n"
-                  "The NAN features would removed later. See more in 'nan_index_mark' attribute.")
+            warnings.warn("There are some NAN values in correlation coefficient matrix, which could be constant features.\n"
+                  "The NAN features would removed later. See more in 'nan_index_mark' attribute.",UserWarning)
 
         cov = np.nan_to_num(cov)
         self.cov = cov
         self.data = data
         self.shrink_list = list(range(self.cov.shape[0]))
         self._shrink_coef(method=method)
         self.filter()
         return self
 
-    def _shrink_coef(self, method="mean" or "max"):
-
+    def _shrink_coef(self, method="mean"):
+        assert method in ["mean" or "max"]
         if self.check_multi:
             self.shrink_list = list(range(self.cov.shape[0]))
             self.shrink_list = list(self.feature_fold(self.shrink_list))
 
             cov = self.cov
             single = tuple([i for i in self.shrink_list if i not in self.multi_index])
             multi = tuple([i for i in self.shrink_list if i in self.multi_index])
@@ -259,39 +242,14 @@
         fea_all = sorted(list(set(fea_all)))
         return fea_all
 
     def _get_support_mask(self):
         check_is_fitted(self, 'support_')
         return self.support_
 
-    def inverse_transform_index(self, index):
-        """inverse the selected index to origin index by support."""
-        if isinstance(index, np.ndarray) and index.dtype == np.bool_:
-            index = np.where(index)[0]
-        index = np.array(list(index))
-
-        return np.where(self.support_)[0][index]
-
-    def transform_index(self, index):
-        """Get support index."""
-        if isinstance(index, np.ndarray) and index.dtype == np.bool_:
-            index = np.where(index)[0]
-
-        return np.array([i for i in index if self.support_[i]])
-
-    def transform(self, data):
-        if isinstance(data, (list, tuple)):
-            return data[self.support_]
-        elif isinstance(data, np.ndarray) and data.ndim == 1:
-            return data[self.support_]
-        elif isinstance(data, np.ndarray) and data.ndim == 2:
-            return data[:, self.support_]
-        else:
-            pass
-
 #
 # if __name__ == "__main__":
 #     # x, y = fetch_california_housing(return_X_y=True)
 #     # co = Corr(threshold=0.7)
 #     # c = co.count_cof(np.corrcoef(x, rowvar=False))[1]
 #     from sklearn.datasets import fetch_california_housing
 #
```

### Comparing `featurebox-0.0.9998/featurebox/selection/exhaustion.py` & `featurebox-0.0.9999/featurebox/selection/exhaustion.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,49 +43,57 @@
 
     best_score_: float
         Best score of best model of best features.
 
     Examples
     ----------
     >>> from sklearn.datasets import fetch_california_housing
+    >>> from sklearn.model_selection import cross_val_predict
     >>> from sklearn.svm import SVR
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
-    >>> svr= SVR()
-    >>> bf = Exhaustion(svr,n_select=(2,),refit=True)
+    >>> X_train,y_train,X_test,y_test = X[:50],y[:50],X[-50:],y[-50:]
+
+    >>> svr = SVR()
+    >>> bf = Exhaustion(svr,n_select=(2,),refit=True,note=False)
     >>> new_x = bf.fit_transform(X,y)
     >>> bf.support_
     array([False, False, False,  True, False,  True, False, False])
-    >>> train_score = bf.score(X[:50],y[:50])  # train score
-    >>> test_score = bf.score(X[-50:],y[-50:]) # test score in more data.
-    >>> np.mean(cross_val_score(bf.estimator_,X[:50,bf.support_],y[:50],cv=5)) # re cv_score in manually.
-    >>> np.mean(cross_val_predict(bf.estimator_,X[:50,bf.support_],y[:50],cv=5)) # re cv_predict for plot.
+    >>> train_score = bf.score(X_train,y_train)  # train score
+    >>> test_score = bf.score(X_test,y_test) # test score in more data.
+    >>> np.mean(cross_val_score(bf.estimator_,X_train[:,bf.support_],y_train,cv=5)) # re cv_score in manually.
+    -2.888471220974372
+    >>> np.mean(cross_val_predict(bf.estimator_,X_train[:,bf.support_],y_train,cv=5)) # re cv_predict for plot.
+    1.6001222987265382
 
     Examples
     ----------
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
+    >>> from sklearn import model_selection
     >>> X,y = fetch_california_housing(return_X_y=True)
     >>> X = X[:100]
     >>> y = y[:100]
     >>> svr= SVR()
-    >>> from sklearn import model_selection
-    >>> gd = model_selection.GridSearchCV(svr, param_grid=[{"C": [1, 10]}], n_jobs=1, cv=5)
-    >>> bf = Exhaustion(gd,n_select=(2,),refit=True)
+
+    >>> gd = model_selection.GridSearchCV(svr, param_grid=[{"C": [1, 10]}], n_jobs=1, cv=3)
+    >>> bf = Exhaustion(gd,n_select=(2,),refit=True,note=False,cv=5)
+    Uniform parameter in SearchCV and Exhaustion:
+    (scoring=None, cv=5, refit=True)
     >>> new_x = bf.fit_transform(X,y)
     >>> bf.support_
     array([False, False, False,  True, False,  True, False, False])
     >>> bf.best_score_
     -0.7336740728050252
     """
 
-    def __init__(self, estimator: BaseEstimator, n_select: Tuple = (2, 3, 4), multi_grade: int = None,
-                 multi_index: List = None, must_index: List = None, n_jobs: int = 1,
-                 refit: bool = False, cv: int = 5, scoring: str = None):
+    def __init__(self, estimator: BaseEstimator, n_select: Tuple = (2, 3, 4),
+                 multi_grade: int = None, multi_index: List = None, must_index: List = None,
+                 n_jobs: int = 1, refit: bool = False, cv: int = 5, scoring: str = None, note=True):
         """
 
         Parameters
         ----------
         estimator:
             sklearn model or GridSearchCV.
         n_select:tuple
@@ -100,58 +108,61 @@
             n_jobs.
         refit:bool
             refit or not, if refit the model would use all data.
         cv:bool
             if estimator is sklearn model, used cv, else pass.
         scoring:None,str
             scoring method name.
+        note:bool
+            print note or not.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         if any((hasattr(estimator, "max_features") and refit,
                 isinstance(estimator, BaseSearchCV) and hasattr(estimator.estimator, "max_features") and refit)):
-            print("For estimator with 'max_features' attribute, the 'max_features' would changed with each sub-data. \n"
-                  "Please change and define 'max_features' by SearchCV testing after Exhaustion.\n")
-        if isinstance(estimator, BaseSearchCV) and isinstance(estimator.n_jobs, int) and estimator.n_jobs > 1:
-            print(f"The 'n_jobs' for SearchCV should keep 1 or None and please pass the 'n_jobs' to {self.__class__}"
-                  f" for parallelization!")
-        if refit:
+            warnings.warn("For estimator with 'max_features' attribute, the 'max_features' would changed with each sub-data. \n"
+                  "Please change and define 'max_features' by SearchCV testing after Exhaustion.\n",UserWarning)
+
+        if refit and note:
             if isinstance(estimator, BaseSearchCV) and estimator.refit is True:
-                warnings.warn(
-                    "\nThe self.estimator_ :{} would used all the X, y data if refit! \n"
-                    "Please be careful with the 'score' and 'predict' if use, "
-                    "which are 'train' score/predict if inputs not changed!!!\n"
-                    "Check 'self.estomator_.cv_result' to get CV result,"
-                    " such as 'self.estomator_.best_score_' for evaluation instead.".format(
-                        estimator.__class__.__name__), UserWarning)
+                print(
+f"""Note:
+    If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
+    1. Be careful with the 'score' and 'predict' functions,
+    Those are **training** score/predict if data in ``predict`` function not changed!
+    Those are **testing** score/predict if data in ``predict`` function changed!
+    2. To get CV result for evaluation:
+    self.estimator_ is the SearchCV object, check 'self.estimator_.cv_result' to get CV result.
+    Using 'self.best_score_' or 'self.estimator_.best_score_' for evaluation,
+    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
             else:
-                warnings.warn(
-                    "\nThe self.estimator_ :{} would used all the X, y data with refit! \n"
-                    "Please be careful with the 'score' and 'predict' functions."
-                    "if inputs not changed, the 'score' and 'predict' are training!!!\n"
-                    "Thus:\n"
-                    "Use 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation instead,\n"
-                    "Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plot instead."
-                    "".format(
-                        estimator.__class__.__name__), UserWarning)
+                print(
+f"""Note:
+    If refit, the self.estimator_ :{estimator.__class__.__name__} would use all the data in ``fit`` function,
+    1. Be careful with the 'score' and 'predict' functions:
+    Those are **training** score/predict, if data in ``predict`` function not changed!
+    Those are **testing** score/predict, if data in ``predict`` function changed!
+    2. To get CV result for evaluation:
+    Use 'self.best_score_' or 'cross_val_score(self.estimator_,X[:, self.support_],y)' for evaluation,
+    Use 'cross_val_predict(self.estimator_,X[:, self.support_],y)' for plotting.""")
 
         if cv <= 1:
             warnings.warn(
                 "\nThe cv <= 1, the exhaustion would not use cross validate, and treat all data as train data, \n"
-                "the scoring would use the estimator.score function, rather than the 'scoring'."
                 "cv<=1 is just used for debug!!!".format(
                     estimator.__class__.__name__), UserWarning)
-            scoring = None
 
         if isinstance(estimator, BaseSearchCV):
-            print(f"Using scoring:{scoring},and cv:{cv}")
+            print(f"Uniform parameter in SearchCV and Exhaustion:\n"
+                  f"(scoring={scoring}, cv={cv}, refit={refit})")
             estimator.scoring = scoring
             estimator.cv = cv
+            estimator.n_jobs = 1
+            estimator.refit = refit
 
         self.scoring = scoring
-
         self.estimator = estimator
         self.score_ = []
         self.n_jobs = n_jobs
         self.n_select = [n_select, ] if isinstance(n_select, int) else n_select
         self.refit = refit
         self.cv = cv
 
@@ -221,25 +232,26 @@
         [i.sort() for i in slice_all]
 
         scores = parallelize(n_jobs=self.n_jobs, func=score, iterable=slice_all)
 
         feature_combination = slice_all
         index = np.argmax(scores)
         select_feature = np.array(feature_combination[int(index)])
-        su = np.zeros(x.shape[1], dtype=np.bool)
+        su = np.zeros(x.shape[1], dtype=bool)
         su[select_feature] = 1
         self.best_score_ = max(scores)
         self.score_ = scores
         self.support_ = su
         self.estimator_ = clone(self.estimator)
 
         if self.refit:
             if hasattr(self.estimator, "max_features"):
                 self.estimator_.max_features = select_feature.shape[0]
             elif isinstance(self.estimator, BaseSearchCV) and hasattr(self.estimator.estimator, "max_features"):
+                self.estimator_.refit = self.refit
                 self.estimator_.estimator.max_features = select_feature.shape[0]
             self.estimator_.fit(x[:, select_feature], y)
         self.n_feature_ = len(select_feature)
         self.score_ex = list(zip(feature_combination, scores))
         self.scatter = list(zip([len(i) for i in slice_all], scores))
         self.score_ex.sort(key=lambda _: _[1], reverse=True)
```

### Comparing `featurebox-0.0.9998/featurebox/selection/ga.py` & `featurebox-0.0.9999/featurebox/selection/ga.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from deap import tools
 from deap.algorithms import varAnd
 from deap.tools import mutShuffleIndexes
 from mgetool.newclass import create
 from mgetool.tool import check_random_state, parallelize
 from sklearn.base import BaseEstimator, MetaEstimatorMixin
 from sklearn.feature_selection import SelectorMixin
-from sklearn.metrics import r2_score
+from sklearn.metrics import r2_score, check_scoring
 from sklearn.model_selection import cross_val_score
 from sklearn.model_selection._search import BaseSearchCV
 from sklearn.utils.validation import check_is_fitted
 
 from featurebox.selection.multibase import MultiBase
 
 
@@ -142,23 +142,30 @@
     GA with binding. Please just passing training data.
 
     Examples
     ---------
     >>> from sklearn.datasets import fetch_california_housing
     >>> from sklearn.svm import SVR
     >>> data = fetch_california_housing()
-    >>> x = data.data[:50]
-    >>> y = data.target[:50]
+    >>> X = data.data
+    >>> y = data.target
+    >>> X_train,y_train,X_test,y_test = X[:50],y[:50],X[-50:],y[-50:]
     >>> svr = SVR(gamma="scale", C=100)
-    >>> ga = GA(estimator=svr, n_jobs=2, pop_n=50, hof_n=1, cxpb=0.8, mutpb=0.4, ngen=3, max_or_min="max", mut_indpb=0.1, min_=2, multi_index=[0, 5],random_state=0)
-    >>> ga.fit(x_rain, y_train)
-
-    Then
-
-    >>> ga.score(x_test, y_test)
+    >>> ga = GA(estimator=svr, n_jobs=2, pop_n=50, hof_n=1, cxpb=0.8, mutpb=0.4, ngen=3,
+    ... max_or_min="max", mut_indpb=0.1, min_=2, multi_index=[0, 5],random_state=0)
+    >>> ga.fit(X_train, y_train)
+    gen	nevals	min    	max
+    1  	50    	-4.9231	-1.09124
+    2  	43    	-3.83152  -1.09124
+    3  	46    	-4.9231   -1.09124
+    [1, 1, 1, 1, 0, 0, 1, 0] (-1.039237326973499,)
+    GA(cxpb=0.8, estimator=SVR(C=100), multi_index=(0, 5), mut_indpb=0.1, mutpb=0.4,
+       ngen=3, pop_n=50, random_state=0)
+    >>> ga.score(X_test, y_test)
+    -28.542309712899435
 
     """
 
     def __init__(self, estimator, n_jobs=2, pop_n=1000, hof_n=1, cxpb=0.6, mutpb=0.3, ngen=40, max_or_min="max",
                  mut_indpb=0.05, max_=None, min_=2, random_state=None, multi_grade=2, multi_index=None, must_index=None,
                  cv: int = 5, scoring=None):
         """
@@ -199,15 +206,17 @@
             if estimator is sklearn model, used cv, else pass.
         """
         super().__init__(multi_grade=multi_grade, multi_index=multi_index, must_index=must_index)
         assert cv >= 3
         if isinstance(estimator, BaseSearchCV):
             print(f"Using scoring:{scoring},and cv:{cv}")
             estimator.scoring = scoring
-            self.cv = cv
+            estimator.cv = cv
+            estimator.n_jobs = 1
+
         self.scoring = scoring
         self.estimator = estimator
         self.n_jobs = n_jobs
         self.pop_n = pop_n
         self.hof_n = hof_n
         self.cxpb = cxpb
         self.mutpb = mutpb
@@ -217,15 +226,15 @@
         self.min_ = min_
         self.max_or_min = max_or_min
         self.random_state = random_state
         self.cv = cv
 
         check_random_state(random_state)
         random.seed(random_state)
-        np.random.seed(0)
+        np.random.seed(random_state)
 
         self.toolbox = base.Toolbox()
         if max_or_min == "max":
             FitnessMax = create("FitnessMax", base.Fitness, weights=(1.0,))
         else:
             FitnessMax = create("FitnessMax", base.Fitness, weights=(-1.0,))
         self.Individual = create("Individual", list, fitness=FitnessMax)
@@ -279,16 +288,16 @@
         stats = tools.Statistics(lambda ind: ind.fitness.values)
         stats.register("min", np.min)
         stats.register("max", np.max)
 
         pop = toolbox.population(n=self.pop_n)
         self.hof = tools.HallOfFame(self.hof_n)
 
-        eaSimple(pop, self.toolbox, cxpb=self.cxpb, mutpb=self.mutpb, ngen=self.ngen, n_jobs=self.n_jobs,
-                 stats=stats, halloffame=self.hof, verbose=True)
+        eaSimple(pop, self.toolbox, cxpb=self.cxpb, mutpb=self.mutpb, ngen=self.ngen,
+                 n_jobs=self.n_jobs, stats=stats, halloffame=self.hof, verbose=True)
         for i in self.hof.items:
             print(self.unfold(i), i.fitness)
         support_ = self.unfold(self.hof.items[0])
         self.support_ = np.array(support_) > 0
         return self
 
     def unfold(self, ind):
@@ -317,23 +326,22 @@
                 return sc,
         else:
             if return_model:
                 return 0, None
             else:
                 return 0,
 
-    def socre_func(self, ind, model, x, y):
+    def socre_func(self, ind, model, x, y, scoring=None):
         sss = self.unfold(ind)
         index = np.where(np.array(sss) == 1)[0]
         x = x[:, index]
+        scoring = scoring if scoring is not None else self.scoring
+        scorer = check_scoring(model, scoring=scoring, allow_none=False)
         if x.shape[1] > 1:
-            svr = model
-            y2 = svr.predict(x)
-            sc = r2_score(y, y2)
-            return sc
+            return scorer(model, x, y)
         else:
             raise TypeError("only one feature, error")
 
     def predict_func(self, ind, model, x):
         sss = self.unfold(ind)
         index = np.where(np.array(sss) == 1)[0]
         x = x[:, index]
@@ -356,15 +364,16 @@
         X : array of shape [n_samples, n_feature]
             The input0 samples.
 
         y : array of shape [n_samples]
             The target values.
         """
 
-        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y, return_model=True)[1]
+        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y,
+                                return_model=True)[1]
         score = self.fitness_func(self.hof.items[0], mod, X, y, return_model=False)
         return score
 
     def score(self, X, y):
         """Reduce X to the selected feature and then return the score of the underlying estimator.
 
         Parameters
@@ -372,27 +381,29 @@
         X : array of shape [n_samples, n_feature]
             The input0 samples.
 
         y : array of shape [n_samples]
             The target values.
         """
 
-        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y, return_model=True)[1]
+        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y,
+                                return_model=True)[1]
         score = self.socre_func(self.hof.items[0], mod, X, y)
         return score
 
     def predict(self, X):
         """Reduce X to the selected feature and then return the score of the underlying estimator.
 
         Parameters
         ----------
         X : array of shape [n_samples, n_feature]
             The input0 samples.
         """
-        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y, return_model=True)[1]
+        mod = self.fitness_func(self.hof.items[0], self.estimator, self.X, self.y,
+                                return_model=True)[1]
         score = self.predict_func(self.hof.items[0], mod, X)
         return score
 
 # if __name__ == "__main__":
 #     from sklearn.svm import SVR
 #     from sklearn.datasets import fetch_california_housing
 #     data = fetch_california_housing()
```

### Comparing `featurebox-0.0.9998/featurebox/selection/multibase.py` & `featurebox-0.0.9999/featurebox/selection/multibase.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,50 +2,51 @@
 
 # @Time   : 2019/5/26 0:47
 # @Author : Administrator
 # @Project : feature_preparation
 # @FileName: multibase.py
 # @Software: PyCharm
 import itertools
-from typing import List
+from typing import List, Optional, Tuple, Sequence, Any, Union
 
 import numpy as np
 
 
 class MultiBase(object):
     """Base method for binding"""
 
-    def __init__(self, multi_grade: int = 2, multi_index: List = None, must_index: List = None):
+    def __init__(self, multi_grade: int = 2, multi_index: Optional[Union[List, Tuple]] = None,
+                 must_index: Optional[Union[List, Tuple]] = None):
         """
 
         Parameters
         ----------
-        multi_grade:
+        multi_grade: int
             binding_group size, calculate the correction between binding
-        multi_index:list
+        multi_index: list,tuple,None
             the range of multi_grade:[min,max)
-        must_index:list,None
+        must_index: list,tuple,None
             the columns force to index
         """
         self.multi_grade = multi_grade
-        self.multi_index = multi_index
-        self.must_index = must_index
+        self.multi_index = tuple(multi_index) if multi_index is not None else multi_index
+        self.must_index = tuple(must_index) if must_index is not None else must_index
 
     @property
     def check_multi(self):
         multi_index = self.multi_index
         if multi_index is None:
             return False
         elif isinstance(multi_index, (list, tuple)):
             if len(multi_index) == 2 and isinstance(multi_index[0], int) and isinstance(multi_index[1], int):
                 return True
             else:
-                raise TypeError("multi_index should be None or iterable type with 2 number")
+                raise TypeError("multi_index should be None or iterable type with 2 number.")
         else:
-            raise TypeError("multi_index should be None or iterable type with 2 number")
+            raise TypeError("multi_index should be None or iterable type with 2 number.")
 
     @property
     def check_must(self):
         must_index = self.must_index
         if must_index is None:
             return False
         elif isinstance(must_index, (list, tuple)):
@@ -88,62 +89,82 @@
             else:
                 return list(must_index)
         else:
             return []
 
     def _feature_fold(self, feature, raw=False):
         multi_grade, multi_index = self.multi_grade, self.multi_index
+        feature = list(feature)
         if self.check_multi:
-            feature = np.sort(feature)
-            single = np.array([_ for _ in feature if _ < multi_index[0] or _ >= multi_index[1]])
-            com_com = np.array([_ for _ in feature if multi_index[1] > _ >= multi_index[0]])
+            feature.sort()
+            single = [_ for _ in feature if _ < multi_index[0] or _ >= multi_index[1]]
+            com_com = [_ for _ in feature if multi_index[1] > _ >= multi_index[0]]
             com_sin = com_com[::multi_grade]
-            res = np.hstack((single, com_sin))
+            single.extend(com_sin)
+            res = single
         else:
-            res = np.array(feature)
+            res = feature
+
         if not raw:
-            return np.sort(res).astype(int)
-        else:
-            return res.astype(int)
+            res.sort()
+
+        return res
 
     def feature_fold(self, feature):
-        fea2 = list(self._feature_fold(feature, raw=True))
+        fea2 = list(self._feature_fold(feature))
         add = self.must_fold_add
         fea2.extend(add)
-        return np.array(list(set(fea2)))
+        fea2 = list(set(fea2))
+        fea2.sort()
+        return np.array(fea2)
 
     def _feature_unfold(self, feature, raw=False):
         multi_grade, multi_index = self.multi_grade, self.multi_index
+        feature = list(feature)
         if self.check_multi:
-            single = np.array([_ for _ in feature if _ < multi_index[0] or _ >= multi_index[1]])
-            com_sin = np.array([_ for _ in feature if multi_index[1] > _ >= multi_index[0]])
+            single = [_ for _ in feature if _ < multi_index[0] or _ >= multi_index[1]]
+            com_sin = [_ for _ in feature if multi_index[1] > _ >= multi_index[0]]
             com_com = list(com_sin)
             while multi_grade - 1:
-                com_com.extend(com_sin + (multi_grade - 1))
                 multi_grade -= 1
-            res = np.array(list(set(np.hstack((single, np.array(com_com))))))
+                com_com.extend([i + multi_grade for i in com_sin])
+            single.extend(com_com)
+            res = list(set(single))
         else:
-            res = np.array(feature)
+            res = feature
+
         if not raw:
-            return np.sort(res).astype(int)
-        else:
-            return res.astype(int)
+            res.sort()
+
+        return res
 
     def feature_unfold(self, feature):
-        fea2 = list(self._feature_unfold(feature, raw=True))
+        fea2 = list(self._feature_unfold(feature))
         add = self.must_unfold_add
         fea2.extend(add)
-        return np.array(list(set(fea2)))
+        fea2 = list(set(fea2))
+        fea2.sort()
+        return np.array(fea2)
 
     def inverse_transform_index(self, index):
         """inverse the selected index to origin index by support."""
         if isinstance(index, np.ndarray) and index.dtype == np.bool_:
             index = np.where(index)[0]
         index = np.array(list(index))
 
         return np.where(self.support_)[0][index]
 
     def transform_index(self, index):
         """Get support index."""
         if isinstance(index, np.ndarray) and index.dtype == np.bool_:
             index = np.where(index)[0]
         return np.array([i for i in index if self.support_[i]])
+
+    def transform(self, data: Any):
+        if isinstance(data, np.ndarray) and data.ndim == 1:
+            return data[self.support_]
+        elif isinstance(data, np.ndarray) and data.ndim == 2:
+            return data[:, self.support_]
+        elif isinstance(data, Sequence):
+            return data[self.support_]
+        else:
+            raise ValueError
```

### Comparing `featurebox-0.0.9998/featurebox/utils/quickmethod.py` & `featurebox-0.0.9999/featurebox/utils/quickmethod.py`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/featurebox.egg-info/PKG-INFO` & `featurebox-0.0.9999/featurebox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurebox
-Version: 0.0.9998
+Version: 0.0.9999
 Summary: This is an box contains tools for machine learning.Some of code are non-originality, just copy for use. All the referenced code are marked,details can be shown in their sources
 Home-page: https://github.com/boliqq07/featurebox
 Author: wangchangxin
 Author-email: 986798607@qq.com
 Maintainer: wangchangxin
 License: UNKNOWN
 Keywords: features,combination,selection
```

### Comparing `featurebox-0.0.9998/featurebox.egg-info/SOURCES.txt` & `featurebox-0.0.9999/featurebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featurebox-0.0.9998/setup.py` & `featurebox-0.0.9999/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='featurebox',
-    version='0.0.9998',
+    version='0.0.9999',
     keywords=['features', "combination", "selection"],
     description='This is an box contains tools for machine learning.'
                 'Some of code are non-originality, just copy for use. All the referenced code are marked,'
                 'details can be shown in their sources',
     install_requires=['path', 'pandas', 'numpy', 'sympy', 'scipy', 'scikit-learn', 'joblib', 'matplotlib',
                       'deprecated',
                       'requests', 'tqdm', 'six', "pymatgen", "deap", "numba", "ase", "mgetool>=0.0.62"],
```

