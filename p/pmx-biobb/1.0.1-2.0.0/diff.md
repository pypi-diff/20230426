# Comparing `tmp/pmx_biobb-1.0.1.tar.gz` & `tmp/pmx_biobb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pmx_biobb-1.0.1.tar", last modified: Mon Sep 28 10:03:50 2020, max compression
+gzip compressed data, was "dist/pmx_biobb-2.0.0.tar", last modified: Wed Apr 26 11:39:39 2023, max compression
```

## Comparing `pmx_biobb-1.0.1.tar` & `pmx_biobb-2.0.0.tar`

### file list

```diff
@@ -1,619 +1,318 @@
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/
--rw-r--r--   0 pau        (501) staff       (20)     7651 2020-09-27 11:11:55.000000 pmx_biobb-1.0.1/LICENSE
--rw-r--r--   0 pau        (501) staff       (20)       95 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/MANIFEST.in
--rw-r--r--   0 pau        (501) staff       (20)     3111 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)     2087 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/README.rst
--rw-r--r--   0 pau        (501) staff       (20)      194 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/setup.cfg
--rw-r--r--   0 pau        (501) staff       (20)     2142 2020-09-28 10:00:45.000000 pmx_biobb-1.0.1/setup.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/
--rw-r--r--   0 pau        (501) staff       (20)     2261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/__init__.py
--rw-r--r--   0 pau        (501) staff       (20)      496 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/_version.py
--rw-r--r--   0 pau        (501) staff       (20)    80539 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/alchemy.py
--rw-r--r--   0 pau        (501) staff       (20)    12683 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/analysis.py
--rw-r--r--   0 pau        (501) staff       (20)    15974 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/atom.py
--rw-r--r--   0 pau        (501) staff       (20)    14221 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/atomselection.py
--rw-r--r--   0 pau        (501) staff       (20)    11726 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/builder.py
--rw-r--r--   0 pau        (501) staff       (20)    34297 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/chain.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx/data/
--rw-r--r--   0 pau        (501) staff       (20)   233765 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/aminoacids.pkl
--rw-r--r--   0 pau        (501) staff       (20) 17363760 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/bbdep.pkl
--rw-r--r--   0 pau        (501) staff       (20)     1786 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/blosum62_new.mat
--rw-r--r--   0 pau        (501) staff       (20)   144604 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/bp.pkl
--rw-r--r--   0 pau        (501) staff       (20)   149219 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/bp_amber.pkl
--rw-r--r--   0 pau        (501) staff       (20)   148935 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/bp_charmm.pkl
--rw-r--r--   0 pau        (501) staff       (20)   210364 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/ffamber99sb.rtp
--rw-r--r--   0 pau        (501) staff       (20)    39498 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/ffamber99sbbon.itp
--rw-r--r--   0 pau        (501) staff       (20)     5732 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/ffamber99sbnb.itp
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)      661 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
--rw-r--r--   0 pau        (501) staff       (20)    12694 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
--rw-r--r--   0 pau        (501) staff       (20)     9997 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8884 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      849 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    80500 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5339 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    66560 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     8192 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)       79 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      947 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3882 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  3071584 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1260735 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    21524 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2589 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5335 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      130 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    45478 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7972 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      722 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129919 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2589 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4978 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7476 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      709 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129937 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     9997 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9416 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    99627 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4652 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    36127 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     6772 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      704 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      951 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  3290968 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1389335 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       84 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2060 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8026 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1519 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      181 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    44420 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     6253 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)    13027 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    37937 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)      244 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1660 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9612 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    88617 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    74128 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    47717 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)   144554 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     2792 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)     1208 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2882 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)        0 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
--rw-r--r--   0 pau        (501) staff       (20)    48593 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
--rw-r--r--   0 pau        (501) staff       (20)       70 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  2828420 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1165390 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      164 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1884 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      126 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)     9712 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      910 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      916 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1369 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1419 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1576 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     2237 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      915 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
--rw-r--r--   0 pau        (501) staff       (20)      306 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    24002 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    82367 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)  1123865 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)  1614095 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7941 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      435 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2734 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     2079 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       92 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
--rw-r--r--   0 pau        (501) staff       (20)     1134 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8979 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1397 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      198 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
--rw-r--r--   0 pau        (501) staff       (20)  1130785 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5220 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
--rw-r--r--   0 pau        (501) staff       (20)       92 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  3015999 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1267062 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   283035 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   123173 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1339 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
--rw-r--r--   0 pau        (501) staff       (20)      619 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      625 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1026 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1242 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      221 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3940 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/elements.dat
--rw-r--r--   0 pau        (501) staff       (20)        9 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb-c.tdb
--rw-r--r--   0 pau        (501) staff       (20)        9 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb-n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     7223 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb.atp
--rw-r--r--   0 pau        (501) staff       (20)    14479 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1013 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb.itp
--rw-r--r--   0 pau        (501) staff       (20)  5011072 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1492892 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sb.rtp
--rw-r--r--   0 pau        (501) staff       (20)    39431 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sbbon.itp
--rw-r--r--   0 pau        (501) staff       (20)    10006 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ffamber99sbnb.itp
--rw-r--r--   0 pau        (501) staff       (20)     5360 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)    10612 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/residuetypes.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)     1357 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      343 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)   106028 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/tip3p.gro
--rw-r--r--   0 pau        (501) staff       (20)      638 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)      656 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/vdwradii.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/data/mutff/xlateat.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2593 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9416 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101867 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4826 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7013 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      668 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      951 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sb-star-ildn-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)      661 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.am
--rw-r--r--   0 pau        (501) staff       (20)    12642 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/Makefile.in
--rw-r--r--   0 pau        (501) staff       (20)     2591 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8884 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      877 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    80505 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4826 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29931 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      522 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dummies.atp.save
--rw-r--r--   0 pau        (501) staff       (20)     1624 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/dummies_nonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    32696 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7013 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      726 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      947 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1948 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3883 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)     6624 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/list.dat
--rw-r--r--   0 pau        (501) staff       (20)  2607852 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1065143 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30276 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/amber99sbmut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       84 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2060 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8123 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1519 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      181 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    44527 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     6253 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)    13369 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    37939 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)      244 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1660 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9612 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    88617 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    74254 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffnabonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    47717 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)   144264 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     2800 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)     1208 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2882 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)        0 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/lipids.hdb
--rw-r--r--   0 pau        (501) staff       (20)    48593 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/lipids.rtp
--rw-r--r--   0 pau        (501) staff       (20)       70 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  2548759 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1044644 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      164 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)      261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     1884 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      265 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      126 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)     9712 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      910 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      916 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1369 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1419 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1576 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     2237 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      915 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/tips3p.itp
--rw-r--r--   0 pau        (501) staff       (20)      306 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm22starmut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)       92 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)      808 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     3326 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1028 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      120 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    27458 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     4758 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4603 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    41515 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)    90492 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    38702 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/ffnabonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    32806 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/ffnanonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    49793 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      294 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      575 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2567 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     1319 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/gromacs_c27_ions.itp
--rw-r--r--   0 pau        (501) staff       (20)     1767 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       70 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/mutres.arn
--rw-r--r--   0 pau        (501) staff       (20)  2556763 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1069116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      553 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      559 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      925 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1109 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      804 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/tips3p.itp
--rw-r--r--   0 pau        (501) staff       (20)      244 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)      262 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/charmm36mut.ff/watermodels.itp
--rw-r--r--   0 pau        (501) staff       (20)     3940 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/elements.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2012 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/1propanol.itp
--rw-r--r--   0 pau        (501) staff       (20)     1837 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     3736 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1274 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      120 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)    44642 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5449 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     1438 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/atomname2type.n2t
--rw-r--r--   0 pau        (501) staff       (20)    39621 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    38196 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/backup_atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    52104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/dummies.dat
--rw-r--r--   0 pau        (501) staff       (20)     1461 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/ethanol.itp
--rw-r--r--   0 pau        (501) staff       (20)   220780 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)    67018 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)       33 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      882 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     4479 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     2024 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)      868 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/methanol.itp
--rw-r--r--   0 pau        (501) staff       (20)  2827396 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1273343 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)      561 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      567 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      636 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1112 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1434 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)      173 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/oplsaamut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     9412 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/residuetypes.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)      343 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)      656 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/vdwradii.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45/xlateat.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:49.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    21524 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)     2589 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     5335 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      130 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    45478 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7972 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      677 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129919 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)     2589 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.arn
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     9412 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.hdb
--rw-r--r--   0 pau        (501) staff       (20)       10 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      903 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.r2b
--rw-r--r--   0 pau        (501) staff       (20)   101863 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5207 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/aminoacids.vsd
--rw-r--r--   0 pau        (501) staff       (20)     4978 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    36227 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_ffbonded_for_ildn_test.itp
--rw-r--r--   0 pau        (501) staff       (20)  1202088 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/backup_mutres
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/correct_ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.arn
--rw-r--r--   0 pau        (501) staff       (20)     3104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    29892 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    10830 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffberger.itp
--rw-r--r--   0 pau        (501) staff       (20)    36132 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7476 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)      673 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      974 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     1949 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/gbsa.itp
--rw-r--r--   0 pau        (501) staff       (20)     3886 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)  2805564 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres.mtp
--rw-r--r--   0 pau        (501) staff       (20)  1181333 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres.rtp
--rw-r--r--   0 pau        (501) staff       (20)   300774 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   129937 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)    16346 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer.itp
--rw-r--r--   0 pau        (501) staff       (20)    18595 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/popc_AmbBer_posre.itp
--rw-r--r--   0 pau        (501) staff       (20)      116 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.arn
--rw-r--r--   0 pau        (501) staff       (20)     4104 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.hdb
--rw-r--r--   0 pau        (501) staff       (20)      145 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.r2b
--rw-r--r--   0 pau        (501) staff       (20)    30277 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/rna.rtp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      746 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)      802 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1261 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1317 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip4pew.itp
--rw-r--r--   0 pau        (501) staff       (20)     1870 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/tip5p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1250 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/urea.itp
--rw-r--r--   0 pau        (501) staff       (20)      214 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/amber99sb-star-ildn-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3873 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/atommass.dat
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/
--rw-r--r--   0 pau        (501) staff       (20)    23195 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/atomtypes.atp
--rw-r--r--   0 pau        (501) staff       (20)    82367 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/cmap.itp
--rw-r--r--   0 pau        (501) staff       (20)    25243 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/dna.rtp_backup
--rw-r--r--   0 pau        (501) staff       (20)  1123867 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/ffbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)  1611878 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/ffnonbonded.itp
--rw-r--r--   0 pau        (501) staff       (20)     7960 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/forcefield.doc
--rw-r--r--   0 pau        (501) staff       (20)      435 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/forcefield.itp
--rw-r--r--   0 pau        (501) staff       (20)     2734 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/gb.itp
--rw-r--r--   0 pau        (501) staff       (20)     2079 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/ions.itp
--rw-r--r--   0 pau        (501) staff       (20)       92 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.arn
--rw-r--r--   0 pau        (501) staff       (20)     1134 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.c.tdb
--rw-r--r--   0 pau        (501) staff       (20)     8889 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.hdb
--rw-r--r--   0 pau        (501) staff       (20)     1397 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.n.tdb
--rw-r--r--   0 pau        (501) staff       (20)      198 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.r2b
--rw-r--r--   0 pau        (501) staff       (20)  1131001 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.rtp
--rw-r--r--   0 pau        (501) staff       (20)     5220 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/merged.vsd
--rw-r--r--   0 pau        (501) staff       (20)   283035 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.mtp
--rw-r--r--   0 pau        (501) staff       (20)   123173 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/mutres_dna.rtp
--rw-r--r--   0 pau        (501) staff       (20)     1339 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/nbfix.itp
--rw-r--r--   0 pau        (501) staff       (20)      619 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spc.itp
--rw-r--r--   0 pau        (501) staff       (20)      625 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/spce.itp
--rw-r--r--   0 pau        (501) staff       (20)     1026 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip3p.itp
--rw-r--r--   0 pau        (501) staff       (20)     1242 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/tip4p.itp
--rw-r--r--   0 pau        (501) staff       (20)      221 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/charmm36m-mut.ff/watermodels.dat
--rw-r--r--   0 pau        (501) staff       (20)     3940 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/elements.dat
--rw-r--r--   0 pau        (501) staff       (20)     9892 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/residuetypes.dat
--rw-r--r--   0 pau        (501) staff       (20)    29266 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/spc216.gro
--rw-r--r--   0 pau        (501) staff       (20)      343 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/specbond.dat
--rw-r--r--   0 pau        (501) staff       (20)      656 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/vdwradii.dat
--rw-r--r--   0 pau        (501) staff       (20)      447 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/mutff45dna/xlateat.dat
--rw-r--r--   0 pau        (501) staff       (20)    70529 2020-09-27 11:16:14.000000 pmx_biobb-1.0.1/src/pmx/data/rna.pkl
--rw-r--r--   0 pau        (501) staff       (20)    35229 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/estimators.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx/extensions/
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/
--rw-r--r--   0 pau        (501) staff       (20)    13896 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/Energy.c
--rw-r--r--   0 pau        (501) staff       (20)    15145 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/Geometry.c
--rw-r--r--   0 pau        (501) staff       (20)    20514 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/Geometry.h
--rw-r--r--   0 pau        (501) staff       (20)     2086 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/cpp_test.cpp
--rw-r--r--   0 pau        (501) staff       (20)     3939 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/init.c
--rw-r--r--   0 pau        (501) staff       (20)     4662 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/pmx.h
--rw-r--r--   0 pau        (501) staff       (20)    17556 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/pmx/wrap_Geometry.c
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/
--rw-r--r--   0 pau        (501) staff       (20)     8847 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/trr2xtc.c
--rw-r--r--   0 pau        (501) staff       (20)    64408 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile.c
--rw-r--r--   0 pau        (501) staff       (20)    23730 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile.h
--rw-r--r--   0 pau        (501) staff       (20)    13474 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c
--rw-r--r--   0 pau        (501) staff       (20)    14744 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_trr.c
--rw-r--r--   0 pau        (501) staff       (20)     2364 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_trr.h
--rw-r--r--   0 pau        (501) staff       (20)     3629 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c
--rw-r--r--   0 pau        (501) staff       (20)     2255 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h
--rw-r--r--   0 pau        (501) staff       (20)    29075 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/ffparser.py
--rw-r--r--   0 pau        (501) staff       (20)    92246 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/forcefield.py
--rw-r--r--   0 pau        (501) staff       (20)     7685 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/geometry.py
--rw-r--r--   0 pau        (501) staff       (20)     8701 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/gmx.py
--rw-r--r--   0 pau        (501) staff       (20)   123096 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/library.py
--rw-r--r--   0 pau        (501) staff       (20)    43826 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/model.py
--rw-r--r--   0 pau        (501) staff       (20)    28167 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/molecule.py
--rw-r--r--   0 pau        (501) staff       (20)     7345 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/mutdb.py
--rw-r--r--   0 pau        (501) staff       (20)     8874 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/ndx.py
--rw-r--r--   0 pau        (501) staff       (20)    16599 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/options.py
--rw-r--r--   0 pau        (501) staff       (20)     5036 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/parser.py
--rw-r--r--   0 pau        (501) staff       (20)    11783 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/rotamer.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx/scripts/
--rw-r--r--   0 pau        (501) staff       (20)        0 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/__init__.py
--rwxr-xr-x   0 pau        (501) staff       (20)    32128 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/analyze_dhdl.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2629 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/cli.py
--rwxr-xr-x   0 pau        (501) staff       (20)    73999 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/generate_hybrid_residue.py
--rwxr-xr-x   0 pau        (501) staff       (20)     6946 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/generate_hybrid_topology.py
--rwxr-xr-x   0 pau        (501) staff       (20)     2705 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/make_double_box.py
--rw-r--r--   0 pau        (501) staff       (20)    19970 2020-09-28 09:57:58.000000 pmx_biobb-1.0.1/src/pmx/scripts/md_setup.py
--rwxr-xr-x   0 pau        (501) staff       (20)    23029 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/mutate.py
--rw-r--r--   0 pau        (501) staff       (20)     7819 2020-09-28 09:54:14.000000 pmx_biobb-1.0.1/src/pmx/scripts/prepare_crooks_runs.py
--rwxr-xr-x   0 pau        (501) staff       (20)     1475 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/set_gmxlib.py
--rw-r--r--   0 pau        (501) staff       (20)    17636 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/scripts/setup_abfe.py
--rw-r--r--   0 pau        (501) staff       (20)    13621 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/utils.py
--rw-r--r--   0 pau        (501) staff       (20)     9906 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/xdrfile.py
--rw-r--r--   0 pau        (501) staff       (20)     1784 2020-09-27 11:15:45.000000 pmx_biobb-1.0.1/src/pmx/xtc.py
-drwxr-xr-x   0 pau        (501) staff       (20)        0 2020-09-28 10:03:50.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/
--rw-r--r--   0 pau        (501) staff       (20)     3111 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/PKG-INFO
--rw-r--r--   0 pau        (501) staff       (20)    30202 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/SOURCES.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/dependency_links.txt
--rw-r--r--   0 pau        (501) staff       (20)       53 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/entry_points.txt
--rw-r--r--   0 pau        (501) staff       (20)        1 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/not-zip-safe
--rw-r--r--   0 pau        (501) staff       (20)       30 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/requires.txt
--rw-r--r--   0 pau        (501) staff       (20)        4 2020-09-28 10:03:48.000000 pmx_biobb-1.0.1/src/pmx_biobb.egg-info/top_level.txt
--rw-r--r--   0 pau        (501) staff       (20)    68835 2020-09-28 10:02:25.000000 pmx_biobb-1.0.1/versioneer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/
+-rw-r--r--   0 pau        (501) staff       (20)     7651 2023-04-25 13:43:32.000000 pmx_biobb-2.0.0/LICENSE
+-rw-r--r--   0 pau        (501) staff       (20)       95 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/MANIFEST.in
+-rw-r--r--   0 pau        (501) staff       (20)     2860 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 14:02:40.000000 pmx_biobb-2.0.0/README.rst
+-rw-r--r--   0 pau        (501) staff       (20)      194 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/setup.cfg
+-rw-r--r--   0 pau        (501) staff       (20)     2183 2023-04-25 13:59:12.000000 pmx_biobb-2.0.0/setup.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)     2261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)      459 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/_version.py
+-rw-r--r--   0 pau        (501) staff       (20)    80750 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/alchemy.py
+-rw-r--r--   0 pau        (501) staff       (20)    12908 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/analysis.py
+-rw-r--r--   0 pau        (501) staff       (20)    15992 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/atom.py
+-rw-r--r--   0 pau        (501) staff       (20)    14221 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/atomselection.py
+-rw-r--r--   0 pau        (501) staff       (20)    13429 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/builder.py
+-rw-r--r--   0 pau        (501) staff       (20)    34519 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/chain.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/
+-rw-r--r--   0 pau        (501) staff       (20)   233765 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/aminoacids.pkl
+-rw-r--r--   0 pau        (501) staff       (20) 17363760 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/bbdep.pkl
+-rw-r--r--   0 pau        (501) staff       (20)     1786 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/blosum62_new.mat
+-rw-r--r--   0 pau        (501) staff       (20)   144604 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/bp.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   149219 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/bp_amber.pkl
+-rw-r--r--   0 pau        (501) staff       (20)   148935 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/bp_charmm.pkl
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)      661 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am
+-rw-r--r--   0 pau        (501) staff       (20)    12694 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in
+-rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8884 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      849 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    80500 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     5339 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    66560 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     8192 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)       79 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      947 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3882 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  3071584 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1260735 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    21524 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     5335 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      130 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)    45478 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7972 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      722 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129919 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)     2589 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9412 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   101863 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     4978 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    36227 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1202088 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    10830 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp
+-rw-r--r--   0 pau        (501) staff       (20)    36132 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7476 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      709 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      974 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1949 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  2805564 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1181333 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   300774 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   129937 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    16346 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp
+-rw-r--r--   0 pau        (501) staff       (20)    18595 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)     9997 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9416 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)       10 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      903 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)   104467 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5207 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)     4652 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     3104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    29892 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    36127 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     6772 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)      704 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      951 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1948 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp
+-rw-r--r--   0 pau        (501) staff       (20)     3886 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)  3290968 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1389335 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      116 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)     4104 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      145 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    30277 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      746 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)      802 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1317 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1870 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1250 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp
+-rw-r--r--   0 pau        (501) staff       (20)      214 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)     3873 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/atommass.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)       84 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.arn
+-rw-r--r--   0 pau        (501) staff       (20)     2060 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8026 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)     1519 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      181 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.r2b
+-rw-r--r--   0 pau        (501) staff       (20)    44420 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     6253 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd
+-rw-r--r--   0 pau        (501) staff       (20)    13027 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    37937 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp
+-rw-r--r--   0 pau        (501) staff       (20)      244 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1660 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     9612 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)    88617 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)    74128 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)    47717 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)   144554 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2792 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)     1208 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2882 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1767 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/lipids.hdb
+-rw-r--r--   0 pau        (501) staff       (20)    48593 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp
+-rw-r--r--   0 pau        (501) staff       (20)       70 2023-04-25 13:50:06.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/mutres.arn
+-rw-r--r--   0 pau        (501) staff       (20)  2828420 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1165390 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      164 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.arn
+-rw-r--r--   0 pau        (501) staff       (20)      261 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     1884 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb
+-rw-r--r--   0 pau        (501) staff       (20)      265 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      126 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.r2b
+-rw-r--r--   0 pau        (501) staff       (20)     9712 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)      910 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      916 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1369 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1419 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1576 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2237 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      915 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      306 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/watermodels.dat
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/
+-rw-r--r--   0 pau        (501) staff       (20)    24002 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp
+-rw-r--r--   0 pau        (501) staff       (20)    82367 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1123865 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)  1614095 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp
+-rw-r--r--   0 pau        (501) staff       (20)     7941 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc
+-rw-r--r--   0 pau        (501) staff       (20)      435 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2734 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp
+-rw-r--r--   0 pau        (501) staff       (20)     2079 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.arn
+-rw-r--r--   0 pau        (501) staff       (20)     1134 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb
+-rw-r--r--   0 pau        (501) staff       (20)     8979 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb
+-rw-r--r--   0 pau        (501) staff       (20)     1397 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb
+-rw-r--r--   0 pau        (501) staff       (20)      198 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.r2b
+-rw-r--r--   0 pau        (501) staff       (20)  1133668 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     5220 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd
+-rw-r--r--   0 pau        (501) staff       (20)       92 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres.arn
+-rw-r--r--   0 pau        (501) staff       (20)  3015999 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp
+-rw-r--r--   0 pau        (501) staff       (20)  1267062 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp
+-rw-r--r--   0 pau        (501) staff       (20)   283035 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp
+-rw-r--r--   0 pau        (501) staff       (20)   123173 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp
+-rw-r--r--   0 pau        (501) staff       (20)     1339 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp
+-rw-r--r--   0 pau        (501) staff       (20)      619 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp
+-rw-r--r--   0 pau        (501) staff       (20)      625 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1026 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp
+-rw-r--r--   0 pau        (501) staff       (20)     1242 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp
+-rw-r--r--   0 pau        (501) staff       (20)      221 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/watermodels.dat
+-rw-r--r--   0 pau        (501) staff       (20)     3940 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/elements.dat
+-rw-r--r--   0 pau        (501) staff       (20)    10624 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/residuetypes.dat
+-rw-r--r--   0 pau        (501) staff       (20)    29266 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/spc216.gro
+-rw-r--r--   0 pau        (501) staff       (20)      343 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/specbond.dat
+-rw-r--r--   0 pau        (501) staff       (20)      848 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/vdwradii.dat
+-rw-r--r--   0 pau        (501) staff       (20)      447 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/mutff/xlateat.dat
+-rw-r--r--   0 pau        (501) staff       (20)    70529 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/data/rna.pkl
+-rw-r--r--   0 pau        (501) staff       (20)    36875 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/estimators.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/extensions/
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/
+-rw-r--r--   0 pau        (501) staff       (20)    13896 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/Energy.c
+-rw-r--r--   0 pau        (501) staff       (20)    15145 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/Geometry.c
+-rw-r--r--   0 pau        (501) staff       (20)    20514 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/Geometry.h
+-rw-r--r--   0 pau        (501) staff       (20)     2086 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/cpp_test.cpp
+-rw-r--r--   0 pau        (501) staff       (20)     3939 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/init.c
+-rw-r--r--   0 pau        (501) staff       (20)     4662 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/pmx.h
+-rw-r--r--   0 pau        (501) staff       (20)    17556 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/pmx/wrap_Geometry.c
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/
+-rw-r--r--   0 pau        (501) staff       (20)     8847 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/trr2xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)    64408 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile.c
+-rw-r--r--   0 pau        (501) staff       (20)    23730 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile.h
+-rw-r--r--   0 pau        (501) staff       (20)    13474 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_c_test.c
+-rw-r--r--   0 pau        (501) staff       (20)    14744 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_trr.c
+-rw-r--r--   0 pau        (501) staff       (20)     2364 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_trr.h
+-rw-r--r--   0 pau        (501) staff       (20)     3629 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_xtc.c
+-rw-r--r--   0 pau        (501) staff       (20)     2255 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_xtc.h
+-rw-r--r--   0 pau        (501) staff       (20)    29075 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/ffparser.py
+-rw-r--r--   0 pau        (501) staff       (20)    97348 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/forcefield.py
+-rw-r--r--   0 pau        (501) staff       (20)     7685 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/geometry.py
+-rw-r--r--   0 pau        (501) staff       (20)     8707 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/gmx.py
+-rw-r--r--   0 pau        (501) staff       (20)     6179 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/jobscript.py
+-rw-r--r--   0 pau        (501) staff       (20)   123096 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/library.py
+-rw-r--r--   0 pau        (501) staff       (20)   117960 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/ligand_alchemy.py
+-rw-r--r--   0 pau        (501) staff       (20)    46038 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/model.py
+-rw-r--r--   0 pau        (501) staff       (20)    28167 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/molecule.py
+-rw-r--r--   0 pau        (501) staff       (20)     7345 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/mutdb.py
+-rw-r--r--   0 pau        (501) staff       (20)     8874 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/ndx.py
+-rw-r--r--   0 pau        (501) staff       (20)    16599 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/options.py
+-rw-r--r--   0 pau        (501) staff       (20)     5036 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/parser.py
+-rw-r--r--   0 pau        (501) staff       (20)    21628 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/rosetta.py
+-rw-r--r--   0 pau        (501) staff       (20)    15211 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/rosetta_analyze.py
+-rw-r--r--   0 pau        (501) staff       (20)    11783 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/rotamer.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/scripts/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/__init__.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    32251 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/analyze_dhdl.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    19768 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/atomMapping.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    11939 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/build_cyclic_top.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2988 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/cli.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    73999 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/generate_hybrid_residue.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     6989 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/generate_hybrid_topology.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx/scripts/icolos_entrypoints/
+-rw-r--r--   0 pau        (501) staff       (20)        0 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/icolos_entrypoints/__init__.py
+-rw-r--r--   0 pau        (501) staff       (20)     7137 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/icolos_entrypoints/assemble_systems.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    12867 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/ligandHybrid.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     2705 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/make_double_box.py
+-rw-r--r--   0 pau        (501) staff       (20)    19943 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/md_setup.py
+-rwxr-xr-x   0 pau        (501) staff       (20)    23029 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/mutate.py
+-rw-r--r--   0 pau        (501) staff       (20)     7795 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/prepare_crooks_runs.py
+-rwxr-xr-x   0 pau        (501) staff       (20)     1475 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/set_gmxlib.py
+-rw-r--r--   0 pau        (501) staff       (20)    17636 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/scripts/setup_abfe.py
+-rw-r--r--   0 pau        (501) staff       (20)    15258 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/utils.py
+-rw-r--r--   0 pau        (501) staff       (20)    11331 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/xdrfile.py
+-rw-r--r--   0 pau        (501) staff       (20)     1784 2023-04-25 13:50:07.000000 pmx_biobb-2.0.0/src/pmx/xtc.py
+drwxr-xr-x   0 pau        (501) staff       (20)        0 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/
+-rw-r--r--   0 pau        (501) staff       (20)     2860 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/PKG-INFO
+-rw-r--r--   0 pau        (501) staff       (20)    14242 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/SOURCES.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/dependency_links.txt
+-rw-r--r--   0 pau        (501) staff       (20)       53 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/entry_points.txt
+-rw-r--r--   0 pau        (501) staff       (20)        1 2023-04-26 11:15:51.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/not-zip-safe
+-rw-r--r--   0 pau        (501) staff       (20)       30 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/requires.txt
+-rw-r--r--   0 pau        (501) staff       (20)        4 2023-04-26 11:39:39.000000 pmx_biobb-2.0.0/src/pmx_biobb.egg-info/top_level.txt
+-rw-r--r--   0 pau        (501) staff       (20)    65993 2023-04-26 11:38:14.000000 pmx_biobb-2.0.0/versioneer.py
```

### Comparing `pmx_biobb-1.0.1/LICENSE` & `pmx_biobb-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/PKG-INFO` & `pmx_biobb-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pmx_biobb
-Version: 1.0.1
+Version: 2.0.0
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger
 Author-email: seeliger.biosoft@gmail.de
 License: GPL 3
