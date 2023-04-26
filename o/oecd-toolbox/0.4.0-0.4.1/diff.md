# Comparing `tmp/oecd_toolbox-0.4.0.tar.gz` & `tmp/oecd_toolbox-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oecd_toolbox-0.4.0.tar", last modified: Mon Apr 17 20:38:20 2023, max compression
+gzip compressed data, was "oecd_toolbox-0.4.1.tar", last modified: Wed Apr 26 09:41:32 2023, max compression
```

## Comparing `oecd_toolbox-0.4.0.tar` & `oecd_toolbox-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.148713 oecd_toolbox-0.4.0/
--rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     5783 2023-04-17 20:38:20.148713 oecd_toolbox-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     5176 2023-04-17 20:28:40.000000 oecd_toolbox-0.4.0/README.md
--rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      856 2023-04-17 20:38:20.158070 oecd_toolbox-0.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.008434 oecd_toolbox-0.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.096961 oecd_toolbox-0.4.0/src/oecd_toolbox/
--rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/__init__.py
--rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/converters.py
--rw-rw-rw-   0        0        0    13022 2023-04-17 20:35:35.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/csv_writers.py
--rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.4.0/src/oecd_toolbox/downloaders.py
-drwxrwxrwx   0        0        0        0 2023-04-17 20:38:20.142523 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/
--rw-rw-rw-   0        0        0     5783 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 20:38:19.000000 oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.399867 oecd_toolbox-0.4.1/
+-rw-rw-rw-   0        0        0     1131 2021-12-03 19:53:43.000000 oecd_toolbox-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0     5795 2023-04-26 09:41:32.399867 oecd_toolbox-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5176 2023-04-26 09:39:10.000000 oecd_toolbox-0.4.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      868 2023-04-26 09:41:32.407350 oecd_toolbox-0.4.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.239796 oecd_toolbox-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.352439 oecd_toolbox-0.4.1/src/oecd_toolbox/
+-rw-rw-rw-   0        0        0        0 2021-12-03 19:53:44.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/__init__.py
+-rw-rw-rw-   0        0        0     7046 2022-12-01 16:43:33.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/converters.py
+-rw-rw-rw-   0        0        0    13022 2023-04-26 09:39:10.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/csv_writers.py
+-rw-rw-rw-   0        0        0     5112 2022-02-04 15:48:18.000000 oecd_toolbox-0.4.1/src/oecd_toolbox/downloaders.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:41:32.393998 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     5795 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-26 09:41:32.000000 oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/top_level.txt
```

### Comparing `oecd_toolbox-0.4.0/LICENSE` & `oecd_toolbox-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.0/PKG-INFO` & `oecd_toolbox-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: oecd_toolbox
-Version: 0.4.0
+Version: 0.4.1
 Summary: OECD fetcher building templates and helpers
 Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
-Author: Gyorgy Gyomai, Isaac Afambo
+Author: Gyorgy Gyomai, Isaac Afambo, Alena Brin
 Author-email: gyorgy.gyomai@oecd.org
 Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OECD Toolbox
 A library of abstract classes that can serve as a skeleton for writing downloaders and converters for DbNomics style fetchers.
 Additionally it contains utility/helper functions to handle common operations or transformations in both the downloading and conversion process.
```

### Comparing `oecd_toolbox-0.4.0/README.md` & `oecd_toolbox-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.0/setup.cfg` & `oecd_toolbox-0.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206f 6563 645f 746f 6f6c 626f 780d   = oecd_toolbox.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e30  .version = 0.4.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 2e31  .version = 0.4.1
 00000030: 0d0a 6175 7468 6f72 203d 2047 796f 7267  ..author = Gyorg
 00000040: 7920 4779 6f6d 6169 2c20 4973 6161 6320  y Gyomai, Isaac 
