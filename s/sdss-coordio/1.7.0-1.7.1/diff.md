# Comparing `tmp/sdss-coordio-1.7.0.tar.gz` & `tmp/sdss-coordio-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-coordio-1.7.0.tar", last modified: Sat Apr 15 21:06:00 2023, max compression
+gzip compressed data, was "sdss-coordio-1.7.1.tar", last modified: Tue Apr 25 15:59:54 2023, max compression
```

## Comparing `sdss-coordio-1.7.0.tar` & `sdss-coordio-1.7.1.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.504047 sdss-coordio-1.7.0/
--rw-r--r--   0 runner     (501) staff       (20)     1504 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       62 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-15 21:06:00.504233 sdss-coordio-1.7.0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.338636 sdss-coordio-1.7.0/cextern/
--rw-r--r--   0 runner     (501) staff       (20)      343 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/README.md
--rw-r--r--   0 runner     (501) staff       (20)    12507 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/conv.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.345707 sdss-coordio-1.7.0/cextern/dimage/
--rw-r--r--   0 runner     (501) staff       (20)     3150 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dallpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     1295 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dcen3x3.c
--rw-r--r--   0 runner     (501) staff       (20)     3239 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dfind.c
--rw-r--r--   0 runner     (501) staff       (20)     2553 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dfloodfill.c
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dimage.h
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dmedsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)     1351 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dobjects.c
--rw-r--r--   0 runner     (501) staff       (20)     3798 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     2856 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/drefine.c
--rw-r--r--   0 runner     (501) staff       (20)     1872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dselip.c
--rw-r--r--   0 runner     (501) staff       (20)     1252 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dsigma.c
--rw-r--r--   0 runner     (501) staff       (20)     3854 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/dsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/readme.txt
--rw-r--r--   0 runner     (501) staff       (20)     1984 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/dimage/simplexy.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.477114 sdss-coordio-1.7.0/cextern/sofa/
--rw-r--r--   0 runner     (501) staff       (20)     6468 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/a2af.c
--rw-r--r--   0 runner     (501) staff       (20)     6374 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/a2tf.c
--rw-r--r--   0 runner     (501) staff       (20)     6611 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ab.c
--rw-r--r--   0 runner     (501) staff       (20)     7187 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ae2hd.c
--rw-r--r--   0 runner     (501) staff       (20)     6087 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/af2a.c
--rw-r--r--   0 runner     (501) staff       (20)     4955 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/anp.c
--rw-r--r--   0 runner     (501) staff       (20)     4983 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/anpm.c
--rw-r--r--   0 runner     (501) staff       (20)     9173 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcg.c
--rw-r--r--   0 runner     (501) staff       (20)     9278 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcg13.c
--rw-r--r--   0 runner     (501) staff       (20)     9669 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apci.c
--rw-r--r--   0 runner     (501) staff       (20)     9954 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apci13.c
--rw-r--r--   0 runner     (501) staff       (20)    12864 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apco.c
--rw-r--r--   0 runner     (501) staff       (20)    14172 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apco13.c
--rw-r--r--   0 runner     (501) staff       (20)    11004 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcs.c
--rw-r--r--   0 runner     (501) staff       (20)     9686 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apcs13.c
--rw-r--r--   0 runner     (501) staff       (20)     8285 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aper.c
--rw-r--r--   0 runner     (501) staff       (20)     9207 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aper13.c
--rw-r--r--   0 runner     (501) staff       (20)    10588 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apio.c
--rw-r--r--   0 runner     (501) staff       (20)    12842 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/apio13.c
--rw-r--r--   0 runner     (501) staff       (20)     8257 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atci13.c
--rw-r--r--   0 runner     (501) staff       (20)     7978 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciq.c
--rw-r--r--   0 runner     (501) staff       (20)     9826 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciqn.c
--rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atciqz.c
--rw-r--r--   0 runner     (501) staff       (20)    12474 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atco13.c
--rw-r--r--   0 runner     (501) staff       (20)     7919 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atic13.c
--rw-r--r--   0 runner     (501) staff       (20)     8735 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aticq.c
--rw-r--r--   0 runner     (501) staff       (20)    10634 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/aticqn.c
--rw-r--r--   0 runner     (501) staff       (20)    11485 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atio13.c
--rw-r--r--   0 runner     (501) staff       (20)    11389 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atioq.c
--rw-r--r--   0 runner     (501) staff       (20)    12003 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoc13.c
--rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoi13.c
--rw-r--r--   0 runner     (501) staff       (20)    11115 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/atoiq.c
--rw-r--r--   0 runner     (501) staff       (20)     6640 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bi00.c
--rw-r--r--   0 runner     (501) staff       (20)     8454 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bp00.c
--rw-r--r--   0 runner     (501) staff       (20)     7280 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bp06.c
--rw-r--r--   0 runner     (501) staff       (20)     5822 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/bpn2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     7375 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7362 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7165 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2i06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7592 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ibpn.c
--rw-r--r--   0 runner     (501) staff       (20)     7162 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ixy.c
--rw-r--r--   0 runner     (501) staff       (20)     6391 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2ixys.c
--rw-r--r--   0 runner     (501) staff       (20)     5320 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2s.c
--rw-r--r--   0 runner     (501) staff       (20)     8083 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7985 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7970 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2t06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6652 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2tcio.c
--rw-r--r--   0 runner     (501) staff       (20)     6679 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2teqx.c
--rw-r--r--   0 runner     (501) staff       (20)     8786 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2tpe.c
--rw-r--r--   0 runner     (501) staff       (20)     8249 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/c2txy.c
--rw-r--r--   0 runner     (501) staff       (20)     6962 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cal2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     4897 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cp.c
--rw-r--r--   0 runner     (501) staff       (20)     4990 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/cr.c
--rw-r--r--   0 runner     (501) staff       (20)     9794 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/d2dtf.c
--rw-r--r--   0 runner     (501) staff       (20)     7240 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/d2tf.c
--rw-r--r--   0 runner     (501) staff       (20)    13394 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dat.c
--rw-r--r--   0 runner     (501) staff       (20)    63548 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     9375 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/dtf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     7237 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eceq06.c
--rw-r--r--   0 runner     (501) staff       (20)     7251 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ecm06.c
--rw-r--r--   0 runner     (501) staff       (20)     6929 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00.c
--rw-r--r--   0 runner     (501) staff       (20)     7105 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7436 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6632 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ee06a.c
--rw-r--r--   0 runner     (501) staff       (20)    12358 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eect00.c
--rw-r--r--   0 runner     (501) staff       (20)     6688 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eform.c
--rw-r--r--   0 runner     (501) staff       (20)     7000 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eo06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6082 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eors.c
--rw-r--r--   0 runner     (501) staff       (20)     5398 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epb.c
--rw-r--r--   0 runner     (501) staff       (20)     5342 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epb2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     5327 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epj.c
--rw-r--r--   0 runner     (501) staff       (20)     5330 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epj2jd.c
--rw-r--r--   0 runner     (501) staff       (20)   152024 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/epv00.c
--rw-r--r--   0 runner     (501) staff       (20)     7238 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eqec06.c
--rw-r--r--   0 runner     (501) staff       (20)     6953 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/eqeq94.c
--rw-r--r--   0 runner     (501) staff       (20)     6978 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/era00.c
--rw-r--r--   0 runner     (501) staff       (20)     5789 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fad03.c
--rw-r--r--   0 runner     (501) staff       (20)     5756 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fae03.c
--rw-r--r--   0 runner     (501) staff       (20)     5883 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faf03.c
--rw-r--r--   0 runner     (501) staff       (20)     5768 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faju03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fal03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/falp03.c
--rw-r--r--   0 runner     (501) staff       (20)     5760 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fama03.c
--rw-r--r--   0 runner     (501) staff       (20)     5770 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fame03.c
--rw-r--r--   0 runner     (501) staff       (20)     5631 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fane03.c
--rw-r--r--   0 runner     (501) staff       (20)     5826 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faom03.c
--rw-r--r--   0 runner     (501) staff       (20)     5754 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fapa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5765 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fasa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5629 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/faur03.c
--rw-r--r--   0 runner     (501) staff       (20)     5764 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fave03.c
--rw-r--r--   0 runner     (501) staff       (20)    12333 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk425.c
--rw-r--r--   0 runner     (501) staff       (20)     9855 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk45z.c
--rw-r--r--   0 runner     (501) staff       (20)    12391 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk524.c
--rw-r--r--   0 runner     (501) staff       (20)     7422 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk52h.c
--rw-r--r--   0 runner     (501) staff       (20)     7286 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk54z.c
--rw-r--r--   0 runner     (501) staff       (20)     6198 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk5hip.c
--rw-r--r--   0 runner     (501) staff       (20)     8093 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fk5hz.c
--rw-r--r--   0 runner     (501) staff       (20)     7061 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fw2m.c
--rw-r--r--   0 runner     (501) staff       (20)     6147 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/fw2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     8396 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/g2icrs.c
--rw-r--r--   0 runner     (501) staff       (20)     6710 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gc2gd.c
--rw-r--r--   0 runner     (501) staff       (20)     8338 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gc2gde.c
--rw-r--r--   0 runner     (501) staff       (20)     6783 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gd2gc.c
--rw-r--r--   0 runner     (501) staff       (20)     6968 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gd2gce.c
--rw-r--r--   0 runner     (501) staff       (20)     7699 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst00.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7688 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gmst82.c
--rw-r--r--   0 runner     (501) staff       (20)     7470 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7770 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7536 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7174 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7099 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/gst94.c
--rw-r--r--   0 runner     (501) staff       (20)     7614 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/h2fk5.c
--rw-r--r--   0 runner     (501) staff       (20)     7382 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hd2ae.c
--rw-r--r--   0 runner     (501) staff       (20)     6333 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hd2pa.c
--rw-r--r--   0 runner     (501) staff       (20)     8684 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/hfk5z.c
--rw-r--r--   0 runner     (501) staff       (20)     8382 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/icrs2g.c
--rw-r--r--   0 runner     (501) staff       (20)     4970 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ir.c
--rw-r--r--   0 runner     (501) staff       (20)     8269 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/jd2cal.c
--rw-r--r--   0 runner     (501) staff       (20)     7559 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/jdcalf.c
--rw-r--r--   0 runner     (501) staff       (20)     7662 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ld.c
--rw-r--r--   0 runner     (501) staff       (20)     8829 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ldn.c
--rw-r--r--   0 runner     (501) staff       (20)     5982 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ldsun.c
--rw-r--r--   0 runner     (501) staff       (20)     7014 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/lteceq.c
--rw-r--r--   0 runner     (501) staff       (20)     7567 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltecm.c
--rw-r--r--   0 runner     (501) staff       (20)     7019 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/lteqec.c
--rw-r--r--   0 runner     (501) staff       (20)     6500 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltp.c
--rw-r--r--   0 runner     (501) staff       (20)     6581 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpb.c
--rw-r--r--   0 runner     (501) staff       (20)     7601 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpecl.c
--rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ltpequ.c
--rw-r--r--   0 runner     (501) staff       (20)    27755 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/makefile
--rw-r--r--   0 runner     (501) staff       (20)     6728 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6713 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6660 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/num06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/numat.c
--rw-r--r--   0 runner     (501) staff       (20)   119801 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut00a.c
--rw-r--r--   0 runner     (501) staff       (20)    19020 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7823 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut06a.c
--rw-r--r--   0 runner     (501) staff       (20)    16295 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nut80.c
--rw-r--r--   0 runner     (501) staff       (20)     6473 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/nutm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6414 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/obl06.c
--rw-r--r--   0 runner     (501) staff       (20)     6459 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/obl80.c
--rw-r--r--   0 runner     (501) staff       (20)    13793 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p06e.c
--rw-r--r--   0 runner     (501) staff       (20)     5029 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5276 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/p2s.c
--rw-r--r--   0 runner     (501) staff       (20)     6768 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pap.c
--rw-r--r--   0 runner     (501) staff       (20)     5638 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pas.c
--rw-r--r--   0 runner     (501) staff       (20)     7817 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pb06.c
--rw-r--r--   0 runner     (501) staff       (20)     5008 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pdp.c
--rw-r--r--   0 runner     (501) staff       (20)     7964 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pfw06.c
--rw-r--r--   0 runner     (501) staff       (20)    23180 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/plan94.c
--rw-r--r--   0 runner     (501) staff       (20)     4887 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pm.c
--rw-r--r--   0 runner     (501) staff       (20)     6579 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat00.c
--rw-r--r--   0 runner     (501) staff       (20)     6683 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat06.c
--rw-r--r--   0 runner     (501) staff       (20)     7548 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmat76.c
--rw-r--r--   0 runner     (501) staff       (20)     5090 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmp.c
--rw-r--r--   0 runner     (501) staff       (20)     7054 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmpx.c
--rw-r--r--   0 runner     (501) staff       (20)    10220 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pmsafe.c
--rw-r--r--   0 runner     (501) staff       (20)     5495 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn.c
--rw-r--r--   0 runner     (501) staff       (20)     9146 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00.c
--rw-r--r--   0 runner     (501) staff       (20)     8833 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00a.c
--rw-r--r--   0 runner     (501) staff       (20)     8825 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn00b.c
--rw-r--r--   0 runner     (501) staff       (20)     9253 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn06.c
--rw-r--r--   0 runner     (501) staff       (20)     8282 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pn06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6802 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6797 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6835 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6778 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pnm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6453 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pom00.c
--rw-r--r--   0 runner     (501) staff       (20)     5087 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ppp.c
--rw-r--r--   0 runner     (501) staff       (20)     5275 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ppsp.c
--rw-r--r--   0 runner     (501) staff       (20)     7813 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pr00.c
--rw-r--r--   0 runner     (501) staff       (20)     8023 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/prec76.c
--rw-r--r--   0 runner     (501) staff       (20)     4958 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pv2p.c
--rw-r--r--   0 runner     (501) staff       (20)     6861 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pv2s.c
--rw-r--r--   0 runner     (501) staff       (20)     5587 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvdpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvm.c
--rw-r--r--   0 runner     (501) staff       (20)     5182 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvmpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5177 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvppv.c
--rw-r--r--   0 runner     (501) staff       (20)    10128 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvstar.c
--rw-r--r--   0 runner     (501) staff       (20)     7712 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvtob.c
--rw-r--r--   0 runner     (501) staff       (20)     5373 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvu.c
--rw-r--r--   0 runner     (501) staff       (20)     5280 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvup.c
--rw-r--r--   0 runner     (501) staff       (20)     5842 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pvxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5234 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/pxp.c
--rw-r--r--   0 runner     (501) staff       (20)    11663 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/refco.c
--rw-r--r--   0 runner     (501) staff       (20)     5989 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rm2v.c
--rw-r--r--   0 runner     (501) staff       (20)     5996 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rv2m.c
--rw-r--r--   0 runner     (501) staff       (20)     5807 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rx.c
--rw-r--r--   0 runner     (501) staff       (20)     5298 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5144 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rxr.c
--rw-r--r--   0 runner     (501) staff       (20)     5848 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ry.c
--rw-r--r--   0 runner     (501) staff       (20)     5817 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/rz.c
--rw-r--r--   0 runner     (501) staff       (20)    15540 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00.c
--rw-r--r--   0 runner     (501) staff       (20)     7781 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7772 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s00b.c
--rw-r--r--   0 runner     (501) staff       (20)    15442 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s06.c
--rw-r--r--   0 runner     (501) staff       (20)     7799 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s06a.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2c.c
--rw-r--r--   0 runner     (501) staff       (20)     5209 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2p.c
--rw-r--r--   0 runner     (501) staff       (20)     5636 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5282 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/s2xpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5877 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sepp.c
--rw-r--r--   0 runner     (501) staff       (20)     5424 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/seps.c
--rw-r--r--   0 runner     (501) staff       (20)    26863 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sofa.h
--rw-r--r--   0 runner     (501) staff       (20)     8772 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sofam.h
--rw-r--r--   0 runner     (501) staff       (20)     6557 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sp00.c
--rw-r--r--   0 runner     (501) staff       (20)    10677 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/starpm.c
--rw-r--r--   0 runner     (501) staff       (20)    11959 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/starpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5038 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5101 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/sxpv.c
--rw-r--r--   0 runner     (501) staff       (20)   241327 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/t_sofa_c.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taitt.c
--rw-r--r--   0 runner     (501) staff       (20)     5901 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taiut1.c
--rw-r--r--   0 runner     (501) staff       (20)     7493 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/taiutc.c
--rw-r--r--   0 runner     (501) staff       (20)     6987 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tcbtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tcgtt.c
--rw-r--r--   0 runner     (501) staff       (20)     7109 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tdbtcb.c
--rw-r--r--   0 runner     (501) staff       (20)     6353 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tdbtt.c
--rw-r--r--   0 runner     (501) staff       (20)     6062 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tf2a.c
--rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     8685 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpors.c
--rw-r--r--   0 runner     (501) staff       (20)     8649 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tporv.c
--rw-r--r--   0 runner     (501) staff       (20)     6534 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpsts.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpstv.c
--rw-r--r--   0 runner     (501) staff       (20)     7253 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpxes.c
--rw-r--r--   0 runner     (501) staff       (20)     7927 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tpxev.c
--rw-r--r--   0 runner     (501) staff       (20)     5136 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tr.c
--rw-r--r--   0 runner     (501) staff       (20)     5263 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/trxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5291 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/trxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5841 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttai.c
--rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttcg.c
--rw-r--r--   0 runner     (501) staff       (20)     6345 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/tttdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5794 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ttut1.c
--rw-r--r--   0 runner     (501) staff       (20)     5898 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1tai.c
--rw-r--r--   0 runner     (501) staff       (20)     5798 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1tt.c
--rw-r--r--   0 runner     (501) staff       (20)     8782 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/ut1utc.c
--rw-r--r--   0 runner     (501) staff       (20)     8283 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/utctai.c
--rw-r--r--   0 runner     (501) staff       (20)     7458 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/utcut1.c
--rw-r--r--   0 runner     (501) staff       (20)   133674 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xy06.c
--rw-r--r--   0 runner     (501) staff       (20)     7028 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7010 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7056 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/xys06a.c
--rw-r--r--   0 runner     (501) staff       (20)     4820 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zp.c
--rw-r--r--   0 runner     (501) staff       (20)     4874 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4967 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/cextern/sofa/zr.c
--rw-r--r--   0 runner     (501) staff       (20)     2386 2023-04-15 21:06:00.505559 sdss-coordio-1.7.0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2697 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.334758 sdss-coordio-1.7.0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.489105 sdss-coordio-1.7.0/src/coordio/
--rw-r--r--   0 runner     (501) staff       (20)     1178 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12342 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/astrometry.py
--rw-r--r--   0 runner     (501) staff       (20)     5635 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/calibration.py
--rw-r--r--   0 runner     (501) staff       (20)    51063 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     9926 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     7570 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/defaults.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.490147 sdss-coordio-1.7.0/src/coordio/etc/
--rw-r--r--   0 runner     (501) staff       (20)       73 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/etc/astrometrynet.cfg
--rw-r--r--   0 runner     (501) staff       (20)      366 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/etc/coordio.yml
--rw-r--r--   0 runner     (501) staff       (20)      722 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    12748 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/extraction.py
--rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/fitData.py
--rw-r--r--   0 runner     (501) staff       (20)    24723 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/guide.py
--rw-r--r--   0 runner     (501) staff       (20)     5870 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/iers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.490642 sdss-coordio-1.7.0/src/coordio/include/
--rw-r--r--   0 runner     (501) staff       (20)     1992 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/include/coordio.h
--rw-r--r--   0 runner     (501) staff       (20)     4013 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/site.py
--rw-r--r--   0 runner     (501) staff       (20)    14255 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/sky.py
--rw-r--r--   0 runner     (501) staff       (20)     6440 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/sofa_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    10661 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/tangent.py
--rw-r--r--   0 runner     (501) staff       (20)    13390 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     6451 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/time.py
--rw-r--r--   0 runner     (501) staff       (20)    51462 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/transforms.py
--rw-r--r--   0 runner     (501) staff       (20)    33540 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3734 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/wok.py
--rw-r--r--   0 runner     (501) staff       (20)    14872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/zernike.py
--rw-r--r--   0 runner     (501) staff       (20)    12907 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/src/coordio/zhaoburge.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.494410 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6867 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-15 21:02:48.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      483 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2023-04-15 21:06:00.000000 sdss-coordio-1.7.0/src/sdss_coordio.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-15 21:06:00.503631 sdss-coordio-1.7.0/tests/
--rw-r--r--   0 runner     (501) staff       (20)    13006 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_conv.py
--rw-r--r--   0 runner     (501) staff       (20)     7006 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     1386 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_fpScale.py
--rw-r--r--   0 runner     (501) staff       (20)     4290 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_guide.py
--rw-r--r--   0 runner     (501) staff       (20)     1418 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_iers.py
--rw-r--r--   0 runner     (501) staff       (20)    11447 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_libcoordio.py
--rw-r--r--   0 runner     (501) staff       (20)     5271 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_offset.py
--rw-r--r--   0 runner     (501) staff       (20)     8074 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_plPlug.py
--rw-r--r--   0 runner     (501) staff       (20)     5525 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     1105 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_site.py
--rw-r--r--   0 runner     (501) staff       (20)     5302 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_sky.py
--rw-r--r--   0 runner     (501) staff       (20)     1171 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_sofa.py
--rw-r--r--   0 runner     (501) staff       (20)     3340 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_tangent.py
--rw-r--r--   0 runner     (501) staff       (20)     2738 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_tangentToPositioner2.py
--rw-r--r--   0 runner     (501) staff       (20)    13872 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_time.py
--rw-r--r--   0 runner     (501) staff       (20)     2588 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_wok.py
--rw-r--r--   0 runner     (501) staff       (20)     1363 2023-04-15 21:02:23.000000 sdss-coordio-1.7.0/tests/test_zern.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.480330 sdss-coordio-1.7.1/
+-rw-r--r--   0 runner     (501) staff       (20)     1504 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/LICENSE.md
+-rw-r--r--   0 runner     (501) staff       (20)       62 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-25 15:59:54.480571 sdss-coordio-1.7.1/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      796 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:53.374465 sdss-coordio-1.7.1/cextern/
+-rw-r--r--   0 runner     (501) staff       (20)      343 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/README.md
+-rw-r--r--   0 runner     (501) staff       (20)    12507 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/conv.cpp
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:53.397643 sdss-coordio-1.7.1/cextern/dimage/
+-rw-r--r--   0 runner     (501) staff       (20)     3150 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dallpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     1295 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dcen3x3.c
+-rw-r--r--   0 runner     (501) staff       (20)     3239 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dfind.c
+-rw-r--r--   0 runner     (501) staff       (20)     2553 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dfloodfill.c
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dimage.h
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dmedsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dobjects.c
+-rw-r--r--   0 runner     (501) staff       (20)     3798 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dpeaks.c
+-rw-r--r--   0 runner     (501) staff       (20)     2856 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/drefine.c
+-rw-r--r--   0 runner     (501) staff       (20)     1872 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dselip.c
+-rw-r--r--   0 runner     (501) staff       (20)     1252 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dsigma.c
+-rw-r--r--   0 runner     (501) staff       (20)     3854 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/dsmooth.c
+-rw-r--r--   0 runner     (501) staff       (20)       58 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/readme.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1984 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/dimage/simplexy.c
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:53.886735 sdss-coordio-1.7.1/cextern/sofa/
+-rw-r--r--   0 runner     (501) staff       (20)     6468 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/a2af.c
+-rw-r--r--   0 runner     (501) staff       (20)     6374 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/a2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)     6611 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ab.c
+-rw-r--r--   0 runner     (501) staff       (20)     7187 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ae2hd.c
+-rw-r--r--   0 runner     (501) staff       (20)     6087 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/af2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4955 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/anp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4983 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/anpm.c
+-rw-r--r--   0 runner     (501) staff       (20)     9173 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     9278 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apcg13.c
+-rw-r--r--   0 runner     (501) staff       (20)     9669 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apci.c
+-rw-r--r--   0 runner     (501) staff       (20)     9954 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apci13.c
+-rw-r--r--   0 runner     (501) staff       (20)    12864 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apco.c
+-rw-r--r--   0 runner     (501) staff       (20)    14172 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apco13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11004 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apcs.c
+-rw-r--r--   0 runner     (501) staff       (20)     9686 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apcs13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8285 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/aper.c
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/aper13.c
+-rw-r--r--   0 runner     (501) staff       (20)    10588 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apio.c
+-rw-r--r--   0 runner     (501) staff       (20)    12842 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/apio13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8257 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atci13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7978 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atciq.c
+-rw-r--r--   0 runner     (501) staff       (20)     9826 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atciqn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7729 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atciqz.c
+-rw-r--r--   0 runner     (501) staff       (20)    12474 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atco13.c
+-rw-r--r--   0 runner     (501) staff       (20)     7919 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atic13.c
+-rw-r--r--   0 runner     (501) staff       (20)     8735 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/aticq.c
+-rw-r--r--   0 runner     (501) staff       (20)    10634 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/aticqn.c
+-rw-r--r--   0 runner     (501) staff       (20)    11485 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atio13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11389 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atioq.c
+-rw-r--r--   0 runner     (501) staff       (20)    12003 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atoc13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11902 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atoi13.c
+-rw-r--r--   0 runner     (501) staff       (20)    11115 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/atoiq.c
+-rw-r--r--   0 runner     (501) staff       (20)     6640 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/bi00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8454 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/bp00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7280 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/bp06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5822 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/bpn2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     7375 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2i00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7362 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2i00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7165 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2i06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7592 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2ibpn.c
+-rw-r--r--   0 runner     (501) staff       (20)     7162 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2ixy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6391 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2ixys.c
+-rw-r--r--   0 runner     (501) staff       (20)     5320 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     8083 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2t00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7985 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2t00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7970 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2t06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6652 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2tcio.c
+-rw-r--r--   0 runner     (501) staff       (20)     6679 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2teqx.c
+-rw-r--r--   0 runner     (501) staff       (20)     8786 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2tpe.c
+-rw-r--r--   0 runner     (501) staff       (20)     8249 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/c2txy.c
+-rw-r--r--   0 runner     (501) staff       (20)     6962 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/cal2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     4897 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/cp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4990 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/cpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/cr.c
+-rw-r--r--   0 runner     (501) staff       (20)     9794 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/d2dtf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7240 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/d2tf.c
+-rw-r--r--   0 runner     (501) staff       (20)    13394 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/dat.c
+-rw-r--r--   0 runner     (501) staff       (20)    63548 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/dtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     9375 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/dtf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     7237 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eceq06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7251 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ecm06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6929 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ee00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7105 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ee00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7436 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ee00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6632 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ee06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    12358 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eect00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6688 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eform.c
+-rw-r--r--   0 runner     (501) staff       (20)     7000 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eo06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6082 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eors.c
+-rw-r--r--   0 runner     (501) staff       (20)     5398 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/epb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5342 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/epb2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)     5327 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/epj.c
+-rw-r--r--   0 runner     (501) staff       (20)     5330 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/epj2jd.c
+-rw-r--r--   0 runner     (501) staff       (20)   152024 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/epv00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7238 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eqec06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6953 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/eqeq94.c
+-rw-r--r--   0 runner     (501) staff       (20)     6978 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/era00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5789 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fad03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5756 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fae03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5883 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/faf03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5768 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/faju03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fal03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5758 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/falp03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5760 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fama03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5770 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fame03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5631 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fane03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5826 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/faom03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5754 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fapa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5765 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fasa03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5629 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/faur03.c
+-rw-r--r--   0 runner     (501) staff       (20)     5764 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fave03.c
+-rw-r--r--   0 runner     (501) staff       (20)    12333 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk425.c
+-rw-r--r--   0 runner     (501) staff       (20)     9855 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk45z.c
+-rw-r--r--   0 runner     (501) staff       (20)    12391 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk524.c
+-rw-r--r--   0 runner     (501) staff       (20)     7422 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk52h.c
+-rw-r--r--   0 runner     (501) staff       (20)     7286 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk54z.c
+-rw-r--r--   0 runner     (501) staff       (20)     6198 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk5hip.c
+-rw-r--r--   0 runner     (501) staff       (20)     8093 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fk5hz.c
+-rw-r--r--   0 runner     (501) staff       (20)     7061 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fw2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     6147 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/fw2xy.c
+-rw-r--r--   0 runner     (501) staff       (20)     8396 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/g2icrs.c
+-rw-r--r--   0 runner     (501) staff       (20)     6710 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gc2gd.c
+-rw-r--r--   0 runner     (501) staff       (20)     8338 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gc2gde.c
+-rw-r--r--   0 runner     (501) staff       (20)     6783 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gd2gc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6968 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gd2gce.c
+-rw-r--r--   0 runner     (501) staff       (20)     7699 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gmst00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gmst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7688 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gmst82.c
+-rw-r--r--   0 runner     (501) staff       (20)     7470 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gst00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7770 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gst00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7536 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gst06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7174 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gst06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7099 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/gst94.c
+-rw-r--r--   0 runner     (501) staff       (20)     7614 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/h2fk5.c
+-rw-r--r--   0 runner     (501) staff       (20)     7382 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/hd2ae.c
+-rw-r--r--   0 runner     (501) staff       (20)     6333 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/hd2pa.c
+-rw-r--r--   0 runner     (501) staff       (20)     8684 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/hfk5z.c
+-rw-r--r--   0 runner     (501) staff       (20)     8382 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/icrs2g.c
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ir.c
+-rw-r--r--   0 runner     (501) staff       (20)     8269 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/jd2cal.c
+-rw-r--r--   0 runner     (501) staff       (20)     7559 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/jdcalf.c
+-rw-r--r--   0 runner     (501) staff       (20)     7662 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ld.c
+-rw-r--r--   0 runner     (501) staff       (20)     8829 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ldn.c
+-rw-r--r--   0 runner     (501) staff       (20)     5982 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ldsun.c
+-rw-r--r--   0 runner     (501) staff       (20)     7014 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/lteceq.c
+-rw-r--r--   0 runner     (501) staff       (20)     7567 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ltecm.c
+-rw-r--r--   0 runner     (501) staff       (20)     7019 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/lteqec.c
+-rw-r--r--   0 runner     (501) staff       (20)     6500 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ltp.c
+-rw-r--r--   0 runner     (501) staff       (20)     6581 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ltpb.c
+-rw-r--r--   0 runner     (501) staff       (20)     7601 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ltpecl.c
+-rw-r--r--   0 runner     (501) staff       (20)     7880 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ltpequ.c
+-rw-r--r--   0 runner     (501) staff       (20)    27755 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/makefile
+-rw-r--r--   0 runner     (501) staff       (20)     6728 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/num00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6713 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/num00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6660 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/num06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6057 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/numat.c
+-rw-r--r--   0 runner     (501) staff       (20)   119801 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/nut00a.c
+-rw-r--r--   0 runner     (501) staff       (20)    19020 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/nut00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7823 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/nut06a.c
+-rw-r--r--   0 runner     (501) staff       (20)    16295 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/nut80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6473 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/nutm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6414 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/obl06.c
+-rw-r--r--   0 runner     (501) staff       (20)     6459 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/obl80.c
+-rw-r--r--   0 runner     (501) staff       (20)    13793 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/p06e.c
+-rw-r--r--   0 runner     (501) staff       (20)     5029 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/p2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5276 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/p2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     6768 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pap.c
+-rw-r--r--   0 runner     (501) staff       (20)     5638 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pas.c
+-rw-r--r--   0 runner     (501) staff       (20)     7817 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pb06.c
+-rw-r--r--   0 runner     (501) staff       (20)     5008 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pdp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7964 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pfw06.c
+-rw-r--r--   0 runner     (501) staff       (20)    23180 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/plan94.c
+-rw-r--r--   0 runner     (501) staff       (20)     4887 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pm.c
+-rw-r--r--   0 runner     (501) staff       (20)     6579 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmat00.c
+-rw-r--r--   0 runner     (501) staff       (20)     6683 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmat06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7548 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmat76.c
+-rw-r--r--   0 runner     (501) staff       (20)     5090 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7054 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmpx.c
+-rw-r--r--   0 runner     (501) staff       (20)    10220 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pmsafe.c
+-rw-r--r--   0 runner     (501) staff       (20)     5495 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn.c
+-rw-r--r--   0 runner     (501) staff       (20)     9146 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8833 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     8825 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     9253 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn06.c
+-rw-r--r--   0 runner     (501) staff       (20)     8282 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pn06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6802 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pnm00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6797 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pnm00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     6835 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pnm06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6778 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pnm80.c
+-rw-r--r--   0 runner     (501) staff       (20)     6453 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pom00.c
+-rw-r--r--   0 runner     (501) staff       (20)     5087 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ppp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5275 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ppsp.c
+-rw-r--r--   0 runner     (501) staff       (20)     7813 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pr00.c
+-rw-r--r--   0 runner     (501) staff       (20)     8023 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/prec76.c
+-rw-r--r--   0 runner     (501) staff       (20)     4958 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pv2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     6861 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pv2s.c
+-rw-r--r--   0 runner     (501) staff       (20)     5587 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvdpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvm.c
+-rw-r--r--   0 runner     (501) staff       (20)     5182 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvmpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5177 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvppv.c
+-rw-r--r--   0 runner     (501) staff       (20)    10128 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvstar.c
+-rw-r--r--   0 runner     (501) staff       (20)     7712 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvtob.c
+-rw-r--r--   0 runner     (501) staff       (20)     5373 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvu.c
+-rw-r--r--   0 runner     (501) staff       (20)     5280 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvup.c
+-rw-r--r--   0 runner     (501) staff       (20)     5842 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pvxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5234 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/pxp.c
+-rw-r--r--   0 runner     (501) staff       (20)    11663 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/refco.c
+-rw-r--r--   0 runner     (501) staff       (20)     5989 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rm2v.c
+-rw-r--r--   0 runner     (501) staff       (20)     5996 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rv2m.c
+-rw-r--r--   0 runner     (501) staff       (20)     5807 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rx.c
+-rw-r--r--   0 runner     (501) staff       (20)     5298 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5144 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5337 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rxr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5848 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ry.c
+-rw-r--r--   0 runner     (501) staff       (20)     5817 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/rz.c
+-rw-r--r--   0 runner     (501) staff       (20)    15540 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s00.c
+-rw-r--r--   0 runner     (501) staff       (20)     7781 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7772 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s00b.c
+-rw-r--r--   0 runner     (501) staff       (20)    15442 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7799 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     5073 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s2c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s2p.c
+-rw-r--r--   0 runner     (501) staff       (20)     5636 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s2pv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5282 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/s2xpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5877 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sepp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5424 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/seps.c
+-rw-r--r--   0 runner     (501) staff       (20)    26863 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sofa.h
+-rw-r--r--   0 runner     (501) staff       (20)     8772 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sofam.h
+-rw-r--r--   0 runner     (501) staff       (20)     6557 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sp00.c
+-rw-r--r--   0 runner     (501) staff       (20)    10677 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/starpm.c
+-rw-r--r--   0 runner     (501) staff       (20)    11959 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/starpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5038 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5101 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/sxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)   241327 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/t_sofa_c.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/taitt.c
+-rw-r--r--   0 runner     (501) staff       (20)     5901 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/taiut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     7493 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/taiutc.c
+-rw-r--r--   0 runner     (501) staff       (20)     6987 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tcbtdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5845 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tcgtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     7109 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tdbtcb.c
+-rw-r--r--   0 runner     (501) staff       (20)     6353 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tdbtt.c
+-rw-r--r--   0 runner     (501) staff       (20)     6062 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tf2a.c
+-rw-r--r--   0 runner     (501) staff       (20)     6066 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tf2d.c
+-rw-r--r--   0 runner     (501) staff       (20)     8685 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tpors.c
+-rw-r--r--   0 runner     (501) staff       (20)     8649 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tporv.c
+-rw-r--r--   0 runner     (501) staff       (20)     6534 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tpsts.c
+-rw-r--r--   0 runner     (501) staff       (20)     7337 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tpstv.c
+-rw-r--r--   0 runner     (501) staff       (20)     7253 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tpxes.c
+-rw-r--r--   0 runner     (501) staff       (20)     7927 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tpxev.c
+-rw-r--r--   0 runner     (501) staff       (20)     5136 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tr.c
+-rw-r--r--   0 runner     (501) staff       (20)     5263 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/trxp.c
+-rw-r--r--   0 runner     (501) staff       (20)     5291 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/trxpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     5841 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tttai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5913 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tttcg.c
+-rw-r--r--   0 runner     (501) staff       (20)     6345 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/tttdb.c
+-rw-r--r--   0 runner     (501) staff       (20)     5794 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ttut1.c
+-rw-r--r--   0 runner     (501) staff       (20)     5898 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ut1tai.c
+-rw-r--r--   0 runner     (501) staff       (20)     5798 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ut1tt.c
+-rw-r--r--   0 runner     (501) staff       (20)     8782 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/ut1utc.c
+-rw-r--r--   0 runner     (501) staff       (20)     8283 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/utctai.c
+-rw-r--r--   0 runner     (501) staff       (20)     7458 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/utcut1.c
+-rw-r--r--   0 runner     (501) staff       (20)   133674 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/xy06.c
+-rw-r--r--   0 runner     (501) staff       (20)     7028 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/xys00a.c
+-rw-r--r--   0 runner     (501) staff       (20)     7010 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/xys00b.c
+-rw-r--r--   0 runner     (501) staff       (20)     7056 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/xys06a.c
+-rw-r--r--   0 runner     (501) staff       (20)     4820 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/zp.c
+-rw-r--r--   0 runner     (501) staff       (20)     4874 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/zpv.c
+-rw-r--r--   0 runner     (501) staff       (20)     4967 2023-04-25 15:57:59.000000 sdss-coordio-1.7.1/cextern/sofa/zr.c
+-rw-r--r--   0 runner     (501) staff       (20)     2386 2023-04-25 15:59:54.522794 sdss-coordio-1.7.1/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2697 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:53.350818 sdss-coordio-1.7.1/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.366272 sdss-coordio-1.7.1/src/coordio/
+-rw-r--r--   0 runner     (501) staff       (20)     1178 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12342 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/astrometry.py
+-rw-r--r--   0 runner     (501) staff       (20)     5635 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/calibration.py
+-rw-r--r--   0 runner     (501) staff       (20)    51063 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     9926 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     7570 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/defaults.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.367828 sdss-coordio-1.7.1/src/coordio/etc/
+-rw-r--r--   0 runner     (501) staff       (20)       73 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/etc/astrometrynet.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      366 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/etc/coordio.yml
+-rw-r--r--   0 runner     (501) staff       (20)      722 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    12748 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/extraction.py
+-rwxr-xr-x   0 runner     (501) staff       (20)    13362 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/fitData.py
+-rw-r--r--   0 runner     (501) staff       (20)    30645 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     5870 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/iers.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.368413 sdss-coordio-1.7.1/src/coordio/include/
+-rw-r--r--   0 runner     (501) staff       (20)     1992 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/include/coordio.h
+-rw-r--r--   0 runner     (501) staff       (20)     4013 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     4146 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/site.py
+-rw-r--r--   0 runner     (501) staff       (20)    14255 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     6440 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/sofa_bindings.py
+-rw-r--r--   0 runner     (501) staff       (20)    10661 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)    13390 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     6451 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/time.py
+-rw-r--r--   0 runner     (501) staff       (20)    51462 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/transforms.py
+-rw-r--r--   0 runner     (501) staff       (20)    33682 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     3734 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/wok.py
+-rw-r--r--   0 runner     (501) staff       (20)    14872 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/zernike.py
+-rw-r--r--   0 runner     (501) staff       (20)    12907 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/src/coordio/zhaoburge.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.467072 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     1737 2023-04-25 15:59:53.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6867 2023-04-25 15:59:53.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-25 15:59:53.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-25 15:58:37.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      483 2023-04-25 15:59:53.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        8 2023-04-25 15:59:53.000000 sdss-coordio-1.7.1/src/sdss_coordio.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-25 15:59:54.479612 sdss-coordio-1.7.1/tests/
+-rw-r--r--   0 runner     (501) staff       (20)    13006 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     7006 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_coordinate.py
+-rw-r--r--   0 runner     (501) staff       (20)     1386 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_fpScale.py
+-rw-r--r--   0 runner     (501) staff       (20)     4290 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_guide.py
+-rw-r--r--   0 runner     (501) staff       (20)     1418 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_iers.py
+-rw-r--r--   0 runner     (501) staff       (20)    11447 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_libcoordio.py
+-rw-r--r--   0 runner     (501) staff       (20)     5197 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_offset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8074 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_plPlug.py
+-rw-r--r--   0 runner     (501) staff       (20)     5525 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_positioner.py
+-rw-r--r--   0 runner     (501) staff       (20)     1105 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_site.py
+-rw-r--r--   0 runner     (501) staff       (20)     5302 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_sky.py
+-rw-r--r--   0 runner     (501) staff       (20)     1171 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_sofa.py
+-rw-r--r--   0 runner     (501) staff       (20)     3340 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_tangent.py
+-rw-r--r--   0 runner     (501) staff       (20)     2738 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_tangentToPositioner2.py
+-rw-r--r--   0 runner     (501) staff       (20)    13872 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_telescope.py
+-rw-r--r--   0 runner     (501) staff       (20)     1407 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_time.py
+-rw-r--r--   0 runner     (501) staff       (20)     2588 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_wok.py
+-rw-r--r--   0 runner     (501) staff       (20)     1363 2023-04-25 15:58:00.000000 sdss-coordio-1.7.1/tests/test_zern.py
```

### Comparing `sdss-coordio-1.7.0/LICENSE.md` & `sdss-coordio-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/PKG-INFO` & `sdss-coordio-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.7.0
+Version: 1.7.1
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.0/README.md` & `sdss-coordio-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/conv.cpp` & `sdss-coordio-1.7.1/cextern/conv.cpp`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dallpeaks.c` & `sdss-coordio-1.7.1/cextern/dimage/dallpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dcen3x3.c` & `sdss-coordio-1.7.1/cextern/dimage/dcen3x3.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dfind.c` & `sdss-coordio-1.7.1/cextern/dimage/dfind.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dfloodfill.c` & `sdss-coordio-1.7.1/cextern/dimage/dfloodfill.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dimage.h` & `sdss-coordio-1.7.1/cextern/dimage/dimage.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dmedsmooth.c` & `sdss-coordio-1.7.1/cextern/dimage/dmedsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dobjects.c` & `sdss-coordio-1.7.1/cextern/dimage/dobjects.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dpeaks.c` & `sdss-coordio-1.7.1/cextern/dimage/dpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/drefine.c` & `sdss-coordio-1.7.1/cextern/dimage/drefine.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dselip.c` & `sdss-coordio-1.7.1/cextern/dimage/dselip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dsigma.c` & `sdss-coordio-1.7.1/cextern/dimage/dsigma.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/dsmooth.c` & `sdss-coordio-1.7.1/cextern/dimage/dsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/dimage/simplexy.c` & `sdss-coordio-1.7.1/cextern/dimage/simplexy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/a2af.c` & `sdss-coordio-1.7.1/cextern/sofa/a2af.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/a2tf.c` & `sdss-coordio-1.7.1/cextern/sofa/a2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ab.c` & `sdss-coordio-1.7.1/cextern/sofa/ab.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ae2hd.c` & `sdss-coordio-1.7.1/cextern/sofa/ae2hd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/af2a.c` & `sdss-coordio-1.7.1/cextern/sofa/af2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/anp.c` & `sdss-coordio-1.7.1/cextern/sofa/anp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/anpm.c` & `sdss-coordio-1.7.1/cextern/sofa/anpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apcg.c` & `sdss-coordio-1.7.1/cextern/sofa/apcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apcg13.c` & `sdss-coordio-1.7.1/cextern/sofa/apcg13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apci.c` & `sdss-coordio-1.7.1/cextern/sofa/apci.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apci13.c` & `sdss-coordio-1.7.1/cextern/sofa/apci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apco.c` & `sdss-coordio-1.7.1/cextern/sofa/apco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apco13.c` & `sdss-coordio-1.7.1/cextern/sofa/apco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apcs.c` & `sdss-coordio-1.7.1/cextern/sofa/apcs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apcs13.c` & `sdss-coordio-1.7.1/cextern/sofa/apcs13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/aper.c` & `sdss-coordio-1.7.1/cextern/sofa/aper.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/aper13.c` & `sdss-coordio-1.7.1/cextern/sofa/aper13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apio.c` & `sdss-coordio-1.7.1/cextern/sofa/apio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/apio13.c` & `sdss-coordio-1.7.1/cextern/sofa/apio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atci13.c` & `sdss-coordio-1.7.1/cextern/sofa/atci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atciq.c` & `sdss-coordio-1.7.1/cextern/sofa/atciq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atciqn.c` & `sdss-coordio-1.7.1/cextern/sofa/atciqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atciqz.c` & `sdss-coordio-1.7.1/cextern/sofa/atciqz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atco13.c` & `sdss-coordio-1.7.1/cextern/sofa/atco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atic13.c` & `sdss-coordio-1.7.1/cextern/sofa/atic13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/aticq.c` & `sdss-coordio-1.7.1/cextern/sofa/aticq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/aticqn.c` & `sdss-coordio-1.7.1/cextern/sofa/aticqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atio13.c` & `sdss-coordio-1.7.1/cextern/sofa/atio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atioq.c` & `sdss-coordio-1.7.1/cextern/sofa/atioq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atoc13.c` & `sdss-coordio-1.7.1/cextern/sofa/atoc13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atoi13.c` & `sdss-coordio-1.7.1/cextern/sofa/atoi13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/atoiq.c` & `sdss-coordio-1.7.1/cextern/sofa/atoiq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/bi00.c` & `sdss-coordio-1.7.1/cextern/sofa/bi00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/bp00.c` & `sdss-coordio-1.7.1/cextern/sofa/bp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/bp06.c` & `sdss-coordio-1.7.1/cextern/sofa/bp06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/bpn2xy.c` & `sdss-coordio-1.7.1/cextern/sofa/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2i00a.c` & `sdss-coordio-1.7.1/cextern/sofa/c2i00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2i00b.c` & `sdss-coordio-1.7.1/cextern/sofa/c2i00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2i06a.c` & `sdss-coordio-1.7.1/cextern/sofa/c2i06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2ibpn.c` & `sdss-coordio-1.7.1/cextern/sofa/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2ixy.c` & `sdss-coordio-1.7.1/cextern/sofa/c2ixy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2ixys.c` & `sdss-coordio-1.7.1/cextern/sofa/c2ixys.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2s.c` & `sdss-coordio-1.7.1/cextern/sofa/c2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2t00a.c` & `sdss-coordio-1.7.1/cextern/sofa/c2t00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2t00b.c` & `sdss-coordio-1.7.1/cextern/sofa/c2t00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2t06a.c` & `sdss-coordio-1.7.1/cextern/sofa/c2t06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2tcio.c` & `sdss-coordio-1.7.1/cextern/sofa/c2tcio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2teqx.c` & `sdss-coordio-1.7.1/cextern/sofa/c2teqx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2tpe.c` & `sdss-coordio-1.7.1/cextern/sofa/c2tpe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/c2txy.c` & `sdss-coordio-1.7.1/cextern/sofa/c2txy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/cal2jd.c` & `sdss-coordio-1.7.1/cextern/sofa/cal2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/cp.c` & `sdss-coordio-1.7.1/cextern/sofa/cp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/cpv.c` & `sdss-coordio-1.7.1/cextern/sofa/cpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/cr.c` & `sdss-coordio-1.7.1/cextern/sofa/cr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/d2dtf.c` & `sdss-coordio-1.7.1/cextern/sofa/d2dtf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/d2tf.c` & `sdss-coordio-1.7.1/cextern/sofa/d2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/dat.c` & `sdss-coordio-1.7.1/cextern/sofa/dat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/dtdb.c` & `sdss-coordio-1.7.1/cextern/sofa/dtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/dtf2d.c` & `sdss-coordio-1.7.1/cextern/sofa/dtf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eceq06.c` & `sdss-coordio-1.7.1/cextern/sofa/eceq06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ecm06.c` & `sdss-coordio-1.7.1/cextern/sofa/ecm06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ee00.c` & `sdss-coordio-1.7.1/cextern/sofa/ee00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ee00a.c` & `sdss-coordio-1.7.1/cextern/sofa/ee00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ee00b.c` & `sdss-coordio-1.7.1/cextern/sofa/ee00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ee06a.c` & `sdss-coordio-1.7.1/cextern/sofa/ee06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eect00.c` & `sdss-coordio-1.7.1/cextern/sofa/eect00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eform.c` & `sdss-coordio-1.7.1/cextern/sofa/eform.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eo06a.c` & `sdss-coordio-1.7.1/cextern/sofa/eo06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eors.c` & `sdss-coordio-1.7.1/cextern/sofa/eors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/epb.c` & `sdss-coordio-1.7.1/cextern/sofa/epb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/epb2jd.c` & `sdss-coordio-1.7.1/cextern/sofa/epb2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/epj.c` & `sdss-coordio-1.7.1/cextern/sofa/epj.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/epj2jd.c` & `sdss-coordio-1.7.1/cextern/sofa/epj2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/epv00.c` & `sdss-coordio-1.7.1/cextern/sofa/epv00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eqec06.c` & `sdss-coordio-1.7.1/cextern/sofa/eqec06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/eqeq94.c` & `sdss-coordio-1.7.1/cextern/sofa/eqeq94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/era00.c` & `sdss-coordio-1.7.1/cextern/sofa/era00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fad03.c` & `sdss-coordio-1.7.1/cextern/sofa/fad03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fae03.c` & `sdss-coordio-1.7.1/cextern/sofa/fae03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/faf03.c` & `sdss-coordio-1.7.1/cextern/sofa/faf03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/faju03.c` & `sdss-coordio-1.7.1/cextern/sofa/faju03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fal03.c` & `sdss-coordio-1.7.1/cextern/sofa/fal03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/falp03.c` & `sdss-coordio-1.7.1/cextern/sofa/falp03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fama03.c` & `sdss-coordio-1.7.1/cextern/sofa/fama03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fame03.c` & `sdss-coordio-1.7.1/cextern/sofa/fame03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fane03.c` & `sdss-coordio-1.7.1/cextern/sofa/fane03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/faom03.c` & `sdss-coordio-1.7.1/cextern/sofa/faom03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fapa03.c` & `sdss-coordio-1.7.1/cextern/sofa/fapa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fasa03.c` & `sdss-coordio-1.7.1/cextern/sofa/fasa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/faur03.c` & `sdss-coordio-1.7.1/cextern/sofa/faur03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fave03.c` & `sdss-coordio-1.7.1/cextern/sofa/fave03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk425.c` & `sdss-coordio-1.7.1/cextern/sofa/fk425.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk45z.c` & `sdss-coordio-1.7.1/cextern/sofa/fk45z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk524.c` & `sdss-coordio-1.7.1/cextern/sofa/fk524.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk52h.c` & `sdss-coordio-1.7.1/cextern/sofa/fk52h.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk54z.c` & `sdss-coordio-1.7.1/cextern/sofa/fk54z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk5hip.c` & `sdss-coordio-1.7.1/cextern/sofa/fk5hip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fk5hz.c` & `sdss-coordio-1.7.1/cextern/sofa/fk5hz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fw2m.c` & `sdss-coordio-1.7.1/cextern/sofa/fw2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/fw2xy.c` & `sdss-coordio-1.7.1/cextern/sofa/fw2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/g2icrs.c` & `sdss-coordio-1.7.1/cextern/sofa/g2icrs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gc2gd.c` & `sdss-coordio-1.7.1/cextern/sofa/gc2gd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gc2gde.c` & `sdss-coordio-1.7.1/cextern/sofa/gc2gde.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gd2gc.c` & `sdss-coordio-1.7.1/cextern/sofa/gd2gc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gd2gce.c` & `sdss-coordio-1.7.1/cextern/sofa/gd2gce.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gmst00.c` & `sdss-coordio-1.7.1/cextern/sofa/gmst00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gmst06.c` & `sdss-coordio-1.7.1/cextern/sofa/gmst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gmst82.c` & `sdss-coordio-1.7.1/cextern/sofa/gmst82.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gst00a.c` & `sdss-coordio-1.7.1/cextern/sofa/gst00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gst00b.c` & `sdss-coordio-1.7.1/cextern/sofa/gst00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gst06.c` & `sdss-coordio-1.7.1/cextern/sofa/gst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gst06a.c` & `sdss-coordio-1.7.1/cextern/sofa/gst06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/gst94.c` & `sdss-coordio-1.7.1/cextern/sofa/gst94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/h2fk5.c` & `sdss-coordio-1.7.1/cextern/sofa/h2fk5.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/hd2ae.c` & `sdss-coordio-1.7.1/cextern/sofa/hd2ae.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/hd2pa.c` & `sdss-coordio-1.7.1/cextern/sofa/hd2pa.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/hfk5z.c` & `sdss-coordio-1.7.1/cextern/sofa/hfk5z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/icrs2g.c` & `sdss-coordio-1.7.1/cextern/sofa/icrs2g.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ir.c` & `sdss-coordio-1.7.1/cextern/sofa/ir.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/jd2cal.c` & `sdss-coordio-1.7.1/cextern/sofa/jd2cal.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/jdcalf.c` & `sdss-coordio-1.7.1/cextern/sofa/jdcalf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ld.c` & `sdss-coordio-1.7.1/cextern/sofa/ld.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ldn.c` & `sdss-coordio-1.7.1/cextern/sofa/ldn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ldsun.c` & `sdss-coordio-1.7.1/cextern/sofa/ldsun.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/lteceq.c` & `sdss-coordio-1.7.1/cextern/sofa/lteceq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ltecm.c` & `sdss-coordio-1.7.1/cextern/sofa/ltecm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/lteqec.c` & `sdss-coordio-1.7.1/cextern/sofa/lteqec.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ltp.c` & `sdss-coordio-1.7.1/cextern/sofa/ltp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ltpb.c` & `sdss-coordio-1.7.1/cextern/sofa/ltpb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ltpecl.c` & `sdss-coordio-1.7.1/cextern/sofa/ltpecl.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ltpequ.c` & `sdss-coordio-1.7.1/cextern/sofa/ltpequ.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/makefile` & `sdss-coordio-1.7.1/cextern/sofa/makefile`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/num00a.c` & `sdss-coordio-1.7.1/cextern/sofa/num00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/num00b.c` & `sdss-coordio-1.7.1/cextern/sofa/num00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/num06a.c` & `sdss-coordio-1.7.1/cextern/sofa/num06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/numat.c` & `sdss-coordio-1.7.1/cextern/sofa/numat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/nut00a.c` & `sdss-coordio-1.7.1/cextern/sofa/nut00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/nut00b.c` & `sdss-coordio-1.7.1/cextern/sofa/nut00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/nut06a.c` & `sdss-coordio-1.7.1/cextern/sofa/nut06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/nut80.c` & `sdss-coordio-1.7.1/cextern/sofa/nut80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/nutm80.c` & `sdss-coordio-1.7.1/cextern/sofa/nutm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/obl06.c` & `sdss-coordio-1.7.1/cextern/sofa/obl06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/obl80.c` & `sdss-coordio-1.7.1/cextern/sofa/obl80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/p06e.c` & `sdss-coordio-1.7.1/cextern/sofa/p06e.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/p2pv.c` & `sdss-coordio-1.7.1/cextern/sofa/p2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/p2s.c` & `sdss-coordio-1.7.1/cextern/sofa/p2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pap.c` & `sdss-coordio-1.7.1/cextern/sofa/pap.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pas.c` & `sdss-coordio-1.7.1/cextern/sofa/pas.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pb06.c` & `sdss-coordio-1.7.1/cextern/sofa/pb06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pdp.c` & `sdss-coordio-1.7.1/cextern/sofa/pdp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pfw06.c` & `sdss-coordio-1.7.1/cextern/sofa/pfw06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/plan94.c` & `sdss-coordio-1.7.1/cextern/sofa/plan94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pm.c` & `sdss-coordio-1.7.1/cextern/sofa/pm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmat00.c` & `sdss-coordio-1.7.1/cextern/sofa/pmat00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmat06.c` & `sdss-coordio-1.7.1/cextern/sofa/pmat06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmat76.c` & `sdss-coordio-1.7.1/cextern/sofa/pmat76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmp.c` & `sdss-coordio-1.7.1/cextern/sofa/pmp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmpx.c` & `sdss-coordio-1.7.1/cextern/sofa/pmpx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pmsafe.c` & `sdss-coordio-1.7.1/cextern/sofa/pmsafe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn.c` & `sdss-coordio-1.7.1/cextern/sofa/pn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn00.c` & `sdss-coordio-1.7.1/cextern/sofa/pn00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn00a.c` & `sdss-coordio-1.7.1/cextern/sofa/pn00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn00b.c` & `sdss-coordio-1.7.1/cextern/sofa/pn00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn06.c` & `sdss-coordio-1.7.1/cextern/sofa/pn06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pn06a.c` & `sdss-coordio-1.7.1/cextern/sofa/pn06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pnm00a.c` & `sdss-coordio-1.7.1/cextern/sofa/pnm00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pnm00b.c` & `sdss-coordio-1.7.1/cextern/sofa/pnm00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pnm06a.c` & `sdss-coordio-1.7.1/cextern/sofa/pnm06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pnm80.c` & `sdss-coordio-1.7.1/cextern/sofa/pnm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pom00.c` & `sdss-coordio-1.7.1/cextern/sofa/pom00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ppp.c` & `sdss-coordio-1.7.1/cextern/sofa/ppp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ppsp.c` & `sdss-coordio-1.7.1/cextern/sofa/ppsp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pr00.c` & `sdss-coordio-1.7.1/cextern/sofa/pr00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/prec76.c` & `sdss-coordio-1.7.1/cextern/sofa/prec76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pv2p.c` & `sdss-coordio-1.7.1/cextern/sofa/pv2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pv2s.c` & `sdss-coordio-1.7.1/cextern/sofa/pv2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvdpv.c` & `sdss-coordio-1.7.1/cextern/sofa/pvdpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvm.c` & `sdss-coordio-1.7.1/cextern/sofa/pvm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvmpv.c` & `sdss-coordio-1.7.1/cextern/sofa/pvmpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvppv.c` & `sdss-coordio-1.7.1/cextern/sofa/pvppv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvstar.c` & `sdss-coordio-1.7.1/cextern/sofa/pvstar.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvtob.c` & `sdss-coordio-1.7.1/cextern/sofa/pvtob.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvu.c` & `sdss-coordio-1.7.1/cextern/sofa/pvu.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvup.c` & `sdss-coordio-1.7.1/cextern/sofa/pvup.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pvxpv.c` & `sdss-coordio-1.7.1/cextern/sofa/pvxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/pxp.c` & `sdss-coordio-1.7.1/cextern/sofa/pxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/refco.c` & `sdss-coordio-1.7.1/cextern/sofa/refco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rm2v.c` & `sdss-coordio-1.7.1/cextern/sofa/rm2v.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rv2m.c` & `sdss-coordio-1.7.1/cextern/sofa/rv2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rx.c` & `sdss-coordio-1.7.1/cextern/sofa/rx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rxp.c` & `sdss-coordio-1.7.1/cextern/sofa/rxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rxpv.c` & `sdss-coordio-1.7.1/cextern/sofa/rxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rxr.c` & `sdss-coordio-1.7.1/cextern/sofa/rxr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ry.c` & `sdss-coordio-1.7.1/cextern/sofa/ry.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/rz.c` & `sdss-coordio-1.7.1/cextern/sofa/rz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s00.c` & `sdss-coordio-1.7.1/cextern/sofa/s00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s00a.c` & `sdss-coordio-1.7.1/cextern/sofa/s00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s00b.c` & `sdss-coordio-1.7.1/cextern/sofa/s00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s06.c` & `sdss-coordio-1.7.1/cextern/sofa/s06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s06a.c` & `sdss-coordio-1.7.1/cextern/sofa/s06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s2c.c` & `sdss-coordio-1.7.1/cextern/sofa/s2c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s2p.c` & `sdss-coordio-1.7.1/cextern/sofa/s2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s2pv.c` & `sdss-coordio-1.7.1/cextern/sofa/s2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/s2xpv.c` & `sdss-coordio-1.7.1/cextern/sofa/s2xpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sepp.c` & `sdss-coordio-1.7.1/cextern/sofa/sepp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/seps.c` & `sdss-coordio-1.7.1/cextern/sofa/seps.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sofa.h` & `sdss-coordio-1.7.1/cextern/sofa/sofa.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sofam.h` & `sdss-coordio-1.7.1/cextern/sofa/sofam.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sp00.c` & `sdss-coordio-1.7.1/cextern/sofa/sp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/starpm.c` & `sdss-coordio-1.7.1/cextern/sofa/starpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/starpv.c` & `sdss-coordio-1.7.1/cextern/sofa/starpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sxp.c` & `sdss-coordio-1.7.1/cextern/sofa/sxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/sxpv.c` & `sdss-coordio-1.7.1/cextern/sofa/sxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/t_sofa_c.c` & `sdss-coordio-1.7.1/cextern/sofa/t_sofa_c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/taitt.c` & `sdss-coordio-1.7.1/cextern/sofa/taitt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/taiut1.c` & `sdss-coordio-1.7.1/cextern/sofa/taiut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/taiutc.c` & `sdss-coordio-1.7.1/cextern/sofa/taiutc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tcbtdb.c` & `sdss-coordio-1.7.1/cextern/sofa/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tcgtt.c` & `sdss-coordio-1.7.1/cextern/sofa/tcgtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tdbtcb.c` & `sdss-coordio-1.7.1/cextern/sofa/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tdbtt.c` & `sdss-coordio-1.7.1/cextern/sofa/tdbtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tf2a.c` & `sdss-coordio-1.7.1/cextern/sofa/tf2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tf2d.c` & `sdss-coordio-1.7.1/cextern/sofa/tf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tpors.c` & `sdss-coordio-1.7.1/cextern/sofa/tpors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tporv.c` & `sdss-coordio-1.7.1/cextern/sofa/tporv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tpsts.c` & `sdss-coordio-1.7.1/cextern/sofa/tpsts.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tpstv.c` & `sdss-coordio-1.7.1/cextern/sofa/tpstv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tpxes.c` & `sdss-coordio-1.7.1/cextern/sofa/tpxes.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tpxev.c` & `sdss-coordio-1.7.1/cextern/sofa/tpxev.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tr.c` & `sdss-coordio-1.7.1/cextern/sofa/tr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/trxp.c` & `sdss-coordio-1.7.1/cextern/sofa/trxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/trxpv.c` & `sdss-coordio-1.7.1/cextern/sofa/trxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tttai.c` & `sdss-coordio-1.7.1/cextern/sofa/tttai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tttcg.c` & `sdss-coordio-1.7.1/cextern/sofa/tttcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/tttdb.c` & `sdss-coordio-1.7.1/cextern/sofa/tttdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ttut1.c` & `sdss-coordio-1.7.1/cextern/sofa/ttut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ut1tai.c` & `sdss-coordio-1.7.1/cextern/sofa/ut1tai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ut1tt.c` & `sdss-coordio-1.7.1/cextern/sofa/ut1tt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/ut1utc.c` & `sdss-coordio-1.7.1/cextern/sofa/ut1utc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/utctai.c` & `sdss-coordio-1.7.1/cextern/sofa/utctai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/utcut1.c` & `sdss-coordio-1.7.1/cextern/sofa/utcut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/xy06.c` & `sdss-coordio-1.7.1/cextern/sofa/xy06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/xys00a.c` & `sdss-coordio-1.7.1/cextern/sofa/xys00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/xys00b.c` & `sdss-coordio-1.7.1/cextern/sofa/xys00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/xys06a.c` & `sdss-coordio-1.7.1/cextern/sofa/xys06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/zp.c` & `sdss-coordio-1.7.1/cextern/sofa/zp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/zpv.c` & `sdss-coordio-1.7.1/cextern/sofa/zpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/cextern/sofa/zr.c` & `sdss-coordio-1.7.1/cextern/sofa/zr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/setup.cfg` & `sdss-coordio-1.7.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-coordio
-version = 1.7.0
+version = 1.7.1
 author = Conor Sayres
 author_email = csayres@uw.edu
 description = Coordinate conversion for SDSS-V
 url = https://github.com/sdss/coordio
 project_urls = 
 	Repository = https://github.com/sdss/coordio
 	Documentation = https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.0/setup.py` & `sdss-coordio-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/__init__.py` & `sdss-coordio-1.7.1/src/coordio/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/astrometry.py` & `sdss-coordio-1.7.1/src/coordio/astrometry.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/calibration.py` & `sdss-coordio-1.7.1/src/coordio/calibration.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/conv.py` & `sdss-coordio-1.7.1/src/coordio/conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/coordinate.py` & `sdss-coordio-1.7.1/src/coordio/coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/defaults.py` & `sdss-coordio-1.7.1/src/coordio/defaults.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/exceptions.py` & `sdss-coordio-1.7.1/src/coordio/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/extraction.py` & `sdss-coordio-1.7.1/src/coordio/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/fitData.py` & `sdss-coordio-1.7.1/src/coordio/fitData.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/guide.py` & `sdss-coordio-1.7.1/src/coordio/guide.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import pathlib
 import re
 import warnings
 from dataclasses import dataclass
 from typing import Any
 
 import numpy