-Description: pmx: alchemistry in gromacs
-        ===========================
-        
-        |build| |cov|
-        
-        **Warning:** this is a development version of ``pmx``, it is not stable or reliable yet. You are welcome to
-        try/test it and provide feedback, but use at your own risk. The current stable version of ``pmx`` can
-        be found in the master branch: https://github.com/deGrootLab/pmx
-        
-        ``pmx`` is a python library that allows users to setup and analyse molecular
-        dynamics simulations with the `Gromacs <http://gromacs.org>`_ package.
-        Among its main features are the setup and analysis of alchemical free energy
-        calculations for protein, nucleic acid, and small molecule mutations.
-        
-        https://degrootlab.github.io/pmx/
-        
-        Citations
-        ---------
-        ``pmx`` is a research software. If you make use of it in scientific publications, please cite the following papers::
-        
-            @article{Gapsys2015pmx,
-                title = {pmx: Automated protein structure and topology
-                generation for alchemical perturbations},
-                author = {Gapsys, Vytautas and Michielssens, Servaas
-                and Seeliger, Daniel and de Groot, Bert L.},
-                journal = {Journal of Computational Chemistry},
-                volume = {36},
-                number = {5},
-                pages = {348--354},
-                year = {2015},
-                doi = {10.1002/jcc.23804}
-            }
-        
-            @article{Seeliger2010pmx,
-                title = {Protein Thermostability Calculations Using
-                Alchemical Free Energy Simulations},
-                author = {Seeliger, Daniel and de Groot, Bert L.},
-                journal = {Biophysical Journal},
-                volume = {98},
-                number = {10},
-                pages = {2309--2316},
-                year = {2010},
-                doi = {10.1016/j.bpj.2010.01.051}
-            }
-        
-        
-        License
-        -------
-        ``pmx`` is licensed under the GNU Lesser General Public License v3.0 (LGPL v3).
-        
-        .. |build| image:: https://travis-ci.org/deGrootLab/pmx.svg?branch=master
-            :alt: Build Status
-            :scale: 100%
-            :target: https://travis-ci.org/deGrootLab/pmx
-        
-        .. |cov| image:: https://codecov.io/gh/deGrootLab/pmx/branch/develop/graph/badge.svg
-            :alt: Code coverage
-            :scale: 100%
-            :target: https://codecov.io/gh/deGrootLab/pmx
-        
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.7.*
+Requires-Python: >=3.7
+License-File: LICENSE
+
+pmx: alchemistry in gromacs
+===========================
+
+|build| |cov|
+
+**PMX_BIOBB DISTRIBUTION VERSION**: 2.0.0
+**Based on the PMX Icolos branch commit**: https://github.com/deGrootLab/pmx/commit/80f4f8a1552c37e3d926f950d91db77cd4dea9cf
+
+**Warning:** this is a development version of ``pmx``, it is not stable or reliable yet. You are welcome to
+try/test it and provide feedback, but use at your own risk. The current stable version of ``pmx`` can
+be found in the master branch: https://github.com/deGrootLab/pmx
+
+``pmx`` is a python library that allows users to setup and analyse molecular
+dynamics simulations with the `Gromacs <http://gromacs.org>`_ package.
+Among its main features are the setup and analysis of alchemical free energy
+calculations for protein, nucleic acid, and small molecule mutations.
+
+https://degrootlab.github.io/pmx/
+
+Citations
+---------
+``pmx`` is a research software. If you make use of it in scientific publications, please cite the following papers::
+
+    @article{Gapsys2015pmx,
+        title = {pmx: Automated protein structure and topology
+        generation for alchemical perturbations},
+        author = {Gapsys, Vytautas and Michielssens, Servaas
+        and Seeliger, Daniel and de Groot, Bert L.},
+        journal = {Journal of Computational Chemistry},
+        volume = {36},
+        number = {5},
+        pages = {348--354},
+        year = {2015},
+        doi = {10.1002/jcc.23804}
+    }
+
+    @article{Seeliger2010pmx,
+        title = {Protein Thermostability Calculations Using
+        Alchemical Free Energy Simulations},
+        author = {Seeliger, Daniel and de Groot, Bert L.},
+        journal = {Biophysical Journal},
+        volume = {98},
+        number = {10},
+        pages = {2309--2316},
+        year = {2010},
+        doi = {10.1016/j.bpj.2010.01.051}
+    }
+
+
+License
+-------
+``pmx`` is licensed under the GNU Lesser General Public License v3.0 (LGPL v3).
+
+.. |build| image:: https://travis-ci.org/deGrootLab/pmx.svg?branch=master
+    :alt: Build Status
+    :scale: 100%
+    :target: https://travis-ci.org/deGrootLab/pmx
+
+.. |cov| image:: https://codecov.io/gh/deGrootLab/pmx/branch/develop/graph/badge.svg
+    :alt: Code coverage
+    :scale: 100%
+    :target: https://codecov.io/gh/deGrootLab/pmx
+
+
```

### Comparing `pmx_biobb-1.0.1/README.rst` & `pmx_biobb-2.0.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 pmx: alchemistry in gromacs
 ===========================
 
 |build| |cov|
 
+**PMX_BIOBB DISTRIBUTION VERSION**: 2.0.0
+**Based on the PMX Icolos branch commit**: https://github.com/deGrootLab/pmx/commit/80f4f8a1552c37e3d926f950d91db77cd4dea9cf
+
 **Warning:** this is a development version of ``pmx``, it is not stable or reliable yet. You are welcome to
 try/test it and provide feedback, but use at your own risk. The current stable version of ``pmx`` can
 be found in the master branch: https://github.com/deGrootLab/pmx
 
 ``pmx`` is a python library that allows users to setup and analyse molecular
 dynamics simulations with the `Gromacs <http://gromacs.org>`_ package.
 Among its main features are the setup and analysis of alchemical free energy
```

### Comparing `pmx_biobb-1.0.1/setup.py` & `pmx_biobb-2.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,20 +36,21 @@
                   )
 extensions = [pmx, xdrio]
 
 # -----
 # Setup
 # -----
 setup(name='pmx_biobb',
-      version='1.0.1',
+      version='2.0.0',
       cmdclass=versioneer.get_cmdclass(),
       description='Toolkit for free-energy calculation setup/analysis '
                   'and biomolecular structure handling',
       long_description=readme(),
       classifiers=[
+        'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Programming Language :: Python',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering',
       ],
       url='https://github.com/deGrootLab/pmx/tree/develop',
       author='Daniel Seeliger',
@@ -58,10 +59,10 @@
       packages=['pmx'],
       package_dir={'': 'src'},
       include_package_data=True,
       zip_safe=False,
       ext_modules=extensions,
       tests_require=['pytest'],
       install_requires=['numpy', 'scipy', 'matplotlib', 'future'],
-      python_requires="==3.7.*",
+      python_requires=">=3.7",
       entry_points={'console_scripts': ['pmx = pmx.scripts.cli:entry_point']},
       )
