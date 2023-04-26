# Comparing `tmp/pgradd-2.9.8.tar.gz` & `tmp/pgradd-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgradd-2.9.8.tar", last modified: Wed Apr  5 15:12:55 2023, max compression
+gzip compressed data, was "pgradd-2.9.9.tar", last modified: Wed Apr 26 18:43:47 2023, max compression
```

## Comparing `pgradd-2.9.8.tar` & `pgradd-2.9.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.094118 pgradd-2.9.8/
--rw-rw-rw-   0        0        0     1086 2019-05-15 16:40:29.000000 pgradd-2.9.8/LICENSE.md
--rw-rw-rw-   0        0        0       52 2019-11-22 20:35:06.000000 pgradd-2.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0    13149 2023-04-05 15:12:55.088133 pgradd-2.9.8/PKG-INFO
--rw-rw-rw-   0        0        0    12509 2023-01-26 19:19:10.000000 pgradd-2.9.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.827256 pgradd-2.9.8/pgradd/
--rw-rw-rw-   0        0        0      519 2021-11-29 14:56:42.000000 pgradd-2.9.8/pgradd/Consts.py
--rw-rw-rw-   0        0        0     2297 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/DrawMol.py
--rw-rw-rw-   0        0        0     6387 2018-12-16 22:53:40.000000 pgradd-2.9.8/pgradd/Error.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.867331 pgradd-2.9.8/pgradd/GroupAdd/
--rw-rw-rw-   0        0        0     2039 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/GroupAdd/DataDir.py
--rw-rw-rw-   0        0        0     5160 2019-04-09 14:39:28.000000 pgradd-2.9.8/pgradd/GroupAdd/Group.py
--rw-rw-rw-   0        0        0    13213 2023-01-27 19:30:44.000000 pgradd-2.9.8/pgradd/GroupAdd/Library.py
--rw-rw-rw-   0        0        0    18728 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/GroupAdd/Scheme.py
--rw-rw-rw-   0        0        0      743 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/GroupAdd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.883833 pgradd-2.9.8/pgradd/RDkitWrapper/
--rw-rw-rw-   0        0        0     8438 2018-12-29 14:46:24.000000 pgradd-2.9.8/pgradd/RDkitWrapper/GenRxnNet.py
--rw-rw-rw-   0        0        0    25339 2022-09-16 16:59:30.000000 pgradd-2.9.8/pgradd/RDkitWrapper/MolQuery.py
--rw-rw-rw-   0        0        0    14848 2018-12-20 14:47:28.000000 pgradd-2.9.8/pgradd/RDkitWrapper/ReactionQuery.py
--rw-rw-rw-   0        0        0       59 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/RDkitWrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.904667 pgradd-2.9.8/pgradd/RINGParser/
--rw-rw-rw-   0        0        0    12200 2018-12-20 16:44:48.000000 pgradd-2.9.8/pgradd/RINGParser/Grammar.py
--rw-rw-rw-   0        0        0    21120 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/RINGParser/MolQueryRead.py
--rw-rw-rw-   0        0        0    13964 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/RINGParser/Parser.py
--rw-rw-rw-   0        0        0    21697 2019-06-13 14:25:03.000000 pgradd-2.9.8/pgradd/RINGParser/ReactionQueryRead.py
--rw-rw-rw-   0        0        0     2566 2019-11-22 20:45:45.000000 pgradd-2.9.8/pgradd/RINGParser/Reader.py
--rw-rw-rw-   0        0        0      818 2018-12-20 16:45:37.000000 pgradd-2.9.8/pgradd/RINGParser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.920931 pgradd-2.9.8/pgradd/ThermoChem/
--rw-rw-rw-   0        0        0     1197 2018-12-20 17:15:10.000000 pgradd-2.9.8/pgradd/ThermoChem/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-01-18 18:54:39.000000 pgradd-2.9.8/pgradd/ThermoChem/base.py
--rw-rw-rw-   0        0        0     4383 2023-01-18 23:26:46.000000 pgradd-2.9.8/pgradd/ThermoChem/group_data.py
--rw-rw-rw-   0        0        0    16924 2021-11-29 15:38:04.000000 pgradd-2.9.8/pgradd/ThermoChem/incomplete.py
--rw-rw-rw-   0        0        0     9043 2019-11-22 20:45:45.000000 pgradd-2.9.8/pgradd/ThermoChem/raw_data.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.943385 pgradd-2.9.8/pgradd/Units/
--rw-rw-rw-   0        0        0     1706 2018-12-29 16:19:22.000000 pgradd-2.9.8/pgradd/Units/__init__.py
--rw-rw-rw-   0        0        0     1625 2018-12-21 14:25:11.000000 pgradd-2.9.8/pgradd/Units/builtin.py
--rw-rw-rw-   0        0        0     1251 2018-12-20 17:25:27.000000 pgradd-2.9.8/pgradd/Units/db.py
--rw-rw-rw-   0        0        0     3496 2018-12-20 17:24:51.000000 pgradd-2.9.8/pgradd/Units/helpers.py
--rw-rw-rw-   0        0        0     7091 2018-12-20 17:19:02.000000 pgradd-2.9.8/pgradd/Units/parser.py
--rw-rw-rw-   0        0        0    20179 2018-12-21 15:17:45.000000 pgradd-2.9.8/pgradd/Units/qty.py
--rw-rw-rw-   0        0        0      198 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/Units/utils.py
--rw-rw-rw-   0        0        0      243 2023-04-05 15:12:11.000000 pgradd-2.9.8/pgradd/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.793423 pgradd-2.9.8/pgradd/data/
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.952190 pgradd-2.9.8/pgradd/data/BensonGA/
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.979586 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/
--rw-rw-rw-   0        0        0     1978 2020-01-15 20:34:34.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/corrections.yaml
--rw-rw-rw-   0        0        0      517 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/extra.yaml
--rw-rw-rw-   0        0        0    11010 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/hydrocarbons.yaml
--rw-rw-rw-   0        0        0    10942 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/hydrocarbons_original.yaml
--rw-rw-rw-   0        0        0      473 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/index.yaml
--rw-rw-rw-   0        0        0    11851 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/nitrogenates.yaml
--rw-rw-rw-   0        0        0      135 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/original.yaml
--rw-rw-rw-   0        0        0    12563 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/oxygenates.yaml
--rw-rw-rw-   0        0        0     2511 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/radicals.yaml
--rw-rw-rw-   0        0        0     7885 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/strain.yaml
--rw-rw-rw-   0        0        0       73 2021-11-29 15:41:26.000000 pgradd-2.9.8/pgradd/data/BensonGA/library.yaml
--rw-rw-rw-   0        0        0    41354 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/BensonGA/scheme.yaml
--rw-rw-rw-   0        0        0    48379 2021-11-29 15:41:50.000000 pgradd-2.9.8/pgradd/data/BensonGA/surface_benson.lib.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.991554 pgradd-2.9.8/pgradd/data/GRWAqueous2018/
--rw-rw-rw-   0        0        0       45 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GRWAqueous2018/library.yaml
--rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GRWAqueous2018/scheme.yaml
--rw-rw-rw-   0        0        0    60197 2018-12-17 14:17:49.000000 pgradd-2.9.8/pgradd/data/GRWAqueous2018/surface.yaml
--rw-rw-rw-   0        0        0    30434 2018-12-17 14:27:11.000000 pgradd-2.9.8/pgradd/data/GRWAqueous2018/uq.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.006747 pgradd-2.9.8/pgradd/data/GRWSurface2018/
--rw-rw-rw-   0        0        0       45 2021-07-06 19:33:14.000000 pgradd-2.9.8/pgradd/data/GRWSurface2018/library.yaml
--rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GRWSurface2018/scheme.yaml
--rw-rw-rw-   0        0        0    60197 2018-12-17 20:31:02.000000 pgradd-2.9.8/pgradd/data/GRWSurface2018/surface.yaml
--rw-rw-rw-   0        0        0    30434 2019-05-15 16:40:29.000000 pgradd-2.9.8/pgradd/data/GRWSurface2018/uq.yaml
--rw-rw-rw-   0        0        0     1369 2020-05-02 12:56:26.000000 pgradd-2.9.8/pgradd/data/GRWSurface2018/uq_crossvalidation.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.018577 pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/
--rw-rw-rw-   0        0        0       34 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/library.yaml
--rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/scheme.yaml
--rw-rw-rw-   0        0        0    66712 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/surface.yaml
--rw-rw-rw-   0        0        0    36088 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/uq.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.031542 pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/
--rw-rw-rw-   0        0        0       45 2019-05-15 17:23:54.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/library.yaml
--rw-rw-rw-   0        0        0    24957 2019-05-15 17:23:54.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/scheme.yaml
--rw-rw-rw-   0        0        0    66429 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/surface.yaml
--rw-rw-rw-   0        0        0    36092 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/uq.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.045506 pgradd-2.9.8/pgradd/data/SalciccioliGA2012/
--rw-rw-rw-   0        0        0       34 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/SalciccioliGA2012/library.yaml
--rw-rw-rw-   0        0        0    21737 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/SalciccioliGA2012/scheme.yaml
--rw-rw-rw-   0        0        0    34680 2020-08-27 13:45:27.000000 pgradd-2.9.8/pgradd/data/SalciccioliGA2012/surface.yaml
--rw-rw-rw-   0        0        0    47868 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/data/SalciccioliGA2012/surface_benson.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.055481 pgradd-2.9.8/pgradd/data/XieGA2022/
--rw-rw-rw-   0        0        0       34 2022-01-31 15:26:40.000000 pgradd-2.9.8/pgradd/data/XieGA2022/library.yaml
--rw-rw-rw-   0        0        0    26708 2022-01-31 15:26:40.000000 pgradd-2.9.8/pgradd/data/XieGA2022/scheme.yaml
--rw-rw-rw-   0        0        0    21191 2022-01-31 18:31:38.000000 pgradd-2.9.8/pgradd/data/XieGA2022/surface.yaml
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.063459 pgradd-2.9.8/pgradd/tests/
--rw-rw-rw-   0        0        0        0 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/tests/__init__.py
--rw-rw-rw-   0        0        0    13303 2020-05-21 15:47:24.000000 pgradd-2.9.8/pgradd/tests/test_RINGparser_RDkitwrapper_test.py
--rw-rw-rw-   0        0        0     5693 2023-01-26 18:08:41.000000 pgradd-2.9.8/pgradd/tests/test_SMILES_to_thermo_examples.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:55.083146 pgradd-2.9.8/pgradd/yaml_io/
--rw-rw-rw-   0        0        0      554 2018-10-31 00:55:43.000000 pgradd-2.9.8/pgradd/yaml_io/__init__.py
--rw-rw-rw-   0        0        0     7267 2023-01-27 19:42:10.000000 pgradd-2.9.8/pgradd/yaml_io/builtins.py
--rw-rw-rw-   0        0        0      359 2018-12-21 20:52:50.000000 pgradd-2.9.8/pgradd/yaml_io/common.py
--rw-rw-rw-   0        0        0     2892 2018-12-29 16:25:56.000000 pgradd-2.9.8/pgradd/yaml_io/lib_interface.py
--rw-rw-rw-   0        0        0    16048 2023-01-27 19:31:32.000000 pgradd-2.9.8/pgradd/yaml_io/schema.py
--rw-rw-rw-   0        0        0     1662 2018-12-21 20:51:22.000000 pgradd-2.9.8/pgradd/yaml_io/yaml_io.py
-drwxrwxrwx   0        0        0        0 2023-04-05 15:12:54.848475 pgradd-2.9.8/pgradd.egg-info/
--rw-rw-rw-   0        0        0    13149 2023-04-05 15:12:54.000000 pgradd-2.9.8/pgradd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2898 2023-04-05 15:12:54.000000 pgradd-2.9.8/pgradd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       36 2023-04-05 15:12:54.000000 pgradd-2.9.8/pgradd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-05 15:12:54.000000 pgradd-2.9.8/pgradd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-05 15:12:54.000000 pgradd-2.9.8/pgradd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-06-13 14:53:35.000000 pgradd-2.9.8/pgradd.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-05 15:12:55.095115 pgradd-2.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1513 2023-04-05 15:12:11.000000 pgradd-2.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.735343 pgradd-2.9.9/
+-rw-rw-rw-   0        0        0     1086 2019-05-15 16:40:29.000000 pgradd-2.9.9/LICENSE.md
+-rw-rw-rw-   0        0        0       52 2019-11-22 20:35:06.000000 pgradd-2.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    13170 2023-04-26 18:43:47.728993 pgradd-2.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0    12530 2023-04-26 18:42:12.000000 pgradd-2.9.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.309840 pgradd-2.9.9/pgradd/
+-rw-rw-rw-   0        0        0      519 2021-11-29 14:56:42.000000 pgradd-2.9.9/pgradd/Consts.py
+-rw-rw-rw-   0        0        0     2297 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/DrawMol.py
+-rw-rw-rw-   0        0        0     6387 2018-12-16 22:53:40.000000 pgradd-2.9.9/pgradd/Error.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.362925 pgradd-2.9.9/pgradd/GroupAdd/
+-rw-rw-rw-   0        0        0     2039 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/GroupAdd/DataDir.py
+-rw-rw-rw-   0        0        0     5160 2019-04-09 14:39:28.000000 pgradd-2.9.9/pgradd/GroupAdd/Group.py
+-rw-rw-rw-   0        0        0    13213 2023-01-27 19:30:44.000000 pgradd-2.9.9/pgradd/GroupAdd/Library.py
+-rw-rw-rw-   0        0        0    18728 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/GroupAdd/Scheme.py
+-rw-rw-rw-   0        0        0      743 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/GroupAdd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.389622 pgradd-2.9.9/pgradd/RDkitWrapper/
+-rw-rw-rw-   0        0        0     8438 2018-12-29 14:46:24.000000 pgradd-2.9.9/pgradd/RDkitWrapper/GenRxnNet.py
+-rw-rw-rw-   0        0        0    25339 2022-09-16 16:59:30.000000 pgradd-2.9.9/pgradd/RDkitWrapper/MolQuery.py
+-rw-rw-rw-   0        0        0    14848 2018-12-20 14:47:28.000000 pgradd-2.9.9/pgradd/RDkitWrapper/ReactionQuery.py
+-rw-rw-rw-   0        0        0       59 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/RDkitWrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.427684 pgradd-2.9.9/pgradd/RINGParser/
+-rw-rw-rw-   0        0        0    12200 2018-12-20 16:44:48.000000 pgradd-2.9.9/pgradd/RINGParser/Grammar.py
+-rw-rw-rw-   0        0        0    21120 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/RINGParser/MolQueryRead.py
+-rw-rw-rw-   0        0        0    13964 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/RINGParser/Parser.py
+-rw-rw-rw-   0        0        0    21697 2019-06-13 14:25:03.000000 pgradd-2.9.9/pgradd/RINGParser/ReactionQueryRead.py
+-rw-rw-rw-   0        0        0     2566 2019-11-22 20:45:45.000000 pgradd-2.9.9/pgradd/RINGParser/Reader.py
+-rw-rw-rw-   0        0        0      818 2018-12-20 16:45:37.000000 pgradd-2.9.9/pgradd/RINGParser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.455541 pgradd-2.9.9/pgradd/ThermoChem/
+-rw-rw-rw-   0        0        0     1197 2018-12-20 17:15:10.000000 pgradd-2.9.9/pgradd/ThermoChem/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-01-18 18:54:39.000000 pgradd-2.9.9/pgradd/ThermoChem/base.py
+-rw-rw-rw-   0        0        0     4383 2023-01-18 23:26:46.000000 pgradd-2.9.9/pgradd/ThermoChem/group_data.py
+-rw-rw-rw-   0        0        0    16941 2023-04-06 14:33:23.000000 pgradd-2.9.9/pgradd/ThermoChem/incomplete.py
+-rw-rw-rw-   0        0        0     9043 2019-11-22 20:45:45.000000 pgradd-2.9.9/pgradd/ThermoChem/raw_data.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.492711 pgradd-2.9.9/pgradd/Units/
+-rw-rw-rw-   0        0        0     1706 2018-12-29 16:19:22.000000 pgradd-2.9.9/pgradd/Units/__init__.py
+-rw-rw-rw-   0        0        0     1625 2018-12-21 14:25:11.000000 pgradd-2.9.9/pgradd/Units/builtin.py
+-rw-rw-rw-   0        0        0     1251 2018-12-20 17:25:27.000000 pgradd-2.9.9/pgradd/Units/db.py
+-rw-rw-rw-   0        0        0     3496 2018-12-20 17:24:51.000000 pgradd-2.9.9/pgradd/Units/helpers.py
+-rw-rw-rw-   0        0        0     7091 2018-12-20 17:19:02.000000 pgradd-2.9.9/pgradd/Units/parser.py
+-rw-rw-rw-   0        0        0    20179 2018-12-21 15:17:45.000000 pgradd-2.9.9/pgradd/Units/qty.py
+-rw-rw-rw-   0        0        0      198 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/Units/utils.py
+-rw-rw-rw-   0        0        0      243 2023-04-26 18:42:12.000000 pgradd-2.9.9/pgradd/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.262256 pgradd-2.9.9/pgradd/data/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.506565 pgradd-2.9.9/pgradd/data/BensonGA/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.556077 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/
+-rw-rw-rw-   0        0        0     1978 2020-01-15 20:34:34.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/corrections.yaml
+-rw-rw-rw-   0        0        0      517 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/extra.yaml
+-rw-rw-rw-   0        0        0    11010 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/hydrocarbons.yaml
+-rw-rw-rw-   0        0        0    10942 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/hydrocarbons_original.yaml
+-rw-rw-rw-   0        0        0      473 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/index.yaml
+-rw-rw-rw-   0        0        0    11851 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/nitrogenates.yaml
+-rw-rw-rw-   0        0        0      135 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/original.yaml
+-rw-rw-rw-   0        0        0    12563 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/oxygenates.yaml
+-rw-rw-rw-   0        0        0     2511 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/radicals.yaml
+-rw-rw-rw-   0        0        0     7885 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/strain.yaml
+-rw-rw-rw-   0        0        0       73 2021-11-29 15:41:26.000000 pgradd-2.9.9/pgradd/data/BensonGA/library.yaml
+-rw-rw-rw-   0        0        0    41354 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/BensonGA/scheme.yaml
+-rw-rw-rw-   0        0        0    48379 2021-11-29 15:41:50.000000 pgradd-2.9.9/pgradd/data/BensonGA/surface_benson.lib.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.576203 pgradd-2.9.9/pgradd/data/GRWAqueous2018/
+-rw-rw-rw-   0        0        0       45 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GRWAqueous2018/library.yaml
+-rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GRWAqueous2018/scheme.yaml
+-rw-rw-rw-   0        0        0    60197 2018-12-17 14:17:49.000000 pgradd-2.9.9/pgradd/data/GRWAqueous2018/surface.yaml
+-rw-rw-rw-   0        0        0    30434 2018-12-17 14:27:11.000000 pgradd-2.9.9/pgradd/data/GRWAqueous2018/uq.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.601187 pgradd-2.9.9/pgradd/data/GRWSurface2018/
+-rw-rw-rw-   0        0        0       45 2021-07-06 19:33:14.000000 pgradd-2.9.9/pgradd/data/GRWSurface2018/library.yaml
+-rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GRWSurface2018/scheme.yaml
+-rw-rw-rw-   0        0        0    60197 2018-12-17 20:31:02.000000 pgradd-2.9.9/pgradd/data/GRWSurface2018/surface.yaml
+-rw-rw-rw-   0        0        0    30434 2019-05-15 16:40:29.000000 pgradd-2.9.9/pgradd/data/GRWSurface2018/uq.yaml
+-rw-rw-rw-   0        0        0     1369 2020-05-02 12:56:26.000000 pgradd-2.9.9/pgradd/data/GRWSurface2018/uq_crossvalidation.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.621595 pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/
+-rw-rw-rw-   0        0        0       34 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/library.yaml
+-rw-rw-rw-   0        0        0    24957 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/scheme.yaml
+-rw-rw-rw-   0        0        0    66712 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/surface.yaml
+-rw-rw-rw-   0        0        0    36088 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/uq.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.642194 pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/
+-rw-rw-rw-   0        0        0       45 2019-05-15 17:23:54.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/library.yaml
+-rw-rw-rw-   0        0        0    24957 2019-05-15 17:23:54.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/scheme.yaml
+-rw-rw-rw-   0        0        0    66429 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/surface.yaml
+-rw-rw-rw-   0        0        0    36092 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/uq.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.667096 pgradd-2.9.9/pgradd/data/SalciccioliGA2012/
+-rw-rw-rw-   0        0        0       34 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/SalciccioliGA2012/library.yaml
+-rw-rw-rw-   0        0        0    21737 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/SalciccioliGA2012/scheme.yaml
+-rw-rw-rw-   0        0        0    34680 2020-08-27 13:45:27.000000 pgradd-2.9.9/pgradd/data/SalciccioliGA2012/surface.yaml
+-rw-rw-rw-   0        0        0    47868 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/data/SalciccioliGA2012/surface_benson.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.681777 pgradd-2.9.9/pgradd/data/XieGA2022/
+-rw-rw-rw-   0        0        0       34 2022-01-31 15:26:40.000000 pgradd-2.9.9/pgradd/data/XieGA2022/library.yaml
+-rw-rw-rw-   0        0        0    26708 2022-01-31 15:26:40.000000 pgradd-2.9.9/pgradd/data/XieGA2022/scheme.yaml
+-rw-rw-rw-   0        0        0    21191 2022-01-31 18:31:38.000000 pgradd-2.9.9/pgradd/data/XieGA2022/surface.yaml
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.694734 pgradd-2.9.9/pgradd/tests/
+-rw-rw-rw-   0        0        0        0 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/tests/__init__.py
+-rw-rw-rw-   0        0        0    13303 2020-05-21 15:47:24.000000 pgradd-2.9.9/pgradd/tests/test_RINGparser_RDkitwrapper_test.py
+-rw-rw-rw-   0        0        0     5693 2023-01-26 18:08:41.000000 pgradd-2.9.9/pgradd/tests/test_SMILES_to_thermo_examples.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.725641 pgradd-2.9.9/pgradd/yaml_io/
+-rw-rw-rw-   0        0        0      554 2018-10-31 00:55:43.000000 pgradd-2.9.9/pgradd/yaml_io/__init__.py
+-rw-rw-rw-   0        0        0     7267 2023-01-27 19:42:10.000000 pgradd-2.9.9/pgradd/yaml_io/builtins.py
+-rw-rw-rw-   0        0        0      359 2018-12-21 20:52:50.000000 pgradd-2.9.9/pgradd/yaml_io/common.py
+-rw-rw-rw-   0        0        0     2892 2018-12-29 16:25:56.000000 pgradd-2.9.9/pgradd/yaml_io/lib_interface.py
+-rw-rw-rw-   0        0        0    16048 2023-01-27 19:31:32.000000 pgradd-2.9.9/pgradd/yaml_io/schema.py
+-rw-rw-rw-   0        0        0     1662 2018-12-21 20:51:22.000000 pgradd-2.9.9/pgradd/yaml_io/yaml_io.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:43:47.332730 pgradd-2.9.9/pgradd.egg-info/
+-rw-rw-rw-   0        0        0    13170 2023-04-26 18:43:47.000000 pgradd-2.9.9/pgradd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2898 2023-04-26 18:43:47.000000 pgradd-2.9.9/pgradd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       36 2023-04-26 18:43:47.000000 pgradd-2.9.9/pgradd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-26 18:43:47.000000 pgradd-2.9.9/pgradd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 18:43:47.000000 pgradd-2.9.9/pgradd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-06-13 14:53:35.000000 pgradd-2.9.9/pgradd.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-26 18:43:47.735343 pgradd-2.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1513 2023-04-26 18:42:12.000000 pgradd-2.9.9/setup.py
```

### Comparing `pgradd-2.9.8/LICENSE.md` & `pgradd-2.9.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/PKG-INFO` & `pgradd-2.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgradd
-Version: 2.9.8
+Version: 2.9.9
 Summary: Python package implements the Group Additivity (GA) method for estimating thermodynamic properties
 Home-page: https://github.com/VlachosGroup/PythonGroupAdditivity
 Author: Vlachos Research Group
 Author-email: vlachos@udel.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,17 +40,17 @@
 Citing this work
 ----------------
 G.R. Wittreich, D.G. Vlachos, Python Group Additivity (pGrAdd) software for estimating species thermochemical properties Comput. Phys. Commun. 273 (2022) 108277 https://doi.org/10.1016/j.cpc.2021.108277
 
 Developers
 ----------
 