+import numpy.typing as nt
 import pandas
 import scipy.ndimage
 from astropy.coordinates import SkyCoord
 from astropy.io import fits
 from astropy.time import Time
 from astropy.wcs import WCS, FITSFixedWarning
 from astropy.wcs.utils import fit_wcs_from_points
+from matplotlib import pyplot as plt
 from scipy.spatial import KDTree
 from skimage.registration import phase_cross_correlation
 
 from coordio.conv import guideToTangent, tangentToWok
 
 from . import Site, calibration, defaults
 from .astrometry import astrometrynet_quick
@@ -73,15 +75,14 @@
     __warn_arrays__ = ["guide_warn"]
 
     xBin: int
     yBin: int
     guide_warn: numpy.ndarray
 
     def __new__(cls, value, **kwargs):
-
         xBin = kwargs.get("xBin", None)
         if xBin is None:
             kwargs["xBin"] = 1
 
         yBin = kwargs.get("yBin", None)
         if yBin is None:
             kwargs["yBin"] = 1
@@ -215,16 +216,15 @@
     focal = FocalPlane(wok, wavelength=wavelength, site=site)
     field = Field(focal, field_center=boresight)
     observed = Observed(field, wavelength=wavelength, site=site)
 
     if icrs is False:
         return (observed.ra[0], observed.dec[0])
     else:
-        icrs = ICRS(observed)
-        return icrs[0]
+        return ICRS(observed)[0]
 
 
 def radec_to_gfa(
     observatory: str,
     ra: float | numpy.ndarray,
     dec: float | numpy.ndarray,
     gfa_id: int,
@@ -451,31 +451,35 @@
     return wcs, error
 
 
 @dataclass
 class GuiderFit:
     """Results of a guider data fit."""
 
+    cameras: list[int]
     gfa_wok: pandas.DataFrame
     astro_wok: pandas.DataFrame
+    coeffs: list[float]
     delta_ra: float
     delta_dec: float
     delta_rot: float
     delta_scale: float
     xrms: float
     yrms: float
     rms: float
+    rms_data: pandas.DataFrame
+    fit: pandas.DataFrame
+    fit_rms: pandas.DataFrame
     only_radec: bool = False
 
 
 class GuiderFitter:
     """Fits guider data, returning the measured offsets."""
 
     def __init__(self, observatory: str):
-
         self.observatory = observatory.upper()
 
         self.plate_scale = defaults.PLATE_SCALE[self.observatory]
         self.pixel_size = defaults.GFA_PIXEL_SIZE
         self.pixel_scale = 1.0 / self.plate_scale * self.pixel_size * 3600 / 1000
 
         self.reference_pixel: tuple[int, int] = (1024, 1024)
@@ -501,15 +505,14 @@
             )
 
         gfaCoords = calibration.gfaCoords.loc[self.observatory]
 
         wok_coords = {}
 
         for gfa_id in range(1, 7):