```

### Comparing `pmx_biobb-1.0.1/src/pmx/__init__.py` & `pmx_biobb-2.0.0/src/pmx/__init__.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/alchemy.py` & `pmx_biobb-2.0.0/src/pmx/alchemy.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,14 +230,20 @@
     ffbonded_file = os.path.join(topol.ffpath, 'ffbonded.itp')
 
     # main function that returns the Topology with filled B states
     def process_topol(topol, ff, ffbonded_file, verbose=False, scaleDih=1.0):
         pmxtop = deepcopy(topol)
         # create model with residue list
         m = Model(atoms=pmxtop.atoms, renumber_residues=False)
+        # need to sequentially renumber residues, 
+        # because --keep_resid flag may leave residues numbered non-sequentially
+        counter = 0
+        for r in m.residues:
+            counter += 1 
+            r.id = counter
         # use model residue list
         pmxtop.residues = m.residues
         # get list of hybrid residues and their params
         rlist, rdic = _get_hybrid_residues(m=m, ff=ff, version='new',
                                            verbose=verbose)
         # correct b-states
         pmxtop.assign_fftypes()
@@ -1204,15 +1210,14 @@
     dih9 = []  # here I will accumulate multiple entries of type 9 dihedrals
     explicit_def = _explicit_defined_dihedrals(ffbonded, ff)
     ildn_used = []  # ildn dihedrals that already were encountered
     opls_used = []  # opls dihedrals that already were encountered
 #    scaleDih = 0.0  # scale dihedrals with dummies
 
     for r in rlist:
-        idx = r.id - 1
         dih = rdic[r.resname][3]
         imp = rdic[r.resname][2]
         for d in imp+dih:
             al = []
             for name in d[:4]:
                 if name.startswith('+'):
                     next = r.chain.fetch_residue(idx=r.id+1)
