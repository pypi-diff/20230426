# Comparing `tmp/csgapi-0.1.3.tar.gz` & `tmp/csgapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csgapi-0.1.3.tar", last modified: Fri Feb 24 16:14:26 2023, max compression
+gzip compressed data, was "csgapi-0.1.4.tar", last modified: Wed Apr 26 15:34:46 2023, max compression
```

## Comparing `csgapi-0.1.3.tar` & `csgapi-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,66 @@
-drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-02-24 16:14:26.120179 csgapi-0.1.3/
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     3771 2023-02-24 16:14:26.120179 csgapi-0.1.3/PKG-INFO
-drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-02-24 16:14:26.120179 csgapi-0.1.3/csgapi/
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      108 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/__init__.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    16195 2023-02-24 16:00:20.000000 csgapi-0.1.3/csgapi/base.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    20732 2023-02-24 16:00:33.000000 csgapi-0.1.3/csgapi/client.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    22411 2023-02-24 16:00:37.000000 csgapi-0.1.3/csgapi/mixin.py
-drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-02-24 16:14:26.120179 csgapi-0.1.3/csgapi/objects/
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      108 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/__init__.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1088 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/accelerator_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1163 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/application.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1215 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/architecture.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1218 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/benchmarks.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1191 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/codename.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1147 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/continent.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1239 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/country.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1211 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/file_system.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1192 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/firmware.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1276 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/floating_point_unit.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1002 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/genera.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1974 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/green500.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1072 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/has_accelerator.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1083 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/has_interconnect.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1017 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/has_memory.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1120 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/has_operating_system.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1050 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/has_processor.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1156 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/interconnect.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1097 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/interconnect_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1272 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/interconnect_family.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1170 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/isas.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1216 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/manufacturer.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1043 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/memory_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1265 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/microarchitectures.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1613 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/ontology_type.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1674 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/operating_system.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1126 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/operating_system_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1238 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/other_software.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1048 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/pointer.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1070 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/processor_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1160 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/processor_hierarchy.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      977 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/processors.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1123 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/region.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1131 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/segment.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/spec1995.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/spec2000.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/spec2006.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/spec2017.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1301 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/system_configuration.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1172 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/system_family.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1220 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/system_manufacturer.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1220 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/system_state.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1650 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/systems.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1044 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/top500.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1085 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/top500_ranks.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1279 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/objects/used_to_run.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1274 2023-02-24 16:13:58.000000 csgapi-0.1.3/csgapi/setup.py
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     2946 2023-02-24 15:47:39.000000 csgapi-0.1.3/csgapi/utils.py
-drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-02-24 16:14:26.120179 csgapi-0.1.3/csgapi.egg-info/
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     3771 2023-02-24 16:14:26.000000 csgapi-0.1.3/csgapi.egg-info/PKG-INFO
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1744 2023-02-24 16:14:26.000000 csgapi-0.1.3/csgapi.egg-info/SOURCES.txt
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)        1 2023-02-24 16:14:26.000000 csgapi-0.1.3/csgapi.egg-info/dependency_links.txt
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)       15 2023-02-24 16:14:26.000000 csgapi-0.1.3/csgapi.egg-info/requires.txt
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)        7 2023-02-24 16:14:26.000000 csgapi-0.1.3/csgapi.egg-info/top_level.txt
--rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)       38 2023-02-24 16:14:26.120179 csgapi-0.1.3/setup.cfg
+drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-04-26 15:34:46.732418 csgapi-0.1.4/
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     3784 2023-04-26 15:34:46.732418 csgapi-0.1.4/PKG-INFO
+drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-04-26 15:34:46.728418 csgapi-0.1.4/csgapi/
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      108 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/__init__.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    16195 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/base.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    20846 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/client.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)    22411 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/mixin.py
+drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-04-26 15:34:46.732418 csgapi-0.1.4/csgapi/objects/
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      108 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/__init__.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1088 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/accelerator_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1163 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/application.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1215 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/architecture.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1218 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/benchmarks.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1187 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/codename.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1147 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/continent.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      896 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/coprocessors.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1239 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/country.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1207 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/file_system.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1188 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/firmware.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1272 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/floating_point_unit.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1002 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/genera.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      905 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/graphics_cards.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     2410 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/green500.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1072 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/has_accelerator.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1083 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/has_interconnect.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1017 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/has_memory.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1120 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/has_operating_system.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1050 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/has_processor.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1156 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/interconnect.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1097 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/interconnect_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1268 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/interconnect_family.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1170 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/isas.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1212 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/manufacturer.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1043 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/memory_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1265 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/microarchitectures.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1687 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/ontology_type.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1683 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/operating_system.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1126 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/operating_system_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1234 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/other_software.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1045 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/pointer.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1070 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/processor_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1160 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/processor_hierarchy.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)      977 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/processors.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1123 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/region.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1131 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/segment.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/spec1995.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/spec2000.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/spec2006.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1060 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/spec2017.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1301 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/system_configuration.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1172 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/system_family.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1220 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/system_manufacturer.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1216 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/system_state.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1938 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/objects/systems.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1044 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/top500.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1085 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/top500_ranks.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1279 2023-04-26 15:21:56.000000 csgapi-0.1.4/csgapi/objects/used_to_run.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1287 2023-04-26 15:27:42.000000 csgapi-0.1.4/csgapi/setup.py
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     2941 2023-04-26 15:23:48.000000 csgapi-0.1.4/csgapi/utils.py
+drwxr-xr-x   0 aniramadoss2002 (25590) Majors   (10000)        0 2023-04-26 15:34:46.732418 csgapi-0.1.4/csgapi.egg-info/
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     3784 2023-04-26 15:34:46.000000 csgapi-0.1.4/csgapi.egg-info/PKG-INFO
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)     1808 2023-04-26 15:34:46.000000 csgapi-0.1.4/csgapi.egg-info/SOURCES.txt
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)        1 2023-04-26 15:34:46.000000 csgapi-0.1.4/csgapi.egg-info/dependency_links.txt
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)       15 2023-04-26 15:34:46.000000 csgapi-0.1.4/csgapi.egg-info/requires.txt
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)        7 2023-04-26 15:34:46.000000 csgapi-0.1.4/csgapi.egg-info/top_level.txt
+-rw-r--r--   0 aniramadoss2002 (25590) Majors   (10000)       38 2023-04-26 15:34:46.732418 csgapi-0.1.4/setup.cfg
```

### Comparing `csgapi-0.1.3/PKG-INFO` & `csgapi-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: csgapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: API for interacting with the Computer Systems Genome database.
 Home-page: https://csgenome.org/