-
             camera_coords: pandas.DataFrame = gfaCoords.loc[gfa_id]
 
             b = camera_coords[["xWok", "yWok", "zWok"]].to_numpy().squeeze()
             iHat = camera_coords[["ix", "iy", "iz"]].to_numpy().squeeze()
             jHat = camera_coords[["jx", "jy", "jz"]].to_numpy().squeeze()
             kHat = camera_coords[["kx", "ky", "kz"]].to_numpy().squeeze()
 
@@ -629,21 +632,20 @@
         self,
         path: str | pathlib.Path,
         pixels: numpy.ndarray | None = None,
     ):
         """Adds an astrometric solution from a ``proc-gimg`` image."""
 
         hdu = fits.open(str(path))
+        header = hdu[1].header
 
-        is_proc = len(hdu) > 1 and "SOLVED" in hdu[1].header
+        is_proc = len(hdu) > 1 and "SOLVED" in header
         if not is_proc:
             raise CoordIOError(f"{path!s} is not a proc-gimg image.")
 
-        header = hdu[1].header
-
         if header["OBSERVAT"] != self.observatory:
             raise CoordIOError("GFA image is from a different observatory.")
 
         if not header.get("SOLVED", False):
             raise CoordIOError(f"Image {path!s} has not been astrometrically solved.")
 
         wcs = WCS(header)