```

### Comparing `pmx_biobb-1.0.1/src/pmx/analysis.py` & `pmx_biobb-2.0.0/src/pmx/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,18 @@
     ndata : int
         number of data points in the input file.
     '''
 
     # check lambda0 is either 0 or 1
     assert lambda0 in [0, 1]
 
-    lines = open(fn, encoding="ISO-8859-1").readlines()
+    try:
+        lines = open(fn, encoding="ISO-8859-1").readlines()
+    except:
+        return None, None
     if not lines:
         return None, None
 
     # extract dgdl datapoints into r
     # TODO: we removed the check for file integrity. We could have an
     # optional files integrity check before calling this integration func
 
@@ -348,21 +351,28 @@
         x = x2
     mf, devf, Af = data2gauss(wf)
     mb, devb, Ab = data2gauss(wr)
 
     maxi = max(wf+wr)
     mini = min(wf+wr)
 
-    sm1 = smooth(np.array(wf))
-    sm2 = smooth(np.array(wr))
     plt.subplot(1, 2, 1)
     plt.plot(x1, wf, 'g-', linewidth=2, label="Forward (0->1)", alpha=.3)
-    plt.plot(x1, sm1, 'g-', linewidth=3)
     plt.plot(x2, wr, 'b-', linewidth=2, label="Backward (1->0)", alpha=.3)
-    plt.plot(x2, sm2, 'b-', linewidth=3)
+    ### smoothing ###
+    try:
+        sm1 = smooth(np.array(wf))
+        plt.plot(x1, sm1, 'g-', linewidth=3)
+    except:
+        print("Plotting: no smoothing for Wf")
+    try:
+        sm2 = smooth(np.array(wr))
+        plt.plot(x2, sm2, 'b-', linewidth=3)
+    except:
+        print("Plotting: no smoothing for Wr")
     plt.legend(shadow=True, fancybox=True, loc='upper center',
                prop={'size': 12})
     plt.ylabel(r'W [kJ/mol]', fontsize=20)
     plt.xlabel(r'# Snapshot', fontsize=20)
     plt.grid(lw=2)
     plt.xlim(0, x[-1]+1)
     xl = plt.gca()
```

### Comparing `pmx_biobb-1.0.1/src/pmx/atom.py` & `pmx_biobb-2.0.0/src/pmx/atom.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         self.name = line[12:16].strip()
         self.altloc = line[16]
         self.resname = line[17:21].strip()
         self.chain_id = line[21]
         try:
             self.resnr = int(line[22:27])
         except:
-            self.resnr = line[22:27]  # contains insertion code
+            self.resnr = line[22:27].lstrip().rstrip()  # contains insertion code
 
         self.x = [float(line[30:38]),
                   float(line[39:46]),
                   float(line[47:54])]
         try:
             self.occ = float(line[55:60])
         except:
```

### Comparing `pmx_biobb-1.0.1/src/pmx/atomselection.py` & `pmx_biobb-2.0.0/src/pmx/atomselection.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/builder.py` & `pmx_biobb-2.0.0/src/pmx/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,21 +43,23 @@
     >>> ch = build_chain('FGHRTCV',hydrogens = False) # build chain without H
     >>> ch = build_chain('FGHRTCV',ss='HHHHHHH') build as helix
     >>> ch = build_chain('FGHRTCV',dihedrals = ((phi1,psi1,omega1),(...)))
     build chain with defined dihedral angles
 """
 
 import sys
+import copy as cp
 from numpy import array, pi, linalg, cross
 from . import library
 from .geometry import Rotation
 from .chain import Chain
 from .atom import Atom
 from .model import Model
 from .molecule import Molecule
+from . import geometry
 
 
 def add_bp(m, strand=None, bRNA=False):
     if strand:
         N = len(strand)/2
         if bRNA:
             N = len(strand)
@@ -254,15 +256,39 @@
     mol.remove_atom(R)
     bR.bonds.append(bb)
     bb.bonds.append(bR)
     for a in mol.atoms:
         master.append(a)
 
 
-def make_residue(key, hydrogens=True):
+def _is_mainchain( a ):
+    if a.name=='N':
+        return(True)
+    if a.name=='H' or a.name=='HN' or a.name=='H1' or a.name=='H2' or a.name=='H3':
+        return(True)
+    if a.name=='CA':
+        return(True)
+    if a.name=='C':
+        return(True)
+    if a.name=='O' or a.name=='OXT' or a.name=='OX' or a.name=='OT':
+        return(True)
+    return(False)
+
+def make_stereoisomer_residue( m ):
+    mtmp = cp.deepcopy( m )
+    # fit
+    N1, CA1, C1 = m.fetchm(['N', 'CA', 'C'])
+    N2, CA2, C2 = mtmp.fetchm(['N', 'CA', 'C'])
+    geometry.fit_atoms( [N1,CA1,C1], [C2,CA2,N2], mtmp.atoms )
+    for atmp,a in zip(mtmp.atoms,m.atoms):
+        if _is_mainchain( a )==False:
+            a.x = atmp.x
+    return(m)
+
+def make_residue(key, hydrogens=True, chirality='L'):
     """ returns a molecule object with
     default geometry"""
 
     if key not in library._aacids:
         raise(KeyError, "Residue %s not known" % key)
     m = Molecule()
     m.unity = 'A'
@@ -277,19 +303,44 @@
             a.symbol = a.name[0]
             a.x = entry[1]
             a.occ = 1.
             a.resname = key
             a.m = library._atommass[a.symbol]
             a.unity = 'A'
             m.atoms.append(a)
+
+    if chirality=='D':
+        m = make_stereoisomer_residue( m )
     return m
 
 
 def build_chain(sequence, dihedrals=None,
-                hydrogens=True, ss=None, chain_id='X'):
+                hydrogens=True, ss=None, chain_id='X', bCyclic=False, bCap=False,
+                chirality=None):
+
+    # chirality 
+    if chirality==None:
+        chirality = ''
+        for s in sequence:
+            chirality = chirality+'L'
+
+    # if cyclic, form dihedrals
+    n = len(sequence)
+    if bCyclic==True:
+        dihedrals = []
+        fudge = float(n)/5.0 # empirical fudge to have some space between the termini
+        dphi = 2.0*360.0/float(n+fudge)
+        if bCap==True: # leave space for caps
+            dphi = 2.0*360.0/float(n+fudge+1)
+        dpsi = 0.0
+        dom = 180.0
+        sign = -1.0
+        for i in range(0,n):
+            dihedrals.append( (sign*dphi,-1.0*sign*dpsi,dom) )
+            sign = -1.0*sign
 
     ch = Chain()
     if dihedrals is None:
         if ss is None:
             dihedrals = []
             for i in range(len(sequence)):
                 dihedrals.append(library._extended)
@@ -300,38 +351,45 @@
                     dihedrals.append(library._extended)
                 elif s == 'H':
                     dihedrals.append(library._helix)
                 elif s == 'E':
                     dihedrals.append(library._anti_beta)
 
     rl = []
-    start = make_residue(library._aacids_dic[sequence[0]], hydrogens=hydrogens)
+    start = make_residue(library._aacids_dic[sequence[0]], hydrogens=hydrogens, chirality=chirality[0])
     start.set_resid(1)
     set_psi(start, dihedrals[0][1])
     rl.append(start)
-    for i, aa in enumerate(sequence[1:]):
-        phi, psi, om = dihedrals[i+1]
-        phi2, psi2, om2 = dihedrals[i]
+    for i in range(1,n):
+        aa = sequence[i]
+        ld = chirality[i]
+        phi, psi, om = dihedrals[i]
+        phi2, psi2, om2 = dihedrals[i-1]
         mol = attach_aminoacid(start, library._aacids_ext_amber[aa],
                                hydrogens=hydrogens,
-                               phi=phi, psi=psi, omega=om2)
-        mol.set_resid(i+2)
-        set_phi(start, mol, dihedrals[i+1][0])
+                               phi=phi, psi=psi, omega=om2,chirality=ld)
+        mol.set_resid(i+1)
+        set_phi(start, mol, dihedrals[i][0])
         start = mol
         rl.append(mol)
     al = []
     for r in rl:
         al += r.atoms
     ch.unity = 'A'
     ch.atoms = al
     ch.renumber_atoms()
     ch.residues = rl
     ch.set_chain_id(chain_id)
     for atom in ch.atoms:
         atom.unity = 'A'
+
+    if bCap==True:
+        ch.add_nterm_cap()
+        ch.add_cterm_cap()
+
     return ch
 
 
 def set_phi(mol1, mol2, phi):
     # select c, n, ca, c
     C = mol1.fetchm(['C'])[0]
     N, CA, C2 = mol2.fetchm(['N', 'CA', 'C'])
@@ -373,17 +431,17 @@
     r = Rotation(C.x, N.x)
     for atom in mol2.atoms:
         if atom.name != 'N':
             atom.x = r.apply(atom.x, delta)
 
 
 def attach_aminoacid(mol, resname, hydrogens=True,
-                     omega=180., phi=-139., psi=135.):
+                     omega=180., phi=-139., psi=135., chirality='L'):
 
-    new = make_residue(resname, hydrogens=hydrogens)
+    new = make_residue(resname, hydrogens=hydrogens, chirality=chirality)
     # we need Ca, C and O from mol
     Ca, C, O = mol.fetchm(['CA', 'C', 'O'])
     # and N from new
     N, CA2 = new.fetchm(['N', 'CA'])
 
     l = 1.33  # length of peptide bond
```

### Comparing `pmx_biobb-1.0.1/src/pmx/chain.py` & `pmx_biobb-2.0.0/src/pmx/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,19 +277,24 @@
             for r in self.model.residues:
                 for atom in r.atoms:
                     self.model.atoms.append(atom)
         self.atoms = []
         for r in self.residues:
             for atom in r.atoms:
                 self.atoms.append(atom)
-        if midx != -1:
+        if midx != -1: # renumber in the model
             if renumber_atoms is True:
                 self.model.renumber_atoms()
             if renumber_residues is True:
                 self.model.renumber_residues()
+        else: # renumber in the chain
+            if renumber_atoms is True:
+                self.renumber_atoms()
+            if renumber_residues is True:
+                self.renumber_residues()
         self.make_residue_tree()
 
     def replace_residue(self, residue, new, bKeepResNum=False):
         """Replaces a residue.
 
         Parameters
         ----------
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/aminoacids.pkl` & `pmx_biobb-2.0.0/src/pmx/data/aminoacids.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/bbdep.pkl` & `pmx_biobb-2.0.0/src/pmx/data/bbdep.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/blosum62_new.mat` & `pmx_biobb-2.0.0/src/pmx/data/blosum62_new.mat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/bp.pkl` & `pmx_biobb-2.0.0/src/pmx/data/bp.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/bp_amber.pkl` & `pmx_biobb-2.0.0/src/pmx/data/bp_amber.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/bp_charmm.pkl` & `pmx_biobb-2.0.0/src/pmx/data/bp_charmm.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/ffamber99sbnb.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffnonbonded.itp`

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,115 @@
-; ########################################################################
-; #                                                                      #
-; #            ffamber ports for GROMACS 3.3.1 - August 2007             #
-; #       Eric J. Sorin - CSU Long Beach, Dept. of Chem & Biochem        #
-; # With significant contributions from Sanghyun Park and Jory Z. Ruscio #
-; #   Please cite: Sorin & Pande (2005). Biophys. J. 88(4), 2472-2493.   #
-; #            For additional information, tools, and updates            #
-; #          please consult http://chemistry.csulb.edu/ffamber/          #
-; #                                                                      #
-; ########################################################################
 [ atomtypes ]
-; name     bond_type  mass   charge ptype  sigma      epsilon
-amber99_1     BR     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_2     C      0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_3     CA     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_4     CB     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_5     CC     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_6     CK     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_7     CM     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_8     CN     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_9     CQ     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_10    CR     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_11    CT     0.0000  0.0000  A   3.39967e-01  4.57730e-01
-amber99_12    CV     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_13    CW     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_14    C*     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_15    Ca     0.0000  0.0000  A   3.05240e-01  1.92376e+00
-amber99_16    F      0.0000  0.0000  A   3.11815e-01  2.55224e-01
-amber99_17    H      0.0000  0.0000  A   1.06908e-01  6.56888e-02
-amber99_18    HC     0.0000  0.0000  A   2.64953e-01  6.56888e-02
-amber99_19    H1     0.0000  0.0000  A   2.47135e-01  6.56888e-02
-amber99_20    H2     0.0000  0.0000  A   2.29317e-01  6.56888e-02
-amber99_21    H3     0.0000  0.0000  A   2.11499e-01  6.56888e-02
-amber99_22    HA     0.0000  0.0000  A   2.59964e-01  6.27600e-02
-amber99_23    H4     0.0000  0.0000  A   2.51055e-01  6.27600e-02
-amber99_24    H5     0.0000  0.0000  A   2.42146e-01  6.27600e-02
-amber99_25    HO     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_26    HS     0.0000  0.0000  A   1.06908e-01  6.56888e-02
-amber99_27    HW     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_28    HP     0.0000  0.0000  A   1.95998e-01  6.56888e-02
-amber99_29    I      0.0000  0.0000  A   4.18722e-01  1.67360e+00
-amber99_30    Cl     0.0000  0.0000  A   4.40104e-01  4.18400e-01
-amber99_31    Na     0.0000  0.0000  A   3.32840e-01  1.15897e-02
-amber99_32    IB     0.0000  0.0000  A   8.90899e-01  4.18400e-01
-amber99_33    Mg     0.0000  0.0000  A   1.41225e-01  3.74342e+00
-amber99_34    N      0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_35    NA     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_36    NB     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_37    NC     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_38    N2     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_39    N3     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_40    N*     0.0000  0.0000  A   3.25000e-01  7.11280e-01
-amber99_41    O      0.0000  0.0000  A   2.95992e-01  8.78640e-01
-amber99_42    OW     0.0000  0.0000  A   3.15061e-01  6.36386e-01
-amber99_43    OH     0.0000  0.0000  A   3.06647e-01  8.80314e-01
-amber99_44    OS     0.0000  0.0000  A   3.00001e-01  7.11280e-01
-amber99_45    O2     0.0000  0.0000  A   2.95992e-01  8.78640e-01
-amber99_46    P      0.0000  0.0000  A   3.74177e-01  8.36800e-01
-amber99_47    S      0.0000  0.0000  A   3.56359e-01  1.04600e+00
-amber99_48    SH     0.0000  0.0000  A   3.56359e-01  1.04600e+00
-amber99_49    CU     0.0000  0.0000  A   3.39967e-01  3.59824e-01
-amber99_50    FE     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_51    K      0.0000  0.0000  A   4.73602e-01  1.37235e-03
-amber99_52    Rb     0.0000  0.0000  A   5.26699e-01  7.11280e-04
-amber99_53    Cs     0.0000  0.0000  A   6.04920e-01  3.37230e-04
+; name      at.num  mass     charge ptype  sigma      epsilon
+Br          35      79.90    0.0000  A   0.00000e+00  0.00000e+00
+C            6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CA           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CB           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CC           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CK           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CM           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CN           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CQ           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CR           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CT           6      12.01    0.0000  A   3.39967e-01  4.57730e-01
+CV           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+CW           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+C*           6      12.01    0.0000  A   3.39967e-01  3.59824e-01
+C0          20      40.08    0.0000  A   3.05240e-01  1.92376e+00
+F            9      19.00    0.0000  A   3.11815e-01  2.55224e-01
+H            1       1.008   0.0000  A   1.06908e-01  6.56888e-02
+HC           1       1.008   0.0000  A   2.64953e-01  6.56888e-02
+H1           1       1.008   0.0000  A   2.47135e-01  6.56888e-02
+H2           1       1.008   0.0000  A   2.29317e-01  6.56888e-02
+H3           1       1.008   0.0000  A   2.11499e-01  6.56888e-02
+HA           1       1.008   0.0000  A   2.59964e-01  6.27600e-02
+H4           1       1.008   0.0000  A   2.51055e-01  6.27600e-02
+H5           1       1.008   0.0000  A   2.42146e-01  6.27600e-02
+HO           1       1.008   0.0000  A   0.00000e+00  0.00000e+00
+HS           1       1.008   0.0000  A   1.06908e-01  6.56888e-02
+HW           1       1.008   0.0000  A   0.00000e+00  0.00000e+00
+HP           1       1.008   0.0000  A   1.95998e-01  6.56888e-02
+I           53     126.9     0.0000  A   4.18722e-01  1.67360e+00
+Cl          17      35.45    0.0000  A   4.40104e-01  4.18400e-01
+Na          11      22.99    0.0000  A   3.32840e-01  1.15897e-02
+IB           0     131.0     0.0000  A   8.90899e-01  4.18400e-01
+MG          12      24.305   0.0000  A   1.41225e-01  3.74342e+00
+N            7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+NA           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+NB           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+NC           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+N2           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+N3           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+N*           7      14.01    0.0000  A   3.25000e-01  7.11280e-01
+O            8      16.00    0.0000  A   2.95992e-01  8.78640e-01
+OW           8      16.00    0.0000  A   3.15061e-01  6.36386e-01
+OH           8      16.00    0.0000  A   3.06647e-01  8.80314e-01
+OS           8      16.00    0.0000  A   3.00001e-01  7.11280e-01
+O2           8      16.00    0.0000  A   2.95992e-01  8.78640e-01
+P           15      30.97    0.0000  A   3.74177e-01  8.36800e-01
+S           16      32.06    0.0000  A   3.56359e-01  1.04600e+00
+SH          16      32.06    0.0000  A   3.56359e-01  1.04600e+00
+CU          29      63.55    0.0000  A   3.39967e-01  3.59824e-01
+FE          26      55.00    0.0000  A   0.00000e+00  0.00000e+00
+K           19      39.10    0.0000  A   4.73602e-01  1.37235e-03
+Rb          37      85.47    0.0000  A   5.26699e-01  7.11280e-04
+Cs          55     132.91    0.0000  A   6.04920e-01  3.37230e-04
 ; spc water - use only with spc.itp & settles
-amber99_54    OW     0.0000  0.0000  A   3.16557e-01  6.50629e-01
-amber99_55    HW     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_56    Li     0.0000  0.0000  A   2.02590e-01  7.65672e-02
-amber99_57    Zn     0.0000  0.0000  A   1.95998e-01  5.23000e-02
-amber99_58    Sr     0.0000  0.0000  A   3.10247e-01  4.94658e-01
-amber99_59    Ba     0.0000  0.0000  A   3.78472e-01  1.97050e-01
+OW_spc       8      15.9994  0.0000  A   3.16557e-01  6.50629e-01
+HW_spc       1       1.0080  0.0000  A   0.00000e+00  0.00000e+00
+Li           3       6.94    0.0000  A   2.02590e-01  7.65672e-02
+Zn          30      65.4     0.0000  A   1.95998e-01  5.23000e-02
 ;tip4p-EW
-amber99_60    HW     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_61    OW     0.0000  0.0000  A   3.16435e-01  6.80946e-01
+HW_tip4pew   1       1.008   0.0000  A   0.00000e+00  0.00000e+00
+OW_tip4pew   8      16.00    0.0000  A   3.16435e-01  6.80946e-01
 ; tip4p
-amber99_62    HW     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_63    OW     0.0000  0.0000  A   3.15365e-01  6.48520e-01
+HW_tip4p     1       1.008   0.0000  A   0.00000e+00  0.00000e+00
+OW_tip4p     8      16.00    0.0000  A   3.15365e-01  6.48520e-01
 ;tip5p
-amber99_64    HW     0.0000  0.0000  A   0.00000e+00  0.00000e+00
-amber99_65    OW     0.0000  0.0000  A   3.12000e-01  6.69440e-01
-;tip3p heavy
-amber99_66    HW     4.0320  0.0000  A   0.00000e+00  0.00000e+00
-amber99_67    OW     9.9520  0.0000  A   3.15061e-01  6.36386e-01
+HW_tip5p     1       1.008   0.0000  A   0.00000e+00  0.00000e+00
+OW_tip5p     8      16.00    0.0000  A   3.12000e-01  6.69440e-01
 ; dummy defs
 ; MW=Dummy mass for tip4p/EW/5p water extra point charge
-MW           MW      0.0000  0.0000  A   0.00000e+00  0.00000e+00
-MNH3         MNH3    0.0000  0.0000  A   0.00000e+00  0.00000e+00
-MNH2         MNH2    0.0000  0.0000  A   0.00000e+00  0.00000e+00
-MCH3A        MCH3A   0.0000  0.0000  A   0.00000e+00  0.00000e+00
-MCH3B        MCH3B   0.0000  0.0000  A   0.00000e+00  0.00000e+00
+MW           0       0.0000  0.0000  A   0.00000e+00  0.00000e+00
+; Dummy masses for rigid CH3 and NH3 groups
+MCH3         0       0.0000  0.0000  A   0.00000e+00  0.00000e+00
+MNH3         0       0.0000  0.0000  A   0.00000e+00  0.00000e+00
+DUM_HC    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_H     	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CT    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_H1    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_C*    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CW    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_H4    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CB    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_NA    	0	14.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CN    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CA    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_HA    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_C     	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_O     	0	16.00	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_OH    	0	16.00	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_HO    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_SH    	0	32.06	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_HS    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_O2    	0	16.00	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CC    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CV    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_CR    	0	12.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_H5    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_NB    	0	14.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_HP    	0	1.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_N3    	0	14.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_S     	0	32.06	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_N     	0	14.01	   0.0000  A   0.00000e+00 0.00000e+00
+DUM_N2    	0	14.01	   0.0000  A   0.00000e+00 0.00000e+00
+;ions
+amber99_143   11    0.0000  0.0000  A   2.35000e-01  4.18818e-01
+amber99_144   17    0.0000  0.0000  A   4.40000e-01  5.43502e-01
+; Joung ions
+; TIP3P
+amber99_333   17   0.0000  0.0000  A  4.47766e-01  1.48913e-01
+amber99_337   19    0.0000  0.0000  A  3.03796e-01  8.10369e-01
+amber99_338   11   0.0000  0.0000  A  2.43928e-01  3.65846e-01
+; SPCE
+amber99_351   17    0.0000  0.0000  A  4.83045e-01  5.34924e-02
+amber99_356   11    0.0000  0.0000  A  2.15954e-01  1.47545e+00
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/Makefile.am`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/Makefile.in`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber14sbmut.ff/urea.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber14sbmut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.arn_backup`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-bsc1-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_ffbonded_for_ildn_test.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/backup_mutres`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/correct_ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffberger.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/popc_AmbBer_posre.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-dna-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.arn`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.r2b`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.rtp`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,127 @@
      C     O
     -C     N
  [ impropers ]
     -C    CA     N     H
     CA    +N     C     O
     N     CA     C    +N    105.4       0.75       1
 
+; VG: phosphothreonine q=-2 
+[ TPO ]
+ [ atoms ]
+       N N            -0.516301     1
+       H H            0.293600     2
+      CA CT           -0.313510     3
+      HA H1           0.215772     4
+      CB CT           0.623862     5
+      HB H1           0.009989     6
+     CG2 CT           -0.406805     7
+    HG21 HC           0.071662     8
+    HG22 HC           0.071662     9
+    HG23 HC           0.071662    10
+      OG OS           -0.545231    11
+       P P            1.366058    12
+     O1P O2           -0.965707    13
+     O2P O2           -0.965707    14
+     O3P O2           -0.965707    15
+       C C            0.536601    16
+       O O            -0.581901    17
+
+ [ bonds ]
+       N        H   0.1010 363170.0000 
+       N       CA   0.1449 282000.0000 
+      CA       HA   0.1090 284510.0000 
+      CA       CB   0.1526 259410.0000 
+      CA        C   0.1522 265270.0000 
+      CB       HB   0.1090 284510.0000 
+      CB      CG2   0.1526 259410.0000 
+      CB       OG   0.1410 267780.0000 
+     CG2     HG21   0.1090 284510.0000 
+     CG2     HG22   0.1090 284510.0000 
+     CG2     HG23   0.1090 284510.0000 
+      OG        P   0.1610 439320.0000 
+       P      O1P   0.1480 439320.0000 
+       P      O2P   0.1480 439320.0000 
+       P      O3P   0.1480 439320.0000 
+       C        O   0.1229 476980.0000 
+      -C     N
+
+ [ angles ]
+       N       CA       HA 109.5000 418.4000 
+       N       CA       CB 109.7000 669.4400 
+       N       CA        C 110.1000 527.1800 
+       H        N       CA 118.0400 418.4000 
+      CA       CB       HB 109.5000 418.4000 
+      CA       CB      CG2 109.5000 334.7200 
+      CA       CB       OG 109.5000 418.4000 
+      CA        C        O 120.4000 669.4400 
+      HA       CA       CB 109.5000 418.4000 
+      HA       CA        C 109.5000 418.4000 
+      CB       CA        C 111.1000 527.1800 
+      CB      CG2     HG21 109.5000 418.4000 
+      CB      CG2     HG22 109.5000 418.4000 
+      CB      CG2     HG23 109.5000 418.4000 
+      CB       OG        P 120.5000 836.8000 
+      HB       CB      CG2 109.5000 418.4000 
+      HB       CB       OG 109.5000 418.4000 
+     CG2       CB       OG 109.5000 418.4000 
+    HG21      CG2     HG22 109.5000 292.8800 
+    HG21      CG2     HG23 109.5000 292.8800 
+    HG22      CG2     HG23 109.5000 292.8800 
+      OG        P      O1P 108.2300 836.8000 
+      OG        P      O2P 108.2300 836.8000 
+      OG        P      O3P 108.2300 836.8000 
+     O1P        P      O2P 119.9000 1171.5000 
+     O1P        P      O3P 119.9000 1171.5000 
+     O2P        P      O3P 119.9000 1171.5000 
+
+ [ dihedrals ]
+       N       CA       CB HB   0.0000   0.6508   3.0000 
+       N       CA       CB CG2   0.0000   0.6508   3.0000 
+       N       CA       CB OG   0.0000   0.6508   3.0000 
+       N       CA        C O   0.0000   0.0000   0.0000 
+       H        N       CA HA   0.0000   0.0000   0.0000 
+       H        N       CA CB   0.0000   0.0000   0.0000 
+       H        N       CA C   0.0000   0.0000   0.0000 
+      CA       CB      CG2 HG21   0.0000   0.6694   3.0000 
+      CA       CB      CG2 HG22   0.0000   0.6694   3.0000 
+      CA       CB      CG2 HG23   0.0000   0.6694   3.0000 
+      CA       CB       OG P   0.0000   1.6039   3.0000 
+      HA       CA       CB HB   0.0000   0.6508   3.0000 
+      HA       CA       CB CG2   0.0000   0.6508   3.0000 
+      HA       CA       CB OG   0.0000   0.0000   0.0000 
+      HA       CA       CB OG   0.0000   1.0460   1.0000 
+      HA       CA        C O   0.0000   0.0000   0.0000 
+      HA       CA        C O   0.0000   3.3472   1.0000 
+      HA       CA        C O 180.0000   0.3347   3.0000 
+      CB       CA        C O   0.0000   0.0000   0.0000 
+      CB       OG        P O1P   0.0000   1.0460   3.0000 
+      CB       OG        P O2P   0.0000   1.0460   3.0000 
+      CB       OG        P O3P   0.0000   1.0460   3.0000 
+      HB       CB       CA C   0.0000   0.6508   3.0000 
+      HB       CB      CG2 HG21   0.0000   0.6508   3.0000 
+      HB       CB      CG2 HG22   0.0000   0.6508   3.0000 
+      HB       CB      CG2 HG23   0.0000   0.6508   3.0000 
+      HB       CB       OG P   0.0000   1.6039   3.0000 
+     CG2       CB       CA C   0.0000   0.6508   3.0000 
+     CG2       CB       OG P   0.0000   1.6039   3.0000 
+    HG21      CG2       CB OG   0.0000   0.0000   0.0000 
+    HG21      CG2       CB OG   0.0000   1.0460   1.0000 
+    HG22      CG2       CB OG   0.0000   0.0000   0.0000 
+    HG22      CG2       CB OG   0.0000   1.0460   1.0000 
+    HG23      CG2       CB OG   0.0000   0.0000   0.0000 
+    HG23      CG2       CB OG   0.0000   1.0460   1.0000 
+      OG       CB       CA C   0.0000   0.6508   3.0000 
+
+ [ impropers ]
+    -C    CA     N     H
+    CA    +N     C     O
+    N     CA     C    +N    105.4       0.75       1
+
+
 [ LEU ]
  [ atoms ]
      N    N           -0.41570     1
      H    H            0.27190     2
     CA    CT          -0.05180     3
     HA    H1           0.09220     4
     CB    CT          -0.11020     5
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/gbsa.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/amber99sb-star-ildn-mut.ff/urea.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/atommass.dat` & `pmx_biobb-2.0.0/src/pmx/data/mutff/atommass.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/aminoacids.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnabonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnanonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/forcefield.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/lipids.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/rna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip4pew.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tip5p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm22star-mut.ff/tips3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/atomtypes.atp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/cmap.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ffbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ffnonbonded.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/forcefield.doc`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/gb.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/ions.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.c.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.hdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.n.tdb`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.rtp`

 * *Files 0% similar despite different names*

```diff
@@ -61172,7 +61172,114 @@
         OW      OT      -0.834  0
         HW1     HT      0.417   0
         HW2     HT      0.417   0
  [ bonds ]
         OW      HW1
         OW      HW2
         HW1     HW2
+
+; VG: phosphothreonine q=-2
+[ TPO ]
+ [ atoms ]
+       N NH1          -0.470000     1
+      HN H            0.310000     2
+      CA CT1          0.070000     3
+      HA HB1          0.090000     4
+      CB CT1          -0.090000     5
+      HB HA1          0.090000     6
+     OG1 ON2          -0.400000     7
+       P P            1.100000     8
+     O1P ON3          -0.900000     9
+     O2P ON3          -0.900000    10
+     O3P ON3          -0.900000    11
+     CG2 CT3          -0.270000    12
+    HG21 HA3          0.090000    13
+    HG22 HA3          0.090000    14
+    HG23 HA3          0.090000    15
+       C C            0.510000    16
+       O O            -0.510000    17
+
+ [ bonds ]
+       N       HN 
+       N       CA 
+      CA       CB 
+      CA        C 
+      CA       HA 
+      CB      OG1 
+      CB      CG2 
+      CB       HB 
+     OG1        P 
+       P      O3P 
+       P      O1P 
+       P      O2P 
+     CG2     HG21 
+     CG2     HG22 
+     CG2     HG23 
+       C        O 
+       C       +N
+
+ [ angles ]
+      HN        N       CA 
+       N       CA       HA 
+       N       CA       CB 
+       N       CA        C 
+      HA       CA       CB 
+      HA       CA        C 
+      CB       CA        C 
+      CA       CB       HB 
+      CA       CB      OG1 
+      CA       CB      CG2 
+      HB       CB      OG1 
+      HB       CB      CG2 
+     OG1       CB      CG2 
+      CB      OG1        P 
+     OG1        P      O1P 
+     OG1        P      O2P 
+     OG1        P      O3P 
+     O1P        P      O2P 
+     O1P        P      O3P 
+     O2P        P      O3P 
+      CB      CG2     HG21 
+      CB      CG2     HG22 
+      CB      CG2     HG23 
+    HG21      CG2     HG22 
+    HG21      CG2     HG23 
+    HG22      CG2     HG23 
+      CA        C        O 
+
+ [ dihedrals ]
+       N       CA       CB HB 
+       N       CA       CB OG1 
+       N       CA       CB CG2 
+       N       CA        C O 
+      HN        N       CA HA 
+      HN        N       CA CB 
+      HN        N       CA C 
+      CA       CB      OG1 P 
+      CA       CB      CG2 HG21 
+      CA       CB      CG2 HG22 
+      CA       CB      CG2 HG23 
+      HA       CA       CB HB 
+      HA       CA       CB OG1 
+      HA       CA       CB CG2 
+      HA       CA        C O 
+      CB       CA        C O 
+      CB      OG1        P O1P 
+      CB      OG1        P O2P 
+      CB      OG1        P O3P
+       C       CA       CB HB 
+      HB       CB      OG1 P 
+      HB       CB      CG2 HG21 
+      HB       CB      CG2 HG22 
+      HB       CB      CG2 HG23 
+       C       CA       CB OG1 
+     OG1       CB      CG2 HG21 
+     OG1       CB      CG2 HG22 
+     OG1       CB      CG2 HG23 
+     CG2       CB      OG1 P 
+       C       CA       CB CG2 
+
+  [ impropers ]
+            N    -C    CA    HN
+            C    CA    +N     O
+  [ cmap ]
+           -C     N    CA     C    +N
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/merged.vsd`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.mtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/mutres_dna.rtp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/nbfix.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/spc.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/spce.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/tip3p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp` & `pmx_biobb-2.0.0/src/pmx/data/mutff/charmm36m-mut.ff/tip4p.itp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/elements.dat` & `pmx_biobb-2.0.0/src/pmx/data/mutff/elements.dat`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/residuetypes.dat` & `pmx_biobb-2.0.0/src/pmx/data/mutff/residuetypes.dat`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+TPO	Protein
 ABU	Protein
 ACE	Protein
 AIB	Protein
 ALA  	Protein
 ARG  	Protein
 ARGN	Protein
 ASN	Protein
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/spc216.gro` & `pmx_biobb-2.0.0/src/pmx/data/mutff/spc216.gro`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/data/mutff/vdwradii.dat` & `pmx_biobb-2.0.0/src/pmx/data/mutff/vdwradii.dat`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 ; Very approximate VanderWaals radii
 ; only used for drawing atoms as balls or for calculating atomic overlap.
 ; longest matches are used
 ; '???' or '*' matches any residue name
 ; 'AAA' matches any protein residue name
-???  C     0.15
-???  F     0.12
-???  H     0.04
-???  N     0.110
-???  O     0.105
-???  S     0.16
+; Source: http://en.wikipedia.org/wiki/Van_der_Waals_radius
+; These come from A. Bondi, "van der Waals Volumes and Radii",
+; J. Phys. Chem. 68 (1964) 441-451
+???  H     0.12
+???  C     0.17
+???  N     0.155
+???  O     0.152
+???  F     0.147
+???  P     0.18
+???  S     0.18
+???  Cl    0.175
 ; Water charge sites
 SOL  MW    0
 SOL  LP    0
 ; Masses for vsite construction
 GLY  MN1   0
 GLY  MN2   0
 ALA  MCB1  0
```

### Comparing `pmx_biobb-1.0.1/src/pmx/data/rna.pkl` & `pmx_biobb-2.0.0/src/pmx/data/rna.pkl`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/estimators.py` & `pmx_biobb-2.0.0/src/pmx/estimators.py`

 * *Files 2% similar despite different names*

```diff
@@ -790,25 +790,27 @@
         self.nr = len(wr)
         self.beta = 1./(kb*self.T)
         self.M = kb * self.T * np.log(float(self.nf) / float(self.nr))
 
         # Calculate all BAR properties available
         self.dg = self.calc_dg(self.wf, self.wr, self.T)
         self.err = self.calc_err(self.dg, self.wf, self.wr, self.T)
+        self.conv = self.calc_conv(self.dg, self.wf, self.wr, self.T)
         if nboots > 0:
             self.err_boot = self.calc_err_boot(self.wf, self.wr, nboots,
                                                self.T)
-        self.conv = self.calc_conv(self.dg, self.wf, self.wr, self.T)
-        if nboots > 0:
             self.conv_err_boot = self.calc_conv_err_boot(self.dg, self.wf,
                                                          self.wr, nboots,
                                                          self.T)
         if nblocks > 1:
             self.err_blocks = self.calc_err_blocks(self.wf, self.wr, nblocks,
                                                    self.T)
+            self.conv_err_blocks = self.calc_conv_err_blocks(self.dg, self.wf,
+                                                         self.wr, nblocks,
+                                                         self.T)
 
     @staticmethod
     def calc_dg(wf, wr, T):
         '''Estimates and returns the free energy difference.
 
         Parameters
         ----------
