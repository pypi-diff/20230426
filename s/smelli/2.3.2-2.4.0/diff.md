# Comparing `tmp/smelli-2.3.2.tar.gz` & `tmp/smelli-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smelli-2.3.2.tar", last modified: Fri Oct  1 16:48:47 2021, max compression
+gzip compressed data, was "smelli-2.4.0.tar", last modified: Wed Apr 26 17:38:07 2023, max compression
```

## Comparing `smelli-2.3.2.tar` & `smelli-2.4.0.tar`

### file list

```diff
@@ -1,109 +1,106 @@
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.758816 smelli-2.3.2/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1215 2018-10-17 10:17:39.000000 smelli-2.3.2/.gitignore
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      246 2021-03-08 01:04:07.000000 smelli-2.3.2/.travis.yml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1113 2018-10-17 10:17:39.000000 smelli-2.3.2/LICENSE
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       34 2018-10-17 10:17:39.000000 smelli-2.3.2/MANIFEST.in
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3798 2021-10-01 16:48:47.758816 smelli-2.3.2/PKG-INFO
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     2707 2021-03-08 01:04:07.000000 smelli-2.3.2/README.md
--rwxrwxr-x   0 stangl    (1001) stangl    (1001)      230 2020-11-24 20:08:38.000000 smelli-2.3.2/deploy.sh
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       38 2021-10-01 16:48:47.758816 smelli-2.3.2/setup.cfg
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1141 2021-03-08 01:04:07.000000 smelli-2.3.2/setup.py
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.750815 smelli-2.3.2/smelli/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      309 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/__init__.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       52 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/_version.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)    10722 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/ckm.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)    46734 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/classes.py
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.746815 smelli-2.3.2/smelli/data/
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.750815 smelli-2.3.2/smelli/data/cache/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      710 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/cache/fast_likelihood_leptons.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      710 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/cache/fast_likelihood_leptons.yaml_fix_ckm.p
--rw-rw-r--   0 stangl    (1001) stangl    (1001)   409675 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/cache/fast_likelihood_quarks.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
--rw-rw-r--   0 stangl    (1001) stangl    (1001)   416916 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/cache/fast_likelihood_quarks_fixckm.yaml_fix_ckm.p
--rwxrwxr-x   0 stangl    (1001) stangl    (1001)     1426 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/cache/save_covariances.py
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.750815 smelli-2.3.2/smelli/data/test/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       76 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/test/wcxf.yaml
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.754815 smelli-2.3.2/smelli/data/yaml/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      228 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/fast_likelihood_leptons.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      849 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/fast_likelihood_quarks.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      935 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/fast_likelihood_quarks_fixckm.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      168 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_bcpv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      145 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_bqnunu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      128 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_eeww.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      128 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_ewpt.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      130 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_higgs.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       96 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_lept.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      266 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_lfu_fccc.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      248 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_lfu_fcnc.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      243 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/likelihood_lfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      168 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_rd_rds.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      139 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/likelihood_zlfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       60 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_bcpv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      102 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_bqnunu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       34 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_eeww.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      185 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_ewpt.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       20 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_fixckm.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      249 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_higgs.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       52 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_lept.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       54 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/measurements_leptons.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      193 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_lfu_fccc.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      156 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/measurements_lfu_fcnc.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      315 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/measurements_lfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1994 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/yaml/measurements_quarks.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      168 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_rd_rds.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       68 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/measurements_zlfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      108 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bclnu_lfu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3188 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bctaunu_diff.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       37 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bctaunu_other.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      152 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_beta.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      226 2021-03-08 01:04:07.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstaree_lhcb.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      226 2019-05-24 11:18:25.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarll_lfu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      582 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_atlas_p.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1868 2021-09-10 19:27:59.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_br.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      194 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_cdf.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      586 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_cms.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     2004 2021-09-10 19:27:59.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_lhcb.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      294 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_lhcb_a.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      370 2019-05-23 13:09:56.000000 smelli-2.3.2/smelli/data/yaml/observables_blfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     2004 2021-09-10 19:27:59.000000 smelli-2.3.2/smelli/data/yaml/observables_bpkstarmumu_lhcb.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      136 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bqnunu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       52 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_bqtautau.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       26 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/observables_bsee.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      177 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/data/yaml/observables_bsgamma.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       41 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/observables_bsmumu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      844 2021-10-01 16:43:02.000000 smelli-2.3.2/smelli/data/yaml/observables_bsphimumu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       65 2020-02-29 19:46:46.000000 smelli-2.3.2/smelli/data/yaml/observables_bulnu_lfu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       27 2021-01-03 22:04:58.000000 smelli-2.3.2/smelli/data/yaml/observables_ckm_input.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       84 2020-02-29 19:46:46.000000 smelli-2.3.2/smelli/data/yaml/observables_df2.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3148 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_eeww.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      320 2021-03-08 01:04:07.000000 smelli-2.3.2/smelli/data/yaml/observables_ewpt.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       21 2018-10-17 14:22:05.000000 smelli-2.3.2/smelli/data/yaml/observables_g-2.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      649 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_higgs.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      101 2019-02-06 17:52:31.000000 smelli-2.3.2/smelli/data/yaml/observables_k.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       16 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_klfu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       18 2019-01-31 17:08:21.000000 smelli-2.3.2/smelli/data/yaml/observables_klfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      181 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_lambdablambdall_afb.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       63 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_lambdablambdall_br.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      265 2021-07-10 10:07:51.000000 smelli-2.3.2/smelli/data/yaml/observables_lfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      203 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_n.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       17 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_rd.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       54 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_rds.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      383 2020-02-29 19:46:46.000000 smelli-2.3.2/smelli/data/yaml/observables_rk.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      312 2019-05-23 13:09:56.000000 smelli-2.3.2/smelli/data/yaml/observables_rkstar.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      147 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_sulnu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       66 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_taucc.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       19 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_udlnu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       15 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/observables_udlnu_lfu.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       98 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_xsee.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       42 2018-10-17 10:17:39.000000 smelli-2.3.2/smelli/data/yaml/observables_zlfv.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      672 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/par_ckm_CKMSchemeRmuBtaunuBxlnuDeltaM.yaml
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      824 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/data/yaml/update_ckm.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3400 2020-11-24 20:08:38.000000 smelli-2.3.2/smelli/test_ckm.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     7024 2021-03-08 01:04:07.000000 smelli-2.3.2/smelli/test_classes.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)      148 2021-03-08 02:09:05.000000 smelli-2.3.2/smelli/test_package.py
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     1488 2021-01-03 22:04:58.000000 smelli-2.3.2/smelli/util.py
-drwxrwxr-x   0 stangl    (1001) stangl    (1001)        0 2021-10-01 16:48:47.750815 smelli-2.3.2/smelli.egg-info/
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3798 2021-10-01 16:48:47.000000 smelli-2.3.2/smelli.egg-info/PKG-INFO
--rw-rw-r--   0 stangl    (1001) stangl    (1001)     3841 2021-10-01 16:48:47.000000 smelli-2.3.2/smelli.egg-info/SOURCES.txt
--rw-rw-r--   0 stangl    (1001) stangl    (1001)        1 2021-10-01 16:48:47.000000 smelli-2.3.2/smelli.egg-info/dependency_links.txt
--rw-rw-r--   0 stangl    (1001) stangl    (1001)       75 2021-10-01 16:48:47.000000 smelli-2.3.2/smelli.egg-info/requires.txt
--rw-rw-r--   0 stangl    (1001) stangl    (1001)        7 2021-10-01 16:48:47.000000 smelli-2.3.2/smelli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.120353 smelli-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-26 17:32:50.000000 smelli-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 17:32:50.000000 smelli-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-26 17:38:07.120353 smelli-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-26 17:32:50.000000 smelli-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:38:07.120353 smelli-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-26 17:32:50.000000 smelli-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.108353 smelli-2.4.0/smelli/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47554 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.108353 smelli-2.4.0/smelli/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.112352 smelli-2.4.0/smelli/data/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/cache/fast_likelihood_leptons.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/cache/fast_likelihood_leptons.yaml_fix_ckm.p
+-rw-r--r--   0 runner    (1001) docker     (123)   760905 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/cache/fast_likelihood_quarks.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
+-rw-r--r--   0 runner    (1001) docker     (123)   770770 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/cache/fast_likelihood_quarks_fixckm.yaml_fix_ckm.p
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.112352 smelli-2.4.0/smelli/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/test/wcxf.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.120353 smelli-2.4.0/smelli/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/fast_likelihood_leptons.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/fast_likelihood_quarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/fast_likelihood_quarks_fixckm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_bcpv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_bqnunu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_eeww.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_ewpt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_higgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_lept.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_lfu_fccc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_lfu_fcnc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_lfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_rd_rds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/likelihood_zlfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_bcpv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_bqnunu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_eeww.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_ewpt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_fixckm.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_higgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_lept.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_leptons.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_lfu_fccc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_lfu_fcnc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_lfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_quarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_rd_rds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/measurements_zlfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bctaunu_diff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bctaunu_other.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bdll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_beta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstaree_lhcb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarll_lfu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_atlas_p.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_br.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_cdf.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_cms.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_lhcb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_lhcb_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_blfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bpkstarmumu_lhcb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bqnunu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bqtautau.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bsee.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bsgamma.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bsmumu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bsphimumu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_buenu_lfu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_bulnu_lfu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_ckm_input.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_d.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_df2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_eeww.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_ewpt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_g-2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_higgs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_k.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_klfu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_klfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_lambdablambdall_afb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_lambdablambdall_br.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_lfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_n.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_rd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_rds.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_rk.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_rkstar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_sulnu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_taucc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_udlnu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_udlnu_lfu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_xsee.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/observables_zlfv.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/data/yaml/par_ckm_CKMSchemeRmuBtaunuBxlnuDeltaM.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/test_ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-26 17:32:50.000000 smelli-2.4.0/smelli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:38:07.108353 smelli-2.4.0/smelli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-26 17:38:07.000000 smelli-2.4.0/smelli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-04-26 17:38:07.000000 smelli-2.4.0/smelli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:38:07.000000 smelli-2.4.0/smelli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 17:38:07.000000 smelli-2.4.0/smelli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:38:07.000000 smelli-2.4.0/smelli.egg-info/top_level.txt
```

### Comparing `smelli-2.3.2/LICENSE` & `smelli-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/PKG-INFO` & `smelli-2.4.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 736d 656c  : 2.1.Name: smel
-00000020: 6c69 0a56 6572 7369 6f6e 3a20 322e 332e  li.Version: 2.3.
-00000030: 320a 5375 6d6d 6172 793a 2041 2050 7974  2.Summary: A Pyt
+00000020: 6c69 0a56 6572 7369 6f6e 3a20 322e 342e  li.Version: 2.4.
+00000030: 300a 5375 6d6d 6172 793a 2041 2050 7974  0.Summary: A Pyt
 00000040: 686f 6e20 7061 636b 6167 6520 7072 6f76  hon package prov
 00000050: 6964 696e 6720 6120 676c 6f62 616c 206c  iding a global l
 00000060: 696b 656c 6968 6f6f 6420 6675 6e63 7469  ikelihood functi
 00000070: 6f6e 2069 6e20 7468 6520 7370 6163 6520  on in the space 
 00000080: 6f66 2064 696d 656e 7369 6f6e 2d36 2057  of dimension-6 W
 00000090: 696c 736f 6e20 636f 6566 6669 6369 656e  ilson coefficien
 000000a0: 7473 206f 6620 7468 6520 5374 616e 6461  ts of the Standa
@@ -20,219 +20,185 @@
 00000130: 6b75 6d61 7240 756d 6f6e 7472 6561 6c2e  kumar@umontreal.
 00000140: 6361 3e2c 2050 6574 6572 2053 7461 6e67  ca>, Peter Stang
 00000150: 6c20 3c70 6574 6572 2e73 7461 6e67 6c40  l <peter.stangl@
 00000160: 6c61 7074 682e 636e 7273 2e66 723e 2c20  lapth.cnrs.fr>, 
 00000170: 4461 7669 6420 4d2e 2053 7472 6175 6220  David M. Straub 
 00000180: 3c64 6176 6964 2e73 7472 6175 6240 7475  <david.straub@tu
 00000190: 6d2e 6465 3e0a 4c69 6365 6e73 653a 204d  m.de>.License: M