-Author: Ani Ramadoss
-Author-email: aniramadoss2002@vt.edu
+Author: Computer Systems Genome
+Author-email: csgenomevtteam@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `csgapi-0.1.3/csgapi/base.py` & `csgapi-0.1.4/csgapi/base.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/client.py` & `csgapi-0.1.4/csgapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 
 from .utils import handle_client_exception
 from contextlib import nullcontext
 from typing import Any, Optional
 
 import requests
 import requests.utils
-import sys
-print(sys.path)
 
 
 REDIRECT_MSG = (
     "python-gitlab detected a {status_code} ({reason!r}) redirection. You must update "
     "your GitLab URL to the correct URL to avoid issues. The redirection was from: "
     "{source!r} to {target!r}"
 )
@@ -98,25 +96,25 @@
         from .objects import country, genera, green500, isas, ontology_type, \
             processor_hierarchy, processors, spec1995, spec2000, spec2006, spec2017, \
             top500, top500_ranks, processor_configuration, has_processor, memory_configuration, \
             has_memory, accelerator_configuration, has_accelerator, interconnect_configuration, \
             has_interconnect, operating_system_configuration, has_operating_system, system_configuration
         from .objects import country, application, architecture,\
             continent, region, segment, system_family, system_manufacturer, systems, interconnect, \
-            benchmarks, used_to_run
+            benchmarks, used_to_run, graphics_cards, coprocessors
 
         self.used_to_run = used_to_run.UsedToRunManager(self)
         self.benchmarks = benchmarks.BenchmarksManager(self)
-        self.codename = codename.CodenameManager(self)
+        self.codenames = codename.CodenameManager(self)
         self.file_system = file_system.FileSystemManager(self)
         self.firmware = firmware.FirmwareManager(self)
         self.floating_point_unit = floating_point_unit.FloatingPointUnitManager(self)
         self.interconnect = interconnect.InterconnectManager(self)
         self.interconnect_family = interconnect_family.InterconnectFamilyManager(self)
-        self.manufacturer = manufacturer.ManufacturerManager(self)
+        self.manufacturers = manufacturer.ManufacturerManager(self)
         self.microarchitectures = microarchitectures.MicroarchitecturesManager(self)
         self.operating_system = operating_system.OperatingSystemManager(self)
         self.other_software = other_software.OtherSoftwareManager(self)
         self.pointer = pointer.PointerManager(self)
         self.system_state = system_state.SystemStateManager(self)
         self.genera = genera.GeneraManager(self)
         self.green500 = green500.Green500Manager(self)
@@ -149,14 +147,16 @@
         self.architecture = architecture.ArchitectureManager(self)
         self.continent = continent.ContinentManager(self)
         self.region = region.RegionManager(self)
         self.segment = segment.SegmentManager(self)
         self.system_family = system_family.SystemFamilyManager(self)
         self.system_manufacturer = system_manufacturer.SystemManufacturerManager(self)
         self.systems = systems.SystemsManager(self)
+        self.graphics_cards = graphics_cards.GraphicsCardManager(self)
+        self.coprocessors = coprocessors.CoprocessorManager(self)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args: Any):
         self.session.close()
 
@@ -294,15 +294,14 @@
 
         Raises:
             GitlabHttpError: When the return code is not 2xx
             GitlabParsingError: If the json data could not be parsed
         """
         try:
             result = self.http_request("get", path, params=params)
-            # print(result)
             return result.json()
         except Exception:
             return handle_client_exception(400, {'message': 'Unable to parse result.'})
 
     def http_list(self, path, params=None):
         """Make a GET request to the Gitlab server for list-oriented queries.
         Args:
```

