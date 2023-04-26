# Comparing `tmp/oplab_pipeline-1.1.0.tar.gz` & `tmp/oplab_pipeline-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oplab_pipeline-1.1.0.tar", last modified: Tue Mar 28 13:47:45 2023, max compression
+gzip compressed data, was "oplab_pipeline-1.1.3.tar", last modified: Tue Apr 25 16:16:41 2023, max compression
```

## Comparing `oplab_pipeline-1.1.0.tar` & `oplab_pipeline-1.1.3.tar`

### file list

```diff
@@ -1,217 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6179 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/auv_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    57980 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/camera_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/cone_fitting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_cal/default_yaml/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/default_yaml/default_calibration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/euler_angles_from_rotation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41020 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/laser_calibrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/plane_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/plot_points_and_planes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_cal/ransac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/auv_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/
--rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/mission.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1736 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/jc220/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/jc220/camera.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/auv_nav.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/hybis/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/hybis/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/hybis/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_rov/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.177672 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.181671 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.181671 oplab_pipeline-1.1.0/src/auv_nav/localisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/dead_reckoning.py
--rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/particle_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/pf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/usbl_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/localisation/usbl_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.181671 oplab_pipeline-1.1.0/src/auv_nav/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_combined_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_stereo_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_vehicle_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/generic_csv_payload_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/hybis.py
--rw-r--r--   0 runner    (1001) docker     (123)    38968 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/koyo20rov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/load_matlab_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_NOC_nmea.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_NOC_polpred.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_acfr_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ae2000.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_alr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_autosub.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_biocam_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_eiva_navipac.py
--rw-r--r--   0 runner    (1001) docker     (123)    21690 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_gaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_interlacer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_koyo21rov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ntnu_dvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ntnu_stereo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_phins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_rdi.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_seaxerocks_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_stereo_gopro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_tide_CTI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_usbl_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/parsers/parser_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/auv_nav/plot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/plot/plot_parse_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/plot/plot_process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    83426 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    74281 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/auv_nav/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/body_to_inertial.py
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/csv_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/displayable_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/dvl_level_arm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/inertial_to_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/latlon_wgs84.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/time_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/auv_nav/tools/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/correct_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/attenuation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/debayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/manual_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/pixel_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/rescale.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrections/undistort.py
--rw-r--r--   0 runner    (1001) docker     (123)    56675 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/corrector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/correct_images/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/acfr/
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/acfr/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam/
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam4000_15c/
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/hybis/
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/hybis/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/ntnu_stereo/
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/rosbag/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/stereo_gopro/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/default_yaml/sx3/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/default_yaml/sx3/correct_images.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.185672 oplab_pipeline-1.1.0/src/correct_images/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/depth_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/rosbag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/loaders/xviii.py
--rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/correct_images/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/curve_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/file_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/joblib_tqdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/memmap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/correct_images/tools/numerical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10521 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/camera_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/camera_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     8297 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/console.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/oplab/default_yaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/vehicle.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts1/SSK17-01/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.173671 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts2/SSK16-01/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/filename_to_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/folder_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/oplab/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-28 13:47:45.000000 oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:47:45.189672 oplab_pipeline-1.1.0/src/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/scripts/auv_cd.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/scripts/debayer_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/scripts/extract_rosbag_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/scripts/merge_dataset_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-03-28 13:47:20.000000 oplab_pipeline-1.1.0/src/scripts/pixel_stats_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/auv_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25715 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57980 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/camera_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/cone_fitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_cal/default_yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/default_yaml/default_calibration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/euler_angles_from_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41020 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/laser_calibrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/plane_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/plot_points_and_planes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_cal/ransac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/auv_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14771 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1468 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1736 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1757 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/mission.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1962 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/insite/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/camera.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/auv_nav.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/hybis/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.860730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.868730 oplab_pipeline-1.1.3/src/auv_nav/localisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/dead_reckoning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43615 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31173 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/particle_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19387 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/pf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26656 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_combined_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_stereo_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_vehicle_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/generic_csv_payload_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/hybis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38968 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/koyo20rov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/load_matlab_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_nmea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_polpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_acfr_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17453 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ae2000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_alr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_autosub.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13242 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_biocam_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_eiva_navipac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_gaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_interlacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_koyo21rov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_dvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_stereo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_phins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rdi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15385 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_seaxerocks_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_stereo_gopro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_tide_CTI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_usbl_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/parsers/parser_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/plot_parse_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60072 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/plot/plot_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81521 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74413 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/auv_nav/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/body_to_inertial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/csv_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/displayable_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/dvl_level_arm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/inertial_to_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/latlon_wgs84.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/time_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/auv_nav/tools/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20183 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/correct_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9515 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/attenuation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/debayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/manual_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/pixel_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/rescale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrections/undistort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56562 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/corrector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/correct_images/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.872731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/correct_images.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/depth_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/rosbag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/loaders/xviii.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/correct_images/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/curve_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/file_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/joblib_tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/memmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/correct_images/tools/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/camera_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/camera_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/console.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/vehicle.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/camera.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.864730 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/filename_to_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/folder_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19627 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/oplab/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.876731 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-25 16:16:41.000000 oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:16:41.880731 oplab_pipeline-1.1.3/src/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/auv_cd.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/debayer_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/extract_rosbag_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/merge_dataset_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9179 2023-04-25 16:16:19.000000 oplab_pipeline-1.1.3/src/scripts/pixel_stats_folder.py
```

### Comparing `oplab_pipeline-1.1.0/LICENSE` & `oplab_pipeline-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/PKG-INFO` & `oplab_pipeline-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplab_pipeline
-Version: 1.1.0
+Version: 1.1.3
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![oplab_pipeline](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/oplab_pipeline.yml/badge.svg)](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/oplab_pipeline.yml) [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] [![Code Coverage](https://codecov.io/gh/ocean-perception/oplab_pipeline/branch/master/graph/badge.svg?token=PJBfl6qhp5)](https://codecov.io/gh/ocean-perception/oplab_pipeline) [![Documentation Status](https://readthedocs.org/projects/oplab-pipeline/badge/?version=latest)](https://oplab-pipeline.readthedocs.io/en/latest/?badge=latest) [![Docker Image CI](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/docker_image.yml/badge.svg)](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/docker_image.yml) [![DOI](https://zenodo.org/badge/101513536.svg)](https://zenodo.org/badge/latestdoi/101513536)
 
 
 
 # oplab_pipeline
```

### Comparing `oplab_pipeline-1.1.0/README.md` & `oplab_pipeline-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/setup.py` & `oplab_pipeline-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright (c) 2020, University of Southampton
+Copyright (c) 2023, University of Southampton
 All rights reserved.
 Licensed under the BSD 3-Clause License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import os
 import os.path
@@ -71,15 +71,15 @@
 def git_pep440_version():
     # Is Git installed?
     try:
         subprocess.call(["git", "--version"], stdout=subprocess.PIPE)
     except OSError:
         print("The command git --version was not successful. Is git installed?")
         return None
-    version_full = git_command(["describe", "--tags", "--dirty=.dirty"])
+    version_full = git_command(["describe", "--tags", "--dirty=+dirty"])
     version_tag = git_command(["describe", "--tags", "--abbrev=0"])
     version_tail = version_full[len(version_tag) :]  # noqa
     return version_tag + version_tail.replace("-", ".dev", 1).replace("-", "+", 1)
 
 
 def run_setup():
     """Get version from git, then install."""
@@ -114,14 +114,15 @@
     setup(
         name="oplab_pipeline",
         version=oplab_pipeline_version,
         author="Ocean Perception - University of Southampton",
         author_email="miquel.massot-campos@soton.ac.uk",
         description="Toolchain for AUV dive processing, camera calibration and image correction",  # noqa
         long_description=long_description,
+        long_description_content_type='text/markdown',
         url="https://github.com/ocean-perception/oplab_pipeline",
         packages=find_packages(where="src"),
         package_dir={"": "src"},
         classifiers=classifiers,
         license="BSD",
         entry_points={  # Optional
             "console_scripts": [
```

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/auv_cal.py` & `oplab_pipeline-1.1.3/src/auv_cal/auv_cal.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/calibration.py` & `oplab_pipeline-1.1.3/src/auv_cal/calibration.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/camera_calibrator.py` & `oplab_pipeline-1.1.3/src/auv_cal/camera_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/cone_fitting.py` & `oplab_pipeline-1.1.3/src/auv_cal/cone_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/default_yaml/default_calibration.yaml` & `oplab_pipeline-1.1.3/src/auv_cal/default_yaml/default_calibration.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/euler_angles_from_rotation_matrix.py` & `oplab_pipeline-1.1.3/src/auv_cal/euler_angles_from_rotation_matrix.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/laser_calibrator.py` & `oplab_pipeline-1.1.3/src/auv_cal/laser_calibrator.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/plane_fitting.py` & `oplab_pipeline-1.1.3/src/auv_cal/plane_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/plot_points_and_planes.py` & `oplab_pipeline-1.1.3/src/auv_cal/plot_points_and_planes.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_cal/ransac.py` & `oplab_pipeline-1.1.3/src/auv_cal/ransac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/auv_nav.py` & `oplab_pipeline-1.1.3/src/auv_nav/auv_nav.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/convert.py` & `oplab_pipeline-1.1.3/src/auv_nav/convert.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/dy152/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/alr/jc220/camera.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/alr/jc220/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/auv_nav.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/auv_nav.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -89,38 +89,33 @@
   usbl: True
   dead_reckoning:
     auv_centre: True
     auv_dvl: True
     camera_1: True
     camera_2: True
     camera_3: True
-    chemical: True
     payload: True
   particle_filter:
     auv_centre: True
     auv_dvl: True
     camera_1: True
     camera_2: True
     camera_3: True
-    chemical: True
     payload: True
   ekf:
     auv_centre: True
     camera_1: True
     camera_2: True
     camera_3: True
-    chemical: True
     payload: True
 
 spp_output:
   activate: False
   ekf:
     auv_centre: True
     camera_1: True
     camera_2: True
     camera_3: True
-    chemical: True
 
 plot_output:
   activate: True
-  pdf_plot: False
   html_plot: True
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_rov/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_rov/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ntnu_stereo/tautra21/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/rosbag/grassmap/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/smarty200/stereo_gopro/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts1/SSK17-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml` & `oplab_pipeline-1.1.3/src/auv_nav/default_yaml/ts2/SSK16-01/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/dead_reckoning.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/dead_reckoning.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/ekf.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/ekf.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/particle.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/particle.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/particle_filter.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/particle_filter.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/pf.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/pf.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/usbl_filter.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_filter.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/localisation/usbl_offset.py` & `oplab_pipeline-1.1.3/src/auv_nav/localisation/usbl_offset.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parse.py` & `oplab_pipeline-1.1.3/src/auv_nav/parse.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_combined_raw.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_combined_raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from auv_nav.sensors import (
     Altitude,
     BodyVelocity,
     Camera,
     Depth,
     InertialVelocity,
     Orientation,
-    Other,
+    Payload,
     Usbl,
 )
 from oplab import Console, get_processed_folder
 
 
 class AcfrCombinedRawWriter:
     """
@@ -83,15 +83,15 @@
         elif type(measurement) is Depth:
             data = measurement.to_acfr()
         elif type(measurement) is Usbl:
             data = measurement.to_acfr()
         elif type(measurement) is Orientation:
             data = measurement.to_acfr()
             self.rdi_orientation = measurement
-        elif type(measurement) is Other:
+        elif type(measurement) is Payload:
             pass
         elif type(measurement) is Camera:
             # Get rid of laser images
             if "xxx" in measurement.filename:
                 pass
             else:
                 data = measurement.to_acfr()
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_stereo_pose.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_stereo_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/acfr_vehicle_pose.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/acfr_vehicle_pose.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/generic_csv_payload_parser.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/generic_csv_payload_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from auv_nav.sensors import Other
+from auv_nav.sensors import Payload
 from oplab.console import Console
 from oplab.filename_to_date import FilenameToDate
 
 import pandas as pd
 
 def generic_csv_payload_parser(filepath, columns_dict, timeoffset_s=0):
     data_list = []
@@ -11,15 +11,15 @@
     #f2d = FilenameToDate(None, filepath, columns_dict)
     #df = f2d.df
 
     df = pd.read_csv(filepath)
     df["epoch_timestamp"] = df["corrected_timestamp"]
 
     for index, row in df.iterrows():
-        data = Other()
+        data = Payload()
         data.data = {}
         data.epoch_timestamp = row["epoch_timestamp"] + timeoffset_s
         for key in df.columns:
             if key == "epoch_timestamp":
                 continue
             data.data[key] = row[key]
         data_list.append(data)
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/hybis.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/hybis.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/koyo20rov.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/koyo20rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/load_matlab_file.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/load_matlab_file.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_NOC_nmea.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_nmea.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     category = category
     output_format = ftype
 
     if category == Category.USBL:
         filepath = mission.usbl.filepath
         timezone = mission.usbl.timezone
         beacon_id = mission.usbl.label
-        timeoffset = mission.usbl.timeoffset
+        timeoffset = mission.usbl.timeoffset_s
         timezone_offset = read_timezone(timezone)
         latitude_reference = mission.origin.latitude
         longitude_reference = mission.origin.longitude
 
         usbl = Usbl(
             mission.usbl.std_factor,
             mission.usbl.std_offset,
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_NOC_polpred.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_NOC_polpred.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     sensor_string = "autosub"
     category = category
     output_format = ftype
 
     if category == Category.TIDE:
         filepath = mission.tide.filepath
         timezone = mission.tide.timezone
-        timeoffset = mission.tide.timeoffset
+        timeoffset = mission.tide.timeoffset_s
         timezone_offset = read_timezone(timezone)
 
         tide = Tide(mission.tide.std_offset)
         tide.sensor_string = sensor_string
 
         path = get_raw_folder(outpath / ".." / filepath)
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_acfr_images.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_acfr_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     # parser meta data
     class_string = "measurement"
     frame_string = "body"
     category = "image"
     sensor_string = "acfr_standard"
 
     timezone = mission.image.timezone
-    timeoffset = mission.image.timeoffset
+    timeoffset = mission.image.timeoffset_s
     filepath = mission.image.cameras[0].path
     camera1_label = mission.image.cameras[0].name
     camera2_label = mission.image.cameras[1].name
 
     # read in timezone
     if isinstance(timezone, str):
         if timezone == "utc" or timezone == "UTC":
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ae2000.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ae2000.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 def parse_ae2000(mission: Mission, vehicle: Vehicle, category, ftype, outpath):
     # parser meta data
     class_string = "measurement"
     sensor_string = "ae2000"
 
     # read in date from filename
     timezone = mission.velocity.timezone
-    timeoffset = mission.velocity.timeoffset
+    timeoffset = mission.velocity.timeoffset_s
     filepath = mission.velocity.filepath
 
     if category == "velocity" or category == "altitude":
         if category == "velocity":
             filename = mission.velocity.filename  # e.g. dvl180805123503.csv
         else:
             filename = mission.altitude.filename  # e.g. dvl180805123503.csv
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_alr.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_alr.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # parser meta data
     sensor_string = "alr"
     category = category
     output_format = ftype
     filename = mission.velocity.filename
     filepath = mission.velocity.filepath
 
+    # TODO handle timezone and timeoffsets
+
     # ALR std models
     depth_std_factor = mission.depth.std_factor
     velocity_std_factor = mission.velocity.std_factor
     velocity_std_offset = mission.velocity.std_offset
     orientation_std_offset = mission.orientation.std_offset
     altitude_std_factor = mission.altitude.std_factor
     headingoffset = vehicle.dvl.yaw
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_autosub.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_autosub.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     # parser meta data
     sensor_string = "autosub"
     category = category
     output_format = ftype
     filename = mission.velocity.filename
     filepath = mission.velocity.filepath
 
+    # TODO handle timezone and timeoffsets
+
     # autosub std models
     depth_std_factor = mission.depth.std_factor
     velocity_std_factor = mission.velocity.std_factor
     velocity_std_offset = mission.velocity.std_offset
     orientation_std_offset = mission.orientation.std_offset
     altitude_std_factor = mission.altitude.std_factor
     headingoffset = vehicle.dvl.yaw
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_biocam_images.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_biocam_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     class_string = "measurement"
     frame_string = "body"
     category = "image"
     sensor_string = "biocam"
 
     timezone = mission.image.timezone
     timezone_offset = 0
-    timeoffset = mission.image.timeoffset
+    timeoffset = mission.image.timeoffset_s
     filepath = mission.image.cameras[0].path
     camera1_label = mission.image.cameras[0].name
     camera2_label = mission.image.cameras[1].name
 
     # read in timezone
     if isinstance(timezone, str):
         if timezone == "utc" or timezone == "UTC":
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_eiva_navipac.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_eiva_navipac.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_gaps.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_gaps.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     # parser meta data
     class_string = "measurement"
     sensor_string = "gaps"
     frame_string = "inertial"
 
     timezone = mission.usbl.timezone
-    timeoffset = mission.usbl.timeoffset
+    timeoffset = mission.usbl.timeoffset_s
     filepath = mission.usbl.filepath
     usbl_id = mission.usbl.label
     latitude_reference = mission.origin.latitude
     longitude_reference = mission.origin.longitude
 
     # define headers used in phins
     header_absolute = "$PTSAG"  # '<< $PTSAG' #georeferenced strings
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_interlacer.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_interlacer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_koyo21rov.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_koyo21rov.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ntnu_dvl.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_dvl.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 
     category_str = None
     if category == Category.VELOCITY:
         category_str = "velocity"
     elif category == Category.ALTITUDE:
         category_str = "altitude"
 
+    # TODO handle timezone and timeoffsets
+
     velocity_std_factor = mission.velocity.std_factor
     velocity_std_offset = mission.velocity.std_offset
     heading_offset = vehicle.dvl.yaw
     body_velocity = BodyVelocity(
         velocity_std_factor,
         velocity_std_offset,
         heading_offset,
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_ntnu_stereo.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_ntnu_stereo.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # parser meta data
     class_string = "measurement"
     frame_string = "body"
     category = "image"
     sensor_string = "ntnu_stereo"
 
     timezone = mission.image.timezone
-    timeoffset = mission.image.timeoffset
+    timeoffset = mission.image.timeoffset_s
     filepath = mission.image.cameras[0].path
     camera1_label = "L"
     camera2_label = "R"
 
     # read in timezone
     if isinstance(timezone, str):
         if timezone == "utc" or timezone == "UTC":
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_phins.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_phins.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         # read in date from filename
         yyyy = int(self.filename[0:4])
         mm = int(self.filename[4:6])
         dd = int(self.filename[6:8])
         date = yyyy, mm, dd
 
         self.timestamp = PhinsTimestamp(
-            date, mission.velocity.timezone, mission.velocity.timeoffset
+            date, mission.velocity.timezone, mission.velocity.timeoffset_s
         )
         self.body_velocity = BodyVelocity(
             velocity_std_factor,
             velocity_std_offset,
             self.headingoffset,
             self.timestamp,
         )
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_rdi.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rdi.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,24 @@
     ot.sensor_string = sensor_string
     al.sensor_string = sensor_string
 
     if category == Category.VELOCITY:
         Console.info("... parsing RDI velocity")
         filename = mission.velocity.filename
         filepath = mission.velocity.filepath
-        timeoffset_s = mission.velocity.timeoffset_s
+        timeoffset_s = mission.velocity.offset_s
     elif category == Category.ORIENTATION:
         Console.info("... parsing RDI orientation")
         filename = mission.orientation.filename
         filepath = mission.orientation.filepath
-        timeoffset_s = mission.orientation.timeoffset_s
+        timeoffset_s = mission.orientation.offset_s
     elif category == Category.ALTITUDE:
         Console.info("... parsing RDI altitude")
         filename = mission.altitude.filename
-        timeoffset_s = mission.altitude.timeoffset_s
+        timeoffset_s = mission.altitude.offset_s
         filepath = mission.altitude.filepath
 
     logfile = get_raw_folder(outpath / ".." / filepath / filename)
     data_list = []
     altitude_valid = False
     with logfile.open("r", errors="ignore") as rdi_file:
         for line in rdi_file.readlines():
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_rosbag.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_rosbag.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,35 +141,32 @@
     orientation.sensor_string = "rosbag"
     depth.sensor_string = "rosbag"
     altitude.sensor_string = "rosbag"
     usbl.sensor_string = "rosbag"
 
     # Adjust timezone offsets
     body_velocity.tz_offset_s = (
-        read_timezone(mission.velocity.timezone) * 60 + mission.velocity.timeoffset
+        read_timezone(mission.velocity.timezone) * 60 + mission.velocity.offset_s
     )
     orientation.tz_offset_s = (
-        read_timezone(mission.orientation.timezone) * 60
-        + mission.orientation.timeoffset
+        read_timezone(mission.orientation.timezone) * 60 + mission.orientation.offset_s
     )
     depth.tz_offset_s = (
-        read_timezone(mission.depth.timezone) * 60 + mission.depth.timeoffset
+        read_timezone(mission.depth.timezone) * 60 + mission.depth.offset_s
     )
     altitude.tz_offset_s = (
-        read_timezone(mission.altitude.timezone) * 60 + mission.altitude.timeoffset
-    )
-    usbl.tz_offset_s = (
-        read_timezone(mission.usbl.timezone) * 60 + mission.usbl.timeoffset
+        read_timezone(mission.altitude.timezone) * 60 + mission.altitude.offset_s
     )
+    usbl.tz_offset_s = read_timezone(mission.usbl.timezone) * 60 + mission.usbl.offset_s
 
     if len(mission.image.cameras) > 0:
         camera = Camera()
         camera.sensor_string = mission.image.cameras[0].name
         camera.tz_offset_s = (
-            read_timezone(mission.image.timezone) * 60 + mission.image.timeoffset
+            read_timezone(mission.image.timezone) * 60 + mission.image.offset_s
         )
 
     data_list = []
 
     bagfile = None
     wanted_topic = None
     data_object = None
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_seaxerocks_images.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_seaxerocks_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,24 +25,24 @@
     class_string = "measurement"
     frame_string = "body"
     category_stereo = "image"
     category_laser = "laser"
     sensor_string = "seaxerocks_3"
 
     timezone = mission.image.timezone
-    timeoffset = mission.image.timeoffset
+    timeoffset = mission.image.timeoffset_s
     camera1_filepath = mission.image.cameras[0].path
     camera2_filepath = mission.image.cameras[1].path
     camera3_filepath = mission.image.cameras[2].path
     camera1_label = mission.image.cameras[0].name
     camera2_label = mission.image.cameras[1].name
     camera3_label = mission.image.cameras[2].name
-    camera1_timeoffset = mission.image.cameras[0].timeoffset
-    camera2_timeoffset = mission.image.cameras[1].timeoffset
-    camera3_timeoffset = mission.image.cameras[2].timeoffset
+    camera1_timeoffset = mission.image.cameras[0].timeoffset_s
+    camera2_timeoffset = mission.image.cameras[1].timeoffset_s
+    camera3_timeoffset = mission.image.cameras[2].timeoffset_s
 
     epoch_timestamp_stereo = []
     epoch_timestamp_laser = []
     epoch_timestamp_camera1 = []
     epoch_timestamp_camera2 = []
     epoch_timestamp_camera3 = []
     stereo_index = []
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_stereo_gopro.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_stereo_gopro.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_tide_CTI.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_tide_CTI.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     sensor_string = "alr"
     category = category
     output_format = ftype
 
     if category == Category.TIDE:
         filepath = mission.tide.filepath
         timezone = mission.tide.timezone
-        timeoffset = mission.tide.timeoffset
+        timeoffset = mission.tide.timeoffset_s
         timezone_offset = read_timezone(timezone)
 
         tide = Tide(mission.tide.std_offset)
         tide.sensor_string = sensor_string
 
         path = get_raw_folder(outpath / ".." / filepath)
         file_list = get_file_list(path)
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parse_usbl_dump.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parse_usbl_dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     frame_string = "inertial"
 
     # gaps std models
     distance_std_factor = mission.usbl.std_factor
     distance_std_offset = mission.usbl.std_offset
 
     timezone = mission.usbl.timezone
-    timeoffset = mission.usbl.timeoffset
+    timeoffset = mission.usbl.timeoffset_s
     filepath = mission.usbl.filepath
     filename = mission.usbl.filename
     label = mission.usbl.label
 
     filepath = get_raw_folder(outpath / ".." / filepath)
 
     latitude_reference = mission.origin.latitude
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/parsers/parser_template.py` & `oplab_pipeline-1.1.3/src/auv_nav/parsers/parser_template.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from oplab import Console
 
 
 def parse_template(mission, vehicle, category, output_format, outpath):
     # Get your data from a file using mission paths, for example
     your_data = None
 
+    # TODO handle timezone and timeoffsets
+
     # Let's say you want a new IMU, instance the measurement to work
     orientation = Orientation()
 
     data_list = []
     if category == Category.ORIENTATION:
         Console.info("... parsing orientation")
         for i in your_data:
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/plot/plot_parse_data.py` & `oplab_pipeline-1.1.3/src/auv_nav/plot/plot_parse_data.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/plot/plot_process_data.py` & `oplab_pipeline-1.1.3/src/auv_nav/plot/plot_process_data.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/process.py` & `oplab_pipeline-1.1.3/src/auv_nav/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from auv_nav.sensors import (
     Altitude,
     BodyVelocity,
     Camera,
     Depth,
     InertialVelocity,
     Orientation,
-    Other,
+    Payload,
     SyncedOrientationBodyVelocity,
     Usbl,
 )
 from auv_nav.tools.body_to_inertial import body_to_inertial
 from auv_nav.tools.csv_tools import load_states, spp_csv, write_csv, write_sidescan_csv
 from auv_nav.tools.dvl_level_arm import compute_angular_speeds, correct_lever_arm
 from auv_nav.tools.interpolate import interpolate, interpolate_sensor_list
@@ -148,20 +148,15 @@
     pf_fusion_centre_list = []
     pf_usbl_datapoints = []
     pf_particles_list = []
     pf_northings_std = []
     pf_eastings_std = []
     pf_yaw_std = []
 
-    # placeholders for chemical data
-    chemical_list = []
-    chemical_ekf_list = []
-    chemical_pf_list = []
-
-    # Placeholders for other payloads
+    # Placeholders for payloads
     # We could have more than one payload, so we will store them as a dict of lists
     # where they key is the payload name
     payload_dict = {}
 
     # load auv_nav.yaml for particle filter and other setup
     filepath = Path(filepath).resolve()
     filepath = get_processed_folder(filepath)
@@ -309,31 +304,28 @@
             csv_output_activate = d["activate"]
             csv_usbl = d["usbl"]
             csv_dr_auv_centre = d["dead_reckoning"]["auv_centre"]
             csv_dr_auv_dvl = d["dead_reckoning"]["auv_dvl"]
             csv_dr_camera_1 = d["dead_reckoning"]["camera_1"]
             csv_dr_camera_2 = d["dead_reckoning"]["camera_2"]
             csv_dr_camera_3 = d["dead_reckoning"]["camera_3"]
-            csv_dr_chemical = d["dead_reckoning"].get("chemical", False)
-            csv_dr_payload = d["dead_reckoning"].get("payload", False)
+            csv_dr_payload = d["dead_reckoning"].get("payload", True)
 
             csv_pf_auv_centre = d["particle_filter"]["auv_centre"]
             csv_pf_auv_dvl = d["particle_filter"]["auv_dvl"]
             csv_pf_camera_1 = d["particle_filter"]["camera_1"]
             csv_pf_camera_2 = d["particle_filter"]["camera_2"]
             csv_pf_camera_3 = d["particle_filter"]["camera_3"]
-            csv_pf_chemical = d["particle_filter"].get("chemical", False)
-            csv_pf_payload = d["particle_filter"].get("payload", False)
+            csv_pf_payload = d["particle_filter"].get("payload", True)
 
             csv_ekf_auv_centre = d["ekf"]["auv_centre"]
             csv_ekf_camera_1 = d["ekf"]["camera_1"]
             csv_ekf_camera_2 = d["ekf"]["camera_2"]
             csv_ekf_camera_3 = d["ekf"]["camera_3"]
-            csv_ekf_chemical = d["ekf"].get("chemical", False)
-            csv_ekf_payload = d["ekf"].get("payload", False)
+            csv_ekf_payload = d["ekf"].get("payload", True)
         else:
             csv_output_activate = False
             Console.warn(
                 "csv output undefined in auv_nav.yaml. Has been"
                 + ' set to "False". To activate, add as per'
                 + " default auv_nav.yaml found within auv_nav"
                 + ' file structure and set values to "True".'
@@ -373,14 +365,20 @@
     vehicle = Vehicle(vehicle_file)
 
     Console.info("Loading mission.yaml")
     mission_file = filepath / "mission.yaml"
     mission_file = get_raw_folder(mission_file)
     mission = Mission(mission_file)
 
+    time_str = time.strftime("%Y%m%d_%H%M%S", time.localtime())
+    mission_log = get_processed_folder(filepath) / "log" / (time_str + "_mission.yaml")
+    vehicle_log = get_processed_folder(filepath) / "log" / (time_str + "_vehicle.yaml")
+    mission_file.copy(mission_log)
+    vehicle_file.copy(vehicle_log)
+
     camera1_offsets = [
         vehicle.camera1.surge,
         vehicle.camera1.sway,
         vehicle.camera1.heave,
     ]
     camera2_offsets = [
         vehicle.camera2.surge,
@@ -411,20 +409,14 @@
             ]
         else:
             Console.quit(
                 "BioCam format is expected to have one camera where `records_laser` "
                 "is set to `True`."
             )
 
-    chemical_offset = [
-        vehicle.chemical.surge,
-        vehicle.chemical.sway,
-        vehicle.chemical.heave,
-    ]
-
     outpath = filepath / "nav"
 
     nav_standard_file = outpath / "nav_standard.json"
     nav_standard_file = get_processed_folder(nav_standard_file)
     Console.info("Loading json file {}".format(nav_standard_file))
 
     with nav_standard_file.open("r") as nav_standard:
@@ -506,19 +498,14 @@
                     camera2_list.append(camera2)
 
             if "laser" in parsed_json_data[i]["category"]:
                 camera3 = Camera()
                 camera3.from_json(parsed_json_data[i], "camera3")
                 camera3_list.append(camera3)
 
-            if "chemical" in parsed_json_data[i]["category"]:
-                chemical = Other()
-                chemical.from_json(parsed_json_data[i])
-                chemical_list.append(chemical)
-
     camera1_dr_list = copy.deepcopy(camera1_list)
     camera2_dr_list = copy.deepcopy(camera2_list)
     camera3_dr_list = copy.deepcopy(camera3_list)
 
     payload_offset = {}
     for payload in vehicle.payloads:
         payload_offset[payload] = [
@@ -537,27 +524,25 @@
         else:
             Console.quit("Payload format {} not supported.".format(payload_format))
 
     if particle_filter_activate:
         camera1_pf_list = copy.deepcopy(camera1_list)
         camera2_pf_list = copy.deepcopy(camera2_list)
         camera3_pf_list = copy.deepcopy(camera3_list)
-        chemical_pf_list = copy.deepcopy(chemical_list)
         pf_payload_dict = {}
         for key in payload_dict:
             if "_pf" not in key and "_ekf" not in key:
                 pf_payload_dict[key + "_pf"] = copy.deepcopy(payload_dict[key])
         payload_dict = {**payload_dict, **pf_payload_dict}
 
     if ekf_activate:
         camera1_ekf_list = copy.deepcopy(camera1_list)
         camera2_ekf_list = copy.deepcopy(camera2_list)
         camera3_ekf_list = copy.deepcopy(camera3_list)
         camera3_ekf_list_at_dvl = copy.deepcopy(camera3_list)
-        chemical_ekf_list = copy.deepcopy(chemical_list)
         ekf_payload_dict = {}
         for key in payload_dict:
             if "_pf" not in key and "_ekf" not in key:
                 ekf_payload_dict[key + "_ekf"] = copy.deepcopy(payload_dict[key])
         payload_dict = {**payload_dict, **ekf_payload_dict}
 
     # make path for processed outputs
@@ -1570,44 +1555,15 @@
         for c in range(len(camera3_ekf_list_at_dvl)):
             # append to the temp empty list. [remove] or[pop] or [del] will fail because list index is updated
             if camera3_ekf_list_at_dvl[c].depth is not None:
                 _temp_ekf.append(camera3_ekf_list_at_dvl[c])
         # Deep-copy of the temporal list
         camera3_ekf_list_at_dvl = copy.deepcopy(_temp_ekf)
 
-    # perform interpolations of state data to chemical time stamps for both
-    # DR and PF
-    if len(chemical_list) > 1:
-        interpolate_sensor_list(
-            chemical_list,
-            "chemical",
-            chemical_offset,
-            origin_offsets,
-            latlon_reference,
-            dead_reckoning_centre_list,
-        )
-        if len(pf_fusion_centre_list) > 1:
-            interpolate_sensor_list(
-                chemical_pf_list,
-                "chemical",
-                chemical_offset,
-                origin_offsets,
-                latlon_reference,
-                pf_fusion_centre_list,
-            )
-        if len(chemical_ekf_list) > 1:
-            interpolate_sensor_list(
-                chemical_ekf_list,
-                "chemical",
-                chemical_offset,
-                origin_offsets,
-                latlon_reference,
-                ekf_list,
-            )
-
+    # Interpolate state data to payload time stamps for DR, EKF and PF
     for key in payload_dict:
         if "_pf" not in key and "_ekf" not in key:
             interpolate_sensor_list(
                 payload_dict[key],
                 key,
                 payload_offset[key],
                 origin_offsets,
@@ -1796,21 +1752,14 @@
             args=[drcsvpath, dead_reckoning_dvl_list, "auv_dr_dvl", csv_dr_auv_dvl],
         )
         t.start()
         threads.append(t)
 
         t = threading.Thread(
             target=write_csv,
-            args=[drcsvpath, chemical_list, "auv_dr_chemical", csv_dr_chemical],
-        )
-        t.start()
-        threads.append(t)
-
-        t = threading.Thread(
-            target=write_csv,
             args=[
                 pfcsvpath,
                 pf_fusion_centre_list,
                 "auv_pf_centre",
                 csv_pf_auv_centre,
             ],
         )
@@ -1822,65 +1771,51 @@
             args=[pfcsvpath, pf_fusion_dvl_list, "auv_pf_dvl", csv_pf_auv_dvl],
         )
         t.start()
         threads.append(t)
 
         t = threading.Thread(
             target=write_csv,
-            args=[pfcsvpath, chemical_pf_list, "auv_pf_chemical", csv_pf_chemical],
-        )
-        t.start()
-        threads.append(t)
-
-        t = threading.Thread(
-            target=write_csv,
             args=[ekfcsvpath, ekf_list, "auv_ekf_centre", csv_ekf_auv_centre],
         )
         t.start()
         threads.append(t)
 
-        t = threading.Thread(
-            target=write_csv,
-            args=[ekfcsvpath, chemical_ekf_list, "auv_ekf_chemical", csv_ekf_chemical],
-        )
-        t.start()
-        threads.append(t)
-
         for key in payload_dict:
             if "_pf" in key:
                 t = threading.Thread(
                     target=write_csv,
                     args=[
                         pfcsvpath,
                         payload_dict[key],
-                        "auv_" + key,
+                        key,
                         csv_pf_payload,
                     ],
                 )
                 t.start()
                 threads.append(t)
             elif "_ekf" in key:
                 t = threading.Thread(
                     target=write_csv,
                     args=[
                         ekfcsvpath,
                         payload_dict[key],
-                        "auv_" + key,
+                        key,
                         csv_ekf_payload,
                     ],
                 )
                 t.start()
                 threads.append(t)
-            else:
+            else:  # dead reckoning
                 t = threading.Thread(
                     target=write_csv,
                     args=[
                         drcsvpath,
                         payload_dict[key],
-                        "auv_" + key,
+                        key + "_dr",
                         csv_dr_payload,
                     ],
                 )
                 t.start()
                 threads.append(t)
 
         if len(camera1_dr_list) > 0:
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/sensors.py` & `oplab_pipeline-1.1.3/src/auv_nav/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -2110,41 +2110,50 @@
                     "filename": self.right.filename,
                 }
             ],
         }
         return data
 
 
-class Other(SyncedOrientationBodyVelocity):
+class Payload(SyncedOrientationBodyVelocity):
     def __init__(self):
         super().__init__()
         self.data = None
 
     def from_json(self, json):
         self.epoch_timestamp = json["epoch_timestamp"]
         self.data = json["data"]
 
     def get_csv_header(self):
-        str_to_write = super().get_csv_header()
-        # Remove the newline, we will write it later
-        str_to_write = str_to_write.replace("\n", "")
+        str_to_write = (
+            "northing [m],easting [m],depth [m],altitude [m],"
+            "latitude [deg],longitude [deg],"
+        )
         if isinstance(self.data, pd.DataFrame):
-            str_to_write += "," + ",".join(self.data.columns) + "\n"
-        if isinstance(self.data, dict):
-            str_to_write += "," + ",".join(self.data.keys()) + "\n"
+            str_to_write += ",".join(self.data.columns) + "\n"
+        elif isinstance(self.data, dict):
+            str_to_write += ",".join(self.data.keys()) + "\n"
         else:
-            str_to_write = str_to_write.replace("\n", ",data\n")
+            #str_to_write = str_to_write.replace("\n", ",data\n")
+            str_to_write += "data\n"
+
         return str_to_write
 
     def to_csv_row(self):
-        str_to_write = super().to_csv_row()
-        # Remove the newline, we will write it later
-        str_to_write = str_to_write.replace("\n", "")
+        str_to_write = (
+            str(self.northings) + ","
+            + str(self.eastings) + ","
+            + str(self.depth) + ","
+            + str(self.altitude) + ","
+            + str(self.latitude) + ","
+            + str(self.longitude)
+        )
         if isinstance(self.data, pd.DataFrame):
             str_to_write += ",".join(str(self.data.values)) + "\n"
-        if isinstance(self.data, dict):
+        elif isinstance(self.data, dict):
             for value in self.data.values():
                 str_to_write += "," + str(value)
             str_to_write += "\n"
         else:
             str_to_write += "," + str(self.data) + "\n"
+
         return str_to_write
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/body_to_inertial.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/body_to_inertial.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/csv_tools.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/csv_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from auv_nav.sensors import (
     Altitude,
     BodyVelocity,
     Camera,
     Depth,
     Orientation,
-    Other,
+    Payload,
     SyncedOrientationBodyVelocity,
     Tide,
     Usbl,
 )
 from oplab import Console
 
 
@@ -33,15 +33,15 @@
     data_list: Union[
         List[BodyVelocity],
         List[Orientation],
         List[Depth],
         List[Altitude],
         List[Usbl],
         List[Tide],
-        List[Other],
+        List[Payload],
         List[Camera],
         List[SyncedOrientationBodyVelocity],
     ],
     csv_filename: str,
     csv_flag: Optional[bool] = True,
     mutex: Optional[Lock] = None,
 ):
```

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/displayable_path.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/displayable_path.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/dvl_level_arm.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/dvl_level_arm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/graph.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/graph.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/inertial_to_body.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/inertial_to_body.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/interpolate.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/interpolate.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/latlon_wgs84.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/latlon_wgs84.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/time_conversions.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/time_conversions.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/auv_nav/tools/transformations.py` & `oplab_pipeline-1.1.3/src/auv_nav/tools/transformations.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/correct_images.py` & `oplab_pipeline-1.1.3/src/correct_images/correct_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/__init__.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/attenuation.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/attenuation.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/debayer.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/debayer.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/gamma.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/gamma.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/manual_balance.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/manual_balance.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/pixel_stat.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/pixel_stat.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/rescale.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/rescale.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrections/undistort.py` & `oplab_pipeline-1.1.3/src/correct_images/corrections/undistort.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/corrector.py` & `oplab_pipeline-1.1.3/src/correct_images/corrector.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,21 @@
     fname = original_file.name
     dest_file = dest_dir / fname
     original_file.copy(dest_file)
 
 
 class Corrector:
     def __init__(
-        self, mode, force=False, suffix=None, camera=None, correct_config=None, path=None
+        self,
+        mode,
+        force=False,
+        suffix=None,
+        camera=None,
+        correct_config=None,
+        path=None,
     ):
         """Constructor for the Corrector class
 
         Parameters
         ----------
         mode : str
             mode of the corrector. Can be "parse" or "process"
@@ -132,15 +138,15 @@
         # From get image list
         self.altitude_csv_path = None
         self.trimmed_csv_path = None
         self.camera_params_file_path = None
 
         self.memmaps_to_remove = []
 
-        assert(mode in ["parse", "process"])
+        assert mode in ["parse", "process"]
         self.mode = mode
         self.force = force
 
         # if path is None then user must define it externally and call set_path
         if path is not None:
             # Set the path for the corrector
             self.set_path(path)
@@ -192,18 +198,26 @@
         self.correct_config = correct_config
 
         """Load general configuration parameters"""
         self.correction_method = self.correct_config.method
         # if self.correction_method == "colour_correction":
         self.distance_metric = self.correct_config.color_correction.distance_metric
         self.distance_path = self.correct_config.color_correction.metric_path
-        self.parse_altitude_min = self.correct_config.color_correction.parse_altitude_min
-        self.parse_altitude_max = self.correct_config.color_correction.parse_altitude_max
-        self.process_altitude_min = self.correct_config.color_correction.process_altitude_min
-        self.process_altitude_max = self.correct_config.color_correction.process_altitude_max
+        self.parse_altitude_min = (
+            self.correct_config.color_correction.parse_altitude_min
+        )
+        self.parse_altitude_max = (
+            self.correct_config.color_correction.parse_altitude_max
+        )
+        self.process_altitude_min = (
+            self.correct_config.color_correction.process_altitude_min
+        )
+        self.process_altitude_max = (
+            self.correct_config.color_correction.process_altitude_max
+        )
         self.smoothing = self.correct_config.color_correction.smoothing
         self.window_size = self.correct_config.color_correction.window_size
         self.cameraconfigs = self.correct_config.configs.camera_configs
         self.undistort = self.correct_config.output_settings.undistort_flag
         self.output_format = self.correct_config.output_settings.compression_parameter
 
         # Load camera parameters
@@ -282,15 +296,18 @@
             self.load_configuration(correct_config)  # load the dive config
             # Set the user specified list - if any
             self.user_specified_image_list = self.user_specified_image_list_parse
             # Update list of images by appending user-defined list
             # TODO: this list must be populated from AFTER loading the configuration and BEFORE getting image list
             self.get_imagelist("parse")
 
-        if len(self.altitude_list) < 3 and self.correction_method == "colour_correction":
+        if (
+            len(self.altitude_list) < 3
+            and self.correction_method == "colour_correction"
+        ):
             Console.quit(
                 "Insufficient number of images to compute attenuation",
                 "parameters",
             )
 
         # Show the total number of images after filtering + merging the dives. It should match the sum of the filtered images of each dive.
         if len(path_list) > 1:
@@ -500,15 +517,15 @@
         self.altitude_list = []
 
         # If using colour_correction, we need to read in the navigation
         if (
             self.correction_method == "colour_correction"
             or self.camera.extension == "bag"
         ):
-            assert(mode in ["parse", "process"])
+            assert mode in ["parse", "process"]
             if mode == "parse":
                 altitude_min = self.parse_altitude_min
                 altitude_max = self.parse_altitude_max
             elif mode == "process":
                 altitude_min = self.process_altitude_min
                 altitude_max = self.process_altitude_max
 
@@ -546,15 +563,15 @@
             self.altitude_csv_path = full_metric_path / metric_file
 
             # Check if file exists
             if not self.altitude_csv_path.exists():
                 Console.quit(
                     "Cannot find altitude csv file expected to be save at ",
                     self.altitude_csv_path,
-                    ". Run auv_nav first."
+                    ". Run auv_nav first.",
                 )
 
             # read dataframe for corresponding distance csv path
             dataframe = pd.read_csv(self.altitude_csv_path)
 
             # get imagelist for given camera object
             if self.user_specified_image_list != "none":
@@ -621,17 +638,17 @@
                 )
                 Console.error("You may need to reprocess the dive with auv_nav")
                 Console.quit("No images were found.")
 
             # WARNING: what happens in a multidive setup when the current dive has no images (but the rest of the dive does)?
             Console.info(
                 len(self.altitude_list),
-                "/",
+                "of",
                 len(distance_list),
-                "Images filtered as per altitude range...",
+                "images remaining after applying altitude filter",
             )
         else:
             # Copy the images list from the camera
             self.camera_image_list = self.camera.image_list
 
             # Join the current image list with the original image list (copy)
             self.camera_image_list.extend(_original_image_list)
@@ -651,49 +668,46 @@
             self.depth_map_list = []
             return
         elif self.distance_metric == "altitude":
             Console.info("Null distance matrix created")
             self.depth_map_list = []
             return
         elif self.distance_metric == "depth_map":
-            path_depth = self.path_processed / "depth_map"
+            # Load depth maps
+            path_depth = self.path_processed / "3d_reconstruction" / "depth_maps"
             if not path_depth.exists():
                 Console.quit(
-                    "Depth maps folder", path_depth, "does not exist. Aborting..."
+                    "Depth maps folder", path_depth, "does not exist."
                 )
-            else:
-                Console.info("Path to depth maps found...")
-                depth_map_list = list(path_depth.glob("*map.npy"))
-                self.depth_map_list = []
-                images_to_drop = []
-                for img_idx, image_path in enumerate(self.camera_image_list):
-                    dm_found = False
-                    for item in depth_map_list:
-                        if Path(image_path).stem in Path(item).stem:
-                            self.depth_map_list.append(Path(item))
-                            dm_found = True
-                            break
-                    if not dm_found:
-                        # Drop that image - its depth map is missing
-                        images_to_drop.append(img_idx)
-                # Drop the images that do not have a depth map
-                if len(images_to_drop) > 0:
-                    Console.info(
-                        "Dropped images without depth map:", len(images_to_drop)
-                    )
-                    for idx in sorted(images_to_drop, reverse=True):
-                        del self.camera_image_list[idx]
-
-                Console.info("...done generating depth_map_list")
+            images_to_drop = []
+            for img_idx, image_path in enumerate(self.camera_image_list):
+                p = path_depth / os.path.relpath(image_path, self.path_raw)
+                p = p.with_name(p.stem + "_depthmap.npy")
+                if p.exists():
+                    self.depth_map_list.append(p)
+                else:
+                    images_to_drop.append(img_idx)
 
-                if len(self.camera_image_list) != len(self.depth_map_list):
+            # Drop images that do not have a corresponding depth map
+            if len(images_to_drop) > 0:
+                if len(images_to_drop) == len(self.camera_image_list):
                     Console.quit(
-                        f"The number of images ({len(self.camera_image_list)})",
-                        f"is different from the number of depth maps ({len(self.depth_map_list)}).",
+                        "No depth maps found in", path_depth,
+                        "\nLast path checked:", p
                     )
+                Console.info(
+                    "Dropping", len(images_to_drop), "of", len(self.camera_image_list),
+                    "images for which no depth maps exists."
+                )
+                for idx in sorted(images_to_drop, reverse=True):
+                    del self.camera_image_list[idx]
+            assert(len(self.camera_image_list) == len(self.depth_map_list))
+
+            Console.info("Depth maps loaded")
+            return
 
     # compute correction parameters either for attenuation correction or
     # static correction of images
     def generate_attenuation_correction_parameters(self):
         """Generates image stats and attenuation coefficients and saves the
         parameters for process"""
 
@@ -740,15 +754,15 @@
         max_bin_size_gb = 50.0
         max_bin_size = int(max_bin_size_gb / image_size_gb)
 
         self.bin_band = 0.1
         hist_bins = np.arange(
             self.parse_altitude_min,
             self.parse_altitude_max + 0.5 * self.bin_band,
-            self.bin_band
+            self.bin_band,
         )
 
         distance_vector = None
 
         if self.depth_map_list and self.distance_metric == "depth_map":
             Console.info("Computing depth map histogram with", hist_bins.size, "bins")
 
@@ -799,15 +813,15 @@
 
             with tqdm_joblib(
                 tqdm(
                     desc="Computing altitude histogram",
                     total=hist_bins.size - 1,
                 )
             ):
-                joblib.Parallel(n_jobs=-2, verbose=0)( 
+                joblib.Parallel(n_jobs=-2, verbose=0)(
                     # Do not prefer="threads" as in certain cases this can cause the
                     # program to crash when calling plt.imshow() in compute_distance_bin
                     joblib.delayed(self.compute_distance_bin)(
                         idxs,
                         idx_bin,
                         images_map,
                         distances_map,
@@ -1214,17 +1228,15 @@
             len(self.camera_image_list),
             "images for color, distortion, gamma corrections...",
         )
 
         with tqdm_joblib(
             tqdm(desc="Correcting images", total=len(self.camera_image_list))
         ):
-            self.processed_image_list = joblib.Parallel(
-                n_jobs=-2, verbose=0
-            )(
+            self.processed_image_list = joblib.Parallel(n_jobs=-2, verbose=0)(
                 joblib.delayed(self.process_image)(idx)
                 for idx in range(0, len(self.camera_image_list))
             )
 
         # write a filelist.csv containing image filenames and navigation
         image_names = []
         for path in self.processed_image_list:
```

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/acfr/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/acfr/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/biocam4000_15c/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/hybis/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/hybis/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/ntnu_stereo/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/rosbag/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/rosbag/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/stereo_gopro/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/default_yaml/sx3/correct_images.yaml` & `oplab_pipeline-1.1.3/src/correct_images/default_yaml/sx3/correct_images.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/loaders/default.py` & `oplab_pipeline-1.1.3/src/correct_images/loaders/default.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/loaders/depth_map.py` & `oplab_pipeline-1.1.3/src/correct_images/loaders/depth_map.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/loaders/loader.py` & `oplab_pipeline-1.1.3/src/correct_images/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/loaders/rosbag.py` & `oplab_pipeline-1.1.3/src/correct_images/loaders/rosbag.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/loaders/xviii.py` & `oplab_pipeline-1.1.3/src/correct_images/loaders/xviii.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/parser.py` & `oplab_pipeline-1.1.3/src/correct_images/parser.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/tools/curve_fitting.py` & `oplab_pipeline-1.1.3/src/correct_images/tools/curve_fitting.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/tools/file_handlers.py` & `oplab_pipeline-1.1.3/src/correct_images/tools/file_handlers.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/tools/joblib_tqdm.py` & `oplab_pipeline-1.1.3/src/correct_images/tools/joblib_tqdm.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/tools/memmap.py` & `oplab_pipeline-1.1.3/src/correct_images/tools/memmap.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/correct_images/tools/numerical.py` & `oplab_pipeline-1.1.3/src/correct_images/tools/numerical.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/__init__.py` & `oplab_pipeline-1.1.3/src/oplab/__init__.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/camera_models.py` & `oplab_pipeline-1.1.3/src/oplab/camera_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     @property
     def aspect_ratio(self):
         return float(self.image_width) / float(self.image_height)
 
     @property
     def rectification_maps(self):
         mapx, mapy = cv2.initUndistortRectifyMap(
-            self.intrinsics,
-            self.distortion,
+            self.K,
+            self.d,
             self.R,
             self.P,
             self.size,
             cv2.CV_32FC1,
         )
         return mapx, mapy
```

### Comparing `oplab_pipeline-1.1.0/src/oplab/camera_system.py` & `oplab_pipeline-1.1.3/src/oplab/camera_system.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/console.py` & `oplab_pipeline-1.1.3/src/oplab/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,8 +287,10 @@
         )
         fh.setFormatter(formatter)
         logger = logging.getLogger()
         logger.setLevel(logging.DEBUG)
         fh.setLevel(logging.DEBUG)  # or any level you want
         logger.addHandler(fh)
         if logger is not None:
-            logger.info("oplab_pipeline version: " + str(Console.get_version()))
+            logger.info("oplab_pipeline version: " + Console.get_version())
+            logger.info("User: " + Console.get_username())
+            logger.info("Hostname: " + Console.get_hostname())
```

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/ae2000/YK17-23C/vehicle.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,16 @@
   surge_m: 0.150375 # 0.147875
   sway_m: 0
   heave_m: 0.514
   roll_deg: 0
   pitch_deg: 0
   yaw_deg: 0
 
-chemical:
-  surge_m: 0.4
-  sway_m: 0
-  heave_m: -0.5
-  roll_deg: 0
-  pitch_deg: 0
-  yaw_deg: 0
+
+payloads:
+  payload_0:
+    surge_m: 0.4
+    sway_m: 0
+    heave_m: -0.5
+    roll_deg: 0
+    pitch_deg: 0
+    yaw_deg: 0
```

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/camera.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/camera.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/mission.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/as6/DY109/vehicle.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/as6/DY109/vehicle.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/ts1/SSK17-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml` & `oplab_pipeline-1.1.3/src/oplab/default_yaml/ts2/SSK16-01/mission.yaml`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/filename_to_date.py` & `oplab_pipeline-1.1.3/src/oplab/filename_to_date.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/oplab/folder_structure.py` & `oplab_pipeline-1.1.3/src/oplab/folder_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,11 +132,11 @@
             p.unlink()
     folder.rmdir()
 
 
 def _copy(self, target):
     if not target.parent.exists():
         target.parent.mkdir(exist_ok=True, parents=True)
-    shutil.copy(str(self), str(target))  # str() only there for Python < (3, 6)
+    shutil.copyfile(str(self), str(target))  # str() only there for Python < (3, 6)
 
 
 Path.copy = _copy
```

### Comparing `oplab_pipeline-1.1.0/src/oplab/mission.py` & `oplab_pipeline-1.1.3/src/oplab/mission.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         node["longitude"] = self.longitude
         node["coordinate_reference_system"] = self.crs
         node["date"] = self.date
 
 
 class CameraEntry:
     def __init__(self, node=None):
+        self.name = None
         self.records_laser = False
         self.origin = None
         self.type = None
         self.path = None
         self.timeoffset = None
         if node is not None:
             self.name = node["name"]
@@ -104,16 +105,17 @@
         if hasattr(self, "timeoffset"):
             node["timeoffset"] = self.timeoffset
 
 
 class TimeZoneEntry:
     def __init__(self):
         self.timezone = 0
-        self.timeoffset = 0
+        self.offset_s = 0
         self.timeoffset_s = 0
+        self.timezone_s = 0
 
     def load(self, node):
         self.timezone = node.get("timezone", 0)
         # read in timezone
         if isinstance(self.timezone, str):
             if self.timezone == "utc" or self.timezone == "UTC":
                 self.timezone = 0
@@ -129,20 +131,21 @@
                         "Error: timezone",
                         self.timezone,
                         "in mission.yaml not recognised,",
                         " please enter value from UTC in",
                         " hours",
                     )
 
-        self.timeoffset = node.get("timeoffset", 0)
-        self.timeoffset_s = +self.timezone * 60 * 60 + self.timeoffset
+        self.timeoffset_s = node.get("timeoffset", 0)
+        self.timezone_s = self.timezone * 60 * 60
+        self.offset_s = self.timezone_s + self.timeoffset_s
 
     def write(self, node):
         node["timezone"] = self.timezone
-        node["timeoffset"] = self.timeoffset
+        node["timeoffset"] = self.timeoffset_s
 
 
 class PayloadEntry(TimeZoneEntry):
     def __init__(self):
         super().__init__()
         self.path = ""
         self.format = ""
@@ -169,19 +172,19 @@
         self.cameras = []
         self.calibration = None
         self._empty = True
 
     def empty(self):
         return self._empty
 
-    def load(self, node, version=1):
+    def load(self, node, mission_yaml_version=1):
         super().load(node)
         self.format = node["format"]
         self._empty = False
-        if version == 1 or version == 2:
+        if mission_yaml_version >= 1:
             for camera in node["cameras"]:
                 self.cameras.append(CameraEntry(camera))
             if "origin" not in node["cameras"][0]:
                 # Assuming that the camera names in mission.yaml corresponds
                 # to the frame names in vehicle.yaml
                 for i, camera in enumerate(self.cameras):
                     camera.origin = camera.name
@@ -272,34 +275,14 @@
         node["filepath"] = self.filepath
         node["filename"] = self.filename
         node["label"] = self.label
         node["id"] = self.label
         node["std_factor"] = self.std_factor
         node["std_offset"] = self.std_offset
 
-    def get_offset_s(self):
-        if isinstance(self.timezone, str):
-            if self.timezone == "utc" or self.timezone == "UTC":
-                self.timezone_offset = 0
-            elif self.timezone == "jst" or self.timezone == "JST":
-                self.timezone_offset = 9
-        else:
-            try:
-                self.timezone_offset = float(self.timezone)
-            except ValueError:
-                print(
-                    "Error: timezone",
-                    self.timezone,
-                    "in mission.yaml not recognised, ",
-                    "please enter value from UTC in hours",
-                )
-                return
-            timeoffset = -self.timezone_offset * 60 * 60 + self.timeoffset
-            return timeoffset
-
 
 class Mission:
     """Mission class that parses and writes mission.yaml"""
 
     def __init__(self, filename=None):
         self.version = 0
         self.origin = OriginEntry()
@@ -406,19 +389,25 @@
                 if "dead_reckoning" in data:
                     self.dead_reckoning.load(data["dead_reckoning"])
 
                 if "image" in data:
                     self.image.load(data["image"], self.version)
                     for camera in self.image.cameras:
                         if camera.origin not in vehicle_data:
-                            Console.error(
-                                "The camera mounted at "
-                                + camera.origin
-                                + " does not correspond to any frame in vehicle.yaml."  # noqa
-                            )
+                            if camera.name:
+                                Console.error(
+                                    "The camera "
+                                    + camera.name
+                                    + " does not correspond to any frame in vehicle.yaml."  # noqa
+                                )
+                            else:
+                                Console.error(
+                                    "The image node in the mission.yaml file does not "
+                                    "seem to be valid."  # noqa
+                                )
                             error_and_exit()
 
                 if "payloads" in data:
                     for payload_entry in data["payloads"]:
                         payload = PayloadEntry()
                         payload.load(data["payloads"][payload_entry])
                         self.payloads[payload_entry] = payload
```

### Comparing `oplab_pipeline-1.1.0/src/oplab/vehicle.py` & `oplab_pipeline-1.1.3/src/oplab/vehicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-Copyright (c) 2020, University of Southampton
+Copyright (c) 2023, University of Southampton
 All rights reserved.
 Licensed under the BSD 3-Clause License.
 See LICENSE.md file in the project root for full license information.
 """
 
 # Workaround to dump OrderedDict into YAML files
 from collections import OrderedDict
@@ -90,15 +90,14 @@
         self.ins = SensorOffset()
         self.dvl = SensorOffset()
         self.depth = SensorOffset()
         self.usbl = SensorOffset()
         self.camera1 = SensorOffset()
         self.camera2 = SensorOffset()
         self.camera3 = SensorOffset()
-        self.chemical = SensorOffset()
         self.payloads = {}
 
         if filename is None:
             return
 
         self.filename = filename
 
@@ -188,15 +187,18 @@
                         )
                         Console.quit(
                             "Your vehicle.yaml or your mission.yaml are ",
                             "malformed.",
                         )
                     self.camera3.load(self.data[camera_name])
                 if "chemical" in self.data:
-                    self.chemical.load(self.data["chemical"])
+                    Console.warn(
+                        "The node \"chemical\" is deprecated. "
+                        "Please define a payload instead."
+                    )
                 if "payloads" in self.data:
                     for payload_name in self.data["payloads"]:
                         payload = SensorOffset()
                         payload.load(self.data["payloads"][payload_name])
                         self.payloads[payload_name] = payload
         except FileNotFoundError:
             Console.error("The file vehicle.yaml could not be found at the location:")
```

### Comparing `oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/PKG-INFO` & `oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oplab-pipeline
-Version: 1.1.0
+Version: 1.1.3
 Summary: Toolchain for AUV dive processing, camera calibration and image correction
 Home-page: https://github.com/ocean-perception/oplab_pipeline
 Author: Ocean Perception - University of Southampton
 Author-email: miquel.massot-campos@soton.ac.uk
 License: BSD
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![oplab_pipeline](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/oplab_pipeline.yml/badge.svg)](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/oplab_pipeline.yml) [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa] [![Code Coverage](https://codecov.io/gh/ocean-perception/oplab_pipeline/branch/master/graph/badge.svg?token=PJBfl6qhp5)](https://codecov.io/gh/ocean-perception/oplab_pipeline) [![Documentation Status](https://readthedocs.org/projects/oplab-pipeline/badge/?version=latest)](https://oplab-pipeline.readthedocs.io/en/latest/?badge=latest) [![Docker Image CI](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/docker_image.yml/badge.svg)](https://github.com/ocean-perception/oplab_pipeline/actions/workflows/docker_image.yml) [![DOI](https://zenodo.org/badge/101513536.svg)](https://zenodo.org/badge/latestdoi/101513536)
 
 
 
 # oplab_pipeline
```

### Comparing `oplab_pipeline-1.1.0/src/oplab_pipeline.egg-info/SOURCES.txt` & `oplab_pipeline-1.1.3/src/oplab_pipeline.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 src/auv_nav/default_yaml/auv_nav.yaml
 src/auv_nav/default_yaml/ae2000/YK17-23C/camera.yaml
 src/auv_nav/default_yaml/ae2000/YK17-23C/mission.yaml
 src/auv_nav/default_yaml/ae2000/YK17-23C/vehicle.yaml
 src/auv_nav/default_yaml/alr/dy152/camera.yaml
 src/auv_nav/default_yaml/alr/dy152/mission.yaml
 src/auv_nav/default_yaml/alr/dy152/vehicle.yaml
+src/auv_nav/default_yaml/alr/insite/camera.yaml
+src/auv_nav/default_yaml/alr/insite/mission.yaml
+src/auv_nav/default_yaml/alr/insite/vehicle.yaml
 src/auv_nav/default_yaml/alr/jc220/camera.yaml
 src/auv_nav/default_yaml/as6/DY109/camera.yaml
 src/auv_nav/default_yaml/as6/DY109/mission.yaml
 src/auv_nav/default_yaml/as6/DY109/vehicle.yaml
 src/auv_nav/default_yaml/hybis/camera.yaml
 src/auv_nav/default_yaml/hybis/mission.yaml
 src/auv_nav/default_yaml/hybis/vehicle.yaml
```

### Comparing `oplab_pipeline-1.1.0/src/scripts/auv_cd.sh` & `oplab_pipeline-1.1.3/src/scripts/auv_cd.sh`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/scripts/debayer_folder.py` & `oplab_pipeline-1.1.3/src/scripts/debayer_folder.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/scripts/extract_rosbag_images.py` & `oplab_pipeline-1.1.3/src/scripts/extract_rosbag_images.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/scripts/merge_dataset_csv.py` & `oplab_pipeline-1.1.3/src/scripts/merge_dataset_csv.py`

 * *Files identical despite different names*

### Comparing `oplab_pipeline-1.1.0/src/scripts/pixel_stats_folder.py` & `oplab_pipeline-1.1.3/src/scripts/pixel_stats_folder.py`

 * *Files identical despite different names*