@@ -1044,7 +1046,52 @@
             bootB = np.random.choice(wr, size=nr, replace=True)
             conv_boot = BAR.calc_conv(dg, bootA, bootB, T)
             conv_boots.append(conv_boot)
 
         sys.stdout.write('\n')
         err = np.std(conv_boots)
         return err
+
+    @staticmethod
+    def calc_conv_err_blocks(dg, wf, wr, nblocks, T):
+        '''Calculates the standard error of the convergence measure
+        based on a number of blocks the work values are divided into. 
+        It is useful when you run independent
+        equilibrium simulations, so that you can then use their respective
+        work values to compute the standard error based on the repeats.
+
+        Parameters
+        ----------
+        dg : float
+            the BAR free energy estimate
+        wf : array_like
+            array of forward work values.
+        wr : array_like
+            array of reverse work values.
+        T : float
+            temperature
+        nblocks: int
+            number of blocks to divide the data into. This can be for
+            instance the number of independent equilibrium simulations
+            you ran.
+
+        Returns
+        ----------
+        sderr : float
+            the standard error of the convergence measure.
+        '''
+
+        conv_blocks = []
+        # loosely split the arrays
+        wf_split = np.array_split(wf, nblocks)
+        wr_split = np.array_split(wr, nblocks)
+
+        # calculate all dg
+        for wf_block, wr_block in zip(wf_split, wr_split):
+            conv_block = BAR.calc_conv(dg, wf_block, wr_block, T)
+            conv_blocks.append(conv_block)
+
+        # get std err
+        err_blocks = scipy.stats.sem(conv_blocks, ddof=1)
+
+        return err_blocks
+
```

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/Energy.c` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/Energy.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/Geometry.c` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/Geometry.h` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/Geometry.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/cpp_test.cpp` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/cpp_test.cpp`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/init.c` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/init.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/pmx.h` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/pmx.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/pmx/wrap_Geometry.c` & `pmx_biobb-2.0.0/src/pmx/extensions/pmx/wrap_Geometry.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/trr2xtc.c` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/trr2xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile.c` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile.h` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_c_test.c` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_c_test.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_trr.c` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_trr.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_trr.h` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_trr.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_xtc.c` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_xtc.c`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/extensions/xdr/xdrfile_xtc.h` & `pmx_biobb-2.0.0/src/pmx/extensions/xdr/xdrfile_xtc.h`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/ffparser.py` & `pmx_biobb-2.0.0/src/pmx/ffparser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/forcefield.py` & `pmx_biobb-2.0.0/src/pmx/forcefield.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,23 +116,26 @@
         self.virtual_sites2 = []
         self.virtual_sites3 = []
         self.virtual_sites4 = []
         self.has_vsites2 = False
         self.has_vsites3 = False
         self.has_vsites4 = False
         self.has_posre = False
+        self.has_exclusions = False
+        self.exclusions = []
         self.posre = []
         self.molecules = []
         self.footer = []
         self.system = ''
         self.ii = {}  # dict for intermolecular interactions
         self.qA = 0.
         self.qB = 0.
         self.include_itps = []
         self.forcefield = ''
+        self.is_itp = True
         if filename!=None:
             if os.path.splitext(filename)[1] == '.itp':
                 self.is_itp = True
             else:
                 self.is_itp = False
             self.read()
 
@@ -158,14 +161,15 @@
             self.read_pairs(lines)
             self.read_angles(lines)
             self.read_dihedrals(lines)
             self.read_cmap(lines)
             self.read_vsites2(lines)
             self.read_vsites3(lines)
             self.read_vsites4(lines)
+            self.read_exclusions(lines)
             self.read_intermolecular_interactions(lines)
             if self.has_posre:
                 self.read_posre(posre_sections)
             self.__make_residues()
         else: # maybe only atomtypes are available
             self.read_atomtypes(lines)
         if not self.is_itp:
@@ -390,45 +394,45 @@
         idx = [i for i, l in enumerate(lines) if 'intermolecular_interactions' in l]
         if len(idx) == 1:
             lines = lines[:idx[0]]
 
         lst = readSection(lines, '[ angles ]', '[')
         for line in lst:
             entries = line.split()
-            if len(entries) == 4:
+            if len(entries) == 4: # only atoms and angle type
                 idx = [int(x) for x in line.split()]
                 self.angles.append([self.atoms[idx[0]-1], self.atoms[idx[1]-1],
                                     self.atoms[idx[2]-1], idx[3]])
-            elif len(entries) == 6:
+            elif len(entries) == 6: # angle with parameters for type 1, stateA only
                 idx = [int(x) for x in entries[:4]]
                 l = float(entries[4])
                 k = float(entries[5])
                 self.angles.append([self.atoms[idx[0]-1], self.atoms[idx[1]-1],
                                     self.atoms[idx[2]-1], idx[3], [l, k]])
-            elif len(entries) == 8 and entries[3] == '1':
+            elif len(entries) == 8 and entries[3] == '1': # type 1 for states A and B
                 idx = [int(x) for x in entries[:4]]
                 lA = float(entries[4])
                 kA = float(entries[5])
                 lB = float(entries[6])
                 kB = float(entries[7])
                 self.angles.append([self.atoms[idx[0]-1], self.atoms[idx[1]-1],
                                     self.atoms[idx[2]-1], idx[3],
                                     [idx[3], lA, kA], [idx[3], lB, kB]])
-            elif len(entries) == 8 and entries[3] == '5':
+            elif len(entries) == 8 and entries[3] == '5': # type 5 with parameters, stateA only
                 idx = [int(x) for x in entries[:4]]
                 lA1 = float(entries[4])
                 kA1 = float(entries[5])
                 lA2 = float(entries[6])
                 kA2 = float(entries[7])
                 self.angles.append([self.atoms[idx[0]-1],
                                     self.atoms[idx[1]-1],
                                     self.atoms[idx[2]-1],
                                     idx[3],
                                     [idx[3], lA1, kA1, lA2, kA2]])
-            elif len(entries) == 12:
+            elif len(entries) == 12: # type 5 with parameters, states A and B
                 idx = [int(x) for x in entries[:4]]
                 lA1 = float(entries[4])
                 kA1 = float(entries[5])
                 lA2 = float(entries[6])
                 kA2 = float(entries[7])
                 lB1 = float(entries[8])
                 kB1 = float(entries[9])
@@ -487,14 +491,29 @@
                 self.cmap.append([self.atoms[idx[0]-1],
                                   self.atoms[idx[1]-1],
                                   self.atoms[idx[2]-1],
                                   self.atoms[idx[3]-1],
                                   self.atoms[idx[4]-1],
                                   func, rest])
 
+    def read_exclusions(self, lines):
+        starts = []
+        for i, line in enumerate(lines):
+            if line.strip().startswith('[ exclusions ]'):
+                starts.append(i)
+        if starts:
+            self.has_exclusions = True
+        for s in starts:
+            lst = readSection(lines[s:], '[ exclusions ]', '[')
+            for line in lst:
+                entr = line.split()
+                idx = [int(x) for x in entr[:]]
+                toappend = [self.atoms[x-1] for x in idx] 
+                self.exclusions.append( toappend )
+
     def read_vsites2(self, lines):
         starts = []
         for i, line in enumerate(lines):
             if line.strip().startswith('[ virtual_sites2 ]'):
                 starts.append(i)
         if starts:
             self.has_vsites2 = True
@@ -737,15 +756,15 @@
 
     # ===============
     # write functions
     # ===============
     def write(self, outfile, stateBonded='AB', stateTypes='AB', stateQ='AB',
               scale_mass=False, dummy_qA='on', dummy_qB='on', target_qB=None,
               full_morphe=True, write_atypes=True, posre_ifdef=True, posre_include=False,
-              verbose=False):
+              verbose=False, qPrec=6):
         """Writes the Topology to file.
 
         The parameters ``stateBonded``, ``stateTypes``, and ``stateQ`` control
         what to write in the B-state columns of the topology. This is needed
         for free energy calculations. However, if you are writing a
         standard topology file that do not contain information on B-states,
         choose the option 'A' so that only the A-state data will be written.
@@ -788,14 +807,16 @@
         posre_include : bool, optional
             whether to place the position restraints in a separate itp file
             that is included in the topology via an "#include" statement.
             Default is False.
         verbose : bool, optional
             whether to print out information about each atom written. Default
             is False.
+        qPrec : int, optional
+            number of significant digits for charges in topology. Default is 6.
         """
         # open file for writing
         fp = open(outfile, 'w')
 
         # determine the target charges for hybrid residues if they are not
         # provided explicitly
         if target_qB is None:
@@ -828,15 +849,15 @@
 
         # write the molecule section, if there are atoms
         if self.atoms:
             self.write_moleculetype(fp)
             self.write_atoms(fp, charges=stateQ, atomtypes=stateTypes,
                              dummy_qA=dummy_qA, dummy_qB=dummy_qB,
                              scale_mass=scale_mass, target_qB=target_qB,
-                             full_morphe=full_morphe, verbose=verbose)
+                             full_morphe=full_morphe, verbose=verbose, qPrec=qPrec)
             self.write_bonds(fp, state=stateBonded)
             if self.have_constraints:
                 self.write_constraints(fp)
             self.write_pairs(fp)
             self.write_angles(fp, state=stateBonded)
             self.write_dihedrals(fp, state=stateBonded)
             # write cmap only if needed/present
@@ -844,14 +865,16 @@
                 self.write_cmap(fp)
             if self.has_vsites2:
                 self.write_vsites2(fp)
             if self.has_vsites3:
                 self.write_vsites3(fp)
             if self.has_vsites4:
                 self.write_vsites4(fp)
+            if self.has_exclusions:
+                self.write_exclusions(fp)
             if self.has_posre:
                 # NOTE: posre are dealt with in 2 ways: via specific posre
                 # readers/writers and via the footer. This may cause issues
                 # at some point. Ideally, all posre should be written with this
                 # function, and no posre as part of the footer
                 self.write_posre(fp, ifdef=posre_ifdef, use_include=posre_include)
 
@@ -1051,15 +1074,19 @@
     def write_nonbond_params(self, fp):
         print('\n[ nonbond_params ]\n; i  j    func  sigma           epsilon', file=fp)
         for param in self.nonbond_params:
             print('{a1:>10}{a2:>10}{func:>5}{sigma:>20.5e}{epsilon:>20.5e}'.format(**param), file=fp)
 
     def write_atoms(self, fp, charges='AB', atomtypes='AB', dummy_qA='on',
                     dummy_qB='on', scale_mass=True, target_qB=[],
-                    full_morphe=True, verbose=False):
+                    full_morphe=True, verbose=False, qPrec=6):
+
+        # number of significant digits for charges in topology
+        if qPrec>10:
+            qPrec=10
 
         self.qA = 0
         self.qB = 0
         for r in self.residues:
             if _is_perturbed_residue(r):
                 try:
                     target_chargeB = target_qB.pop(0)
@@ -1166,21 +1193,21 @@
                     if hasattr(atom, "contQ") and not full_morphe:
                         qqA = atom.contQ
                     else:
                         qqA = atom.qqA
                 else:
                     qqA = atom.q
                     qqB = atom.qB
-                print('%6d %11s%7d%7s%7s%7d%11.6f%11.4f %11s%11.6f%11.4f'
+                print('%6d %11s%7d%7s%7s%7d %11.{0}f%11.4f %11s %11.{0}f%11.4f'.format(qPrec)
                       % (atom.id, atA, atom.resnr, atom.resname,
                          atom.name, atom.cgnr, qqA, mA, atB, qqB, mB), file=fp)
                 self.qA += qqA
                 self.qB += qqB
             else:
-                print('%6d %11s%7d%7s%7s%7d%11.6f%11.4f'
+                print('%6d %11s%7d%7s%7s%7d %11.{0}f%11.4f'.format(qPrec)
                       % (atom.id, atom.atomtype, atom.resnr, atom.resname,
                          atom.name, atom.cgnr, atom.q, atom.m), file=fp)
                 self.qA += atom.q
                 self.qB += atom.q
         # write qB of latom to qA
         if not full_morphe:
             try:
@@ -1376,14 +1403,21 @@
                 elif state == 'BB':
                     print("%6d %6d %6d %6d %4d %s %s ; %s %s %s %s %s %s %s %s (%s->%s)" %
                           (d[0].id, d[1].id, d[2].id, d[3].id, d[4], bs, bs,
                            d[0].name, d[1].name, d[2].name, d[3].name,
                            d[0].type, d[1].type, d[2].type, d[3].type,
                            A, B), file=fp)
 
+    def write_exclusions(self, fp):
+        print('\n[ exclusions ]', file=fp)
+        for excl in self.exclusions:
+            for ex in excl:
+                print("%6d " % (ex.id), end='', file=fp )
+            print("\n", file=fp )
+
     def write_vsites2(self, fp):
         print('\n[ virtual_sites2 ]', file=fp)
         print(';  ai    aj    ak  funct            c0            c1', file=fp)
         for vs in self.virtual_sites2:
             if len(vs) == 4:
                 print("%6d %6d %6d %4d" % (vs[0].id, vs[1].id,
                                            vs[2].id, vs[3]), file=fp)
@@ -1834,14 +1868,100 @@
                 if a.symbol != 'H':
                     self.posre.append([a, 1, '{0:14.6f} {0:14.6f} {0:14.6f}'.format(k)])
             else:
                 self.posre.append([a, 1, '{0:14.6f} {0:14.6f} {0:14.6f}'.format(k)])
 
         self.has_posre = True
 
+    def as_rtp(self):
+        for i, bond in enumerate(self.bonds):
+            id1 = bond[0].id
+            id2 = bond[1].id
+            self.bonds[i][0] = self.atoms[id1-1]
+            self.bonds[i][1] = self.atoms[id2-1]
+        for i, angle in enumerate(self.angles):
+            id1 = angle[0].id
+            id2 = angle[1].id
+            id3 = angle[2].id
+            self.angles[i][0] = self.atoms[id1-1]
+            self.angles[i][1] = self.atoms[id2-1]
+            self.angles[i][2] = self.atoms[id3-1]
+
+        for i, dih in enumerate(self.dihedrals):
+            id1 = dih[0].id
+            id2 = dih[1].id
+            id3 = dih[2].id
+            id4 = dih[3].id
+            self.dihedrals[i][0] = self.atoms[id1-1]
+            self.dihedrals[i][1] = self.atoms[id2-1]
+            self.dihedrals[i][2] = self.atoms[id3-1]
+            self.dihedrals[i][3] = self.atoms[id4-1]
+
+        for i, vs in enumerate(self.virtual_sites2):
+            id1 = dih[0].id
+            id2 = dih[1].id
+            id3 = dih[2].id
+            self.virtual_sites2[i][0] = self.atoms[id1-1]
+            self.virtual_sites2[i][1] = self.atoms[id2-1]
+            self.virtual_sites2[i][2] = self.atoms[id3-1]
+
+
+    def write_rtp(self, filename ='mol.rtp'):
+        fp = open(filename,'w')
+        fp.write('[ {0} ]\n'.format(self.name))
+        fp.write(' [ atoms ]\n')
+        for atom in self.atoms:
+            fp.write("%8s %-12s %8.6f %5d\n" % \
+                  (atom.name,atom.atomtype,atom.q,atom.cgnr) )
+
+        fp.write(' [ bonds ]\n')
+        for bond in self.bonds:
+            if len(bond)<=3:
+                fp.write("%8s %8s\n"% \
+                      (bond[0].name, bond[1].name) )
+            else:
+                fp.write("%8s %8s %8.4f %8.4f\n"% \
+                      (bond[0].name, bond[1].name, bond[3][0], bond[3][1]) )
+
+        fp.write(' [ angles ]\n')
+        for angle in self.angles:
+            if len(angle)<=4:
+                fp.write("%8s %8s %8s\n"% \
+                      (angle[0].name, angle[1].name,angle[2].name) )
+            elif angle[3]==5: # U-B
+                fp.write("%8s %8s %8s %8.4f %8.4f %8.4f %8.4f\n"% \
+                      (angle[0].name, angle[1].name,angle[2].name,
+                        angle[4][0],angle[4][1],angle[4][2],angle[4][3]) )
+            else:
+                fp.write("%8s %8s %8s %8.4f %8.4f\n"% \
+                      (angle[0].name, angle[1].name,angle[2].name,angle[4][0],angle[4][1]) )
+
+
+        fp.write(' [ dihedrals ]\n')
+        for dih in self.dihedrals:
+            if len(dih)<=5: # no parameters
+                fp.write("%8s %8s %8s %s\n"% \
+                      (dih[0].name, dih[1].name,dih[2].name, dih[3].name))
+            elif dih[4]==3:
+                param = dih[5].split()
+                fp.write("%8s %8s %8s %s %8.4f %8.4f %8.4f %8.4f %8.4f %8.4f\n"% \
+                      (dih[0].name, dih[1].name,dih[2].name, dih[3].name, float(param[0]), float(param[1]), float(param[2]), float(param[3]), float(param[4]), float(param[5])) )
+            elif (dih[4]==1) or (dih[4]==4) or (dih[4]==9):
+                param = dih[5].split()
+                fp.write("%8s %8s %8s %s %8.4f %8.4f %8.4f\n"% \
+                      (dih[0].name, dih[1].name,dih[2].name, dih[3].name,
+                       float(param[0]), float(param[1]), float(param[2])) )
+            elif (dih[4]==2) or (dih[4]==11):
+                param = dih[5].split()
+                fp.write("%8s %8s %8s %s %8.4f %8.4f\n"% \
+                      (dih[0].name, dih[1].name,dih[2].name, dih[3].name,
+                       float(param[0]), float(param([1]))) )
+
+
+
 class MDPError(Exception):
     """MDP Error class.
     """
     def __init__(self, s):
         self.s = s
 
     def __str__(self):
```