-000001a0: 4954 0a44 6573 6372 6970 7469 6f6e 3a20  IT.Description: 
-000001b0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000001c0: 2f74 7261 7669 732d 6369 2e6f 7267 2f73  /travis-ci.org/s
-000001d0: 6d65 6c6c 692f 736d 656c 6c69 223e 215b  melli/smelli">![
-000001e0: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
-000001f0: 7470 733a 2f2f 7472 6176 6973 2d63 692e  tps://travis-ci.
-00000200: 6f72 672f 736d 656c 6c69 2f73 6d65 6c6c  org/smelli/smell
-00000210: 692e 7376 673f 6272 616e 6368 3d6d 6173  i.svg?branch=mas
-00000220: 7465 7229 3c2f 613e 205b 215b 436f 7665  ter)</a> [![Cove
-00000230: 7261 6765 2053 7461 7475 735d 2868 7474  rage Status](htt
-00000240: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
-00000250: 6f2f 7265 706f 732f 6769 7468 7562 2f73  o/repos/github/s
-00000260: 6d65 6c6c 692f 736d 656c 6c69 2f62 6164  melli/smelli/bad
-00000270: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
-00000280: 2f63 6f76 6572 616c 6c73 2e69 6f2f 6769  /coveralls.io/gi
-00000290: 7468 7562 2f73 6d65 6c6c 692f 736d 656c  thub/smelli/smel
-000002a0: 6c69 290a 2020 2020 2020 2020 0a20 2020  li).        .   
-000002b0: 2020 2020 2023 2073 6d65 6c6c 6920 e280       # smelli ..
-000002c0: 9320 6120 676c 6f62 616c 206c 696b 656c  . a global likel
-000002d0: 6968 6f6f 6420 666f 7220 7072 6563 6973  ihood for precis
-000002e0: 696f 6e20 636f 6e73 7472 6169 6e74 730a  ion constraints.
-000002f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000300: 2060 736d 656c 6c69 6020 6973 2061 2050   `smelli` is a P
-00000310: 7974 686f 6e20 7061 636b 6167 6520 7072  ython package pr
-00000320: 6f76 6964 696e 6720 6120 676c 6f62 616c  oviding a global
-00000330: 206c 696b 656c 6968 6f6f 6420 6675 6e63   likelihood func
-00000340: 7469 6f6e 2069 6e20 7468 650a 2020 2020  tion in the.    
-00000350: 2020 2020 7370 6163 6520 6f66 2064 696d      space of dim
-00000360: 656e 7369 6f6e 2d73 6978 2057 696c 736f  ension-six Wilso
-00000370: 6e20 636f 6566 6669 6369 656e 7473 2069  n coefficients i
-00000380: 6e20 7468 6520 5374 616e 6461 7264 204d  n the Standard M
-00000390: 6f64 656c 2045 6666 6563 7469 7665 0a20  odel Effective. 
-000003a0: 2020 2020 2020 2046 6965 6c64 2054 6865         Field The
-000003b0: 6f72 7920 2853 4d45 4654 292e 2054 6865  ory (SMEFT). The
-000003c0: 206c 696b 656c 6968 6f6f 6420 696e 636c   likelihood incl
-000003d0: 7564 6573 2063 6f6e 7472 6962 7574 696f  udes contributio
-000003e0: 6e73 2066 726f 6d0a 2020 2020 2020 2020  ns from.        
-000003f0: 7175 6172 6b20 616e 6420 6c65 7074 6f6e  quark and lepton
-00000400: 2066 6c61 766f 7572 2070 6879 7369 6373   flavour physics
-00000410: 2c20 656c 6563 7472 6f77 6561 6b20 7072  , electroweak pr
-00000420: 6563 6973 696f 6e20 7465 7374 732c 2061  ecision tests, a
-00000430: 6e64 206f 7468 6572 0a20 2020 2020 2020  nd other.       
-00000440: 2070 7265 6369 7369 6f6e 206f 6273 6572   precision obser
-00000450: 7661 626c 6573 2e0a 2020 2020 2020 2020  vables..        
-00000460: 0a20 2020 2020 2020 2054 6865 2070 6163  .        The pac
-00000470: 6b61 6765 2069 7320 6261 7365 6420 6f6e  kage is based on
-00000480: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
-00000490: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
-000004a0: 762d 696f 2f66 6c61 7669 6f29 2066 6f72  v-io/flavio) for
-000004b0: 2074 6865 0a20 2020 2020 2020 2063 616c   the.        cal
-000004c0: 6375 6c61 7469 6f6e 206f 6620 6f62 7365  culation of obse
-000004d0: 7276 6162 6c65 7320 616e 6420 7374 6174  rvables and stat
-000004e0: 6973 7469 6361 6c20 7472 6561 746d 656e  istical treatmen
-000004f0: 7420 616e 640a 2020 2020 2020 2020 5b77  t and.        [w
-00000500: 696c 736f 6e5d 2868 7474 7073 3a2f 2f67  ilson](https://g
-00000510: 6974 6875 622e 636f 6d2f 7769 6c73 6f6e  ithub.com/wilson
-00000520: 2d65 6674 2f77 696c 736f 6e29 2066 6f72  -eft/wilson) for
-00000530: 2074 6865 2072 756e 6e69 6e67 2c20 7472   the running, tr
-00000540: 616e 736c 6174 696f 6e2c 0a20 2020 2020  anslation,.     
-00000550: 2020 2061 6e64 206d 6174 6368 696e 6720     and matching 
-00000560: 6f66 2057 696c 736f 6e20 636f 6566 6669  of Wilson coeffi
-00000570: 6369 656e 7473 2e0a 2020 2020 2020 2020  cients..        
-00000580: 0a20 2020 2020 2020 2023 2320 496e 7374  .        ## Inst
-00000590: 616c 6c61 7469 6f6e 0a20 2020 2020 2020  allation.       
-000005a0: 200a 2020 2020 2020 2020 5468 6520 7061   .        The pa
-000005b0: 636b 6167 6520 7265 7175 6972 6573 2050  ckage requires P
-000005c0: 7974 686f 6e20 7665 7273 696f 6e20 332e  ython version 3.
-000005d0: 3620 6f72 2061 626f 7665 2e20 4974 2063  6 or above. It c
-000005e0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
-000005f0: 7769 7468 0a20 2020 2020 2020 200a 2020  with.        .  
-00000600: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
-00000610: 2020 2020 2020 7079 7468 6f6e 3320 2d6d        python3 -m
-00000620: 2070 6970 2069 6e73 7461 6c6c 2073 6d65   pip install sme
-00000630: 6c6c 6920 2d2d 7573 6572 0a20 2020 2020  lli --user.     
-00000640: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00000650: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000660: 2023 2320 446f 6375 6d65 6e74 6174 696f   ## Documentatio
-00000670: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00000680: 2020 2041 2062 7269 6566 2075 7365 7220     A brief user 
-00000690: 6d61 6e75 616c 2063 616e 2062 6520 666f  manual can be fo
-000006a0: 756e 6420 696e 2074 6865 2070 6170 6572  und in the paper
-000006b0: 2063 6974 6564 2062 656c 6f77 2e0a 2020   cited below..  
-000006c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000006d0: 2320 4369 7461 7469 6f6e 0a20 2020 2020  # Citation.     
-000006e0: 2020 200a 2020 2020 2020 2020 4966 2079     .        If y
-000006f0: 6f75 2075 7365 2060 736d 656c 6c69 6020  ou use `smelli` 
-00000700: 696e 2061 2073 6369 656e 7469 6669 6320  in a scientific 
-00000710: 7075 626c 6963 6174 696f 6e2c 2070 6c65  publication, ple
-00000720: 6173 6520 6369 7465 0a20 2020 2020 2020  ase cite.       
-00000730: 200a 2020 2020 2020 2020 3e20 204a 2e20   .        >  J. 
-00000740: 4165 6269 7363 6865 722c 204a 2e20 4b75  Aebischer, J. Ku
-00000750: 6d61 722c 2050 2e20 5374 616e 676c 2c20  mar, P. Stangl, 
-00000760: 616e 6420 442e 204d 2e20 5374 7261 7562  and D. M. Straub
-00000770: 0a20 2020 2020 2020 203e 0a20 2020 2020  .        >.     
-00000780: 2020 203e 2022 4120 476c 6f62 616c 204c     > "A Global L
-00000790: 696b 656c 6968 6f6f 6420 666f 7220 5072  ikelihood for Pr
-000007a0: 6563 6973 696f 6e20 436f 6e73 7472 6169  ecision Constrai
-000007b0: 6e74 7320 616e 6420 466c 6176 6f75 7220  nts and Flavour 
-000007c0: 416e 6f6d 616c 6965 7322 0a20 2020 2020  Anomalies".     
-000007d0: 2020 203e 0a20 2020 2020 2020 203e 2020     >.        >  
-000007e0: 5b61 7258 6976 3a31 3831 302e 3037 3639  [arXiv:1810.0769
-000007f0: 3820 5b68 6570 2d70 685d 5d28 6874 7470  8 [hep-ph]](http
-00000800: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-00000810: 732f 3138 3130 2e30 3736 3938 290a 2020  s/1810.07698).  
-00000820: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
-00000830: 6c65 6173 6520 616c 736f 2063 6974 6520  lease also cite 
-00000840: 7468 6520 7075 626c 6963 6174 696f 6e73  the publications
-00000850: 206f 6e20 5b66 6c61 7669 6f5d 2868 7474   on [flavio](htt
-00000860: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000870: 6273 2f31 3831 302e 3038 3133 3229 2061  bs/1810.08132) a
-00000880: 6e64 205b 7769 6c73 6f6e 5d28 6874 7470  nd [wilson](http
-00000890: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000008a0: 732f 3138 3034 2e30 3530 3333 292c 2077  s/1804.05033), w
-000008b0: 6869 6368 2061 7265 2074 6865 2070 696c  hich are the pil
-000008c0: 6c61 7273 2060 736d 656c 6c69 6020 6973  lars `smelli` is
-000008d0: 2020 6275 696c 7420 6f6e 2e0a 2020 2020    built on..    
-000008e0: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-000008f0: 4275 6773 2061 6e64 2066 6561 7475 7265  Bugs and feature
-00000900: 2072 6571 7565 7374 730a 2020 2020 2020   requests.      
-00000910: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
-00000920: 6520 7375 626d 6974 2062 7567 7320 616e  e submit bugs an
-00000930: 6420 6665 6174 7572 6520 7265 7175 6573  d feature reques
-00000940: 7473 2075 7369 6e67 0a20 2020 2020 2020  ts using.       
-00000950: 205b 4769 7468 7562 2773 2069 7373 7565   [Github's issue
-00000960: 2073 7973 7465 6d5d 2868 7474 7073 3a2f   system](https:/
-00000970: 2f67 6974 6875 622e 636f 6d2f 736d 656c  /github.com/smel
-00000980: 6c69 2f73 6d65 6c6c 692f 6973 7375 6573  li/smelli/issues
-00000990: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
-000009a0: 2020 2020 2323 2043 6f6e 7472 6962 7574      ## Contribut
-000009b0: 696e 670a 2020 2020 2020 2020 0a20 2020  ing.        .   
-000009c0: 2020 2020 2054 6865 2061 696d 206f 6620       The aim of 
-000009d0: 7468 6520 7061 636b 6167 6520 6973 2074  the package is t
-000009e0: 6f20 7072 6f76 6964 6520 6120 6c69 6b65  o provide a like
-000009f0: 6c69 686f 6f64 2069 6e20 7468 650a 2020  lihood in the.  
-00000a00: 2020 2020 2020 7370 6163 6520 6f66 2064        space of d
-00000a10: 696d 656e 7369 6f6e 2d36 2053 4d45 4654  imension-6 SMEFT
-00000a20: 2057 696c 736f 6e20 636f 6566 6669 6369   Wilson coeffici
-00000a30: 656e 7473 2075 7369 6e67 2061 6c6c 0a20  ents using all. 
-00000a40: 2020 2020 2020 2072 656c 6576 616e 7420         relevant 
-00000a50: 6176 6169 6c61 626c 6520 6578 7065 7269  available experi
-00000a60: 6d65 6e74 616c 206d 6561 7375 7265 6d65  mental measureme
-00000a70: 6e74 732e 2049 6620 796f 7520 7761 6e74  nts. If you want
-00000a80: 0a20 2020 2020 2020 2074 6f20 636f 6e74  .        to cont
-00000a90: 7269 6275 7465 2061 6464 6974 696f 6e61  ribute additiona
-00000aa0: 6c20 6f62 7365 7276 6162 6c65 732c 2074  l observables, t
-00000ab0: 6865 2065 6173 6965 7374 2077 6179 2069  he easiest way i
-00000ac0: 730a 2020 2020 2020 2020 746f 2069 6d70  s.        to imp
-00000ad0: 6c65 6d65 6e74 2074 6865 206f 6273 6572  lement the obser
-00000ae0: 7661 626c 6520 696e 205b 666c 6176 696f  vable in [flavio
-00000af0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000b00: 2e63 6f6d 2f66 6c61 762d 696f 2f66 6c61  .com/flav-io/fla
-00000b10: 7669 6f29 2e20 4f62 7365 7276 6162 6c65  vio). Observable
-00000b20: 730a 2020 2020 2020 2020 696d 706c 656d  s.        implem
-00000b30: 656e 7465 6420 7468 6572 6520 6361 6e20  ented there can 
-00000b40: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-00000b50: 6c69 6b65 6c69 686f 6f64 2073 696d 706c  likelihood simpl
-00000b60: 790a 2020 2020 2020 2020 6279 2061 6464  y.        by add
-00000b70: 696e 6720 6120 636f 7272 6573 706f 6e64  ing a correspond
-00000b80: 696e 6720 656e 7472 7920 696e 206f 6e65  ing entry in one
-00000b90: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00000ba0: 5b6f 6273 6572 7661 626c 6520 5941 4d4c  [observable YAML
-00000bb0: 2066 696c 6573 5d28 6874 7470 733a 2f2f   files](https://
-00000bc0: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
-00000bd0: 692f 736d 656c 6c69 2f74 7265 652f 6d61  i/smelli/tree/ma
-00000be0: 7374 6572 2f73 6d65 6c6c 692f 6461 7461  ster/smelli/data
-00000bf0: 2f79 616d 6c29 2e0a 2020 2020 2020 2020  /yaml)..        
-00000c00: 0a20 2020 2020 2020 2041 6c74 6572 6e61  .        Alterna
-00000c10: 7469 7665 6c79 2c20 616c 736f 206f 6273  tively, also obs
-00000c20: 6572 7661 626c 6573 2063 6f6d 7075 7465  ervables compute
-00000c30: 6420 696e 2061 6e79 206f 7468 6572 2073  d in any other s
-00000c40: 7461 6e64 616c 6f6e 6520 5079 7468 6f6e  tandalone Python
-00000c50: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
-00000c60: 696e 636f 7270 6f72 6174 6564 2069 6e20  incorporated in 
-00000c70: 7072 696e 6369 706c 6520 6173 206c 6f6e  principle as lon
-00000c80: 6720 6173 2069 7420 6164 6865 7265 7320  g as it adheres 
-00000c90: 746f 2074 6865 205b 5743 7866 2073 7461  to the [WCxf sta
-00000ca0: 6e64 6172 645d 2868 7474 7073 3a2f 2f77  ndard](https://w
-00000cb0: 6378 662e 6769 7468 7562 2e69 6f29 2e0a  cxf.github.io)..
-00000cc0: 2020 2020 2020 2020 4966 2079 6f75 2077          If you w
-00000cd0: 616e 7420 746f 2066 6f6c 6c6f 7720 7468  ant to follow th
-00000ce0: 6973 2072 6f75 7465 2c20 706c 6561 7365  is route, please
-00000cf0: 206f 7065 6e20 616e 205b 6973 7375 655d   open an [issue]
-00000d00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d10: 636f 6d2f 736d 656c 6c69 2f73 6d65 6c6c  com/smelli/smell
-00000d20: 692f 6973 7375 6573 2920 746f 2073 7461  i/issues) to sta
-00000d30: 7274 2074 6865 2064 6973 6375 7373 696f  rt the discussio
-00000d40: 6e20 6f6e 2068 6f77 2074 6f20 696e 7465  n on how to inte
-00000d50: 6772 6174 6520 6974 2e0a 2020 2020 2020  grate it..      
-00000d60: 2020 0a20 2020 2020 2020 2023 2320 436f    .        ## Co
-00000d70: 6e74 7269 6275 746f 7273 0a20 2020 2020  ntributors.     
-00000d80: 2020 200a 2020 2020 2020 2020 496e 2061     .        In a
-00000d90: 6c70 6861 6265 7469 6361 6c20 6f72 6465  lphabetical orde
-00000da0: 723a 0a20 2020 2020 2020 200a 2020 2020  r:.        .    
-00000db0: 2020 2020 2d20 4a61 736f 6e20 4165 6269      - Jason Aebi
-00000dc0: 7363 6865 720a 2020 2020 2020 2020 2d20  scher.        - 
-00000dd0: 4d61 7474 6865 7720 4b69 726b 0a20 2020  Matthew Kirk.   
-00000de0: 2020 2020 202d 204a 6163 6b79 204b 756d       - Jacky Kum
-00000df0: 6172 0a20 2020 2020 2020 202d 2050 6574  ar.        - Pet
-00000e00: 6572 2053 7461 6e67 6c0a 2020 2020 2020  er Stangl.      
-00000e10: 2020 2d20 4461 7669 6420 4d2e 2053 7472    - David M. Str
-00000e20: 6175 620a 2020 2020 2020 2020 0a20 2020  aub.        .   
-00000e30: 2020 2020 2023 2320 4c69 6365 6e73 650a       ## License.
-00000e40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000e50: 2073 6d65 6c6c 6920 6973 2072 656c 6561   smelli is relea
-00000e60: 7365 6420 756e 6465 7220 7468 6520 4d49  sed under the MI
-00000e70: 5420 6c69 6365 6e73 652e 0a20 2020 2020  T license..     
-00000e80: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
-00000e90: 4b4e 4f57 4e0a 4465 7363 7269 7074 696f  KNOWN.Descriptio
-00000ea0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000eb0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-00000ec0: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
-00000ed0: 7374 696e 670a                           sting.
+000001a0: 4954 0a50 6c61 7466 6f72 6d3a 2055 4e4b  IT.Platform: UNK
+000001b0: 4e4f 574e 0a44 6573 6372 6970 7469 6f6e  NOWN.Description
+000001c0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000001d0: 6578 742f 6d61 726b 646f 776e 0a50 726f  ext/markdown.Pro
+000001e0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
+000001f0: 7469 6e67 0a4c 6963 656e 7365 2d46 696c  ting.License-Fil
+00000200: 653a 204c 4943 454e 5345 0a0a 5b21 5b75  e: LICENSE..[![u
+00000210: 6e69 7420 7465 7374 735d 2868 7474 7073  nit tests](https
+00000220: 3a2f 2f67 6974 6875 622e 636f 6d2f 666c  ://github.com/fl
+00000230: 6176 2d69 6f2f 666c 6176 696f 2f61 6374  av-io/flavio/act
+00000240: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
+00000250: 6573 742e 796d 6c2f 6261 6467 652e 7376  est.yml/badge.sv
+00000260: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000270: 7562 2e63 6f6d 2f73 6d65 6c6c 692f 736d  ub.com/smelli/sm
+00000280: 656c 6c69 2f61 6374 696f 6e73 2f77 6f72  elli/actions/wor
+00000290: 6b66 6c6f 7773 2f74 6573 742e 796d 6c29  kflows/test.yml)
+000002a0: 0a0a 0a0a 0a23 2073 6d65 6c6c 6920 e280  .....# smelli ..
+000002b0: 9320 6120 676c 6f62 616c 206c 696b 656c  . a global likel
+000002c0: 6968 6f6f 6420 666f 7220 7072 6563 6973  ihood for precis
+000002d0: 696f 6e20 636f 6e73 7472 6169 6e74 730a  ion constraints.
+000002e0: 0a60 736d 656c 6c69 6020 6973 2061 2050  .`smelli` is a P
+000002f0: 7974 686f 6e20 7061 636b 6167 6520 7072  ython package pr
+00000300: 6f76 6964 696e 6720 6120 676c 6f62 616c  oviding a global
+00000310: 206c 696b 656c 6968 6f6f 6420 6675 6e63   likelihood func
+00000320: 7469 6f6e 2069 6e20 7468 650a 7370 6163  tion in the.spac
+00000330: 6520 6f66 2064 696d 656e 7369 6f6e 2d73  e of dimension-s
+00000340: 6978 2057 696c 736f 6e20 636f 6566 6669  ix Wilson coeffi
+00000350: 6369 656e 7473 2069 6e20 7468 6520 5374  cients in the St
+00000360: 616e 6461 7264 204d 6f64 656c 2045 6666  andard Model Eff
+00000370: 6563 7469 7665 0a46 6965 6c64 2054 6865  ective.Field The
+00000380: 6f72 7920 2853 4d45 4654 292e 2054 6865  ory (SMEFT). The
+00000390: 206c 696b 656c 6968 6f6f 6420 696e 636c   likelihood incl
+000003a0: 7564 6573 2063 6f6e 7472 6962 7574 696f  udes contributio
+000003b0: 6e73 2066 726f 6d0a 7175 6172 6b20 616e  ns from.quark an
+000003c0: 6420 6c65 7074 6f6e 2066 6c61 766f 7572  d lepton flavour
+000003d0: 2070 6879 7369 6373 2c20 656c 6563 7472   physics, electr
+000003e0: 6f77 6561 6b20 7072 6563 6973 696f 6e20  oweak precision 
+000003f0: 7465 7374 732c 2061 6e64 206f 7468 6572  tests, and other
+00000400: 0a70 7265 6369 7369 6f6e 206f 6273 6572  .precision obser
+00000410: 7661 626c 6573 2e0a 0a54 6865 2070 6163  vables...The pac
+00000420: 6b61 6765 2069 7320 6261 7365 6420 6f6e  kage is based on
+00000430: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
+00000440: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
+00000450: 762d 696f 2f66 6c61 7669 6f29 2066 6f72  v-io/flavio) for
+00000460: 2074 6865 0a63 616c 6375 6c61 7469 6f6e   the.calculation
+00000470: 206f 6620 6f62 7365 7276 6162 6c65 7320   of observables 
+00000480: 616e 6420 7374 6174 6973 7469 6361 6c20  and statistical 
+00000490: 7472 6561 746d 656e 7420 616e 640a 5b77  treatment and.[w
+000004a0: 696c 736f 6e5d 2868 7474 7073 3a2f 2f67  ilson](https://g
+000004b0: 6974 6875 622e 636f 6d2f 7769 6c73 6f6e  ithub.com/wilson
+000004c0: 2d65 6674 2f77 696c 736f 6e29 2066 6f72  -eft/wilson) for
+000004d0: 2074 6865 2072 756e 6e69 6e67 2c20 7472   the running, tr
+000004e0: 616e 736c 6174 696f 6e2c 0a61 6e64 206d  anslation,.and m
+000004f0: 6174 6368 696e 6720 6f66 2057 696c 736f  atching of Wilso
+00000500: 6e20 636f 6566 6669 6369 656e 7473 2e0a  n coefficients..
+00000510: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000520: 0a0a 5468 6520 7061 636b 6167 6520 7265  ..The package re
+00000530: 7175 6972 6573 2050 7974 686f 6e20 7665  quires Python ve
+00000540: 7273 696f 6e20 332e 3620 6f72 2061 626f  rsion 3.6 or abo
+00000550: 7665 2e20 4974 2063 616e 2062 6520 696e  ve. It can be in
+00000560: 7374 616c 6c65 6420 7769 7468 0a0a 6060  stalled with..``
+00000570: 6062 6173 680a 7079 7468 6f6e 3320 2d6d  `bash.python3 -m
+00000580: 2070 6970 2069 6e73 7461 6c6c 2073 6d65   pip install sme
+00000590: 6c6c 6920 2d2d 7573 6572 0a60 6060 0a0a  lli --user.```..
+000005a0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
+000005b0: 6e0a 0a41 2062 7269 6566 2075 7365 7220  n..A brief user 
+000005c0: 6d61 6e75 616c 2063 616e 2062 6520 666f  manual can be fo
+000005d0: 756e 6420 696e 2074 6865 2070 6170 6572  und in the paper
+000005e0: 2063 6974 6564 2062 656c 6f77 2e0a 0a23   cited below...#
+000005f0: 2320 4369 7461 7469 6f6e 0a0a 4966 2079  # Citation..If y
+00000600: 6f75 2075 7365 2060 736d 656c 6c69 6020  ou use `smelli` 
+00000610: 696e 2061 2073 6369 656e 7469 6669 6320  in a scientific 
+00000620: 7075 626c 6963 6174 696f 6e2c 2070 6c65  publication, ple
+00000630: 6173 6520 6369 7465 0a0a 3e20 204a 2e20  ase cite..>  J. 
+00000640: 4165 6269 7363 6865 722c 204a 2e20 4b75  Aebischer, J. Ku
+00000650: 6d61 722c 2050 2e20 5374 616e 676c 2c20  mar, P. Stangl, 
+00000660: 616e 6420 442e 204d 2e20 5374 7261 7562  and D. M. Straub
+00000670: 0a3e 0a3e 2022 4120 476c 6f62 616c 204c  .>.> "A Global L
+00000680: 696b 656c 6968 6f6f 6420 666f 7220 5072  ikelihood for Pr
+00000690: 6563 6973 696f 6e20 436f 6e73 7472 6169  ecision Constrai
+000006a0: 6e74 7320 616e 6420 466c 6176 6f75 7220  nts and Flavour 
+000006b0: 416e 6f6d 616c 6965 7322 0a3e 0a3e 2020  Anomalies".>.>  
+000006c0: 5b61 7258 6976 3a31 3831 302e 3037 3639  [arXiv:1810.0769
+000006d0: 3820 5b68 6570 2d70 685d 5d28 6874 7470  8 [hep-ph]](http
+000006e0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000006f0: 732f 3138 3130 2e30 3736 3938 290a 0a50  s/1810.07698)..P
+00000700: 6c65 6173 6520 616c 736f 2063 6974 6520  lease also cite 
+00000710: 7468 6520 7075 626c 6963 6174 696f 6e73  the publications
+00000720: 206f 6e20 5b66 6c61 7669 6f5d 2868 7474   on [flavio](htt
+00000730: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000740: 6273 2f31 3831 302e 3038 3133 3229 2061  bs/1810.08132) a
+00000750: 6e64 205b 7769 6c73 6f6e 5d28 6874 7470  nd [wilson](http
+00000760: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00000770: 732f 3138 3034 2e30 3530 3333 292c 2077  s/1804.05033), w
+00000780: 6869 6368 2061 7265 2074 6865 2070 696c  hich are the pil
+00000790: 6c61 7273 2060 736d 656c 6c69 6020 6973  lars `smelli` is
+000007a0: 2020 6275 696c 7420 6f6e 2e0a 0a23 2320    built on...## 
+000007b0: 4275 6773 2061 6e64 2066 6561 7475 7265  Bugs and feature
+000007c0: 2072 6571 7565 7374 730a 0a50 6c65 6173   requests..Pleas
+000007d0: 6520 7375 626d 6974 2062 7567 7320 616e  e submit bugs an
+000007e0: 6420 6665 6174 7572 6520 7265 7175 6573  d feature reques
+000007f0: 7473 2075 7369 6e67 0a5b 4769 7468 7562  ts using.[Github
+00000800: 2773 2069 7373 7565 2073 7973 7465 6d5d  's issue system]
+00000810: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000820: 636f 6d2f 736d 656c 6c69 2f73 6d65 6c6c  com/smelli/smell
+00000830: 692f 6973 7375 6573 292e 0a0a 2323 2043  i/issues)...## C
+00000840: 6f6e 7472 6962 7574 696e 670a 0a54 6865  ontributing..The
+00000850: 2061 696d 206f 6620 7468 6520 7061 636b   aim of the pack
+00000860: 6167 6520 6973 2074 6f20 7072 6f76 6964  age is to provid
+00000870: 6520 6120 6c69 6b65 6c69 686f 6f64 2069  e a likelihood i
+00000880: 6e20 7468 650a 7370 6163 6520 6f66 2064  n the.space of d
+00000890: 696d 656e 7369 6f6e 2d36 2053 4d45 4654  imension-6 SMEFT
+000008a0: 2057 696c 736f 6e20 636f 6566 6669 6369   Wilson coeffici
+000008b0: 656e 7473 2075 7369 6e67 2061 6c6c 0a72  ents using all.r
+000008c0: 656c 6576 616e 7420 6176 6169 6c61 626c  elevant availabl
+000008d0: 6520 6578 7065 7269 6d65 6e74 616c 206d  e experimental m
+000008e0: 6561 7375 7265 6d65 6e74 732e 2049 6620  easurements. If 
+000008f0: 796f 7520 7761 6e74 0a74 6f20 636f 6e74  you want.to cont
+00000900: 7269 6275 7465 2061 6464 6974 696f 6e61  ribute additiona
+00000910: 6c20 6f62 7365 7276 6162 6c65 732c 2074  l observables, t
+00000920: 6865 2065 6173 6965 7374 2077 6179 2069  he easiest way i
+00000930: 730a 746f 2069 6d70 6c65 6d65 6e74 2074  s.to implement t
+00000940: 6865 206f 6273 6572 7661 626c 6520 696e  he observable in
+00000950: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
+00000960: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
+00000970: 762d 696f 2f66 6c61 7669 6f29 2e20 4f62  v-io/flavio). Ob
+00000980: 7365 7276 6162 6c65 730a 696d 706c 656d  servables.implem
+00000990: 656e 7465 6420 7468 6572 6520 6361 6e20  ented there can 
+000009a0: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
+000009b0: 6c69 6b65 6c69 686f 6f64 2073 696d 706c  likelihood simpl
+000009c0: 790a 6279 2061 6464 696e 6720 6120 636f  y.by adding a co
+000009d0: 7272 6573 706f 6e64 696e 6720 656e 7472  rresponding entr
+000009e0: 7920 696e 206f 6e65 206f 6620 7468 650a  y in one of the.
+000009f0: 5b6f 6273 6572 7661 626c 6520 5941 4d4c  [observable YAML
+00000a00: 2066 696c 6573 5d28 6874 7470 733a 2f2f   files](https://
+00000a10: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
+00000a20: 692f 736d 656c 6c69 2f74 7265 652f 6d61  i/smelli/tree/ma
+00000a30: 7374 6572 2f73 6d65 6c6c 692f 6461 7461  ster/smelli/data
+00000a40: 2f79 616d 6c29 2e0a 0a41 6c74 6572 6e61  /yaml)...Alterna
+00000a50: 7469 7665 6c79 2c20 616c 736f 206f 6273  tively, also obs
+00000a60: 6572 7661 626c 6573 2063 6f6d 7075 7465  ervables compute
+00000a70: 6420 696e 2061 6e79 206f 7468 6572 2073  d in any other s
+00000a80: 7461 6e64 616c 6f6e 6520 5079 7468 6f6e  tandalone Python
+00000a90: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
+00000aa0: 696e 636f 7270 6f72 6174 6564 2069 6e20  incorporated in 
+00000ab0: 7072 696e 6369 706c 6520 6173 206c 6f6e  principle as lon
+00000ac0: 6720 6173 2069 7420 6164 6865 7265 7320  g as it adheres 
+00000ad0: 746f 2074 6865 205b 5743 7866 2073 7461  to the [WCxf sta
+00000ae0: 6e64 6172 645d 2868 7474 7073 3a2f 2f77  ndard](https://w
+00000af0: 6378 662e 6769 7468 7562 2e69 6f29 2e0a  cxf.github.io)..
+00000b00: 4966 2079 6f75 2077 616e 7420 746f 2066  If you want to f
+00000b10: 6f6c 6c6f 7720 7468 6973 2072 6f75 7465  ollow this route
+00000b20: 2c20 706c 6561 7365 206f 7065 6e20 616e  , please open an
+00000b30: 205b 6973 7375 655d 2868 7474 7073 3a2f   [issue](https:/
+00000b40: 2f67 6974 6875 622e 636f 6d2f 736d 656c  /github.com/smel
+00000b50: 6c69 2f73 6d65 6c6c 692f 6973 7375 6573  li/smelli/issues
+00000b60: 2920 746f 2073 7461 7274 2074 6865 2064  ) to start the d
+00000b70: 6973 6375 7373 696f 6e20 6f6e 2068 6f77  iscussion on how
+00000b80: 2074 6f20 696e 7465 6772 6174 6520 6974   to integrate it
+00000b90: 2e0a 0a23 2320 436f 6e74 7269 6275 746f  ...## Contributo
+00000ba0: 7273 0a0a 4d61 696e 7461 696e 6572 3a0a  rs..Maintainer:.
+00000bb0: 0a2d 2050 6574 6572 2053 7461 6e67 6c20  .- Peter Stangl 
+00000bc0: 2840 7065 7465 7273 7461 6e67 6c29 0a0a  (@peterstangl)..
+00000bd0: 436f 6e74 7269 6275 746f 7273 2028 696e  Contributors (in
+00000be0: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
+00000bf0: 6465 7229 3a0a 0a2d 204a 6173 6f6e 2041  der):..- Jason A
+00000c00: 6562 6973 6368 6572 0a2d 204d 6174 c49b  ebischer.- Mat..
+00000c10: 6a20 4875 6465 630a 2d20 4d61 7474 6865  j Hudec.- Matthe
+00000c20: 7720 4b69 726b 0a2d 204a 6163 6b79 204b  w Kirk.- Jacky K
+00000c30: 756d 6172 0a2d 204e 696c 6164 7269 2053  umar.- Niladri S
+00000c40: 6168 6f6f 0a2d 2041 6c65 6b73 2053 6d6f  ahoo.- Aleks Smo
+00000c50: 6c6b 6f76 69c4 8d0a 2d20 5065 7465 7220  lkovi...- Peter 
+00000c60: 5374 616e 676c 0a2d 2044 6176 6964 204d  Stangl.- David M
+00000c70: 2e20 5374 7261 7562 0a0a 2323 204c 6963  . Straub..## Lic
+00000c80: 656e 7365 0a0a 736d 656c 6c69 2069 7320  ense..smelli is 
+00000c90: 7265 6c65 6173 6564 2075 6e64 6572 2074  released under t
+00000ca0: 6865 204d 4954 206c 6963 656e 7365 2e0a  he MIT license..
+00000cb0: 0a0a                                     ..
```

### Comparing `smelli-2.3.2/README.md` & `smelli-2.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,171 @@
-00000000: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000010: 2f74 7261 7669 732d 6369 2e6f 7267 2f73  /travis-ci.org/s
-00000020: 6d65 6c6c 692f 736d 656c 6c69 223e 215b  melli/smelli">![
-00000030: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
-00000040: 7470 733a 2f2f 7472 6176 6973 2d63 692e  tps://travis-ci.
-00000050: 6f72 672f 736d 656c 6c69 2f73 6d65 6c6c  org/smelli/smell
-00000060: 692e 7376 673f 6272 616e 6368 3d6d 6173  i.svg?branch=mas
-00000070: 7465 7229 3c2f 613e 205b 215b 436f 7665  ter)</a> [![Cove
-00000080: 7261 6765 2053 7461 7475 735d 2868 7474  rage Status](htt
-00000090: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
-000000a0: 6f2f 7265 706f 732f 6769 7468 7562 2f73  o/repos/github/s
-000000b0: 6d65 6c6c 692f 736d 656c 6c69 2f62 6164  melli/smelli/bad
-000000c0: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
-000000d0: 2f63 6f76 6572 616c 6c73 2e69 6f2f 6769  /coveralls.io/gi
-000000e0: 7468 7562 2f73 6d65 6c6c 692f 736d 656c  thub/smelli/smel
-000000f0: 6c69 290a 0a23 2073 6d65 6c6c 6920 e280  li)..# smelli ..
-00000100: 9320 6120 676c 6f62 616c 206c 696b 656c  . a global likel
-00000110: 6968 6f6f 6420 666f 7220 7072 6563 6973  ihood for precis
-00000120: 696f 6e20 636f 6e73 7472 6169 6e74 730a  ion constraints.
-00000130: 0a60 736d 656c 6c69 6020 6973 2061 2050  .`smelli` is a P
-00000140: 7974 686f 6e20 7061 636b 6167 6520 7072  ython package pr
-00000150: 6f76 6964 696e 6720 6120 676c 6f62 616c  oviding a global
-00000160: 206c 696b 656c 6968 6f6f 6420 6675 6e63   likelihood func
-00000170: 7469 6f6e 2069 6e20 7468 650a 7370 6163  tion in the.spac
-00000180: 6520 6f66 2064 696d 656e 7369 6f6e 2d73  e of dimension-s
-00000190: 6978 2057 696c 736f 6e20 636f 6566 6669  ix Wilson coeffi
-000001a0: 6369 656e 7473 2069 6e20 7468 6520 5374  cients in the St
-000001b0: 616e 6461 7264 204d 6f64 656c 2045 6666  andard Model Eff
-000001c0: 6563 7469 7665 0a46 6965 6c64 2054 6865  ective.Field The
-000001d0: 6f72 7920 2853 4d45 4654 292e 2054 6865  ory (SMEFT). The
-000001e0: 206c 696b 656c 6968 6f6f 6420 696e 636c   likelihood incl
-000001f0: 7564 6573 2063 6f6e 7472 6962 7574 696f  udes contributio
-00000200: 6e73 2066 726f 6d0a 7175 6172 6b20 616e  ns from.quark an
-00000210: 6420 6c65 7074 6f6e 2066 6c61 766f 7572  d lepton flavour
-00000220: 2070 6879 7369 6373 2c20 656c 6563 7472   physics, electr
-00000230: 6f77 6561 6b20 7072 6563 6973 696f 6e20  oweak precision 
-00000240: 7465 7374 732c 2061 6e64 206f 7468 6572  tests, and other
-00000250: 0a70 7265 6369 7369 6f6e 206f 6273 6572  .precision obser
-00000260: 7661 626c 6573 2e0a 0a54 6865 2070 6163  vables...The pac
-00000270: 6b61 6765 2069 7320 6261 7365 6420 6f6e  kage is based on
-00000280: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
-00000290: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
-000002a0: 762d 696f 2f66 6c61 7669 6f29 2066 6f72  v-io/flavio) for
-000002b0: 2074 6865 0a63 616c 6375 6c61 7469 6f6e   the.calculation
-000002c0: 206f 6620 6f62 7365 7276 6162 6c65 7320   of observables 
-000002d0: 616e 6420 7374 6174 6973 7469 6361 6c20  and statistical 
-000002e0: 7472 6561 746d 656e 7420 616e 640a 5b77  treatment and.[w
-000002f0: 696c 736f 6e5d 2868 7474 7073 3a2f 2f67  ilson](https://g
-00000300: 6974 6875 622e 636f 6d2f 7769 6c73 6f6e  ithub.com/wilson
-00000310: 2d65 6674 2f77 696c 736f 6e29 2066 6f72  -eft/wilson) for
-00000320: 2074 6865 2072 756e 6e69 6e67 2c20 7472   the running, tr
-00000330: 616e 736c 6174 696f 6e2c 0a61 6e64 206d  anslation,.and m
-00000340: 6174 6368 696e 6720 6f66 2057 696c 736f  atching of Wilso
-00000350: 6e20 636f 6566 6669 6369 656e 7473 2e0a  n coefficients..
-00000360: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
-00000370: 0a0a 5468 6520 7061 636b 6167 6520 7265  ..The package re
-00000380: 7175 6972 6573 2050 7974 686f 6e20 7665  quires Python ve
-00000390: 7273 696f 6e20 332e 3620 6f72 2061 626f  rsion 3.6 or abo
-000003a0: 7665 2e20 4974 2063 616e 2062 6520 696e  ve. It can be in
-000003b0: 7374 616c 6c65 6420 7769 7468 0a0a 6060  stalled with..``
-000003c0: 6062 6173 680a 7079 7468 6f6e 3320 2d6d  `bash.python3 -m
-000003d0: 2070 6970 2069 6e73 7461 6c6c 2073 6d65   pip install sme
-000003e0: 6c6c 6920 2d2d 7573 6572 0a60 6060 0a0a  lli --user.```..
-000003f0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00000400: 6e0a 0a41 2062 7269 6566 2075 7365 7220  n..A brief user 
-00000410: 6d61 6e75 616c 2063 616e 2062 6520 666f  manual can be fo
-00000420: 756e 6420 696e 2074 6865 2070 6170 6572  und in the paper
-00000430: 2063 6974 6564 2062 656c 6f77 2e0a 0a23   cited below...#
-00000440: 2320 4369 7461 7469 6f6e 0a0a 4966 2079  # Citation..If y
-00000450: 6f75 2075 7365 2060 736d 656c 6c69 6020  ou use `smelli` 
-00000460: 696e 2061 2073 6369 656e 7469 6669 6320  in a scientific 
-00000470: 7075 626c 6963 6174 696f 6e2c 2070 6c65  publication, ple
-00000480: 6173 6520 6369 7465 0a0a 3e20 204a 2e20  ase cite..>  J. 
-00000490: 4165 6269 7363 6865 722c 204a 2e20 4b75  Aebischer, J. Ku
-000004a0: 6d61 722c 2050 2e20 5374 616e 676c 2c20  mar, P. Stangl, 
-000004b0: 616e 6420 442e 204d 2e20 5374 7261 7562  and D. M. Straub
-000004c0: 0a3e 0a3e 2022 4120 476c 6f62 616c 204c  .>.> "A Global L
-000004d0: 696b 656c 6968 6f6f 6420 666f 7220 5072  ikelihood for Pr
-000004e0: 6563 6973 696f 6e20 436f 6e73 7472 6169  ecision Constrai
-000004f0: 6e74 7320 616e 6420 466c 6176 6f75 7220  nts and Flavour 
-00000500: 416e 6f6d 616c 6965 7322 0a3e 0a3e 2020  Anomalies".>.>  
-00000510: 5b61 7258 6976 3a31 3831 302e 3037 3639  [arXiv:1810.0769
-00000520: 3820 5b68 6570 2d70 685d 5d28 6874 7470  8 [hep-ph]](http
-00000530: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-00000540: 732f 3138 3130 2e30 3736 3938 290a 0a50  s/1810.07698)..P
-00000550: 6c65 6173 6520 616c 736f 2063 6974 6520  lease also cite 
-00000560: 7468 6520 7075 626c 6963 6174 696f 6e73  the publications
-00000570: 206f 6e20 5b66 6c61 7669 6f5d 2868 7474   on [flavio](htt
-00000580: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000590: 6273 2f31 3831 302e 3038 3133 3229 2061  bs/1810.08132) a
-000005a0: 6e64 205b 7769 6c73 6f6e 5d28 6874 7470  nd [wilson](http
-000005b0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000005c0: 732f 3138 3034 2e30 3530 3333 292c 2077  s/1804.05033), w
-000005d0: 6869 6368 2061 7265 2074 6865 2070 696c  hich are the pil
-000005e0: 6c61 7273 2060 736d 656c 6c69 6020 6973  lars `smelli` is
-000005f0: 2020 6275 696c 7420 6f6e 2e0a 0a23 2320    built on...## 
-00000600: 4275 6773 2061 6e64 2066 6561 7475 7265  Bugs and feature
-00000610: 2072 6571 7565 7374 730a 0a50 6c65 6173   requests..Pleas
-00000620: 6520 7375 626d 6974 2062 7567 7320 616e  e submit bugs an
-00000630: 6420 6665 6174 7572 6520 7265 7175 6573  d feature reques
-00000640: 7473 2075 7369 6e67 0a5b 4769 7468 7562  ts using.[Github
-00000650: 2773 2069 7373 7565 2073 7973 7465 6d5d  's issue system]
-00000660: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000670: 636f 6d2f 736d 656c 6c69 2f73 6d65 6c6c  com/smelli/smell
-00000680: 692f 6973 7375 6573 292e 0a0a 2323 2043  i/issues)...## C
-00000690: 6f6e 7472 6962 7574 696e 670a 0a54 6865  ontributing..The
-000006a0: 2061 696d 206f 6620 7468 6520 7061 636b   aim of the pack
-000006b0: 6167 6520 6973 2074 6f20 7072 6f76 6964  age is to provid
-000006c0: 6520 6120 6c69 6b65 6c69 686f 6f64 2069  e a likelihood i
-000006d0: 6e20 7468 650a 7370 6163 6520 6f66 2064  n the.space of d
-000006e0: 696d 656e 7369 6f6e 2d36 2053 4d45 4654  imension-6 SMEFT
-000006f0: 2057 696c 736f 6e20 636f 6566 6669 6369   Wilson coeffici
-00000700: 656e 7473 2075 7369 6e67 2061 6c6c 0a72  ents using all.r
-00000710: 656c 6576 616e 7420 6176 6169 6c61 626c  elevant availabl
-00000720: 6520 6578 7065 7269 6d65 6e74 616c 206d  e experimental m
-00000730: 6561 7375 7265 6d65 6e74 732e 2049 6620  easurements. If 
-00000740: 796f 7520 7761 6e74 0a74 6f20 636f 6e74  you want.to cont
-00000750: 7269 6275 7465 2061 6464 6974 696f 6e61  ribute additiona
-00000760: 6c20 6f62 7365 7276 6162 6c65 732c 2074  l observables, t
-00000770: 6865 2065 6173 6965 7374 2077 6179 2069  he easiest way i
-00000780: 730a 746f 2069 6d70 6c65 6d65 6e74 2074  s.to implement t
-00000790: 6865 206f 6273 6572 7661 626c 6520 696e  he observable in
-000007a0: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
-000007b0: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
-000007c0: 762d 696f 2f66 6c61 7669 6f29 2e20 4f62  v-io/flavio). Ob
-000007d0: 7365 7276 6162 6c65 730a 696d 706c 656d  servables.implem
-000007e0: 656e 7465 6420 7468 6572 6520 6361 6e20  ented there can 
-000007f0: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-00000800: 6c69 6b65 6c69 686f 6f64 2073 696d 706c  likelihood simpl
-00000810: 790a 6279 2061 6464 696e 6720 6120 636f  y.by adding a co
-00000820: 7272 6573 706f 6e64 696e 6720 656e 7472  rresponding entr
-00000830: 7920 696e 206f 6e65 206f 6620 7468 650a  y in one of the.
-00000840: 5b6f 6273 6572 7661 626c 6520 5941 4d4c  [observable YAML
-00000850: 2066 696c 6573 5d28 6874 7470 733a 2f2f   files](https://
-00000860: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
-00000870: 692f 736d 656c 6c69 2f74 7265 652f 6d61  i/smelli/tree/ma
-00000880: 7374 6572 2f73 6d65 6c6c 692f 6461 7461  ster/smelli/data
-00000890: 2f79 616d 6c29 2e0a 0a41 6c74 6572 6e61  /yaml)...Alterna
-000008a0: 7469 7665 6c79 2c20 616c 736f 206f 6273  tively, also obs
-000008b0: 6572 7661 626c 6573 2063 6f6d 7075 7465  ervables compute
-000008c0: 6420 696e 2061 6e79 206f 7468 6572 2073  d in any other s
-000008d0: 7461 6e64 616c 6f6e 6520 5079 7468 6f6e  tandalone Python
-000008e0: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
-000008f0: 696e 636f 7270 6f72 6174 6564 2069 6e20  incorporated in 
-00000900: 7072 696e 6369 706c 6520 6173 206c 6f6e  principle as lon
-00000910: 6720 6173 2069 7420 6164 6865 7265 7320  g as it adheres 
-00000920: 746f 2074 6865 205b 5743 7866 2073 7461  to the [WCxf sta
-00000930: 6e64 6172 645d 2868 7474 7073 3a2f 2f77  ndard](https://w
-00000940: 6378 662e 6769 7468 7562 2e69 6f29 2e0a  cxf.github.io)..
-00000950: 4966 2079 6f75 2077 616e 7420 746f 2066  If you want to f
-00000960: 6f6c 6c6f 7720 7468 6973 2072 6f75 7465  ollow this route
-00000970: 2c20 706c 6561 7365 206f 7065 6e20 616e  , please open an
-00000980: 205b 6973 7375 655d 2868 7474 7073 3a2f   [issue](https:/
-00000990: 2f67 6974 6875 622e 636f 6d2f 736d 656c  /github.com/smel
-000009a0: 6c69 2f73 6d65 6c6c 692f 6973 7375 6573  li/smelli/issues
-000009b0: 2920 746f 2073 7461 7274 2074 6865 2064  ) to start the d
-000009c0: 6973 6375 7373 696f 6e20 6f6e 2068 6f77  iscussion on how
-000009d0: 2074 6f20 696e 7465 6772 6174 6520 6974   to integrate it
-000009e0: 2e0a 0a23 2320 436f 6e74 7269 6275 746f  ...## Contributo
-000009f0: 7273 0a0a 496e 2061 6c70 6861 6265 7469  rs..In alphabeti
-00000a00: 6361 6c20 6f72 6465 723a 0a0a 2d20 4a61  cal order:..- Ja
-00000a10: 736f 6e20 4165 6269 7363 6865 720a 2d20  son Aebischer.- 
-00000a20: 4d61 7474 6865 7720 4b69 726b 0a2d 204a  Matthew Kirk.- J
-00000a30: 6163 6b79 204b 756d 6172 0a2d 2050 6574  acky Kumar.- Pet
-00000a40: 6572 2053 7461 6e67 6c0a 2d20 4461 7669  er Stangl.- Davi
-00000a50: 6420 4d2e 2053 7472 6175 620a 0a23 2320  d M. Straub..## 
-00000a60: 4c69 6365 6e73 650a 0a73 6d65 6c6c 6920  License..smelli 
-00000a70: 6973 2072 656c 6561 7365 6420 756e 6465  is released unde
-00000a80: 7220 7468 6520 4d49 5420 6c69 6365 6e73  r the MIT licens
-00000a90: 652e 0a                                  e..
+00000000: 5b21 5b75 6e69 7420 7465 7374 735d 2868  [![unit tests](h
+00000010: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000020: 6d2f 666c 6176 2d69 6f2f 666c 6176 696f  m/flav-io/flavio
+00000030: 2f61 6374 696f 6e73 2f77 6f72 6b66 6c6f  /actions/workflo
+00000040: 7773 2f74 6573 742e 796d 6c2f 6261 6467  ws/test.yml/badg
+00000050: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000060: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
+00000070: 692f 736d 656c 6c69 2f61 6374 696f 6e73  i/smelli/actions
+00000080: 2f77 6f72 6b66 6c6f 7773 2f74 6573 742e  /workflows/test.
+00000090: 796d 6c29 0a0a 0a0a 0a23 2073 6d65 6c6c  yml).....# smell
+000000a0: 6920 e280 9320 6120 676c 6f62 616c 206c  i ... a global l
+000000b0: 696b 656c 6968 6f6f 6420 666f 7220 7072  ikelihood for pr
+000000c0: 6563 6973 696f 6e20 636f 6e73 7472 6169  ecision constrai
+000000d0: 6e74 730a 0a60 736d 656c 6c69 6020 6973  nts..`smelli` is
+000000e0: 2061 2050 7974 686f 6e20 7061 636b 6167   a Python packag
+000000f0: 6520 7072 6f76 6964 696e 6720 6120 676c  e providing a gl
+00000100: 6f62 616c 206c 696b 656c 6968 6f6f 6420  obal likelihood 
+00000110: 6675 6e63 7469 6f6e 2069 6e20 7468 650a  function in the.
+00000120: 7370 6163 6520 6f66 2064 696d 656e 7369  space of dimensi
+00000130: 6f6e 2d73 6978 2057 696c 736f 6e20 636f  on-six Wilson co
+00000140: 6566 6669 6369 656e 7473 2069 6e20 7468  efficients in th
+00000150: 6520 5374 616e 6461 7264 204d 6f64 656c  e Standard Model
+00000160: 2045 6666 6563 7469 7665 0a46 6965 6c64   Effective.Field
+00000170: 2054 6865 6f72 7920 2853 4d45 4654 292e   Theory (SMEFT).
+00000180: 2054 6865 206c 696b 656c 6968 6f6f 6420   The likelihood 
+00000190: 696e 636c 7564 6573 2063 6f6e 7472 6962  includes contrib
+000001a0: 7574 696f 6e73 2066 726f 6d0a 7175 6172  utions from.quar
+000001b0: 6b20 616e 6420 6c65 7074 6f6e 2066 6c61  k and lepton fla
+000001c0: 766f 7572 2070 6879 7369 6373 2c20 656c  vour physics, el
+000001d0: 6563 7472 6f77 6561 6b20 7072 6563 6973  ectroweak precis
+000001e0: 696f 6e20 7465 7374 732c 2061 6e64 206f  ion tests, and o
+000001f0: 7468 6572 0a70 7265 6369 7369 6f6e 206f  ther.precision o
+00000200: 6273 6572 7661 626c 6573 2e0a 0a54 6865  bservables...The
+00000210: 2070 6163 6b61 6765 2069 7320 6261 7365   package is base
+00000220: 6420 6f6e 205b 666c 6176 696f 5d28 6874  d on [flavio](ht
+00000230: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000240: 2f66 6c61 762d 696f 2f66 6c61 7669 6f29  /flav-io/flavio)
+00000250: 2066 6f72 2074 6865 0a63 616c 6375 6c61   for the.calcula
+00000260: 7469 6f6e 206f 6620 6f62 7365 7276 6162  tion of observab
+00000270: 6c65 7320 616e 6420 7374 6174 6973 7469  les and statisti
+00000280: 6361 6c20 7472 6561 746d 656e 7420 616e  cal treatment an
+00000290: 640a 5b77 696c 736f 6e5d 2868 7474 7073  d.[wilson](https
+000002a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7769  ://github.com/wi
+000002b0: 6c73 6f6e 2d65 6674 2f77 696c 736f 6e29  lson-eft/wilson)
+000002c0: 2066 6f72 2074 6865 2072 756e 6e69 6e67   for the running
+000002d0: 2c20 7472 616e 736c 6174 696f 6e2c 0a61  , translation,.a
+000002e0: 6e64 206d 6174 6368 696e 6720 6f66 2057  nd matching of W
+000002f0: 696c 736f 6e20 636f 6566 6669 6369 656e  ilson coefficien
+00000300: 7473 2e0a 0a23 2320 496e 7374 616c 6c61  ts...## Installa
+00000310: 7469 6f6e 0a0a 5468 6520 7061 636b 6167  tion..The packag
+00000320: 6520 7265 7175 6972 6573 2050 7974 686f  e requires Pytho
+00000330: 6e20 7665 7273 696f 6e20 332e 3620 6f72  n version 3.6 or
+00000340: 2061 626f 7665 2e20 4974 2063 616e 2062   above. It can b
+00000350: 6520 696e 7374 616c 6c65 6420 7769 7468  e installed with
+00000360: 0a0a 6060 6062 6173 680a 7079 7468 6f6e  ..```bash.python
+00000370: 3320 2d6d 2070 6970 2069 6e73 7461 6c6c  3 -m pip install
+00000380: 2073 6d65 6c6c 6920 2d2d 7573 6572 0a60   smelli --user.`
+00000390: 6060 0a0a 0a23 2320 446f 6375 6d65 6e74  ``...## Document
+000003a0: 6174 696f 6e0a 0a41 2062 7269 6566 2075  ation..A brief u
+000003b0: 7365 7220 6d61 6e75 616c 2063 616e 2062  ser manual can b
+000003c0: 6520 666f 756e 6420 696e 2074 6865 2070  e found in the p
+000003d0: 6170 6572 2063 6974 6564 2062 656c 6f77  aper cited below
+000003e0: 2e0a 0a23 2320 4369 7461 7469 6f6e 0a0a  ...## Citation..
+000003f0: 4966 2079 6f75 2075 7365 2060 736d 656c  If you use `smel
+00000400: 6c69 6020 696e 2061 2073 6369 656e 7469  li` in a scienti
+00000410: 6669 6320 7075 626c 6963 6174 696f 6e2c  fic publication,
+00000420: 2070 6c65 6173 6520 6369 7465 0a0a 3e20   please cite..> 
+00000430: 204a 2e20 4165 6269 7363 6865 722c 204a   J. Aebischer, J
+00000440: 2e20 4b75 6d61 722c 2050 2e20 5374 616e  . Kumar, P. Stan
+00000450: 676c 2c20 616e 6420 442e 204d 2e20 5374  gl, and D. M. St
+00000460: 7261 7562 0a3e 0a3e 2022 4120 476c 6f62  raub.>.> "A Glob
+00000470: 616c 204c 696b 656c 6968 6f6f 6420 666f  al Likelihood fo
+00000480: 7220 5072 6563 6973 696f 6e20 436f 6e73  r Precision Cons
+00000490: 7472 6169 6e74 7320 616e 6420 466c 6176  traints and Flav
+000004a0: 6f75 7220 416e 6f6d 616c 6965 7322 0a3e  our Anomalies".>
+000004b0: 0a3e 2020 5b61 7258 6976 3a31 3831 302e  .>  [arXiv:1810.
+000004c0: 3037 3639 3820 5b68 6570 2d70 685d 5d28  07698 [hep-ph]](
+000004d0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+000004e0: 672f 6162 732f 3138 3130 2e30 3736 3938  g/abs/1810.07698
+000004f0: 290a 0a50 6c65 6173 6520 616c 736f 2063  )..Please also c
+00000500: 6974 6520 7468 6520 7075 626c 6963 6174  ite the publicat
+00000510: 696f 6e73 206f 6e20 5b66 6c61 7669 6f5d  ions on [flavio]
+00000520: 2868 7474 7073 3a2f 2f61 7278 6976 2e6f  (https://arxiv.o
+00000530: 7267 2f61 6273 2f31 3831 302e 3038 3133  rg/abs/1810.0813
+00000540: 3229 2061 6e64 205b 7769 6c73 6f6e 5d28  2) and [wilson](
+00000550: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
+00000560: 672f 6162 732f 3138 3034 2e30 3530 3333  g/abs/1804.05033
+00000570: 292c 2077 6869 6368 2061 7265 2074 6865  ), which are the
+00000580: 2070 696c 6c61 7273 2060 736d 656c 6c69   pillars `smelli
+00000590: 6020 6973 2020 6275 696c 7420 6f6e 2e0a  ` is  built on..
+000005a0: 0a23 2320 4275 6773 2061 6e64 2066 6561  .## Bugs and fea
+000005b0: 7475 7265 2072 6571 7565 7374 730a 0a50  ture requests..P
+000005c0: 6c65 6173 6520 7375 626d 6974 2062 7567  lease submit bug
+000005d0: 7320 616e 6420 6665 6174 7572 6520 7265  s and feature re
+000005e0: 7175 6573 7473 2075 7369 6e67 0a5b 4769  quests using.[Gi
+000005f0: 7468 7562 2773 2069 7373 7565 2073 7973  thub's issue sys
+00000600: 7465 6d5d 2868 7474 7073 3a2f 2f67 6974  tem](https://git
+00000610: 6875 622e 636f 6d2f 736d 656c 6c69 2f73  hub.com/smelli/s
+00000620: 6d65 6c6c 692f 6973 7375 6573 292e 0a0a  melli/issues)...
+00000630: 2323 2043 6f6e 7472 6962 7574 696e 670a  ## Contributing.
+00000640: 0a54 6865 2061 696d 206f 6620 7468 6520  .The aim of the 
+00000650: 7061 636b 6167 6520 6973 2074 6f20 7072  package is to pr
+00000660: 6f76 6964 6520 6120 6c69 6b65 6c69 686f  ovide a likeliho
+00000670: 6f64 2069 6e20 7468 650a 7370 6163 6520  od in the.space 
+00000680: 6f66 2064 696d 656e 7369 6f6e 2d36 2053  of dimension-6 S
+00000690: 4d45 4654 2057 696c 736f 6e20 636f 6566  MEFT Wilson coef
+000006a0: 6669 6369 656e 7473 2075 7369 6e67 2061  ficients using a
+000006b0: 6c6c 0a72 656c 6576 616e 7420 6176 6169  ll.relevant avai
+000006c0: 6c61 626c 6520 6578 7065 7269 6d65 6e74  lable experiment
+000006d0: 616c 206d 6561 7375 7265 6d65 6e74 732e  al measurements.
+000006e0: 2049 6620 796f 7520 7761 6e74 0a74 6f20   If you want.to 
+000006f0: 636f 6e74 7269 6275 7465 2061 6464 6974  contribute addit
+00000700: 696f 6e61 6c20 6f62 7365 7276 6162 6c65  ional observable
+00000710: 732c 2074 6865 2065 6173 6965 7374 2077  s, the easiest w
+00000720: 6179 2069 730a 746f 2069 6d70 6c65 6d65  ay is.to impleme
+00000730: 6e74 2074 6865 206f 6273 6572 7661 626c  nt the observabl
+00000740: 6520 696e 205b 666c 6176 696f 5d28 6874  e in [flavio](ht
+00000750: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000760: 2f66 6c61 762d 696f 2f66 6c61 7669 6f29  /flav-io/flavio)
+00000770: 2e20 4f62 7365 7276 6162 6c65 730a 696d  . Observables.im
+00000780: 706c 656d 656e 7465 6420 7468 6572 6520  plemented there 
+00000790: 6361 6e20 6265 2061 6464 6564 2074 6f20  can be added to 
+000007a0: 7468 6520 6c69 6b65 6c69 686f 6f64 2073  the likelihood s
+000007b0: 696d 706c 790a 6279 2061 6464 696e 6720  imply.by adding 
+000007c0: 6120 636f 7272 6573 706f 6e64 696e 6720  a corresponding 
+000007d0: 656e 7472 7920 696e 206f 6e65 206f 6620  entry in one of 
+000007e0: 7468 650a 5b6f 6273 6572 7661 626c 6520  the.[observable 
+000007f0: 5941 4d4c 2066 696c 6573 5d28 6874 7470  YAML files](http
+00000800: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000810: 6d65 6c6c 692f 736d 656c 6c69 2f74 7265  melli/smelli/tre
+00000820: 652f 6d61 7374 6572 2f73 6d65 6c6c 692f  e/master/smelli/
+00000830: 6461 7461 2f79 616d 6c29 2e0a 0a41 6c74  data/yaml)...Alt
+00000840: 6572 6e61 7469 7665 6c79 2c20 616c 736f  ernatively, also
+00000850: 206f 6273 6572 7661 626c 6573 2063 6f6d   observables com
+00000860: 7075 7465 6420 696e 2061 6e79 206f 7468  puted in any oth
+00000870: 6572 2073 7461 6e64 616c 6f6e 6520 5079  er standalone Py
+00000880: 7468 6f6e 2070 6163 6b61 6765 2063 616e  thon package can
+00000890: 2062 6520 696e 636f 7270 6f72 6174 6564   be incorporated
+000008a0: 2069 6e20 7072 696e 6369 706c 6520 6173   in principle as
+000008b0: 206c 6f6e 6720 6173 2069 7420 6164 6865   long as it adhe
+000008c0: 7265 7320 746f 2074 6865 205b 5743 7866  res to the [WCxf
+000008d0: 2073 7461 6e64 6172 645d 2868 7474 7073   standard](https
+000008e0: 3a2f 2f77 6378 662e 6769 7468 7562 2e69  ://wcxf.github.i
+000008f0: 6f29 2e0a 4966 2079 6f75 2077 616e 7420  o)..If you want 
+00000900: 746f 2066 6f6c 6c6f 7720 7468 6973 2072  to follow this r
+00000910: 6f75 7465 2c20 706c 6561 7365 206f 7065  oute, please ope
+00000920: 6e20 616e 205b 6973 7375 655d 2868 7474  n an [issue](htt
+00000930: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000940: 736d 656c 6c69 2f73 6d65 6c6c 692f 6973  smelli/smelli/is
+00000950: 7375 6573 2920 746f 2073 7461 7274 2074  sues) to start t
+00000960: 6865 2064 6973 6375 7373 696f 6e20 6f6e  he discussion on
+00000970: 2068 6f77 2074 6f20 696e 7465 6772 6174   how to integrat
+00000980: 6520 6974 2e0a 0a23 2320 436f 6e74 7269  e it...## Contri
+00000990: 6275 746f 7273 0a0a 4d61 696e 7461 696e  butors..Maintain
+000009a0: 6572 3a0a 0a2d 2050 6574 6572 2053 7461  er:..- Peter Sta
+000009b0: 6e67 6c20 2840 7065 7465 7273 7461 6e67  ngl (@peterstang
+000009c0: 6c29 0a0a 436f 6e74 7269 6275 746f 7273  l)..Contributors
+000009d0: 2028 696e 2061 6c70 6861 6265 7469 6361   (in alphabetica
+000009e0: 6c20 6f72 6465 7229 3a0a 0a2d 204a 6173  l order):..- Jas
+000009f0: 6f6e 2041 6562 6973 6368 6572 0a2d 204d  on Aebischer.- M
+00000a00: 6174 c49b 6a20 4875 6465 630a 2d20 4d61  at..j Hudec.- Ma
+00000a10: 7474 6865 7720 4b69 726b 0a2d 204a 6163  tthew Kirk.- Jac
+00000a20: 6b79 204b 756d 6172 0a2d 204e 696c 6164  ky Kumar.- Nilad
+00000a30: 7269 2053 6168 6f6f 0a2d 2041 6c65 6b73  ri Sahoo.- Aleks
+00000a40: 2053 6d6f 6c6b 6f76 69c4 8d0a 2d20 5065   Smolkovi...- Pe
+00000a50: 7465 7220 5374 616e 676c 0a2d 2044 6176  ter Stangl.- Dav
+00000a60: 6964 204d 2e20 5374 7261 7562 0a0a 2323  id M. Straub..##
+00000a70: 204c 6963 656e 7365 0a0a 736d 656c 6c69   License..smelli
+00000a80: 2069 7320 7265 6c65 6173 6564 2075 6e64   is released und
+00000a90: 6572 2074 6865 204d 4954 206c 6963 656e  er the MIT licen
+00000aa0: 7365 2e0a                                se..
```

### Comparing `smelli-2.3.2/setup.py` & `smelli-2.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,10 +27,10 @@
         'numpy>=1.16.5',
         'flavio>=' + __flavio__version__,
         'wilson',
         'pandas',
         'multipledispatch'
       ],
       extras_require={
-            'testing': ['nose'],
+            'testing': ['pytest'],
       },
       )