--  Gerhard R Wittreich, P.E.
--  Geun Ho Gu
--  Michael Salciccioli
+-  Gerhard R Wittreich, Ph.D., P.E.
+-  Geun Ho Gu, Ph.D.
+-  Michael Salciccioli, Ph.D.
 -  Stephen M. Edie
 
 Required Packages
 -----------------
 
 -  Python2/Python3
 -  `pmutt`_ >= 1.3.2
```

### Comparing `pgradd-2.9.8/README.rst` & `pgradd-2.9.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 Citing this work
 ----------------
 G.R. Wittreich, D.G. Vlachos, Python Group Additivity (pGrAdd) software for estimating species thermochemical properties Comput. Phys. Commun. 273 (2022) 108277 https://doi.org/10.1016/j.cpc.2021.108277
 
 Developers
 ----------
 
--  Gerhard R Wittreich, P.E.
--  Geun Ho Gu
--  Michael Salciccioli
+-  Gerhard R Wittreich, Ph.D., P.E.
+-  Geun Ho Gu, Ph.D.
+-  Michael Salciccioli, Ph.D.
 -  Stephen M. Edie
 
 Required Packages
 -----------------
 
 -  Python2/Python3
 -  `pmutt`_ >= 1.3.2
```

### Comparing `pgradd-2.9.8/pgradd/Consts.py` & `pgradd-2.9.9/pgradd/Consts.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/DrawMol.py` & `pgradd-2.9.9/pgradd/DrawMol.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Error.py` & `pgradd-2.9.9/pgradd/Error.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/GroupAdd/DataDir.py` & `pgradd-2.9.9/pgradd/GroupAdd/DataDir.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/GroupAdd/Group.py` & `pgradd-2.9.9/pgradd/GroupAdd/Group.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/GroupAdd/Library.py` & `pgradd-2.9.9/pgradd/GroupAdd/Library.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/GroupAdd/Scheme.py` & `pgradd-2.9.9/pgradd/GroupAdd/Scheme.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/GroupAdd/__init__.py` & `pgradd-2.9.9/pgradd/GroupAdd/__init__.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RDkitWrapper/GenRxnNet.py` & `pgradd-2.9.9/pgradd/RDkitWrapper/GenRxnNet.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RDkitWrapper/MolQuery.py` & `pgradd-2.9.9/pgradd/RDkitWrapper/MolQuery.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RDkitWrapper/ReactionQuery.py` & `pgradd-2.9.9/pgradd/RDkitWrapper/ReactionQuery.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/Grammar.py` & `pgradd-2.9.9/pgradd/RINGParser/Grammar.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/MolQueryRead.py` & `pgradd-2.9.9/pgradd/RINGParser/MolQueryRead.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/Parser.py` & `pgradd-2.9.9/pgradd/RINGParser/Parser.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/ReactionQueryRead.py` & `pgradd-2.9.9/pgradd/RINGParser/ReactionQueryRead.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/Reader.py` & `pgradd-2.9.9/pgradd/RINGParser/Reader.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/RINGParser/__init__.py` & `pgradd-2.9.9/pgradd/RINGParser/__init__.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/ThermoChem/__init__.py` & `pgradd-2.9.9/pgradd/ThermoChem/__init__.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/ThermoChem/base.py` & `pgradd-2.9.9/pgradd/ThermoChem/base.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/ThermoChem/group_data.py` & `pgradd-2.9.9/pgradd/ThermoChem/group_data.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/ThermoChem/incomplete.py` & `pgradd-2.9.9/pgradd/ThermoChem/incomplete.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                 return self._correlation.get_HoRT(T)
             except OutsideCorrelationError:
                 raise IncompleteDataError(
                     "Cannot evaluate ND_H: no heat capacity data for T=%g"
                     % T)
     get_HoRT.__doc__ = ThermochemBase.get_HoRT.__doc__
 