@@ -655,14 +657,15 @@
         self,
         field_ra: float,
         field_dec: float,
         field_pa: float = 0.0,
         offset: tuple[float, float, float] | numpy.ndarray = (0.0, 0.0, 0.0),
         scale_rms: bool = False,
         only_radec: bool = False,
+        cameras: list[int] | None = None,
     ):
         """Performs the fit and returns a `.GuiderFit` object.
 
         The fit is performed using `.umeyama`.
 
         Parameters
         ----------
@@ -691,18 +694,21 @@
             raise CoordIOError("Astro data has not been set.")
 
         camera_ids: list[int] = []
         xwok_gfa: list[float] = []
         ywok_gfa: list[float] = []
         xwok_astro: list[float] = []
         ywok_astro: list[float] = []
+        use_detections: list[bool] = []
+        used_cameras: set[int] = set([])
 
         for d in self.astro_data.itertuples():
-
-            camera_id: int = d.gfa_id
+            camera_id: int = int(d.gfa_id)
+            if cameras is None or camera_id in cameras:
+                used_cameras.add(camera_id)
 
             camera_ids.append(camera_id)
 
             x_wok, y_wok, _ = gfa_to_wok(self.observatory, d.x, d.y, camera_id)
             xwok_gfa.append(x_wok)
             ywok_gfa.append(y_wok)
 
@@ -718,35 +724,42 @@
                 d.obstime,
                 focalScale=1.0,  # Guider scale is relative to 1
             )
 
             xwok_astro += _xwok_astro.tolist()
             ywok_astro += _ywok_astro.tolist()
 
-        # X: GFA to wok coordinates as a 2D array
-        # Y: ICRS to wok coordinates as a 2D array
-        X = numpy.array([xwok_gfa, ywok_gfa])
-        Y = numpy.array([xwok_astro, ywok_astro])
+            # Use these detections fit unless we are excluding the camera.
+            use_detections.append(cameras is None or camera_id in cameras)
+
+        # Create arrays with all detections, then with only selected ones.
+        X_all: nt.NDArray[numpy.float32] = numpy.array([xwok_gfa, ywok_gfa])
+        Y_all: nt.NDArray[numpy.float32] = numpy.array([xwok_astro, ywok_astro])
+        X_fit = X_all[:, use_detections]  # GFA to wok coordinates as a 2D array
+        Y_fit = Y_all[:, use_detections]  # ICRS to wok coordinates as a 2D array
 
         try:
-            c, R, t = umeyama(X, Y)
+            c, R, t = umeyama(X_fit, Y_fit)
         except ValueError:
             if only_radec is True:
                 warnings.warn(
                     "Cannot fit using Umeyama. Assuming unitary rotation and scale.",
                     CoordIOUserWarning,
                 )
                 c = 1.0
                 R = numpy.array([[1, 0], [1, 0]])
+                t = numpy.array([0.0, 0.0])
             else:
                 return False
 
         if only_radec is True:
             # Override the translation component with a simple average translation
-            t = (Y - X).mean(axis=1).T
+            t = (Y_fit - X_fit).mean(axis=1).T
+
+        coeffs = [c, R, t]
 
         # delta_x and delta_y only align with RA/Dec if PA=0. Otherwise we need to
         # project using the PA.
         pa_rad = numpy.deg2rad(field_pa - offset_pa / 3600.0)
         delta_ra = t[0] * numpy.cos(pa_rad) + t[1] * numpy.sin(pa_rad)
         delta_dec = -t[0] * numpy.sin(pa_rad) + t[1] * numpy.cos(pa_rad)
 
@@ -755,45 +768,208 @@
         delta_dec = float(numpy.round(delta_dec / self.plate_scale * 3600.0, 3))
 
         delta_rot = -numpy.rad2deg(numpy.arctan2(R[1, 0], R[0, 0])) * 3600.0
         delta_rot = float(numpy.round(delta_rot, 1))
 
         delta_scale = float(numpy.round(c, 6))
 
-        if scale_rms:
-            xwok_astro = list(numpy.array(xwok_astro) / delta_scale)
-            ywok_astro = list(numpy.array(ywok_astro) / delta_scale)
-
-        delta_x = (numpy.array(xwok_gfa) - numpy.array(xwok_astro)) ** 2
-        delta_y = (numpy.array(ywok_gfa) - numpy.array(ywok_astro)) ** 2
-
-        xrms = numpy.sqrt(numpy.sum(delta_x) / len(delta_x))
-        yrms = numpy.sqrt(numpy.sum(delta_y) / len(delta_y))
-        rms = numpy.sqrt(numpy.sum(delta_x + delta_y) / len(delta_x))
-
-        # Convert to arcsec and round up
-        xrms = float(numpy.round(xrms / self.plate_scale * 3600.0, 3))
-        yrms = float(numpy.round(yrms / self.plate_scale * 3600.0, 3))
-        rms = float(numpy.round(rms / self.plate_scale * 3600.0, 3))
+        detection_id = numpy.arange(len(xwok_astro)) + 1
 
         astro_wok = pandas.DataFrame.from_records(
-            {"gfa_id": camera_ids, "xwok": xwok_astro, "ywok": ywok_astro}
+            {
+                "gfa_id": camera_ids,
+                "detection_id": detection_id,
+                "xwok": xwok_astro.copy(),
+                "ywok": ywok_astro.copy(),
+                "selected": numpy.array(use_detections).astype(int),
+            },
+            index=["gfa_id", "detection_id"],
         )
 
         gfa_wok = pandas.DataFrame.from_records(
-            {"gfa_id": camera_ids, "xwok": xwok_gfa, "ywok": ywok_gfa}
+            {
+                "gfa_id": camera_ids,
+                "detection_id": detection_id,
+                "xwok": xwok_gfa.copy(),
+                "ywok": ywok_gfa.copy(),
+                "selected": numpy.array(use_detections).astype(int),
+            },
+            index=["gfa_id", "detection_id"],
         )
 
+        rms_df = self.calculate_rms(gfa_wok, astro_wok, scale=c if scale_rms else 1)
+
+        fit_data = c * R @ X_all + t[numpy.newaxis].T
+        fit_df = pandas.DataFrame.from_records(
+            {
+                "gfa_id": camera_ids,
+                "detection_id": detection_id,
+                "xwok": fit_data[0, :],
+                "ywok": fit_data[1, :],
+                "selected": numpy.array(use_detections).astype(int),
+            },
+            index=["gfa_id", "detection_id"],
+        )
+        fit_rms_df = self.calculate_rms(fit_df, astro_wok)
+
         self.result = GuiderFit(
+            list(used_cameras),
             gfa_wok,
             astro_wok,
+            coeffs,
             delta_ra,
             delta_dec,
             delta_rot,
             delta_scale,
-            xrms,
-            yrms,
-            rms,
+            rms_df.loc[0].xrms,
+            rms_df.loc[0].yrms,
+            rms_df.loc[0].rms,
+            rms_df,
+            fit_df,
+            fit_rms_df,
             only_radec=only_radec,
         )
 
         return self.result
+
+    def calculate_rms(
+        self,
+        gfa_wok: pandas.DataFrame,
+        astro_wok: pandas.DataFrame,
+        scale: float = 1,
+    ):
+        """Calculates the RMS of the measurements.
+
+        Parameters
+        ----------
+        gfa_wok
+            GFA to wok coordinates data. The data frame contains three columns:
+            ``gfa_id``, ``xwok``, and ``ywok``.
+        astro_wok
+            Astrometric solution to wok coordinates data. The data frame contains
+            three columns: ``gfa_id``, ``xwok``, and ``ywok``.
+        scale
+            Factor by which to scale coordinates.
+
+        Returns
+        -------
+        rms
+            A data frame with columns ``gfa_id``, ``xrms``, ``yrms``, ``rms``
+            for the x, y, and combined RMS measurements for each camera. An
+            additional ``gfa_id=0`` is added with the RMS measurements for all
+            GFA cameras combined. RMS values are returned in mm on wok coordinates.
+
+        """
+
+        def calc_rms(gfa_cam: pandas.DataFrame):
+            gfa_id = gfa_cam.index.values[0][0]
+            astro_cam = astro_wok.loc[gfa_id]
+
+            delta = gfa_cam - astro_cam
+            xrms = numpy.sqrt(numpy.mean(delta.xwok**2))
+            yrms = numpy.sqrt(numpy.mean(delta.ywok**2))
+            rms = numpy.sqrt(numpy.mean(delta.xwok**2 + delta.ywok**2))
+
+            return pandas.Series([xrms, yrms, rms], index=["xrms", "yrms", "rms"])
+
+        astro_wok = astro_wok.copy()
+        gfa_wok = gfa_wok.copy()
+        gfa_wok.loc[:, ["xwok", "ywok"]] *= scale
+
+        rms_df = gfa_wok.groupby("gfa_id").apply(calc_rms)
+
+        delta = gfa_wok - astro_wok
+        xrms = numpy.sqrt(numpy.mean(delta.xwok**2))
+        yrms = numpy.sqrt(numpy.mean(delta.ywok**2))
+        rms = numpy.sqrt(numpy.mean(delta.xwok**2 + delta.ywok**2))
+
+        rms_df.loc[0, :] = (xrms, yrms, rms)
+
+        return rms_df
+
+    def plot_fit(self, filename: str | pathlib.Path):
+        """Plot the fit results."""
+
+        if self.result is None:
+            raise RuntimeError("fit() needs to be run before plot_fit().")
+
+        fig, ax = plt.subplots(2, 3)
+        fig.tight_layout()
+
+        iax = 0
+        jax = 0
+        direction = 1
+        for cam_id in range(1, 7):
+            one_arcsec = self.plate_scale / 3600.0
+
+            camera_note = None
+            color = "k"
+
+            if cam_id in self.result.fit.index:
+                X = self.result.fit.loc[cam_id].xwok
+                Y = self.result.fit.loc[cam_id].ywok
+
+                U = self.result.astro_wok.loc[cam_id].xwok
+                V = self.result.astro_wok.loc[cam_id].ywok
+                U = U - X
+                V = V - Y
+
+                rms_mm = float(self.result.fit_rms.loc[cam_id].rms)
+                rms = numpy.round(rms_mm / self.plate_scale * 3600, 4)
+
+                if self.result.cameras and cam_id not in self.result.cameras:
+                    camera_note = "Not fit"
+                    color = "r"
+
+            else:
+                X = Y = U = V = []
+                rms = -999
+                camera_note = "Disabled / not solved"
+                color = "r"
+
+            q = ax[iax][jax].quiver(
+                X,
+                Y,
+                U,
+                V,
+                color=color,
+                units="xy",
+                angles="xy",
+                scale_units="inches",
+                scale=0.15,
+            )
+
+            if cam_id == 1:
+                ax[iax][jax].quiverkey(q, 0.2, 0.9, one_arcsec, label="1 arcsec")
+
+            text1 = ax[iax][jax].text(
+                0.5,
+                0.95,
+                f"RMS: {rms}",
+                color=color,
+                horizontalalignment="center",
+                verticalalignment="center",
+                transform=ax[iax][jax].transAxes,
+            )
+            text1.set_bbox(dict(facecolor="white", alpha=1, edgecolor="none"))
+
+            if camera_note:
+                text2 = ax[iax][jax].text(
+                    0.5,
+                    0.90,
+                    camera_note,
+                    color=color,
+                    horizontalalignment="center",
+                    verticalalignment="center",
+                    transform=ax[iax][jax].transAxes,
+                )
+                text2.set_bbox(dict(facecolor="white", alpha=1, edgecolor="none"))
+
+            ax[iax][jax].set_title(f"GFA{cam_id}", color=color)
+
+            jax += direction
+            if jax == 3:
+                jax = -1
+                iax = 1
+                direction = -1
+
+        fig.savefig(str(filename))
```

### Comparing `sdss-coordio-1.7.0/src/coordio/iers.py` & `sdss-coordio-1.7.1/src/coordio/iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/include/coordio.h` & `sdss-coordio-1.7.1/src/coordio/include/coordio.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/positioner.py` & `sdss-coordio-1.7.1/src/coordio/positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/site.py` & `sdss-coordio-1.7.1/src/coordio/site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/sky.py` & `sdss-coordio-1.7.1/src/coordio/sky.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/sofa_bindings.py` & `sdss-coordio-1.7.1/src/coordio/sofa_bindings.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/tangent.py` & `sdss-coordio-1.7.1/src/coordio/tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/telescope.py` & `sdss-coordio-1.7.1/src/coordio/telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/time.py` & `sdss-coordio-1.7.1/src/coordio/time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/transforms.py` & `sdss-coordio-1.7.1/src/coordio/transforms.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/utils.py` & `sdss-coordio-1.7.1/src/coordio/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -797,15 +797,15 @@
             if skybrightness <= offset_min_skybrightness:
                 offset_flag[:] += 8
                 r[:] = 0.
     return r, offset_flag
 
 
 def object_offset(mag, mag_limits, lunation, waveName, fmagloss=None,
-                  safety_factor=0.5, beta=5, FWHM=1.7, skybrightness=None,
+                  safety_factor=None, beta=5, FWHM=1.7, skybrightness=None,
                   offset_min_skybrightness=None, can_offset=None):
     """
     Returns the offset needed for object with mag to be
     observed at mag_limit. Currently assumption is all offsets
     are set in positive RA direction.
 
     Parameters