### Comparing `pmx_biobb-1.0.1/src/pmx/geometry.py` & `pmx_biobb-2.0.0/src/pmx/geometry.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/gmx.py` & `pmx_biobb-2.0.0/src/pmx/gmx.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,28 +186,28 @@
         other_flags += ' -neutral'
 
     call('echo "SOL" | {gmx} genion -s {s} -p {p} -o {o} -np {np} -nn {nn} -conc {conc} '
          '{other_flags}'.format(gmx=gmx, s=s, p=p, o=o, np=np, nn=nn, conc=conc, other_flags=other_flags),
          shell=True)
 
 
-def trjconv(f, s, o='trjconv.xtc', ur='rect', pbc='none', fit='none',
+def trjconv(f, s, o='trjconv.xtc', ur='compact', pbc='none', fit='none',
             out_grp='System', fit_grp='C-alpha', sep=False, other_flags=''):
     """Simple ``gmx trjconv`` wrapper.
 
     Parameters
     ----------
     f : str
         input structure of trajectory file
     s : str
         input tpr file
     o : str, optional
         output trajectory/structure file. Default is "trjconv.xtc"
     ur : str, optional
-        unit-cell representation: rect, tric, compact. Default is 'rect'.
+        unit-cell representation: rect, tric, compact. Default is 'compact'.
     pbc : str, optional
         PBC treatment: none, mol, res, atom, nojump, cluster, whole.
         Default is 'none'.
     fit : str, optional
         fit molecule to ref structure in the structure file: none, rot+trans,
         rotxy+transxy, translation, transxy, progressive.
         Default is 'none'.
@@ -230,19 +230,19 @@
 
     gmx = get_gmx()
 
     if sep is True:
         other_flags += ' -sep'
 
     if fit == 'none':
-        call('echo "{out_grp}" | {gmx} trjconv -f {f} -s {s} -o {o} -ur {ur} -pdb {pbc}'
+        call('echo "{out_grp}" | {gmx} trjconv -f {f} -s {s} -o {o} -ur {ur} -pbc {pbc}'
              '{other_flags}'.format(gmx=gmx, f=f, s=s, o=o, ur=ur, pbc=pbc, out_grp=out_grp, other_flags=other_flags),
              shell=True)
     else:
-        call('echo "{fit_grp}" "{out_grp}" | {gmx} trjconv -f {f} -s {s} -o {o} -ur {ur} -pdb {pbc} -fit {fit}'
+        call('echo "{fit_grp}" "{out_grp}" | {gmx} trjconv -f {f} -s {s} -o {o} -ur {ur} -pbc {pbc} -fit {fit}'
              '{other_flags}'.format(gmx=gmx, f=f, s=s, o=o, ur=ur, pbc=pbc, fit=fit,
                                     out_grp=out_grp, fit_grp=fit_grp, other_flags=other_flags),
              shell=True)
 
 
 def mdrun(s, deffnm='md', verbose=False, other_flags=''):
     """Simple ``gmx mdrun`` wrapper.
```

### Comparing `pmx_biobb-1.0.1/src/pmx/library.py` & `pmx_biobb-2.0.0/src/pmx/library.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/model.py` & `pmx_biobb-2.0.0/src/pmx/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 import numpy as np
 from . import _pmx as _p
 from . import library
 from . import chain
 from .atomselection import Atomselection
 from .molecule import Molecule
 from .atom import Atom
+from string import digits
 
 
 __all__ = ['Model']
 
 
 class Model(Atomselection):
     """Model Class.
@@ -121,14 +122,17 @@
         discontinuous residue indices(?). Default is True.
     bNoNewID : bool
         whether to assign new chain IDs? If True, new chain IDs starting
         with 'pmx' will be assigned(?). Only relevant if bPDBTER is True.
         Default is True.
     bPDBGAP : bool
         whether search for gaps in the chain to assign new chain IDs.
+    bPDBMASS : bool
+        whether to guess masses from the atom library (will fail for
+        complex atom naming, e.g. ND will not be interpreted as nitrogen)
 
     Attributes
     ----------
     title : str
         title of model. Default is 'PMX MODEL'.
     filename : str
         filename from which the Model was imported, otherwise None.
@@ -144,15 +148,15 @@
         3x3 array containing the box vectors. See Gromacs manual, Table 3.1
     moltype : str
         Type of system: protein, dna, rna, or unknown if organic molecule or
         a mix of molecules are in the system.
     """
     def __init__(self, filename=None, pdbline=None, renumber_atoms=True,
                  renumber_residues=True, rename_atoms=False, scale_coords=None,
-                 bPDBTER=True, bNoNewID=True, bPDBGAP=False,
+                 bPDBTER=True, bNoNewID=True, bPDBGAP=False, bPDBMASS=False,
                  **kwargs):
 
         Atomselection.__init__(self)
         self.title = 'PMX MODEL'
         self.filename = filename
         self.chains = []
         self.chdic = {}
@@ -162,15 +166,15 @@
         self.have_bonds = 0  # FIXME/QUESTION: same as above: never used -> remove?
         self.box = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
         self.unity = 'A'
         for key, val in kwargs.items():
             setattr(self, key, val)
 
         if filename is not None:
-            self.read(filename=filename, bPDBTER=bPDBTER, bNoNewID=bNoNewID, bPDBGAP=bPDBGAP)
+            self.read(filename=filename, bPDBTER=bPDBTER, bNoNewID=bNoNewID, bPDBGAP=bPDBGAP, bPDBMASS=bPDBMASS)
         if pdbline is not None:
             self.__readPDB(pdbline=pdbline)
         if self.atoms:
             self.unity = self.atoms[0].unity
             self.make_chains()
             self.make_residues()
         if self.residues and not self.atoms:
@@ -200,14 +204,16 @@
             elif scale_coords == 'nm':
                 self.a2nm()
             else:
                 raise ValueError('unknown unit %s for coordinates' % scale_coords)
 
         self.assign_moltype()
 
+
+
     def __str__(self):
         s = '< Model: moltype=%s, nchain=%d, nres=%d, natom=%d >' %\
             (self.moltype, len(self.chains), len(self.residues),
              len(self.atoms))
         return s
 
     def writePIR(self, filename, title=""):
@@ -402,22 +408,23 @@
                 return(True)
             if int(str1[0:-1])==int(str2[0:-1])-1: # 52A, 53B
                 return(True)
         return(False)
         
     # TODO: make readPDB and readPDBTER a single function. It seems like
     # readPDBTER is more general PDB reader?
-    def __readPDBTER(self, fname=None, pdbline=None, bNoNewID=True, bPDBGAP=False):
+    def __readPDBTER(self, fname=None, pdbline=None, bNoNewID=True, bPDBGAP=False, bPDBMASS=False):
         """Reads a PDB file with more options than __readPDB ?"""
         if pdbline:
             lines = pdbline.split('\n')
         else:
             lines = open(fname, 'r').readlines()
 
-        chainIDstring = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnoprstuvwxyz123456789'
+        chainIDstringInit = 'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnoprstuvwxyz123456789'
+        chainIDstring = copy.deepcopy(chainIDstringInit)
         bNewChain = True
         chainID = ' '
         prevID = ' '
         prevAtomName = ' '
         prevResID = 0
         prevResName = ' '
         usedChainIDs = []
@@ -431,37 +438,52 @@
                 a = Atom().readPDBString(line, origID=atomcount)
                 atomcount += 1
                 # identify chain change by ID (when no TER is there)
                 if (a.chain_id != prevID):
                     bNewChain = True
                 if (self.__check_if_gap( prevCatom,a )==True and bPDBGAP==True):
                     bNewChain = True
+                if a.resname=='ACE' and prevResName!='ACE':
+                    bNewChain = True
                 if (a.resnr != prevResID):
                     try:
                         if self.__compareWithoutLastChar(prevResID,a.resnr)==True: # there are some special cases where residues are named, e.g. 52, 52A, 52B, ...
                             bNewChain = False
                         elif a.resnr != prevResID+1:
                             bNewChain = True
                         if (prevAtomName == 'OC2') or (prevAtomName == 'OXT') or (prevAtomName == 'OT2'):
                             bNewChain = True
                         if (prevAtomName == 'HH33') and ((prevResName=='NME') or (prevResName=='NAC') or (prevResName=='CT3')): # NME cap
                             bNewChain = True
+                        # do not assign new chain IDs for waters, ions 
+                        if (a.resname=='WAT') or (a.resname=='SOL') or (a.resname=='TIP3') or (a.resname=='HOH') \
+                           or (a.resname=='NA') or (a.resname=='CL') \
+                           or (a.resname=='NaJ') or (a.resname=='Na') or (a.resname=='Cl') or (a.resname=='K') or (a.resname=='KJ') \
+                           or (a.resname=='MG') or (a.resname=='Mg') or (a.resname=='CA') or (a.resname=='Ca') or (a.resname=='CaJ') \
+                           or (a.resname=='ZN') or (a.resname=='Zn'): # add other ions when needed
+                            bNewChain = False
+                            chainID = ''
                     except TypeError:
                         bNewChain = False
+                        chainID = ''
                 prevID = a.chain_id
                 prevResID = a.resnr
                 prevAtomName = a.name
                 prevResName = a.resname
                 if a.name == 'C':
                     prevCatom = a
                 if bNewChain==True:
                     if ((a.chain_id==' ') or (a.chain_id==chainID) or (a.chain_id in usedChainIDs) and bNoNewID==False):
                         # find a new chain id
                         bFound = False
                         while bFound==False:
+                            if len(chainIDstring)==0: # used up all the IDs
+                                chainIDstring = copy.deepcopy(chainIDstringInit)
+                                chainID = "pmxX"
+                                break
                             foo = chainIDstring[0]
                             chainIDstring = chainIDstring.lstrip(chainIDstring[0])
                             if foo not in usedChainIDs:
                                 bFound=True
                                 chainID = foo
                                 if bNoNewID==True:
                                     chainID = "pmx"+foo
@@ -485,26 +507,35 @@
                 if a.chain_id in newChainDict.keys():
                     a.chain_id = newChainDict[a.chain_id]
                 # ID not yet encountered
                 else:
                     # find a suitable ID
                     bFound = False
                     while bFound==False:
+                        if len(chainIDstring)==0: # used up all the IDs
+                            chainIDstring = copy.deepcopy(chainIDstringInit)
+                            newChainDict[a.chain_id] = "X"
+                            a.chain_id = "X"
+                            break
                         foo = chainIDstring[0]
                         chainIDstring = chainIDstring.lstrip(chainIDstring[0])
                         # found
                         if foo not in usedChainIDs:
                             bFound=True
                             usedChainIDs.append(foo)
                             newChainDict[a.chain_id] = foo
                             a.chain_id = foo
 
         self.make_chains()
         self.make_residues()
         self.unity = 'A'
+
+        if bPDBMASS==True:
+            assign_masses_to_model( self )
+
         return self
 
     def __readGRO(self, filename):
         """Reads a GRO file"""
         l = open(filename).readlines()
         # first line is name/comment
         name = l[0].rstrip()
@@ -580,15 +611,15 @@
         elif bool(residues) and residues <= library._dna_residues:
             self.moltype = 'dna'
         elif bool(residues) and residues <= library._rna_residues:
             self.moltype = 'rna'
         else:
             self.moltype = 'unknown'
 
-    def read(self, filename, bPDBTER=False, bNoNewID=True, bPDBGAP=False):
+    def read(self, filename, bPDBTER=False, bNoNewID=True, bPDBGAP=False, bPDBMASS=False):
         """PDB/GRO file reader.
 
         Parameters
         ----------
         filename : str
             name of input file
         bPDBTER : bool, optional
@@ -601,15 +632,15 @@
             whether search for gaps in the chain to assign new chain IDs.
         """
         ext = filename.split('.')[-1]
         if ext == 'pdb':
             if bPDBTER is True:
                 return self.__readPDBTER(fname=filename,
                                          pdbline=None,
-                                         bNoNewID=bNoNewID, bPDBGAP=bPDBGAP)
+                                         bNoNewID=bNoNewID, bPDBGAP=bPDBGAP, bPDBMASS=bPDBMASS)
             else:
                 return self.__readPDB(fname=filename)
         elif ext == 'gro':
             return self.__readGRO(filename)
         else:
             raise IOError('ERROR: Can only read pdb or gro!')
 
@@ -927,30 +958,40 @@
     model.unity = model.atoms[0].unity
     model.make_chains()
     model.make_residues()
     model.assign_moltype()
     return model
 
 
-def assign_masses_to_model(model, topology):
+def assign_masses_to_model(model, topology=None):
     '''Assigns masses to the Model atoms given the ones present in the Topology.
 
     Parameters
     ----------
     model : Model
         Model object of the molecule.
     topology : Topology
-        Topology object of the same molecule.
+        Topology object of the same molecule. When no topology provided, standard library masses are used.
     '''
-    for ma, ta in zip(model.atoms, topology.atoms):
-        if ma.name != ta.name:
-            raise ValueError('mismatch of atom names between Model and '
-                             'Topology objects provided')
-        ma.m = ta.m
-
+    
+    if topology!=None:
+        for ma, ta in zip(model.atoms, topology.atoms):
+            if ma.name != ta.name:
+                raise ValueError('mismatch of atom names between Model and '
+                                 'Topology objects provided')
+            ma.m = ta.m
+    else:
+        for a in model.atoms:
+            aname = a.name
+            aname = aname.upper()
+            aname = aname.translate(str.maketrans('','',digits))
+            if aname not in library._atommass.keys():
+                a.m = 0.0
+            else:
+                a.m = library._atommass[aname]
 
 def double_box(m1, m2, r=2.5, d=1.5, bLongestAxis=False, verbose=False):
     '''Places two structures (two Model objects) into a single box.
     The box is a rectangular cuboid in which the two structures are placed in
     such a way to minimise the box volume.
 
     Parameters
```

### Comparing `pmx_biobb-1.0.1/src/pmx/molecule.py` & `pmx_biobb-2.0.0/src/pmx/molecule.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/mutdb.py` & `pmx_biobb-2.0.0/src/pmx/mutdb.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/ndx.py` & `pmx_biobb-2.0.0/src/pmx/ndx.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/options.py` & `pmx_biobb-2.0.0/src/pmx/options.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/parser.py` & `pmx_biobb-2.0.0/src/pmx/parser.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/rotamer.py` & `pmx_biobb-2.0.0/src/pmx/rotamer.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/analyze_dhdl.py` & `pmx_biobb-2.0.0/src/pmx/scripts/analyze_dhdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     parser.add_argument('-b',
                         metavar='nboots',
                         dest='nboots',
                         type=int,
                         help='Number of bootstrap samples to use for the '
                         'bootstrap estimate of the standard errors. Default '
                         'is 0 (no bootstrap).',
-                        default=0)
+                        default=100)
     parser.add_argument('-n',
                         metavar='nblocks',
                         dest='nblocks',
                         type=int,
                         help='Number of blocks to divide the data into for '
                         'an estimate of the standard error. You can use this '
                         'when multiple independent equilibrium simulations'
@@ -539,14 +539,16 @@
         if nblocks > 1:
             _tee(out, '  BAR: Std Err (blocks)  = {e:8.{p}f} {u}'.format(e=bar.err_blocks*unit_fact, p=prec, u=units), quiet=quiet)
 
         _tee(out, '  BAR: Conv = %8.2f' % bar.conv, quiet=quiet)
 
         if nboots > 0:
             _tee(out, '  BAR: Conv Std Err (bootstrap) = %8.2f' % bar.conv_err_boot, quiet=quiet)
+        if nblocks > 1:
+            _tee(out, '  BAR: Conv Std Err (blocks) = %8.2f' % bar.conv_err_blocks, quiet=quiet)
 
     # =========
     # Jarzynski
     # =========
     if 'jarz' in methods:
         _tee(out, '\n --------------------------------------------------------', quiet=quiet)
         _tee(out, '             Jarzynski estimator     ', quiet=quiet)
```

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/cli.py` & `pmx_biobb-2.0.0/src/pmx/scripts/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,23 +12,26 @@
         parser = ArgumentParser(
             description='''
     ------------------------
     pmx command line scripts
     ------------------------
 
     Available commands are:
-        mutate       Mutate protein or DNA/RNA
-        gentop       Fill hybrid topology with B states
-        analyse      Estimate free energy from Gromacs xvg files
+        mutate        Mutate protein or DNA/RNA
+        gentop        Fill hybrid topology with B states
+        analyse       Estimate free energy from Gromacs xvg files
 
-        doublebox    Place two input structures into a single box
-        abfe         Setup files for an ABFE calculation
+        atomMapping   Ligand alchemy: map atoms for morphing
+        ligandHybrid  Ligand alchemy: hybrid structure/topology
 
-        genlib       Generate pmx ff library
-        gmxlib       Show/set GMXLIB path''',
+        doublebox     Place two input structures into a single box
+        abfe          Setup files for an ABFE calculation
+
+        genlib        Generate pmx ff library
+        gmxlib        Show/set GMXLIB path''',
             formatter_class=RawTextHelpFormatter)
 
         parser.add_argument('-v', '--version', action='version',
                             version=__version__)
         parser.add_argument('command', help=SUPPRESS)
         # parse_args defaults to [1:] for args, but you need to
         # exclude the rest of the args too, or validation will fail
@@ -48,14 +51,22 @@
         from . import generate_hybrid_topology
         generate_hybrid_topology.entry_point()
 
     def analyse(self):
         from . import analyze_dhdl
         analyze_dhdl.entry_point()
 
+    def atomMapping(self):
+        from . import atomMapping
+        atomMapping.entry_point()
+
+    def ligandHybrid(self):
+        from . import ligandHybrid
+        ligandHybrid.entry_point()
+
     def doublebox(self):
         from . import make_double_box
         make_double_box.entry_point()
 
     def abfe(self):
         from . import setup_abfe
         setup_abfe.entry_point()
@@ -70,15 +81,15 @@
 
 
 def check_unknown_cmd(unknowns):
     '''Checks unknown command line arguments are raises a warning if unexpected
     commands are found.
     '''
     expected = ['pmx', 'analyse', 'mutate', 'doublebox', 'gentop', 'gmxlib',
-                'genlib', 'abfe']
+                'genlib', 'abfe', 'atomMapping', 'ligandHybrid']
 
     for cmd in unknowns:
         if cmd not in expected:
             print('Unknown command found in your command line: "{}". '
                   'This command will be ignored'.format(cmd))
```

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/generate_hybrid_residue.py` & `pmx_biobb-2.0.0/src/pmx/scripts/generate_hybrid_residue.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/generate_hybrid_topology.py` & `pmx_biobb-2.0.0/src/pmx/scripts/generate_hybrid_topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,24 +140,24 @@
     topol = Topology(top_file, ff=ff, version='new')
 
     # fill the B states
     pmxtop, pmxitps = gen_hybrid_top(topol=topol, recursive=recursive,
                                      verbose=True, scaleDih=scaleDih)
 
     # get the base path for the .itp file output
-    basepath = outfile.rsplit('/',1)[0]
+    basepath = os.path.abspath(outfile).rsplit('/',1)[0]
 
     # write hybrid itps if present
     replace = {}
     if len(pmxitps) > 0:
         for pmxitp in pmxitps:
             itp_fn = os.path.basename(pmxitp.filename)
             out_fn = '{0}/pmx_{1}'.format(basepath,itp_fn)
             # store old/new itp names for replacement in top file
-            replace[itp_fn] = out_fn
+            replace[itp_fn] = 'pmx_{0}'.format(itp_fn) #out_fn
             print('\nlog_> Writing itp file "%s""' % out_fn)
             pmxitp.write(out_fn, scale_mass=scale_mass)
 
     # write hybrid topology
     print('\nlog_> Writing topology file "%s""' % outfile)
     pmxtop.write(outfile, scale_mass=scale_mass)
```

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/make_double_box.py` & `pmx_biobb-2.0.0/src/pmx/scripts/make_double_box.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/md_setup.py` & `pmx_biobb-2.0.0/src/pmx/scripts/md_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,28 +187,28 @@
         self.mutations = []
         if self.mutation_tags:
             self.mutations_from_tags()
         self.runs = []
         self.is_single_chain = False
         
     def read_mutation_file(self, mut_file ):
-        print ('\n\t\t\tReading mutation file: %s\n' % mut_file)
+        print '\n\t\t\tReading mutation file: %s\n' % mut_file
         l = open(mut_file).readlines()
         count = 1
         for line in l:
             entr = line.strip()
             if entr:
-                print('\t\t\t (%d) ->  %s' % (count, entr))
+                print '\t\t\t (%d) ->  %s' % (count, entr)
                 self.mutation_tags.append( entr )
                 count+=1
         
 
     def setup(self):
         self.read_pdb()
-        print( '\n\n')
+        print '\n\n'
         for m in self.mutations:
             self.setup_mutation_run(m)
 
     def read_pdb( self ):
         self.model = Model(self.md_in_conf)
         if len(self.model.chains) == 1:
             self.is_single_chain = True
@@ -234,15 +234,15 @@
             if chain not in affected_chains:
                 affected_chains.append( chain )
         name = '-'.join(muts)
         if str(self.__class__).split('.')[1] == 'DiscreteTI':
             name+='.dti'
         elif str(self.__class__).split('.')[1] == 'CrooksMD':
             name+='.crooks'
-        print ('\n\t\t\tPreparing mutation run -> %s \n' % name)
+        print '\n\t\t\tPreparing mutation run -> %s \n' % name
         if os.path.isdir( name ):
             shutil.rmtree(name)
         os.mkdir(name)
         self.runs.append( name )
         shutil.copy(self.md_in_conf, name)
         script_file = os.path.join(name,'mutations.txt')
         fp = open(script_file,'w')
@@ -262,15 +262,15 @@
             itp_file = 'topol_Protein.itp' 
             run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
             run_command( self.make_mutation, run )
             shutil.move(itp_file, itp_file+'.save')
             shutil.move('newtop.itp', itp_file)
         else:
             for chain in affected_chains:
-                print ('Applying changes to topology of chain %s' % chain)
+                print 'Applying changes to topology of chain %s' % chain
                 itp_file = 'topol_Protein_chain_%s.itp' % chain
                 run = '~/software/pmx/scripts/make_bstate_beta45.py -itp %s' % itp_file
                 run_command( self.make_mutation, run )
                 shutil.move(itp_file, itp_file+'.save')
                 shutil.move('newtop.itp', itp_file)
         os.chdir('..')            
         
@@ -285,30 +285,30 @@
 
     def do_crooks( self, mdp_file, min_mdp_file, time, nruns ):
         mdp = MDP().read( mdp_file)
         min_mdp = MDP().read( min_mdp_file)
         self.prepare_min_mdp_files(min_mdp, time )
         self.prepare_eq_mdp_files(mdp, time )
         for r in self.runs:
-            print ('\n\t\t\tSetting up Crooks run -> %s\n' % r)
+            print '\n\t\t\tSetting up Crooks run -> %s\n' % r
 
             self.minimize_states( r )
             self.setup_equilibration_runs( r, nruns )
         
     def minimize_states( self, path ):
 
         os.chdir(path)
         run = 'grompp -f ../crooks_minA.mdp -c gmx.pdb -o minA.tpr'
         run_command( self.minimize_states, run )
         run = 'grompp -f ../crooks_minB.mdp -c gmx.pdb -o minB.tpr'
         run_command( self.minimize_states, run )