```

### Comparing `smelli-2.3.2/smelli/ckm.py` & `smelli-2.4.0/smelli/ckm.py`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/classes.py` & `smelli-2.4.0/smelli/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 from functools import partial
 from operator import itemgetter
 from numbers import Number
 import inspect
 from flavio.math.optimize import minimize_robust
 from smelli import _flavio_up_to_date
+from itertools import chain
 
 
 # by default, smelli uses leading log accuracy for SMEFT running!
 Wilson.set_default_option('smeft_accuracy', 'leadinglog')
 
 
 class GlobalLikelihood(object):
@@ -132,14 +133,15 @@
         self.eft = eft
         self.basis = basis or self._default_bases[self.eft]
         par_dict = par_dict or {}  # initialize empty if not given
         # take missing parameters from flavio defaults
         self.par_dict_default = flavio.default_parameters.get_central_all()
         self.par_dict_default.update(par_dict)
         self._par_dict_sm = None
+        self._observables = None
         self.fix_ckm = fix_ckm
         if self.fix_ckm:
             self._fast_likelihoods_yaml = self._fast_likelihoods_yaml_fixckm
         try:
             self._ckm_scheme = get_ckm_schemes()[ckm_scheme]
             self._ckm_scheme_name = ckm_scheme
         except:
@@ -309,14 +311,25 @@
 
     def load_exp_covariances(self, folder):
         for name, flh in self.fast_likelihoods.items():
             filename = os.path.join(folder, name + '.p')
             flh.exp_covariance.load(filename)
 
     @property
+    def observables(self):
+        if self._observables is None:
+            self._observables = set.union(*(
+                set(lh.observables) for lh in chain(
+                    self.fast_likelihoods.values(),
+                    self.likelihoods.values()
+                )
+            ))
+        return self._observables
+
+    @property
     def log_likelihood_sm(self):
         if self._log_likelihood_sm is None:
             self._log_likelihood_sm = self._log_likelihood(self.par_dict_sm, flavio.WilsonCoefficients())
         return self._log_likelihood_sm
 
     def _check_sm_cov_loaded(self):
         """Check if the SM covariances have been computed or loaded."""
@@ -755,26 +768,35 @@
     def log_likelihood(self, par_dict, w, delta):
         gp = self.gl.parameter_point(w)
         return gp.log_likelihood_global()
 
 
 class CustomLikelihood(object):
     def __init__(self, likelihood, observables):
+        if set(observables) - likelihood.observables:
+            raise ValueError(
+                'The following observables are not part of any included '
+                '(fast)likelihood and thus cannot be used in a custom '
+                'likelihood: {}.'.format(', '.join(
+                    str(obs) for obs
+                    in set(observables) - likelihood.observables
+                ))
+            )
         self.likelihood = likelihood
-        self.observables = observables
+        self.observables = set(observables)
         self.exclude_obs = self._get_exclude_obs_dict()
 
     def _get_exclude_obs_dict(self):
         """Get a dictionary with observables to be excluded from each
         (Fast)Likelihood instance."""
         exclude_obs = {}
         for lhs_or_flhs in (self.likelihood.likelihoods,
                             self.likelihood.fast_likelihoods):
             for lh_name, lh in lhs_or_flhs.items():
-                exclude_observables = set(lh.observables) - set(self.observables)
+                exclude_observables = set(lh.observables) - self.observables
                 if set(lh.observables) != exclude_observables:
                     exclude_obs[lh_name] = exclude_observables
         return exclude_obs
 
     def log_likelihood(self, par_dict, wc_obj, delta=False):
         custom_log_likelihood = 0
         for lh_name, exclude_observables in self.exclude_obs.items():
```

