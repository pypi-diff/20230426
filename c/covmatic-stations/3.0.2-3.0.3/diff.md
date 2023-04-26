# Comparing `tmp/covmatic-stations-3.0.2.tar.gz` & `tmp/covmatic-stations-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/covmatic-stations-3.0.2.tar", last modified: Wed Apr  5 13:53:05 2023, max compression
+gzip compressed data, was "dist/covmatic-stations-3.0.3.tar", last modified: Wed Apr 26 12:47:22 2023, max compression
```

## Comparing `covmatic-stations-3.0.2.tar` & `covmatic-stations-3.0.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/
--rw-r--r--   0 root         (0) root         (0)     1050 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8834 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8170 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/
--rw-r--r--   0 root         (0) root         (0)     1356 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/a/
--rw-r--r--   0 root         (0) root         (0)     5224 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23355 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/a.py
--rw-r--r--   0 root         (0) root         (0)     7712 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/aBioerPreparation.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/copan_24.py
--rw-r--r--   0 root         (0) root         (0)     4627 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/copan_48.py
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/copan_48_correction.json
--rw-r--r--   0 root         (0) root         (0)     5634 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/copan_48_saliva.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationA.json
--rw-r--r--   0 root         (0) root         (0)      181 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationAP1000.json
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationAP1000Reload.json
--rw-r--r--   0 root         (0) root         (0)      145 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationAP300.json
--rw-r--r--   0 root         (0) root         (0)      247 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationAReloadMixin.json
--rw-r--r--   0 root         (0) root         (0)     1571 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationATechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationATechnogenetics24.json
--rw-r--r--   0 root         (0) root         (0)      198 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/msg/StationATechnogenetics48.json
--rw-r--r--   0 root         (0) root         (0)     9547 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/p1000.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/p1000reload.py
--rw-r--r--   0 root         (0) root         (0)     1281 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/p300.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/reload.py
--rw-r--r--   0 root         (0) root         (0)    16556 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/a/technogenetics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/b/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32204 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/b.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/magnet_heights.json
--rw-r--r--   0 root         (0) root         (0)     1649 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/magnets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/b/msg/
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/msg/StationB.json
--rw-r--r--   0 root         (0) root         (0)     2806 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/msg/StationBTechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/msg/StationBTechnogeneticsWashBRemoval.json
--rw-r--r--   0 root         (0) root         (0)    24730 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/nest_12_reservoir_15ml_modified.json
--rw-r--r--   0 root         (0) root         (0)    17522 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/technogenetics.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/b/technogenetics_short.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/
--rw-r--r--   0 root         (0) root         (0)    22106 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/Bioer_full_dw.py
--rw-r--r--   0 root         (0) root         (0)    10649 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/Bioer_preparation.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/msg/
--rw-r--r--   0 root         (0) root         (0)      472 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/bioer/msg/BioerProtocol.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/c/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12774 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/bioer_mastermix_prep.py
--rw-r--r--   0 root         (0) root         (0)    16605 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/c.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/c/msg/
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/msg/StationC.json
--rw-r--r--   0 root         (0) root         (0)      582 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/msg/StationCBioerMastermixPrep.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/msg/StationCTechnogenetics.json
--rw-r--r--   0 root         (0) root         (0)     5005 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/c/technogenetics.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/geometry.py
--rw-r--r--   0 root         (0) root         (0)      560 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/hardware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/labware/
--rw-r--r--   0 root         (0) root         (0)    30016 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/labware/bioer_96_wellplate_2000ul.json
--rw-r--r--   0 root         (0) root         (0)     1370 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/labware/biofil_1_reservoir_500000ul.json
--rw-r--r--   0 root         (0) root         (0)     1983 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/labware/biofil_3_reservoir_200000ul.json
--rw-r--r--   0 root         (0) root         (0)     4044 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/lights.py
--rw-r--r--   0 root         (0) root         (0)     4804 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/movement_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/msg/
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/msg/Station.json
--rw-r--r--   0 root         (0) root         (0)     5589 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/multi_tube_source.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/request.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/sound_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations/sounds/
--rw-r--r--   0 root         (0) root         (0)    43884 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/sounds/alarm.mp3
--rw-r--r--   0 root         (0) root         (0)    20897 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/sounds/beep.mp3
--rw-r--r--   0 root         (0) root         (0)    23816 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/sounds/beep2.mp3
--rw-r--r--   0 root         (0) root         (0)    50089 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/sounds/finish.mp3
--rw-r--r--   0 root         (0) root         (0)    25070 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/station.py
--rw-r--r--   0 root         (0) root         (0)    13362 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/covmatic_stations/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8834 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2689 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/covmatic_stations.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 13:53:05.000000 covmatic-stations-3.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2702 2023-04-05 13:52:51.000000 covmatic-stations-3.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8834 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8170 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/a/
+-rw-r--r--   0 root         (0) root         (0)     5224 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23355 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/a.py
+-rw-r--r--   0 root         (0) root         (0)     7712 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/aBioerPreparation.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_24.py
+-rw-r--r--   0 root         (0) root         (0)     4627 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48.py
+-rw-r--r--   0 root         (0) root         (0)       47 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48_correction.json
+-rw-r--r--   0 root         (0) root         (0)     5634 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/copan_48_saliva.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationA.json
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP1000.json
+-rw-r--r--   0 root         (0) root         (0)      204 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP1000Reload.json
+-rw-r--r--   0 root         (0) root         (0)      145 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAP300.json
+-rw-r--r--   0 root         (0) root         (0)      247 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationAReloadMixin.json
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)      198 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics24.json
+-rw-r--r--   0 root         (0) root         (0)      198 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics48.json
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p1000.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p1000reload.py
+-rw-r--r--   0 root         (0) root         (0)     1281 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/p300.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/reload.py
+-rw-r--r--   0 root         (0) root         (0)    16556 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/a/technogenetics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/b/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32204 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/b.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/magnet_heights.json
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/magnets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationB.json
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)      538 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json
+-rw-r--r--   0 root         (0) root         (0)      473 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsWashBRemoval.json
+-rw-r--r--   0 root         (0) root         (0)    24730 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/nest_12_reservoir_15ml_modified.json
+-rw-r--r--   0 root         (0) root         (0)    17522 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/technogenetics.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/b/technogenetics_short.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/
+-rw-r--r--   0 root         (0) root         (0)    22106 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_full_dw.py
+-rw-r--r--   0 root         (0) root         (0)    10649 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_preparation.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/msg/
+-rw-r--r--   0 root         (0) root         (0)      472 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/bioer/msg/BioerProtocol.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/c/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12774 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/bioer_mastermix_prep.py
+-rw-r--r--   0 root         (0) root         (0)    16605 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/c.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationC.json
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCBioerMastermixPrep.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCTechnogenetics.json
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/c/technogenetics.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/geometry.py
+-rw-r--r--   0 root         (0) root         (0)      560 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/hardware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/labware/
+-rw-r--r--   0 root         (0) root         (0)    30016 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/bioer_96_wellplate_2000ul.json
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/biofil_1_reservoir_500000ul.json
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/labware/biofil_3_reservoir_200000ul.json
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/lights.py
+-rw-r--r--   0 root         (0) root         (0)     5008 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/movement_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/msg/
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/msg/Station.json
+-rw-r--r--   0 root         (0) root         (0)     5589 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/multi_tube_source.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/request.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sound_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/
+-rw-r--r--   0 root         (0) root         (0)    43884 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/alarm.mp3
+-rw-r--r--   0 root         (0) root         (0)    20897 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/beep.mp3
+-rw-r--r--   0 root         (0) root         (0)    23816 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/beep2.mp3
+-rw-r--r--   0 root         (0) root         (0)    50089 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/sounds/finish.mp3
+-rw-r--r--   0 root         (0) root         (0)    25253 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/station.py
+-rw-r--r--   0 root         (0) root         (0)    13334 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/covmatic_stations/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8834 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2689 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-26 12:47:21.000000 covmatic-stations-3.0.3/covmatic_stations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 12:47:22.000000 covmatic-stations-3.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2702 2023-04-26 12:47:05.000000 covmatic-stations-3.0.3/setup.py
```

### Comparing `covmatic-stations-3.0.2/LICENSE` & `covmatic-stations-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/MANIFEST.in` & `covmatic-stations-3.0.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/PKG-INFO` & `covmatic-stations-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-stations
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for the COVMATIC Opentrons stations
 Home-page: https://github.com/covmatic/stations
 Author: Marco Tiraboschi
 Author-email: marco.tiraboschi@unimi.it
 Maintainer: Marco Tiraboschi, Agostino Facotti, Giada Facoetti
 Maintainer-email: marco.tiraboschi@unimi.it, agostino.facotti@gmail.com, giada.facoetti@hotmail.it
 License: UNKNOWN
