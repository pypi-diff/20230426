# Comparing `tmp/chronoz-1.0.tar.gz` & `tmp/chronoz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronoz-1.0.tar", last modified: Sun Aug 14 14:57:32 2022, max compression
+gzip compressed data, was "chronoz-1.0.1.tar", last modified: Mon Nov 28 00:59:47 2022, max compression
```

## Comparing `chronoz-1.0.tar` & `chronoz-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-08-14 14:57:32.585909 chronoz-1.0/
--rw-rw-rw-   0        0        0     7167 2022-02-24 20:07:01.000000 chronoz-1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2022-08-14 13:45:35.000000 chronoz-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      474 2022-08-14 14:57:32.585909 chronoz-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-08-14 13:45:14.000000 chronoz-1.0/README.md
--rw-rw-rw-   0        0        0      108 2022-02-21 10:25:54.000000 chronoz-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      710 2022-08-14 14:57:32.585909 chronoz-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-14 14:57:32.564041 chronoz-1.0/src/
-drwxrwxrwx   0        0        0        0 2022-08-14 14:57:32.579398 chronoz-1.0/src/chronoz.egg-info/
--rw-rw-rw-   0        0        0      474 2022-08-14 14:57:32.000000 chronoz-1.0/src/chronoz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2022-08-14 14:57:32.000000 chronoz-1.0/src/chronoz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-14 14:57:32.000000 chronoz-1.0/src/chronoz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-08-14 14:57:32.000000 chronoz-1.0/src/chronoz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-28 00:59:47.439120 chronoz-1.0.1/
+-rw-rw-rw-   0        0        0     7167 2022-02-24 20:07:01.000000 chronoz-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       23 2022-11-28 00:59:23.000000 chronoz-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      476 2022-11-28 00:59:47.439120 chronoz-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-08-14 13:45:14.000000 chronoz-1.0.1/README.md
+-rw-rw-rw-   0        0        0      108 2022-02-21 10:25:54.000000 chronoz-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      712 2022-11-28 00:59:47.439120 chronoz-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-28 00:59:47.416989 chronoz-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2022-11-28 00:59:47.416989 chronoz-1.0.1/src/chronoz/
+-rw-rw-rw-   0        0        0     5579 2022-11-28 00:50:11.000000 chronoz-1.0.1/src/chronoz/chronoz.py
+-rw-rw-rw-   0        0        0        0 2022-08-14 14:48:40.000000 chronoz-1.0.1/src/chronoz/init.py
+drwxrwxrwx   0        0        0        0 2022-11-28 00:59:47.439120 chronoz-1.0.1/src/chronoz.egg-info/
+-rw-rw-rw-   0        0        0      476 2022-11-28 00:59:47.000000 chronoz-1.0.1/src/chronoz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2022-11-28 00:59:47.000000 chronoz-1.0.1/src/chronoz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-28 00:59:47.000000 chronoz-1.0.1/src/chronoz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2022-11-28 00:59:47.000000 chronoz-1.0.1/src/chronoz.egg-info/top_level.txt
```

### Comparing `chronoz-1.0/LICENSE` & `chronoz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chronoz-1.0/setup.cfg` & `chronoz-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6872 6f6e 6f7a 0d0a 7665 7273   = chronoz..vers
-00000020: 696f 6e20 3d20 312e 300d 0a61 7574 686f  ion = 1.0..autho
-00000030: 7220 3d20 5369 6d6f 6e20 5a6f 7a6f 6c0d  r = Simon Zozol.
-00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 7369 6d6f 6e2e 7a6f 7a6f 6c40 676d 6169  simon.zozol@gmai
-00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
-00000070: 6f6e 203d 200d 0a6c 6f6e 675f 6465 7363  on = ..long_desc
-00000080: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000090: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-000000a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000b0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000c0: 6d61 726b 646f 776e 0d0a 6874 7470 7320  markdown..https 
-000000d0: 3d20 2f2f 6269 7462 7563 6b65 742e 6f72  = //bitbucket.or
-000000e0: 672f 686f 6c79 7079 7468 6f6e 2f7a 7a63  g/holypython/zzc
-000000f0: 6872 6f6e 6f2f 7372 632f 6d61 7374 6572  hrono/src/master
-00000100: 2f0d 0a63 6c61 7373 6966 6965 7273 203d  /..classifiers =
-00000110: 200d 0a09 546f 7069 6320 3a3a 2053 6f66   ...Topic :: Sof
-00000120: 7477 6172 6520 4465 7665 6c6f 706d 656e  tware Developmen
-00000130: 740d 0a09 5072 6f67 7261 6d6d 696e 6720  t...Programming 
-00000140: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000150: 6f6e 203a 3a20 332e 360d 0a09 4c69 6365  on :: 3.6...Lice
-00000160: 6e73 6520 3a3a 2043 4330 2031 2e30 2055  nse :: CC0 1.0 U
-00000170: 6e69 7665 7273 616c 2028 4343 3020 312e  niversal (CC0 1.
-00000180: 3029 2050 7562 6c69 6320 446f 6d61 696e  0) Public Domain
-00000190: 2044 6564 6963 6174 696f 6e0d 0a09 4f70   Dedication...Op
-000001a0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-000001b0: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-000001c0: 0d0a 0944 6576 656c 6f70 6d65 6e74 2053  ...Development S
-000001d0: 7461 7475 7320 3a3a 2035 202d 2050 726f  tatus :: 5 - Pro
-000001e0: 6475 6374 696f 6e2f 5374 6162 6c65 0d0a  duction/Stable..
-000001f0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a69 6e63  ..[options]..inc
-00000200: 6c75 6465 5f70 6163 6b61 6765 5f64 6174  lude_package_dat
-00000210: 6120 3d20 5472 7565 0d0a 7061 636b 6167  a = True..packag
-00000220: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
-00000230: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-00000240: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-00000250: 7265 7320 3d20 3e3d 332e 360d 0a69 6e73  res = >=3.6..ins
-00000260: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000270: 0d0a 0d0a 5b6f 7074 696f 6e73 2e70 6163  ....[options.pac
-00000280: 6b61 6765 732e 6669 6e64 5d0d 0a77 6865  kages.find]..whe
-00000290: 7265 203d 2073 7263 0d0a 0d0a 5b65 6767  re = src....[egg
-000002a0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000002b0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-000002c0: 2030 0d0a 0d0a                            0....
+00000020: 696f 6e20 3d20 312e 302e 310d 0a61 7574  ion = 1.0.1..aut
+00000030: 686f 7220 3d20 5369 6d6f 6e20 5a6f 7a6f  hor = Simon Zozo
+00000040: 6c0d 0a61 7574 686f 725f 656d 6169 6c20  l..author_email 
+00000050: 3d20 7369 6d6f 6e2e 7a6f 7a6f 6c40 676d  = simon.zozol@gm
+00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
+00000070: 7469 6f6e 203d 200d 0a6c 6f6e 675f 6465  tion = ..long_de
+00000080: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+00000090: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+000000a0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000b0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+000000c0: 742f 6d61 726b 646f 776e 0d0a 6874 7470  t/markdown..http
+000000d0: 7320 3d20 2f2f 6269 7462 7563 6b65 742e  s = //bitbucket.
+000000e0: 6f72 672f 686f 6c79 7079 7468 6f6e 2f7a  org/holypython/z
+000000f0: 7a63 6872 6f6e 6f2f 7372 632f 6d61 7374  zchrono/src/mast
+00000100: 6572 2f0d 0a63 6c61 7373 6966 6965 7273  er/..classifiers
+00000110: 203d 200d 0a09 546f 7069 6320 3a3a 2053   = ...Topic :: S
+00000120: 6f66 7477 6172 6520 4465 7665 6c6f 706d  oftware Developm
+00000130: 656e 740d 0a09 5072 6f67 7261 6d6d 696e  ent...Programmin
+00000140: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000150: 7468 6f6e 203a 3a20 332e 360d 0a09 4c69  thon :: 3.6...Li
+00000160: 6365 6e73 6520 3a3a 2043 4330 2031 2e30  cense :: CC0 1.0
+00000170: 2055 6e69 7665 7273 616c 2028 4343 3020   Universal (CC0 
+00000180: 312e 3029 2050 7562 6c69 6320 446f 6d61  1.0) Public Doma
+00000190: 696e 2044 6564 6963 6174 696f 6e0d 0a09  in Dedication...
+000001a0: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+000001b0: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+000001c0: 6e74 0d0a 0944 6576 656c 6f70 6d65 6e74  nt...Development
+000001d0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
+000001e0: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
+000001f0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
+00000200: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
+00000210: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
+00000220: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
+00000230: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
+00000240: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
+00000250: 7569 7265 7320 3d20 3e3d 332e 360d 0a69  uires = >=3.6..i
+00000260: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
+00000270: 3d20 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  = ....[options.p
+00000280: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+00000290: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+000002a0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002b0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002c0: 203d 2030 0d0a 0d0a                       = 0....
```