### Comparing `smelli-2.3.2/smelli/data/yaml/fast_likelihood_quarks.yaml` & `smelli-2.4.0/smelli/data/yaml/fast_likelihood_quarks.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -18,13 +18,17 @@
   # b->ulnu
   - observables_bulnu_lfu.yaml
   # DF=2
   - observables_df2.yaml
   # K
   - observables_k.yaml
   - observables_sulnu.yaml
+  # D
+  - observables_d.yaml
   # u->dlnu
   - observables_n.yaml
   - observables_beta.yaml
   - observables_udlnu.yaml
+  # b->dll
+  - observables_bdll.yaml
 include_measurements: !include_merge_list
   - measurements_quarks.yaml
```

### Comparing `smelli-2.3.2/smelli/data/yaml/fast_likelihood_quarks_fixckm.yaml` & `smelli-2.4.0/smelli/data/yaml/fast_likelihood_quarks_fixckm.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -18,16 +18,20 @@
   # b->ulnu
   - observables_bulnu_lfu.yaml
   # DF=2
   - observables_df2.yaml
   # K
   - observables_k.yaml
   - observables_sulnu.yaml
+  # D
+  - observables_d.yaml
   # u->dlnu
   - observables_n.yaml
   - observables_beta.yaml
   - observables_udlnu.yaml