```

### Comparing `covmatic-stations-3.0.2/README.md` & `covmatic-stations-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/__init__.py` & `covmatic-stations-3.0.3/covmatic_stations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 
 logging.basicConfig(
     level=logging.INFO,
     format='%(asctime)s %(name)-12s %(levelname)-8s: %(message)s',
     datefmt='%Y-%m-%d %H:%M:%S',
 )
 logging.getLogger("asyncio").setLevel(logging.WARNING)
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json` & `covmatic-stations-3.0.3/covmatic_stations/a/COPAN 15 Tube Rack 14000 µL.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/__init__.py` & `covmatic-stations-3.0.3/covmatic_stations/a/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/a.py` & `covmatic-stations-3.0.3/covmatic_stations/a/a.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/aBioerPreparation.py` & `covmatic-stations-3.0.3/covmatic_stations/a/aBioerPreparation.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/copan_24.py` & `covmatic-stations-3.0.3/covmatic_stations/a/copan_24.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/copan_48.py` & `covmatic-stations-3.0.3/covmatic_stations/a/copan_48.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/copan_48_saliva.py` & `covmatic-stations-3.0.3/covmatic_stations/a/copan_48_saliva.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/msg/StationA.json` & `covmatic-stations-3.0.3/covmatic_stations/a/msg/StationA.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/msg/StationATechnogenetics.json` & `covmatic-stations-3.0.3/covmatic_stations/a/msg/StationATechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/p1000.py` & `covmatic-stations-3.0.3/covmatic_stations/a/p1000.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/p1000reload.py` & `covmatic-stations-3.0.3/covmatic_stations/a/p1000reload.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/p300.py` & `covmatic-stations-3.0.3/covmatic_stations/a/p300.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/reload.py` & `covmatic-stations-3.0.3/covmatic_stations/a/reload.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/a/technogenetics.py` & `covmatic-stations-3.0.3/covmatic_stations/a/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/__init__.py` & `covmatic-stations-3.0.3/covmatic_stations/b/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/b.py` & `covmatic-stations-3.0.3/covmatic_stations/b/b.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/magnet_heights.json` & `covmatic-stations-3.0.3/covmatic_stations/b/magnet_heights.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/magnets.py` & `covmatic-stations-3.0.3/covmatic_stations/b/magnets.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/msg/StationB.json` & `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationB.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/msg/StationBTechnogenetics.json` & `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json` & `covmatic-stations-3.0.3/covmatic_stations/b/msg/StationBTechnogeneticsElutionRemoval.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/nest_12_reservoir_15ml_modified.json` & `covmatic-stations-3.0.3/covmatic_stations/b/nest_12_reservoir_15ml_modified.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/technogenetics.py` & `covmatic-stations-3.0.3/covmatic_stations/b/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/b/technogenetics_short.py` & `covmatic-stations-3.0.3/covmatic_stations/b/technogenetics_short.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/bioer/Bioer_full_dw.py` & `covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_full_dw.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/bioer/Bioer_preparation.py` & `covmatic-stations-3.0.3/covmatic_stations/bioer/Bioer_preparation.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/bioer/__init__.py` & `covmatic-stations-3.0.3/covmatic_stations/bioer/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/__init__.py` & `covmatic-stations-3.0.3/covmatic_stations/c/__init__.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/bioer_mastermix_prep.py` & `covmatic-stations-3.0.3/covmatic_stations/c/bioer_mastermix_prep.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/c.py` & `covmatic-stations-3.0.3/covmatic_stations/c/c.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/msg/StationC.json` & `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationC.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/msg/StationCBioerMastermixPrep.json` & `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCBioerMastermixPrep.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/msg/StationCTechnogenetics.json` & `covmatic-stations-3.0.3/covmatic_stations/c/msg/StationCTechnogenetics.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/c/technogenetics.py` & `covmatic-stations-3.0.3/covmatic_stations/c/technogenetics.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/geometry.py` & `covmatic-stations-3.0.3/covmatic_stations/geometry.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/hardware.py` & `covmatic-stations-3.0.3/covmatic_stations/hardware.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/labware/bioer_96_wellplate_2000ul.json` & `covmatic-stations-3.0.3/covmatic_stations/labware/bioer_96_wellplate_2000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/labware/biofil_1_reservoir_500000ul.json` & `covmatic-stations-3.0.3/covmatic_stations/labware/biofil_1_reservoir_500000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/labware/biofil_3_reservoir_200000ul.json` & `covmatic-stations-3.0.3/covmatic_stations/labware/biofil_3_reservoir_200000ul.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/lights.py` & `covmatic-stations-3.0.3/covmatic_stations/lights.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         self._t = t
     
     def stop(self):
         self._on = False
         self.join()
     
     def initial_state(self) -> bool:
-        return self._ctx._hw_manager.hardware.get_lights()
+        return self._ctx.rail_lights_on
     
     def set_light(self, s: bool):
-        self._ctx._hw_manager.hardware.set_lights(rails=s)
+        self._ctx.set_rail_lights(s)
     
     def run(self):
         self._on = True
         self._state_initial = self.initial_state()
         while self._on:
             self._state = not self._state
             self.set_light(self._state)
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations/movement_manager.py` & `covmatic-stations-3.0.3/covmatic_stations/movement_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     def __init__(self, ctx: ProtocolContext, logger=logging.getLogger(__name__)):
         self._ctx = ctx
         self._hw_helper = HardwareHelper(ctx)
         self._home_pos: dict = {}
         self._logger = logger
 
     def move_to_home(self, safety_margin=10, force: bool = False):
-        ''' Move pipettes near home
+        """ Move pipettes near home
             without really homing to save time since homing is not needed
             :param safety_margin: the distance to keep from home position (not to hit the home switches)
             :param force: force the movement without checking if the gantry is near home
-        '''
+        """
         self._ctx.comment("Moving near home")
         if Mount.LEFT not in self._home_pos or Mount.RIGHT not in self._home_pos:
             self._ctx.home()
             self.save_home_pos_if_needed()
         else:
             actual_pos = dict()
             for m in [Mount.LEFT, Mount.RIGHT]:
@@ -46,36 +46,46 @@
                 self._hw_helper.move_rel(target_mount, delta_pos)
 
     def home(self):
         self._ctx.home()
         self.save_home_pos_if_needed()
 
     def save_home_pos_if_needed(self):
-        ''' saves the home position for the first time
+        """ saves the home position for the first time
             ==>> WARNING: To be called right AFTER a home command <<==