### Comparing `csgapi-0.1.3/csgapi/mixin.py` & `csgapi-0.1.4/csgapi/mixin.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/accelerator_configuration.py` & `csgapi-0.1.4/csgapi/objects/accelerator_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/application.py` & `csgapi-0.1.4/csgapi/objects/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class ApplicationManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/application"
     _obj_cls = Application
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Application, super(ApplicationManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/architecture.py` & `csgapi-0.1.4/csgapi/objects/architecture.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class ArchitectureManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/architecture"
     _obj_cls = Architecture
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Architecture, super(ArchitectureManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/benchmarks.py` & `csgapi-0.1.4/csgapi/objects/benchmarks.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/codename.py` & `csgapi-0.1.4/csgapi/objects/codename.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since codename is a look up table,
 # our API does not support DELETE for it
 class CodenameManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "processors/codename"
     _obj_cls = Codename
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Codename, super(CodenameManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/continent.py` & `csgapi-0.1.4/csgapi/objects/continent.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class ContinentManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/continent"
     _obj_cls = Continent
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Continent, super(ContinentManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/country.py` & `csgapi-0.1.4/csgapi/objects/country.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/file_system.py` & `csgapi-0.1.4/csgapi/objects/file_system.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since file_system is a look up table,
 # our API does not support DELETE for it
 class FileSystemManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/file_system"
     _obj_cls = FileSystem
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(FileSystem, super(FileSystemManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/firmware.py` & `csgapi-0.1.4/csgapi/objects/firmware.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,17 @@
 
 # NOTE: even tho Delete Mixin is integrated, since firmware is a look up table,
 # our API does not support DELETE for it
 class FirmwareManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/firmware"
 
     _obj_cls = Firmware
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Firmware, super(FirmwareManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/floating_point_unit.py` & `csgapi-0.1.4/csgapi/objects/floating_point_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since floating_point_unit is a look up table,
 # our API does not support DELETE for it
 class FloatingPointUnitManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/floating_point_unit"
     _obj_cls = FloatingPointUnit
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(FloatingPointUnit, super(FloatingPointUnitManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/genera.py` & `csgapi-0.1.4/csgapi/objects/genera.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/green500.py` & `csgapi-0.1.4/csgapi/objects/green500.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     _id_attr = "uid"
     # pass
 
 
 class Green500Manager(GetMixin, CreateMixin, DeleteMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/green500"
     _obj_cls = Green500
-    _create_attrs = RequiredOptional(required=("information_source",), optional=("benchmark_type", "green500_rank", "green500_previous_rank", \
-        "top500_rank", "install_year", "publication_date", "power", "power_quality_level", \
-            "power_source", "measured_cores", "total_cores", "optimized_run_hpl", \
-                "optimized_run_peak_power", "submission_type_id", "mflops_per_watt", \
-                    "efficiency", "r_max", "r_peak", "n_max", "note"))
+    _create_attrs = RequiredOptional(required=("information_source",), optional=("benchmark_type", "green500_rank", "green500_previous_rank",
+                                                                                 "top500_rank", "install_year", "publication_date", "power", "power_quality_level",
+                                                                                 "power_source", "measured_cores", "total_cores", "optimized_run_hpl",
+                                                                                 "optimized_run_peak_power", "submission_type_id", "mflops_per_watt",
+                                                                                 "efficiency", "r_max", "r_peak", "n_max", "note"))
     # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
-    _update_attrs = RequiredOptional(required=(), optional=("benchmark_type", "green500_rank", "green500_previous_rank", \
-        "top500_rank", "information_source", "install_year", "publication_date", "power", "power_quality_level", \
-            "power_source", "measured_cores", "total_cores", "optimized_run_hpl", \
-                "optimized_run_peak_power", "submission_type_id", "mflops_per_watt", \
-                    "efficiency", "r_max", "r_peak", "n_max", "note"))
+    _update_attrs = RequiredOptional(required=(), optional=("benchmark_type", "green500_rank", "green500_previous_rank",
+                                                            "top500_rank", "information_source", "install_year", "publication_date", "power", "power_quality_level",
+                                                            "power_source", "measured_cores", "total_cores", "optimized_run_hpl",
+                                                            "optimized_run_peak_power", "submission_type_id", "mflops_per_watt",
+                                                            "efficiency", "r_max", "r_peak", "n_max", "note"))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Green500, super(Green500Manager, self).get(uid=uid, params=params))
```

### Comparing `csgapi-0.1.3/csgapi/objects/has_accelerator.py` & `csgapi-0.1.4/csgapi/objects/has_accelerator.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/has_interconnect.py` & `csgapi-0.1.4/csgapi/objects/has_interconnect.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/has_memory.py` & `csgapi-0.1.4/csgapi/objects/has_memory.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/has_operating_system.py` & `csgapi-0.1.4/csgapi/objects/has_operating_system.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/has_processor.py` & `csgapi-0.1.4/csgapi/objects/has_processor.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/interconnect.py` & `csgapi-0.1.4/csgapi/objects/interconnect.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/interconnect_configuration.py` & `csgapi-0.1.4/csgapi/objects/interconnect_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/interconnect_family.py` & `csgapi-0.1.4/csgapi/objects/interconnect_family.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since interconnect_family is a look up table,
 # our API does not support DELETE for it
 class InterconnectFamilyManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "interconnect_family"
     _obj_cls = InterconnectFamily
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(InterconnectFamily, super(InterconnectFamilyManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/isas.py` & `csgapi-0.1.4/csgapi/objects/isas.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/manufacturer.py` & `csgapi-0.1.4/csgapi/objects/manufacturer.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since manufacturer is a look up table,
 # our API does not support DELETE for it
 class ManufacturerManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "manufacturer"
     _obj_cls = Manufacturer
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Manufacturer, super(ManufacturerManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/memory_configuration.py` & `csgapi-0.1.4/csgapi/objects/memory_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/microarchitectures.py` & `csgapi-0.1.4/csgapi/objects/microarchitectures.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/ontology_type.py` & `csgapi-0.1.4/csgapi/objects/ontology_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,19 @@
     _id_attr = "uid"
     # pass
 
 
 class OntologyTypeManager(GetMixin, CreateMixin, DeleteMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "ontology_type"
     _obj_cls = OntologyType
-    _create_attrs = RequiredOptional(required=(), optional=("memory_type", "other_type", "generation", "standard", "module", "standard_type", "clock_rate", "cycle_time", "transfer_rate", "bandwidth", "cl_trcd_trp", "cas_latency", "voltage", "dimm_pins", "sodimm_pins", "microdimm_pins"))
+    _create_attrs = RequiredOptional(required=(), optional=("memory_type", "other_type", "generation", "standard", "module", "standard_type", "clock_rate",
+                                     "cycle_time", "transfer_rate", "bandwidth", "cl_trcd_trp", "cas_latency", "voltage", "dimm_pins", "sodimm_pins", "microdimm_pins"))
     # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
-    _update_attrs = RequiredOptional(required=(), optional=("memory_type", "other_type", "generation", "standard", "module", "standard_type", "clock_rate", "cycle_time", "transfer_rate", "bandwidth", "cl_trcd_trp", "cas_latency", "voltage", "dimm_pins", "sodimm_pins", "microdimm_pins"))
+    _update_attrs = RequiredOptional(required=(), optional=("memory_type", "other_type", "generation", "standard", "module", "standard_type", "clock_rate",
+                                     "cycle_time", "transfer_rate", "bandwidth", "cl_trcd_trp", "cas_latency", "voltage", "dimm_pins", "sodimm_pins", "microdimm_pins"))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(OntologyType, super(OntologyTypeManager, self).get(uid=uid, params=params))
```

### Comparing `csgapi-0.1.3/csgapi/objects/operating_system.py` & `csgapi-0.1.4/csgapi/objects/operating_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,25 +15,25 @@
     # pass
 
 
 # NOTE: even tho Delete Mixin is integrated, since operating_system is a look up table,
 # our API does not support DELETE for it
 class OperatingSystemManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "operating_system"
-    #TODO: find path name
+    # TODO: find path name
 
     _obj_cls = OperatingSystem
-    _create_attrs = RequiredOptional(required=("name",)) #"os_name", "kernel", "file_system", "os_family", "release_date", "end_of_life_date", "os_version" )) 
-    #NOTE: Check if attributes are required or optional (for both create and update)
-    #TODO: figure out if the auth section should be passed in here, 
+    # "os_name", "kernel", "file_system", "os_family", "release_date", "end_of_life_date", "os_version" ))
+    _create_attrs = RequiredOptional(required=("name",))
+    # NOTE: Check if attributes are required or optional (for both create and update)
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
-    _update_attrs = RequiredOptional(required=("name",)) #, optional=("kernel", "file_system", "os_family", "release_date", "end_of_life_date", "os_version"))
-    #TODO: Fix attributes, which are required/optional? Why the discrepancy btwn
+    # , optional=("kernel", "file_system", "os_family", "release_date", "end_of_life_date", "os_version"))
+    _update_attrs = RequiredOptional(required=("name",))
+    # TODO: Fix attributes, which are required/optional? Why the discrepancy btwn
     # models.py and the schema?
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(OperatingSystem, super(OperatingSystemManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/operating_system_configuration.py` & `csgapi-0.1.4/csgapi/objects/operating_system_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/other_software.py` & `csgapi-0.1.4/csgapi/objects/other_software.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since other_software is a look up table,
 # our API does not support DELETE for it
 class OtherSoftwareManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/other_software"
     _obj_cls = OtherSoftware
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(OtherSoftware, super(OtherSoftwareManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/pointer.py` & `csgapi-0.1.4/csgapi/objects/pointer.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,17 +16,15 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since pointer is a look up table,
 # our API does not support DELETE for it
 class PointerManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/pointer"
     _obj_cls = Pointer
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Pointer, super(PointerManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/processor_configuration.py` & `csgapi-0.1.4/csgapi/objects/processor_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/processor_hierarchy.py` & `csgapi-0.1.4/csgapi/objects/processor_hierarchy.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/processors.py` & `csgapi-0.1.4/csgapi/objects/processors.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/region.py` & `csgapi-0.1.4/csgapi/objects/region.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class RegionManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/region"
     _obj_cls = Region
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Region, super(RegionManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/segment.py` & `csgapi-0.1.4/csgapi/objects/segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class SegmentManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/segment"
     _obj_cls = Segment
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(Segment, super(SegmentManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/spec1995.py` & `csgapi-0.1.4/csgapi/objects/spec1995.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/spec2000.py` & `csgapi-0.1.4/csgapi/objects/spec2000.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/spec2006.py` & `csgapi-0.1.4/csgapi/objects/spec2006.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/spec2017.py` & `csgapi-0.1.4/csgapi/objects/spec2017.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/system_configuration.py` & `csgapi-0.1.4/csgapi/objects/system_configuration.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/system_family.py` & `csgapi-0.1.4/csgapi/objects/system_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class SystemFamilyManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/system_family"
     _obj_cls = SystemFamily
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(SystemFamily, super(SystemFamilyManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/system_manufacturer.py` & `csgapi-0.1.4/csgapi/objects/system_manufacturer.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
 
 # NOTE: even tho Delete Mixin is integrated, since country is a look up table,
 # out API does not dupport DELETE for it
 class SystemManufacturerManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "systems/system_manufacturer"
     _obj_cls = SystemManufacturer
     _create_attrs = RequiredOptional(required=("name",))
-    #TODO: figure out if the auth section should be passed in here,
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(SystemManufacturer, super(SystemManufacturerManager, self).get(uid=uid, params=params))
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/system_state.py` & `csgapi-0.1.4/csgapi/objects/system_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,17 @@
 
 
 # NOTE: even tho Delete Mixin is integrated, since system_state is a look up table,
 # our API does not support DELETE for it
 class SystemStateManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, RESTManager):
     _path = "benchmarks/system_state"
     _obj_cls = SystemState
-    _create_attrs = RequiredOptional(required=("name",)) 
-    #TODO: figure out if the auth section should be passed in here, 
+    _create_attrs = RequiredOptional(required=("name",))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
     _update_attrs = RequiredOptional(required=("name",))
 
     def get(self, uid=None, params=None):
-        # NOTE: the casting allows each object to follow the logic implemented in the 
+        # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
         return cast(SystemState, super(SystemStateManager, self).get(uid=uid, params=params))
-
-
```

### Comparing `csgapi-0.1.3/csgapi/objects/systems.py` & `csgapi-0.1.4/csgapi/objects/systems.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,23 +13,23 @@
     _id_attr = "uid"
     # pass
 
 
 class SystemsManager(GetMixin, CreateMixin, UpdateMixin, ListMixin, DeleteMixin, RESTManager):
     _path = "systems"
     _obj_cls = Systems
-    _create_attrs = RequiredOptional(required=(), optional=("moniker", "system_model",\
-        "system_family_id", "architecture_id", "system_manufacturer_id", "computer", \
-            "site", "application_id", "country_id", "region_id", "continent_id", "segment_id", \
-            "system_address", "latitude", "longitude"))
-    #TODO: figure out if the auth section should be passed in here,
+    _create_attrs = RequiredOptional(required=(), optional=("moniker", "system_model",
+                                                            "system_family_id", "architecture_id", "system_manufacturer_id", "computer",
+                                                            "site", "application_id", "country_id", "region_id", "continent_id", "segment_id",
+                                                            "system_address", "latitude", "longitude"))
+    # TODO: figure out if the auth section should be passed in here,
     # if so we need the func in mixin to refactor attrs before calling POST
-    _update_attrs = RequiredOptional(required=(), optional=("moniker", "system_model",\
-        "system_family_id", "architecture_id", "system_manufacturer_id", "computer", \
-            "site", "application_id", "country_id", "region_id", "continent_id", "segment_id", \
-            "system_address", "latitude", "longitude"))
+    _update_attrs = RequiredOptional(required=(), optional=("moniker", "system_model",
+                                                            "system_family_id", "architecture_id", "system_manufacturer_id", "computer",
+                                                            "site", "application_id", "country_id", "region_id", "continent_id", "segment_id",
+                                                            "system_address", "latitude", "longitude"))
 
     def get(self, uid=None, params=None):
         # NOTE: the casting allows each object to follow the logic implemented in the
         # MIXIN utils w/o the need to repeating it each time. it also allows customization
         # in each obj
-        return cast(Systems, super(SystemsManager, self).get(uid=uid, params=params))
+        return cast(Systems, super(SystemsManager, self).get(uid=uid, params=params))
```

### Comparing `csgapi-0.1.3/csgapi/objects/top500.py` & `csgapi-0.1.4/csgapi/objects/top500.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/top500_ranks.py` & `csgapi-0.1.4/csgapi/objects/top500_ranks.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/objects/used_to_run.py` & `csgapi-0.1.4/csgapi/objects/used_to_run.py`

 * *Files identical despite different names*

### Comparing `csgapi-0.1.3/csgapi/utils.py` & `csgapi-0.1.4/csgapi/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from flask import current_app
 import traceback
 
+
 def handle_client_exception(status=500, error_data={}, ex=None):
     """Exception handler for endpoints. This wraps error message
     in a common format and allows the user-specified return code.
     Use this in except block to return relvent error message to the
     client. For example:
     ```
     try:
@@ -12,15 +13,15 @@
     except orm_exception.NoResultFound:
         handle_exception(404, {'message': 'Object with uid={} not found.'.format(pid)})
     ```
 
     :param int status: HTTP status code to send back. Default 500
     :param error_data: Error data to send back
     """
-    # NOTE: adjusted to output json format 
+    # NOTE: adjusted to output json format
     # print traceback to logger if the exception is passed in
     # we don't need to log every case that comes through here since
     # some exception are expected and handle properly outside this function
     if ex is not None:
         current_app.logger.error(traceback.format_exc())
     payload = {}
     payload['status'] = status
@@ -42,17 +43,17 @@
     return (not failed, msg)
 
 
 class CSGServerError(Exception):
     def __init__(self, error_message, response_code, response_body):
 
         Exception.__init__(self, error_message)
-        self.response_code = response_code # Http status code
-        self.response_body = response_body # Full http response
-        
+        self.response_code = response_code  # Http status code
+        self.response_body = response_body  # Full http response
+
         # Parsed error message from server
         try:
             # if we receive str/bytes we try to convert to unicode/str to have
             # consistent message types (see #616)
             if (isinstance(error_message, bytes)):
                 self.error_message = error_message.decode()
             else:
@@ -81,8 +82,8 @@
             try:
                 return f(*args, **kwargs)
             except GitlabHttpError as e:
                 raise error(e.error_message, e.response_code, e.response_body) from e
 
         return cast(__F, wrapped_f)
 
-    return wrap
+    return wrap
```

### Comparing `csgapi-0.1.3/csgapi.egg-info/PKG-INFO` & `csgapi-0.1.4/csgapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: csgapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: API for interacting with the Computer Systems Genome database.
 Home-page: https://csgenome.org/
-Author: Ani Ramadoss
-Author-email: aniramadoss2002@vt.edu
+Author: Computer Systems Genome
+Author-email: csgenomevtteam@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `csgapi-0.1.3/csgapi.egg-info/SOURCES.txt` & `csgapi-0.1.4/csgapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 csgapi/objects/__init__.py
 csgapi/objects/accelerator_configuration.py
 csgapi/objects/application.py
 csgapi/objects/architecture.py
 csgapi/objects/benchmarks.py
 csgapi/objects/codename.py
 csgapi/objects/continent.py
+csgapi/objects/coprocessors.py
 csgapi/objects/country.py
 csgapi/objects/file_system.py
 csgapi/objects/firmware.py
 csgapi/objects/floating_point_unit.py
 csgapi/objects/genera.py
+csgapi/objects/graphics_cards.py
 csgapi/objects/green500.py
 csgapi/objects/has_accelerator.py
 csgapi/objects/has_interconnect.py
 csgapi/objects/has_memory.py
 csgapi/objects/has_operating_system.py
 csgapi/objects/has_processor.py
 csgapi/objects/interconnect.py
```