+  # b->dll
+  - observables_bdll.yaml
   # CKM input observables
   - observables_ckm_input.yaml
 include_measurements: !include_merge_list
   - measurements_quarks.yaml
   - measurements_fixckm.yaml
```

### Comparing `smelli-2.3.2/smelli/data/yaml/measurements_quarks.yaml` & `smelli-2.4.0/smelli/data/yaml/measurements_quarks.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 - ATLAS B->K*mumu 2017 FL
 - ATLAS B->K*mumu 2017 P1
 - ATLAS B->K*mumu 2017 P4p
 - ATLAS B->K*mumu 2017 P5p
-- AS combination Bs->mumu 2021
-- CMS Bs->mumu effective lifetime 2019
+- CMS Bs->mumu effective lifetime 2022
 - LHCb Bs->mumu effective lifetime 2021
 - B->Xgamma WA 2017
 - BaBar B->Xll 2013
 - Belle B0->pitaunu 2015 total BR
 - Belle phigamma 2014
+- BESIII D+->Kenu 2017
+- BESIII D0->pienu 2015
+- BESIII D0->Kenu 2015
+- BESIII D+->pienu 2017
 - CDF B+->K*mumu 2012
 - CDF B+>Kmumu 2012
 - CDF B0->K*mumu AFB 2012
 - CDF B0->K*mumu BR 2012
 - CDF B0->K*mumu FL 2012
 - CDF B0->Kmumu 2012
 - CDF Bs->phimumu 2012