-        '''
+        """
         for m in [Mount.LEFT, Mount.RIGHT]:
             self._logger.debug("Saving mount {}".format(m))
             if self._home_pos.get(m, None) is None:
                 self._home_pos[m] = self._hw_helper.get_gantry_position(m, True)
 
     def retract(self):
-        ''' We try to retract the pipette attached
-            if we have zero or two pipette retract both two axes.'''
-        self._logger.debug("Retracting mount {}".format(self._mount))
-        self._hw_helper.retract(self._mount)
+        """ We try to retract each pipette attached """
+        for m in self._mounts:
+            self._hw_helper.retract(m)
 
     @property
     def _mount(self):
-        ''' Get the actual mount to use for pseudo-homing
-            if only one pipette is present that mount is taken, otherwise the left one '''
+        """ Get the actual mount to use for pseudo-homing
+            if only one pipette is present that mount is taken, otherwise the left one """
         mount = Mount.LEFT if 'left' in self._ctx.loaded_instruments else Mount.RIGHT
         self._logger.debug("Returning mount {}".format(mount))
         return mount
 
+    @property
+    def _mounts(self):
+        """ Get a list of mounted pipettes mount"""
+        mounts = []
+        if 'left' in self._ctx.loaded_instruments:
+            mounts.append(Mount.LEFT)
+        if 'right' in self._ctx.loaded_instruments:
+            mounts.append(Mount.RIGHT)
+
+        return mounts
+
     def _need_home(self, actual_positions, safety_margin: float) -> bool:
         x_is_near_home = False
         y_is_near_home = False
 
         for m in [Mount.LEFT, Mount.RIGHT]:
             if m in actual_positions:
                 self._logger.debug("Mount {}, Actual x: {}, trash x: {}".format(m, actual_positions[m].x, self._ctx.fixed_trash['A1'].center().point.x))
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations/msg/Station.json` & `covmatic-stations-3.0.3/covmatic_stations/msg/Station.json`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/multi_tube_source.py` & `covmatic-stations-3.0.3/covmatic_stations/multi_tube_source.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/request.py` & `covmatic-stations-3.0.3/covmatic_stations/request.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/sound_manager.py` & `covmatic-stations-3.0.3/covmatic_stations/sound_manager.py`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/sounds/alarm.mp3` & `covmatic-stations-3.0.3/covmatic_stations/sounds/alarm.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/sounds/beep.mp3` & `covmatic-stations-3.0.3/covmatic_stations/sounds/beep.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/sounds/beep2.mp3` & `covmatic-stations-3.0.3/covmatic_stations/sounds/beep2.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/sounds/finish.mp3` & `covmatic-stations-3.0.3/covmatic_stations/sounds/finish.mp3`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/covmatic_stations/station.py` & `covmatic-stations-3.0.3/covmatic_stations/station.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,16 +421,14 @@
         blink_period: float = 1,
         color: str = 'red',
         delay_time: float = 0,
         home: bool = True,
         level: int = logging.INFO,
         pause: bool = True,
     ):
-        # Note: changed default homing method to 'move_to_home' Agos, 2021-09-13
-
         old_color = self._button.color
         self._button.color = color
 
         self.watchdog_stop()
 
         if msg:
             self.msg = msg
@@ -440,25 +438,26 @@
         if blink and not self._ctx.is_simulating():
             self._sound_manager.play("beep")
             lt = (BlinkingLightHTTP if self._dummy_lights else BlinkingLight)(self._ctx, t=blink_period/2)
             lt.start()
         if delay_time > 0:
             self.status = "delay"
             self.watchdog_start(delay_time * 1.2)
-            self._ctx.delay(delay_time)
+            self._ctx.delay(delay_time, msg=self.msg)
             self.watchdog_stop()
         if pause:
             self.status = "pause"
-            self._ctx.pause()
+            self._ctx.pause(msg=self.msg)
             self._ctx.delay(0.1)  # pad to avoid pause leaking
         if blink and not self._ctx.is_simulating():
             lt.stop()
         self._button.color = old_color
         self.status = "running"
         self.msg = ""
+        self.watchdog_start()
 
 
 
     def dual_pause(self, msg: str, cols: Tuple[str, str] = ('red', 'yellow'), between: Optional[Callable] = None, home: Tuple[bool, bool] = (True, False)):
         msg = self.get_msg(msg)
         self._msg = "{}.\n{}".format(msg, self.get_msg("stop blink"))
         self.pause(self.msg, color=cols[0], home=home[0])
@@ -475,23 +474,26 @@
     def delay(self,
         mins: float,
         msg: str = "",
         color: str = 'yellow',
         home: bool = True,
         level: int = logging.INFO,
     ):
-        self.pause(
-            msg=self.get_msg_format("delay minutes", self.get_msg(msg), mins, self.get_msg("skip delay") if self._skip_delay else ""),
-            blink=False,
-            color=color,
-            delay_time=0 if self._skip_delay else (60 * mins),
-            home=home,
-            level=level,
-            pause=self._skip_delay,
-        )
+        if self._run_stage:
+            self.pause(
+                msg=self.get_msg_format("delay minutes", self.get_msg(msg), mins, self.get_msg("skip delay") if self._skip_delay else ""),
+                blink=False,
+                color=color,
+                delay_time=0 if self._skip_delay else (60 * mins),
+                home=home,
+                level=level,
+                pause=self._skip_delay,
+            )
+        else:
+            self.logger.info("Skipping delay of {} mins because no stage run before.".format(mins))
 
     ''' Managed delay
         we start counting, doing something (eg. mixing samples) than we wait for timer to elapse'''
     ''' Start counting function '''
     def delay_start_count(self):
         self._delay_manager.start()
 
@@ -589,14 +591,15 @@
         self._timer = Timer(timeout, self._handler)
         self._timer.start()
 
     def stop(self):
         self._logger.debug("Stopping watchdog")
         if self._timer is not None:
             self._timer.cancel()
+            self._timer = None
 
     def reset(self, timeout: int = 180):
         self.stop()
         self.start(timeout)
 
     def default_handler(self):
         self._logger.info("Default timeout handler reached.")
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations/utils.py` & `covmatic-stations-3.0.3/covmatic_stations/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if self.last_dollar == record['$']:
             if record['$'] == 'before':
                 self.level += 1
             else:
                 self.level -= 1
         self.last_dollar = record['$']
         if record['$'] == 'before':
-            return ' '.join(['\t' * self.level, record['payload'].get('text', '').format(**record['payload'])])
+            return ' '.join(['\t' * self.level, record['payload'].get('text', '')])
     
     def __call__(self, record: Dict[str, Any]):
         s = self.format(record)
         url = self.url
         if url and s:
             self.logfail_count.setdefault(url, 0)
             if self.logfail_count[url] < self.logfail_max:
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations.egg-info/PKG-INFO` & `covmatic-stations-3.0.3/covmatic_stations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covmatic-stations
-Version: 3.0.2
+Version: 3.0.3
 Summary: Package for the COVMATIC Opentrons stations
 Home-page: https://github.com/covmatic/stations
 Author: Marco Tiraboschi
 Author-email: marco.tiraboschi@unimi.it
 Maintainer: Marco Tiraboschi, Agostino Facotti, Giada Facoetti
 Maintainer-email: marco.tiraboschi@unimi.it, agostino.facotti@gmail.com, giada.facoetti@hotmail.it
 License: UNKNOWN
```

### Comparing `covmatic-stations-3.0.2/covmatic_stations.egg-info/SOURCES.txt` & `covmatic-stations-3.0.3/covmatic_stations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covmatic-stations-3.0.2/setup.py` & `covmatic-stations-3.0.3/setup.py`

 * *Files identical despite different names*