@@ -873,14 +873,19 @@
             - 8: offsets should not be used as sky brightness is <=
                  minimum offset sky brightness
             - 16: no offsets applied because can_offset = False
             - 32: no offset applied because mag <= offset_bright_limit
                   (offset_bright_limit is G = 6 for Boss and
                    H = 1 for Apogee).
     """
+    if safety_factor is None:
+        if lunation == 'bright':
+            safety_factor = 0.5
+        else:
+            safety_factor = 1.0
     delta_ra, offset_flag = offset_definition(mag, mag_limits, lunation, waveName,
                                               fmagloss=fmagloss,
                                               safety_factor=safety_factor, beta=beta,
                                               FWHM=FWHM, skybrightness=skybrightness,
                                               offset_min_skybrightness=offset_min_skybrightness,
                                               can_offset=can_offset)
     if isinstance(delta_ra, float):
```

### Comparing `sdss-coordio-1.7.0/src/coordio/wok.py` & `sdss-coordio-1.7.1/src/coordio/wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/zernike.py` & `sdss-coordio-1.7.1/src/coordio/zernike.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/coordio/zhaoburge.py` & `sdss-coordio-1.7.1/src/coordio/zhaoburge.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/src/sdss_coordio.egg-info/PKG-INFO` & `sdss-coordio-1.7.1/src/sdss_coordio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.7.0
+Version: 1.7.1
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
```

### Comparing `sdss-coordio-1.7.0/src/sdss_coordio.egg-info/SOURCES.txt` & `sdss-coordio-1.7.1/src/sdss_coordio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_conv.py` & `sdss-coordio-1.7.1/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_coordinate.py` & `sdss-coordio-1.7.1/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_fpScale.py` & `sdss-coordio-1.7.1/tests/test_fpScale.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_guide.py` & `sdss-coordio-1.7.1/tests/test_guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_iers.py` & `sdss-coordio-1.7.1/tests/test_iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_libcoordio.py` & `sdss-coordio-1.7.1/tests/test_libcoordio.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_offset.py` & `sdss-coordio-1.7.1/tests/test_offset.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 fmagloss = Moffat2dInterp()
 
 
 def test_all_flags():
     def  test_flags(flag, mag, mag_limits, lunation, waveName,
                     sky, offset_min_skybrightness, can_off):
         delta_ra, delta_dec, offset_flag = object_offset(mag, mag_limits, lunation,
-                                                         waveName, fmagloss=fmagloss, safety_factor=0.1,
-                                                         beta=5, FWHM=1.7, skybrightness=sky,
+                                                         waveName, fmagloss=fmagloss,
+                                                         skybrightness=sky,
                                                          offset_min_skybrightness=offset_min_skybrightness,
                                                          can_offset=can_off)
         assert offset_flag == flag
         assert delta_dec == 0.
         if flag > 0:
             assert delta_ra == 0.
         else:
             assert delta_ra > 0.
 
         if can_off is None:
             can_off_arr = None
         else:
             can_off_arr = numpy.array([can_off])
         delta_ra, delta_dec, offset_flag = object_offset(numpy.array([mag]), mag_limits, lunation,
-                                                         waveName, fmagloss=fmagloss, safety_factor=0.1,
-                                                         beta=5, FWHM=1.7, skybrightness=sky,
+                                                         waveName, fmagloss=fmagloss,
+                                                         skybrightness=sky,
                                                          offset_min_skybrightness=offset_min_skybrightness,
                                                          can_offset=can_off_arr)
         assert numpy.all(offset_flag == flag)
         assert numpy.all(delta_dec == 0.)
         if flag > 0:
             assert numpy.all(delta_ra == 0.)
         else:
```

### Comparing `sdss-coordio-1.7.0/tests/test_plPlug.py` & `sdss-coordio-1.7.1/tests/test_plPlug.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_positioner.py` & `sdss-coordio-1.7.1/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_site.py` & `sdss-coordio-1.7.1/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_sky.py` & `sdss-coordio-1.7.1/tests/test_sky.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_sofa.py` & `sdss-coordio-1.7.1/tests/test_sofa.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_tangent.py` & `sdss-coordio-1.7.1/tests/test_tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_tangentToPositioner2.py` & `sdss-coordio-1.7.1/tests/test_tangentToPositioner2.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_telescope.py` & `sdss-coordio-1.7.1/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_time.py` & `sdss-coordio-1.7.1/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_wok.py` & `sdss-coordio-1.7.1/tests/test_wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.7.0/tests/test_zern.py` & `sdss-coordio-1.7.1/tests/test_zern.py`

 * *Files identical despite different names*