+- CLEO D->Kenu 2009
+- CLEO D->pienu 2009
 - CMS B->K*mumu 2013 combined with 2015
 - CMS B->K*mumu 2013 combined with 2015 BR
 - CMS B->K*mumu 2015 4.3-6
 - CMS B->K*mumu 2015 4.3-6 BR
 - CMS B->K*mumu 2017 P1
 - CMS B->K*mumu 2017 P5p
-- Ft(0+) Hardy/Towner 2014
+- Ft(0+) Hardy/Towner 2020
+- GSSS combination Bs->mumu 2022
 - HFAG K*gamma summer 2015
 - HFAG UT summer 2015
 - HFAG acp 2016
 - HFAG osc summer 2015
 - HFAG rad 2014
 - HFLAV D mixing 2019
-- HFLAV rad 2018
 - ISTRA+ Kl3 2003
 - K+->pinunu E949 2009
-- K+->pinunu NA62 2019
+- K+->pinunu NA62 2021
 - KL->pinunu KOTO 2018
+- KLOE-2 KS->pienu 2022
+- KLOE-2 KS->pimunu 2019
 - LHCb B+->K*mumu 2020 P 0.1-0.98
 - LHCb B+->K*mumu 2020 P 1.1-2.5
 - LHCb B+->K*mumu 2020 P 15-19
 - LHCb B+->K*mumu 2020 P 2.5-4
 - LHCb B+->K*mumu 2020 P 4-6
 - LHCb B+->K*mumu BR 2014
 - LHCb B+->Kmumu BR 2014
@@ -63,13 +70,19 @@
 - Mostovoi lambda_n 2001
 - Moulson Kl3 averages 2014
 - Neutron A parameter PERKEO II 2012
 - Neutron A parameter PERKEO III 2018
 - Neutron A parameter UCNA 2017
 - Neutron averages GACS 2018 1
 - Neutron averages GACS 2018 2
-- PDG 2015
+- PDG 2022
 - PDG 2018 Kll
+- PDG 2022 D->lnu
+- PDG 2022 D->Plnu
 - PDG epsp/eps
 - PDG kaon CPV
 - aCORN atilde_n 2017
 - nTRV R_n 2011
+- LHCb B->pimumu 2015
+- LHCb Bs->K*mumu 2018
+- Belle B+->pi+ee 2008
+- Belle B->munu 2020
```

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bctaunu_diff.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bctaunu_diff.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_atlas_p.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_atlas_p.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_br.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_br.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_cms.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_cms.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bkstarmumu_lhcb.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bkstarmumu_lhcb.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bpkstarmumu_lhcb.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bpkstarmumu_lhcb.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_bsphimumu.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_bsphimumu.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_eeww.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_eeww.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/data/yaml/observables_higgs.yaml` & `smelli-2.4.0/smelli/data/yaml/observables_higgs.yaml`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/test_ckm.py` & `smelli-2.4.0/smelli/test_ckm.py`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli/test_classes.py` & `smelli-2.4.0/smelli/test_classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,25 +40,32 @@
         ll_sm = gl.parameter_point({}, 100)
         for k, v in ll_sm.log_likelihood_dict().items():
             self.assertEqual(v, 0, msg="Failed for {}".format(k))
         # check just that this does not give an error
         ll_np = gl.parameter_point({'C9_bsmumu': -1}, 4.8)
 
     def test_incl_excl(self):
-        gl = GlobalLikelihood(eft='WET', basis='flavio', include_likelihoods=['fast_likelihood_quarks.yaml'])
+        gl = GlobalLikelihood(
+            eft='WET', basis='flavio',
+            include_likelihoods=['fast_likelihood_quarks.yaml'])
         ll = gl.parameter_point({}, 100).log_likelihood_dict()
-        self.assertSetEqual(set(ll.keys()), {'fast_likelihood_quarks.yaml', 'global'})
-        gl = GlobalLikelihood(eft='WET', basis='flavio', include_likelihoods=['likelihood_lfv.yaml'])
+        self.assertSetEqual(set(ll.keys()),
+                            {'fast_likelihood_quarks.yaml', 'global'})
+        gl = GlobalLikelihood(eft='WET', basis='flavio',
+                              include_likelihoods=['likelihood_lfv.yaml'])
         ll = gl.parameter_point({}, 100).log_likelihood_dict()
         self.assertSetEqual(set(ll.keys()), {'likelihood_lfv.yaml', 'global'})
-        gl = GlobalLikelihood(eft='WET', basis='flavio', exclude_likelihoods=['likelihood_lfv.yaml'])
+        gl = GlobalLikelihood(eft='WET', basis='flavio',
+                              exclude_likelihoods=['likelihood_lfv.yaml'])
         ll = gl.parameter_point({}, 100).log_likelihood_dict()
         self.assertNotIn('likelihood_lfv.yaml', set(ll.keys()))
-        self.assertRaises(ValueError, GlobalLikelihood, include_likelihoods=["nonexistent_likelihood.yaml"])
-        self.assertRaises(ValueError, GlobalLikelihood, exclude_likelihoods=["nonexistent_likelihood.yaml"])
+        self.assertRaises(ValueError, GlobalLikelihood,
+                          include_likelihoods=["nonexistent_likelihood.yaml"])
+        self.assertRaises(ValueError, GlobalLikelihood,
+                          exclude_likelihoods=["nonexistent_likelihood.yaml"])
 
     def test_chi2_min(self):
         gl_ewpt = GlobalLikelihood(fix_ckm=True, include_likelihoods=[
             'likelihood_ewpt.yaml',
         ])
         def wc_fct_2D_2args(S,T):
             return {
@@ -165,14 +172,23 @@
         ))
         self.assertTrue(all(
             min_data_2D_2threads['likelihood_ewpt.yaml']['coords_min']
             ==
             min_data_2D_2args['likelihood_ewpt.yaml']['coords_min']
         ))
 
+    def test_custom_likelihoods(self):
+        self.assertRaises(ValueError, GlobalLikelihood,
+                          custom_likelihoods={"with_typo": ["deltaMs"]})
+        self.assertRaises(ValueError, GlobalLikelihood,
+                          include_likelihoods=["likelihood_ewpt.yaml"],
+                          custom_likelihoods={"not_included": ["DeltaM_s"]})
+        self.assertRaises(ValueError, GlobalLikelihood,
+                          exclude_likelihoods=["likelihood_ewpt.yaml"],
+                          custom_likelihoods={"excluded": ["m_W"]})
 
 class TestGlobalLikelihoodPoint(unittest.TestCase):
 
     def test_obstable(self):
         gl = GlobalLikelihood()
         res = gl.parameter_point({'lq1_2223': 1e-8}, 91.1876)
         self.assertIsInstance(res, GlobalLikelihoodPoint)
```

### Comparing `smelli-2.3.2/smelli/util.py` & `smelli-2.4.0/smelli/util.py`

 * *Files identical despite different names*

### Comparing `smelli-2.3.2/smelli.egg-info/PKG-INFO` & `smelli-2.4.0/smelli.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 736d 656c  : 2.1.Name: smel
-00000020: 6c69 0a56 6572 7369 6f6e 3a20 322e 332e  li.Version: 2.3.
-00000030: 320a 5375 6d6d 6172 793a 2041 2050 7974  2.Summary: A Pyt
+00000020: 6c69 0a56 6572 7369 6f6e 3a20 322e 342e  li.Version: 2.4.
+00000030: 300a 5375 6d6d 6172 793a 2041 2050 7974  0.Summary: A Pyt
 00000040: 686f 6e20 7061 636b 6167 6520 7072 6f76  hon package prov
 00000050: 6964 696e 6720 6120 676c 6f62 616c 206c  iding a global l
 00000060: 696b 656c 6968 6f6f 6420 6675 6e63 7469  ikelihood functi
 00000070: 6f6e 2069 6e20 7468 6520 7370 6163 6520  on in the space 
 00000080: 6f66 2064 696d 656e 7369 6f6e 2d36 2057  of dimension-6 W
 00000090: 696c 736f 6e20 636f 6566 6669 6369 656e  ilson coefficien
 000000a0: 7473 206f 6620 7468 6520 5374 616e 6461  ts of the Standa
@@ -20,219 +20,185 @@
 00000130: 6b75 6d61 7240 756d 6f6e 7472 6561 6c2e  kumar@umontreal.
 00000140: 6361 3e2c 2050 6574 6572 2053 7461 6e67  ca>, Peter Stang
 00000150: 6c20 3c70 6574 6572 2e73 7461 6e67 6c40  l <peter.stangl@
 00000160: 6c61 7074 682e 636e 7273 2e66 723e 2c20  lapth.cnrs.fr>, 
 00000170: 4461 7669 6420 4d2e 2053 7472 6175 6220  David M. Straub 
 00000180: 3c64 6176 6964 2e73 7472 6175 6240 7475  <david.straub@tu
 00000190: 6d2e 6465 3e0a 4c69 6365 6e73 653a 204d  m.de>.License: M