-    def get_SoR(self, T):
+    def get_SoR(self, T, S_elements=None):
         if self.ND_S_ref is None:
             raise IncompleteDataError(
                 "Cannot evaluate ND_S: no entropy data is available")
         elif not self.ND_Cp_data:
             if T != self.T_ref:
                 warn(
                     "Evaluation of ND_S_ref with (T=%g <=> T_ref=%g) will not"
```

### Comparing `pgradd-2.9.8/pgradd/ThermoChem/raw_data.py` & `pgradd-2.9.9/pgradd/ThermoChem/raw_data.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/__init__.py` & `pgradd-2.9.9/pgradd/Units/__init__.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/builtin.py` & `pgradd-2.9.9/pgradd/Units/builtin.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/db.py` & `pgradd-2.9.9/pgradd/Units/db.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/helpers.py` & `pgradd-2.9.9/pgradd/Units/helpers.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/parser.py` & `pgradd-2.9.9/pgradd/Units/parser.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/Units/qty.py` & `pgradd-2.9.9/pgradd/Units/qty.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/corrections.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/corrections.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/extra.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/extra.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/hydrocarbons.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/hydrocarbons.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/hydrocarbons_original.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/hydrocarbons_original.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/nitrogenates.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/nitrogenates.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/oxygenates.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/oxygenates.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/radicals.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/radicals.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/gas_benson/strain.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/gas_benson/strain.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/scheme.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/BensonGA/surface_benson.lib.yaml` & `pgradd-2.9.9/pgradd/data/BensonGA/surface_benson.lib.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWAqueous2018/scheme.yaml` & `pgradd-2.9.9/pgradd/data/GRWAqueous2018/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWAqueous2018/surface.yaml` & `pgradd-2.9.9/pgradd/data/GRWAqueous2018/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWAqueous2018/uq.yaml` & `pgradd-2.9.9/pgradd/data/GRWAqueous2018/uq.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWSurface2018/scheme.yaml` & `pgradd-2.9.9/pgradd/data/GRWSurface2018/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWSurface2018/surface.yaml` & `pgradd-2.9.9/pgradd/data/GRWSurface2018/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWSurface2018/uq.yaml` & `pgradd-2.9.9/pgradd/data/GRWSurface2018/uq.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GRWSurface2018/uq_crossvalidation.txt` & `pgradd-2.9.9/pgradd/data/GRWSurface2018/uq_crossvalidation.txt`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/scheme.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/surface.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Aq/uq.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Aq/uq.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/scheme.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/surface.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/GuSolventGA2017Vac/uq.yaml` & `pgradd-2.9.9/pgradd/data/GuSolventGA2017Vac/uq.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/SalciccioliGA2012/scheme.yaml` & `pgradd-2.9.9/pgradd/data/SalciccioliGA2012/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/SalciccioliGA2012/surface.yaml` & `pgradd-2.9.9/pgradd/data/SalciccioliGA2012/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/SalciccioliGA2012/surface_benson.yaml` & `pgradd-2.9.9/pgradd/data/SalciccioliGA2012/surface_benson.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/XieGA2022/scheme.yaml` & `pgradd-2.9.9/pgradd/data/XieGA2022/scheme.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/data/XieGA2022/surface.yaml` & `pgradd-2.9.9/pgradd/data/XieGA2022/surface.yaml`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/tests/test_RINGparser_RDkitwrapper_test.py` & `pgradd-2.9.9/pgradd/tests/test_RINGparser_RDkitwrapper_test.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/tests/test_SMILES_to_thermo_examples.py` & `pgradd-2.9.9/pgradd/tests/test_SMILES_to_thermo_examples.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/yaml_io/__init__.py` & `pgradd-2.9.9/pgradd/yaml_io/__init__.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/yaml_io/builtins.py` & `pgradd-2.9.9/pgradd/yaml_io/builtins.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/yaml_io/lib_interface.py` & `pgradd-2.9.9/pgradd/yaml_io/lib_interface.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/yaml_io/schema.py` & `pgradd-2.9.9/pgradd/yaml_io/schema.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd/yaml_io/yaml_io.py` & `pgradd-2.9.9/pgradd/yaml_io/yaml_io.py`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/pgradd.egg-info/PKG-INFO` & `pgradd-2.9.9/pgradd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgradd
-Version: 2.9.8
+Version: 2.9.9
 Summary: Python package implements the Group Additivity (GA) method for estimating thermodynamic properties
 Home-page: https://github.com/VlachosGroup/PythonGroupAdditivity
 Author: Vlachos Research Group
 Author-email: vlachos@udel.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,17 +40,17 @@
 Citing this work
 ----------------
 G.R. Wittreich, D.G. Vlachos, Python Group Additivity (pGrAdd) software for estimating species thermochemical properties Comput. Phys. Commun. 273 (2022) 108277 https://doi.org/10.1016/j.cpc.2021.108277
 
 Developers
 ----------
 
--  Gerhard R Wittreich, P.E.
--  Geun Ho Gu
--  Michael Salciccioli
+-  Gerhard R Wittreich, Ph.D., P.E.
+-  Geun Ho Gu, Ph.D.
+-  Michael Salciccioli, Ph.D.
 -  Stephen M. Edie
 
 Required Packages
 -----------------
 
 -  Python2/Python3
 -  `pmutt`_ >= 1.3.2
```

### Comparing `pgradd-2.9.8/pgradd.egg-info/SOURCES.txt` & `pgradd-2.9.9/pgradd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgradd-2.9.8/setup.py` & `pgradd-2.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Import the lengthy rich-text README as the package's long
 # description:
 with open('README.rst', 'r') as fh:
 	long_description = fh.read()
 
 setuptools_info = {
 	'name': 'pgradd',
-	'version': '2.9.8',
+	'version': '2.9.9',
 	'author': 'Vlachos Research Group',
 	'author_email': 'vlachos@udel.edu',
 	'description': 'Python package implements the Group Additivity (GA) method for estimating thermodynamic properties',
 	'long_description': long_description,
 	'zip_safe': True,
 	'url': 'https://github.com/VlachosGroup/PythonGroupAdditivity',
 	'packages': setuptools.find_packages(),
```