-00000050: 4166 616d 626f 0d0a 6175 7468 6f72 5f65  Afambo..author_e
-00000060: 6d61 696c 203d 2067 796f 7267 792e 6779  mail = gyorgy.gy
-00000070: 6f6d 6169 406f 6563 642e 6f72 670d 0a64  omai@oecd.org..d
-00000080: 6573 6372 6970 7469 6f6e 203d 204f 4543  escription = OEC
-00000090: 4420 6665 7463 6865 7220 6275 696c 6469  D fetcher buildi
-000000a0: 6e67 2074 656d 706c 6174 6573 2061 6e64  ng templates and
-000000b0: 2068 656c 7065 7273 0d0a 6c6f 6e67 5f64   helpers..long_d
-000000c0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000d0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000100: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000110: 203d 2068 7474 7073 3a2f 2f67 6974 6c61   = https://gitla
-00000120: 622e 616c 676f 6261 6e6b 2e6f 6563 642e  b.algobank.oecd.
-00000130: 6f72 672f 6f65 6364 2d64 6174 612d 6665  org/oecd-data-fe
-00000140: 7463 6865 7273 312f 4f45 4344 2d54 4f4f  tchers1/OECD-TOO
-00000150: 4c42 4f58 0d0a 7072 6f6a 6563 745f 7572  LBOX..project_ur
-00000160: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-00000170: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-00000180: 746c 6162 2e61 6c67 6f62 616e 6b2e 6f65  tlab.algobank.oe
-00000190: 6364 2e6f 7267 2f6f 6563 642d 6461 7461  cd.org/oecd-data
-000001a0: 2d66 6574 6368 6572 7331 2f4f 4543 442d  -fetchers1/OECD-
-000001b0: 544f 4f4c 424f 582f 2d2f 6973 7375 6573  TOOLBOX/-/issues
-000001c0: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-000001d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000001e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001f0: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-00000200: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000210: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-00000220: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000230: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000240: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000250: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-00000260: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000270: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000280: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000290: 3d33 2e37 0d0a 696e 7374 616c 6c5f 7265  =3.7..install_re
-000002a0: 7175 6972 6573 203d 200d 0a09 6462 6e6f  quires = ...dbno
-000002b0: 6d69 6373 2d66 6574 6368 6572 2d74 6f6f  mics-fetcher-too
-000002c0: 6c62 6f78 3d3d 302e 302e 390d 0a09 6462  lbox==0.0.9...db
-000002d0: 6e6f 6d69 6373 2d64 6174 612d 6d6f 6465  nomics-data-mode
-000002e0: 6c3d 3d30 2e31 332e 3230 0d0a 0970 7974  l==0.13.20...pyt
-000002f0: 686f 6e2d 736c 7567 6966 793e 3d35 2e30  hon-slugify>=5.0
-00000300: 2e32 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .2....[options.p
-00000310: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000320: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-00000330: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000340: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000350: 203d 2030 0d0a 0d0a                       = 0....
+00000050: 4166 616d 626f 2c20 416c 656e 6120 4272  Afambo, Alena Br
+00000060: 696e 0d0a 6175 7468 6f72 5f65 6d61 696c  in..author_email
+00000070: 203d 2067 796f 7267 792e 6779 6f6d 6169   = gyorgy.gyomai
+00000080: 406f 6563 642e 6f72 670d 0a64 6573 6372  @oecd.org..descr
+00000090: 6970 7469 6f6e 203d 204f 4543 4420 6665  iption = OECD fe
+000000a0: 7463 6865 7220 6275 696c 6469 6e67 2074  tcher building t
+000000b0: 656d 706c 6174 6573 2061 6e64 2068 656c  emplates and hel
+000000c0: 7065 7273 0d0a 6c6f 6e67 5f64 6573 6372  pers..long_descr
+000000d0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+000000e0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+000000f0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000100: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000110: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000120: 7474 7073 3a2f 2f67 6974 6c61 622e 616c  ttps://gitlab.al
+00000130: 676f 6261 6e6b 2e6f 6563 642e 6f72 672f  gobank.oecd.org/
+00000140: 6f65 6364 2d64 6174 612d 6665 7463 6865  oecd-data-fetche
+00000150: 7273 312f 4f45 4344 2d54 4f4f 4c42 4f58  rs1/OECD-TOOLBOX
+00000160: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000170: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+00000180: 3d20 6874 7470 733a 2f2f 6769 746c 6162  = https://gitlab
+00000190: 2e61 6c67 6f62 616e 6b2e 6f65 6364 2e6f  .algobank.oecd.o
+000001a0: 7267 2f6f 6563 642d 6461 7461 2d66 6574  rg/oecd-data-fet
+000001b0: 6368 6572 7331 2f4f 4543 442d 544f 4f4c  chers1/OECD-TOOL
+000001c0: 424f 582f 2d2f 6973 7375 6573 0d0a 636c  BOX/-/issues..cl
+000001d0: 6173 7369 6669 6572 7320 3d20 0d0a 0950  assifiers = ...P
+000001e0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001f0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000200: 2033 0d0a 094c 6963 656e 7365 203a 3a20   3...License :: 
+00000210: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000220: 4d49 5420 4c69 6365 6e73 650d 0a09 4f70  MIT License...Op
+00000230: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000240: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
+00000250: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a70  ....[options]..p
+00000260: 6163 6b61 6765 5f64 6972 203d 200d 0a09  ackage_dir = ...
+00000270: 3d20 7372 630d 0a70 6163 6b61 6765 7320  = src..packages 
+00000280: 3d20 6669 6e64 3a0d 0a70 7974 686f 6e5f  = find:..python_
+00000290: 7265 7175 6972 6573 203d 203e 3d33 2e39  requires = >=3.9
+000002a0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000002b0: 6573 203d 200d 0a09 6462 6e6f 6d69 6373  es = ...dbnomics
+000002c0: 2d66 6574 6368 6572 2d74 6f6f 6c62 6f78  -fetcher-toolbox
+000002d0: 3d3d 302e 302e 390d 0a09 6462 6e6f 6d69  ==0.0.9...dbnomi
+000002e0: 6373 2d64 6174 612d 6d6f 6465 6c3d 3d30  cs-data-model==0
+000002f0: 2e31 332e 3230 0d0a 0970 7974 686f 6e2d  .13.20...python-
+00000300: 736c 7567 6966 793e 3d35 2e30 2e32 0d0a  slugify>=5.0.2..
+00000310: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
+00000320: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
+00000330: 203d 2073 7263 0d0a 0d0a 5b65 6767 5f69   = src....[egg_i
+00000340: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000350: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000360: 0d0a 0d0a                                ....
```

### Comparing `oecd_toolbox-0.4.0/src/oecd_toolbox/converters.py` & `oecd_toolbox-0.4.1/src/oecd_toolbox/converters.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.0/src/oecd_toolbox/csv_writers.py` & `oecd_toolbox-0.4.1/src/oecd_toolbox/csv_writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                     df = pd.DataFrame(data=series["observations"][1:],columns=series["observations"][0]) 
                     # this only aggregates values, but omits observation attributes that might be in the original file                   
                     df_new_freq = df.groupby(pd.PeriodIndex(df['PERIOD'], freq=target_freq.to_dimension_code()))['VALUE'].apply(f_aggregation)
                     for ind in df_new_freq.index:
                         dim_dict=dict()
                         dim_dict['code'] = series['code']
                         dim_dict['year'], dim_dict['freq'], dim_dict['period'] = get_DC_compatible_date_pandas(ind)
-                        dim_dict['value'] = df_new_freq[ind]
+                        dim_dict['VALUE'] = df_new_freq[ind]
 
                         L.append(dim_dict)
                     
         return L 
     
     series_jsonl_to_csv_base(source_file=source_file, target_file=target_file, obslist_fn=create_DCobservations_list)
```

### Comparing `oecd_toolbox-0.4.0/src/oecd_toolbox/downloaders.py` & `oecd_toolbox-0.4.1/src/oecd_toolbox/downloaders.py`

 * *Files identical despite different names*

### Comparing `oecd_toolbox-0.4.0/src/oecd_toolbox.egg-info/PKG-INFO` & `oecd_toolbox-0.4.1/src/oecd_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: oecd-toolbox
-Version: 0.4.0
+Version: 0.4.1
 Summary: OECD fetcher building templates and helpers
 Home-page: https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX
-Author: Gyorgy Gyomai, Isaac Afambo
+Author: Gyorgy Gyomai, Isaac Afambo, Alena Brin
 Author-email: gyorgy.gyomai@oecd.org
 Project-URL: Bug Tracker, https://gitlab.algobank.oecd.org/oecd-data-fetchers1/OECD-TOOLBOX/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # OECD Toolbox
 A library of abstract classes that can serve as a skeleton for writing downloaders and converters for DbNomics style fetchers.
 Additionally it contains utility/helper functions to handle common operations or transformations in both the downloading and conversion process.
```