-000001a0: 4954 0a44 6573 6372 6970 7469 6f6e 3a20  IT.Description: 
-000001b0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000001c0: 2f74 7261 7669 732d 6369 2e6f 7267 2f73  /travis-ci.org/s
-000001d0: 6d65 6c6c 692f 736d 656c 6c69 223e 215b  melli/smelli">![
-000001e0: 4275 696c 6420 5374 6174 7573 5d28 6874  Build Status](ht
-000001f0: 7470 733a 2f2f 7472 6176 6973 2d63 692e  tps://travis-ci.
-00000200: 6f72 672f 736d 656c 6c69 2f73 6d65 6c6c  org/smelli/smell
-00000210: 692e 7376 673f 6272 616e 6368 3d6d 6173  i.svg?branch=mas
-00000220: 7465 7229 3c2f 613e 205b 215b 436f 7665  ter)</a> [![Cove
-00000230: 7261 6765 2053 7461 7475 735d 2868 7474  rage Status](htt
-00000240: 7073 3a2f 2f63 6f76 6572 616c 6c73 2e69  ps://coveralls.i
-00000250: 6f2f 7265 706f 732f 6769 7468 7562 2f73  o/repos/github/s
-00000260: 6d65 6c6c 692f 736d 656c 6c69 2f62 6164  melli/smelli/bad
-00000270: 6765 2e73 7667 295d 2868 7474 7073 3a2f  ge.svg)](https:/
-00000280: 2f63 6f76 6572 616c 6c73 2e69 6f2f 6769  /coveralls.io/gi
-00000290: 7468 7562 2f73 6d65 6c6c 692f 736d 656c  thub/smelli/smel
-000002a0: 6c69 290a 2020 2020 2020 2020 0a20 2020  li).        .   
-000002b0: 2020 2020 2023 2073 6d65 6c6c 6920 e280       # smelli ..
-000002c0: 9320 6120 676c 6f62 616c 206c 696b 656c  . a global likel
-000002d0: 6968 6f6f 6420 666f 7220 7072 6563 6973  ihood for precis
-000002e0: 696f 6e20 636f 6e73 7472 6169 6e74 730a  ion constraints.
-000002f0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000300: 2060 736d 656c 6c69 6020 6973 2061 2050   `smelli` is a P
-00000310: 7974 686f 6e20 7061 636b 6167 6520 7072  ython package pr
-00000320: 6f76 6964 696e 6720 6120 676c 6f62 616c  oviding a global
-00000330: 206c 696b 656c 6968 6f6f 6420 6675 6e63   likelihood func
-00000340: 7469 6f6e 2069 6e20 7468 650a 2020 2020  tion in the.    
-00000350: 2020 2020 7370 6163 6520 6f66 2064 696d      space of dim
-00000360: 656e 7369 6f6e 2d73 6978 2057 696c 736f  ension-six Wilso
-00000370: 6e20 636f 6566 6669 6369 656e 7473 2069  n coefficients i
-00000380: 6e20 7468 6520 5374 616e 6461 7264 204d  n the Standard M
-00000390: 6f64 656c 2045 6666 6563 7469 7665 0a20  odel Effective. 
-000003a0: 2020 2020 2020 2046 6965 6c64 2054 6865         Field The
-000003b0: 6f72 7920 2853 4d45 4654 292e 2054 6865  ory (SMEFT). The
-000003c0: 206c 696b 656c 6968 6f6f 6420 696e 636c   likelihood incl
-000003d0: 7564 6573 2063 6f6e 7472 6962 7574 696f  udes contributio
-000003e0: 6e73 2066 726f 6d0a 2020 2020 2020 2020  ns from.        
-000003f0: 7175 6172 6b20 616e 6420 6c65 7074 6f6e  quark and lepton
-00000400: 2066 6c61 766f 7572 2070 6879 7369 6373   flavour physics
-00000410: 2c20 656c 6563 7472 6f77 6561 6b20 7072  , electroweak pr
-00000420: 6563 6973 696f 6e20 7465 7374 732c 2061  ecision tests, a
-00000430: 6e64 206f 7468 6572 0a20 2020 2020 2020  nd other.       
-00000440: 2070 7265 6369 7369 6f6e 206f 6273 6572   precision obser
-00000450: 7661 626c 6573 2e0a 2020 2020 2020 2020  vables..        
-00000460: 0a20 2020 2020 2020 2054 6865 2070 6163  .        The pac
-00000470: 6b61 6765 2069 7320 6261 7365 6420 6f6e  kage is based on
-00000480: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
-00000490: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
-000004a0: 762d 696f 2f66 6c61 7669 6f29 2066 6f72  v-io/flavio) for
-000004b0: 2074 6865 0a20 2020 2020 2020 2063 616c   the.        cal
-000004c0: 6375 6c61 7469 6f6e 206f 6620 6f62 7365  culation of obse
-000004d0: 7276 6162 6c65 7320 616e 6420 7374 6174  rvables and stat
-000004e0: 6973 7469 6361 6c20 7472 6561 746d 656e  istical treatmen
-000004f0: 7420 616e 640a 2020 2020 2020 2020 5b77  t and.        [w
-00000500: 696c 736f 6e5d 2868 7474 7073 3a2f 2f67  ilson](https://g
-00000510: 6974 6875 622e 636f 6d2f 7769 6c73 6f6e  ithub.com/wilson
-00000520: 2d65 6674 2f77 696c 736f 6e29 2066 6f72  -eft/wilson) for
-00000530: 2074 6865 2072 756e 6e69 6e67 2c20 7472   the running, tr
-00000540: 616e 736c 6174 696f 6e2c 0a20 2020 2020  anslation,.     
-00000550: 2020 2061 6e64 206d 6174 6368 696e 6720     and matching 
-00000560: 6f66 2057 696c 736f 6e20 636f 6566 6669  of Wilson coeffi
-00000570: 6369 656e 7473 2e0a 2020 2020 2020 2020  cients..        
-00000580: 0a20 2020 2020 2020 2023 2320 496e 7374  .        ## Inst
-00000590: 616c 6c61 7469 6f6e 0a20 2020 2020 2020  allation.       
-000005a0: 200a 2020 2020 2020 2020 5468 6520 7061   .        The pa
-000005b0: 636b 6167 6520 7265 7175 6972 6573 2050  ckage requires P
-000005c0: 7974 686f 6e20 7665 7273 696f 6e20 332e  ython version 3.
-000005d0: 3620 6f72 2061 626f 7665 2e20 4974 2063  6 or above. It c
-000005e0: 616e 2062 6520 696e 7374 616c 6c65 6420  an be installed 
-000005f0: 7769 7468 0a20 2020 2020 2020 200a 2020  with.        .  
-00000600: 2020 2020 2020 6060 6062 6173 680a 2020        ```bash.  
-00000610: 2020 2020 2020 7079 7468 6f6e 3320 2d6d        python3 -m
-00000620: 2070 6970 2069 6e73 7461 6c6c 2073 6d65   pip install sme
-00000630: 6c6c 6920 2d2d 7573 6572 0a20 2020 2020  lli --user.     
-00000640: 2020 2060 6060 0a20 2020 2020 2020 200a     ```.        .
-00000650: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000660: 2023 2320 446f 6375 6d65 6e74 6174 696f   ## Documentatio
-00000670: 6e0a 2020 2020 2020 2020 0a20 2020 2020  n.        .     
-00000680: 2020 2041 2062 7269 6566 2075 7365 7220     A brief user 
-00000690: 6d61 6e75 616c 2063 616e 2062 6520 666f  manual can be fo
-000006a0: 756e 6420 696e 2074 6865 2070 6170 6572  und in the paper
-000006b0: 2063 6974 6564 2062 656c 6f77 2e0a 2020   cited below..  
-000006c0: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-000006d0: 2320 4369 7461 7469 6f6e 0a20 2020 2020  # Citation.     
-000006e0: 2020 200a 2020 2020 2020 2020 4966 2079     .        If y
-000006f0: 6f75 2075 7365 2060 736d 656c 6c69 6020  ou use `smelli` 
-00000700: 696e 2061 2073 6369 656e 7469 6669 6320  in a scientific 
-00000710: 7075 626c 6963 6174 696f 6e2c 2070 6c65  publication, ple
-00000720: 6173 6520 6369 7465 0a20 2020 2020 2020  ase cite.       
-00000730: 200a 2020 2020 2020 2020 3e20 204a 2e20   .        >  J. 
-00000740: 4165 6269 7363 6865 722c 204a 2e20 4b75  Aebischer, J. Ku
-00000750: 6d61 722c 2050 2e20 5374 616e 676c 2c20  mar, P. Stangl, 
-00000760: 616e 6420 442e 204d 2e20 5374 7261 7562  and D. M. Straub
-00000770: 0a20 2020 2020 2020 203e 0a20 2020 2020  .        >.     
-00000780: 2020 203e 2022 4120 476c 6f62 616c 204c     > "A Global L
-00000790: 696b 656c 6968 6f6f 6420 666f 7220 5072  ikelihood for Pr
-000007a0: 6563 6973 696f 6e20 436f 6e73 7472 6169  ecision Constrai
-000007b0: 6e74 7320 616e 6420 466c 6176 6f75 7220  nts and Flavour 
-000007c0: 416e 6f6d 616c 6965 7322 0a20 2020 2020  Anomalies".     
-000007d0: 2020 203e 0a20 2020 2020 2020 203e 2020     >.        >  
-000007e0: 5b61 7258 6976 3a31 3831 302e 3037 3639  [arXiv:1810.0769
-000007f0: 3820 5b68 6570 2d70 685d 5d28 6874 7470  8 [hep-ph]](http
-00000800: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-00000810: 732f 3138 3130 2e30 3736 3938 290a 2020  s/1810.07698).  
-00000820: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
-00000830: 6c65 6173 6520 616c 736f 2063 6974 6520  lease also cite 
-00000840: 7468 6520 7075 626c 6963 6174 696f 6e73  the publications
-00000850: 206f 6e20 5b66 6c61 7669 6f5d 2868 7474   on [flavio](htt
-00000860: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000870: 6273 2f31 3831 302e 3038 3133 3229 2061  bs/1810.08132) a
-00000880: 6e64 205b 7769 6c73 6f6e 5d28 6874 7470  nd [wilson](http
-00000890: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000008a0: 732f 3138 3034 2e30 3530 3333 292c 2077  s/1804.05033), w
-000008b0: 6869 6368 2061 7265 2074 6865 2070 696c  hich are the pil
-000008c0: 6c61 7273 2060 736d 656c 6c69 6020 6973  lars `smelli` is
-000008d0: 2020 6275 696c 7420 6f6e 2e0a 2020 2020    built on..    
-000008e0: 2020 2020 0a20 2020 2020 2020 2023 2320      .        ## 
-000008f0: 4275 6773 2061 6e64 2066 6561 7475 7265  Bugs and feature
-00000900: 2072 6571 7565 7374 730a 2020 2020 2020   requests.      
-00000910: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
-00000920: 6520 7375 626d 6974 2062 7567 7320 616e  e submit bugs an
-00000930: 6420 6665 6174 7572 6520 7265 7175 6573  d feature reques
-00000940: 7473 2075 7369 6e67 0a20 2020 2020 2020  ts using.       
-00000950: 205b 4769 7468 7562 2773 2069 7373 7565   [Github's issue
-00000960: 2073 7973 7465 6d5d 2868 7474 7073 3a2f   system](https:/
-00000970: 2f67 6974 6875 622e 636f 6d2f 736d 656c  /github.com/smel
-00000980: 6c69 2f73 6d65 6c6c 692f 6973 7375 6573  li/smelli/issues
-00000990: 292e 0a20 2020 2020 2020 200a 2020 2020  )..        .    
-000009a0: 2020 2020 2323 2043 6f6e 7472 6962 7574      ## Contribut
-000009b0: 696e 670a 2020 2020 2020 2020 0a20 2020  ing.        .   
-000009c0: 2020 2020 2054 6865 2061 696d 206f 6620       The aim of 
-000009d0: 7468 6520 7061 636b 6167 6520 6973 2074  the package is t
-000009e0: 6f20 7072 6f76 6964 6520 6120 6c69 6b65  o provide a like
-000009f0: 6c69 686f 6f64 2069 6e20 7468 650a 2020  lihood in the.  
-00000a00: 2020 2020 2020 7370 6163 6520 6f66 2064        space of d
-00000a10: 696d 656e 7369 6f6e 2d36 2053 4d45 4654  imension-6 SMEFT
-00000a20: 2057 696c 736f 6e20 636f 6566 6669 6369   Wilson coeffici
-00000a30: 656e 7473 2075 7369 6e67 2061 6c6c 0a20  ents using all. 
-00000a40: 2020 2020 2020 2072 656c 6576 616e 7420         relevant 
-00000a50: 6176 6169 6c61 626c 6520 6578 7065 7269  available experi
-00000a60: 6d65 6e74 616c 206d 6561 7375 7265 6d65  mental measureme
-00000a70: 6e74 732e 2049 6620 796f 7520 7761 6e74  nts. If you want
-00000a80: 0a20 2020 2020 2020 2074 6f20 636f 6e74  .        to cont
-00000a90: 7269 6275 7465 2061 6464 6974 696f 6e61  ribute additiona
-00000aa0: 6c20 6f62 7365 7276 6162 6c65 732c 2074  l observables, t
-00000ab0: 6865 2065 6173 6965 7374 2077 6179 2069  he easiest way i
-00000ac0: 730a 2020 2020 2020 2020 746f 2069 6d70  s.        to imp
-00000ad0: 6c65 6d65 6e74 2074 6865 206f 6273 6572  lement the obser
-00000ae0: 7661 626c 6520 696e 205b 666c 6176 696f  vable in [flavio
-00000af0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00000b00: 2e63 6f6d 2f66 6c61 762d 696f 2f66 6c61  .com/flav-io/fla
-00000b10: 7669 6f29 2e20 4f62 7365 7276 6162 6c65  vio). Observable
-00000b20: 730a 2020 2020 2020 2020 696d 706c 656d  s.        implem
-00000b30: 656e 7465 6420 7468 6572 6520 6361 6e20  ented there can 
-00000b40: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
-00000b50: 6c69 6b65 6c69 686f 6f64 2073 696d 706c  likelihood simpl
-00000b60: 790a 2020 2020 2020 2020 6279 2061 6464  y.        by add
-00000b70: 696e 6720 6120 636f 7272 6573 706f 6e64  ing a correspond
-00000b80: 696e 6720 656e 7472 7920 696e 206f 6e65  ing entry in one
-00000b90: 206f 6620 7468 650a 2020 2020 2020 2020   of the.        
-00000ba0: 5b6f 6273 6572 7661 626c 6520 5941 4d4c  [observable YAML
-00000bb0: 2066 696c 6573 5d28 6874 7470 733a 2f2f   files](https://
-00000bc0: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
-00000bd0: 692f 736d 656c 6c69 2f74 7265 652f 6d61  i/smelli/tree/ma
-00000be0: 7374 6572 2f73 6d65 6c6c 692f 6461 7461  ster/smelli/data
-00000bf0: 2f79 616d 6c29 2e0a 2020 2020 2020 2020  /yaml)..        
-00000c00: 0a20 2020 2020 2020 2041 6c74 6572 6e61  .        Alterna
-00000c10: 7469 7665 6c79 2c20 616c 736f 206f 6273  tively, also obs
-00000c20: 6572 7661 626c 6573 2063 6f6d 7075 7465  ervables compute
-00000c30: 6420 696e 2061 6e79 206f 7468 6572 2073  d in any other s
-00000c40: 7461 6e64 616c 6f6e 6520 5079 7468 6f6e  tandalone Python
-00000c50: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
-00000c60: 696e 636f 7270 6f72 6174 6564 2069 6e20  incorporated in 
-00000c70: 7072 696e 6369 706c 6520 6173 206c 6f6e  principle as lon
-00000c80: 6720 6173 2069 7420 6164 6865 7265 7320  g as it adheres 
-00000c90: 746f 2074 6865 205b 5743 7866 2073 7461  to the [WCxf sta
-00000ca0: 6e64 6172 645d 2868 7474 7073 3a2f 2f77  ndard](https://w
-00000cb0: 6378 662e 6769 7468 7562 2e69 6f29 2e0a  cxf.github.io)..
-00000cc0: 2020 2020 2020 2020 4966 2079 6f75 2077          If you w
-00000cd0: 616e 7420 746f 2066 6f6c 6c6f 7720 7468  ant to follow th
-00000ce0: 6973 2072 6f75 7465 2c20 706c 6561 7365  is route, please
-00000cf0: 206f 7065 6e20 616e 205b 6973 7375 655d   open an [issue]
-00000d00: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d10: 636f 6d2f 736d 656c 6c69 2f73 6d65 6c6c  com/smelli/smell
-00000d20: 692f 6973 7375 6573 2920 746f 2073 7461  i/issues) to sta
-00000d30: 7274 2074 6865 2064 6973 6375 7373 696f  rt the discussio
-00000d40: 6e20 6f6e 2068 6f77 2074 6f20 696e 7465  n on how to inte
-00000d50: 6772 6174 6520 6974 2e0a 2020 2020 2020  grate it..      
-00000d60: 2020 0a20 2020 2020 2020 2023 2320 436f    .        ## Co
-00000d70: 6e74 7269 6275 746f 7273 0a20 2020 2020  ntributors.     
-00000d80: 2020 200a 2020 2020 2020 2020 496e 2061     .        In a
-00000d90: 6c70 6861 6265 7469 6361 6c20 6f72 6465  lphabetical orde
-00000da0: 723a 0a20 2020 2020 2020 200a 2020 2020  r:.        .    
-00000db0: 2020 2020 2d20 4a61 736f 6e20 4165 6269      - Jason Aebi
-00000dc0: 7363 6865 720a 2020 2020 2020 2020 2d20  scher.        - 
-00000dd0: 4d61 7474 6865 7720 4b69 726b 0a20 2020  Matthew Kirk.   
-00000de0: 2020 2020 202d 204a 6163 6b79 204b 756d       - Jacky Kum
-00000df0: 6172 0a20 2020 2020 2020 202d 2050 6574  ar.        - Pet
-00000e00: 6572 2053 7461 6e67 6c0a 2020 2020 2020  er Stangl.      
-00000e10: 2020 2d20 4461 7669 6420 4d2e 2053 7472    - David M. Str
-00000e20: 6175 620a 2020 2020 2020 2020 0a20 2020  aub.        .   
-00000e30: 2020 2020 2023 2320 4c69 6365 6e73 650a       ## License.
-00000e40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00000e50: 2073 6d65 6c6c 6920 6973 2072 656c 6561   smelli is relea
-00000e60: 7365 6420 756e 6465 7220 7468 6520 4d49  sed under the MI
-00000e70: 5420 6c69 6365 6e73 652e 0a20 2020 2020  T license..     
-00000e80: 2020 200a 506c 6174 666f 726d 3a20 554e     .Platform: UN
-00000e90: 4b4e 4f57 4e0a 4465 7363 7269 7074 696f  KNOWN.Descriptio
-00000ea0: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000eb0: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
-00000ec0: 6f76 6964 6573 2d45 7874 7261 3a20 7465  ovides-Extra: te
-00000ed0: 7374 696e 670a                           sting.
+000001a0: 4954 0a50 6c61 7466 6f72 6d3a 2055 4e4b  IT.Platform: UNK
+000001b0: 4e4f 574e 0a44 6573 6372 6970 7469 6f6e  NOWN.Description
+000001c0: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
+000001d0: 6578 742f 6d61 726b 646f 776e 0a50 726f  ext/markdown.Pro
+000001e0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
+000001f0: 7469 6e67 0a4c 6963 656e 7365 2d46 696c  ting.License-Fil
+00000200: 653a 204c 4943 454e 5345 0a0a 5b21 5b75  e: LICENSE..[![u
+00000210: 6e69 7420 7465 7374 735d 2868 7474 7073  nit tests](https
+00000220: 3a2f 2f67 6974 6875 622e 636f 6d2f 666c  ://github.com/fl
+00000230: 6176 2d69 6f2f 666c 6176 696f 2f61 6374  av-io/flavio/act
+00000240: 696f 6e73 2f77 6f72 6b66 6c6f 7773 2f74  ions/workflows/t
+00000250: 6573 742e 796d 6c2f 6261 6467 652e 7376  est.yml/badge.sv
+00000260: 6729 5d28 6874 7470 733a 2f2f 6769 7468  g)](https://gith
+00000270: 7562 2e63 6f6d 2f73 6d65 6c6c 692f 736d  ub.com/smelli/sm
+00000280: 656c 6c69 2f61 6374 696f 6e73 2f77 6f72  elli/actions/wor
+00000290: 6b66 6c6f 7773 2f74 6573 742e 796d 6c29  kflows/test.yml)
+000002a0: 0a0a 0a0a 0a23 2073 6d65 6c6c 6920 e280  .....# smelli ..
+000002b0: 9320 6120 676c 6f62 616c 206c 696b 656c  . a global likel
+000002c0: 6968 6f6f 6420 666f 7220 7072 6563 6973  ihood for precis
+000002d0: 696f 6e20 636f 6e73 7472 6169 6e74 730a  ion constraints.
+000002e0: 0a60 736d 656c 6c69 6020 6973 2061 2050  .`smelli` is a P
+000002f0: 7974 686f 6e20 7061 636b 6167 6520 7072  ython package pr
+00000300: 6f76 6964 696e 6720 6120 676c 6f62 616c  oviding a global
+00000310: 206c 696b 656c 6968 6f6f 6420 6675 6e63   likelihood func
+00000320: 7469 6f6e 2069 6e20 7468 650a 7370 6163  tion in the.spac
+00000330: 6520 6f66 2064 696d 656e 7369 6f6e 2d73  e of dimension-s
+00000340: 6978 2057 696c 736f 6e20 636f 6566 6669  ix Wilson coeffi
+00000350: 6369 656e 7473 2069 6e20 7468 6520 5374  cients in the St
+00000360: 616e 6461 7264 204d 6f64 656c 2045 6666  andard Model Eff
+00000370: 6563 7469 7665 0a46 6965 6c64 2054 6865  ective.Field The
+00000380: 6f72 7920 2853 4d45 4654 292e 2054 6865  ory (SMEFT). The
+00000390: 206c 696b 656c 6968 6f6f 6420 696e 636c   likelihood incl
+000003a0: 7564 6573 2063 6f6e 7472 6962 7574 696f  udes contributio
+000003b0: 6e73 2066 726f 6d0a 7175 6172 6b20 616e  ns from.quark an
+000003c0: 6420 6c65 7074 6f6e 2066 6c61 766f 7572  d lepton flavour
+000003d0: 2070 6879 7369 6373 2c20 656c 6563 7472   physics, electr
+000003e0: 6f77 6561 6b20 7072 6563 6973 696f 6e20  oweak precision 
+000003f0: 7465 7374 732c 2061 6e64 206f 7468 6572  tests, and other
+00000400: 0a70 7265 6369 7369 6f6e 206f 6273 6572  .precision obser
+00000410: 7661 626c 6573 2e0a 0a54 6865 2070 6163  vables...The pac
+00000420: 6b61 6765 2069 7320 6261 7365 6420 6f6e  kage is based on
+00000430: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
+00000440: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
+00000450: 762d 696f 2f66 6c61 7669 6f29 2066 6f72  v-io/flavio) for
+00000460: 2074 6865 0a63 616c 6375 6c61 7469 6f6e   the.calculation
+00000470: 206f 6620 6f62 7365 7276 6162 6c65 7320   of observables 
+00000480: 616e 6420 7374 6174 6973 7469 6361 6c20  and statistical 
+00000490: 7472 6561 746d 656e 7420 616e 640a 5b77  treatment and.[w
+000004a0: 696c 736f 6e5d 2868 7474 7073 3a2f 2f67  ilson](https://g
+000004b0: 6974 6875 622e 636f 6d2f 7769 6c73 6f6e  ithub.com/wilson
+000004c0: 2d65 6674 2f77 696c 736f 6e29 2066 6f72  -eft/wilson) for
+000004d0: 2074 6865 2072 756e 6e69 6e67 2c20 7472   the running, tr
+000004e0: 616e 736c 6174 696f 6e2c 0a61 6e64 206d  anslation,.and m
+000004f0: 6174 6368 696e 6720 6f66 2057 696c 736f  atching of Wilso
+00000500: 6e20 636f 6566 6669 6369 656e 7473 2e0a  n coefficients..
+00000510: 0a23 2320 496e 7374 616c 6c61 7469 6f6e  .## Installation
+00000520: 0a0a 5468 6520 7061 636b 6167 6520 7265  ..The package re
+00000530: 7175 6972 6573 2050 7974 686f 6e20 7665  quires Python ve
+00000540: 7273 696f 6e20 332e 3620 6f72 2061 626f  rsion 3.6 or abo
+00000550: 7665 2e20 4974 2063 616e 2062 6520 696e  ve. It can be in
+00000560: 7374 616c 6c65 6420 7769 7468 0a0a 6060  stalled with..``
+00000570: 6062 6173 680a 7079 7468 6f6e 3320 2d6d  `bash.python3 -m
+00000580: 2070 6970 2069 6e73 7461 6c6c 2073 6d65   pip install sme
+00000590: 6c6c 6920 2d2d 7573 6572 0a60 6060 0a0a  lli --user.```..
+000005a0: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
+000005b0: 6e0a 0a41 2062 7269 6566 2075 7365 7220  n..A brief user 
+000005c0: 6d61 6e75 616c 2063 616e 2062 6520 666f  manual can be fo
+000005d0: 756e 6420 696e 2074 6865 2070 6170 6572  und in the paper
+000005e0: 2063 6974 6564 2062 656c 6f77 2e0a 0a23   cited below...#
+000005f0: 2320 4369 7461 7469 6f6e 0a0a 4966 2079  # Citation..If y
+00000600: 6f75 2075 7365 2060 736d 656c 6c69 6020  ou use `smelli` 
+00000610: 696e 2061 2073 6369 656e 7469 6669 6320  in a scientific 
+00000620: 7075 626c 6963 6174 696f 6e2c 2070 6c65  publication, ple
+00000630: 6173 6520 6369 7465 0a0a 3e20 204a 2e20  ase cite..>  J. 
+00000640: 4165 6269 7363 6865 722c 204a 2e20 4b75  Aebischer, J. Ku
+00000650: 6d61 722c 2050 2e20 5374 616e 676c 2c20  mar, P. Stangl, 
+00000660: 616e 6420 442e 204d 2e20 5374 7261 7562  and D. M. Straub
+00000670: 0a3e 0a3e 2022 4120 476c 6f62 616c 204c  .>.> "A Global L
+00000680: 696b 656c 6968 6f6f 6420 666f 7220 5072  ikelihood for Pr
+00000690: 6563 6973 696f 6e20 436f 6e73 7472 6169  ecision Constrai
+000006a0: 6e74 7320 616e 6420 466c 6176 6f75 7220  nts and Flavour 
+000006b0: 416e 6f6d 616c 6965 7322 0a3e 0a3e 2020  Anomalies".>.>  
+000006c0: 5b61 7258 6976 3a31 3831 302e 3037 3639  [arXiv:1810.0769
+000006d0: 3820 5b68 6570 2d70 685d 5d28 6874 7470  8 [hep-ph]](http
+000006e0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000006f0: 732f 3138 3130 2e30 3736 3938 290a 0a50  s/1810.07698)..P
+00000700: 6c65 6173 6520 616c 736f 2063 6974 6520  lease also cite 
+00000710: 7468 6520 7075 626c 6963 6174 696f 6e73  the publications
+00000720: 206f 6e20 5b66 6c61 7669 6f5d 2868 7474   on [flavio](htt
+00000730: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000740: 6273 2f31 3831 302e 3038 3133 3229 2061  bs/1810.08132) a
+00000750: 6e64 205b 7769 6c73 6f6e 5d28 6874 7470  nd [wilson](http
+00000760: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00000770: 732f 3138 3034 2e30 3530 3333 292c 2077  s/1804.05033), w
+00000780: 6869 6368 2061 7265 2074 6865 2070 696c  hich are the pil
+00000790: 6c61 7273 2060 736d 656c 6c69 6020 6973  lars `smelli` is
+000007a0: 2020 6275 696c 7420 6f6e 2e0a 0a23 2320    built on...## 
+000007b0: 4275 6773 2061 6e64 2066 6561 7475 7265  Bugs and feature
+000007c0: 2072 6571 7565 7374 730a 0a50 6c65 6173   requests..Pleas
+000007d0: 6520 7375 626d 6974 2062 7567 7320 616e  e submit bugs an
+000007e0: 6420 6665 6174 7572 6520 7265 7175 6573  d feature reques
+000007f0: 7473 2075 7369 6e67 0a5b 4769 7468 7562  ts using.[Github
+00000800: 2773 2069 7373 7565 2073 7973 7465 6d5d  's issue system]
+00000810: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000820: 636f 6d2f 736d 656c 6c69 2f73 6d65 6c6c  com/smelli/smell
+00000830: 692f 6973 7375 6573 292e 0a0a 2323 2043  i/issues)...## C
+00000840: 6f6e 7472 6962 7574 696e 670a 0a54 6865  ontributing..The
+00000850: 2061 696d 206f 6620 7468 6520 7061 636b   aim of the pack
+00000860: 6167 6520 6973 2074 6f20 7072 6f76 6964  age is to provid
+00000870: 6520 6120 6c69 6b65 6c69 686f 6f64 2069  e a likelihood i
+00000880: 6e20 7468 650a 7370 6163 6520 6f66 2064  n the.space of d
+00000890: 696d 656e 7369 6f6e 2d36 2053 4d45 4654  imension-6 SMEFT
+000008a0: 2057 696c 736f 6e20 636f 6566 6669 6369   Wilson coeffici
+000008b0: 656e 7473 2075 7369 6e67 2061 6c6c 0a72  ents using all.r
+000008c0: 656c 6576 616e 7420 6176 6169 6c61 626c  elevant availabl
+000008d0: 6520 6578 7065 7269 6d65 6e74 616c 206d  e experimental m
+000008e0: 6561 7375 7265 6d65 6e74 732e 2049 6620  easurements. If 
+000008f0: 796f 7520 7761 6e74 0a74 6f20 636f 6e74  you want.to cont
+00000900: 7269 6275 7465 2061 6464 6974 696f 6e61  ribute additiona
+00000910: 6c20 6f62 7365 7276 6162 6c65 732c 2074  l observables, t
+00000920: 6865 2065 6173 6965 7374 2077 6179 2069  he easiest way i
+00000930: 730a 746f 2069 6d70 6c65 6d65 6e74 2074  s.to implement t
+00000940: 6865 206f 6273 6572 7661 626c 6520 696e  he observable in
+00000950: 205b 666c 6176 696f 5d28 6874 7470 733a   [flavio](https:
+00000960: 2f2f 6769 7468 7562 2e63 6f6d 2f66 6c61  //github.com/fla
+00000970: 762d 696f 2f66 6c61 7669 6f29 2e20 4f62  v-io/flavio). Ob
+00000980: 7365 7276 6162 6c65 730a 696d 706c 656d  servables.implem
+00000990: 656e 7465 6420 7468 6572 6520 6361 6e20  ented there can 
+000009a0: 6265 2061 6464 6564 2074 6f20 7468 6520  be added to the 
+000009b0: 6c69 6b65 6c69 686f 6f64 2073 696d 706c  likelihood simpl
+000009c0: 790a 6279 2061 6464 696e 6720 6120 636f  y.by adding a co
+000009d0: 7272 6573 706f 6e64 696e 6720 656e 7472  rresponding entr
+000009e0: 7920 696e 206f 6e65 206f 6620 7468 650a  y in one of the.
+000009f0: 5b6f 6273 6572 7661 626c 6520 5941 4d4c  [observable YAML
+00000a00: 2066 696c 6573 5d28 6874 7470 733a 2f2f   files](https://
+00000a10: 6769 7468 7562 2e63 6f6d 2f73 6d65 6c6c  github.com/smell
+00000a20: 692f 736d 656c 6c69 2f74 7265 652f 6d61  i/smelli/tree/ma
+00000a30: 7374 6572 2f73 6d65 6c6c 692f 6461 7461  ster/smelli/data
+00000a40: 2f79 616d 6c29 2e0a 0a41 6c74 6572 6e61  /yaml)...Alterna
+00000a50: 7469 7665 6c79 2c20 616c 736f 206f 6273  tively, also obs
+00000a60: 6572 7661 626c 6573 2063 6f6d 7075 7465  ervables compute
+00000a70: 6420 696e 2061 6e79 206f 7468 6572 2073  d in any other s
+00000a80: 7461 6e64 616c 6f6e 6520 5079 7468 6f6e  tandalone Python
+00000a90: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
+00000aa0: 696e 636f 7270 6f72 6174 6564 2069 6e20  incorporated in 
+00000ab0: 7072 696e 6369 706c 6520 6173 206c 6f6e  principle as lon
+00000ac0: 6720 6173 2069 7420 6164 6865 7265 7320  g as it adheres 
+00000ad0: 746f 2074 6865 205b 5743 7866 2073 7461  to the [WCxf sta
+00000ae0: 6e64 6172 645d 2868 7474 7073 3a2f 2f77  ndard](https://w
+00000af0: 6378 662e 6769 7468 7562 2e69 6f29 2e0a  cxf.github.io)..
+00000b00: 4966 2079 6f75 2077 616e 7420 746f 2066  If you want to f
+00000b10: 6f6c 6c6f 7720 7468 6973 2072 6f75 7465  ollow this route
+00000b20: 2c20 706c 6561 7365 206f 7065 6e20 616e  , please open an
+00000b30: 205b 6973 7375 655d 2868 7474 7073 3a2f   [issue](https:/
+00000b40: 2f67 6974 6875 622e 636f 6d2f 736d 656c  /github.com/smel
+00000b50: 6c69 2f73 6d65 6c6c 692f 6973 7375 6573  li/smelli/issues
+00000b60: 2920 746f 2073 7461 7274 2074 6865 2064  ) to start the d
+00000b70: 6973 6375 7373 696f 6e20 6f6e 2068 6f77  iscussion on how
+00000b80: 2074 6f20 696e 7465 6772 6174 6520 6974   to integrate it
+00000b90: 2e0a 0a23 2320 436f 6e74 7269 6275 746f  ...## Contributo
+00000ba0: 7273 0a0a 4d61 696e 7461 696e 6572 3a0a  rs..Maintainer:.
+00000bb0: 0a2d 2050 6574 6572 2053 7461 6e67 6c20  .- Peter Stangl 
+00000bc0: 2840 7065 7465 7273 7461 6e67 6c29 0a0a  (@peterstangl)..
+00000bd0: 436f 6e74 7269 6275 746f 7273 2028 696e  Contributors (in
+00000be0: 2061 6c70 6861 6265 7469 6361 6c20 6f72   alphabetical or
+00000bf0: 6465 7229 3a0a 0a2d 204a 6173 6f6e 2041  der):..- Jason A
+00000c00: 6562 6973 6368 6572 0a2d 204d 6174 c49b  ebischer.- Mat..
+00000c10: 6a20 4875 6465 630a 2d20 4d61 7474 6865  j Hudec.- Matthe
+00000c20: 7720 4b69 726b 0a2d 204a 6163 6b79 204b  w Kirk.- Jacky K
+00000c30: 756d 6172 0a2d 204e 696c 6164 7269 2053  umar.- Niladri S
+00000c40: 6168 6f6f 0a2d 2041 6c65 6b73 2053 6d6f  ahoo.- Aleks Smo
+00000c50: 6c6b 6f76 69c4 8d0a 2d20 5065 7465 7220  lkovi...- Peter 
+00000c60: 5374 616e 676c 0a2d 2044 6176 6964 204d  Stangl.- David M
+00000c70: 2e20 5374 7261 7562 0a0a 2323 204c 6963  . Straub..## Lic
+00000c80: 656e 7365 0a0a 736d 656c 6c69 2069 7320  ense..smelli is 
+00000c90: 7265 6c65 6173 6564 2075 6e64 6572 2074  released under t
+00000ca0: 6865 204d 4954 206c 6963 656e 7365 2e0a  he MIT license..
+00000cb0: 0a0a                                     ..
```

### Comparing `smelli-2.3.2/smelli.egg-info/SOURCES.txt` & `smelli-2.4.0/smelli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-.gitignore
-.travis.yml
 LICENSE
 MANIFEST.in
 README.md