-        print ('\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path ))
+        print '\n\t\t\tRunning energy minimization on %s ( state A ) \n' % ( path )
         run = 'mdrun -v -c emA.pdb -s minA.tpr'
         run_command( self.minimize_states, run )
-        print ('\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path ))
+        print '\n\t\t\tRunning energy minimization on %s ( state B ) \n' % ( path )
         run = 'mdrun -v -c emB.pdb -s minB.tpr'
         run_command( self.minimize_states, run )
         os.chdir('..')
         
     def prepare_eq_mdp_files( self, mdp, time ):
         nsteps = 1000*time/.002
         mdp['nsteps'] = nsteps
@@ -331,15 +331,15 @@
         print >>fp, mdp
         fp.close()
 
         
     def setup_equilibration_runs( self, path, nruns ):
         os.chdir(path)
         for i in range(nruns):
-            print ('\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i ))
+            print '\n\t\t\tPreparing run input file for  %s ( run %d ) \n' % ( path, i )
             os.mkdir('runA.%d' % i)
             os.mkdir('runB.%d' % i)
             run = 'grompp -f ../crooks_eqA.mdp -c emA.pdb -o runA.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             run = 'grompp -f ../crooks_eqB.mdp -c emB.pdb -o runB.%d/topol.tpr' % i
             run_command( self.setup_equilibration_runs, run )
             self.clean_backups()
@@ -382,32 +382,32 @@
     def setup_runs( self, path ):
         os.chdir( path )
         for lda in self.lambda_steps:
             min_mdp = 'dti_min_%4.3f.mdp' % round(lda,3)
             run_mdp = 'dti_%4.3f.mdp' % round(lda,3)
             run_dir = 'run_%4.3f' % round(lda,3)
             os.mkdir( run_dir )
-            print ('\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir ))
+            print '\n\t\t\tRunning energy minimization on %s/%s \n' % ( path, run_dir )
             run = 'grompp -f ../%s -c gmx.pdb -o %s/em.tpr' % (min_mdp, run_dir )
             run_command( self.setup_runs, run )
             os.chdir( run_dir )
             run = 'mdrun -v -c em.pdb -s em.tpr'
             run_command( self.setup_runs, run )
             os.chdir('..')
-            print ('\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir ))
+            print '\n\t\t\tPreparing run input file for  %s/%s \n' % ( path, run_dir )
             run = 'grompp -f ../%s -c %s/em.pdb -o %s/topol.tpr' % (run_mdp, run_dir, run_dir )
             run_command( self.setup_runs, run )
             self.clean_backups()
         os.chdir( '..')
         
     def do_dti( self, mdp, min_mdp, time ):
         self.prepare_dti_min_mdp_files( min_mdp)
         self.prepare_dti_mdp_files( mdp, time)
         for r in self.runs:
-            print ('\n\t\t\tSetting up Discrete TI run -> %s\n' % r)
+            print '\n\t\t\tSetting up Discrete TI run -> %s\n' % r
             self.setup_runs( r )
 
 
         
 def main(argv):
 
     version = "1.0"
@@ -480,15 +480,15 @@
 
     if not cmdl['-skip_md_setup']:
         md = MD( pdb_in = pdb_in, water = water, conc = conc, box_type = box_type, box_size = box_size )
         md.setup()
         free_energy_start_pdb = md.md_in_conf
     else:
         if not bFreeEnergy:
-            print ('Nothing to do........... (no MD, no Free Energy)')
+            print 'Nothing to do........... (no MD, no Free Energy)'
             sys.exit()
     if bFreeEnergy:
         if not free_energy_start_pdb:
             free_energy_start_pdb = pdb_in
         if cmdl['-fe.crooks']:
             crooksMD = CrooksMD( mutation_file, md_in_conf = free_energy_start_pdb)
             crooksMD.setup()
@@ -497,15 +497,15 @@
         if cmdl['-fe.dti']:
             dti = DiscreteTI( mutation_file, md_in_conf = free_energy_start_pdb )
             dti.setup()
             dti.read_lambda_steps( cmdl['-lambda_steps'] )
             dti.do_dti(cmdl['-dti_mdp'], cmdl['-min_mdp'], cmdl['-dti_run_time'] )
 
 
-    print ('\n\t\t\t ....... DONE .......... \n')
+    print '\n\t\t\t ....... DONE .......... \n'
     
 
 
 ##     n_crooks_runs = cmdl['-n_crooks_runs']
 ##     if cmdl.opt['-m'].is_set:
 ##         mut_file  = cmdl['-m']
 ##     else:
```

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/mutate.py` & `pmx_biobb-2.0.0/src/pmx/scripts/mutate.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/prepare_crooks_runs.py` & `pmx_biobb-2.0.0/src/pmx/scripts/prepare_crooks_runs.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,23 +47,23 @@
         print >>sys.stderr, 'Output written to %s' % err_file
         fp = open(err_file, 'w')
         print >>fp, s
         print >>fp, out
         fp.close()
         sys.exit(1)
     else:
-        print ("%-90s" % s, ': ok')
+        print "%-90s" % s, ': ok'
 
 
 def make_dir_tree(skip=4):
 
     # catch all run?.? dirs
     dirs = glob('run?.?')
     for d in dirs:
-        print ('\tPreparing run %s' % d)
+        print '\tPreparing run %s' % d
         os.chdir(d)
         os.mkdir('morphes')
         cmd = 'echo 0| trjconv -f traj.trr -s topol.tpr -skip %d -b 2001 -sep -o morphes/frame.gro' % skip
         run_command(make_dir_tree, cmd)
         os.chdir('morphes')
 
         # put each file into single directory
@@ -105,15 +105,15 @@
     fp.close()
 
 
 def make_run_input_files():
 
     dirs = glob('run?.?')
     for d in dirs:
-        print ('\n\tPreparing run input files %s' % d)
+        print '\n\tPreparing run input files %s' % d
         mdp_file = None
         if d.split('.')[0][-1] == 'A':  # 0->1
             mdp_file = 'crooks_TI_runA.mdp'
         elif d.split('.')[0][-1] == 'B':  # 1->0
             mdp_file = 'crooks_TI_runB.mdp'
         dir_list = glob(os.path.join(d, 'morphes')+'/frame*')
         for f in dir_list:
@@ -189,32 +189,32 @@
 
     run_dir = args.dir
     mdp_file = args.mdp
     sw_time = args.sw_time
     sc_alpha = args.sc_alpha
     sc_sigma = args.sc_sigma
 
-    print ('\n\t Preparing FGTI runs in directory..: %s' % run_dir)
-    print ('\t Template mdp file to use............: %s' % mdp_file)
-    print ('\t Switching time to use...............: %8d ps' % int(sw_time))
-    print ('\t Soft-core alpha to use..............: %8.3f' % sc_alpha)
-    print ('\t Soft-core sigma to use..............: %8.3f' % sc_sigma)
-    print ('\n')
+    print '\n\t Preparing FGTI runs in directory..: %s' % run_dir
+    print '\t Template mdp file to use............: %s' % mdp_file
+    print '\t Switching time to use...............: %8d ps' % int(sw_time)
+    print '\t Soft-core alpha to use..............: %8.3f' % sc_alpha
+    print '\t Soft-core sigma to use..............: %8.3f' % sc_sigma
+    print '\n'
 
 
     os.chdir(run_dir)
 
-    print ('\t Preparing mdp input files........... ')
+    print '\t Preparing mdp input files........... '
 
     prepare_mdp_files(mdp_file, sw_time, sc_alpha, sc_sigma)
 
 
-    print ('\t Preparing directory tree............ ')
+    print '\t Preparing directory tree............ '
     make_dir_tree(skip=args.skip)
     make_run_input_files()
     os.chdir(here)
-    print ('\n\t............... DONE .................\n')
+    print '\n\t............... DONE .................\n'
 
 
 if __name__ == '__main__':
     args = parse_options()
     main(args)
```

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/set_gmxlib.py` & `pmx_biobb-2.0.0/src/pmx/scripts/set_gmxlib.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/scripts/setup_abfe.py` & `pmx_biobb-2.0.0/src/pmx/scripts/setup_abfe.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx/utils.py` & `pmx_biobb-2.0.0/src/pmx/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,61 @@
 import logging
 from glob import glob
 
 
 # =============
 # File IO utils
 # =============
+
+def clean_gromacs_backup_files( path ):
+    """Clean gromacs backup files.
+
+    Parameters
+    ----------
+    path: str
+        path where to delete files starting with #
+    """
+
+    toclean = glob('{0}/*#'.format(path)) 
+    for clean in toclean:
+        os.remove(clean)     
+
+def copy_files_folders( source, target ):
+    """Copy files or folders.
+
+    Parameters
+    ----------
+    source: str
+        path to files/folders
+    target: str
+        target path
+    """
+
+    cmd = 'cp {0} {1} -r'.format(source,target)
+    if os.path.isdir(target):
+        cmd = 'cp {0} {1}/. -r'.format(source,target)
+    os.system(cmd)
+
+def create_folder( path, fname=False ):
+    """Create a folder.
+
+    Parameters
+    ----------
+    path: str
+        full path to the folder. Alternatively, if fname is given,
+        folder fname will be created in this path
+    fname: str, optional
+        name of the folder to create
+    """ 
+    if fname==False:
+        if not os.path.exists(path):
+            os.makedirs(path)
+    elif not os.path.exists(path+'/'+fname):
+        os.makedirs(path+'/'+fname)
+
 def show_ff(gmxlib=None):
     """Prints the list of forcefields available in GMXLIB.
 
     Parameters
     ----------
     gmxlib : str, optional
         Path to force field library. If not set explicitly, it is taken from
@@ -93,14 +140,19 @@
             return fp
         except:
             print('No such file %s' % filename)
 
     else:
         return open(filename, mode)
 
+# this function echanges netmount with home
+def remove_netmount( string ): 
+    regexp = re.compile('netmount')
+    string = regexp.sub('home',string)
+    return(string)
 
 def get_ff_path(ff, verbose=False):
     """Get path of force field.
 
     Parameters
     ----------
     ff : str
@@ -318,14 +370,20 @@
 
     os.path.walk(dir, killBackups, (False, True, True, check))
 
 
 # ======
 # Others
 # ======
+def doLog(fp, s, commandName='ligandHybridTop'):
+    l = '{0}__log_> {1}'.format(commandName,s)
+#   print(sys.stderr,l)
+    print(l)
+    fp.write(l+'\n')
+
 def data2gauss(data):
     '''Takes a one dimensional array and fits a Gaussian.
 
     Parameters
     ----------
     data : list
         1D array of values
@@ -490,7 +548,17 @@
         for atom in atoms:
             print('{0.name} {0.resname} {0.atomtype} {0.atomtypeB} {0.type} '
                   '{0.typeB}'.format(atom), file=sys.stderr)
         print('err_> Exiting', file=sys.stderr)
 
     def __str__(self):
         return repr(self.s)
+
+class importError(Exception):
+    """Exceptions class for importing a module.
+    """
+    def __init__(self, s):
+        self.s = "Could not import: {0}".format(s)
+
+    def __str__(self):
+        return repr(self.s)
+
```

### Comparing `pmx_biobb-1.0.1/src/pmx/xdrfile.py` & `pmx_biobb-2.0.0/src/pmx/xdrfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,21 +38,22 @@
 auto_mode = 0
 out_mode = 42
 
 
 class Frame:
 
     def __init__(self, n, mode, x=None, box=None, units=None, v=None, f=None):
+        scale = 1.0
+        if units == 'A':
+            scale = 0.1
+
         # create vector for x
         self.natoms = n
         # x (coordinates)
         if mode == out_mode:
-            scale = 1.0
-            if units == 'A':
-                scale = 0.1
             self.x = ((c_float*3)*n)()
             i = 0
             for a in range(0, self.natoms):
                 for dim in range(0, 3):
                     self.x[a][dim] = scale*x[i]
                     i += 1
         elif mode & mNumPy and mode != out_mode:
@@ -63,16 +64,34 @@
         # dummy v and f for .trr
         self.v_size = c_size_t(0)
         self.f_size = c_size_t(0)
         if mode&mNumPy and mode!=out_mode:
             self.v=empty((n,3),dtype=float32)
             self.f=empty((n,3),dtype=float32)
         else:
-            self.v=c_size_t(0)#((c_float*3)*n)()
-            self.f=c_size_t(0)#((c_float*3)*n)()
+            if(v is not None):
+                self.v=((c_float*3)*n)()
+                if(mode==out_mode):
+                    i = 0
+                    for a in range(0, self.natoms):
+                        for dim in range(0, 3):
+                            self.v[a][dim] = scale*v[i]
+                            i += 1
+            else:
+                self.v=c_size_t(0)
+            if(f is not None):
+                self.f=((c_float*3)*n)()
+                if(mode==out_mode):
+                    i = 0
+                    for a in range(0, self.natoms):
+                        for dim in range(0, 3):
+                            self.f[a][dim] = scale*f[i]
+                            i += 1
+            else:
+                self.f=c_size_t(0)
 
         # box
         if box is not None:
             self.box = (c_float*3*3)()
             for r in range(0,3):
                 for c in range(0,3):
                     self.box[r][c] = box[r][c]
@@ -82,30 +101,50 @@
             self.box = (c_float*3*3)()
 
     def update_box(self, box):
         for i in range(3):
             for k in range(3):
                 box[i][k] = self.box[i][k]
 
-    def update_atoms(self, atom_sel):
+    def update_atoms(self, atom_sel, uv=False, uf=False):
         for i, atom in enumerate(atom_sel.atoms):
             if atom_sel.unity == 'A':
                 atom.x[0] = self.x[i][0]*10
                 atom.x[1] = self.x[i][1]*10
                 atom.x[2] = self.x[i][2]*10
+                if(uv):
+                    atom.v = [v*10 for v in self.v[i]]
+                else:
+                    atom.v=[0,0,0]
+                    
+                if(uf):
+                    atom.f = [f/10. for f in self.f[i]]
+                else:
+                    atom.f=[0,0,0]
+                    
             else:
                 atom.x[0] = self.x[i][0]
                 atom.x[1] = self.x[i][1]
                 atom.x[2] = self.x[i][2]
+                if(uv):
+                    atom.v = [v for v in self.v[i]]
+                else:
+                    atom.v=[0,0,0]
+                
+                if(uf):
+                    atom.f = [f for f in self.f[i]]
+                else:
+                    atom.f=[0,0,0]
+            
 
-    def update( self, atom_sel ):
+    def update( self, atom_sel, uv=False, uf=False ):
         if(len(atom_sel.atoms)!=self.natoms):
             raise ValueError("Model and Trajectory have different numbers of atoms: %d and %d"\
                              %(len(atom_sel.atoms),self.natoms) )
-        self.update_atoms(atom_sel )
+        self.update_atoms(atom_sel, uv,uf )
         self.update_box( atom_sel.box )
 
 
     def get_natoms(self):
         return self.natoms
     def get_time(self):
         return self.time
@@ -178,15 +217,15 @@
               except:
                   raise IOError("neither _xdrio.so nor _xdrio%s could be loaded"%suf)
 
         #difine a proper return type for xdrfile_open, so that python doesn't truncate the file pointer to an integer
         class XDRFILEstruct(Structure):
             pass;
         self.xdr.xdrfile_open.restype = POINTER(XDRFILEstruct)
-        
+
         #TODO: for safety and future ctypes compatability, declare the argument and return types for all c functions called
 
         #open file
         fn_cp=c_char_p(fn.encode('utf-8')); #ctypes needs an explicit conversion of sdtrings, or only first character is visible in C
         if self.mode==out_mode:
             self.xd = self.xdr.xdrfile_open(fn_cp,"w")
         else:
@@ -212,40 +251,43 @@
         if self.mode&mNumPy and self.mode!=out_mode:
             self.xdr.read_xtc.argtypes=[c_int,c_int,POINTER(c_int),POINTER(c_float),
               ndpointer(ndim=2,dtype=float32),ndpointer(ndim=2,dtype=float32),POINTER(c_float)]
             self.xdr.read_trr.argtypes=[c_int,c_int,POINTER(c_int),POINTER(c_float),POINTER(c_float),
               ndpointer(ndim=2,dtype=float32),ndpointer(ndim=2,dtype=float32),
               POINTER(c_float),POINTER(c_float)]
 
-    def write_xtc_frame( self, step=0, time=0.0, prec=1000.0, lam=0.0, box=False, x=False, units='A', bTrr=False ):
-        f = Frame(self.natoms,self.mode,box=box,x=x,units=units)
+    def write_xtc_frame( self, step=0, time=0.0, prec=1000.0, lam=0.0, box=None, x=None, v=None, f=None, units='A', bTrr=False ):
+        f = Frame(self.natoms,self.mode,box=box,x=x,v=v,f=f,units=units)
         step = c_int(step)
         time = c_float(time)
         prec = c_float(prec)
         lam = c_float(lam)
         if bTrr:
             result = self.xdr.write_trr(self.xd,self.natoms,step,time,lam,f.box,f.x,f.v,f.f)
         else:
             result = self.xdr.write_xtc(self.xd,self.natoms,step,time,f.box,f.x,prec)
 
     def __iter__(self):
-        f = Frame(self.natoms,self.mode)
+        if( self.mode&mTrr):
+            f = Frame(self.natoms,self.mode, v=True, f=True)
+        else:
+            f = Frame(self.natoms,self.mode)
         #temporary c_type variables (frame variables are python type)
         step = c_int()
         time = c_float()
         prec = c_float()
         lam = c_float()
         if self.mode!=out_mode:
             while 1:
                 #read next frame
                 if not self.mode&mTrr:
                     result = self.xdr.read_xtc(self.xd,self.natoms,byref(step),byref(time),f.box,f.x,byref(prec))
                     f.prec=prec.value
                 else:
-                    result = self.xdr.read_trr(self.xd,self.natoms,byref(step),byref(time),byref(lam),f.box,f.x,None,None) #TODO: make v,f possible
+                    result = self.xdr.read_trr(self.xd,self.natoms,byref(step),byref(time),byref(lam),f.box,f.x,f.v,f.f) #TODO: make v,f possible
                     f.lam=lam.value
 
                 #check return value
                 if result==self.exdrENDOFFILE: break
                 if result==self.exdrINT and self.mode&mTrr:
                   break  #TODO: dirty hack. read_trr return exdrINT not exdrENDOFFILE
                 if result!=self.exdrOK: raise IOError("Error reading xdr file")
```

### Comparing `pmx_biobb-1.0.1/src/pmx/xtc.py` & `pmx_biobb-2.0.0/src/pmx/xtc.py`

 * *Files identical despite different names*

### Comparing `pmx_biobb-1.0.1/src/pmx_biobb.egg-info/PKG-INFO` & `pmx_biobb-2.0.0/src/pmx_biobb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,81 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pmx-biobb
-Version: 1.0.1
+Version: 2.0.0
 Summary: Toolkit for free-energy calculation setup/analysis and biomolecular structure handling
 Home-page: https://github.com/deGrootLab/pmx/tree/develop
 Author: Daniel Seeliger
 Author-email: seeliger.biosoft@gmail.de
 License: GPL 3
-Description: pmx: alchemistry in gromacs
-        ===========================
-        
-        |build| |cov|
-        
-        **Warning:** this is a development version of ``pmx``, it is not stable or reliable yet. You are welcome to
-        try/test it and provide feedback, but use at your own risk. The current stable version of ``pmx`` can
-        be found in the master branch: https://github.com/deGrootLab/pmx
-        
-        ``pmx`` is a python library that allows users to setup and analyse molecular
-        dynamics simulations with the `Gromacs <http://gromacs.org>`_ package.
-        Among its main features are the setup and analysis of alchemical free energy
-        calculations for protein, nucleic acid, and small molecule mutations.
-        
-        https://degrootlab.github.io/pmx/
-        
-        Citations
-        ---------
-        ``pmx`` is a research software. If you make use of it in scientific publications, please cite the following papers::
-        
-            @article{Gapsys2015pmx,
-                title = {pmx: Automated protein structure and topology
-                generation for alchemical perturbations},
-                author = {Gapsys, Vytautas and Michielssens, Servaas
-                and Seeliger, Daniel and de Groot, Bert L.},
-                journal = {Journal of Computational Chemistry},
-                volume = {36},
-                number = {5},
-                pages = {348--354},
-                year = {2015},
-                doi = {10.1002/jcc.23804}
-            }
-        
-            @article{Seeliger2010pmx,
-                title = {Protein Thermostability Calculations Using
-                Alchemical Free Energy Simulations},
-                author = {Seeliger, Daniel and de Groot, Bert L.},
-                journal = {Biophysical Journal},
-                volume = {98},
-                number = {10},
-                pages = {2309--2316},
-                year = {2010},
-                doi = {10.1016/j.bpj.2010.01.051}
-            }
-        
-        
-        License
-        -------
-        ``pmx`` is licensed under the GNU Lesser General Public License v3.0 (LGPL v3).
-        
-        .. |build| image:: https://travis-ci.org/deGrootLab/pmx.svg?branch=master
-            :alt: Build Status
-            :scale: 100%
-            :target: https://travis-ci.org/deGrootLab/pmx
-        
-        .. |cov| image:: https://codecov.io/gh/deGrootLab/pmx/branch/develop/graph/badge.svg
-            :alt: Code coverage
-            :scale: 100%
-            :target: https://codecov.io/gh/deGrootLab/pmx
-        
 Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ==3.7.*
+Requires-Python: >=3.7
+License-File: LICENSE
+
+pmx: alchemistry in gromacs
+===========================
+
+|build| |cov|
+
+**PMX_BIOBB DISTRIBUTION VERSION**: 2.0.0
+**Based on the PMX Icolos branch commit**: https://github.com/deGrootLab/pmx/commit/80f4f8a1552c37e3d926f950d91db77cd4dea9cf
+
+**Warning:** this is a development version of ``pmx``, it is not stable or reliable yet. You are welcome to
+try/test it and provide feedback, but use at your own risk. The current stable version of ``pmx`` can
+be found in the master branch: https://github.com/deGrootLab/pmx
+
+``pmx`` is a python library that allows users to setup and analyse molecular
+dynamics simulations with the `Gromacs <http://gromacs.org>`_ package.
+Among its main features are the setup and analysis of alchemical free energy
+calculations for protein, nucleic acid, and small molecule mutations.
+
+https://degrootlab.github.io/pmx/
+
+Citations
+---------
+``pmx`` is a research software. If you make use of it in scientific publications, please cite the following papers::
+
+    @article{Gapsys2015pmx,
+        title = {pmx: Automated protein structure and topology
+        generation for alchemical perturbations},
+        author = {Gapsys, Vytautas and Michielssens, Servaas
+        and Seeliger, Daniel and de Groot, Bert L.},
+        journal = {Journal of Computational Chemistry},
+        volume = {36},
+        number = {5},
+        pages = {348--354},
+        year = {2015},
+        doi = {10.1002/jcc.23804}
+    }
+
+    @article{Seeliger2010pmx,
+        title = {Protein Thermostability Calculations Using
+        Alchemical Free Energy Simulations},
+        author = {Seeliger, Daniel and de Groot, Bert L.},
+        journal = {Biophysical Journal},
+        volume = {98},
+        number = {10},
+        pages = {2309--2316},
+        year = {2010},
+        doi = {10.1016/j.bpj.2010.01.051}
+    }
+
+
+License
+-------
+``pmx`` is licensed under the GNU Lesser General Public License v3.0 (LGPL v3).
+
+.. |build| image:: https://travis-ci.org/deGrootLab/pmx.svg?branch=master
+    :alt: Build Status
+    :scale: 100%
+    :target: https://travis-ci.org/deGrootLab/pmx
+
+.. |cov| image:: https://codecov.io/gh/deGrootLab/pmx/branch/develop/graph/badge.svg
+    :alt: Code coverage
+    :scale: 100%
+    :target: https://codecov.io/gh/deGrootLab/pmx
+
+
```

### Comparing `pmx_biobb-1.0.1/versioneer.py` & `pmx_biobb-2.0.0/versioneer.py`

 * *Files 2% similar despite different names*

```diff
@@ -735,27 +735,25 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
-    """
-    return "1.0.1"
+    1: no tags. git_describe was just HEX. 2.0.0
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%%d.g%%s" %% (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
+        rendered = "2.0.0" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_pre(pieces):
@@ -897,19 +895,14 @@
 
 def get_versions():
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
-    
-    return {"version": "1.0.1", "full-revisionid": None,
-                "dirty": None,
-                "error": "unable to find root of source tree",
-                "date": None}
 
     cfg = get_config()
     verbose = cfg.verbose
 
     try:
         return git_versions_from_keywords(get_keywords(), cfg.tag_prefix,
                                           verbose)
@@ -1242,30 +1235,27 @@
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
-    1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
+    1: no tags. git_describe was just HEX. 2.0.0
     """
-    return "1.0.1"
     if pieces["closest-tag"]:
         rendered = pieces["closest-tag"]
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
+        rendered = "2.0.0"
+
     return rendered
 
 
 def render_pep440_pre(pieces):
     """TAG[.post.devDISTANCE] -- No -dirty.
 
     Exceptions:
@@ -1403,85 +1393,17 @@
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
-    """Get the project version from whatever source is available.
-
-    Returns dict with two keys: 'version' and 'full'.
-    """
-    if "versioneer" in sys.modules:
-        # see the discussion in cmdclass.py:get_cmdclass()
-        del sys.modules["versioneer"]
-
-    root = get_root()
-    cfg = get_config_from_root(root)
-
-    assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
-    handlers = HANDLERS.get(cfg.VCS)
-    assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
-    assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
-
-    versionfile_abs = os.path.join(root, cfg.versionfile_source)
-
-    # extract version from first of: _version.py, VCS command (e.g. 'git
-    # describe'), parentdir. This is meant to work for developers using a
-    # source checkout, for users of a tarball created by 'setup.py sdist',
-    # and for users of a tarball/zipball created by 'git archive' or github's
-    # download-from-tag feature or the equivalent in other VCSes.
-
-    get_keywords_f = handlers.get("get_keywords")
-    from_keywords_f = handlers.get("keywords")
-    if get_keywords_f and from_keywords_f:
-        try:
-            keywords = get_keywords_f(versionfile_abs)
-            ver = from_keywords_f(keywords, cfg.tag_prefix, verbose)
-            if verbose:
-                print("got version from expanded keyword %s" % ver)
-            return ver
-        except NotThisMethod:
-            pass
+    """Get the project version from whatever source is available."""
 
-    try:
-        ver = versions_from_file(versionfile_abs)
-        if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
-        return ver
-    except NotThisMethod:
-        pass
-
-    from_vcs_f = handlers.get("pieces_from_vcs")
-    if from_vcs_f:
-        try:
-            pieces = from_vcs_f(cfg.tag_prefix, root, verbose)
-            ver = render(pieces, cfg.style)
-            if verbose:
-                print("got version from VCS %s" % ver)
-            return ver
-        except NotThisMethod:
-            pass
-
-    try:
-        if cfg.parentdir_prefix:
-            ver = versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
-            if verbose:
-                print("got version from parentdir %s" % ver)
-            return ver
-    except NotThisMethod:
-        pass
-
-    if verbose:
-        print("unable to compute version")
-
-    return {"version": "0+unknown", "full-revisionid": None,
+    return {"version": "2.0.0", "full-revisionid": None,
             "dirty": None, "error": "unable to compute version",
             "date": None}
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
```