-deploy.sh
 setup.py
 smelli/__init__.py
 smelli/_version.py
 smelli/ckm.py
 smelli/classes.py
 smelli/test_ckm.py
 smelli/test_classes.py
@@ -18,15 +15,14 @@
 smelli.egg-info/dependency_links.txt
 smelli.egg-info/requires.txt
 smelli.egg-info/top_level.txt
 smelli/data/cache/fast_likelihood_leptons.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
 smelli/data/cache/fast_likelihood_leptons.yaml_fix_ckm.p
 smelli/data/cache/fast_likelihood_quarks.yaml_CKMSchemeRmuBtaunuBxlnuDeltaM.p
 smelli/data/cache/fast_likelihood_quarks_fixckm.yaml_fix_ckm.p
-smelli/data/cache/save_covariances.py
 smelli/data/test/wcxf.yaml
 smelli/data/yaml/fast_likelihood_leptons.yaml
 smelli/data/yaml/fast_likelihood_quarks.yaml
 smelli/data/yaml/fast_likelihood_quarks_fixckm.yaml
 smelli/data/yaml/likelihood_bcpv.yaml
 smelli/data/yaml/likelihood_bqnunu.yaml
 smelli/data/yaml/likelihood_eeww.yaml
@@ -48,17 +44,17 @@
 smelli/data/yaml/measurements_leptons.yaml
 smelli/data/yaml/measurements_lfu_fccc.yaml
 smelli/data/yaml/measurements_lfu_fcnc.yaml
 smelli/data/yaml/measurements_lfv.yaml
 smelli/data/yaml/measurements_quarks.yaml
 smelli/data/yaml/measurements_rd_rds.yaml
 smelli/data/yaml/measurements_zlfv.yaml
-smelli/data/yaml/observables_bclnu_lfu.yaml
 smelli/data/yaml/observables_bctaunu_diff.yaml
 smelli/data/yaml/observables_bctaunu_other.yaml
+smelli/data/yaml/observables_bdll.yaml
 smelli/data/yaml/observables_beta.yaml
 smelli/data/yaml/observables_bkstaree_lhcb.yaml
 smelli/data/yaml/observables_bkstarll_lfu.yaml
 smelli/data/yaml/observables_bkstarmumu_atlas_p.yaml
 smelli/data/yaml/observables_bkstarmumu_br.yaml
 smelli/data/yaml/observables_bkstarmumu_cdf.yaml
 smelli/data/yaml/observables_bkstarmumu_cms.yaml
@@ -68,16 +64,18 @@
 smelli/data/yaml/observables_bpkstarmumu_lhcb.yaml
 smelli/data/yaml/observables_bqnunu.yaml
 smelli/data/yaml/observables_bqtautau.yaml
 smelli/data/yaml/observables_bsee.yaml
 smelli/data/yaml/observables_bsgamma.yaml
 smelli/data/yaml/observables_bsmumu.yaml
 smelli/data/yaml/observables_bsphimumu.yaml
+smelli/data/yaml/observables_buenu_lfu.yaml
 smelli/data/yaml/observables_bulnu_lfu.yaml
 smelli/data/yaml/observables_ckm_input.yaml
+smelli/data/yaml/observables_d.yaml
 smelli/data/yaml/observables_df2.yaml
 smelli/data/yaml/observables_eeww.yaml
 smelli/data/yaml/observables_ewpt.yaml
 smelli/data/yaml/observables_g-2.yaml
 smelli/data/yaml/observables_higgs.yaml
 smelli/data/yaml/observables_k.yaml
 smelli/data/yaml/observables_klfu.yaml
@@ -92,9 +90,8 @@
 smelli/data/yaml/observables_rkstar.yaml
 smelli/data/yaml/observables_sulnu.yaml
 smelli/data/yaml/observables_taucc.yaml
 smelli/data/yaml/observables_udlnu.yaml
 smelli/data/yaml/observables_udlnu_lfu.yaml
 smelli/data/yaml/observables_xsee.yaml
 smelli/data/yaml/observables_zlfv.yaml
-smelli/data/yaml/par_ckm_CKMSchemeRmuBtaunuBxlnuDeltaM.yaml
-smelli/data/yaml/update_ckm.py
+smelli/data/yaml/par_ckm_CKMSchemeRmuBtaunuBxlnuDeltaM.yaml
```

