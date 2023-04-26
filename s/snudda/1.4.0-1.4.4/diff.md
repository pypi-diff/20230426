# Comparing `tmp/snudda-1.4.0.tar.gz` & `tmp/snudda-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snudda-1.4.0.tar", last modified: Wed Feb 15 16:16:22 2023, max compression
+gzip compressed data, was "snudda-1.4.4.tar", last modified: Wed Apr 26 08:34:26 2023, max compression
```

## Comparing `snudda-1.4.0.tar` & `snudda-1.4.4.tar`

### file list

```diff
@@ -1,540 +1,483 @@
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.721953 snudda-1.4.0/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-1.4.0/LICENSE
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-02-15 16:16:22.721953 snudda-1.4.0/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3711 2022-09-19 09:45:08.000000 snudda-1.4.0/README.md
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2023-02-15 16:16:22.721953 snudda-1.4.0/setup.cfg
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2535 2022-11-04 18:40:55.000000 snudda-1.4.0/setup.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.613957 snudda-1.4.0/snudda/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.617956 snudda-1.4.0/snudda/analyse/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/analyse/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   106766 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/analyse/analyse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7923 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/analyse/analyse_gap_junction_coupling.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3251 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/analyse/analyse_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/analyse/analyse_neuroinformatics2020.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5505 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/analyse/analyse_spike_trains.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18255 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/analyse/analyse_striatum.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2996 2022-10-07 09:01:39.000000 snudda-1.4.0/snudda/analyse/analyse_synapse_location.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7574 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/analyse/analyse_topology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12378 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/analyse/analyse_topology_activity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11030 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/cli.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    29253 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/core.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.613957 snudda-1.4.0/snudda/data/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/InputAxons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.617956 snudda-1.4.0/snudda/data/InputAxons/Cortex/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Cortex/AA0059.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.617956 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.617956 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.621956 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.621956 snudda-1.4.0/snudda/data/InputAxons/GPe2Striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1169 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.625956 snudda-1.4.0/snudda/data/InputAxons/Thalamus/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Thalamus/AA0054.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.625956 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg10/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.625956 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg15/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.625956 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg5/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.629956 snudda-1.4.0/snudda/data/density/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/1001_STRd_Sst_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/252_STRd_Chat_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/252_STRd_Chat_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/352_STRd_Drd1_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/72109410_STRd_Adora2a_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/79556738_STRd_Pvalb_dens.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/combine_densities.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/density/dorsal_striatum_density.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/experiment_config/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.633956 snudda-1.4.0/snudda/data/experiment_config/pair_recording/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      469 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      583 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      635 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      636 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-5.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      595 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-6.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      693 2022-11-11 14:42:41.000000 snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-7.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.633956 snudda-1.4.0/snudda/data/images/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/images/snudda-video-qr-code.png
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.637956 snudda-1.4.0/snudda/data/input_config/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v3.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v4.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-ChIN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-Channel-Activation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-channel-1.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-channel-2.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-v7.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-v8.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5639 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/input_config/input-v10-scaled.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.645955 snudda-1.4.0/snudda/data/mesh/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/GPe.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/GPi.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/SNc.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/SNr.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/STN.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/Striatum-d.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/Striatum-v.obj
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/mesh/get_mesh.ipynb
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/neurons/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.653955 snudda-1.4.0/snudda/data/neurons/mechanisms/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/NO.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3829 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4032 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3836 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2385 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3393 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/concACh.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/concDA.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/concDAfile.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1795 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/hd_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2306 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2065 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2944 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3577 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2872 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3463 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1321 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kdr_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1322 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kdrbca1_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2544 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kir23_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1270 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3123 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3459 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2332 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2985 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3359 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/na3n_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2798 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2371 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2441 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/naf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2560 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3463 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6516 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6386 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6874 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut_double.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.657955 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/h_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.665955 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2629 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/#na_ch.mod#
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/Kv3_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3140 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/M4.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/NO.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/bk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/bk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/bk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/ca_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cadyn_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cadyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3840 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal12_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3844 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal12_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4043 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal13_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4047 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal13_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/caldyn_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/can_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3847 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/can_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3851 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/can_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2398 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cap_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/caq_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/caq_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/car_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3404 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/car_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3408 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/car_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cat32_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cat33_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/concACh.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/concDA.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/concDAfile.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3433 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/hcn12_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/hd_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2306 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/im_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2065 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/it_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2955 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kaf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3583 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kaf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3587 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kaf_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2883 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kas_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3474 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kas_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3478 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kas_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kcnq_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kdr_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1321 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kdr_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kdr_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2544 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir23_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2696 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir23_lts_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1290 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3134 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3470 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3474 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kir_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kv2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2353 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kv4_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3005 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/na2_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3375 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/na3n_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2818 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/na_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2382 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2441 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_lts.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2582 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_lts_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2581 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2585 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_ms_mod.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/par_ggap.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/sk_ch.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/sk_fs.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/sk_ms.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/tmampa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3463 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/tmgabaa.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6516 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/tmglut.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/tmnmda.mod
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/vecevent.mod
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.613957 snudda-1.4.0/snudda/data/neurons/striatum/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/neurons/striatum/chin/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.665955 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/neurons/striatum/dspn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.669955 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.669955 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.669955 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.673955 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/neurons/striatum/fs/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.673955 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.681954 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.685954 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.689954 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.609957 snudda-1.4.0/snudda/data/neurons/striatum/ispn/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.689954 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.693954 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.693954 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.693954 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.613957 snudda-1.4.0/snudda/data/neurons/striatum/lts/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.693954 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.693954 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3907 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.697954 snudda-1.4.0/snudda/data/synapses/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.697954 snudda-1.4.0/snudda/data/synapses/example_data/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/formatinfo.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/pair_pulse_experiment_data.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.701954 snudda-1.4.0/snudda/data/synapses/striatum/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.701954 snudda-1.4.0/snudda/data/synapses/striatum/partial/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      307 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/striatum/readme.txt
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.705953 snudda-1.4.0/snudda/data/synapses/v1/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.705953 snudda-1.4.0/snudda/detect/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/detect/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   155852 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/detect/detect.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16515 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/detect/project.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15527 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/detect/projection_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)   102725 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/detect/prune.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/help.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.705953 snudda-1.4.0/snudda/init/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       40 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/init/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77833 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/init/init.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/init/init_custom.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/init/init_wojtek.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.709953 snudda-1.4.0/snudda/input/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/input/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97553 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/input/input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    47318 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/input/input_tuning.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/input/inspectinput.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5135 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/input/time_varying_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/input/virtual_input.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.709953 snudda-1.4.0/snudda/neuromodulation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neuromodulation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neuromodulation/modulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neuromodulation/modulation_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neuromodulation/modulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neuromodulation/neuromodulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21645 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neuromodulation/neuromodulation_synapse.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neuromodulation/translator.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.709953 snudda-1.4.0/snudda/neurons/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/neurons/index_tree.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32364 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/morphology_data.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18302 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/neuron_model_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/neuron_morphology.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22960 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/neuron_morphology_extended.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21962 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/neurons/neuron_prototype.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.709953 snudda-1.4.0/snudda/place/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/place/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/place/create_cube_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/place/create_slice_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    57171 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/place/place.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4611 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/place/projection_map_finder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54892 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/place/region_mesh.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7972 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/place/rotation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/place/volumetric_mapping.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.713953 snudda-1.4.0/snudda/plotting/
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.713953 snudda-1.4.0/snudda/plotting/Blender/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.713953 snudda-1.4.0/snudda/plotting/Blender/io_mesh_swc/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/io_mesh_swc/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.713953 snudda-1.4.0/snudda/plotting/Blender/visualisation/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/makeNeuronCube.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22786 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_network_old.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      381 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/plotting/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plotLTSdensity.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/plotting/plot_cross_correlogram.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2524 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/plotting/plot_degeneration.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2022-10-07 09:01:39.000000 snudda-1.4.0/snudda/plotting/plot_degeneration_and_growth.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1279 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plot_density.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2779 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plot_density_slice.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/plotting/plot_distance_statistics.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5309 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/plotting/plot_input.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    14861 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/plotting/plot_input_locations.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11861 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/plotting/plot_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plot_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plot_node_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8024 2022-11-04 18:40:55.000000 snudda-1.4.0/snudda/plotting/plot_period_experiment.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/plotting/plot_size_benchmark.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22560 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/plotting/plot_spike_raster_v2.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18674 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/plotting/plot_traces.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.713953 snudda-1.4.0/snudda/prune/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/prune/__init__.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.717953 snudda-1.4.0/snudda/simulate/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/simulate/__init__.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24795 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/simulate/model_current_injections.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/simulate/network_pair_pulse_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/simulate/nrn_simulator_parallel.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22967 2022-11-11 14:42:41.000000 snudda-1.4.0/snudda/simulate/pair_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13157 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/simulate/save_network_recording.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    81843 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/simulate/simulate.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.721953 snudda-1.4.0/snudda/utils/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/__init__.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22026 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/ablate_network.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4842 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/benchmark_logging.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1237 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/cleanup.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2533 2022-11-03 09:16:18.000000 snudda-1.4.0/snudda/utils/clone_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    20576 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/conv_hurt.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/create_parameter_morphology_input_map.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17299 2022-11-11 14:42:41.000000 snudda-1.4.0/snudda/utils/cut.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     3728 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/export_connection_matrix.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     1708 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/export_eroded_connection_matrix.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38634 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/export_sonata.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2310 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/fake_load.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/input_helper.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    48684 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/load.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    15170 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/load_network_simulation.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/memory.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6298 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/merge_synapse_files.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/numpy_encoder.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/pip_upgrade.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3919 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/reposition_neurons.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4840 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/snudda_path.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38349 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/swap_to_degenerated_morphologies.py
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19222 2023-02-15 16:15:38.000000 snudda-1.4.0/snudda/utils/swap_to_degenerated_morphologies_extended.py
--rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     1916 2022-09-19 09:45:08.000000 snudda-1.4.0/snudda/utils/upgrade_old_network_file.py
-drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-02-15 16:16:22.613957 snudda-1.4.0/snudda.egg-info/
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/PKG-INFO
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)    26346 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/SOURCES.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/dependency_links.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/entry_points.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)      197 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/requires.txt
--rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2023-02-15 16:16:22.000000 snudda-1.4.0/snudda.egg-info/top_level.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.348803 snudda-1.4.4/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2022-09-19 09:45:08.000000 snudda-1.4.4/LICENSE
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-04-26 08:34:26.348803 snudda-1.4.4/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3711 2022-09-19 09:45:08.000000 snudda-1.4.4/README.md
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       38 2023-04-26 08:34:26.348803 snudda-1.4.4/setup.cfg
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2677 2023-04-26 08:33:58.000000 snudda-1.4.4/setup.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/analyse/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      199 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   107778 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7923 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_gap_junction_coupling.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3251 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/analyse/analyse_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5575 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/analyse/analyse_neuroinformatics2020.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8650 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse_spike_trains.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18255 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/analyse/analyse_striatum.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2996 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/analyse_synapse_location.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7574 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_topology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12378 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/analyse/analyse_topology_activity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6277 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/analyse/spike_time_tiling_coefficient.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11585 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/cli.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    29470 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/core.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/InputAxons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/data/InputAxons/Cortex/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   432939 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/AA0059.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.256802 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   900524 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.260803 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   597398 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.260803 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1809577 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1269 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   444324 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   464916 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/AA0054.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   513478 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   346069 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.264803 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1022637 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.272802 snudda-1.4.4/snudda/data/density/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    87096 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    74510 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77158 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94468 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95346 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    95932 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    96454 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77578 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    79756 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1132 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/combine_densities.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  2256264 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/density/dorsal_striatum_density.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/experiment_config/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/experiment_config/pair_recording/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      469 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      583 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      635 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      636 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      455 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-5.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      595 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-6.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      693 2022-11-11 14:42:41.000000 snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-7.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/images/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    52659 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/images/snudda-video-qr-code.png
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.276803 snudda-1.4.4/snudda/data/input_config/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3b.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5834 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5811 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5843 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      768 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-ChIN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1831 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-Channel-Activation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-1.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1803 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-2.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5395 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v7.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5409 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v8.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5547 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-tinytest-v9-freq-vectors.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5639 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/input_config/input-v10-scaled.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      506 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/input_config/input_output_dspn_template_IC.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.284803 snudda-1.4.4/snudda/data/mesh/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   192511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/GPe.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    60912 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/GPi.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    68536 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/SNc.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   164445 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/SNr.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    44005 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/STN.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1069021 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-d.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1733004 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1813629 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   763087 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/Striatum-v.obj
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2358 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/mesh/get_mesh.ipynb
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/nest/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.284803 snudda-1.4.4/snudda/data/nest/models/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      272 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      276 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/nest/models/iSPN.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.288802 snudda-1.4.4/snudda/data/neurons/mechanisms/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2111 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/Im_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1375 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/NO.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2598 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4351 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4561 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4723 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2871 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4517 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2986 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3855 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1074 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concACh.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1084 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concDA.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      907 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/concDAfile.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3903 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2247 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/hd_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3028 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3099 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3406 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3407 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4335 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3334 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3932 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1179 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2810 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kdrb_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3594 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3595 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1665 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3586 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4151 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3111 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3677 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na3_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3119 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2833 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3043 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3245 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4291 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7671 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7535 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8029 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_double.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.296803 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1352 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2225 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2511 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2744 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3998 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/ca_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1609 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3249 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3452 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1800 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1663 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3256 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1686 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cap_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2424 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2485 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2814 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2413 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1164 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/h_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2855 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1724 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/im_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2061 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/it_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2364 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2993 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2292 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2886 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1189 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1781 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1250 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      605 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2543 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2882 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1254 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1642 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2082 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na2_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2637 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2076 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1791 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/par_ggap.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1909 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ch.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_fs.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1896 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ms.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2370 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmampa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2893 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5773 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmglut.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1336 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmnmda.mod
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1026 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/vecevent.mod
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/chin/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.296803 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      215 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    89390 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69404 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3194 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      403 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/dspn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   673225 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      936 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92361 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    94239 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    80017 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   600711 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59991 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.300803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   183549 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59972 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.304803 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   660197 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    92630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    99934 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/fs/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.304803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21438 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.312803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  4918863 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19567 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.316803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   620377 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5366 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.320803 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   826139 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      244 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1226312 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5354 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/ispn/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.320803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1013802 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    69979 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)  1153456 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59905 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   587827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    49989 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.324803 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   254041 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      643 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    59125 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    29994 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda/data/neurons/striatum/lts/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      582 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/mechanisms.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    32177 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19983 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3895 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      406 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/protocols.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/synapses/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.328803 snudda-1.4.4/snudda/data/synapses/example_data/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   127486 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      644 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/example_data/M1LH-contra_dSPN.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1623 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/formatinfo.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/pair_pulse_experiment_data.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.332803 snudda-1.4.4/snudda/data/synapses/striatum/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15242 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3494 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    50601 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8102 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18630 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11632 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    97843 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39622 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39725 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39455 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39599 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    39624 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3535 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    28148 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2277 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   140662 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19848 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12939 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   109072 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.332803 snudda-1.4.4/snudda/data/synapses/striatum/partial/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1092 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1079 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3255 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4345 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8626 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5339 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1093 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      413 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/data/synapses/striatum/readme.txt
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/data/synapses/v1/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9657 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3482 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7077 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8386 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13748 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    12464 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13368 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8270 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19238 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8345 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11827 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11864 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16683 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9737 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15282 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    17464 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      751 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      738 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2213 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2943 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5839 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3600 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/detect/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      138 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/detect/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   157811 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/detect/detect.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    16515 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/detect/project.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15527 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/detect/projection_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)   103112 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/detect/prune.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      801 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/help.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/init/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       40 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    77893 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/init/init.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3141 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/init_custom.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2308 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/init/init_wojtek.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/input/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       95 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/input/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    98298 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/input/input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    47318 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/input_tuning.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2809 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/inspectinput.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5135 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/input/time_varying_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1088 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/input/virtual_input.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/neuromodulation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      177 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2679 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7470 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4495 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/modulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7179 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neuromodulation/neuromodulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21645 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neuromodulation/neuromodulation_synapse.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      289 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neuromodulation/translator.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.336803 snudda-1.4.4/snudda/neurons/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      203 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1617 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/neurons/index_tree.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    34255 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/neurons/morphology_data.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18302 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_model_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54245 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_morphology.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    23275 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/neurons/neuron_morphology_extended.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    21962 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/neurons/neuron_prototype.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/place/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      258 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2747 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/create_cube_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3196 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/create_slice_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    57441 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/place/place.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4611 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/projection_map_finder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    54892 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/place/region_mesh.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     7972 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/place/rotation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5670 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/place/volumetric_mapping.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/Blender/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.340803 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      661 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6031 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/plotting/Blender/visualisation/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        0 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1980 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1429 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1217 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4086 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCube.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4371 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5497 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5109 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5250 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22786 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    10089 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network_old.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5344 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_touch_detection.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      381 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3414 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plotLTSdensity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2740 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     9403 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_connectivity.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8658 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_cross_correlogram.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2869 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_degeneration.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6935 2022-10-07 09:01:39.000000 snudda-1.4.4/snudda/plotting/plot_degeneration_and_growth.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1279 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_density.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2779 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_density_slice.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3415 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_distance_statistics.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5309 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_input.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    15738 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/plotting/plot_input_locations.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    11861 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/plotting/plot_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3081 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3703 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_node_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     8024 2022-11-04 18:40:55.000000 snudda-1.4.4/snudda/plotting/plot_period_experiment.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3397 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/plotting/plot_size_benchmark.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22560 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/plotting/plot_spike_raster_v2.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18674 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/plotting/plot_traces.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/prune/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      226 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/prune/__init__.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.344803 snudda-1.4.4/snudda/simulate/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       52 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/__init__.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    24795 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/model_current_injections.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22316 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/network_pair_pulse_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3729 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/simulate/nrn_simulator_parallel.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22967 2022-11-11 14:42:41.000000 snudda-1.4.4/snudda/simulate/pair_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    13157 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/save_network_recording.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    81843 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/simulate/simulate.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.348803 snudda-1.4.4/snudda/utils/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      437 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/__init__.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    22027 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/ablate_network.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     5292 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/benchmark_logging.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1237 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/cleanup.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2533 2022-11-03 09:16:18.000000 snudda-1.4.4/snudda/utils/clone_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    18451 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/conv_hurt.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     1230 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/create_parameter_morphology_input_map.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    17769 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/cut.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     3728 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/export_connection_matrix.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     4512 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/export_eroded_connection_matrix.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    35149 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/export_sonata.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     2310 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/fake_load.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)       80 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/input_helper.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    49806 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/load.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)    15170 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/load_network_simulation.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      278 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/memory.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     6298 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/merge_synapse_files.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      593 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/numpy_encoder.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      185 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/pip_upgrade.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     3919 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/reposition_neurons.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4840 2023-02-15 16:15:38.000000 snudda-1.4.4/snudda/utils/snudda_path.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    38508 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies.py
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    19223 2023-04-26 08:33:58.000000 snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies_extended.py
+-rwxr-xr-x   0 hjorth    (1001) hjorth    (1001)     1916 2022-09-19 09:45:08.000000 snudda-1.4.4/snudda/utils/upgrade_old_network_file.py
+drwxr-xr-x   0 hjorth    (1001) hjorth    (1001)        0 2023-04-26 08:34:26.252802 snudda-1.4.4/snudda.egg-info/
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)     4188 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/PKG-INFO
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)    22867 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/SOURCES.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        1 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/dependency_links.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      417 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/entry_points.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)      197 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/requires.txt
+-rw-r--r--   0 hjorth    (1001) hjorth    (1001)        7 2023-04-26 08:34:26.000000 snudda-1.4.4/snudda.egg-info/top_level.txt
```

### Comparing `snudda-1.4.0/LICENSE` & `snudda-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/PKG-INFO` & `snudda-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 1.4.0
+Version: 1.4.4
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `snudda-1.4.0/README.md` & `snudda-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/setup.py` & `snudda-1.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     print(f"READTHEDOCS = {os.environ.get('READTHEDOCS')}") 
     install_requires = [
         "bluepyopt>=1.11.7",
         "h5py>=3.2.1",
         "ipyparallel>=6.3.0",
         "matplotlib>=3.3.4",
         "mpi4py>=3.0.3",
-        "numpy>=1.20.2",
+        "numpy==1.23.5",  # Numba depends on specific numpy version, so removing this line for now as numba will install its requirements
         "scipy>=1.6.3",
         "sonata>=0.0.2",
         "pyzmq>=22.0.3",
         "setuptools",
         "psutil",
         "numexpr>=2.7.3",
-        "numba>=0.53.1",
+        "numba>=0.56.4",
         # "igraph"
     ]
     
 setuptools.setup(
     name="snudda",
     version=__version__,
     author="Johannes Hjorth",
@@ -59,8 +59,9 @@
                                       "snudda_load = snudda.utils.load:snudda_load_cli",
                                       "snudda_load_simulation_data = snudda.utils.load_network_simulation:load_network_simulation_cli",
                                       "snudda_ablate_network = snudda.utils.ablate_network:snudda_ablate_network_cli",
                                       "snudda_plot_network = snudda.plotting.plot_network:snudda_plot_network_cli",
                                       "snudda_plot_trace = snudda.plotting.plot_traces:snudda_plot_traces_cli"]},
     install_requires=install_requires,
     extras_require={"dev": ["sphinx"]},
+    setup_requires=['wheel']
 )
```

### Comparing `snudda-1.4.0/snudda/analyse/analyse.py` & `snudda-1.4.4/snudda/analyse/analyse.py`

 * *Files 1% similar despite different names*

```diff
@@ -648,15 +648,15 @@
             import pdb
             pdb.set_trace()
 
         return c_id
 
     ############################################################################
 
-    def save_figure(self, plt, fig_name, fig_type="pdf"):
+    def save_figure(self, plt, fig_name, fig_type="png"):
 
         if not os.path.isdir(self.fig_dir):
             print(f"save_figures: Creating directory {self.fig_dir}")
             os.mkdir(self.fig_dir)
 
         full_fig_name = os.path.join(self.fig_dir, f"{fig_name }.{fig_type}")
 
@@ -665,27 +665,28 @@
         plt.gca().spines["top"].set_visible(False)
 
         plt.tight_layout()
         plt.savefig(full_fig_name)
         plt.pause(0.001)
         # plt.savefig(full_fig_name.replace('.pdf', '.eps'))
 
-        print("Wrote " + full_fig_name)
+        print(f"Wrote {full_fig_name}")
 
         if self.close_plots:
             time.sleep(1)
             plt.close()
 
         return full_fig_name
 
     ############################################################################
 
     def plot_num_synapses_per_pair(self, pre_type, post_type, side_len=None,
                                    name_str="", volume_id=None,
-                                   connection_type="synapses"):
+                                   connection_type="synapses",
+                                   sub_title=None):
 
         if volume_id is None:
             volume_id = self.volume_id
 
         if side_len is None:
             side_len = self.side_len
 
@@ -752,15 +753,21 @@
                  range(0, 1 + max_synapses),
                  density=True,
                  align="left",
                  color=self.get_neuron_color(pre_type))
 
         plt.xlabel("Number of " + connection_type)
         plt.ylabel('Probability density')
-        plt.title(f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)}")
+        title_str = f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)}"
+
+        if sub_title is not None:
+            plt.suptitle(f"{title_str}", y=0.9)
+            plt.title(sub_title, fontsize=10)
+        else:
+            plt.title(title_str)
 
         plt.tight_layout()
         plt.draw()
 
         fig_name = f"Network-number-of-{connection_type}-from-{pre_type}-to-{post_type}-per-cell"
 
         self.save_figure(plt, fig_name)
@@ -856,20 +863,27 @@
                                     post_type=None,
                                     num_bins=86,
                                     name_str="",
                                     side_len=None,
                                     exp_max_dist=None,
                                     exp_data=None,
                                     exp_data_detailed=None,
+                                    exp_colour=None,
                                     dist_3d=True,
                                     volume_id=None,
                                     x_max=250,
                                     y_max=None,
                                     connection_type="synapses",
-                                    draw_step=False):
+                                    draw_step=False,
+                                    sub_title=None,
+                                    ax=None,
+                                    return_ax=False,
+                                    colour="black",
+                                    show_plot=None,
+                                    save_figure=True):
 
         if volume_id is None:
             volume_id = self.volume_id
 
         assert pre_type is not None
         assert post_type is not None
 
@@ -928,15 +942,16 @@
         (dist, p_con, count_con, count_all) = \
             self.connection_probability(pre_id, post_id, num_bins, dist_3d=dist_3d,
                                         connection_type=connection_type)
 
         # Now let's plot it
 
         # fig = plt.figure()
-        fig, ax = plt.subplots(1)
+        if ax is None:
+            fig, ax = plt.subplots(1)
 
         matplotlib.rcParams.update({'font.size': 24})
 
         plt_ctr = 0
 
         if exp_data is None:
             exp_data = []
@@ -976,60 +991,64 @@
                 # https://en.wikipedia.org/wiki/Binomial_proportion_confidence_interval#Wilson_score_interval
                 # https://www.tandfonline.com/doi/abs/10.1080/01621459.1927.10502953
                 # Wilson score
                 # Wilson, Edwin B. "Probable inference, the law of succession, and statistical inference." Journal of the American Statistical Association 22.158 (1927): 209-212.
                 ns = exp_num[0]
                 n = exp_num[1]
                 z = 1.96  # This gives us 95% confidence intervall
-                bar_centre = (ns + (z ** 2) / 2) / (n + z * 2)
+                bar_centre = (ns + (z ** 2) / 2) / (n + z ** 2)
                 bar_height = z / (n + z ** 2) * np.sqrt((ns * (n - ns) / n + (z ** 2) / 4))
 
-                plt.errorbar(d_limit * 1e6 / 2, bar_centre, bar_height, color="gray",
-                             elinewidth=1, capsize=5)
+                ax.errorbar(d_limit * 1e6 / 2, bar_centre, bar_height, color="gray",
+                            elinewidth=1, capsize=5)
 
             else:
                 std_exp = 0
 
             if p_exp is not None:
-                plt.plot([0, d_limit * 1e6], [p_exp, p_exp],
-                         color=(0.8, 0.3 * plt_ctr, 0.3 * plt_ctr), linewidth=2)
+
+                if exp_colour is None:
+                    exp_colour = (0.8, 0.3 * plt_ctr, 0.3 * plt_ctr)
+
+                ax.plot([0, d_limit * 1e6], [p_exp, p_exp],
+                        color=exp_colour, linewidth=2)
 
                 # Add a star also
-                plt.plot(d_limit * 1e6 / 2, p_exp,
-                         color=(0.8, 0.3 * plt_ctr, 0.3 * plt_ctr),
-                         marker="D",
-                         markersize=10)
+                ax.plot(d_limit * 1e6 / 2, p_exp,
+                        color=exp_colour,
+                        marker="D",
+                        markersize=10)
 
                 plt_ctr += 1
-                plt.ion()
-                plt.draw()
 
-                if self.show_plots:
+                if self.show_plots or show_plot:
+                    plt.ion()
+                    plt.draw()
                     plt.show()
 
         # Draw the curve itself
         if draw_step:
-            plt.step(dist * 1e6, p_con, color='black', linewidth=2, where="post")
+            plt.step(dist * 1e6, p_con, color=colour, linewidth=2, where="post")
         else:
             d_half_step = (dist[1] - dist[0]) / 2
-            plt.plot((dist + d_half_step) * 1e6, p_con, color='black', linewidth=2)
+            plt.plot((dist + d_half_step) * 1e6, p_con, color=colour, linewidth=2)
 
         plt.xticks(fontsize=14, rotation=0)
         plt.yticks(fontsize=14, rotation=0)
 
         label_size = 22
 
         # Hack to avoid divide by zero
         count_all_b = count_all.copy()
         count_all_b[count_all_b == 0] = 1.0
 
         # This gives us 95% confidence intervall
         z = 1.96
 
-        p_centre = np.array([(ns + (z ** 2) / 2) / (n + z * 2)
+        p_centre = np.array([(ns + (z ** 2) / 2) / (n + z ** 2)
                              for (ns, n) in zip(count_con, count_all_b)]).flatten()
         p_height = np.array([z / (n + z ** 2)
                              * np.sqrt((ns * (n - ns) / n + (z ** 2) / 4))
                              for (ns, n) in zip(count_con, count_all_b)]).flatten()
 
         # Use the last bin larger than xMax as the end
         d_idx = np.where(dist * 1e6 > x_max)[0][0]
@@ -1065,36 +1084,48 @@
         if locs[-1] > plt.ylim()[1]:
             locs = locs[:-1]
             new_labels = new_labels[:-1]
 
         plt.yticks(locs, new_labels)
 
         if connection_type == "synapses":
-            plt.title(f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)}")
+            title_str = f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)}"
         else:
-            plt.title(f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)} ({connection_type})")
+            title_str = f"{self.neuron_name(pre_type)} to {self.neuron_name(post_type)} ({connection_type})"
+
+        if sub_title is not None:
+            plt.suptitle(f"{title_str}", y=0.9)
+            plt.title(sub_title, fontsize=10)
+        else:
+            plt.title(title_str)
 
         plt.tight_layout()
-        plt.ion()
-        plt.draw()
 
         if dist_3d:
             proj_text = '-3D-dist'
         else:
             proj_text = '-2D-dist'
 
         fig_name = (f"Network-distance-dependent-connection-probability-{pre_type}"
                     f"-to-{post_type}-{connection_type}{proj_text}")
 
-        full_fig_name = self.save_figure(plt, fig_name)
+        if save_figure:
+            full_fig_name = self.save_figure(plt, fig_name)
+        else:
+            full_fig_name = None
 
-        if self.show_plots:
+        if self.show_plots or show_plot:
+            plt.ion()
+            plt.draw()
             plt.show()
+            plt.pause(0.001)
+
+        if return_ax:
+            return ax
 
-        plt.pause(0.001)
         return model_probs, full_fig_name
 
     ############################################################################
 
     # expMaxDist=[50e-6,100e-6]
     # expData=[None, None] (none if no exp data, or values)
     # expDataDetailed=[(conA,totA),(conB,totB)]
```

### Comparing `snudda-1.4.0/snudda/analyse/analyse_gap_junction_coupling.py` & `snudda-1.4.4/snudda/analyse/analyse_gap_junction_coupling.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/analyse/analyse_input.py` & `snudda-1.4.4/snudda/analyse/analyse_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/analyse/analyse_neuroinformatics2020.py` & `snudda-1.4.4/snudda/analyse/analyse_neuroinformatics2020.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/analyse/analyse_striatum.py` & `snudda-1.4.4/snudda/analyse/analyse_striatum.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/analyse/analyse_synapse_location.py` & `snudda-1.4.4/snudda/analyse/analyse_synapse_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         if post_type is None:
             post_text = "ALL"
         else:
             post_text = post_type
 
         if fig_path is None:
-            fig_path = os.path.join(self.figure_path, f"Distance-to-soma-{pre_text}-to-{post_text}.png")
+            fig_path = os.path.join(self.figure_path, f"Distance-to-soma-{pre_text}-to-{post_text}.pdf")
 
         dist = self.synapse_distance_to_soma(pre_type=pre_type, post_type=post_type)
 
         plt.figure()
         dist_scaled = [d*1e6 for d in dist]
         bins = np.arange(0, np.ceil(np.max(dist_scaled) / bin_width + 1) * bin_width, bin_width)
         plt.hist(dist_scaled, bins=bins)
```

### Comparing `snudda-1.4.0/snudda/analyse/analyse_topology.py` & `snudda-1.4.4/snudda/analyse/analyse_topology.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/analyse/analyse_topology_activity.py` & `snudda-1.4.4/snudda/analyse/analyse_topology_activity.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/cli.py` & `snudda-1.4.4/snudda/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,55 +55,61 @@
     place_parser.add_argument("-randomseed", "--randomseed", "--seed", default=None, help="Random seed", type=int)
     place_parser.add_argument("--raytraceBorders", help="Ray traces for more precise mesh edge detection",
                               action="store_true", dest="raytrace_borders", default=False)
     place_parser.add_argument("--profile", help="Run python cProfile", action="store_true")
     place_parser.add_argument("--verbose", action="store_true")
     place_parser.add_argument("--h5legacy", help="Use legacy hdf5 support", action="store_true")
     place_parser.add_argument("-parallel", "--parallel", action="store_true", default=False)
+    place_parser.add_argument("-ipython_profile", "--ipython_profile", default=None)
 
     detect_parser = sub_parsers.add_parser("detect")
     detect_parser.add_argument("path", help="Location of network")
     detect_parser.add_argument("-randomseed", "--randomseed", "--seed", default=None, help="Random seed", type=int)
     detect_parser.add_argument("-cont", "--cont", help="Continue partial touch detection", action="store_true")
     detect_parser.add_argument("-hvsize", "--hvsize", default=100,
                                help="Hyper voxel size, eg. 100 = 100x100x100 voxels in hypervoxel")
     detect_parser.add_argument("--volumeID", help="Specify volume ID for detection step")
     detect_parser.add_argument("--profile", help="Run python cProfile", action="store_true")
     detect_parser.add_argument("--verbose", action="store_true")
     detect_parser.add_argument("--h5legacy", help="Use legacy hdf5 support", action="store_true")
     detect_parser.add_argument("-parallel", "--parallel", action="store_true", default=False)
+    detect_parser.add_argument("-ipython_profile", "--ipython_profile", default=None)
+
 
     prune_parser = sub_parsers.add_parser("prune")
     prune_parser.add_argument("path", help="Location of network")
     prune_parser.add_argument("-randomseed", "--randomseed", "--seed", default=None, help="Random seed", type=int)
     prune_parser.add_argument("--configFile", dest="config_file", default=None,
                               help="Prune using different network config file, useful when tuning pruning")
     prune_parser.add_argument("--profile", help="Run python cProfile", action="store_true")
     prune_parser.add_argument("--verbose", action="store_true")
     prune_parser.add_argument("--h5legacy", help="Use legacy hdf5 support", action="store_true")
     prune_parser.add_argument("--keepfiles", action="store_true",
                               help="Keep temp and voxel files after pruning (e.g. useful if you want to rerun pruning)")
     prune_parser.add_argument("--savePutative", action="store_true",
                               help="Also saved network-putative-synapses.hdf5 with unpruned network")
     prune_parser.add_argument("-parallel", "--parallel", action="store_true", default=False)
+    prune_parser.add_argument("-ipython_profile", "--ipython_profile", default=None)
+
 
     input_parser = sub_parsers.add_parser("input")
     input_parser.add_argument("path", help="Location of network")
     input_parser.add_argument("--input", help="Input json config file (for input setup)", default=None)
     input_parser.add_argument("--inputFile", help="Input hdf5 file (for simulation)",
                               dest="input_file", default=None)
     input_parser.add_argument("--networkFile", help="Network file, if not network-synapses.hdf5",
                               dest="network_file")
     input_parser.add_argument("--time", type=float, default=None, help="Duration of simulation in seconds")
     input_parser.add_argument("-randomseed", "--randomseed", "--seed", default=None, help="Random seed", type=int)
     input_parser.add_argument("--profile", help="Run python cProfile", action="store_true")
     input_parser.add_argument("--verbose", action="store_true")
     input_parser.add_argument("--h5legacy", help="Use legacy hdf5 support", action="store_true")
     input_parser.add_argument("-parallel", "--parallel", action="store_true", default=False)
-    input_parser.add_argument("-no_meta_input","--no_meta_input", help="Do not use meta.json as stimulation input", action="store_true", default=False)
+    input_parser.add_argument("-ipython_profile", "--ipython_profile", default=None)
+    input_parser.add_argument("-no_meta_input", "--no_meta_input", help="Do not use meta.json as stimulation input", action="store_true", default=False)
 
     simulate_parser = sub_parsers.add_parser("simulate")
     simulate_parser.add_argument("path", help="Location of network")
     simulate_parser.add_argument("--networkFile", help="Network file, if not network-synapses.hdf5",
                                  dest="network_file", default=None)
     simulate_parser.add_argument("--inputFile", help="Input hdf5 file (for simulation)",
                                  dest="input_file", default=None)
@@ -155,14 +161,19 @@
                "input": snudda.setup_input,
                "export": snudda.export_to_SONATA,
                "convert": snudda.export_to_SONATA,
                "analyse": snudda.analyse,
                "simulate": snudda.simulate,
                "help": snudda.help_info}
 
+    if not hasattr(args, 'ipython_profile'):
+        args.ipython_profile = None
+
+    print(f"args.ipython_profile = {args.ipython_profile}")
+
     if args.profile:
         prof_file = f"profile-{args.action}.prof"
         print(f"Saving profile data to: {prof_file}")
         import cProfile
         cProfile.runctx("actions[args.action](args)", None, locals(), filename=prof_file)
 
         # To analyse profile data:
@@ -175,15 +186,16 @@
         if hasattr(args, "parallel"):
             run_parallel = args.parallel
         else:
             run_parallel = False
 
         running_neuron = (args.action == "simulate")
 
-        bl = BenchmarkLogging(args.path, parallel_flag=run_parallel, running_neuron=running_neuron)
+        bl = BenchmarkLogging(args.path, parallel_flag=run_parallel, running_neuron=running_neuron,
+                              ipython_profile=args.ipython_profile)
         bl.start_timer(args.action)
 
         # Perform the requested action
         actions[args.action](args)
 
         bl.stop_timer(args.action)
         bl.write_log()
```

### Comparing `snudda-1.4.0/snudda/core.py` & `snudda-1.4.4/snudda/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         log_file_name = os.path.join(self.network_path, "log", "place-neurons.txt")
 
         random_seed = args.randomseed
 
         self.setup_log_file(log_file_name)  # sets self.logFile
 
         if args.parallel:
-            self.setup_parallel()  # sets self.d_view
+            self.setup_parallel(ipython_profile=args.ipython_profile)  # sets self.d_view
 
         from snudda.place.place import SnuddaPlace
 
         if args.h5legacy:
             h5libver = "earliest"
         else:
             h5libver = "latest"  # default
@@ -228,15 +228,15 @@
 
         voxel_dir = os.path.join(self.network_path, "voxels")
         self.make_dir_if_needed(voxel_dir)
 
         self.setup_log_file(log_filename)  # sets self.logfile
 
         if args.parallel:
-            self.setup_parallel()  # sets self.d_view
+            self.setup_parallel(ipython_profile=args.ipython_profile)  # sets self.d_view
 
         if args.h5legacy:
             h5libver = "earliest"
         else:
             h5libver = "latest"  # default
 
         from snudda.detect.detect import SnuddaDetect
@@ -296,15 +296,15 @@
         log_filename = os.path.join(self.network_path, "log", "synapse-pruning.txt")
 
         random_seed = args.randomseed
 
         self.setup_log_file(log_filename)  # sets self.logfile
 
         if args.parallel:
-            self.setup_parallel()  # sets self.d_view
+            self.setup_parallel(ipython_profile=args.ipython_profile)  # sets self.d_view
 
         # Optionally set this
         scratch_path = None
 
         if args.h5legacy:
             h5libver = "earliest"
         else:
@@ -344,15 +344,15 @@
         """
 
         print("Setting up inputs, assuming input.json exists")
         log_filename = os.path.join(self.network_path, "log", "setup-input.txt")
         self.setup_log_file(log_filename)  # sets self.logfile
 
         if args.parallel:
-            self.setup_parallel()  # sets self.d_view
+            self.setup_parallel(ipython_profile=args.ipython_profile)  # sets self.d_view
 
         from snudda.input.input import SnuddaInput
 
         if "input" in args and args.input:
             input_config = args.input
         else:
             input_config = os.path.join(self.network_path, "input.json")
@@ -411,16 +411,14 @@
         """
         Export network to SONATA files. (Currently not functioning)
 
         Args:
             args : command line arguments from argparse
         """
 
-        assert False, "Old export to SONATA borken, fixme!"
-        # TODO: Fix this
         from snudda.utils.export_sonata import ExportSonata
 
         print("Exporting to SONATA format")
         print(f"Network path: {self.network_path}")
 
         if args.network_file:
             network_file = args.network_file
@@ -674,41 +672,44 @@
 
     def analyse(self, args):
 
         print("Add analysis code here, see Network_analyse.py")
 
     ############################################################################
 
-    def setup_parallel(self):
+    def setup_parallel(self, ipython_profile=None):
         """Setup ipyparallel workers."""
 
         self.slurm_id = os.getenv('SLURM_JOBID')
 
         if self.slurm_id is None:
             self.slurm_id = 0
         else:
             self.slurm_id = int(self.slurm_id)
 
         self.logfile.write(f"Using slurm_id: {self.slurm_id}")
 
-        ipython_profile = os.getenv('IPYTHON_PROFILE')
+        if ipython_profile is None:
+            ipython_profile = os.getenv('IPYTHON_PROFILE')
+
         if not ipython_profile:
             ipython_profile = "default"
 
         ipython_dir = os.getenv('IPYTHONDIR')
         if not ipython_dir:
             ipython_dir = os.path.join(os.path.abspath(os.getcwd()), ".ipython")
 
         self.logfile.write('Creating ipyparallel client\n')
 
         from ipyparallel import Client
 
         u_file = os.path.join(ipython_dir, f"profile_{ipython_profile}", "security", "ipcontroller-client.json")
+        print(f"Reading IPYPARALLEL connection info from {u_file}\n")
         self.logfile.write(f"Reading IPYPARALLEL connection info from {u_file}\n")
-        self.rc = Client(url_file=u_file, timeout=120, debug=False)
+        self.rc = Client(profile=ipython_profile, url_file=u_file, timeout=120, debug=False)
 
         self.logfile.write(f'Client IDs: {self.rc.ids}')
 
         # http://davidmasad.com/blog/simulation-with-ipyparallel/
         # http://people.duke.edu/~ccc14/sta-663-2016/19C_IPyParallel.html
         self.d_view = self.rc.direct_view(targets='all')  # rc[:] # Direct view into clients
```

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Cortex/AA0059.swc` & `snudda-1.4.4/snudda/data/InputAxons/Cortex/AA0059.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc` & `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc` & `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc` & `snudda-1.4.4/snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc` & `snudda-1.4.4/snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Thalamus/AA0054.swc` & `snudda-1.4.4/snudda/data/InputAxons/Thalamus/AA0054.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc` & `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg10/AA0054-reg10.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc` & `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg15/AA0054-reg15.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc` & `snudda-1.4.4/snudda/data/InputAxons/Thalamus/Reg5/AA0054-reg5.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/1001_STRd_Sst_dens.csv` & `snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/1001_STRd_Sst_dens_smooth.csv` & `snudda-1.4.4/snudda/data/density/1001_STRd_Sst_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/252_STRd_Chat_dens.csv` & `snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/252_STRd_Chat_dens_smooth.csv` & `snudda-1.4.4/snudda/data/density/252_STRd_Chat_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/352_STRd_Drd1_dens.csv` & `snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/352_STRd_Drd1_dens_smooth.csv` & `snudda-1.4.4/snudda/data/density/352_STRd_Drd1_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/72109410_STRd_Adora2a_dens.csv` & `snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv` & `snudda-1.4.4/snudda/data/density/72109410_STRd_Adora2a_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/79556738_STRd_Pvalb_dens.csv` & `snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv` & `snudda-1.4.4/snudda/data/density/79556738_STRd_Pvalb_dens_smooth.csv`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/combine_densities.py` & `snudda-1.4.4/snudda/data/density/combine_densities.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/density/dorsal_striatum_density.json` & `snudda-1.4.4/snudda/data/density/dorsal_striatum_density.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-2.json` & `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-3.json` & `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-3.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-4.json` & `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-4.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-6.json` & `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-6.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/experiment_config/pair_recording/experiment-config-7.json` & `snudda-1.4.4/snudda/data/experiment_config/pair_recording/experiment-config-7.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/images/snudda-video-qr-code.png` & `snudda-1.4.4/snudda/data/images/snudda-video-qr-code.png`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v2.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v3.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v3b.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v3b.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4-cluster-test.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled-v4.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled-v4.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/external-input-dSTR-scaled.json` & `snudda-1.4.4/snudda/data/input_config/external-input-dSTR-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-ChIN.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-ChIN.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-Channel-Activation.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-Channel-Activation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-channel-1.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-1.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-channel-2.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-channel-2.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-v7.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-v7.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-v8.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-v8.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-tinytest-v9-freq-vectors.json` & `snudda-1.4.4/snudda/data/input_config/input-tinytest-v9-freq-vectors.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/input_config/input-v10-scaled.json` & `snudda-1.4.4/snudda/data/input_config/input-v10-scaled.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/GPe.obj` & `snudda-1.4.4/snudda/data/mesh/GPe.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/GPi.obj` & `snudda-1.4.4/snudda/data/mesh/GPi.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/SNc.obj` & `snudda-1.4.4/snudda/data/mesh/SNc.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/SNr.obj` & `snudda-1.4.4/snudda/data/mesh/SNr.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/STN.obj` & `snudda-1.4.4/snudda/data/mesh/STN.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/Striatum-d.obj` & `snudda-1.4.4/snudda/data/mesh/Striatum-d.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj` & `snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj` & `snudda-1.4.4/snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/Striatum-v.obj` & `snudda-1.4.4/snudda/data/mesh/Striatum-v.obj`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/mesh/get_mesh.ipynb` & `snudda-1.4.4/snudda/data/mesh/get_mesh.ipynb`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/Kv3_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/NO.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/NO.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/bk_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/bk_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/bk_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/ca_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/ca_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cadyn_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cadyn_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cal12_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/car_ms.mod`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,82 @@
-TITLE HVA L-type calcium current (Cav1.2)
+TITLE R-type calcium current (Cav2.3)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
-    
+
 ENDCOMMENT
 
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cal12_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
-    RANGE damod, maxMod
+    SUFFIX car_ms
+    USEION ca READ cai, cao WRITE ica VALENCE 2
+    RANGE pbar, ica
+    RANGE modDA, maxModDA, levelDA
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
-    a = 0.17
-    :q = 1	          : room temperature 22-25 C
-    q = 2	          : body temperature 35 C
-    damod = 0
-    maxMod = 1
+    pbar = 0.0 	(cm/s)
+    :q = 1	: room temperature 22 C
+    q = 3	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 } 
 
 ASSIGNED { 
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
+    ica (mA/cm2)
+    eca (mV)
     celsius (degC)
-    cali (mM)
-    calo (mM)
+    cai (mM)
+    cao (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*(h*a+1-a)*ghk(v, cali, calo)*modulation()
+    ica = pbar*m*m*m*h*ghk(v, cai, cao)*modulationDA()
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -74,18 +85,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-8.9))/(-6.7)))
-    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
-    hinf = 1/(1+exp((v-(-13.4))/11.9))
-    htau = 44.3
+    minf = 1/(1+exp((v-(-29))/(-9.6)))
+    mtau = 5.1
+    hinf = 1/(1+exp((v-(-33.3))/17))
+    htau = 22+80/(1+exp((v-(-19))/5))
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -98,54 +109,46 @@
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from P5-P32
-Charles River rat pups [1].   Activation time constant is from the
-rodent neuron culture (both rat and mouse cells), room temperature 22-25
-C [2, Fig.15A]. Inactivation curve of CaL v1.3 current was taken from HEK
-cells [3, Fig.2 and p.819] at room temperature.
-
-Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m1h type was used [5,6]. Activation
-time constant was refitted to avoid singularity.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
-
-[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
-omega-conotoxin-sensitive calcium channels in a mammalian
-neuroblastoma-glioma cell line. J Physiol 448:161-88.
-
-[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
-Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
-properties, pharmacology, and modulation of human, neuronal L-type
-(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
-85:816-827.
+Original data by Foehring  et al (2000) [1] for dissociated MSNs from
+P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
+liquid junction potential was around 8 mV and was not corrected. Kinetics
+of m3h type was fitted.  Inactivation time constants were measured in
+neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
+at room temperature 22 C.
+
+Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
+<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
+activation time constant matched m^3 originally [1]. Smooth fit of
+inactivation time constant from [2,3].
+
+[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
+(2000) Unique properties of R-type calcium currents in neocortical and
+neostriatal neurons. J Neurophysiol 84(5):2225-36.
+
+[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
+biophysical characterization of voltage-gated calcium currents in the
+endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
 
-[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
-Neurobiol 96(1):1-31.
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cal13_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/can_ms.mod`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,32 @@
-TITLE LVA L-type calcium current (Cav1.3)
+TITLE N-type calcium current (Cav2.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
 UNITS {
@@ -25,46 +36,51 @@
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cal13_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
-    RANGE damod, maxMod
+    SUFFIX can_ms
+    USEION ca READ cai, cao WRITE ica VALENCE 2
+    RANGE pbar, ica
+    RANGE modDA, maxModDA, levelDA, modACh, maxModACh, levelACh
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
+    pbar = 0.0 	(cm/s)
+    a = 0.21
     :q = 1	: room temperature 22-25 C
-    q = 2	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    q = 3	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1
+    levelACh = 0
 } 
 
 ASSIGNED { 
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
+    ica (mA/cm2)
+    eca (mV)
     celsius (degC)
-    cali (mM)
-    calo (mM)
+    cai (mM)
+    cao (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*m*h*ghk(v, cali, calo)*modulation()
+    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)*modulationDA()*modulationACh()
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -73,18 +89,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-33))/(-6.7)))
-    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
-    hinf = 1/(1+exp((v-(-13.4))/11.9))
-    htau = 44.3
+    minf = 1/(1+exp((v-(-3))/(-8)))
+    mtau = 0.06+1/(exp((v-25)/18)+exp((v-(-31))/(-44)))
+    hinf = 1/(1+exp((v-(-74.8))/6.5))
+    htau = 70
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -96,61 +112,59 @@
     if (fabs(z) < 1e-4) {
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
 
-FUNCTION modulation() {
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from
-P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
-Fig.1D]. Activation time constant is from the rodent neuron culture (both
-rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
-curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
-at room temperature.
-
-Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
-time constant was refitted to avoid singularity.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
+Model is based on mixed data. Activation curve is from neostriatal
+medium spiny neurons of adult P28+ rats [1, Fig.12F], unspecified
+recording temperature. Potentials were not corrected for the liquid
+junction potential, which was estimated to be 7 mV.  Activation time
+constant is from the rodent neuron culture (both rat and mouse cells),
+room temperature 22-25 C [2, Fig.15B].  Inactivation data is from human
+(HEK) cells [3, Tab.1, Tab.2], supposedly at room temperature.
+
+Kinetics of m2h type is used [2, Fig.5]. Activation of m^2 is fitted
+to the experimental data [1,4], activation time constant corresponds
+to m^2 already [2].  Original model [5,4] was modified by Alexander
+Kozlov <akozlov@kth.se>. Activation time constant was refitted to avoid
+singularity in the expression. Temperature correction factor 3 is used
+for body temperature [4,5].
+
+[1] Bargas J, Howe A, Eberwine J, Cao Y, Surmeier DJ (1994) Cellular
+and molecular characterization of Ca2+ currents in acutely isolated,
+adult rat neostriatal neurons. J Neurosci 14(11 Pt 1):6667-86.
 
 [2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
 omega-conotoxin-sensitive calcium channels in a mammalian
 neuroblastoma-glioma cell line. J Physiol 448:161-88.
 
-[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
-Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
-properties, pharmacology, and modulation of human, neuronal L-type
-(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
-85:816-827.
+[3] McNaughton NC, Randall AD (1997) Electrophysiological properties of
+the human N-type Ca2+ channel: I. Channel gating in Ca2+, Ba2+ and Sr2+
+containing solutions. Neuropharmacology 36(7):895-915.
+
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
 
-[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[5] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
-Neurobiol 96(1):1-31.
-
-[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
-at relatively hyperpolarized membrane potentials and are incompletely
-inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
-
-
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cal_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/caldyn_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/can_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/can_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/can_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_fs.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,30 @@
 TITLE N-type calcium current (Cav2.2)
 
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX can_ms
+    SUFFIX can_fs
     USEION ca READ cai, cao WRITE ica VALENCE 2
     RANGE pbar, ica
-    RANGE damod, maxMod
 }
 
 PARAMETER {
     pbar = 0.0 	(cm/s)
     a = 0.21
     :q = 1	: room temperature 22-25 C
     q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
 } 
 
 ASSIGNED { 
     v (mV)
     ica (mA/cm2)
     eca (mV)
     celsius (degC)
@@ -57,15 +36,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)*modulation()
+    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -97,22 +76,14 @@
     if (fabs(z) < 1e-4) {
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1) 
-}
-
-
 COMMENT
 
 Model is based on mixed data. Activation curve is from neostriatal
 medium spiny neurons of adult P28+ rats [1, Fig.12F], unspecified
 recording temperature. Potentials were not corrected for the liquid
 junction potential, which was estimated to be 7 mV.  Activation time
 constant is from the rodent neuron culture (both rat and mouse cells),
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cap_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cap_ch.mod`

 * *Files 24% similar despite different names*

```diff
@@ -1,116 +1,140 @@
-: HH P-type Calcium current
-: Created 8/13/02 - nwg
-
-: copy by josh for cholinergic interneuron
-
-
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-NEURON {
-	SUFFIX cap_ch
-	USEION ca READ cai, cao WRITE ica
-	RANGE gbar, ica ,g
-	GLOBAL minf,mtau
-	GLOBAL monovalConc, monovalPerm
-    RANGE damod, maxMod
-}
-
-UNITS {
-	(mV) = (millivolt)
-	(mA) = (milliamp)
-	(mM) = (milli/liter)
-	F = 9.6485e4   (coul)
-	R = 8.3145 (joule/degC)
-}
-
-PARAMETER {
-	v (mV)
-
-	gbar = .00005	(cm/s)
-	monovalConc = 140     (mM)
-	monovalPerm = 0
-	celsius = 35
-	cai             (milli/liter)
-	cao             (milli/liter)
-    damod = 0
-    maxMod = 1
-}
-
-ASSIGNED {
-	ica            (mA/cm2)
-        minf
-	mtau           (ms)
-	T              (degC)
-	E              (volts)
-	g	(S/cm2)
-}
-
-STATE {
-	m
-}
-
-INITIAL {
-	rates(v)
-	m = minf
-}
-
-BREAKPOINT {
-     SOLVE states METHOD cnexp
-	g = (1e3) * gbar * m *modulation()
-	ica = g * ghk(v, cai, cao, 2)
-}
-
-DERIVATIVE states {
-	rates(v)
-	m' = (minf - m)/mtau
-}
-
-FUNCTION ghk( v(mV), ci(mM), co(mM), z)  (coul/cm3) { LOCAL Ci
-	T = celsius + 273.19  : Kelvin
-        E = (1e-3) * v
-        Ci = ci + (monovalPerm) * (monovalConc)        : Monovalent permeability
-	if (fabs(1-exp(-z*(F*E)/(R*T))) < 1e-6) { : denominator is small -> Taylor series
-		ghk = (1e-6) * z * F * (Ci-co*exp(-z*(F*E)/(R*T)))*(1-(z*(F*E)/(R*T)))
-	} else {
-		ghk = (1e-6) * z^2*(E*F^2)/(R*T)*(Ci-co*exp(-z*(F*E)/(R*T)))/(1-exp(-z*(F*E)/(R*T)))
-	}
-}
-
-PROCEDURE rates (v (mV)) {
-        UNITSOFF
-	minf = 1/(1+exp(-(v - (-19)) / 5.5))
-	mtau = (mtau_func(v)) * 1e3
-        UNITSON
-}
-
-FUNCTION mtau_func( v (mV) ) (ms) {
-        UNITSOFF
-        if (v > -50) {
-            mtau_func = .000191 + .00376*exp(-((v-(-41.9))/27.8)^2)
-        } else {
-            mtau_func = .00026367 + .1278 * exp(.10327*v)
-        }
-        UNITSON
-}
-
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1) 
-}
+: HH P-type Calcium current
+: Created 8/13/02 - nwg
+
+: copy by josh for cholinergic interneuron
+
+
+COMMENT
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+
+ENDCOMMENT
+
+NEURON {
+	SUFFIX cap_ch
+	USEION ca READ cai, cao WRITE ica
+	RANGE gbar, ica ,g
+	GLOBAL minf,mtau
+	GLOBAL monovalConc, monovalPerm
+        RANGE modDA, maxModDA, levelDA
+        RANGE modACh, maxModACh, levelACh
+}
+
+UNITS {
+	(mV) = (millivolt)
+	(mA) = (milliamp)
+	(mM) = (milli/liter)
+	F = 9.6485e4   (coul)
+	R = 8.3145 (joule/degC)
+}
+
+PARAMETER {
+	v (mV)
+
+	gbar = .00005	(cm/s)
+	monovalConc = 140     (mM)
+	monovalPerm = 0
+	celsius = 35
+	cai             (milli/liter)
+	cao             (milli/liter)
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
+        modACh = 0
+        maxModACh = 1
+        levelACh = 0
+
+
+}
+
+ASSIGNED {
+	ica            (mA/cm2)
+        minf
+	mtau           (ms)
+	T              (degC)
+	E              (volts)
+	g	(S/cm2)
+}
+
+STATE {
+	m
+}
+
+INITIAL {
+	rates(v)
+	m = minf
+}
+
+BREAKPOINT {
+     SOLVE states METHOD cnexp
+	g = (1e3) * gbar * m *modulationDA()*modulationACh()
+	ica = g * ghk(v, cai, cao, 2)
+}
+
+DERIVATIVE states {
+	rates(v)
+	m' = (minf - m)/mtau
+}
+
+FUNCTION ghk( v(mV), ci(mM), co(mM), z)  (coul/cm3) { LOCAL Ci
+	T = celsius + 273.19  : Kelvin
+        E = (1e-3) * v
+        Ci = ci + (monovalPerm) * (monovalConc)        : Monovalent permeability
+	if (fabs(1-exp(-z*(F*E)/(R*T))) < 1e-6) { : denominator is small -> Taylor series
+		ghk = (1e-6) * z * F * (Ci-co*exp(-z*(F*E)/(R*T)))*(1-(z*(F*E)/(R*T)))
+	} else {
+		ghk = (1e-6) * z^2*(E*F^2)/(R*T)*(Ci-co*exp(-z*(F*E)/(R*T)))/(1-exp(-z*(F*E)/(R*T)))
+	}
+}
+
+PROCEDURE rates (v (mV)) {
+        UNITSOFF
+	minf = 1/(1+exp(-(v - (-19)) / 5.5))
+	mtau = (mtau_func(v)) * 1e3
+        UNITSON
+}
+
+FUNCTION mtau_func( v (mV) ) (ms) {
+        UNITSOFF
+        if (v > -50) {
+            mtau_func = .000191 + .00376*exp(-((v-(-41.9))/27.8)^2)
+        } else {
+            mtau_func = .00026367 + .1278 * exp(.10327*v)
+        }
+        UNITSON
+}
+
+
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+FUNCTION modulationACh() {
+    : returns modulation factor
+    
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
+}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/caq_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/caq_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/car_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/car_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/car_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,49 @@
-TITLE R-type calcium current (Cav2.3)
-
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
+TITLE LVA L-type calcium current (Cav1.3)
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX car_ms
-    USEION ca READ cai, cao WRITE ica VALENCE 2
-    RANGE pbar, ica
-    RANGE damod, maxMod
+    SUFFIX cal13_ms
+    USEION cal READ cali, calo WRITE ical VALENCE 2
+    RANGE pbar, ical
 }
 
 PARAMETER {
-    pbar = 0.0 	(cm/s)
-    :q = 1	: room temperature 22 C
-    q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    pbar = 0.0 (cm/s)
+    :q = 1	: room temperature 22-25 C
+    q = 2	: body temperature 35 C
 } 
 
 ASSIGNED { 
     v (mV)
-    ica (mA/cm2)
-    eca (mV)
+    ical (mA/cm2)
+    ecal (mV)
     celsius (degC)
-    cai (mM)
-    cao (mM)
+    cali (mM)
+    calo (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ica = pbar*m*m*m*h*ghk(v, cai, cao)*modulation()
+    ical = pbar*m*m*h*ghk(v, cali, calo)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -73,18 +52,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-29))/(-9.6)))
-    mtau = 5.1
-    hinf = 1/(1+exp((v-(-33.3))/17))
-    htau = 22+80/(1+exp((v-(-19))/5))
+    minf = 1/(1+exp((v-(-33))/(-6.7)))
+    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
+    hinf = 1/(1+exp((v-(-13.4))/11.9))
+    htau = 44.3
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -96,47 +75,53 @@
     if (fabs(z) < 1e-4) {
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
-
-
 COMMENT
 
-Original data by Foehring  et al (2000) [1] for dissociated MSNs from
-P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
-liquid junction potential was around 8 mV and was not corrected. Kinetics
-of m3h type was fitted.  Inactivation time constants were measured in
-neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
-at room temperature 22 C.
-
-Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
-<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
-activation time constant matched m^3 originally [1]. Smooth fit of
-inactivation time constant from [2,3].
-
-[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
-(2000) Unique properties of R-type calcium currents in neocortical and
-neostriatal neurons. J Neurophysiol 84(5):2225-36.
-
-[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
-biophysical characterization of voltage-gated calcium currents in the
-endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
+Activation curve was reconstructed for cultured NAc neurons from
+P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
+Fig.1D]. Activation time constant is from the rodent neuron culture (both
+rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
+curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
+at room temperature.
+
+Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
+<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
+time constant was refitted to avoid singularity.
+
+[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
+characterization of voltage-dependent Ca2+ channels in neurons isolated
+from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
+
+[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
+omega-conotoxin-sensitive calcium channels in a mammalian
+neuroblastoma-glioma cell line. J Physiol 448:161-88.
+
+[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
+Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
+properties, pharmacology, and modulation of human, neuronal L-type
+(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
+85:816-827.
 
-[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
-spike timing-dependent calcium influx during corticostriatal upstates. J
-Neurophysiol 110(7):1631-45.
+[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
+calcium influx and spike timing-dependent plasticity in striatal medium
+spiny neurons. PLoS Comput Biol 8(4):e1002493.
+
+[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
+Neurobiol 96(1):1-31.
+
+[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
+at relatively hyperpolarized membrane potentials and are incompletely
+inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
+
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cat32_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cat32_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/cat33_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cat33_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/concACh.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/concACh.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/concDA.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/concDA.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/concDAfile.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/concDAfile.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/hcn12_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod`

 * *Files 7% similar despite different names*

```diff
@@ -9,38 +9,23 @@
 
 For further details email Matt Nolan at mfnolan@fido.cpmc.columbia.edu.
 
 Reference
 
 Wang J., Chen S., Nolan M.F. and Siegelbaum S.A. (2002). Activity-dependent regulation of HCN pacemaker channels by cyclicAMP: signalling through dynamic allosteric coupling. Neuron 36, 1-20.
 ****
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
 ENDCOMMENT
 
 NEURON {
 	SUFFIX hcn12_ch
 	NONSPECIFIC_CURRENT i
 	RANGE i, ehcn, g, gbar
 	GLOBAL a0, b0, ah, bh, ac, bc, aa0, ba0
 	GLOBAL aa0, ba0, aah, bah, aac, bac
 	GLOBAL kon, koff, b, bf, ai, gca, shift
-    RANGE damod, maxMod
 }
 
 UNITS {
 	(mV) = (millivolt)
 	(molar) = (1/liter)
 	(mM) = (millimolar)
 	(mA) = (milliamp)
@@ -68,16 +53,14 @@
 	bf      = 8.94
 	ai	= 1e-05		(mM)	:concentration cyclic AMP
 	gca     = 1			: relative conductance of the bound state
 	shift   = -17		(mV)	: shift in voltage dependence
 	q10v    = 4                     : q10 value from Magee 1998
 	q10a    = 1.5			: estimated q10 for the cAMP binding reaction
 	celsius			(degC)
-    damod = 0
-    maxMod = 1
 }
 
 ASSIGNED {
 	v	(mV)
 	g	(S/cm2)
 	i	(mA/cm2)
 	alpha	(/ms)
@@ -95,15 +78,15 @@
 
 INITIAL {
 	SOLVE kin STEADYSTATE sparse
 }
 
 BREAKPOINT {
 	SOLVE kin METHOD sparse
-	g = gbar*(o + cao*gca)*modulation()
+	g = gbar*(o + cao*gca)
 	i = g*(v-ehcn)
 }
 
 KINETIC kin {
 	LOCAL qa
 	qa = q10a^((celsius-22 (degC))/10 (degC))
 	rates(v)
@@ -125,13 +108,7 @@
 	} else {
 		alpha = a0*qv / (1 + exp(-((-200)-ah-shift)*ac))
 		beta = b0*qv / (1 + exp(-((-200)-bh-shift)*bc))
 		alphaa = aa0*qv / (1 + exp(-((-200)-aah-shift)*aac))
 		betaa = ba0*qv / (1 + exp(-((-200)-bah-shift)*bac))
 	}
 }
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/im_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/im_lts.mod`

 * *Files 20% similar despite different names*

```diff
@@ -16,37 +16,49 @@
 :
 :   Written by Alain Destexhe, Laval University, 1995
 :
 
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 INDEPENDENT {t FROM 0 TO 1 WITH 1 (ms)}
 
 NEURON {
 	SUFFIX im_lts
 	USEION k READ ek WRITE ik
-    RANGE gkbar, m_inf, tau_m
+        RANGE gkbar, m_inf, tau_m, ik
 	GLOBAL taumax
-    RANGE damod, maxMod
+        RANGE modDA, maxModDA, levelDA
+	RANGE modACh, maxModACh, levelACh
 	
 
 }
 
 UNITS {
 	(mA) = (milliamp)
 	(mV) = (millivolt)
@@ -55,16 +67,20 @@
 
 PARAMETER {
 	v		(mV)
 	celsius = 36    (degC)
 	ek		(mV)
 	gkbar	= 1e-6	(mho/cm2)
 	taumax	= 1000	(ms)		: peak value of tau
-    damod = 0
-    maxMod = 1
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
+        modACh = 0
+        maxModACh = 1 
+        levelACh = 0
 }
 
 
 
 STATE {
 	m
 }
@@ -75,15 +91,15 @@
 	tau_m	(ms)
 	tau_peak	(ms)
 	tadj
 }
 
 BREAKPOINT {
 	SOLVE states METHOD cnexp
-	ik = gkbar * m * (v - ek)*modulation()
+	ik = gkbar * m * (v - ek)*modulationDA()*modulationACh()
 }
 
 DERIVATIVE states { 
 	evaluate_fct(v)
 
 	m' = (m_inf - m) / tau_m
 }
@@ -113,12 +129,18 @@
 	if ((x > -25) && (x < 25)) {
 		exptable = exp(x)
 	} else {
 		exptable = 0.
 	}
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/it_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/it_lts.mod`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 :
 :   Written by Alain Destexhe, Salk Institute, 1993; modified 1995
 :
 
 INDEPENDENT {t FROM 0 TO 1 WITH 1 (ms)}
 
 NEURON {
-	SUFFIX it_lts
+	SUFFIX it
 	USEION ca READ cai,cao WRITE ica
 	GLOBAL q10
 	RANGE gcabar, m_inf, tau_m, h_inf, tau_h, shift
 }
 
 UNITS {
 	(molar) = (1/liter)
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kaf_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_fs.mod`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 TITLE Fast A-type potassium current (Kv4.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
     SUFFIX kaf_fs
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik, q
-    RANGE damod, maxMod
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
     :q = 1	: room temperature (unspecified)
     q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -49,15 +61,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*h*modulation()
+    gk = gbar*m*m*h*modulationDA()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -74,18 +86,18 @@
     minf = 1/(1+exp((v-(-10))/(-17.7)))
     mtau = (0.9+1.1/(1+exp((v-(-30))/10)))*2
     hinf = 1/(1+exp((v-(-75.6))/11.8))
     htau = 14
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
 COMMENT
 
 Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
 dissociated from young adult rats, age P28-P42.  Electrophysiological
 recordings were done at unspecified temperature (room temperature 20-22 C
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kaf_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,26 @@
 TITLE Fast A-type potassium current (Kv4.2)
 
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-
 NEURON {
     SUFFIX kaf_ms
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik, q
-    RANGE damod, maxMod
-    
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 (S/cm2) 
     q = 1	: room temperature (unspecified)
     :q = 2	: body temperature 35 C (Du 2017)
     :q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -52,15 +30,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*h*modulation()
+    gk = gbar*m*m*h
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -93,22 +71,14 @@
     :beta = 0.065/(1+exp((v-(-55))/(-11)))
     :sum = alpha+beta
     :hinf = alpha/sum
     :htau = 1/sum
     :UNITSON
 }
 
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
-
-
 COMMENT
 
 Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
 dissociated from young adult rats, age P28-P42.  Electrophysiological
 recordings were done at unspecified temperature (room temperature 20-22 C
 assumed). Potentials were not corrected for the liquid junction potential
 (estimated 1-2 mV).
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kas_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kas_fs.mod`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,59 @@
 TITLE Slowly inactivating A-type potassium current (Kv1.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
     SUFFIX kas_fs
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik, shift, q
-    RANGE damod, maxMod
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
     a = 0.8
     :q = 1	: room temperature 22-24 C
     q = 3	: body temperature 33 C
     shift = 0
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -51,15 +63,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*(h*a+1-a)*modulation()
+    gk = gbar*m*m*(h*a+1-a)*modulationDA()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -76,18 +88,18 @@
     minf = 1/(1+exp((v-(-27)-shift)/(-16)))
     mtau = 3.4+89.2*exp(-((v-(-34.3))/30.1)^2)
     hinf = 1/(1+exp((v-(-33.5)-shift)/21.5))
     htau = 548.7*6/(exp((v-(-96))/(-29.01))+exp((v-(-96))/100))
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
 COMMENT
 
 Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
 acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
 brain. All recordings were conducted at 22-24 C. No correction for the
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kas_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_ms.mod`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,26 @@
 TITLE Slowly inactivating A-type potassium current (Kv1.2)
 
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-
 NEURON {
     SUFFIX kas_ms
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik
-    RANGE damod, maxMod
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
     a = 0.8
     :q = 1	: room temperature 22-24 C
     q = 3	: body temperature 33 C
-    damod = 0
-    maxMod = 1
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -51,15 +30,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*(h*a+1-a)*modulation()
+    gk = gbar*m*m*(h*a+1-a)
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -90,20 +69,14 @@
     :beta = 0.002/(1+exp((v-50)/(-70)))
     :sum = alpha+beta
     :hinf = a+(alpha/sum)*(1-a)
     :htau = 1/sum
     UNITSON
 }
 
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
-
 COMMENT
 
 Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
 acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
 brain. All recordings were conducted at 22-24 C. No correction for the
 liquid junction potential was reported.
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kcnq_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kdr_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kdr_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kir23_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_fs.mod`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-TITLE Noninactivating inwardly rectifying potassium current (Kir2.3)
+TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
 
 NEURON {
-
-    SUFFIX kir23_lts
+    SUFFIX kir_fs
     USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik			  
+    RANGE gbar, gk, ik, shift
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 (S/cm2) 
-    q = 1	: body temperature 35 C
-    
+    gbar = 0.0 	(S/cm2) 
+    shift = 0
+    q = 1 	: body temperature 35 C
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -44,32 +43,31 @@
 INITIAL {
     rates()
     m = minf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-82))/13))
-    :mtau = 1/(2*exp((v-(-106))/(-12.6))+0.086*exp((v-(-19))/47))  : Steephen (2009)
-    mtau = 1/(exp((v-(-97.3))/(-12.6))+exp((v-96.3)/47))  : Steephen (2009)
+    minf = 1/(1+exp((v-(-82)-shift)/13))
+    mtau = 1/(exp((v-(-103)-shift)/(-14.5))+0.125/(1+exp((v-(-35)-shift)/(-19))))
     UNITSON
 }
 
 COMMENT
 
 Original model by Wolf et al (2005) [1] for the rat MSN cells from the
 nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
 channel expressed in HEK cells [2] and shifted to match extracellular
-concentration of K in rat.  Time constants were derived from Aplysia
-data [3] and adjusted to match the rat experiments [1]. Time constant
-was further tuned [4] to fit the rat data below -80 mV [5].
-
-Non-inactivating component of the Kir channel with m1 kinetics is used
-[1,4].  Kinetics is corrected to the body temperature 35 C.
+concentration of K in rat.  Time constants were derived from Aplysia data
+[3] and adjusted to match the rat experiments [1]. Time constant was
+further tuned [4] to fit the rat data below -80 mV [5].  Kinetics is
+corrected to the body temperature 35 C.
 
+Non-inactivating Kir current was observed in cells expressing Kir2.2
+and/or Kir2.3 [5]. Activation variable with m^1 kinetics is used [1,4].
 Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
 
 [1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kir_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_lts.mod`

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,128 @@
-TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
+TITLE Fast A-type potassium current (Kv4.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
-    SUFFIX kir_fs
+    SUFFIX kaf_lts
     USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, shift
-    RANGE damod, maxMod
+    RANGE gbar, gk, ik, q
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
-    shift = 0
-    q = 1 	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    :q = 1	: room temperature (unspecified)
+    q = 3	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
     minf
     mtau (ms)
+    hinf
+    htau (ms)
 }
 
-STATE { m }
+STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*modulation()
+    gk = gbar*m*m*h*modulationDA()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
+    h' = (hinf-h)/htau*q
 }
 
 INITIAL {
     rates()
     m = minf
+    h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-82)-shift)/13))
-    mtau = 1/(exp((v-(-103)-shift)/(-14.5))+0.125/(1+exp((v-(-35)-shift)/(-19))))
+    minf = 1/(1+exp((v-(-10))/(-17.7)))
+    mtau = (0.9+1.1/(1+exp((v-(-30))/10)))*2
+    hinf = 1/(1+exp((v-(-75.6))/11.8))
+    htau = 14
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
 COMMENT
 
-Original model by Wolf et al (2005) [1] for the rat MSN cells from the
-nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
-channel expressed in HEK cells [2] and shifted to match extracellular
-concentration of K in rat.  Time constants were derived from Aplysia data
-[3] and adjusted to match the rat experiments [1]. Time constant was
-further tuned [4] to fit the rat data below -80 mV [5].  Kinetics is
-corrected to the body temperature 35 C.
-
-Non-inactivating Kir current was observed in cells expressing Kir2.2
-and/or Kir2.3 [5]. Activation variable with m^1 kinetics is used [1,4].
-Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
+Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
+dissociated from young adult rats, age P28-P42.  Electrophysiological
+recordings were done at unspecified temperature (room temperature 20-22 C
+assumed). Potentials were not corrected for the liquid junction potential
+(estimated 1-2 mV).
+
+Conductance kinetics of m2h type is used [2].  Activation m^1 matches
+experimental data [1, Fig.2C]. Activation time constants were fitted to
+tabulated data [1, Fig.2B] by Alexander Kozlov <akozlov@kth.se> and scaled
+up x2 for m2 kinetics.  Slope of inactivation function fitted to the data
+[1, Fig.3B] with half inactivation potential -75.6 mV. Temperature factor
+q between 3 [2] and 1.5 [3] was used for body temperature.
+
+[1] Tkatch T, Baranauskas G, Surmeier DJ (2000) Kv4.2 mRNA abundance and
+A-type K(+) current amplitude are linearly related in basal ganglia and
+basal forebrain neurons. J Neurosci 20(2):579-88.
 
-[1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[2] Kubo Y, Murata Y (2001) Control of rectification and permeation by
-two distinct sites after the second transmembrane region in Kir2.1 K+
-channel. J Physiol 531, 645-660.
-
-[3] Hayashi H, Fishman HM (1988) Inward rectifier K+ channel kinetics
-from analysis of the complex conductance of aplysia neuronal membrane.
-Biophys J 53, 747-757.
-
-[4] Steephen JE, Manchanda R (2009) Differences in biophysical properties
-of nucleus accumbens medium spiny neurons emerging from inactivation of
-inward rectifying potassium currents. J Comput Neurosci 27(3):453-70
-
-[5] Mermelstein PG, Song WJ, Tkatch T, Yan Z, Surmeier DJ (1998)
-Inwardly rectifying potassium (IRK) currents are correlated with IRK
-subunit expression in rat nucleus accumbens medium spiny neurons. J
-Neurosci 18(17):6650-61.
+[3]  Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
+calcium influx and spike timing-dependent plasticity in striatal medium
+spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kir_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_ch.mod`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,57 @@
-TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
+TITLE Noninactivating inwardly rectifying potassium current (Kir2.3)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
-
-
+      
 NEURON {
-    SUFFIX kir_ms
+
+    SUFFIX kir23_ch
     USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, shift
-    RANGE damod, maxMod
+    RANGE gbar, gk, ik
+    RANGE modACh, maxModACh, levelACh
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 	(S/cm2) 
-    shift = 0.0 (mV)
-    q = 1 	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    gbar = 0.0 (S/cm2) 
+    q = 1	: body temperature 35 C
+    modACh = 0
+    maxModACh = 1 
+    levelACh = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -48,15 +59,15 @@
     mtau (ms)
 }
 
 STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*modulation()
+    gk = gbar*m*modulationACh()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
 }
@@ -64,39 +75,38 @@
 INITIAL {
     rates()
     m = minf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-82)-shift)/13))
-    mtau = 1/(exp((v-(-103))/(-14.5))+0.125/(1+exp((v-(-35))/(-19))))
+    minf = 1/(1+exp((v-(-82))/13))
+    :mtau = 1/(2*exp((v-(-106))/(-12.6))+0.086*exp((v-(-19))/47))  : Steephen (2009)
+    mtau = 1/(exp((v-(-97.3))/(-12.6))+exp((v-96.3)/47))  : Steephen (2009)
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
 COMMENT
 
 Original model by Wolf et al (2005) [1] for the rat MSN cells from the
 nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
 channel expressed in HEK cells [2] and shifted to match extracellular
-concentration of K in rat. Measured half-activation values are -109.3
-mV (striatonigral MSN) and -113.2 mV (striatopallidal MSN) [6, Supp
-Tab.1]. Time constants were derived from Aplysia data [3] and adjusted
-to match the rat experiments [1]. Time constant was further tuned [4]
-to fit the rat data below -80 mV [5].  Kinetics is corrected to the body
-temperature 35 C [4].
+concentration of K in rat.  Time constants were derived from Aplysia
+data [3] and adjusted to match the rat experiments [1]. Time constant
+was further tuned [4] to fit the rat data below -80 mV [5].
+
+Non-inactivating component of the Kir channel with m1 kinetics is used
+[1,4].  Kinetics is corrected to the body temperature 35 C.
 
-Non-inactivating Kir current was observed in cells expressing Kir2.2
-and/or Kir2.3 [5]. Activation variable with m^1 kinetics is used [1,4].
 Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
 
 [1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
@@ -113,13 +123,8 @@
 inward rectifying potassium currents. J Comput Neurosci 27(3):453-70
 
 [5] Mermelstein PG, Song WJ, Tkatch T, Yan Z, Surmeier DJ (1998)
 Inwardly rectifying potassium (IRK) currents are correlated with IRK
 subunit expression in rat nucleus accumbens medium spiny neurons. J
 Neurosci 18(17):6650-61.
 
-[6] Shen W, Tian X, Day M, Ulrich S, Tkatch T, Nathanson NM, Surmeier DJ
-(2007) Cholinergic modulation of Kir2 channels selectively elevates
-dendritic excitability in striatopallidal neurons. Nat Neurosci
-10(11):1458-66.
-
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/kv2_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/na2_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/na_ch.mod`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,177 @@
-COMMENT
-NA2_CH.MOD
-
-c1 - c2 - c3 - c4 - c5 - o  - is1
-|    |    |    |    |    |
-i1 - i2 - i3 - i4 - i5 - i6 - is2
-
-FAST
-
-6/18/2003
-
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-    level  [0]: is an additional parameter for scaling modulation. 
-                    Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-
-NEURON {
-	SUFFIX na2_ch
-	USEION na READ ena WRITE ina
-	RANGE g, ina, gbar, a
-	GLOBAL Con, Coff, Oon, Ooff
-	GLOBAL a0, vha, vca
-	GLOBAL b0, vhb, vcb
-	GLOBAL g0
-	GLOBAL d0
-	GLOBAL aS1, aS2, bS
-    RANGE damod, maxMod
-}
-
-UNITS {
-	(mV) = (millivolt)
-	(mA) = (milliamp)
-	(S) = (siemens)
-}
-
-PARAMETER {
-	gbar = 1	(S/cm2)
-
-	a0 = 37		(1/ms)	: alpha
-	vha  = 45	(mV)
-	vca = 40	(mV)
-
-	b0 = 10		(1/ms)	: beta
-	vhb = -50	(mV)
-	vcb = -10	(mV)
-
-	g0 = 40		(1/ms)	: gamma
-
-	d0 = 30		(1/ms)	: delta
-
-	aS1 = 0.0025	(1/ms)
-	aS2 = 0.0002	(1/ms)
-	bS = 0.00017	(1/ms)
-
-	Con = 0.001	(1/ms)
-	Coff = 0.1	(1/ms)
-	Oon = 1.6	(1/ms)
-	Ooff = 0.01	(1/ms)
-    damod = 0
-    maxMod = 1
-}
-
-ASSIGNED {
-	v	(mV)
-	ena	(mV)
-	g	(S/cm2)
-	ina	(mA/cm2)
-	alpha	(1/ms)
-	beta	(1/ms)
-	gamma	(1/ms)
-	delta	(1/ms)
-	a
-}
-
-STATE {
-	c1  : closed
-	c2
-	c3
-	c4
-	c5
-	ct  : total closed
-	o   : open
-	i1  : fast inactivated
-	i2
-	i3
-	i4
-	i5
-	i6   
-	ift : total fast inactivated
-	is1 : slow inactivated
-	is2
-	ist : total slow inactivated
-	it  : total inactivated
-}
-
-BREAKPOINT {
-	SOLVE kin METHOD sparse
-	g = gbar*o*modulation()
-	ina = g*(v-ena)
-	ct = c1 + c2 + c3 + c4 + c5
-	ift = i1 + i2 + i3 + i4 + i5 + i6
-	ist = is1 + is2
-	it = ift + ist
-}
-
-INITIAL {
-	SOLVE kin STEADYSTATE sparse
-}
-
-KINETIC kin{
-	rates(v)
-
-	~ c1 <-> c2 (4*alpha, beta)
-	~ c2 <-> c3 (3*alpha, 2*beta)
-	~ c3 <-> c4 (2*alpha, 3*beta)
-	~ c4 <-> c5 (alpha, 4*beta)
-	~ c5 <-> o  (gamma, delta)
-	~ o <-> is1 (aS1, bS)
-
-	~ i1 <-> i2 (4*alpha*a, beta/a)
-	~ i2 <-> i3 (3*alpha*a, 2*beta/a)
-	~ i3 <-> i4 (2*alpha*a, 3*beta/a)
-	~ i4 <-> i5 (alpha*a, 4*beta/a)
-	~ i5 <-> i6 (gamma, delta)
-	~ i6 <-> is2 (aS2, bS)
-
-	~ c1 <-> i1 (Con, Coff)
-	~ c2 <-> i2 (Con*a, Coff/a)
-	~ c3 <-> i3 (Con*a^2, Coff/a^2)
-	~ c4 <-> i4 (Con*a^3, Coff/a^3)
-	~ c5 <-> i5 (Con*a^4, Coff/a^4)
-	~ o <-> i6  (Oon, Ooff)
-
-	CONSERVE c1+c2+c3+c4+c5+i1+i2+i3+i4+i5+i6+is1+is2+o=1
-}
-
-PROCEDURE rates(v(millivolt)) {
-	alpha = a0*exp((v-vha)/vca)
-	beta = b0*exp((v-vhb)/vcb)
-	gamma = g0
-	delta = d0
-
-	a = ((Coff/Con)/(Ooff/Oon))^(1/8)
-}
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
+COMMENT
+NA_CH.MOD
+
+c1 - c2 - c3 - c4 - c5 - o  - is1
+|    |    |    |    |    |
+i1 - i2 - i3 - i4 - i5 - i6 - is2
+
+SLOW
+
+6/18/2003
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
+    
+ENDCOMMENT
+
+
+
+NEURON {
+	SUFFIX na_ch
+	USEION na READ ena WRITE ina
+	RANGE g, ina, gbar, a
+	GLOBAL Con, Coff, Oon, Ooff
+	GLOBAL a0, vha, vca
+	GLOBAL b0, vhb, vcb
+	GLOBAL g0
+	GLOBAL d0
+	GLOBAL aS1, aS2, bS
+        RANGE modDA, maxModDA, levelDA
+}
+
+UNITS {
+	(mV) = (millivolt)
+	(mA) = (milliamp)
+	(S) = (siemens)
+}
+
+PARAMETER {
+	gbar = 1	(S/cm2)
+
+	a0 = 37		(1/ms)	: alpha
+	vha  = 45	(mV)
+	vca = 40	(mV)
+
+	b0 = 10		(1/ms)	: beta
+	vhb = -50	(mV)
+	vcb = -20	(mV)
+
+	g0 = 40		(1/ms)	: gamma
+
+	d0 = 30		(1/ms)	: delta
+
+	aS1 = 0.0025	(1/ms)
+	aS2 = 0.0002	(1/ms)
+	bS = 0.00017	(1/ms)
+
+	Con = 0.001	(1/ms)
+	Coff = 0.1	(1/ms)
+	Oon = .7	(1/ms)
+	Ooff = 0.01	(1/ms)
+
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
+}
+
+ASSIGNED {
+	v	(mV)
+	ena	(mV)
+	g	(S/cm2)
+	ina	(mA/cm2)
+	alpha	(1/ms)
+	beta	(1/ms)
+	gamma	(1/ms)
+	delta	(1/ms)
+	a
+}
+
+STATE {
+	c1  : closed
+	c2
+	c3
+	c4
+	c5
+	ct  : total closed
+	o   : open
+	i1  : fast inactivated
+	i2
+	i3
+	i4
+	i5
+	i6
+	ift : total fast inactivated
+	is1 : slow inactivated
+	is2
+	ist : total slow inactivated
+	it  : total inactivated
+}
+
+BREAKPOINT {
+	SOLVE kin METHOD sparse
+	g = gbar*o*modulationDA()
+	ina = g*(v-ena)
+	ct = c1 + c2 + c3 + c4 + c5
+	ift = i1 + i2 + i3 + i4 + i5 + i6
+	ist = is1 + is2
+	it = ift + ist
+}
+
+INITIAL {
+	SOLVE kin STEADYSTATE sparse
+}
+
+KINETIC kin{
+	rates(v)
+
+	~ c1 <-> c2 (4*alpha, beta)
+	~ c2 <-> c3 (3*alpha, 2*beta)
+	~ c3 <-> c4 (2*alpha, 3*beta)
+	~ c4 <-> c5 (alpha, 4*beta)
+	~ c5 <-> o  (gamma, delta)
+	~ o <-> is1 (aS1, bS)
+
+	~ i1 <-> i2 (4*alpha*a, beta/a)
+	~ i2 <-> i3 (3*alpha*a, 2*beta/a)
+	~ i3 <-> i4 (2*alpha*a, 3*beta/a)
+	~ i4 <-> i5 (alpha*a, 4*beta/a)
+	~ i5 <-> i6 (gamma, delta)
+	~ i6 <-> is2 (aS2, bS)
+
+	~ c1 <-> i1 (Con, Coff)
+	~ c2 <-> i2 (Con*a, Coff/a)
+	~ c3 <-> i3 (Con*a^2, Coff/a^2)
+	~ c4 <-> i4 (Con*a^3, Coff/a^3)
+	~ c5 <-> i5 (Con*a^4, Coff/a^4)
+	~ o <-> i6  (Oon, Ooff)
+
+	CONSERVE c1+c2+c3+c4+c5+i1+i2+i3+i4+i5+i6+is1+is2+o=1
+
+}
+
+PROCEDURE rates(v(millivolt)) {
+	alpha = a0*exp((v-vha)/vca)
+	beta = b0*exp((v-vhb)/vcb)
+	gamma = g0
+	delta = d0
+
+	a = ((Coff/Con)/(Ooff/Oon))^(1/8)
+}
+
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/na3n_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod`

 * *Files 22% similar despite different names*

```diff
@@ -1,156 +1,132 @@
-TITLE na3
-: Na current 
-: modified from Jeff Magee. M.Migliore may97
-: added sh to account for higher threshold M.Migliore, Apr.2002
-
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-NEURON {
-	SUFFIX na3_lts
-	USEION na READ ena WRITE ina
-	RANGE  gbar, ar, sh
-	GLOBAL minf, hinf, mtau, htau, sinf, taus,qinf, thinf
-	RANGE damod, maxMod
-}
-
-PARAMETER {
-	sh   = 0	(mV)
-	gbar = 0.010   	(mho/cm2)	
-								
-	tha  =  -30	(mV)		: v 1/2 for act	
-	qa   = 7.2	(mV)		: act slope (4.5)		
-	Ra   = 0.4	(/ms)		: open (v)		
-	Rb   = 0.124 	(/ms)		: close (v)		
-
-	thi1  = -45	(mV)		: v 1/2 for inact 	
-	thi2  = -45 	(mV)		: v 1/2 for inact 	
-	qd   = 1.5	(mV)	        : inact tau slope
-	qg   = 1.5      (mV)
-	mmin=0.02	
-	hmin=0.5			
-	q10=2
-	Rg   = 0.01 	(/ms)		: inact recov (v) 	
-	Rd   = .03 	(/ms)		: inact (v)	
-	qq   = 10        (mV)
-	tq   = -55      (mV)
-
-	thinf  = -50 	(mV)		: inact inf slope	
-	qinf  = 4 	(mV)		: inact inf slope 
-
-        vhalfs=-60	(mV)		: slow inact.
-        a0s=0.0003	(ms)		: a0s=b0s
-        zetas=12	(1)
-        gms=0.2		(1)
-        smax=10		(ms)
-        vvh=-58		(mV) 
-        vvs=2		(mV)
-        ar=1		(1)		: 1=no inact., 0=max inact.
-	ena		(mV)            : must be explicitly def. in hoc
-	celsius
-	v 		(mV)
-    damod = 0
-    maxMod = 1
-}
-
-
-UNITS {
-	(mA) = (milliamp)
-	(mV) = (millivolt)
-	(pS) = (picosiemens)
-	(um) = (micron)
-} 
-
-ASSIGNED {
-	ina 		(mA/cm2)
-	thegna		(mho/cm2)
-	minf 		hinf 		
-	mtau (ms)	htau (ms) 	
-	sinf (ms)	taus (ms)
-}
- 
-
-STATE { m h s}
-
-BREAKPOINT {
-    SOLVE states METHOD cnexp
-    thegna = gbar*m*m*m*h*s*modulation()
-	ina = thegna * (v - ena)
-} 
-
-INITIAL {
-	trates(v,ar,sh)
-	m=minf  
-	h=hinf
-	s=sinf
-}
-
-
-FUNCTION alpv(v(mV)) {
-         alpv = 1/(1+exp((v-vvh-sh)/vvs))
-}
-        
-FUNCTION alps(v(mV)) {  
-  alps = exp(1.e-3*zetas*(v-vhalfs-sh)*9.648e4/(8.315*(273.16+celsius)))
-}
-
-FUNCTION bets(v(mV)) {
-  bets = exp(1.e-3*zetas*gms*(v-vhalfs-sh)*9.648e4/(8.315*(273.16+celsius)))
-}
-
-LOCAL mexp, hexp, sexp
-
-DERIVATIVE states {   
-        trates(v,ar,sh)      
-        m' = (minf-m)/mtau
-        h' = (hinf-h)/htau
-        s' = (sinf - s)/taus
-}
-
-PROCEDURE trates(vm,a2,sh2) {  
-        LOCAL  a, b, c, qt
-        qt=q10^((celsius-24)/10)
-	a = trap0(vm,tha+sh2,Ra,qa)
-	b = trap0(-vm,-tha-sh2,Rb,qa)
-	mtau = (1/(a+b))/qt
-        if (mtau<mmin) {mtau=mmin}
-	minf = a/(a+b)
-
-	a = trap0(vm,thi1+sh2,Rd,qd)
-	b = trap0(-vm,-thi2-sh2,Rg,qg)
-	htau =  (1/(a+b))/qt
-        if (htau<hmin) {htau=hmin}
-	hinf = 1/(1+exp((vm-thinf-sh2)/qinf))
-	c=alpv(vm)
-        sinf = c+a2*(1-c)
-        taus = bets(vm)/(a0s*(1+alps(vm)))
-        if (taus<smax) {taus=smax}
-}
-
-FUNCTION trap0(v,th,a,q) {
-	if (fabs(v-th) > 1e-6) {
-	        trap0 = a * (v - th) / (1 - exp(-(v - th)/q))
-	} else {
-	        trap0 = a * q
- 	}
-}	
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}   
+TITLE na3
+: Na current 
+: modified from Jeff Magee. M.Migliore may97
+: added sh to account for higher threshold M.Migliore, Apr.2002
+
+NEURON {
+	SUFFIX na3
+	USEION na READ ena WRITE ina
+	RANGE  gbar, ar, sh
+	GLOBAL minf, hinf, mtau, htau, sinf, taus,qinf, thinf
+}
+
+PARAMETER {
+	sh   = 0	(mV)
+	gbar = 0.010   	(mho/cm2)	
+								
+	tha  =  -30	(mV)		: v 1/2 for act	
+	qa   = 7.2	(mV)		: act slope (4.5)		
+	Ra   = 0.4	(/ms)		: open (v)		
+	Rb   = 0.124 	(/ms)		: close (v)		
+
+	thi1  = -45	(mV)		: v 1/2 for inact 	
+	thi2  = -45 	(mV)		: v 1/2 for inact 	
+	qd   = 1.5	(mV)	        : inact tau slope
+	qg   = 1.5      (mV)
+	mmin=0.02	
+	hmin=0.5			
+	q10=2
+	Rg   = 0.01 	(/ms)		: inact recov (v) 	
+	Rd   = .03 	(/ms)		: inact (v)	
+	qq   = 10        (mV)
+	tq   = -55      (mV)
+
+	thinf  = -50 	(mV)		: inact inf slope	
+	qinf  = 4 	(mV)		: inact inf slope 
+
+        vhalfs=-60	(mV)		: slow inact.
+        a0s=0.0003	(ms)		: a0s=b0s
+        zetas=12	(1)
+        gms=0.2		(1)
+        smax=10		(ms)
+        vvh=-58		(mV) 
+        vvs=2		(mV)
+        ar=1		(1)		: 1=no inact., 0=max inact.
+	ena		(mV)            : must be explicitly def. in hoc
+	celsius
+	v 		(mV)
+}
+
+
+UNITS {
+	(mA) = (milliamp)
+	(mV) = (millivolt)
+	(pS) = (picosiemens)
+	(um) = (micron)
+} 
+
+ASSIGNED {
+	ina 		(mA/cm2)
+	thegna		(mho/cm2)
+	minf 		hinf 		
+	mtau (ms)	htau (ms) 	
+	sinf (ms)	taus (ms)
+}
+ 
+
+STATE { m h s}
+
+BREAKPOINT {
+        SOLVE states METHOD cnexp
+        thegna = gbar*m*m*m*h*s
+	ina = thegna * (v - ena)
+} 
+
+INITIAL {
+	trates(v,ar,sh)
+	m=minf  
+	h=hinf
+	s=sinf
+}
+
+
+FUNCTION alpv(v(mV)) {
+         alpv = 1/(1+exp((v-vvh-sh)/vvs))
+}
+        
+FUNCTION alps(v(mV)) {  
+  alps = exp(1.e-3*zetas*(v-vhalfs-sh)*9.648e4/(8.315*(273.16+celsius)))
+}
+
+FUNCTION bets(v(mV)) {
+  bets = exp(1.e-3*zetas*gms*(v-vhalfs-sh)*9.648e4/(8.315*(273.16+celsius)))
+}
+
+LOCAL mexp, hexp, sexp
+
+DERIVATIVE states {   
+        trates(v,ar,sh)      
+        m' = (minf-m)/mtau
+        h' = (hinf-h)/htau
+        s' = (sinf - s)/taus
+}
+
+PROCEDURE trates(vm,a2,sh2) {  
+        LOCAL  a, b, c, qt
+        qt=q10^((celsius-24)/10)
+	a = trap0(vm,tha+sh2,Ra,qa)
+	b = trap0(-vm,-tha-sh2,Rb,qa)
+	mtau = (1/(a+b))/qt
+        if (mtau<mmin) {mtau=mmin}
+	minf = a/(a+b)
+
+	a = trap0(vm,thi1+sh2,Rd,qd)
+	b = trap0(-vm,-thi2-sh2,Rg,qg)
+	htau =  (1/(a+b))/qt
+        if (htau<hmin) {htau=hmin}
+	hinf = 1/(1+exp((vm-thinf-sh2)/qinf))
+	c=alpv(vm)
+        sinf = c+a2*(1-c)
+        taus = bets(vm)/(a0s*(1+alps(vm)))
+        if (taus<smax) {taus=smax}
+}
+
+FUNCTION trap0(v,th,a,q) {
+	if (fabs(v-th) > 1e-6) {
+	        trap0 = a * (v - th) / (1 - exp(-(v - th)/q))
+	} else {
+	        trap0 = a * q
+ 	}
+}	
+
+
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/na_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/na2_ch.mod`

 * *Files 26% similar despite different names*

```diff
@@ -1,163 +1,174 @@
-COMMENT
-NA_CH.MOD
-
-c1 - c2 - c3 - c4 - c5 - o  - is1
-|    |    |    |    |    |
-i1 - i2 - i3 - i4 - i5 - i6 - is2
-
-SLOW
-
-6/18/2003
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-
-
-NEURON {
-	SUFFIX na_ch
-	USEION na READ ena WRITE ina
-	RANGE g, ina, gbar, a
-	GLOBAL Con, Coff, Oon, Ooff
-	GLOBAL a0, vha, vca
-	GLOBAL b0, vhb, vcb
-	GLOBAL g0
-	GLOBAL d0
-	GLOBAL aS1, aS2, bS
-    RANGE damod, maxMod
-}
-
-UNITS {
-	(mV) = (millivolt)
-	(mA) = (milliamp)
-	(S) = (siemens)
-}
-
-PARAMETER {
-	gbar = 1	(S/cm2)
-
-	a0 = 37		(1/ms)	: alpha
-	vha  = 45	(mV)
-	vca = 40	(mV)
-
-	b0 = 10		(1/ms)	: beta
-	vhb = -50	(mV)
-	vcb = -20	(mV)
-
-	g0 = 40		(1/ms)	: gamma
-
-	d0 = 30		(1/ms)	: delta
-
-	aS1 = 0.0025	(1/ms)
-	aS2 = 0.0002	(1/ms)
-	bS = 0.00017	(1/ms)
-
-	Con = 0.001	(1/ms)
-	Coff = 0.1	(1/ms)
-	Oon = .7	(1/ms)
-	Ooff = 0.01	(1/ms)
-    damod = 0
-    maxMod = 1
-}
-
-ASSIGNED {
-	v	(mV)
-	ena	(mV)
-	g	(S/cm2)
-	ina	(mA/cm2)
-	alpha	(1/ms)
-	beta	(1/ms)
-	gamma	(1/ms)
-	delta	(1/ms)
-	a
-}
-
-STATE {
-	c1  : closed
-	c2
-	c3
-	c4
-	c5
-	ct  : total closed
-	o   : open
-	i1  : fast inactivated
-	i2
-	i3
-	i4
-	i5
-	i6
-	ift : total fast inactivated
-	is1 : slow inactivated
-	is2
-	ist : total slow inactivated
-	it  : total inactivated
-}
-
-BREAKPOINT {
-	SOLVE kin METHOD sparse
-	g = gbar*o*modulation()
-	ina = g*(v-ena)
-	ct = c1 + c2 + c3 + c4 + c5
-	ift = i1 + i2 + i3 + i4 + i5 + i6
-	ist = is1 + is2
-	it = ift + ist
-}
-
-INITIAL {
-	SOLVE kin STEADYSTATE sparse
-}
-
-KINETIC kin{
-	rates(v)
-
-	~ c1 <-> c2 (4*alpha, beta)
-	~ c2 <-> c3 (3*alpha, 2*beta)
-	~ c3 <-> c4 (2*alpha, 3*beta)
-	~ c4 <-> c5 (alpha, 4*beta)
-	~ c5 <-> o  (gamma, delta)
-	~ o <-> is1 (aS1, bS)
-
-	~ i1 <-> i2 (4*alpha*a, beta/a)
-	~ i2 <-> i3 (3*alpha*a, 2*beta/a)
-	~ i3 <-> i4 (2*alpha*a, 3*beta/a)
-	~ i4 <-> i5 (alpha*a, 4*beta/a)
-	~ i5 <-> i6 (gamma, delta)
-	~ i6 <-> is2 (aS2, bS)
-
-	~ c1 <-> i1 (Con, Coff)
-	~ c2 <-> i2 (Con*a, Coff/a)
-	~ c3 <-> i3 (Con*a^2, Coff/a^2)
-	~ c4 <-> i4 (Con*a^3, Coff/a^3)
-	~ c5 <-> i5 (Con*a^4, Coff/a^4)
-	~ o <-> i6  (Oon, Ooff)
-
-	CONSERVE c1+c2+c3+c4+c5+i1+i2+i3+i4+i5+i6+is1+is2+o=1
-
-}
-
-PROCEDURE rates(v(millivolt)) {
-	alpha = a0*exp((v-vha)/vca)
-	beta = b0*exp((v-vhb)/vcb)
-	gamma = g0
-	delta = d0
-
-	a = ((Coff/Con)/(Ooff/Oon))^(1/8)
-}
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
+COMMENT
+NA2_CH.MOD
+
+c1 - c2 - c3 - c4 - c5 - o  - is1
+|    |    |    |    |    |
+i1 - i2 - i3 - i4 - i5 - i6 - is2
+
+FAST
+
+6/18/2003
+
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
+ENDCOMMENT
+
+
+NEURON {
+	SUFFIX na2_ch
+	USEION na READ ena WRITE ina
+	RANGE g, ina, gbar, a
+	GLOBAL Con, Coff, Oon, Ooff
+	GLOBAL a0, vha, vca
+	GLOBAL b0, vhb, vcb
+	GLOBAL g0
+	GLOBAL d0
+	GLOBAL aS1, aS2, bS
+	RANGE modDA, maxModDA, levelDA
+}
+
+UNITS {
+	(mV) = (millivolt)
+	(mA) = (milliamp)
+	(S) = (siemens)
+}
+
+PARAMETER {
+	gbar = 1	(S/cm2)
+
+	a0 = 37		(1/ms)	: alpha
+	vha  = 45	(mV)
+	vca = 40	(mV)
+
+	b0 = 10		(1/ms)	: beta
+	vhb = -50	(mV)
+	vcb = -10	(mV)
+
+	g0 = 40		(1/ms)	: gamma
+
+	d0 = 30		(1/ms)	: delta
+
+	aS1 = 0.0025	(1/ms)
+	aS2 = 0.0002	(1/ms)
+	bS = 0.00017	(1/ms)
+
+	Con = 0.001	(1/ms)
+	Coff = 0.1	(1/ms)
+	Oon = 1.6	(1/ms)
+	Ooff = 0.01	(1/ms)
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
+}
+
+ASSIGNED {
+	v	(mV)
+	ena	(mV)
+	g	(S/cm2)
+	ina	(mA/cm2)
+	alpha	(1/ms)
+	beta	(1/ms)
+	gamma	(1/ms)
+	delta	(1/ms)
+	a
+}
+
+STATE {
+	c1  : closed
+	c2
+	c3
+	c4
+	c5
+	ct  : total closed
+	o   : open
+	i1  : fast inactivated
+	i2
+	i3
+	i4
+	i5
+	i6   
+	ift : total fast inactivated
+	is1 : slow inactivated
+	is2
+	ist : total slow inactivated
+	it  : total inactivated
+}
+
+BREAKPOINT {
+	SOLVE kin METHOD sparse
+	g = gbar*o*modulationDA()
+	ina = g*(v-ena)
+	ct = c1 + c2 + c3 + c4 + c5
+	ift = i1 + i2 + i3 + i4 + i5 + i6
+	ist = is1 + is2
+	it = ift + ist
+}
+
+INITIAL {
+	SOLVE kin STEADYSTATE sparse
+}
+
+KINETIC kin{
+	rates(v)
+
+	~ c1 <-> c2 (4*alpha, beta)
+	~ c2 <-> c3 (3*alpha, 2*beta)
+	~ c3 <-> c4 (2*alpha, 3*beta)
+	~ c4 <-> c5 (alpha, 4*beta)
+	~ c5 <-> o  (gamma, delta)
+	~ o <-> is1 (aS1, bS)
+
+	~ i1 <-> i2 (4*alpha*a, beta/a)
+	~ i2 <-> i3 (3*alpha*a, 2*beta/a)
+	~ i3 <-> i4 (2*alpha*a, 3*beta/a)
+	~ i4 <-> i5 (alpha*a, 4*beta/a)
+	~ i5 <-> i6 (gamma, delta)
+	~ i6 <-> is2 (aS2, bS)
+
+	~ c1 <-> i1 (Con, Coff)
+	~ c2 <-> i2 (Con*a, Coff/a)
+	~ c3 <-> i3 (Con*a^2, Coff/a^2)
+	~ c4 <-> i4 (Con*a^3, Coff/a^3)
+	~ c5 <-> i5 (Con*a^4, Coff/a^4)
+	~ o <-> i6  (Oon, Ooff)
+
+	CONSERVE c1+c2+c3+c4+c5+i1+i2+i3+i4+i5+i6+is1+is2+o=1
+}
+
+PROCEDURE rates(v(millivolt)) {
+	alpha = a0*exp((v-vha)/vca)
+	beta = b0*exp((v-vhb)/vcb)
+	gamma = g0
+	delta = d0
+
+	a = ((Coff/Con)/(Ooff/Oon))^(1/8)
+}
+
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/naf_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod`

 * *Files 25% similar despite different names*

```diff
@@ -1,107 +1,103 @@
-TITLE Fast transient sodium current
-
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-    
-ENDCOMMENT
-
-NEURON {
-    SUFFIX naf_fs
-    USEION na READ ena WRITE ina
-    RANGE gbar, gna, ina, q
-    RANGE damod, maxMod
-}
+TITLE T-type calcium current (Cav3.2)
 
 UNITS {
-    (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
+    (S) = (siemens)
+    (molar) = (1/liter)
+    (mM) = (millimolar)
+    FARADAY = (faraday) (coulomb)
+    R = (k-mole) (joule/degC)
 }
 
-PARAMETER {
-    gbar = 0.0 	(S/cm2) 
-    :q = 1	: room temperature 22 C
-    q = 1.8	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+NEURON {
+    SUFFIX cat32_ms
+    USEION cal READ cali, calo WRITE ical VALENCE 2
+    RANGE pbar, ical
 }
 
-ASSIGNED {
+PARAMETER {
+    pbar = 0.0 (cm/s)
+    :q = 1	: room temperature 21 C
+    q = 3	: body temperature 35 C
+} 
+
+ASSIGNED { 
     v (mV)
-    ena (mV)
-    ina (mA/cm2)
-    gna (S/cm2)
+    ical (mA/cm2)
+    ecal (mV)
+    celsius (degC)
+    cali (mM)
+    calo (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gna = gbar*m*m*m*h*modulation()
-    ina = gna*(v-ena)
-}
-
-DERIVATIVE states {
-    rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+    ical = pbar*m*m*m*h*ghk(v, cali, calo)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
 
+DERIVATIVE states { 
+    rates()
+    m' = (minf-m)/mtau*q
+    h' = (hinf-h)/htau*q
+}
+
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-25))/(-10)))
-    mtau = 0.33+1/(exp((v-(-62))/14)+exp((v-(-60))/(-17)))
-    hinf = 1/(1+exp((v-(-62))/6))
-    htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
+    minf = 1/(1+exp((v-(-54))/(-7.8)))
+    mtau = (2.1+23/(1+exp((v-(-61))/6)))*3
+    hinf = 1/(1+exp((v-(-64.2))/8.8))
+    htau = 30+280/(1+exp((v-(-52))/7))
     UNITSON
 }
 
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
+FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
+    LOCAL z, eci, eco
+    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
+    if(z == 0) {
+        z = z+1e-6
+    }
+    eco = co*(z)/(exp(z)-1)
+    eci = ci*(-z)/(exp(-z)-1)
+    ghk = (1e-3)*2*FARADAY*(eci-eco)
 }
 
 COMMENT
 
-Original data by Ogata and Tatebayashi (1990) [1]. Neostriatal neurons
-of medium size (putative medium spiny neurons) freshly isolated from
-the adult guinea pig brain (either sex, 200 g). Data compensated for
-the liquid junction potential (-13 mV). Experiments carried out at room
-temperature (22 C). Conductance fitted by m3h kinetics.
-
-Smooth fit of mtau and htau data [1] by Alexander Kozlov <akozlov@kth.se>
-assuming natural logarithm of tau values [1, Figs. 5 and 9] and
-temperature correction factor of 1.8-2.1 [2] as suggested by Robert
-Lindroos <robert.lindroos@ki.se>.
-
-[1] Ogata N, Tatebayashi H (1990) Sodium current kinetics in freshly
-isolated neostriatal neurones of the adult guinea pig. Pflugers Arch
-416(5):594-603.
-
-[2] Schwarz JR (1986) The effect of temperature on Na currents in rat
-myelinated nerve fibres. Pflugers Arch. 406(4):397-404.
+Rat Cav3.2 channels were isolated and transfection of human embryonic
+kidney cells was performed [1].  Electrophysiological recordings were
+done in 21 C.
+
+NEURON model by Alexander Kozlov <akozlov@kth.se>. Kinetics of m3h
+type was used [2-4]. Activation time constant was scaled up accordingly.
+
+[1] Iftinca M, McKay BE, Snutch TP, McRory JE, Turner RW, Zamponi
+GW (2006) Temperature dependence of T-type calcium channel
+gating. Neuroscience 142(4):1031-42.
+
+[2] Crunelli V, Toth TI, Cope DW, Blethyn K, Hughes SW (2005) The
+'window' T-type calcium current in brain dynamics of different behavioural
+states. J Physiol 562(Pt 1):121-9.
+
+[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
+and entrainment to oscillations in a computational model of the nucleus
+accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
+
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/naf_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_fs.mod`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,57 @@
 TITLE Fast transient sodium current
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
-    SUFFIX naf_lts
+    SUFFIX naf_fs
     USEION na READ ena WRITE ina
-    RANGE gbar, gna, ina
-    RANGE maxMod
-
+    RANGE gbar, gna, ina, q
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 (S/cm2) 
+    gbar = 0.0 	(S/cm2) 
     :q = 1	: room temperature 22 C
     q = 1.8	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ena (mV)
     ina (mA/cm2)
     gna (S/cm2)
@@ -50,15 +61,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gna = gbar*m*m*m*h
+    gna = gbar*m*m*m*h*modulationDA()
     ina = gna*(v-ena)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -68,38 +79,39 @@
     rates()
     m = minf
     h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    :minf = 1/(1+exp((v-(-25.5))/(-9.2)))
-    :mtau = 0.33+1/(exp((v-(-62))/14)+exp((v-(-60))/(-17)))
-    :hinf = 1/(1+exp((v-(-63.2))/6))
-    :htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
     minf = 1/(1+exp((v-(-25))/(-10)))
     mtau = 0.33+1/(exp((v-(-62))/14)+exp((v-(-60))/(-17)))
     hinf = 1/(1+exp((v-(-62))/6))
     htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
     UNITSON
 }
 
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
 
 COMMENT
 
 Original data by Ogata and Tatebayashi (1990) [1]. Neostriatal neurons
 of medium size (putative medium spiny neurons) freshly isolated from
 the adult guinea pig brain (either sex, 200 g). Data compensated for
 the liquid junction potential (-13 mV). Experiments carried out at room
 temperature (22 C). Conductance fitted by m3h kinetics.
 
 Smooth fit of mtau and htau data [1] by Alexander Kozlov <akozlov@kth.se>
 assuming natural logarithm of tau values [1, Figs. 5 and 9] and
-temperature correction factor of 1.8 [2] as suggested by Robert Lindroos
-<robert.lindroos@ki.se>.
+temperature correction factor of 1.8-2.1 [2] as suggested by Robert
+Lindroos <robert.lindroos@ki.se>.
 
 [1] Ogata N, Tatebayashi H (1990) Sodium current kinetics in freshly
 isolated neostriatal neurones of the adult guinea pig. Pflugers Arch
 416(5):594-603.
 
 [2] Schwarz JR (1986) The effect of temperature on Na currents in rat
 myelinated nerve fibres. Pflugers Arch. 406(4):397-404.
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/naf_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_ms.mod`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 TITLE Fast transient sodium current
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
-    
+
 ENDCOMMENT
 
 NEURON {
     SUFFIX naf_ms
     USEION na READ ena WRITE ina
     RANGE gbar, gna, ina
-    RANGE damod, maxMod
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 (S/cm2) 
     :q = 1	: room temperature 22 C
     q = 1.8	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1 
+    levelACh = 0
 }
 
 ASSIGNED {
     v (mV)
     ena (mV)
     ina (mA/cm2)
     gna (S/cm2)
@@ -49,15 +65,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gna = gbar*m*m*m*h*modulation()
+    gna = gbar*m*m*m*h*modulationDA()*modulationACh()
     ina = gna*(v-ena)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -78,18 +94,24 @@
     minf = 1/(1+exp((v-(-25))/(-10)))
     mtau = 0.33+1/(exp((v-(-62))/14)+exp((v-(-60))/(-17)))
     hinf = 1/(1+exp((v-(-62))/6))
     htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
 COMMENT
 
 Original data by Ogata and Tatebayashi (1990) [1]. Neostriatal neurons
 of medium size (putative medium spiny neurons) freshly isolated from
 the adult guinea pig brain (either sex, 200 g). Data compensated for
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/sk_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/sk_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/sk_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/sk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmampa.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmgabaa.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmgabaa.mod`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,14 @@
 TITLE GABA_A synapse with short-term plasticity
 
-COMMENT
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-
-ENDCOMMENT
-
 NEURON {
     POINT_PROCESS tmGabaA
     RANGE tau1, tau2, e, i, q
     RANGE tau, tauR, tauF, U, u0
-    RANGE failRate, damod, maxMod
+    RANGE failRate
     NONSPECIFIC_CURRENT i
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
     (uS) = (microsiemens)
@@ -37,18 +20,15 @@
     tau2 = 3.75 (ms)  : ORIG: 7.5ms, tau2 > tau1
     e = -65 (mV)
     tau = 3 (ms)
     tauR = 500 (ms)  : tauR > tau
     tauF = 0 (ms)    : tauF >= 0
     U = 0.1 (1) <0, 1>
     u0 = 0 (1) <0, 1>
-    failRate = 0	
-    damod = 0
-    maxMod = 1
-
+    failRate = 0
 }
 
 ASSIGNED {
     v (mV)
     i (nA)
     g (uS)
     factor
@@ -67,15 +47,15 @@
     tp = (tau1*tau2)/(tau2-tau1) * log(tau2/tau1)
     factor = -exp(-tp/tau1) + exp(-tp/tau2)
     factor = 1/factor
 }
 
 BREAKPOINT {
     SOLVE state METHOD cnexp
-    g = (B - A) * modulation()
+    g = B - A
     i = g*(v - e)
 }
 
 DERIVATIVE state {
     A' = -A/tau1
     B' = -B/tau2
 }
@@ -111,21 +91,14 @@
     }
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
-
-FUNCTION modulation() {
-    : returns modulation factor
-    
-    modulation = 1 + damod*(maxMod-1)
-}
-
 COMMENT
 
 (2019-11-25) Synaptic failure rate (failRate) added. Random factor, no
 reproducibility guaranteed in parallel sim.
 
 (2019-09-12) Set GABA reversal potential to -65mV
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmglut.mod`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,22 @@
 TITLE Glutamatergic synapse with short-term plasticity (stp)
 
 COMMENT
 stp can be turned of by setting use_stp == 0
-
---------------------------------------------
-
-neuromodulation is added as functions:
-    
-    modulation = 1 + damod*(maxMod-1)
-
-where:
-    
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
-[] == default values
-{} == ranges
-
 ENDCOMMENT
 
 NEURON {
     THREADSAFE
     POINT_PROCESS tmGlut
     RANGE tau1_ampa, tau2_ampa, tau1_nmda, tau2_nmda
     RANGE g_ampa, g_nmda, i_ampa, i_nmda, nmda_ratio
     RANGE e, g, i, q, mg
     RANGE tau, tauR, tauF, U, u0
     RANGE ca_ratio_ampa, ca_ratio_nmda, mggate, use_stp
-    RANGE failRate, damod, maxModAMPA, maxModNMDA
+    RANGE failRate
     NONSPECIFIC_CURRENT i
     USEION cal WRITE ical VALENCE 2
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
@@ -52,20 +36,17 @@
     tauR = 100 (ms)  : tauR > tau
     tauF = 800 (ms)  : tauF >= 0
     U = 0.3 (1) <0, 1>
     u0 = 0 (1) <0, 1>
     ca_ratio_ampa = 0.005
     ca_ratio_nmda = 0.1
     mg = 1 (mM)
-    damod = 0
-    maxModNMDA = 1
-    maxModAMPA = 1
 
     use_stp = 1     : to turn of use_stp -> use 0
-    failRate = 0
+    failRate = 0	
 }
 
 ASSIGNED {
     v (mV)
     i (nA)
     i_ampa (nA)
     i_nmda (nA)
@@ -106,22 +87,22 @@
 
 BREAKPOINT {
     LOCAL itot_nmda, itot_ampa, mggate
     SOLVE state METHOD cnexp
     
     : NMDA
     mggate    = 1 / (1 + exp(-0.062 (/mV) * v) * (mg / 3.57 (mM)))
-    g_nmda    = (B_nmda - A_nmda) * modNMDA()
+    g_nmda    = B_nmda - A_nmda
     itot_nmda = g_nmda * (v - e) * mggate
     ical_nmda = ca_ratio_nmda*itot_nmda
     i_nmda    = itot_nmda - ical_nmda
     
     : AMPA
-    g_ampa    = (B_ampa - A_ampa) * modAMPA()
-    itot_ampa = g_ampa*(v - e) 
+    g_ampa    = B_ampa - A_ampa
+    itot_ampa = g_ampa*(v - e)
     ical_ampa = ca_ratio_ampa*itot_ampa
     i_ampa    = itot_ampa - ical_ampa
     
     : total values
     ical      = ical_nmda + ical_ampa
     g         = g_ampa + g_nmda
     i         = i_ampa + i_nmda
@@ -187,28 +168,14 @@
     }
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
-
-FUNCTION modAMPA() {
-    : returns modulation factor
-    
-    modAMPA = 1 + damod*(maxModAMPA-1)
-}
-
-
-FUNCTION modNMDA() {
-    : returns modulation factor
-    
-    modNMDA = 1 + damod*(maxModNMDA-1)
-}
-
 COMMENT
 (2019-11-29) Synaptic failure rate (fail) added. Random factor, no
 reproducibility guaranteed in parallel sim.
 
 (2019-08-21) We normalise the activation by U, to make sure that g specifies
              the conductance of the first actvation
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_M1RH_D1.mod`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,52 @@
 TITLE Glutamatergic synapse with short-term plasticity (stp)
 
 COMMENT
 stp can be turned of by setting use_stp == 0
 
 --------------------------------------------
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
 
 ENDCOMMENT
 
 NEURON {
     THREADSAFE
     POINT_PROCESS tmGlut_M1RH_D1
     RANGE tau1_ampa, tau2_ampa, tau1_nmda, tau2_nmda
     RANGE g_ampa, g_nmda, i_ampa, i_nmda, nmda_ratio
     RANGE e, g, i, q, mg
     RANGE tau, tauR, tauF, U, u0
     RANGE ca_ratio_ampa, ca_ratio_nmda, mggate, use_stp
-    RANGE failRate, damod, maxModAMPA, maxModNMDA
+    RANGE modDA, maxMod_AMPADA, levelDA, maxMod_AMPAACh, levelACh
+    RANGE maxMod_NMDADA, modACh, maxMod_NMDAACh
     NONSPECIFIC_CURRENT i
+    RANGE failRateDA, failRateACh, failRate
     USEION cal WRITE ical VALENCE 2
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
     (uS) = (microsiemens)
@@ -54,20 +67,31 @@
     tauR = 100 (ms)  : tauR > tau
     tauF = 800 (ms)  : tauF >= 0
     U = 0.3 (1) <0, 1>
     u0 = 0 (1) <0, 1>
     ca_ratio_ampa = 0.005
     ca_ratio_nmda = 0.1
     mg = 1 (mM)
-    damod = 0
-    maxModNMDA = 1
-    maxModAMPA = 1
 
-    use_stp = 1     : to turn of use_stp -> use 0
     failRate = 0
+    maxMod_AMPADA = 1
+    levelDA = 0
+    
+    maxMod_AMPAACh = 1 
+
+    modDA = 0
+    maxMod_NMDADA = 1
+    
+    modACh = 0
+    maxMod_NMDAACh = 1
+    levelACh = 0
+
+    failRateDA = 0
+    failRateACh = 0
+    use_stp = 1     : to turn of use_stp -> use 0
 }
 
 ASSIGNED {
     v (mV)
     i (nA)
     i_ampa (nA)
     i_nmda (nA)
@@ -112,21 +136,21 @@
 
 BREAKPOINT {
     LOCAL itot_nmda, itot_ampa, mggate
     SOLVE state METHOD cnexp
     
     : NMDA
     mggate    = 1 / (1 + exp(-0.062 (/mV) * v) * (mg / 2.62 (mM))) : 3.57 instead of 2.62 if LJP not corrected
-    g_nmda    = (B_nmda - A_nmda) * modNMDA()
+    g_nmda    = (B_nmda - A_nmda) * modulationDA_NMDA()*modulationACh_NMDA()
     itot_nmda = g_nmda * (v - e) * mggate
     ical_nmda = ca_ratio_nmda*itot_nmda
     i_nmda    = itot_nmda - ical_nmda
     
     : AMPA
-    g_ampa    = (B_ampa - A_ampa) * modAMPA()
+    g_ampa    = (B_ampa - A_ampa) * modulationDA_AMPA() * modulationACh_AMPA()
     itot_ampa = g_ampa*(v - e) 
     ical_ampa = ca_ratio_ampa*itot_ampa
     i_ampa    = itot_ampa - ical_ampa
     
     : total values
     ical      = ical_nmda + ical_ampa
     g         = g_ampa + g_nmda
@@ -157,15 +181,15 @@
     }
 
     if ( weight <= 0 ) {
 VERBATIM
         return;
 ENDVERBATIM
     }    
-    if( urand() > failRate ) { 
+    if( urand() > failRate*(1 + modDA*(failRateDA-1)*levelDA + modACh*(failRateACh-1)*levelACh)) { 
  
       z = z*exp(-(t-tsyn)/tauR)
       z = z + (y*(exp(-(t-tsyn)/tau) - exp(-(t-tsyn)/tauR)) / (tau/tauR - 1) )
       y = y*exp(-(t-tsyn)/tau)
       x = 1-y-z
       if (tauF > 0) {
           u = u*exp(-(t-tsyn)/tauF)
@@ -196,25 +220,36 @@
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
 
-FUNCTION modAMPA() {
+FUNCTION modulationDA_NMDA() {
     : returns modulation factor
     
-    modAMPA = 1 + damod*(maxModAMPA-1)
+    modulationDA_NMDA = 1 + modDA*(maxMod_NMDADA-1)*levelDA 
 }
 
+FUNCTION modulationACh_NMDA() {
+    : returns modulation factor
+    
+    modulationACh_NMDA = 1 + modACh*(maxMod_NMDAACh-1)*levelACh 
+}
+
+FUNCTION modulationDA_AMPA() {
+    : returns modulation factor
+    
+    modulationDA_AMPA = 1 + modDA*(maxMod_AMPADA-1)*levelDA 
+}
 
-FUNCTION modNMDA() {
+FUNCTION modulationACh_AMPA() {
     : returns modulation factor
     
-    modNMDA = 1 + damod*(maxModNMDA-1)
+    modulationACh_AMPA = 1 + modACh*(maxMod_AMPAACh-1)*levelACh 
 }
 
 COMMENT
 (2019-11-29) Synaptic failure rate (fail) added. Random factor, no
 reproducibility guaranteed in parallel sim.
 
 (2019-08-21) We normalise the activation by U, to make sure that g specifies
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmglut_double.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut_double.mod`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 TITLE Glutamatergic synapse with short-term plasticity (stp)
 
 COMMENT
 stp can be turned of by setting use_stp == 0
 
 --------------------------------------------
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
 
 ENDCOMMENT
 
 NEURON {
     THREADSAFE
@@ -26,15 +37,17 @@
     RANGE tau1_ampa, tau2_ampa, tau3_ampa, tau1_nmda, tau2_nmda, tau3_nmda
     RANGE I2_ampa, I3_ampa, I2_nmda, I3_nmda
     RANGE tpeak_ampa, factor_ampa, tpeak_nmda, factor_nmda
     RANGE g_ampa, g_nmda, i_ampa, i_nmda, itot_ampa, itot_nmda, nmda_ratio
     RANGE e, g, i, q, mg
     RANGE tau, tauR, tauF, U, u0
     RANGE ca_ratio_ampa, ca_ratio_nmda, mggate, use_stp
-    RANGE failRate, damod, maxModAMPA, maxModNMDA
+    RANGE failRateDA, failRateACh, failRate
+    RANGE modDA, maxMod_AMPADA, levelDA, maxMod_AMPAACh, levelACh
+    RANGE maxMod_NMDADA, modACh, maxMod_NMDAACh			 
     NONSPECIFIC_CURRENT i
     USEION cal WRITE ical VALENCE 2
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
@@ -49,21 +62,32 @@
     tauR = 100 (ms)  : tauR > tau
     tauF = 100 (ms)  : tauF >= 0
     U = 0.3 (1) <0, 1>
     u0 = 0.1 (1) <0, 1>
     ca_ratio_ampa = 0.005
     ca_ratio_nmda = 0.1
     mg = 1 (mM)
-    damod = 0
-    maxModNMDA = 1
-    maxModAMPA = 1
+    modDA = 0
+    maxMod_AMPADA = 1
+    modACh = 0
+    maxMod_AMPAACh = 1 
+    levelACh = 0
 
-    use_stp = 1     : to turn off use_stp -> use 0
+    
+    maxMod_NMDADA = 1
+    levelDA = 0
+    
+    maxMod_NMDAACh = 1 
+
+    failRateDA = 0
+    failRateACh = 0
     failRate = 0
 
+    use_stp = 1     : to turn off use_stp -> use 0
+
     tau1_ampa      (ms)     
     tau2_ampa      (ms)  
     tau3_ampa      (ms)  
     I2_ampa 
     I3_ampa 
     tpeak_ampa     (ms)
     factor_ampa 
@@ -123,21 +147,21 @@
 
 BREAKPOINT {
     LOCAL itot_nmda, itot_ampa, mggate
     SOLVE state METHOD cnexp
     
     : NMDA
     mggate    = 1 / (1 + exp(-0.062 (/mV) * v) * (mg / 2.62 (mM))) : 3.57 instead of 2.62 if LJP not corrected
-    g_nmda    = (I3_nmda*C_nmda + I2_nmda* B_nmda - (I3_nmda+I2_nmda)* A_nmda) * modNMDA()
+    g_nmda    = (I3_nmda*C_nmda + I2_nmda* B_nmda - (I3_nmda+I2_nmda)* A_nmda) * modulationDA_NMDA()*modulationACh_NMDA()
     itot_nmda = g_nmda * (v - e) * mggate
     ical_nmda = ca_ratio_nmda*itot_nmda
     i_nmda    = itot_nmda - ical_nmda
     
     : AMPA
-    g_ampa    = (I3_ampa*C_ampa + I2_ampa* B_ampa - (I3_ampa+I2_ampa)* A_ampa) * modAMPA()
+    g_ampa    = (I3_ampa*C_ampa + I2_ampa* B_ampa - (I3_ampa+I2_ampa)* A_ampa)  * modulationDA_AMPA() * modulationACh_AMPA()
     itot_ampa = g_ampa*(v - e) 
     ical_ampa = ca_ratio_ampa*itot_ampa
     i_ampa    = itot_ampa - ical_ampa
     
     : total values
     ical      = ical_nmda + ical_ampa
     g         = g_ampa + g_nmda
@@ -170,15 +194,15 @@
     }
 
     if ( weight <= 0 ) {
 VERBATIM
         return;
 ENDVERBATIM
     }    
-    if( urand() > failRate ) { 
+    if( urand() > failRate*(1 + modDA*(failRateDA-1)*levelDA + modACh*(failRateACh-1)*levelACh)) { 
  
       z = z*exp(-(t-tsyn)/tauR)
       z = z + (y*(exp(-(t-tsyn)/tau) - exp(-(t-tsyn)/tauR)) / (tau/tauR - 1) )
       y = y*exp(-(t-tsyn)/tau)
       x = 1-y-z
       if (tauF > 0) {
           u = u*exp(-(t-tsyn)/tauF)
@@ -210,28 +234,39 @@
     }
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
+FUNCTION modulationDA_NMDA() {
+    : returns modulation factor
+    
+    modulationDA_NMDA = 1 + modDA*(maxMod_NMDADA-1)*levelDA 
+}
 
-FUNCTION modAMPA() {
+FUNCTION modulationACh_NMDA() {
     : returns modulation factor
     
-    modAMPA = 1 + damod*(maxModAMPA-1)
+    modulationACh_NMDA = 1 + modACh*(maxMod_NMDAACh-1)*levelACh 
 }
 
+FUNCTION modulationDA_AMPA() {
+    : returns modulation factor
+    
+    modulationDA_AMPA = 1 + modDA*(maxMod_AMPADA-1)*levelDA 
+}
 
-FUNCTION modNMDA() {
+FUNCTION modulationACh_AMPA() {
     : returns modulation factor
     
-    modNMDA = 1 + damod*(maxModNMDA-1)
+    modulationACh_AMPA = 1 + modACh*(maxMod_AMPAACh-1)*levelACh 
 }
 
+
 COMMENT
 (2020-09) C_ampa and C_nmda added to take into account a second decay time constant.
 tpeak_ampa, tpeak_nmda, factor_ampa and factor_nmda are now calculated during the fitting procedure.
 g_nmda and g_ampa updated.
 mggate updated to take into account LJP correction. Ilaria Carannante, ilariac@kth.se
 
 (2019-11-29) Synaptic failure rate (fail) added. Random factor, no
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/tmnmda.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms/vecevent.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/Kv3_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/bk_ch.mod`

 * *Files 20% similar despite different names*

```diff
@@ -88,7 +88,18 @@
 
 INITIAL {
         rates(v)
         m = minf
         z = zinf
         h = hinf
 }
+
+COMMENT
+From model:
+Maurice N, Mercer J, Chan CS, Hernandez-Lopez S, Held J, Tkatch T, Surmeier DJ. 
+D2 dopamine receptor-mediated modulation of voltage-dependent Na+ channels 
+reduces autonomous activity in striatal cholinergic interneurons. 
+J Neurosci. 2004 Nov 17;24(46):10289-301. doi: 10.1523/JNEUROSCI.2155-04.2004. 
+PMID: 15548642; PMCID: PMC6730305.
+
+
+ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/bk_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/bk_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/ca_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/ca_ch.mod`

 * *Files 8% similar despite different names*

```diff
@@ -147,10 +147,18 @@
 }
 	
 COMMENT
 At this time, conductances (and channel states and currents are
 calculated at the midpoint of a dt interval.  Membrane potential and
 concentrations are calculated at the edges of a dt interval.  With
 secondorder=2 everything turns out to be second order correct.
+
+From model:
+Maurice N, Mercer J, Chan CS, Hernandez-Lopez S, Held J, Tkatch T, Surmeier DJ. 
+D2 dopamine receptor-mediated modulation of voltage-dependent Na+ channels 
+reduces autonomous activity in striatal cholinergic interneurons. 
+J Neurosci. 2004 Nov 17;24(46):10289-301. doi: 10.1523/JNEUROSCI.2155-04.2004. 
+PMID: 15548642; PMCID: PMC6730305.
+
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cadyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cal12_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cal13_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/can_ms.mod`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-TITLE LVA L-type calcium current (Cav1.3)
+TITLE N-type calcium current (Cav2.2)
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cal13_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
+    SUFFIX can_ms
+    USEION ca READ cai, cao WRITE ica VALENCE 2
+    RANGE pbar, ica
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
+    pbar = 0.0 	(cm/s)
+    a = 0.21
     :q = 1	: room temperature 22-25 C
-    q = 2	: body temperature 35 C
+    q = 3	: body temperature 35 C
 } 
 
 ASSIGNED { 
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
+    ica (mA/cm2)
+    eca (mV)
     celsius (degC)
-    cali (mM)
-    calo (mM)
+    cai (mM)
+    cao (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*m*h*ghk(v, cali, calo)
+    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -52,18 +53,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-33))/(-6.7)))
-    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
-    hinf = 1/(1+exp((v-(-13.4))/11.9))
-    htau = 44.3
+    minf = 1/(1+exp((v-(-3))/(-8)))
+    mtau = 0.06+1/(exp((v-25)/18)+exp((v-(-31))/(-44)))
+    hinf = 1/(1+exp((v-(-74.8))/6.5))
+    htau = 70
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -77,51 +78,44 @@
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from
-P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
-Fig.1D]. Activation time constant is from the rodent neuron culture (both
-rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
-curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
-at room temperature.
-
-Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
-time constant was refitted to avoid singularity.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
+Model is based on mixed data. Activation curve is from neostriatal
+medium spiny neurons of adult P28+ rats [1, Fig.12F], unspecified
+recording temperature. Potentials were not corrected for the liquid
+junction potential, which was estimated to be 7 mV.  Activation time
+constant is from the rodent neuron culture (both rat and mouse cells),
+room temperature 22-25 C [2, Fig.15B].  Inactivation data is from human
+(HEK) cells [3, Tab.1, Tab.2], supposedly at room temperature.
+
+Kinetics of m2h type is used [2, Fig.5]. Activation of m^2 is fitted
+to the experimental data [1,4], activation time constant corresponds
+to m^2 already [2].  Original model [5,4] was modified by Alexander
+Kozlov <akozlov@kth.se>. Activation time constant was refitted to avoid
+singularity in the expression. Temperature correction factor 3 is used
+for body temperature [4,5].
+
+[1] Bargas J, Howe A, Eberwine J, Cao Y, Surmeier DJ (1994) Cellular
+and molecular characterization of Ca2+ currents in acutely isolated,
+adult rat neostriatal neurons. J Neurosci 14(11 Pt 1):6667-86.
 
 [2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
 omega-conotoxin-sensitive calcium channels in a mammalian
 neuroblastoma-glioma cell line. J Physiol 448:161-88.
 
-[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
-Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
-properties, pharmacology, and modulation of human, neuronal L-type
-(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
-85:816-827.
+[3] McNaughton NC, Randall AD (1997) Electrophysiological properties of
+the human N-type Ca2+ channel: I. Channel gating in Ca2+, Ba2+ and Sr2+
+containing solutions. Neuropharmacology 36(7):895-915.
+
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
 
-[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[5] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
-Neurobiol 96(1):1-31.
-
-[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
-at relatively hyperpolarized membrane potentials and are incompletely
-inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
-
-
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caldyn_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/can_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_fs.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-TITLE N-type calcium current (Cav2.2)
+TITLE R-type calcium current (Cav2.3)
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX can_fs
+    SUFFIX car_fs
     USEION ca READ cai, cao WRITE ica VALENCE 2
     RANGE pbar, ica
 }
 
 PARAMETER {
     pbar = 0.0 	(cm/s)
-    a = 0.21
-    :q = 1	: room temperature 22-25 C
+    :q = 1	: room temperature 22 C
     q = 3	: body temperature 35 C
 } 
 
 ASSIGNED { 
     v (mV)
     ica (mA/cm2)
     eca (mV)
@@ -36,15 +35,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)
+    ica = pbar*m*m*m*h*ghk(v, cai, cao)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -53,18 +52,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-3))/(-8)))
-    mtau = 0.06+1/(exp((v-25)/18)+exp((v-(-31))/(-44)))
-    hinf = 1/(1+exp((v-(-74.8))/6.5))
-    htau = 70
+    minf = 1/(1+exp((v-(-29))/(-9.6)))
+    mtau = 5.1
+    hinf = 1/(1+exp((v-(-33.3))/17))
+    htau = 22+80/(1+exp((v-(-19))/5))
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -78,44 +77,37 @@
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 COMMENT
 
-Model is based on mixed data. Activation curve is from neostriatal
-medium spiny neurons of adult P28+ rats [1, Fig.12F], unspecified
-recording temperature. Potentials were not corrected for the liquid
-junction potential, which was estimated to be 7 mV.  Activation time
-constant is from the rodent neuron culture (both rat and mouse cells),
-room temperature 22-25 C [2, Fig.15B].  Inactivation data is from human
-(HEK) cells [3, Tab.1, Tab.2], supposedly at room temperature.
-
-Kinetics of m2h type is used [2, Fig.5]. Activation of m^2 is fitted
-to the experimental data [1,4], activation time constant corresponds
-to m^2 already [2].  Original model [5,4] was modified by Alexander
-Kozlov <akozlov@kth.se>. Activation time constant was refitted to avoid
-singularity in the expression. Temperature correction factor 3 is used
-for body temperature [4,5].
-
-[1] Bargas J, Howe A, Eberwine J, Cao Y, Surmeier DJ (1994) Cellular
-and molecular characterization of Ca2+ currents in acutely isolated,
-adult rat neostriatal neurons. J Neurosci 14(11 Pt 1):6667-86.
-
-[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
-omega-conotoxin-sensitive calcium channels in a mammalian
-neuroblastoma-glioma cell line. J Physiol 448:161-88.
-
-[3] McNaughton NC, Randall AD (1997) Electrophysiological properties of
-the human N-type Ca2+ channel: I. Channel gating in Ca2+, Ba2+ and Sr2+
-containing solutions. Neuropharmacology 36(7):895-915.
+Original data by Foehring  et al (2000) [1] for dissociated MSNs from
+P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
+liquid junction potential was around 8 mV and was not corrected. Kinetics
+of m3h type was fitted.  Inactivation time constants were measured in
+neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
+at room temperature 22 C.
+
+Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
+<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
+activation time constant matched m^3 originally [1]. Smooth fit of
+inactivation time constant from [2,3].
+
+[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
+(2000) Unique properties of R-type calcium currents in neocortical and
+neostriatal neurons. J Neurophysiol 84(5):2225-36.
+
+[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
+biophysical characterization of voltage-gated calcium currents in the
+endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
 
-[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
-spike timing-dependent calcium influx during corticostriatal upstates. J
-Neurophysiol 110(7):1631-45.
-
-[5] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
+
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/can_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/car_ms.mod`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-TITLE N-type calcium current (Cav2.2)
+TITLE R-type calcium current (Cav2.3)
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX can_ms
+    SUFFIX car_ms
     USEION ca READ cai, cao WRITE ica VALENCE 2
     RANGE pbar, ica
 }
 
 PARAMETER {
     pbar = 0.0 	(cm/s)
-    a = 0.21
-    :q = 1	: room temperature 22-25 C
+    :q = 1	: room temperature 22 C
     q = 3	: body temperature 35 C
 } 
 
 ASSIGNED { 
     v (mV)
     ica (mA/cm2)
     eca (mV)
@@ -36,15 +35,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ica = pbar*m*m*(h*a+1-a)*ghk(v, cai, cao)
+    ica = pbar*m*m*m*h*ghk(v, cai, cao)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -53,18 +52,18 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-3))/(-8)))
-    mtau = 0.06+1/(exp((v-25)/18)+exp((v-(-31))/(-44)))
-    hinf = 1/(1+exp((v-(-74.8))/6.5))
-    htau = 70
+    minf = 1/(1+exp((v-(-29))/(-9.6)))
+    mtau = 5.1
+    hinf = 1/(1+exp((v-(-33.3))/17))
+    htau = 22+80/(1+exp((v-(-19))/5))
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
     eco = co*efun(z)
@@ -78,44 +77,37 @@
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 COMMENT
 
-Model is based on mixed data. Activation curve is from neostriatal
-medium spiny neurons of adult P28+ rats [1, Fig.12F], unspecified
-recording temperature. Potentials were not corrected for the liquid
-junction potential, which was estimated to be 7 mV.  Activation time
-constant is from the rodent neuron culture (both rat and mouse cells),
-room temperature 22-25 C [2, Fig.15B].  Inactivation data is from human
-(HEK) cells [3, Tab.1, Tab.2], supposedly at room temperature.
-
-Kinetics of m2h type is used [2, Fig.5]. Activation of m^2 is fitted
-to the experimental data [1,4], activation time constant corresponds
-to m^2 already [2].  Original model [5,4] was modified by Alexander
-Kozlov <akozlov@kth.se>. Activation time constant was refitted to avoid
-singularity in the expression. Temperature correction factor 3 is used
-for body temperature [4,5].
-
-[1] Bargas J, Howe A, Eberwine J, Cao Y, Surmeier DJ (1994) Cellular
-and molecular characterization of Ca2+ currents in acutely isolated,
-adult rat neostriatal neurons. J Neurosci 14(11 Pt 1):6667-86.
-
-[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
-omega-conotoxin-sensitive calcium channels in a mammalian
-neuroblastoma-glioma cell line. J Physiol 448:161-88.
-
-[3] McNaughton NC, Randall AD (1997) Electrophysiological properties of
-the human N-type Ca2+ channel: I. Channel gating in Ca2+, Ba2+ and Sr2+
-containing solutions. Neuropharmacology 36(7):895-915.
+Original data by Foehring  et al (2000) [1] for dissociated MSNs from
+P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
+liquid junction potential was around 8 mV and was not corrected. Kinetics
+of m3h type was fitted.  Inactivation time constants were measured in
+neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
+at room temperature 22 C.
+
+Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
+<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
+activation time constant matched m^3 originally [1]. Smooth fit of
+inactivation time constant from [2,3].
+
+[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
+(2000) Unique properties of R-type calcium currents in neocortical and
+neostriatal neurons. J Neurophysiol 84(5):2225-36.
+
+[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
+biophysical characterization of voltage-gated calcium currents in the
+endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
 
-[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
-spike timing-dependent calcium influx during corticostriatal upstates. J
-Neurophysiol 110(7):1631-45.
-
-[5] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
+
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cap_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cap_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caq_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/caq_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/caq_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/car_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-TITLE R-type calcium current (Cav2.3)
+TITLE T-type calcium current (Cav3.3)
 
 UNITS {
     (mV) = (millivolt)
     (mA) = (milliamp)
     (S) = (siemens)
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX car_fs
-    USEION ca READ cai, cao WRITE ica VALENCE 2
-    RANGE pbar, ica
+    SUFFIX cat33_ms
+    USEION cal READ cali, calo WRITE ical VALENCE 2
+    RANGE pbar, ical
 }
 
 PARAMETER {
-    pbar = 0.0 	(cm/s)
-    :q = 1	: room temperature 22 C
+    pbar = 0.0 (cm/s)
+    :q = 1	: room temperature 21 C
     q = 3	: body temperature 35 C
 } 
 
 ASSIGNED { 
     v (mV)
-    ica (mA/cm2)
-    eca (mV)
+    ical (mA/cm2)
+    ecal (mV)
     celsius (degC)
-    cai (mM)
-    cao (mM)
+    cali (mM)
+    calo (mM)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ica = pbar*m*m*m*h*ghk(v, cai, cao)
+    ical = pbar*m*m*m*h*ghk(v, cali, calo)
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -52,58 +52,48 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-29))/(-9.6)))
-    mtau = 5.1
-    hinf = 1/(1+exp((v-(-33.3))/17))
-    htau = 22+80/(1+exp((v-(-19))/5))
+    minf = 1/(1+exp((v-(-81))/(-5.8)))
+    mtau = (2.3+20/(1+exp((v-(-60))/9)))*3
+    hinf = 1/(1+exp((v-(-78.3))/6.5))
+    htau = 125+140/(1+exp((v-(-60))/3))
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
     LOCAL z, eci, eco
     z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    eco = co*efun(z)
-    eci = ci*efun(-z)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
-}
-
-FUNCTION efun(z) {
-    if (fabs(z) < 1e-4) {
-        efun = 1-z/2
-    }else{
-        efun = z/(exp(z)-1)
+    if(z == 0) {
+        z = z+1e-6
     }
+    eco = co*(z)/(exp(z)-1)
+    eci = ci*(-z)/(exp(-z)-1)
+    ghk = (1e-3)*2*FARADAY*(eci-eco)
 }
 
 COMMENT
 
-Original data by Foehring  et al (2000) [1] for dissociated MSNs from
-P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
-liquid junction potential was around 8 mV and was not corrected. Kinetics
-of m3h type was fitted.  Inactivation time constants were measured in
-neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
-at room temperature 22 C.
-
-Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
-<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
-activation time constant matched m^3 originally [1]. Smooth fit of
-inactivation time constant from [2,3].
-
-[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
-(2000) Unique properties of R-type calcium currents in neocortical and
-neostriatal neurons. J Neurophysiol 84(5):2225-36.
-
-[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
-biophysical characterization of voltage-gated calcium currents in the
-endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
+Rat Cav3.2 channels were isolated and transfection of human embryonic
+kidney cells was performed [1].  Electrophysiological recordings were
+done in 21 C.
+
+NEURON model by Alexander Kozlov <akozlov@kth.se>. Kinetics of m3h
+type was used [2-4]. Activation time constant was scaled up accordingly.
+
+[1] Iftinca M, McKay BE, Snutch TP, McRory JE, Turner RW, Zamponi
+GW (2006) Temperature dependence of T-type calcium channel
+gating. Neuroscience 142(4):1031-42.
+
+[2] Crunelli V, Toth TI, Cope DW, Blethyn K, Hughes SW (2005) The
+'window' T-type calcium current in brain dynamics of different behavioural
+states. J Physiol 562(Pt 1):121-9.
 
 [3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
 [4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/car_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ch.mod`

 * *Files 23% similar despite different names*

```diff
@@ -1,113 +1,83 @@
-TITLE R-type calcium current (Cav2.3)
+TITLE SK-type calcium activated K channel (KCa2.2)
 
 UNITS {
+    (molar) = (1/liter)
     (mV) = (millivolt)
     (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
     (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX car_ms
-    USEION ca READ cai, cao WRITE ica VALENCE 2
-    RANGE pbar, ica
+    SUFFIX sk_ch
+    USEION ca READ cai
+    USEION k READ ek WRITE ik
+    RANGE gbar, ik
 }
 
 PARAMETER {
-    pbar = 0.0 	(cm/s)
-    :q = 1	: room temperature 22 C
-    q = 3	: body temperature 35 C
-} 
+    gbar = 0.0 (mho/cm2)
+    :q = 1	: room temperature 22-25 C
+    q = 2	: body temperature 35 C
+}
 
-ASSIGNED { 
+ASSIGNED {
     v (mV)
-    ica (mA/cm2)
-    eca (mV)
-    celsius (degC)
-    cai (mM)
-    cao (mM)
-    minf
-    mtau (ms)
-    hinf
-    htau (ms)
+    ik (mA/cm2)
+    cai (mM) 
+    ek (mV)
+    oinf
+    otau (ms)
 }
 
-STATE { m h }
+STATE { o }
 
 BREAKPOINT {
-    SOLVE states METHOD cnexp
-    ica = pbar*m*m*m*h*ghk(v, cai, cao)
+    SOLVE state METHOD cnexp
+    ik = gbar*o*(v-ek)
+}
+
+DERIVATIVE state {
+    rate(v, cai)
+    o' = (oinf-o)/otau*q
 }
 
 INITIAL {
-    rates()
-    m = minf
-    h = hinf
-}
-
-DERIVATIVE states { 
-    rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
-}
-
-PROCEDURE rates() {
-    UNITSOFF
-    minf = 1/(1+exp((v-(-29))/(-9.6)))
-    mtau = 5.1
-    hinf = 1/(1+exp((v-(-33.3))/17))
-    htau = 22+80/(1+exp((v-(-19))/5))
-    UNITSON
-}
-
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    eco = co*efun(z)
-    eci = ci*efun(-z)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
-}
-
-FUNCTION efun(z) {
-    if (fabs(z) < 1e-4) {
-        efun = 1-z/2
-    }else{
-        efun = z/(exp(z)-1)
-    }
+    rate(v, cai)
+    o = oinf
+}
+
+PROCEDURE rate(v (mV), ca (mM)) {
+    LOCAL a
+    a = (ca/0.57e-3)^5.2
+    oinf = a/(1+a)
+    otau = 4.9
 }
 
 COMMENT
 
-Original data by Foehring  et al (2000) [1] for dissociated MSNs from
-P28-P42 Sprague-Dawley rat brain. Unspecified recording temperature. The
-liquid junction potential was around 8 mV and was not corrected. Kinetics
-of m3h type was fitted.  Inactivation time constants were measured in
-neurons from endopiriform nucleus of P7-P21 Hartley guinea pigs [2]
-at room temperature 22 C.
-
-Original NEURON model by Wolf (2005) [3] modified by Alexander Kozlov
-<akozlov@kth.se>. Activation curve fitted to m^3 kinetics as in [4],
-activation time constant matched m^3 originally [1]. Smooth fit of
-inactivation time constant from [2,3].
-
-[1] Foehring RC, Mermelstein PG, Song WJ, Ulrich S, Surmeier DJ
-(2000) Unique properties of R-type calcium currents in neocortical and
-neostriatal neurons. J Neurophysiol 84(5):2225-36.
-
-[2] Brevi S, de Curtis M, Magistretti J (2001) Pharmacological and
-biophysical characterization of voltage-gated calcium currents in the
-endopiriform nucleus of the guinea pig. J Neurophysiol 85(5):2076-87.
-
-[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
+Experimental data was obtained for the apamin-sensitive clone rSK2 from
+rat brain cDNA expressed in Xenopus oocytes [1,2].  All experiments were
+performed at room tempretaure.
+
+Original model [3] used calcium dependence from [2, Fig.2] and calcium
+activation time constant from [1,  Fig.13A]. NEURON implementation by
+Alexander Kozlov <akozlov@kth.se> follows the revised model [4].
+
+[1] Hirschberg B, Maylie J, Adelman JP, Marrion NV (1998) Gating of
+recombinant small-conductance Ca-activated K+ channels by calcium. J
+Gen Physiol 111(4):565-81.
+
+[2] Maylie J, Bond CT, Herson PS, Lee WS, Adelman JP (2004) Small
+conductance Ca2+-activated K+ channels and calmodulin. J Physiol 554(Pt
+2):255-61.
+
+[3] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
+calcium influx and spike timing-dependent plasticity in striatal medium
+spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 [4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
 spike timing-dependent calcium influx during corticostriatal upstates. J
 Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cat32_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir_ms.mod`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,98 @@
-TITLE T-type calcium current (Cav3.2)
+TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
+
+NEURON {
+    SUFFIX kir_ms
+    USEION k READ ek WRITE ik
+    RANGE gbar, gk, ik, shift
+}
 
 UNITS {
+    (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
-    (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
-}
-
-NEURON {
-    SUFFIX cat32_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
-    :q = 1	: room temperature 21 C
-    q = 3	: body temperature 35 C
-} 
+    gbar = 0.0 	(S/cm2) 
+    shift = 0.0 (mV)
+    q = 1 	: body temperature 35 C
+}
 
-ASSIGNED { 
+ASSIGNED {
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
-    celsius (degC)
-    cali (mM)
-    calo (mM)
+    ek (mV)
+    ik (mA/cm2)
+    gk (S/cm2)
     minf
     mtau (ms)
-    hinf
-    htau (ms)
 }
 
-STATE { m h }
+STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*m*m*h*ghk(v, cali, calo)
+    gk = gbar*m
+    ik = gk*(v-ek)
 }
 
-INITIAL {
+DERIVATIVE states {
     rates()
-    m = minf
-    h = hinf
+    m' = (minf-m)/mtau*q
 }
 
-DERIVATIVE states { 
+INITIAL {
     rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+    m = minf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-54))/(-7.8)))
-    mtau = (2.1+23/(1+exp((v-(-61))/6)))*3
-    hinf = 1/(1+exp((v-(-64.2))/8.8))
-    htau = 30+280/(1+exp((v-(-52))/7))
+    minf = 1/(1+exp((v-(-82)-shift)/13))
+    mtau = 1/(exp((v-(-103))/(-14.5))+0.125/(1+exp((v-(-35))/(-19))))
     UNITSON
 }
 
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    if(z == 0) {
-        z = z+1e-6
-    }
-    eco = co*(z)/(exp(z)-1)
-    eci = ci*(-z)/(exp(-z)-1)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
-}
-
 COMMENT
 
-Rat Cav3.2 channels were isolated and transfection of human embryonic
-kidney cells was performed [1].  Electrophysiological recordings were
-done in 21 C.
-
-NEURON model by Alexander Kozlov <akozlov@kth.se>. Kinetics of m3h
-type was used [2-4]. Activation time constant was scaled up accordingly.
-
-[1] Iftinca M, McKay BE, Snutch TP, McRory JE, Turner RW, Zamponi
-GW (2006) Temperature dependence of T-type calcium channel
-gating. Neuroscience 142(4):1031-42.
-
-[2] Crunelli V, Toth TI, Cope DW, Blethyn K, Hughes SW (2005) The
-'window' T-type calcium current in brain dynamics of different behavioural
-states. J Physiol 562(Pt 1):121-9.
+Original model by Wolf et al (2005) [1] for the rat MSN cells from the
+nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
+channel expressed in HEK cells [2] and shifted to match extracellular
+concentration of K in rat. Measured half-activation values are -109.3
+mV (striatonigral MSN) and -113.2 mV (striatopallidal MSN) [6, Supp
+Tab.1]. Time constants were derived from Aplysia data [3] and adjusted
+to match the rat experiments [1]. Time constant was further tuned [4]
+to fit the rat data below -80 mV [5].  Kinetics is corrected to the body
+temperature 35 C [4].
+
+Non-inactivating Kir current was observed in cells expressing Kir2.2
+and/or Kir2.3 [5]. Activation variable with m^1 kinetics is used [1,4].
+Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
 
-[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
-spike timing-dependent calcium influx during corticostriatal upstates. J
-Neurophysiol 110(7):1631-45.
+[2] Kubo Y, Murata Y (2001) Control of rectification and permeation by
+two distinct sites after the second transmembrane region in Kir2.1 K+
+channel. J Physiol 531, 645-660.
+
+[3] Hayashi H, Fishman HM (1988) Inward rectifier K+ channel kinetics
+from analysis of the complex conductance of aplysia neuronal membrane.
+Biophys J 53, 747-757.
+
+[4] Steephen JE, Manchanda R (2009) Differences in biophysical properties
+of nucleus accumbens medium spiny neurons emerging from inactivation of
+inward rectifying potassium currents. J Comput Neurosci 27(3):453-70
+
+[5] Mermelstein PG, Song WJ, Tkatch T, Yan Z, Surmeier DJ (1998)
+Inwardly rectifying potassium (IRK) currents are correlated with IRK
+subunit expression in rat nucleus accumbens medium spiny neurons. J
+Neurosci 18(17):6650-61.
+
+[6] Shen W, Tian X, Day M, Ulrich S, Tkatch T, Nathanson NM, Surmeier DJ
+(2007) Cholinergic modulation of Kir2 channels selectively elevates
+dendritic excitability in striatopallidal neurons. Nat Neurosci
+10(11):1458-66.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/cat33_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_fs.mod`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,83 @@
-TITLE T-type calcium current (Cav3.3)
+TITLE SK-type calcium activated K channel (KCa2.2)
 
 UNITS {
+    (molar) = (1/liter)
     (mV) = (millivolt)
     (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
     (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cat33_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
+    SUFFIX sk_fs
+    USEION ca READ cai
+    USEION k READ ek WRITE ik
+    RANGE gbar, ik
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
-    :q = 1	: room temperature 21 C
-    q = 3	: body temperature 35 C
-} 
+    gbar = 0.0 	(mho/cm2)
+    :q = 1	: room temperature
+    q = 3	: body temperature
+}
 
-ASSIGNED { 
+ASSIGNED {
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
-    celsius (degC)
-    cali (mM)
-    calo (mM)
-    minf
-    mtau (ms)
-    hinf
-    htau (ms)
+    ik (mA/cm2)
+    cai (mM) 
+    ek (mV)
+    oinf
+    otau (ms)
 }
 
-STATE { m h }
+STATE { o }
 
 BREAKPOINT {
-    SOLVE states METHOD cnexp
-    ical = pbar*m*m*m*h*ghk(v, cali, calo)
+    SOLVE state METHOD cnexp
+    ik = gbar*o*(v-ek)
+}
+
+DERIVATIVE state {
+    rate(v, cai)
+    o' = (oinf-o)/otau*q
 }
 
 INITIAL {
-    rates()
-    m = minf
-    h = hinf
-}
-
-DERIVATIVE states { 
-    rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
-}
-
-PROCEDURE rates() {
-    UNITSOFF
-    minf = 1/(1+exp((v-(-81))/(-5.8)))
-    mtau = (2.3+20/(1+exp((v-(-60))/9)))*3
-    hinf = 1/(1+exp((v-(-78.3))/6.5))
-    htau = 125+140/(1+exp((v-(-60))/3))
-    UNITSON
-}
-
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    if(z == 0) {
-        z = z+1e-6
-    }
-    eco = co*(z)/(exp(z)-1)
-    eci = ci*(-z)/(exp(-z)-1)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
+    rate(v, cai)
+    o = oinf
+}
+
+PROCEDURE rate(v (mV), ca (mM)) {
+    LOCAL a
+    a = (ca/0.57e-3)^5.2
+    oinf = a/(1+a)
+    otau = 4.9
 }
 
 COMMENT
 
-Rat Cav3.2 channels were isolated and transfection of human embryonic
-kidney cells was performed [1].  Electrophysiological recordings were
-done in 21 C.
-
-NEURON model by Alexander Kozlov <akozlov@kth.se>. Kinetics of m3h
-type was used [2-4]. Activation time constant was scaled up accordingly.
-
-[1] Iftinca M, McKay BE, Snutch TP, McRory JE, Turner RW, Zamponi
-GW (2006) Temperature dependence of T-type calcium channel
-gating. Neuroscience 142(4):1031-42.
-
-[2] Crunelli V, Toth TI, Cope DW, Blethyn K, Hughes SW (2005) The
-'window' T-type calcium current in brain dynamics of different behavioural
-states. J Physiol 562(Pt 1):121-9.
-
-[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
+Experimental data was obtained for the apamin-sensitive clone rSK2 from
+rat brain cDNA expressed in Xenopus oocytes [1,2].  All experiments were
+performed at room tempretaure.
+
+Original model [3] used calcium dependence from [2, Fig.2] and calcium
+activation time constant from [1,  Fig.13]. NEURON implementation by
+Alexander Kozlov <akozlov@kth.se> follows the revised model [4].
+
+[1] Hirschberg B, Maylie J, Adelman JP, Marrion NV (1998) Gating of
+recombinant small-conductance Ca-activated K+ channels by calcium. J
+Gen Physiol 111(4):565-81.
+
+[2] Maylie J, Bond CT, Herson PS, Lee WS, Adelman JP (2004) Small
+conductance Ca2+-activated K+ channels and calmodulin. J Physiol 554(Pt
+2):255-61.
+
+[3] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
+calcium influx and spike timing-dependent plasticity in striatal medium
+spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 [4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
 spike timing-dependent calcium influx during corticostriatal upstates. J
 Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/h_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/h_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/hcn12_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/hcn12_ch.mod`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 COMMENT
 
-Josh Held's adaptation to suit HCN1+2.  12/22/2003
-
-****
-Kinetic model of HCN2 channel gating from Wang et al 2002.
-
-In this model channel opening is coupled to a change in the affinity of the cyclic nucleotide binding domain for cAMP which is manifest as a shift in the activation curve toward more positive potentials.  This model explains the slow activation kinetics of Ih associated with low concentrations of cAMP.
-
-For further details email Matt Nolan at mfnolan@fido.cpmc.columbia.edu.
-
-Reference
-
-Wang J., Chen S., Nolan M.F. and Siegelbaum S.A. (2002). Activity-dependent regulation of HCN pacemaker channels by cyclicAMP: signalling through dynamic allosteric coupling. Neuron 36, 1-20.
-****
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
 ENDCOMMENT
 
 NEURON {
 	SUFFIX hcn12_ch
 	NONSPECIFIC_CURRENT i
 	RANGE i, ehcn, g, gbar
 	GLOBAL a0, b0, ah, bh, ac, bc, aa0, ba0
 	GLOBAL aa0, ba0, aah, bah, aac, bac
 	GLOBAL kon, koff, b, bf, ai, gca, shift
+	RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
 	(mV) = (millivolt)
 	(molar) = (1/liter)
 	(mM) = (millimolar)
 	(mA) = (milliamp)
@@ -53,14 +65,19 @@
 	bf      = 8.94
 	ai	= 1e-05		(mM)	:concentration cyclic AMP
 	gca     = 1			: relative conductance of the bound state
 	shift   = -17		(mV)	: shift in voltage dependence
 	q10v    = 4                     : q10 value from Magee 1998
 	q10a    = 1.5			: estimated q10 for the cAMP binding reaction
 	celsius			(degC)
+	modDA = 0
+        maxModDA = 1
+        levelDA = 0
+
+	
 }
 
 ASSIGNED {
 	v	(mV)
 	g	(S/cm2)
 	i	(mA/cm2)
 	alpha	(/ms)
@@ -78,15 +95,15 @@
 
 INITIAL {
 	SOLVE kin STEADYSTATE sparse
 }
 
 BREAKPOINT {
 	SOLVE kin METHOD sparse
-	g = gbar*(o + cao*gca)
+	g = gbar*(o + cao*gca)*modulationDA()
 	i = g*(v-ehcn)
 }
 
 KINETIC kin {
 	LOCAL qa
 	qa = q10a^((celsius-22 (degC))/10 (degC))
 	rates(v)
@@ -108,7 +125,31 @@
 	} else {
 		alpha = a0*qv / (1 + exp(-((-200)-ah-shift)*ac))
 		beta = b0*qv / (1 + exp(-((-200)-bh-shift)*bc))
 		alphaa = aa0*qv / (1 + exp(-((-200)-aah-shift)*aac))
 		betaa = ba0*qv / (1 + exp(-((-200)-bah-shift)*bac))
 	}
 }
+
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+COMMENT
+
+Josh Held's adaptation to suit HCN1+2.  12/22/2003
+
+****
+Kinetic model of HCN2 channel gating from Wang et al 2002.
+
+In this model channel opening is coupled to a change in the affinity of the cyclic nucleotide binding domain for cAMP which is manifest as a shift in the activation curve toward more positive potentials.  This model explains the slow activation kinetics of Ih associated with low concentrations of cAMP.
+
+For further details email Matt Nolan at mfnolan@fido.cpmc.columbia.edu.
+
+Reference
+
+Wang J., Chen S., Nolan M.F. and Siegelbaum S.A. (2002). Activity-dependent regulation of HCN pacemaker channels by cyclicAMP: signalling through dynamic allosteric coupling. Neuron 36, 1-20.
+****
+
+ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/im_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/im_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kaf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kaf_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kas_fs.mod`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-TITLE Fast A-type potassium current (Kv4.2)
+TITLE Slowly inactivating A-type potassium current (Kv1.2)
 
 NEURON {
-    SUFFIX kaf_ms
+    SUFFIX kas_fs
     USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, q
+    RANGE gbar, gk, ik, shift, q
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 (S/cm2) 
-    q = 1	: room temperature (unspecified)
-    :q = 2	: body temperature 35 C (Du 2017)
-    :q = 3	: body temperature 35 C
+    gbar = 0.0 	(S/cm2) 
+    a = 0.8
+    :q = 1	: room temperature 22-24 C
+    q = 3	: body temperature 33 C
+    shift = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -30,15 +31,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*h
+    gk = gbar*m*m*(h*a+1-a)
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -48,65 +49,42 @@
     rates()
     m = minf
     h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-10))/(-17.7)))
-    mtau = 0.9+1.1/(1+exp((v-(-30))/10))
-    hinf = 1/(1+exp((v-(-75.6))/11.8))
-    htau = 14
+    minf = 1/(1+exp((v-(-27)-shift)/(-16)))
+    mtau = 3.4+89.2*exp(-((v-(-34.3))/30.1)^2)
+    hinf = 1/(1+exp((v-(-33.5)-shift)/21.5))
+    htau = 548.7*6/(exp((v-(-96))/(-29.01))+exp((v-(-96))/100))
     UNITSON
-
-    :Du 2017
-    :LOCAL alpha, beta, sum
-    :UNITSOFF
-    :alpha = 1.5/(1+exp((v-4)/(-17)))
-    :beta = 0.6/(1+exp((v-10)/9))
-    :sum = alpha+beta
-    :minf = alpha/sum
-    :mtau = 1/sum
-    :
-    :alpha = 0.105/(1+exp((v-(-121))/22))
-    :beta = 0.065/(1+exp((v-(-55))/(-11)))
-    :sum = alpha+beta
-    :hinf = alpha/sum
-    :htau = 1/sum
-    :UNITSON
 }
 
 COMMENT
 
-Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
-dissociated from young adult rats, age P28-P42.  Electrophysiological
-recordings were done at unspecified temperature (room temperature 20-22 C
-assumed). Potentials were not corrected for the liquid junction potential
-(estimated 1-2 mV).
-
-Activation m^1 matches experimental data [1, Fig.2C]. Activation time
-constants fit tabulated data [1, Fig.2B].  Slope of inactivation function
-fitted to the data [1, Fig.3B] with half inactivation potential -75.6
-mV. Temperature factor q between 1.5 [3] and 3 [2] was used for body
-temperature.  Conductance kinetics of m2h type is used [2], no corrections
-for m^2 applied. Later modification by Du [4] is close to this model.
-
-[1] Tkatch T, Baranauskas G, Surmeier DJ (2000) Kv4.2 mRNA abundance and
-A-type K(+) current amplitude are linearly related in basal ganglia and
-basal forebrain neurons. J Neurosci 20(2):579-88.
+Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
+acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
+brain. All recordings were conducted at 22-24 C. No correction for the
+liquid junction potential was reported.
+
+Conductance kinetics of m2h type is used [1] with partial inactivation,
+m2 (a h + (1-a)). Fraction a is set to 0.8, as in [1, Fig.6B]; other
+values for a are possible [2] (see also kas.mod in companion code).
+Equation for htau [1] is corrected to match the authors' data [1, Fig.6B]
+by Alexander Kozlov <akozlov@kth.se>.  Time constants were corrected to
+body temperature with factor q=3 [1,3].
+
+[1] Shen W, Hernandez-Lopez S, Tkatch T, Held JE, Surmeier DJ (2004)
+Kv1.2-containing K+ channels regulate subthreshold excitability of
+striatal medium spiny neurons. J Neurophysiol 91(3):1337-49.
 
 [2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[3]  Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[4] Du K, Wu YW, Lindroos R, Liu Y, Rózsa B, Katona G, Ding JB,
-Kotaleski JH (2017) Cell-type-specific inhibition of the dendritic
-plateau potential in striatal spiny projection neurons. Proc Natl Acad
-Sci USA 114:E7612-E7621.
+[3] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+spike timing-dependent calcium influx during corticostriatal upstates. J
+Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kas_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/sk_ms.mod`

 * *Files 25% similar despite different names*

```diff
@@ -1,90 +1,83 @@
-TITLE Slowly inactivating A-type potassium current (Kv1.2)
-
-NEURON {
-    SUFFIX kas_fs
-    USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, shift, q
-}
+TITLE SK-type calcium activated K channel (KCa2.2)
 
 UNITS {
-    (S) = (siemens)
+    (molar) = (1/liter)
     (mV) = (millivolt)
     (mA) = (milliamp)
+    (mM) = (millimolar)
+}
+
+NEURON {
+    SUFFIX sk_ms
+    USEION ca READ cai
+    USEION k READ ek WRITE ik
+    RANGE gbar, ik
 }
 
 PARAMETER {
-    gbar = 0.0 	(S/cm2) 
-    a = 0.8
-    :q = 1	: room temperature 22-24 C
-    q = 3	: body temperature 33 C
-    shift = 0
+    gbar = 0.0 	(mho/cm2)
+    :q = 1	: room temperature
+    q = 1	: body temperature
 }
 
 ASSIGNED {
     v (mV)
-    ek (mV)
     ik (mA/cm2)
-    gk (S/cm2)
-    minf
-    mtau (ms)
-    hinf
-    htau (ms)
+    cai (mM) 
+    ek (mV)
+    oinf
+    otau (ms)
 }
 
-STATE { m h }
+STATE { o }
 
 BREAKPOINT {
-    SOLVE states METHOD cnexp
-    gk = gbar*m*m*(h*a+1-a)
-    ik = gk*(v-ek)
+    SOLVE state METHOD cnexp
+    ik = gbar*o*(v-ek)
 }
 
-DERIVATIVE states {
-    rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+DERIVATIVE state {
+    rate(v, cai)
+    o' = (oinf-o)/otau*q
 }
 
 INITIAL {
-    rates()
-    m = minf
-    h = hinf
+    rate(v, cai)
+    o = oinf
 }
 
-PROCEDURE rates() {
-    UNITSOFF
-    minf = 1/(1+exp((v-(-27)-shift)/(-16)))
-    mtau = 3.4+89.2*exp(-((v-(-34.3))/30.1)^2)
-    hinf = 1/(1+exp((v-(-33.5)-shift)/21.5))
-    htau = 548.7*6/(exp((v-(-96))/(-29.01))+exp((v-(-96))/100))
-    UNITSON
+PROCEDURE rate(v (mV), ca (mM)) {
+    LOCAL a
+    a = (ca/0.57e-3)^5.2
+    oinf = a/(1+a)
+    otau = 4.9
 }
 
 COMMENT
 
-Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
-acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
-brain. All recordings were conducted at 22-24 C. No correction for the
-liquid junction potential was reported.
-
-Conductance kinetics of m2h type is used [1] with partial inactivation,
-m2 (a h + (1-a)). Fraction a is set to 0.8, as in [1, Fig.6B]; other
-values for a are possible [2] (see also kas.mod in companion code).
-Equation for htau [1] is corrected to match the authors' data [1, Fig.6B]
-by Alexander Kozlov <akozlov@kth.se>.  Time constants were corrected to
-body temperature with factor q=3 [1,3].
-
-[1] Shen W, Hernandez-Lopez S, Tkatch T, Held JE, Surmeier DJ (2004)
-Kv1.2-containing K+ channels regulate subthreshold excitability of
-striatal medium spiny neurons. J Neurophysiol 91(3):1337-49.
-
-[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
+Experimental data was obtained for the apamin-sensitive clone rSK2 from
+rat brain cDNA expressed in Xenopus oocytes [1,2].  All experiments were
+performed at room tempretaure.
+
+Original model [3] used calcium dependence from [2, Fig.2] and calcium
+activation time constant from [1,  Fig.13]. NEURON implementation by
+Alexander Kozlov <akozlov@kth.se> follows the revised model [4].
+
+[1] Hirschberg B, Maylie J, Adelman JP, Marrion NV (1998) Gating of
+recombinant small-conductance Ca-activated K+ channels by calcium. J
+Gen Physiol 111(4):565-81.
+
+[2] Maylie J, Bond CT, Herson PS, Lee WS, Adelman JP (2004) Small
+conductance Ca2+-activated K+ channels and calmodulin. J Physiol 554(Pt
+2):255-61.
+
+[3] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
+calcium influx and spike timing-dependent plasticity in striatal medium
+spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
-[3] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
+[4] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
 spike timing-dependent calcium influx during corticostriatal upstates. J
 Neurophysiol 110(7):1631-45.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kas_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kas_ms.mod`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,61 @@
 TITLE Slowly inactivating A-type potassium current (Kv1.2)
 
+COMMENT
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
+ENDCOMMENT
+
+
 NEURON {
     SUFFIX kas_ms
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik
+    RANGE modDA, maxModDA, levelDA
+
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
     a = 0.8
     :q = 1	: room temperature 22-24 C
     q = 3	: body temperature 33 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -30,15 +65,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*(h*a+1-a)
+    gk = gbar*m*m*(h*a+1-a)*modulationDA()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -69,14 +104,21 @@
     :beta = 0.002/(1+exp((v-50)/(-70)))
     :sum = alpha+beta
     :hinf = a+(alpha/sum)*(1-a)
     :htau = 1/sum
     UNITSON
 }
 
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+
 COMMENT
 
 Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
 acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
 brain. All recordings were conducted at 22-24 C. No correction for the
 liquid junction potential was reported.
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kcnq_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdr_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kdrbca1_lts.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kir2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kir_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kir_fs.mod`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,57 @@
 TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
 
+COMMENT
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
+ENDCOMMENT
+
 NEURON {
     SUFFIX kir_fs
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik, shift
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 	(S/cm2) 
     shift = 0
     q = 1 	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
@@ -27,15 +59,15 @@
     mtau (ms)
 }
 
 STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m
+    gk = gbar*m*modulationDA()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
 }
@@ -48,14 +80,21 @@
 PROCEDURE rates() {
     UNITSOFF
     minf = 1/(1+exp((v-(-82)-shift)/13))
     mtau = 1/(exp((v-(-103)-shift)/(-14.5))+0.125/(1+exp((v-(-35)-shift)/(-19))))
     UNITSON
 }
 
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+
 COMMENT
 
 Original model by Wolf et al (2005) [1] for the rat MSN cells from the
 nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
 channel expressed in HEK cells [2] and shifted to match extracellular
 concentration of K in rat.  Time constants were derived from Aplysia data
 [3] and adjusted to match the rat experiments [1]. Time constant was
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/kv4_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na2_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na2_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na3n_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/na3_lts.mod`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,46 @@
 TITLE na3
 : Na current 
 : modified from Jeff Magee. M.Migliore may97
 : added sh to account for higher threshold M.Migliore, Apr.2002
 
+COMMENT
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+
+ENDCOMMENT
+
 NEURON {
-	SUFFIX na3
+	SUFFIX na3_lts
 	USEION na READ ena WRITE ina
-	RANGE  gbar, ar, sh
+	RANGE  gbar, ar, sh, ina
 	GLOBAL minf, hinf, mtau, htau, sinf, taus,qinf, thinf
+	RANGE modDA, maxModDA, levelDA
 }
 
 PARAMETER {
 	sh   = 0	(mV)
 	gbar = 0.010   	(mho/cm2)	
 								
 	tha  =  -30	(mV)		: v 1/2 for act	
@@ -41,14 +70,17 @@
         smax=10		(ms)
         vvh=-58		(mV) 
         vvs=2		(mV)
         ar=1		(1)		: 1=no inact., 0=max inact.
 	ena		(mV)            : must be explicitly def. in hoc
 	celsius
 	v 		(mV)
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
 }
 
 
 UNITS {
 	(mA) = (milliamp)
 	(mV) = (millivolt)
 	(pS) = (picosiemens)
@@ -63,16 +95,16 @@
 	sinf (ms)	taus (ms)
 }
  
 
 STATE { m h s}
 
 BREAKPOINT {
-        SOLVE states METHOD cnexp
-        thegna = gbar*m*m*m*h*s
+    SOLVE states METHOD cnexp
+    thegna = gbar*m*m*m*h*s*modulationDA()
 	ina = thegna * (v - ena)
 } 
 
 INITIAL {
 	trates(v,ar,sh)
 	m=minf  
 	h=hinf
@@ -125,8 +157,12 @@
 	if (fabs(v-th) > 1e-6) {
 	        trap0 = a * (v - th) / (1 - exp(-(v - th)/q))
 	} else {
 	        trap0 = a * q
  	}
 }	
 
-        
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/na_ch.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/na_ch.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/naf_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_fs.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/naf_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/naf_ms.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmampa.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmampa.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmglut.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmglut.mod`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,51 @@
 TITLE Glutamatergic synapse with short-term plasticity (stp)
 
 COMMENT
 stp can be turned of by setting use_stp == 0
+
+--------------------------------------------
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+
 ENDCOMMENT
 
 NEURON {
     THREADSAFE
     POINT_PROCESS tmGlut
     RANGE tau1_ampa, tau2_ampa, tau1_nmda, tau2_nmda
     RANGE g_ampa, g_nmda, i_ampa, i_nmda, nmda_ratio
     RANGE e, g, i, q, mg
     RANGE tau, tauR, tauF, U, u0
     RANGE ca_ratio_ampa, ca_ratio_nmda, mggate, use_stp
-    RANGE failRate
+    RANGE failRateDA, failRateACh, failRate
+    RANGE modDA, maxMod_AMPADA, levelDA, maxMod_AMPAACh, levelACh
+    RANGE maxMod_NMDADA, modACh, maxMod_NMDAACh 
     NONSPECIFIC_CURRENT i
     USEION cal WRITE ical VALENCE 2
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
@@ -36,17 +65,31 @@
     tauR = 100 (ms)  : tauR > tau
     tauF = 800 (ms)  : tauF >= 0
     U = 0.3 (1) <0, 1>
     u0 = 0 (1) <0, 1>
     ca_ratio_ampa = 0.005
     ca_ratio_nmda = 0.1
     mg = 1 (mM)
+    
+    modDA = 0
+    maxMod_AMPADA = 1
+    modACh = 0
+    maxMod_AMPAACh = 1 
+    levelACh = 0
+
+    
+    maxMod_NMDADA = 1
+    levelDA = 0
+    
+    maxMod_NMDAACh = 1 
 
+    failRateDA = 0
+    failRateACh = 0
+    failRate = 0
     use_stp = 1     : to turn of use_stp -> use 0
-    failRate = 0	
 }
 
 ASSIGNED {
     v (mV)
     i (nA)
     i_ampa (nA)
     i_nmda (nA)
@@ -87,22 +130,22 @@
 
 BREAKPOINT {
     LOCAL itot_nmda, itot_ampa, mggate
     SOLVE state METHOD cnexp
     
     : NMDA
     mggate    = 1 / (1 + exp(-0.062 (/mV) * v) * (mg / 3.57 (mM)))
-    g_nmda    = B_nmda - A_nmda
+    g_nmda    = (B_nmda - A_nmda) * modulationDA_NMDA()*modulationACh_NMDA()
     itot_nmda = g_nmda * (v - e) * mggate
     ical_nmda = ca_ratio_nmda*itot_nmda
     i_nmda    = itot_nmda - ical_nmda
     
     : AMPA
-    g_ampa    = B_ampa - A_ampa
-    itot_ampa = g_ampa*(v - e)
+    g_ampa    = (B_ampa - A_ampa) * modulationDA_AMPA() * modulationACh_AMPA()
+    itot_ampa = g_ampa*(v - e) 
     ical_ampa = ca_ratio_ampa*itot_ampa
     i_ampa    = itot_ampa - ical_ampa
     
     : total values
     ical      = ical_nmda + ical_ampa
     g         = g_ampa + g_nmda
     i         = i_ampa + i_nmda
@@ -130,15 +173,15 @@
     }
 
     if ( weight <= 0 ) {
 VERBATIM
         return;
 ENDVERBATIM
     }    
-    if( urand() > failRate ) { 
+    if( urand() > failRate*(1 + modDA*(failRateDA-1)*levelDA + modACh*(failRateACh-1)*levelACh)) { 
  
       z = z*exp(-(t-tsyn)/tauR)
       z = z + (y*(exp(-(t-tsyn)/tau) - exp(-(t-tsyn)/tauR)) / (tau/tauR - 1) )
       y = y*exp(-(t-tsyn)/tau)
       x = 1-y-z
       if (tauF > 0) {
           u = u*exp(-(t-tsyn)/tauF)
@@ -168,14 +211,39 @@
     }
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
+
+FUNCTION modulationDA_NMDA() {
+    : returns modulation factor
+    
+    modulationDA_NMDA = 1 + modDA*(maxMod_NMDADA-1)*levelDA 
+}
+
+FUNCTION modulationACh_NMDA() {
+    : returns modulation factor
+    
+    modulationACh_NMDA = 1 + modACh*(maxMod_NMDAACh-1)*levelACh 
+}
+
+FUNCTION modulationDA_AMPA() {
+    : returns modulation factor
+    
+    modulationDA_AMPA = 1 + modDA*(maxMod_AMPADA-1)*levelDA 
+}
+
+FUNCTION modulationACh_AMPA() {
+    : returns modulation factor
+    
+    modulationACh_AMPA = 1 + modACh*(maxMod_AMPAACh-1)*levelACh 
+}
+
 COMMENT
 (2019-11-29) Synaptic failure rate (fail) added. Random factor, no
 reproducibility guaranteed in parallel sim.
 
 (2019-08-21) We normalise the activation by U, to make sure that g specifies
              the conductance of the first actvation
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/tmnmda.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/tmnmda.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanisms.OLD/vecevent.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms.OLD/vecevent.mod`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/#na_ch.mod#` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kv4_ch.mod`

 * *Files 27% similar despite different names*

```diff
@@ -1,162 +1,143 @@
 COMMENT
-NA_CH.MOD
 
-c1 - c2 - c3 - c4 - c5 - o  - is1
-|    |    |    |    |    |
-i1 - i2 - i3 - i4 - i5 - i6 - is2
+c1 - c2 - c3 - c4 - o
+|    |    |    |    |
+i1 - i2 - i3 - i4 - i5 - is
 
-SLOW
 
-6/18/2003
-
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
-
 NEURON {
-	SUFFIX na_ch
-	USEION na READ ena WRITE ina
-	RANGE g, ina, gbar, a
-	GLOBAL Con, Coff, Oon, Ooff
-	GLOBAL a0, vha, vca
-	GLOBAL b0, vhb, vcb
-	GLOBAL g0
-	GLOBAL d0
-	GLOBAL aS1, aS2, bRANGE damod, maxMod
+	SUFFIX kv4_ch
+	USEION k READ ek WRITE ik
+	RANGE g, ik, gbar
+	GLOBAL alpha, beta
+	GLOBAL ci, ic, oi, io, a, b, am, bm, vc, gamma, delta, vha, vhb
+	GLOBAL i5is, isi5
+	GLOBAL q10i, q10v
+        RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
 	(mV) = (millivolt)
 	(mA) = (milliamp)
 	(S) = (siemens)
 }
 
 PARAMETER {
 	gbar = 1	(S/cm2)
-
-	a0 = 37		(1/ms)	: alpha
-	vha  = 45	(mV)
-	vca = 40	(mV)
-
-	b0 = 10		(1/ms)	: beta
-	vhb = -50	(mV)
-	vcb = -20	(mV)
-
-	g0 = 40		(1/ms)	: gamma
-
-	d0 = 30		(1/ms)	: delta
-
-	aS1 = 0.0025	(1/ms)
-	aS2 = 0.0002	(1/ms)
-	bS = 0.00017	(1/ms)
-
-	Con = 0.001	(1/ms)
-	Coff = 0.1	(1/ms)
-	Oon = .7	(1/ms)
-	Ooff = 0.01	(1/ms)
-    damod = 0
-    maxMod = 1
+	gamma = 200	(1/ms)
+	delta = 4	(1/ms)
+	a = 3
+	b = 40
+	ic = 500	(/ms)
+	oi = 1e-9	(/ms)
+	io = .01	(/ms)
+	ci = .2		(/ms)
+	am = 1		(1/ms)
+	bm = 7		(1/ms)
+	vc = 10		(mV)
+	vha = -75	(mV)
+	vhb = -30	(mV)
+	i5is = .001	(/ms)
+	isi5 = .001	(/ms)
+	q10i = 3
+	q10v = 3
+	celsius		(degC)
+        modDA = 0
+        maxModDA = 1
+        levelDA = 0
 }
 
 ASSIGNED {
 	v	(mV)
-	ena	(mV)
+	ek	(mV)
 	g	(S/cm2)
-	ina	(mA/cm2)
-	alpha	(1/ms)
-	beta	(1/ms)
-	gamma	(1/ms)
-	delta	(1/ms)
-	a
+	ik	(mA/cm2)
+	alpha	(/ms)
+	beta	(/ms)
 }
 
 STATE {
-	c1  : closed
+	c1
 	c2
 	c3
 	c4
-	c5
-	ct  : total closed
-	o   : open
-	i1  : fast inactivated
+	o
+	i1
 	i2
 	i3
 	i4
 	i5
-	i6
-	ift : total fast inactivated
-	is1 : slow inactivated
-	is2
-	ist : total slow inactivated
-	it  : total inactivated
+	is
 }
 
 BREAKPOINT {
 	SOLVE kin METHOD sparse
-	g = gbar*o*modulation()
-	ina = g*(v-ena)
-	ct = c1 + c2 + c3 + c4 + c5
-	ift = i1 + i2 + i3 + i4 + i5 + i6
-	ist = is1 + is2
-	it = ift + ist
+	g = gbar*o*modulationDA()
+	ik = g*(v-ek)
 }
 
 INITIAL {
 	SOLVE kin STEADYSTATE sparse
 }
 
-KINETIC kin{
+KINETIC kin{LOCAL q10
+	q10 = q10i^((celsius - 22 (degC))/10 (degC))
 	rates(v)
+	~ c1 <-> c2 (3*alpha,beta)
+	~ c2 <-> c3 (2*alpha,2*beta)
+	~ c3 <-> c4 (alpha,3*beta)
+	~ c4 <-> o  (q10*gamma,q10*delta)
 
-	~ c1 <-> c2 (4*alpha, beta)
-	~ c2 <-> c3 (3*alpha, 2*beta)
-	~ c3 <-> c4 (2*alpha, 3*beta)
-	~ c4 <-> c5 (alpha, 4*beta)
-	~ c5 <-> o  (gamma, delta)
-	~ o <-> is1 (aS1, bS)
+	~ i1 <-> i2 (3*alpha*a,beta/b)
+	~ i2 <-> i3 (2*alpha*a,2*beta/b)
+	~ i3 <-> i4 (alpha*a,3*beta/b)
+	~ i4 <-> i5 (q10*gamma,q10*delta)
+	~ i5 <-> is (q10*i5is,q10*isi5)
 
-	~ i1 <-> i2 (4*alpha*a, beta/a)
-	~ i2 <-> i3 (3*alpha*a, 2*beta/a)
-	~ i3 <-> i4 (2*alpha*a, 3*beta/a)
-	~ i4 <-> i5 (alpha*a, 4*beta/a)
-	~ i5 <-> i6 (gamma, delta)
-	~ i6 <-> is2 (aS2, bS)
-
-	~ c1 <-> i1 (Con, Coff)
-	~ c2 <-> i2 (Con*a, Coff/a)
-	~ c3 <-> i3 (Con*a^2, Coff/a^2)
-	~ c4 <-> i4 (Con*a^3, Coff/a^3)
-	~ c5 <-> i5 (Con*a^4, Coff/a^4)
-	~ o <-> i6  (Oon, Ooff)
-
-	CONSERVE c1+c2+c3+c4+c5+i1+i2+i3+i4+i5+i6+is1+is2+o=1
+	~ i1 <-> c1 (q10*ic,q10*ci)
+	~ i2 <-> c2 (q10*ic/b,q10*ci*a)
+	~ i3 <-> c3 (q10*ic/b^2,q10*ci*a^2)
+	~ i4 <-> c4 (q10*ic/b^3,q10*ci*a^3)
+	~ i5 <-> o  (q10*io,q10*oi)
 
+	CONSERVE c1+c2+c3+c4+i1+i2+i3+i4+i5+o+is=1
 }
 
-PROCEDURE rates(v(millivolt)) {
-	alpha = a0*exp((v-vha)/vca)
-	beta = b0*exp((v-vhb)/vcb)
-	gamma = g0
-	delta = d0
-
-	a = ((Coff/Con)/(Ooff/Oon))^(1/8)
+PROCEDURE rates(v(millivolt)) {LOCAL q10
+	q10 = q10v^((celsius - 22 (degC))/10 (degC))
+	alpha = q10*am*exp((v-vha)/vc)
+	beta = q10*bm*exp((v-vhb)/-vc)
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal12_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cal13_ms.mod`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,32 @@
-TITLE HVA L-type calcium current (Cav1.2)
+TITLE LVA L-type calcium current (Cav1.3)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
 UNITS {
@@ -25,28 +36,31 @@
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cal12_ms
+    SUFFIX cal13_ms
     USEION cal READ cali, calo WRITE ical VALENCE 2
     RANGE pbar, ical
-    RANGE maxMod
-    POINTER damod
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
 }
 
 PARAMETER {
     pbar = 0.0 (cm/s)
-    a = 0.17
-    :q = 1	          : room temperature 22-25 C
-    q = 2	          : body temperature 35 C
-    damod = 0
-    maxMod = 1
+    :q = 1	: room temperature 22-25 C
+    q = 2	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1
+    levelACh = 0
 } 
 
 ASSIGNED { 
     v (mV)
     ical (mA/cm2)
     ecal (mV)
     celsius (degC)
@@ -58,15 +72,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*(h*a+1-a)*ghk(v, cali, calo)*modulation()
+    ical = pbar*m*m*h*ghk(v, cali, calo)*modulationDA()*modulationACh()
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -75,15 +89,15 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-8.9))/(-6.7)))
+    minf = 1/(1+exp((v-(-33))/(-6.7)))
     mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
     hinf = 1/(1+exp((v-(-13.4))/11.9))
     htau = 44.3
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
@@ -99,31 +113,38 @@
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+FUNCTION modulationACh() {
+    : returns modulation factor
+    
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from P5-P32
-Charles River rat pups [1].   Activation time constant is from the
-rodent neuron culture (both rat and mouse cells), room temperature 22-25
-C [2, Fig.15A]. Inactivation curve of CaL v1.3 current was taken from HEK
-cells [3, Fig.2 and p.819] at room temperature.
+Activation curve was reconstructed for cultured NAc neurons from
+P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
+Fig.1D]. Activation time constant is from the rodent neuron culture (both
+rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
+curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
+at room temperature.
 
 Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m1h type was used [5,6]. Activation
+<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
 time constant was refitted to avoid singularity.
 
 [1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
 characterization of voltage-dependent Ca2+ channels in neurons isolated
 from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
 
 [2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
@@ -145,8 +166,13 @@
 Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
 calcium influx and spike timing-dependent plasticity in striatal medium
 spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 [6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
 Neurobiol 96(1):1-31.
 
+[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
+at relatively hyperpolarized membrane potentials and are incompletely
+inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
+
+
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal12_ms_mod.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kaf_ms.mod`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,168 @@
-TITLE HVA L-type calcium current (Cav1.2)
+TITLE Fast A-type potassium current (Kv4.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
+NEURON {
+    SUFFIX kaf_ms
+    USEION k READ ek WRITE ik
+    RANGE gbar, gk, ik, q
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
+    RANGE modShift
+}
+
 UNITS {
+    (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
-    (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
-}
-
-NEURON {
-    SUFFIX cal12_ms_mod
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
-    RANGE maxMod
-    POINTER damod
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
-    a = 0.17
-    :q = 1	          : room temperature 22-25 C
-    q = 2	          : body temperature 35 C
-    damod = 0
-    maxMod = 1
-} 
+    gbar = 0.0 (S/cm2) 
+    q = 1	: room temperature (unspecified)
+    :q = 2	: body temperature 35 C (Du 2017)
+    :q = 3	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modShift = 0
+    modACh = 0
+    maxModACh = 1
+    levelACh = 0
+
 
-ASSIGNED { 
+
+}
+
+ASSIGNED {
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
-    celsius (degC)
-    cali (mM)
-    calo (mM)
+    ek (mV)
+    ik (mA/cm2)
+    gk (S/cm2)
     minf
     mtau (ms)
     hinf
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*(h*a+1-a)*ghk(v, cali, calo)*modulation()
+    gk = gbar*m*m*h*modulationDA()
+    modShift = modulationACh()				     
+    ik = gk*(v-ek)
 }
 
-INITIAL {
+DERIVATIVE states {
     rates()
-    m = minf
-    h = hinf
+    m' = (minf-m)/mtau*q
+    h' = (hinf-h)/htau*q
 }
 
-DERIVATIVE states { 
+INITIAL {
     rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+    m = minf
+    h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-8.9))/(-6.7)))
-    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
-    hinf = 1/(1+exp((v-(-13.4))/11.9))
-    htau = 44.3
+    minf = 1/(1+exp((v-(-10+modShift))/(-17.7)))
+    mtau = 0.9+1.1/(1+exp((v-(-30))/10))
+    hinf = 1/(1+exp((v-(-75.6))/11.8))
+    htau = 14
     UNITSON
-}
-
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    eco = co*efun(z)
-    eci = ci*efun(-z)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
-}
 
-FUNCTION efun(z) {
-    if (fabs(z) < 1e-4) {
-        efun = 1-z/2
-    }else{
-        efun = z/(exp(z)-1)
-    }
+    :Du 2017
+    :LOCAL alpha, beta, sum
+    :UNITSOFF
+    :alpha = 1.5/(1+exp((v-4)/(-17)))
+    :beta = 0.6/(1+exp((v-10)/9))
+    :sum = alpha+beta
+    :minf = alpha/sum
+    :mtau = 1/sum
+    :
+    :alpha = 0.105/(1+exp((v-(-121))/22))
+    :beta = 0.065/(1+exp((v-(-55))/(-11)))
+    :sum = alpha+beta
+    :hinf = alpha/sum
+    :htau = 1/sum
+    :UNITSON
 }
 
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
+FUNCTION modulationACh() {
+    : returns modulation factor
+    
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
+}
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from P5-P32
-Charles River rat pups [1].   Activation time constant is from the
-rodent neuron culture (both rat and mouse cells), room temperature 22-25
-C [2, Fig.15A]. Inactivation curve of CaL v1.3 current was taken from HEK
-cells [3, Fig.2 and p.819] at room temperature.
-
-Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m1h type was used [5,6]. Activation
-time constant was refitted to avoid singularity.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
-
-[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
-omega-conotoxin-sensitive calcium channels in a mammalian
-neuroblastoma-glioma cell line. J Physiol 448:161-88.
-
-[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
-Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
-properties, pharmacology, and modulation of human, neuronal L-type
-(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
-85:816-827.
+Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
+dissociated from young adult rats, age P28-P42.  Electrophysiological
+recordings were done at unspecified temperature (room temperature 20-22 C
+assumed). Potentials were not corrected for the liquid junction potential
+(estimated 1-2 mV).
+
+Activation m^1 matches experimental data [1, Fig.2C]. Activation time
+constants fit tabulated data [1, Fig.2B].  Slope of inactivation function
+fitted to the data [1, Fig.3B] with half inactivation potential -75.6
+mV. Temperature factor q between 1.5 [3] and 3 [2] was used for body
+temperature.  Conductance kinetics of m2h type is used [2], no corrections
+for m^2 applied. Later modification by Du [4] is close to this model.
+
+[1] Tkatch T, Baranauskas G, Surmeier DJ (2000) Kv4.2 mRNA abundance and
+A-type K(+) current amplitude are linearly related in basal ganglia and
+basal forebrain neurons. J Neurosci 20(2):579-88.
 
-[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+[3]  Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
 Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
 calcium influx and spike timing-dependent plasticity in striatal medium
 spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
-[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
-Neurobiol 96(1):1-31.
+[4] Du K, Wu YW, Lindroos R, Liu Y, Rózsa B, Katona G, Ding JB,
+Kotaleski JH (2017) Cell-type-specific inhibition of the dendritic
+plateau potential in striatal spiny projection neurons. Proc Natl Acad
+Sci USA 114:E7612-E7621.
 
 ENDCOMMENT
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal13_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kir23_lts.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,130 @@
-TITLE LVA L-type calcium current (Cav1.3)
+TITLE Noninactivating inwardly rectifying potassium current (Kir2.3)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
+      
+NEURON {
 
+    SUFFIX kir23_lts
+    USEION k READ ek WRITE ik
+    RANGE gbar, gk, ik
+    RANGE modACh, maxModACh, levelACh
+}
 
 UNITS {
+    (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
-    (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
-}
-
-NEURON {
-    SUFFIX cal13_ms
-    USEION cal READ cali, calo WRITE ical VALENCE 2
-    RANGE pbar, ical
-    RANGE maxMod
-    POINTER damod
 }
 
 PARAMETER {
-    pbar = 0.0 (cm/s)
-    :q = 1	: room temperature 22-25 C
-    q = 2	: body temperature 35 C
-    damod = 0
-    maxMod = 1
-} 
+    gbar = 0.0 (S/cm2) 
+    q = 1	: body temperature 35 C
+    modACh = 0
+    maxModACh = 1 
+    levelACh = 0
+}
 
-ASSIGNED { 
+ASSIGNED {
     v (mV)
-    ical (mA/cm2)
-    ecal (mV)
-    celsius (degC)
-    cali (mM)
-    calo (mM)
+    ek (mV)
+    ik (mA/cm2)
+    gk (S/cm2)
     minf
     mtau (ms)
-    hinf
-    htau (ms)
 }
 
-STATE { m h }
+STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*m*h*ghk(v, cali, calo)*modulation()
+    gk = gbar*m*modulationACh()
+    ik = gk*(v-ek)
 }
 
-INITIAL {
+DERIVATIVE states {
     rates()
-    m = minf
-    h = hinf
+    m' = (minf-m)/mtau*q
 }
 
-DERIVATIVE states { 
+INITIAL {
     rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+    m = minf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-33))/(-6.7)))
-    mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
-    hinf = 1/(1+exp((v-(-13.4))/11.9))
-    htau = 44.3
+    minf = 1/(1+exp((v-(-82))/13))
+    :mtau = 1/(2*exp((v-(-106))/(-12.6))+0.086*exp((v-(-19))/47))  : Steephen (2009)
+    mtau = 1/(exp((v-(-97.3))/(-12.6))+exp((v-96.3)/47))  : Steephen (2009)
     UNITSON
 }
 
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    eco = co*efun(z)
-    eci = ci*efun(-z)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
-}
-
-FUNCTION efun(z) {
-    if (fabs(z) < 1e-4) {
-        efun = 1-z/2
-    }else{
-        efun = z/(exp(z)-1)
-    }
-}
-
-
-FUNCTION modulation() {
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
-
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from
-P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
-Fig.1D]. Activation time constant is from the rodent neuron culture (both
-rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
-curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
-at room temperature.
-
-Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
-time constant was refitted to avoid singularity.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
-
-[2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
-omega-conotoxin-sensitive calcium channels in a mammalian
-neuroblastoma-glioma cell line. J Physiol 448:161-88.
-
-[3] Bell DC, Butcher AJ, Berrow NS, Page KM, Brust PF, Nesterova A,
-Stauderman KA, Seabrook GR, Nurnberg B, Dolphin AC (2001) Biophysical
-properties, pharmacology, and modulation of human, neuronal L-type
-(alpha(1D), Ca(V)1.3) voltage-dependent calcium currents. J Neurophysiol
-85:816-827.
+Original model by Wolf et al (2005) [1] for the rat MSN cells from the
+nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
+channel expressed in HEK cells [2] and shifted to match extracellular
+concentration of K in rat.  Time constants were derived from Aplysia
+data [3] and adjusted to match the rat experiments [1]. Time constant
+was further tuned [4] to fit the rat data below -80 mV [5].
 
-[4] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+Non-inactivating component of the Kir channel with m1 kinetics is used
+[1,4].  Kinetics is corrected to the body temperature 35 C.
+
+Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
+
+[1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[5] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
-Neurobiol 96(1):1-31.
-
-[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
-at relatively hyperpolarized membrane potentials and are incompletely
-inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
-
+[2] Kubo Y, Murata Y (2001) Control of rectification and permeation by
+two distinct sites after the second transmembrane region in Kir2.1 K+
+channel. J Physiol 531, 645-660.
+
+[3] Hayashi H, Fishman HM (1988) Inward rectifier K+ channel kinetics
+from analysis of the complex conductance of aplysia neuronal membrane.
+Biophys J 53, 747-757.
+
+[4] Steephen JE, Manchanda R (2009) Differences in biophysical properties
+of nucleus accumbens medium spiny neurons emerging from inactivation of
+inward rectifying potassium currents. J Comput Neurosci 27(3):453-70
+
+[5] Mermelstein PG, Song WJ, Tkatch T, Yan Z, Surmeier DJ (1998)
+Inwardly rectifying potassium (IRK) currents are correlated with IRK
+subunit expression in rat nucleus accumbens medium spiny neurons. J
+Neurosci 18(17):6650-61.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/cal13_ms_mod.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cal12_ms.mod`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,32 @@
-TITLE LVA L-type calcium current (Cav1.3)
+TITLE HVA L-type calcium current (Cav1.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
 UNITS {
@@ -25,27 +36,33 @@
     (molar) = (1/liter)
     (mM) = (millimolar)
     FARADAY = (faraday) (coulomb)
     R = (k-mole) (joule/degC)
 }
 
 NEURON {
-    SUFFIX cal13_ms_mod
+    SUFFIX cal12_ms
     USEION cal READ cali, calo WRITE ical VALENCE 2
     RANGE pbar, ical
-    RANGE maxMod
-    POINTER damod
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
 }
 
 PARAMETER {
     pbar = 0.0 (cm/s)
-    :q = 1	: room temperature 22-25 C
-    q = 2	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    a = 0.17
+    :q = 1	          : room temperature 22-25 C
+    q = 2	          : body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1 
+    levelACh = 0
+		   
 } 
 
 ASSIGNED { 
     v (mV)
     ical (mA/cm2)
     ecal (mV)
     celsius (degC)
@@ -57,15 +74,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    ical = pbar*m*m*h*ghk(v, cali, calo)*modulation()
+    ical = pbar*m*(h*a+1-a)*ghk(v, cali, calo)*modulationDA()*modulationACh()
 }
 
 INITIAL {
     rates()
     m = minf
     h = hinf
 }
@@ -74,15 +91,15 @@
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-33))/(-6.7)))
+    minf = 1/(1+exp((v-(-8.9))/(-6.7)))
     mtau = 0.06+1/(exp((v-10)/20)+exp((v-(-17))/-48))
     hinf = 1/(1+exp((v-(-13.4))/11.9))
     htau = 44.3
     UNITSON
 }
 
 FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
@@ -98,32 +115,37 @@
         efun = 1-z/2
     }else{
         efun = z/(exp(z)-1)
     }
 }
 
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
+
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1) 
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
 
 COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from
-P5-P32 Charles River rat pups [1] and shifted to match LVA data [7,
-Fig.1D]. Activation time constant is from the rodent neuron culture (both
-rat and mouse cells), room temperature 22-25 C [2, Fig.15A]. Inactivation
-curve of CaL v1.3 current was taken from HEK cells [3, Fig.2 and p.819]
-at room temperature.
+Activation curve was reconstructed for cultured NAc neurons from P5-P32
+Charles River rat pups [1].   Activation time constant is from the
+rodent neuron culture (both rat and mouse cells), room temperature 22-25
+C [2, Fig.15A]. Inactivation curve of CaL v1.3 current was taken from HEK
+cells [3, Fig.2 and p.819] at room temperature.
 
 Original NEURON model by Wolf (2005) [4] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Kinetics of m2h type was used [5,6]. Activation
+<akozlov@csc.kth.se>. Kinetics of m1h type was used [5,6]. Activation
 time constant was refitted to avoid singularity.
 
 [1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
 characterization of voltage-dependent Ca2+ channels in neurons isolated
 from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
 
 [2] Kasai H, Neher E (1992) Dihydropyridine-sensitive and
@@ -145,13 +167,10 @@
 Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
 calcium influx and spike timing-dependent plasticity in striatal medium
 spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 [6] Tuckwell HC (2012) Quantitative aspects of L-type Ca2+ currents. Prog
 Neurobiol 96(1):1-31.
 
-[7] Xu W, Lipscombe D (2001) Neuronal cav1.3 L-type channels activate
-at relatively hyperpolarized membrane potentials and are incompletely
-inhibited by dihydropyridines. J Neurosci 21(16): 5944-5951.
-
+add justification for modulation
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/caq_ms.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/it_lts.mod`

 * *Files 27% similar despite different names*

```diff
@@ -1,105 +1,149 @@
-TITLE Q-type calcium current (Cav2.1)
+TITLE Low threshold calcium current
+:
+:   Ca++ current responsible for low threshold spikes (LTS)
+:   THALAMOCORTICAL CELLS
+:   Differential equations
+:
+:   Model based on the data of Huguenard & McCormick, J Neurophysiol
+:   68: 1373-1383, 1992 and Huguenard & Prince, J Neurosci.
+:   12: 3804-3817, 1992.
+:
+:   Features:
+:
+:	- kinetics described by Nernst equations using a m2h format
+:	- activation considered at steady-state
+:	- inactivation fit to Huguenard's data using a bi-exp function
+:	- shift for screening charge, q10 of inactivation of 3
+:
+:
+:   Written by Alain Destexhe, Salk Institute, 1993; modified 1995
+:
+
+INDEPENDENT {t FROM 0 TO 1 WITH 1 (ms)}
+
+COMMENT
+
+Neuromodulation is added as functions:
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
+
+where:
+    
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
+[] == default values
+{} == ranges
+    
+ENDCOMMENT
+
 
-UNITS {
-    (mV) = (millivolt)
-    (mA) = (milliamp)
-    (S) = (siemens)
-    (molar) = (1/liter)
-    (mM) = (millimolar)
-    FARADAY = (faraday) (coulomb)
-    R = (k-mole) (joule/degC)
-}
 
 NEURON {
-    SUFFIX caq_ms
-    USEION ca READ cai, cao WRITE ica VALENCE 2
-    RANGE pbar, ica
+	SUFFIX it_lts
+	USEION ca READ cai,cao WRITE ica
+	GLOBAL q10
+	RANGE gcabar, m_inf, tau_m, h_inf, tau_h, shift
+        RANGE modDA, maxModDA, levelDA
 }
 
-PARAMETER {
-    pbar = 0.0 (cm/s)
-    :q = 1	: room temperature 22 C
-    q = 3	: body temperature 35 C
-} 
-
-ASSIGNED { 
-    v (mV)
-    ica (mA/cm2)
-    eca (mV)
-    celsius (degC)
-    cai (mM)
-    cao (mM)
-    minf
-    mtau (ms)
+UNITS {
+	(molar) = (1/liter)
+	(mV) =	(millivolt)
+	(mA) =	(milliamp)
+	(mM) =	(millimolar)
+
+	FARADAY = (faraday) (coulomb)
+	R = (k-mole) (joule/degC)
 }
 
-STATE { m }
+PARAMETER {
+	v		(mV)
+	celsius	= 36	(degC)
+	gcabar	= 0.002	(mho/cm2)
+	q10	= 3			: Q10 of inactivation
+	shift	= 2 	(mV)		: corresponds to 2mM ext Ca++
+	cai	= 2.4e-4 (mM)		: adjusted for eca=120 mV
+	cao	= 2	(mM)
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+}
+
+STATE {
+	h
+}
+
+ASSIGNED {
+	ica	(mA/cm2)
+	carev	(mV)
+	m_inf
+	tau_m	(ms)			: dummy variable for compatibility
+	h_inf
+	tau_h	(ms)
+	phi_h
+}
 
 BREAKPOINT {
-    SOLVE states METHOD cnexp
-    ica = pbar*m*m*ghk(v, cai, cao)
+	SOLVE castate METHOD cnexp
+	carev = (1e3) * (R*(celsius+273.15))/(2*FARADAY) * log (cao/cai)
+	ica = gcabar * m_inf * m_inf * h * (v-carev)
 }
 
-INITIAL {
-    rates()
-    m = minf
-}
+DERIVATIVE castate {
+	evaluate_fct(v)
 
-DERIVATIVE states { 
-    rates()
-    m' = (minf-m)/mtau*q
+	h' = (h_inf - h) / tau_h
 }
 
-PROCEDURE rates() {
-    UNITSOFF
-    minf = 1/(1+exp((v-(-16.3))/(-7.9)))
-    mtau = 1.13*2
-    UNITSON
-}
 
-FUNCTION ghk(v (mV), ci (mM), co (mM)) (.001 coul/cm3) {
-    LOCAL z, eci, eco
-    z = (1e-3)*2*FARADAY*v/(R*(celsius+273.15))
-    eco = co*efun(z)
-    eci = ci*efun(-z)
-    ghk = (1e-3)*2*FARADAY*(eci-eco)
+UNITSOFF
+INITIAL {
+	h = 0
+
+:
+:   Transformation to 36 deg assuming Q10 of 3 for h
+:   (as in Coulter et al., J Physiol 414: 587, 1989)
+:
+	phi_h = q10 ^ ((celsius-24 (degC) )/10 (degC) )
 }
 
-FUNCTION efun(z) {
-    if (fabs(z) < 1e-4) {
-        efun = 1-z/2
-    }else{
-        efun = z/(exp(z)-1)
-    }
+PROCEDURE evaluate_fct(v(mV)) { LOCAL Vm
+
+	Vm = v + shift
+
+	m_inf = 1.0 / ( 1 + exp(-(Vm+57)/6.2) )
+	h_inf = 1.0 / ( 1 + exp((Vm+81)/4.0) )
+
+:	if(Vm < -80) {
+:		tau_h = exp((Vm+467)/66.6) / phi_h
+:	} else {
+:		tau_h = ( 28 + exp(-(Vm+22)/10.5) ) / phi_h
+:	}
+
+	tau_h = 30.8 + (211.4 + exp((Vm+113.2)/5)) / (1 + exp((Vm+84)/3.2))
+
+	tau_h = tau_h / phi_h
+
 }
 
-COMMENT
 
-Activation curve was reconstructed for cultured NAc neurons from P5-P32
-Charles River rat pups [1].  Activation time constant was measured in
-culture neurons from cerebellum of P2-P5 rat pups [2] at room temperature
-22 C.
-
-Original NEURON model by Wolf (2005) [3] was modified by Alexander Kozlov
-<akozlov@csc.kth.se>. Activation curve was fitted to m2 kinetics [4],
-activation time constant was scaled up as well.
-
-[1] Churchill D, Macvicar BA (1998) Biophysical and pharmacological
-characterization of voltage-dependent Ca2+ channels in neurons isolated
-from rat nucleus accumbens. J Neurophysiol 79(2):635-47.
-
-[2] Randall A, Tsien RW (1995) Pharmacological dissection of multiple
-types of Ca2+ channel currents in rat cerebellar granule neurons. J
-Neurosci 15(4):2995-3012.
-
-[3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
-
-[4] Brown AM, Schwindt PC, Crill WE (1993) Voltage dependence and
-activation kinetics of pharmacologically defined components of the
-high-threshold calcium current in rat neocortical neurons. J Neurophysiol
-70(4):1530-43.
+UNITSON
 
-ENDCOMMENT
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
+}
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kaf_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kdr_lts.mod`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,119 @@
-TITLE Fast A-type potassium current (Kv4.2)
+TITLE Fast delayed rectifier potassium current (Kv3.1/3.2)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
+
 NEURON {
-    SUFFIX kaf_fs
+    SUFFIX kdr_lts
     USEION k READ ek WRITE ik
     RANGE gbar, gk, ik, q
-    RANGE maxMod
-    POINTER damod
+    RANGE modDA, maxModDA, levelDA
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 	(S/cm2) 
-    :q = 1	: room temperature (unspecified)
+    gbar = 0.0 (S/cm2) 
+    :q = 1	: room temperature
     q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
     minf
     mtau (ms)
-    hinf
-    htau (ms)
 }
 
-STATE { m h }
+STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*h*modulation()
+    gk = gbar*m
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
 }
 
 INITIAL {
     rates()
     m = minf
-    h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-10))/(-17.7)))
-    mtau = (0.9+1.1/(1+exp((v-(-30))/10)))*2
-    hinf = 1/(1+exp((v-(-75.6))/11.8))
-    htau = 14
+    minf = 1/(1+exp((v-(-13))/(-6)))
+    mtau = 11.1
     UNITSON
 }
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
 COMMENT
 
-Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
-dissociated from young adult rats, age P28-P42.  Electrophysiological
-recordings were done at unspecified temperature (room temperature 20-22 C
-assumed). Potentials were not corrected for the liquid junction potential
-(estimated 1-2 mV).
-
-Conductance kinetics of m2h type is used [2].  Activation m^1 matches
-experimental data [1, Fig.2C]. Activation time constants were fitted to
-tabulated data [1, Fig.2B] by Alexander Kozlov <akozlov@kth.se> and scaled
-up x2 for m2 kinetics.  Slope of inactivation function fitted to the data
-[1, Fig.3B] with half inactivation potential -75.6 mV. Temperature factor
-q between 3 [2] and 1.5 [3] was used for body temperature.
-
-[1] Tkatch T, Baranauskas G, Surmeier DJ (2000) Kv4.2 mRNA abundance and
-A-type K(+) current amplitude are linearly related in basal ganglia and
-basal forebrain neurons. J Neurosci 20(2):579-88.
-
-[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
+Original data and model by Baranauskas et al (1999) [1] for globus
+pallidus neurons from young adult rat.  The temperature was not
+specified. Potentials were not corrected for the liquid junction
+potential, which was estimated to be 1-2 mV.
+
+Kinetics of m1 type is used as in [2,3]. Room temperature 20-23 C
+is assumed.
+
+NEURON implementation by Alexander Kozlov <akozlov@kth.se>.
+
+[1] Baranauskas G, Tkatch T, Surmeier DJ (1999) Delayed rectifier currents
+in rat globus pallidus neurons are attributable to Kv2.1 and Kv3.1/3.2
+K(+) channels. J Neurosci 19(15):6394-404.
+
+[2] Migliore M, Hoffman DA, Magee JC, Johnston D (1999) Role of an
+A-type K+ conductance in the back-propagation of action potentials in the
+dendrites of hippocampal pyramidal neurons. J Comput Neurosci 7(1):5-15.
 
-[3]  Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
+[3] Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
 Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
 calcium influx and spike timing-dependent plasticity in striatal medium
 spiny neurons. PLoS Comput Biol 8(4):e1002493.
 
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kaf_ms_mod.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/kir_ms.mod`

 * *Files 27% similar despite different names*

```diff
@@ -1,142 +1,147 @@
-TITLE Fast A-type potassium current (Kv4.2)
+TITLE Non-inactivating inwardly rectifying potassium current (Kir2.3)
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 
 NEURON {
-    SUFFIX kaf_ms_mod
+    SUFFIX kir_ms
     USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, q
-    RANGE maxMod
-    POINTER damod
+    RANGE gbar, gk, ik, shift
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
-    gbar = 0.0 (S/cm2) 
-    q = 1	: room temperature (unspecified)
-    :q = 2	: body temperature 35 C (Du 2017)
-    :q = 3	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    gbar = 0.0 	(S/cm2) 
+    shift = 0.0 (mV)
+    q = 1 	: body temperature 35 C
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1
+    levelACh = 0
 }
 
 ASSIGNED {
     v (mV)
     ek (mV)
     ik (mA/cm2)
     gk (S/cm2)
     minf
     mtau (ms)
-    hinf
-    htau (ms)
 }
 
-STATE { m h }
+STATE { m }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gk = gbar*m*m*h*modulation()
+    gk = gbar*m*modulationDA()*modulationACh()
     ik = gk*(v-ek)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
 }
 
 INITIAL {
     rates()
     m = minf
-    h = hinf
 }
 
 PROCEDURE rates() {
     UNITSOFF
-    minf = 1/(1+exp((v-(-10))/(-17.7)))
-    mtau = 0.9+1.1/(1+exp((v-(-30))/10))
-    hinf = 1/(1+exp((v-(-75.6))/11.8))
-    htau = 14
+    minf = 1/(1+exp((v-(-82)-shift)/13))
+    mtau = 1/(exp((v-(-103))/(-14.5))+0.125/(1+exp((v-(-35))/(-19))))
     UNITSON
-
-    :Du 2017
-    :LOCAL alpha, beta, sum
-    :UNITSOFF
-    :alpha = 1.5/(1+exp((v-4)/(-17)))
-    :beta = 0.6/(1+exp((v-10)/9))
-    :sum = alpha+beta
-    :minf = alpha/sum
-    :mtau = 1/sum
-    :
-    :alpha = 0.105/(1+exp((v-(-121))/22))
-    :beta = 0.065/(1+exp((v-(-55))/(-11)))
-    :sum = alpha+beta
-    :hinf = alpha/sum
-    :htau = 1/sum
-    :UNITSON
 }
 
-
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
+FUNCTION modulationACh() {
+    : returns modulation factor
+    
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
+}
 
 COMMENT
 
-Original data by Tkatch et al (2000) [1]. Neostriatal neurons were acutely
-dissociated from young adult rats, age P28-P42.  Electrophysiological
-recordings were done at unspecified temperature (room temperature 20-22 C
-assumed). Potentials were not corrected for the liquid junction potential
-(estimated 1-2 mV).
-
-Activation m^1 matches experimental data [1, Fig.2C]. Activation time
-constants fit tabulated data [1, Fig.2B].  Slope of inactivation function
-fitted to the data [1, Fig.3B] with half inactivation potential -75.6
-mV. Temperature factor q between 1.5 [3] and 3 [2] was used for body
-temperature.  Conductance kinetics of m2h type is used [2], no corrections
-for m^2 applied. Later modification by Du [4] is close to this model.
-
-[1] Tkatch T, Baranauskas G, Surmeier DJ (2000) Kv4.2 mRNA abundance and
-A-type K(+) current amplitude are linearly related in basal ganglia and
-basal forebrain neurons. J Neurosci 20(2):579-88.
+Original model by Wolf et al (2005) [1] for the rat MSN cells from the
+nucleus accumbens.  The activation curve was fitted to a mouse Kir2.1
+channel expressed in HEK cells [2] and shifted to match extracellular
+concentration of K in rat. Measured half-activation values are -109.3
+mV (striatonigral MSN) and -113.2 mV (striatopallidal MSN) [6, Supp
+Tab.1]. Time constants were derived from Aplysia data [3] and adjusted
+to match the rat experiments [1]. Time constant was further tuned [4]
+to fit the rat data below -80 mV [5].  Kinetics is corrected to the body
+temperature 35 C [4].
+
+Non-inactivating Kir current was observed in cells expressing Kir2.2
+and/or Kir2.3 [5]. Activation variable with m^1 kinetics is used [1,4].
+Smooth fit of the time constants by Alexander Kozlov <akozlov@kth.se>.
 
-[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
+[1] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
 
-[3]  Evans RC, Morera-Herreras T, Cui Y, Du K, Sheehan T, Kotaleski JH,
-Venance L, Blackwell KT (2012) The effects of NMDA subunit composition on
-calcium influx and spike timing-dependent plasticity in striatal medium
-spiny neurons. PLoS Comput Biol 8(4):e1002493.
-
-[4] Du K, Wu YW, Lindroos R, Liu Y, Rózsa B, Katona G, Ding JB,
-Kotaleski JH (2017) Cell-type-specific inhibition of the dendritic
-plateau potential in striatal spiny projection neurons. Proc Natl Acad
-Sci USA 114:E7612-E7621.
+[2] Kubo Y, Murata Y (2001) Control of rectification and permeation by
+two distinct sites after the second transmembrane region in Kir2.1 K+
+channel. J Physiol 531, 645-660.
+
+[3] Hayashi H, Fishman HM (1988) Inward rectifier K+ channel kinetics
+from analysis of the complex conductance of aplysia neuronal membrane.
+Biophys J 53, 747-757.
+
+[4] Steephen JE, Manchanda R (2009) Differences in biophysical properties
+of nucleus accumbens medium spiny neurons emerging from inactivation of
+inward rectifying potassium currents. J Comput Neurosci 27(3):453-70
+
+[5] Mermelstein PG, Song WJ, Tkatch T, Yan Z, Surmeier DJ (1998)
+Inwardly rectifying potassium (IRK) currents are correlated with IRK
+subunit expression in rat nucleus accumbens medium spiny neurons. J
+Neurosci 18(17):6650-61.
+
+[6] Shen W, Tian X, Day M, Ulrich S, Tkatch T, Nathanson NM, Surmeier DJ
+(2007) Cholinergic modulation of Kir2 channels selectively elevates
+dendritic excitability in striatopallidal neurons. Nat Neurosci
+10(11):1458-66.
 
 ENDCOMMENT
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/kas_fs.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/cal_ch.mod`

 * *Files 27% similar despite different names*

```diff
@@ -1,117 +1,161 @@
-TITLE Slowly inactivating A-type potassium current (Kv1.2)
+:Migliore file Modify by Maciej Lazarewicz (mailto:mlazarew@gmu.edu) May/16/2001
+
+TITLE l-calcium channel
+: l-type calcium channel
+
+: copy by josh
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
-    SUFFIX kas_fs
-    USEION k READ ek WRITE ik
-    RANGE gbar, gk, ik, shift, q
-    RANGE maxMod
-    POINTER damod
+	SUFFIX cal_ch
+	USEION ca READ cai,cao WRITE ica
+        RANGE  gbar,ica , gcal
+	GLOBAL vhm, vcm
+	GLOBAL Ctm, atm, btm, tm0, vhtm
+        GLOBAL minf,tau
+        RANGE modACh, maxModACh, levelACh
+
 }
 
 UNITS {
-    (S) = (siemens)
-    (mV) = (millivolt)
-    (mA) = (milliamp)
+	(mA) 	= 	(milliamp)
+	(mV) 	= 	(millivolt)
+	FARADAY =  	(faraday)  (kilocoulombs)
+	R 	= 	(k-mole) (joule/degC)
+	KTOMV 	= .0853 (mV/degC)
 }
 
 PARAMETER {
-    gbar = 0.0 	(S/cm2) 
-    a = 0.8
-    :q = 1	: room temperature 22-24 C
-    q = 3	: body temperature 33 C
-    shift = 0
-    damod = 0
-    maxMod = 1
+	v (mV)
+	celsius = 6.3	(degC)
+	gbar	= .003 	(mho/cm2)
+	ki	= .001 	(mM)
+	cai 		(mM)
+	cao 		(mM)
+        tfa	= 1
+	vhm = -1.5
+	vcm = 5.6
+	Ctm = 3
+	atm = 12
+	btm = 11
+	tm0 = 0
+	vhtm = -2
+        modACh = 0
+        maxModACh = 1
+        levelACh = 0
+
 }
 
+STATE { m }
+
 ASSIGNED {
-    v (mV)
-    ek (mV)
-    ik (mA/cm2)
-    gk (S/cm2)
-    minf
-    mtau (ms)
-    hinf
-    htau (ms)
+	ica (mA/cm2)
+        gcal (mho/cm2)
+        minf
+        tau   (ms)
 }
 
-STATE { m h }
-
 BREAKPOINT {
-    SOLVE states METHOD cnexp
-    gk = gbar*m*m*(h*a+1-a)*modulation()
-    ik = gk*(v-ek)
+	SOLVE state METHOD cnexp
+	gcal = gbar*m*m*h2(cai)*modulationACh()
+	ica  = gcal*ghk(v,cai,cao)
 }
 
-DERIVATIVE states {
-    rates()
-    m' = (minf-m)/mtau*q
-    h' = (hinf-h)/htau*q
+INITIAL {
+	rate(v)
+	m = minf
 }
 
-INITIAL {
-    rates()
-    m = minf
-    h = hinf
+FUNCTION h2(cai(mM)) {
+	h2 = ki/(ki+cai)
 }
 
-PROCEDURE rates() {
-    UNITSOFF
-    minf = 1/(1+exp((v-(-27)-shift)/(-16)))
-    mtau = 3.4+89.2*exp(-((v-(-34.3))/30.1)^2)
-    hinf = 1/(1+exp((v-(-33.5)-shift)/21.5))
-    htau = 548.7*6/(exp((v-(-96))/(-29.01))+exp((v-(-96))/100))
-    UNITSON
+FUNCTION ghk(v(mV), ci(mM), co(mM)) (mV) {
+        LOCAL nu,f
+
+        f = KTF(celsius)/2
+        nu = v/f
+        ghk=-f*(1. - (ci/co)*exp(nu))*efun(nu)
+}
+
+FUNCTION KTF(celsius (DegC)) (mV) {
+        KTF = ((25./293.15)*(celsius + 273.15))
+}
+
+FUNCTION efun(z) {
+	if (fabs(z) < 1e-4) {
+		efun = 1 - z/2
+	}else{
+		efun = z/(exp(z) - 1)
+	}
+}
+
+FUNCTION alp(v(mV)) (1/ms) {
+	TABLE FROM -150 TO 150 WITH 200
+	alp = 15.69*(-1.0*v+81.5)/(exp((-1.0*v+81.5)/10.0)-1.0)
 }
 
-FUNCTION modulation() {
+FUNCTION bet(v(mV)) (1/ms) {
+	TABLE FROM -150 TO 150 WITH 200
+	bet = 0.29*exp(-v/10.86)
+}
+
+DERIVATIVE state {  
+        rate(v)
+        m' = (minf - m)/tau
+}
+
+PROCEDURE rate(v (mV)) { :callable from hoc
+        LOCAL a
+
+        a    = alp(v)
+        :tau  = 1/(tfa*(a + bet(v)))
+        :minf = tfa*a*tau
+	tau = Ctm/(exp((v-vhtm)/atm) + exp((vhtm-v)/btm)) + tm0
+	minf = 1/(1+exp(-(v-vhm)/vcm))
+}
+ 
+FUNCTION modulationACh() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
 }
 
-COMMENT
 
-Experimental data by Shen et al (2004) [1]. Medium spiny neurons were
-acutely dissociated from from young adult (P21-P28) Sprague-Dawley rat
-brain. All recordings were conducted at 22-24 C. No correction for the
-liquid junction potential was reported.
-
-Conductance kinetics of m2h type is used [1] with partial inactivation,
-m2 (a h + (1-a)). Fraction a is set to 0.8, as in [1, Fig.6B]; other
-values for a are possible [2] (see also kas.mod in companion code).
-Equation for htau [1] is corrected to match the authors' data [1, Fig.6B]
-by Alexander Kozlov <akozlov@kth.se>.  Time constants were corrected to
-body temperature with factor q=3 [1,3].
-
-[1] Shen W, Hernandez-Lopez S, Tkatch T, Held JE, Surmeier DJ (2004)
-Kv1.2-containing K+ channels regulate subthreshold excitability of
-striatal medium spiny neurons. J Neurophysiol 91(3):1337-49.
-
-[2] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
-O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
-and entrainment to oscillations in a computational model of the nucleus
-accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
-
-[3] Evans RC, Maniar YM, Blackwell KT (2013) Dynamic modulation of
-spike timing-dependent calcium influx during corticostriatal upstates. J
-Neurophysiol 110(7):1631-45.
 
-ENDCOMMENT
+
+
+
+
+
+
+
+
+
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/naf_lts.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/naf_lts.mod`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 TITLE Fast transient sodium current
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
                     e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
     
 ENDCOMMENT
 
 NEURON {
     SUFFIX naf_lts
     USEION na READ ena WRITE ina
-    RANGE gbar, gna, ina
-    RANGE maxMod
+    RANGE gbar, gna, ina, q
+    RANGE modDA, maxModDA, levelDA
 
 }
 
 UNITS {
     (S) = (siemens)
     (mV) = (millivolt)
     (mA) = (milliamp)
 }
 
 PARAMETER {
     gbar = 0.0 (S/cm2) 
     :q = 1	: room temperature 22 C
     q = 1.8	: body temperature 35 C
-    damod = 0
-    maxMod = 1
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
 }
 
 ASSIGNED {
     v (mV)
     ena (mV)
     ina (mA/cm2)
     gna (S/cm2)
@@ -50,15 +62,15 @@
     htau (ms)
 }
 
 STATE { m h }
 
 BREAKPOINT {
     SOLVE states METHOD cnexp
-    gna = gbar*m*m*m*h
+    gna = gbar*m*m*m*h*modulationDA()
     ina = gna*(v-ena)
 }
 
 DERIVATIVE states {
     rates()
     m' = (minf-m)/mtau*q
     h' = (hinf-h)/htau*q
@@ -77,17 +89,22 @@
     :hinf = 1/(1+exp((v-(-63.2))/6))
     :htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
     minf = 1/(1+exp((v-(-25))/(-10)))
     mtau = 0.33+1/(exp((v-(-62))/14)+exp((v-(-60))/(-17)))
     hinf = 1/(1+exp((v-(-62))/6))
     htau = 0.6+1/(exp((v-(-44))/8)+exp((v-(-99))/(-44)))
     UNITSON
+	       }
+	       
+FUNCTION modulationDA() {
+    : returns modulation factor
+    
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
-
 COMMENT
 
 Original data by Ogata and Tatebayashi (1990) [1]. Neostriatal neurons
 of medium size (putative medium spiny neurons) freshly isolated from
 the adult guinea pig brain (either sex, 200 g). Data compensated for
 the liquid junction potential (-13 mV). Experiments carried out at room
 temperature (22 C). Conductance fitted by m3h kinetics.
```

### Comparing `snudda-1.4.0/snudda/data/neurons/mechanismsWithModulation/tmgabaa.mod` & `snudda-1.4.4/snudda/data/neurons/mechanisms/tmgabaa.mod`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 TITLE GABA_A synapse with short-term plasticity
 
 COMMENT
 
-neuromodulation is added as functions:
+Neuromodulation is added as functions:
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA
 
 where:
     
-    damod  [0]: is a switch for turning modulation on or off {1/0}
-    maxMod [1]: is the maximum modulation for this specific channel (read from the param file)
-                e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
-
+    modDA  [0]: is a switch for turning modulation on or off {1/0}
+    maxModDA [1]: is the maximum modulation for this specific channel (read from the param file)
+                    e.g. 10% increase would correspond to a factor of 1.1 (100% +10%) {0-inf}
+    levelDA  [0]: is an additional parameter for scaling modulation. 
+                Can be used simulate non static modulation by gradually changing the value from 0 to 1 {0-1}
+									
+	  Further neuromodulators can be added by for example:
+          modulationDA = 1 + modDA*(maxModDA-1)
+	  modulationACh = 1 + modACh*(maxModACh-1)
+	  ....
+
+	  etc. for other neuromodulators
+	  
+	   
+								     
 [] == default values
 {} == ranges
 
 ENDCOMMENT
 
 NEURON {
     POINT_PROCESS tmGabaA
     RANGE tau1, tau2, e, i, q
     RANGE tau, tauR, tauF, U, u0
-    RANGE failRate, damod, maxMod
+    RANGE modDA, maxModDA, levelDA
+    RANGE modACh, maxModACh, levelACh
+    RANGE failRateDA, failRateACh, failRate
     NONSPECIFIC_CURRENT i
 }
 
 UNITS {
     (nA) = (nanoamp)
     (mV) = (millivolt)
     (uS) = (microsiemens)
@@ -37,18 +50,23 @@
     tau2 = 3.75 (ms)  : ORIG: 7.5ms, tau2 > tau1
     e = -65 (mV)
     tau = 3 (ms)
     tauR = 500 (ms)  : tauR > tau
     tauF = 0 (ms)    : tauF >= 0
     U = 0.1 (1) <0, 1>
     u0 = 0 (1) <0, 1>
-    failRate = 0	
-    damod = 0
-    maxMod = 1
-
+    modDA = 0
+    maxModDA = 1
+    levelDA = 0
+    modACh = 0
+    maxModACh = 1 
+    levelACh = 0
+    failRateDA = 0
+    failRateACh = 0
+    failRate = 0
 }
 
 ASSIGNED {
     v (mV)
     i (nA)
     g (uS)
     factor
@@ -67,15 +85,15 @@
     tp = (tau1*tau2)/(tau2-tau1) * log(tau2/tau1)
     factor = -exp(-tp/tau1) + exp(-tp/tau2)
     factor = 1/factor
 }
 
 BREAKPOINT {
     SOLVE state METHOD cnexp
-    g = (B - A) * modulation()
+    g = (B - A)*modulationDA()*modulationACh()
     i = g*(v - e)
 }
 
 DERIVATIVE state {
     A' = -A/tau1
     B' = -B/tau2
 }
@@ -89,15 +107,15 @@
         tsyn = t
     }
     if ( weight <= 0 ) {
 VERBATIM
         return;
 ENDVERBATIM
     }
-    if( urand() > failRate ) { 
+    if( urand() > failRate*(1 + modDA*(failRateDA-1)*levelDA + modACh*(failRateACh-1)*levelACh)) { 
       z = z*exp(-(t-tsyn)/tauR)
       z = z + (y*(exp(-(t-tsyn)/tau) - exp(-(t-tsyn)/tauR)) / (tau/tauR - 1) )
       y = y*exp(-(t-tsyn)/tau)
       x = 1-y-z
       if (tauF > 0) {
           u = u*exp(-(t-tsyn)/tauF)
           u = u + U*(1-u)
@@ -112,20 +130,25 @@
 }
 
 FUNCTION urand() {
     urand = scop_random(1)
 }
 
 
-FUNCTION modulation() {
+FUNCTION modulationDA() {
     : returns modulation factor
     
-    modulation = 1 + damod*(maxMod-1)
+    modulationDA = 1 + modDA*(maxModDA-1)*levelDA 
 }
 
+FUNCTION modulationACh() {
+    : returns modulation factor
+    
+    modulationACh = 1 + modACh*(maxModACh-1)*levelACh 
+}
 COMMENT
 
 (2019-11-25) Synaptic failure rate (failRate) added. Random factor, no
 reproducibility guaranteed in parallel sim.
 
 (2019-09-12) Set GABA reversal potential to -65mV
 
@@ -147,9 +170,8 @@
 [2] Tsodyks M, Uziel A, Markram H (2000) Synchrony generation in recurrent
 networks with frequency-dependent synapses. J Neurosci. 20(1):RC50.
 
 [3] Wolf JA, Moyer JT, Lazarewicz MT, Contreras D, Benoit-Marand M,
 O'Donnell P, Finkel LH (2005) NMDA/AMPA ratio impacts state transitions
 and entrainment to oscillations in a computational model of the nucleus
 accumbens medium spiny projection neuron. J Neurosci 25(40):9080-95.
-
 ENDCOMMENT
```

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/modulationDAACh.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/WT-P270-20-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c10_D1-mWT-P270-20-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/21-6-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c6_D1-m21-6-DE-v20190503/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/WT-1215MSN03-cor-rep-ax2.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/dspn/str-dspn-e150917_c9_d1-mWT-1215MSN03-v20190521/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e160628_FS2-mMTC180800A-IDB-v20190226/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/DR-rat-Mar-13-08-1-536-R-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161024_FS16-mDR-rat-Mar-13-08-1-536-R-v20190225/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/MTC180800A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e161205_FS1-mMTC180800A-IDB-v20190312/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/MTC251001A-IDB-cor-rep.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/fs/str-fs-e180418_FS5-mMTC251001A-IDB-v20190301/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/51-5-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150908_c4_D2-m51-5-DE-v20190611/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/WT-MSN1-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e150917_c11_D2-mWT-MSN1-v20190603/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/WT-P270-09-15ak-cor.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e151123_c1_D2-mWT-P270-09-v20190527/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/46-3-DE-cor-rep-ax.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/mechanisms.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/ispn/str-ispn-e160118_c10_D2-m46-3-DE-v20190529/parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py` & `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/fix_indexing.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/lts_morp_2019-11-07_centered_no_axon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json` & `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/modulation.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc` & `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/morphologies/lts_morp_2019-11-07_centered_noAxon.swc`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json` & `snudda-1.4.4/snudda/data/neurons/striatum/lts/LTS_Experiment-9862_20181211/parameters.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9857142857142858%*

 * *Differences: {'13': "{'param_name': 'gbar_kdr_lts', 'mech_param': 'gbar'}",*

 * * '14': "{'param_name': 'gbar_kdr_lts', 'mech_param': 'gbar'}"}*

```diff
@@ -93,25 +93,25 @@
         "sectionlist": "somatic",
         "type": "range",
         "value": 5.882451633944143
     },
     {
         "dist_type": "uniform",
         "mech": "kdrb",
-        "mech_param": "gkdrbar",
-        "param_name": "gkdrbar_kdr_lts",
+        "mech_param": "gbar",
+        "param_name": "gbar_kdr_lts",
         "sectionlist": "somatic",
         "type": "range",
         "value": 0.09108261547197531
     },
     {
         "dist_type": "uniform",
         "mech": "kdrb",
-        "mech_param": "gkdrbar",
-        "param_name": "gkdrbar_kdr_lts",
+        "mech_param": "gbar",
+        "param_name": "gbar_kdr_lts",
         "sectionlist": "basal",
         "type": "range",
         "value": 1.3382408358529078e-05
     },
     {
         "dist_type": "uniform",
         "mech": "im",
```

### Comparing `snudda-1.4.0/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json` & `snudda-1.4.4/snudda/data/synapses/example_data/10_MSN12_GBZ_CC_H20.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/example_data/M1LH-contra_dSPN.json` & `snudda-1.4.4/snudda/data/synapses/example_data/M1LH-contra_dSPN.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/formatinfo.txt` & `snudda-1.4.4/snudda/data/synapses/formatinfo.txt`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1LH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/M1RH_Analysis_190925.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-DI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FD-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-FI-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-ID-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json` & `snudda-1.4.4/snudda/data/synapses/striatum/PlanertFitting-II-tmgaba-fit.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json` & `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-LTS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/S1_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json` & `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-CHAT.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-FS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json` & `snudda-1.4.4/snudda/data/synapses/striatum/TH_Analysis_191001.h5-parameters-MS.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DD.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-DI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FD.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-FI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-ID.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-II.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json` & `snudda-1.4.4/snudda/data/synapses/striatum/partial/trace_table.txt-parameters-LI.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_LH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/M1_Analysis_RH_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-LTS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/S1_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-CH-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-FS-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND1-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/TH_Analysis_extr_UP.pxp-traceList-MSND2-require-H20-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-DI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FD-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-FI-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-ID-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json` & `snudda-1.4.4/snudda/data/synapses/v1/trace_table.txt-II-model-parameters.json`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/detect/detect.py` & `snudda-1.4.4/snudda/detect/detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import itertools
 import json
 import os
 import sys
 import time
 import timeit
 from collections import OrderedDict
+import gc
 
 import h5py
 import numexpr
 import numpy as np
 from numba import jit
 
 import snudda.utils.memory
@@ -289,15 +290,15 @@
 
         """
 
         # Normally rc is assigned in init, but let's have option to get it here also
         if rc is not None:
             self.rc = rc
 
-        # We need to setup the workers
+        # We need to set up the workers
         if self.rc is not None:
             d_view = self.rc.direct_view(targets='all')
         else:
             d_view = None
 
         if self.role == "master":
 
@@ -439,23 +440,29 @@
 
                     if voxel_overflow_ctr > 0:
                         self.write_log(f"!!! HyperID {hyper_id} OVERFLOWED {voxel_overflow_ctr} TIMES"
                                        f"(execution time {exec_time} s)", is_error=True)
                         self.voxel_overflow_counter += voxel_overflow_ctr
                     else:
                         if exec_time > 100 or self.verbose:
-                            # Only print the long running hyper voxels
+                            # Only print the hyper voxels taking a long time to complete
                             self.write_log(f"HyperID {hyper_id} completed "
                                            f"- {num_syn} synapses found ({np.around(exec_time, 1)} s)",
                                            force_print=True)
                         elif not info_msg_written:
                             self.write_log(f"Suppressing printouts for hyper voxels that complete in < 100 seconds.",
                                            force_print=True)
                             info_msg_written = True
 
+                    if len(remaining) == 0:
+                        # If there are no more hypervoxels to process, free the memory
+                        # so that any workers still running can have more memory available
+                        cmd_free_str = "sd.free_memory()"
+                        rc["worker_idx"].execute(cmd_free_str, block=False)
+
             # Check that there are neurons in the hyper voxel, otherwise skip it.
             if worker_status[worker_idx] is None and job_idx < len(remaining):
                 self.write_log(f"{time.strftime('%Y-%m-%d %H:%M:%S', time.localtime())}"
                                f" Starting hyper voxel {remaining[job_idx]} on worker {worker_idx}")
 
                 cmd_str = f"result = sd.process_hyper_voxel({remaining[job_idx]})"
                 worker_status[worker_idx] = rc[worker_idx].execute(cmd_str, block=False)
@@ -701,15 +708,15 @@
             # Don't forget to rotate
             axon_cloud = np.matmul(neuron.rotation,
                                    axon_cloud.transpose()).transpose() + neuron.position
 
             axon_loc = np.floor((axon_cloud[:, :3] - self.simulation_origo) / self.hyper_voxel_width).astype(int)
 
         if axon_loc is not None:
-            inside_idx = np.logical_and(0 <= axon_loc, axon_loc < self.hyper_voxel_id_lookup.shape[None, :])
+            inside_idx = np.sum(np.logical_and(0 <= axon_loc, axon_loc < self.hyper_voxel_id_lookup.shape), axis=1) == 3
             hyper_voxel_id = np.unique(self.hyper_voxel_id_lookup[tuple(axon_loc[inside_idx, :].T)])
 
         return hyper_voxel_id
 
     def preallocate_empty_hyper_voxel_dict(self):
 
         # First assign hyperVoxelID to the space
@@ -1039,14 +1046,28 @@
         self.hyper_voxel_rng = np.random.default_rng(random_seed)
 
         self.hyper_voxel_coords[hyper_voxel_id] = hyper_voxel_origo
 
         self.hyper_voxel_origo = hyper_voxel_origo
         self.hyper_voxel_id = hyper_voxel_id
 
+        # Clear lookup tables, just to be safe
+        self.hyper_voxel_synapse_lookup = None
+        self.hyper_voxel_gap_junction_lookup = None
+
+        if SnuddaDetect.memory_fraction_free() < 0.2:
+            # Clear some variables to free memory, reset max values to default, and perform garbage collection
+            self.hyper_voxel_synapses = None
+            self.hyper_voxel_gap_junctions = None
+            self.max_synapses = 2000000
+            self.max_gap_junctions = 100000
+            self.neuron_cache = dict([])
+            self.extra_axon_cache = dict([])
+            gc.collect()
+
         if self.hyper_voxel_synapses is None:
             self.hyper_voxel_synapses = np.zeros((self.max_synapses, 13), dtype=np.int32)
             self.hyper_voxel_synapse_ctr = 0
         else:
             self.hyper_voxel_synapses[:] = 0
             self.hyper_voxel_synapse_ctr = 0
 
@@ -1054,18 +1075,14 @@
             self.hyper_voxel_gap_junctions = np.zeros((self.max_synapses, 11),
                                                       dtype=np.int32)
             self.hyper_voxel_gap_junction_ctr = 0
         else:
             self.hyper_voxel_gap_junctions[:] = 0
             self.hyper_voxel_gap_junction_ctr = 0
 
-        # Clear lookup tables, just to be safe
-        self.hyper_voxel_synapse_lookup = None
-        self.hyper_voxel_gap_junction_lookup = None
-
         # Used by plotHyperVoxel to make sure synapses are displayed correctly
         self.hyper_voxel_offset = None
 
         # Which axons populate the different voxels
         if self.axon_voxels is None:
             self.axon_voxels = np.zeros((self.num_bins[0],
                                          self.num_bins[1],
@@ -1126,14 +1143,42 @@
 
         if self.role == "worker":
             # Let's clear the cache between hyper voxels if we are running in parallel
             # (less chance of cache hits between hyper voxels, and avoid too many copies cached)
             self.neuron_cache = dict()
             self.extra_axon_cache = dict()
 
+    def free_memory(self):
+        # Clear some variables to free memory, reset max values to default, and perform garbage collection
+        self.hyper_voxel_synapses = None
+        self.hyper_voxel_gap_junctions = None
+        self.max_synapses = 2000000
+        self.max_gap_junctions = 100000
+
+        self.neuron_cache = dict([])
+        self.extra_axon_cache = dict([])
+
+        self.axon_voxels = None
+        self.axon_voxel_ctr = None
+        self.axon_soma_dist = None
+
+        self.dend_voxels = None
+        self.dend_voxel_ctr = None
+        self.dend_sec_id = None
+        self.dend_sec_x = None
+        self.dend_soma_dist = None
+
+        mem_available_before = self.memory_fraction_free()
+
+        gc.collect()
+
+        mem_available_after = self.memory_fraction_free()
+
+        self.writelog(f"Hyper voxel memory freed. Free before {mem_available_before}%, free after {mem_available_after}%")
+
     ############################################################################
 
     # hyperID is only needed if we have neurons without axons, ie we use
     # axon density
 
     def detect_synapses(self):
 
@@ -1203,15 +1248,15 @@
                                 cluster_spread = con_dict[con_type]["clusterSpread"]
                                 
                                 if isinstance(cluster_spread, (np.ndarray, list)):
                                     cluster_spread = np.maximum(np.abs(self.hyper_voxel_rng.normal(loc=cluster_spread[0],
                                                                                                    scale=cluster_spread[1])),
                                                                 5e-6)
 
-                                # This uses clone in neuron_prototype which should be cached
+                                # This uses clone in neuron_prototype which should be cached (not anymore, but will be cached for 2nd hit)
                                 neuron = self.load_neuron(self.neurons[d_id])
                                 
                                 try:
                                     cluster_sec_x, syn_coords, soma_dist \
                                         = neuron.cluster_synapses(sec_id=d_sec_id, sec_x=d_sec_x,
                                                                   count=cluster_size, distance=cluster_spread,
                                                                   rng=self.hyper_voxel_rng)
@@ -1351,20 +1396,22 @@
         # 1. Find neurons within hyper voxel that have no axon
         no_axon_neurons = self.hyper_voxels[hyper_id]["axon_density"]
 
         if len(no_axon_neurons) == 0:
             # No neurons without axons
             return
 
-        for na_neuron in no_axon_neurons:
+        for na_neuron_id in no_axon_neurons:
 
             # There are two types of axon density specified
             # - Spherically symmetric
             # - f(x,y,z) in SWC coordinates
 
+            na_neuron = self.neurons[na_neuron_id]
+
             if na_neuron["axonDensityType"] == "r":
 
                 # 2. Check that we have cumulative probability distribution for
                 #    radial distance, if not compute and cache
 
                 if na_neuron["type"] in self.axon_cum_density_cache:
                     (na_cum_density, na_points) = self.axon_cum_density_cache[na_neuron["type"]]
@@ -2376,14 +2423,19 @@
 
                 for neuron_id in hv[hid]["neurons"]:
                     assert neuron_id not in self.hyper_voxels[hid]["neurons"], \
                         f"Internal error, neuron_id {neuron_id } already exists hyper_voxel {hid}"
 
                     self.hyper_voxels[hid]["neurons"][neuron_id] = hv[hid]["neurons"][neuron_id]
 
+                for neuron_id in hv[hid]["axon_density"]:
+                    assert neuron_id not in self.hyper_voxels[hid]["axon_density"], \
+                        f"Internal error, neuron_id {neuron_id} already exists hyper_voxel {hid} (axon_density)"
+                    self.hyper_voxels[hid]["axon_density"].append(neuron_id)
+
         # Sort for reproducibility
         self.count_and_sort_neurons_in_hypervoxels()
         self.generate_hyper_voxel_random_seeds()
 
         # Distribute the new list to all neurons
         d_view.push({"sd.hyper_voxels": self.hyper_voxels}, block=True)
 
@@ -2449,15 +2501,15 @@
 
             for n, d_seed in zip(neurons, distribution_seeds):
 
                 ctr = ctr + 1
                 if ctr % 10000 == 0:
                     self.write_log(f"Assignment counter: {ctr}")
 
-                neuron = self.load_neuron(n)
+                neuron = self.load_neuron(n, use_cache=False)
                 neuron_id = n["neuronID"]
 
                 tree_info = self.get_hypervoxel_coords_and_section_id(neuron=neuron)
                 section_info = self.group_section_info(tree_info=tree_info)
                 density_hyper_voxel_id = self.get_density_location(neuron=neuron, seed=d_seed)
 
                 # First loop over section info, add info
@@ -2644,15 +2696,15 @@
                 # By using "in" for comparison, we can pass a list of volumeID also
                 if volume_id is not None and n["volumeID"] not in volume_id:
                     self.write_log(f"Skipping {n['name']} when calculating hyper voxel size")
                     # Only include neurons belonging to the volume ID
                     # we are looking at now
                     continue
 
-                neuron = self.load_neuron(n)
+                neuron = self.load_neuron(n, use_cache=False)
                 for subtree in neuron.morphology_data.values():
                     try:
                         max_coord = np.maximum(max_coord, np.max(subtree.geometry[:, :3], axis=0))
                         min_coord = np.minimum(min_coord, np.min(subtree.geometry[:, :3], axis=0))
                     except:
                         import traceback
                         print(traceback.format_exc())
@@ -2768,14 +2820,15 @@
         neuron_id : ID of the neurons
         section_id :
 
         """
 
         # Can we move the iterator into numba?
         for section in neuron.section_iterator_selective(section_type=3, section_id=section_id):
+
             voxel_overflow_ctr = SnuddaDetect.fill_voxels_dend_helper(voxel_space=voxel_space,
                                                                       voxel_space_ctr=voxel_space_ctr,
                                                                       voxel_sec_id=voxel_sec_id,
                                                                       voxel_sec_x=voxel_sec_x,
                                                                       voxel_soma_dist=voxel_soma_dist,
                                                                       point_idx=section.point_idx,
                                                                       geometry=section.morphology_data.geometry,
@@ -2784,15 +2837,14 @@
                                                                       self_hyper_voxel_origo=self.hyper_voxel_origo,
                                                                       self_voxel_size=self.voxel_size,
                                                                       self_num_bins=self.num_bins,
                                                                       self_max_dend=self.max_dend,
                                                                       self_step_multiplier=self.step_multiplier)
             self.voxel_overflow_counter += voxel_overflow_ctr
 
-    # Temporarily disabling NUMBA, since amax does not support axis in NUMBA
     @staticmethod
     @jit(nopython=True, fastmath=True, cache=True)
     def fill_voxels_dend_helper(voxel_space, voxel_space_ctr,
                                 voxel_sec_id, voxel_sec_x,
                                 voxel_soma_dist,
                                 point_idx, geometry, section_data, neuron_id: int,
                                 self_hyper_voxel_origo, self_voxel_size,
@@ -2858,23 +2910,18 @@
         for i in range(0, dv_step.shape[0]):
             dv_step[i, :] /= num_steps[i]
 
         ds_step = np.divide(np.diff(section_x), num_steps)
         dd_step = np.divide(np.diff(scaled_soma_dist), num_steps)
 
         # Remove this check later... should be done in morphology_data
-        if (num_steps <= 0).any():
+        if (num_steps <= 0).any(): 
             print(f"Found zero length dendrite segment in neuron_id {neuron_id}")
             raise ValueError(f"Found zero length dendrite segment (please check morphologies).")
 
-        # if neuron_id == 0 and section_id[-1] == 48:
-        #     print("Check the loop, second iteration...")
-        #     import pdb
-        #     pdb.set_trace()
-
         # Loop through all point-pairs of the section
         for idx in range(0, len(scaled_soma_dist)-1):
 
             if point_inside[idx] or point_inside[idx+1]:
                 # Either of the points are within the cube + padding zone
 
                 steps = np.arange(0, num_steps[idx] + 1)
@@ -2939,19 +2986,14 @@
         section_id : section id to add
         subtree : which subtree
 
         """
 
         for section in neuron.section_iterator_selective(section_type=2, section_id=section_id, subtree=subtree):
 
-            # if section.section_id == 219 and neuron_id == 21:
-            #     print("Explore axon")
-            #     import pdb
-            #     pdb.set_trace()
-
             voxel_overflow_ctr = SnuddaDetect.fill_voxels_axon_helper(voxel_space=voxel_space,
                                                                       voxel_space_ctr=voxel_space_ctr,
                                                                       voxel_axon_dist=voxel_axon_dist,
                                                                       point_idx=section.point_idx,
                                                                       geometry=section.morphology_data.geometry,
                                                                       neuron_id=neuron_id,
                                                                       self_hyper_voxel_origo=self.hyper_voxel_origo,
@@ -3108,15 +3150,15 @@
             # !!! Suggestion for optimisation. Place neurons with GJ first, then do
             # GJ touch detection, after that add rest of neurons (to get complete set)
             # and then do axon-dend synapse touch detection
 
             for neuron_id in sorted(self.hyper_voxels[hyper_id]["neurons"].keys()):
 
                 neuron_info = self.hyper_voxels[hyper_id]["neurons"][neuron_id]
-                neuron = self.load_neuron(self.neurons[neuron_id])
+                neuron = self.load_neuron(self.neurons[neuron_id], use_cache=False)  # !!! Cached objects get huge
 
                 if "soma" in neuron_info:
                     self.fill_voxels_soma(self.dend_voxels,
                                           self.dend_voxel_ctr,
                                           self.dend_sec_id,
                                           self.dend_sec_x,
                                           neuron,
@@ -3141,18 +3183,14 @@
                                               voxel_space_ctr=self.axon_voxel_ctr,
                                               voxel_axon_dist=self.axon_soma_dist,
                                               neuron=neuron,
                                               neuron_id=neuron_id,
                                               section_id=section_id,
                                               subtree=subtree)
 
-            # if hyper_id == 813:   #56:
-            #     import pdb
-            #     pdb.set_trace()
-
             # This should be outside the neuron loop
             # This places axon voxels for neurons without axon morphologies
             self.place_synapses_no_axon(hyper_id,
                                         self.axon_voxels,
                                         self.axon_voxel_ctr,
                                         self.axon_soma_dist)
 
@@ -3280,15 +3318,15 @@
 
             num_neurons = self.hyper_voxels[self.hyper_voxel_id]["neuronCtr"]
 
             if plot_neuron_id is None:
                 plot_neuron_id = self.hyper_voxels[self.hyper_voxel_id]["neurons"][:num_neurons]
 
             for neuronID in plot_neuron_id:
-                neuron = self.load_neuron(self.neurons[neuronID])
+                neuron = self.load_neuron(self.neurons[neuronID], use_cache=False)
 
                 neuron.plot_neuron(axis=ax,
                                    plot_axon=draw_axons,
                                    plot_dendrite=draw_dendrites,
                                    plot_origo=self.hyper_voxel_origo, plot_scale=1 / self.voxel_size,
                                    soma_colour=(0, 0, 0),
                                    axon_colour=(1, 0, 0),
@@ -3483,14 +3521,20 @@
     def memory():
 
         memory_available, memory_total = snudda.utils.memory.memory_status()
         res = f"Memory: {memory_available} free, {memory_total} total"
 
         return res
 
+    @staticmethod
+    def memory_fraction_free():
+        memory_available, memory_total = snudda.utils.memory.memory_status()
+
+        return memory_available / memory_total
+
 @staticmethod
 def amax_helper(matrix) -> np.array:
     # Same as numpy.amax with axis=1
 
     max_val = matrix[:, 0].copy()
     for j in range(1, matrix.shape[1]):
         for i in range(0, matrix.shape[0]):
```

### Comparing `snudda-1.4.0/snudda/detect/project.py` & `snudda-1.4.4/snudda/detect/project.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/detect/projection_detection.py` & `snudda-1.4.4/snudda/detect/projection_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/detect/prune.py` & `snudda-1.4.4/snudda/detect/prune.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,21 +352,22 @@
                 merge_files_gj : List of files containing gap junctions
                 merge_neuron_range_gj : List of neuron ranges in each file
                 merge_gj_ctr : List of gap junction count for each file
 
         """
 
         if not os.path.exists(self.merge_info_file):
+            print(f"No file {self.merge_info_file}")
             return None
 
         try:
             merge_files_syn, merge_neuron_range_syn, merge_syn_ctr, \
             merge_files_gj, merge_neuron_range_gj, merge_gj_ctr = self.get_merge_info_helper()
         except:
-            self.write_log(f"Problem readin merge info from {self.merge_info_file}")
+            self.write_log(f"Problem reading merge info from {self.merge_info_file}")
             return None
 
         # Check that the merge info file is more recent than all the files it refer to
 
         merge_info_time = os.path.getmtime(self.merge_info_file)
         for f_name in merge_files_syn + merge_files_gj:
             if f_name is not None and not os.path.exists(f_name):
@@ -683,15 +684,15 @@
         if config_file is None:
             config_file = self.hist_file["meta/configFile"][()]
 
         self.check_network_config_integrity(config_file=config_file)
         with open(config_file, "r") as f:
             self.config = json.load(f, object_pairs_hook=collections.OrderedDict)
 
-        self.population_unit_id = self.hist_file["network/neurons/populationUnitID"][()]
+        self.population_unit_id = self.hist_file["network/neurons/populationUnitID"][()].copy()
 
         # Normally we use type names as lookups, but since we will do this
         # many millions of times, we create an temporary typeID number
         self.make_type_numbering()
 
         orig_connectivity_distributions = json.loads(self.hist_file["meta/connectivityDistributions"][()],
                                                      object_pairs_hook=collections.OrderedDict)
@@ -807,15 +808,25 @@
             self.write_log(f"Output file already set: {self.out_file.filename}")
             return
 
         if output_file is None:
             output_file = os.path.join(self.network_path, "network-synapses.hdf5")
 
         self.write_log(f"Writing to {output_file}")
-        out_file = h5py.File(output_file, "w", libver=self.h5libver, driver=self.h5driver)
+
+        # Already hdf5 file, add to it
+        if isinstance(output_file, h5py._hl.files.File):
+            out_file = output_file
+
+            if "config" in out_file:
+                self.write_log(f"Output file already has config, assuming all data present: {out_file.filename}")
+                return
+        else:
+            out_file = h5py.File(output_file, "w", libver=self.h5libver, driver=self.h5driver)
+
         out_file.create_dataset("config", data=json.dumps(self.config))
 
         # Copy over meta data
         self.hist_file.copy("meta", out_file)
 
         cfg = json.loads(self.hist_file["meta/config"][()], object_pairs_hook=collections.OrderedDict)
         morph_group = out_file.create_group("morphologies")
```

### Comparing `snudda-1.4.0/snudda/help.py` & `snudda-1.4.4/snudda/help.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/init/init.py` & `snudda-1.4.4/snudda/init/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -915,15 +915,15 @@
                                   slice_depth=slice_depth,
                                   d_min=d_min)
 
         elif num_neurons <= 1e6:  # 1e6
             print("Using cube for striatum")
             # 1.73 million neurons, volume of allen striatal mesh is 21.5mm3
             striatum_volume = 1e-9 * num_neurons / neuron_density  # 80.5e3
-            striatum_side_len = striatum_volume ** (1. / 3)
+            striatum_side_len = np.maximum(striatum_volume ** (1. / 3), 50e-6)  # We do a minimum of 10 micrometer cube
             striatum_centre = np.array([4750e-6, 4000e-6, 7750e-6])
 
             if num_neurons < 500:
                 mesh_bin_width = striatum_side_len
             elif num_neurons < 5000:
                 mesh_bin_width = striatum_side_len / 5
             else:
```

### Comparing `snudda-1.4.0/snudda/init/init_custom.py` & `snudda-1.4.4/snudda/init/init_custom.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/init/init_wojtek.py` & `snudda-1.4.4/snudda/init/init_wojtek.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/input/input.py` & `snudda-1.4.4/snudda/input/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -539,16 +539,22 @@
         """ Read input configuration from JSON file. """
 
         self.write_log(f"Loading input configuration from {self.input_config_file}")
 
         with open(snudda_parse_path(self.input_config_file, self.snudda_data), 'rt') as f:
             self.input_info = json.load(f, object_pairs_hook=OrderedDict)
 
+        max_time = self.time
+
         for neuron_type in self.input_info:
             for input_type in self.input_info[neuron_type]:
+
+                if "end" in self.input_info[neuron_type][input_type]:
+                    max_time = max(max_time, np.max(self.input_info[neuron_type][input_type]["end"]))
+
                 if "parameterFile" in self.input_info[neuron_type][input_type]:
                     # Allow user to use $DATA to refer to snudda data directory
                     par_file = snudda_parse_path(self.input_info[neuron_type][input_type]["parameterFile"],
                                                  self.snudda_data)
 
                     with open(par_file, 'r') as f:
                         par_data_dict = json.load(f, object_pairs_hook=OrderedDict)
@@ -573,14 +579,19 @@
                     self.input_info[neuron_type][input_type]["parameterList"] = par_data
                 except:
                     import traceback
                     self.write_log(traceback.format_exc(), is_error=True)
                     self.write_log(f"Did you forget to specify the name of the input to {neuron_type}?")
                     sys.exit(-1)
 
+        if max_time > self.time:
+            self.write_log(f"Found input that ends at {max_time}, "
+                           f"increasing input generation from {self.time} to {max_time}", force_print=True)
+            self.time = max_time
+
     ############################################################################
 
     # Each synaptic input will contain a fraction of population unit spikes, which are
     # taken from a stream of spikes unique to that particular population unit
     # This function generates these correlated spikes
 
     def make_population_unit_spike_trains(self, rng):
@@ -614,16 +625,21 @@
 
                 if "populationUnitID" in self.input_info[cell_type][input_type]:
                     pop_unit_list = self.input_info[cell_type][input_type]["populationUnitID"]
 
                     if type(pop_unit_list) != list:
                         pop_unit_list = [pop_unit_list]
                 else:
+                    # We do not want to generate "global" mother spikes for population unit 0
+                    # For population unit 0, mother spikes are unique to each neuron
                     pop_unit_list = self.all_population_units
 
+                # This makes sure that we do not give population unit wide mother spikes to population unit 0
+                pop_unit_list = set(pop_unit_list) - {0}
+
                 if input_type == "VirtualNeuron":
                     # No population unit spike trains needed for virtual neurons, reads input from file
                     pass
 
                 # Handle Poisson input
                 elif self.input_info[cell_type][input_type]["generator"] == "poisson":
 
@@ -1674,27 +1690,27 @@
         if "PopulationUnits" in self.network_config:
 
             all_id = []
             for volume in self.network_config["PopulationUnits"]:
                 if "unitID" in self.network_config["PopulationUnits"][volume]:
                     all_id += self.network_config["PopulationUnits"][volume]["unitID"]
 
-            all_id = sorted(all_id)
+            all_id = set(all_id) - {0}
 
             if "AllUnitID" in self.network_config["PopulationUnits"]:
-                self.all_population_units = sorted(self.network_config["PopulationUnits"]["AllUnitID"])
+                self.all_population_units = set(self.network_config["PopulationUnits"]["AllUnitID"])
                 assert all_id == self.all_population_units, \
                     (f"Inconsistency: AllUnitID = {self.all_population_units}, "
                      f"but all units in unitID blocks = {all_id}")
             else:
                 self.write_log("Missing AllUnitID tag, deriving it from unitID tag for volumes")
                 self.all_population_units = all_id
 
         else:
-            self.all_population_units = [0]
+            self.all_population_units = {}
 
     def generate_seeds(self, num_states):
 
         """ From the master seed, generate a seed sequence for inputs. """
 
         ss = np.random.SeedSequence(self.random_seed)
         all_seeds = ss.generate_state(num_states + 1)
@@ -2085,15 +2101,15 @@
                 (f"Virtual neuron {self.neuron_name[neuron_id]}"
                  f" should have only one spike train, fix nSpikeTrains in config")
 
             # Virtual neurons input handled through touch detection
             input_loc = None
 
             num_inputs = 1
-            p_keep = np.divide(1, (num_inputs - np.sqrt(correlation) * (num_inputs - 1)))
+            p_keep = np.sqrt(correlation)
 
             # !!! Pass the input_generator
             spikes = self.make_correlated_spikes(freq=freq,
                                                  time_range=time_range,
                                                  num_spike_trains=1,
                                                  p_keep=p_keep,
                                                  population_unit_spikes=population_unit_spikes,
```

### Comparing `snudda-1.4.0/snudda/input/input_tuning.py` & `snudda-1.4.4/snudda/input/input_tuning.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/input/inspectinput.py` & `snudda-1.4.4/snudda/input/inspectinput.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/input/time_varying_input.py` & `snudda-1.4.4/snudda/input/time_varying_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/input/virtual_input.py` & `snudda-1.4.4/snudda/input/virtual_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neuromodulation/modulation.py` & `snudda-1.4.4/snudda/neuromodulation/modulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neuromodulation/modulation_network.py` & `snudda-1.4.4/snudda/neuromodulation/modulation_network.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neuromodulation/modulation_synapse.py` & `snudda-1.4.4/snudda/neuromodulation/modulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neuromodulation/neuromodulation.py` & `snudda-1.4.4/snudda/neuromodulation/neuromodulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neuromodulation/neuromodulation_synapse.py` & `snudda-1.4.4/snudda/neuromodulation/neuromodulation_synapse.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neurons/index_tree.py` & `snudda-1.4.4/snudda/neurons/index_tree.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neurons/morphology_data.py` & `snudda-1.4.4/snudda/neurons/morphology_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import pickle
 
 import numpy as np
-from copy import deepcopy
 from scipy.spatial import cKDTree
 
 import snudda.utils
 
 # TODO: Move constants like 1000 * sec_x to separate file
 
 
@@ -14,19 +13,23 @@
 
     """ Holds parent_id, children_id, points_id"""
 
     __slots__ = ["section_id", "parent_section_id", "parent_point_idx", "parent_section_type",
                  "child_section_id", "point_idx", "section_type",
                  "morphology_data", "neuron_id"]
 
+    # Använd numpy structured arrays? https://numpy.org/doc/stable/user/basics.rec.html
+    # Ta bort slots??
+    # Dataclass: https://stackoverflow.com/questions/35988/c-like-structures-in-python/45426493#45426493
+
     section_id: int
     parent_section_idx: int
     parent_point_idx: int
     parent_section_type: int
-    child_section_id: dict
+    child_section_id: np.ndarray  # First row is child_section_id, second row is child_section_type
     point_idx: np.ndarray
     section_type: int
     morphology_data: object
     neuron_id: int  # Is this set, is it used?
 
     def __init__(self, section_id, section_type, morphology_data, build_section=True):
 
@@ -42,15 +45,15 @@
 
         if build_section:
             self.build_section()
 
     def build_section(self):
 
         idx = np.where((self.morphology_data.section_data[:, 0] == self.section_id)
-                       & (self.morphology_data.section_data[:, 2] == self.section_type))[0]
+                       & (self.morphology_data.section_data[:, 2] == self.section_type))[0].astype(np.int32)
 
         if len(idx) == 0:
             raise ValueError(f"Section id {self.section_id} has no points in morphology_data")
 
         if not (np.diff(idx) == 1).all():
             raise ValueError(f"Points on section must be consecutive")
 
@@ -60,38 +63,47 @@
             self.point_idx = idx
             self.parent_point_idx = -1
             self.parent_section_type = -1
             self.parent_section_id = -9999
         elif self.morphology_data.section_data[parent_idx, 2] != self.morphology_data.section_data[idx[0], 2]:
             # Special case, root node -- parent section is of different type (e.g. soma -- dend)
             self.point_idx = idx
-            self.parent_point_idx = self.morphology_data.section_data[self.point_idx[0], 3]
-            self.parent_section_type = self.morphology_data.section_data[parent_idx, 2]
-            self.parent_section_id = self.morphology_data.section_data[self.parent_point_idx, 0]
+            self.parent_point_idx = int(self.morphology_data.section_data[self.point_idx[0], 3])
+            self.parent_section_type = int(self.morphology_data.section_data[parent_idx, 2])
+            self.parent_section_id = int(self.morphology_data.section_data[self.parent_point_idx, 0])
         else:
-            self.point_idx = np.concatenate(([self.morphology_data.section_data[idx[0], 3]], idx))
-            self.parent_point_idx = self.morphology_data.section_data[self.point_idx[0], 3]
-            self.parent_section_type = self.morphology_data.section_data[parent_idx, 2]
-            self.parent_section_id = self.morphology_data.section_data[self.parent_point_idx, 0]
+            self.point_idx = np.concatenate(([self.morphology_data.section_data[idx[0], 3]], idx), dtype=np.int32)
+            self.parent_point_idx = int(self.morphology_data.section_data[self.point_idx[0], 3])
+            self.parent_section_type = int(self.morphology_data.section_data[parent_idx, 2])
+            self.parent_section_id = int(self.morphology_data.section_data[self.parent_point_idx, 0])
 
         # By definition only the last point in a section can be a parent to other sections
         child_idx = np.where(self.morphology_data.section_data[:, 3] == idx[-1])[0]
 
-        self.child_section_id = dict()
+        temp_child_section_id = dict()
         for child_section_id, child_type in zip(self.morphology_data.section_data[child_idx, 0],
                                                 self.morphology_data.section_data[child_idx, 2]):
             # self.child_section_id is a dict, which holds the child_section_id for different
             # types (e.g. 1=soma, 2=axon, 3=dend, 4=apical)
-            if child_type not in self.child_section_id:
-                self.child_section_id[child_type] = []
+            if child_type not in temp_child_section_id:
+                temp_child_section_id[child_type] = []
+
+            temp_child_section_id[child_type].append(child_section_id)
 
-            self.child_section_id[child_type].append(child_section_id)
+#        for child_type in self.child_section_id.keys():
+#            self.child_section_id[child_type] = np.array(self.child_section_id[child_type])
 
-        for child_type in self.child_section_id.keys():
-            self.child_section_id[child_type] = np.array(self.child_section_id[child_type])
+        section_id = []
+        section_type = []
+        for child_type in temp_child_section_id.keys():
+            section_id += temp_child_section_id[child_type]
+            section_type += [child_type]*len(temp_child_section_id[child_type])
+
+        # Convert dictionary to np.array to conserve memory
+        self.child_section_id = np.array([section_id, section_type], dtype=np.int16)
 
         # Also check it above
         bastard_idx = np.where((idx[0] <= self.morphology_data.section_data[:, 3])
                                & (self.morphology_data.section_data[:, 3] < idx[-1]))[0]
 
         if not (bastard_idx == idx[1:]).all():
             raise ValueError(f"Only last point in section may have children outside section.")
@@ -119,16 +131,20 @@
             new_smd.point_idx = self.point_idx
             new_smd.parent_point_idx = self.parent_point_idx
             new_smd.child_section_id = self.child_section_id
             new_smd.parent_section_id = self.parent_section_id
 
             # Prevent the user from changing these now that the memory is shared
             self.point_idx.setflags(write=False)
-            for cs in self.child_section_id.values():
-                cs.setflags(write=False)
+
+            # for cs in self.child_section_id.values():
+            #     cs.setflags(write=False)
+
+            self.child_section_id.setflags(write=False)
+
         else:
             new_smd.point_idx = self.point_idx.copy()
             new_smd.parent_point_idx = self.parent_point_idx
             new_smd.parent_section_id = self.parent_section_id
 
             new_smd = dict()
             for key, val in self.child_section_id.items():
@@ -141,14 +157,18 @@
         return self.morphology_data.geometry[self.point_idx, :3]
 
     @property
     def radie(self):
         return self.morphology_data.geometry[self.point_idx, 3]
 
     @property
+    def soma_distance(self):
+        return self.morphology_data.geometry[self.point_idx, 4]
+
+    @property
     def section_x(self):
         # Double check that this creates a copy of the data before overwriting first element with 0
         sec_x = self.morphology_data.section_data[self.point_idx, 1] / 1e3
         if self.parent_section_type != 1:
             # If parent is not soma, set first section_x to 0
             sec_x[0] = 0
         return sec_x
@@ -164,15 +184,20 @@
         Args:
             swc_file (str): Path to SWC file
             parent_tree_info (tuple, optional): Specify subtree attachment point
                                                 (MorphologyData, parent_label, parent_point_idx, arc_factor)
 
     """
 
-    def __init__(self, swc_file=None, parent_tree_info=None, snudda_data=None, verbose=False, use_cache=True):
+    __slots__ = ["swc_file", "snudda_data", "verbose", "cache_version",
+                 "geometry", "section_data", "sections",
+                 "point_lookup", "rotation", "position", "parent_tree_info", "is_loaded", "kd_tree_lookup"]
+
+    def __init__(self, swc_file=None, parent_tree_info=None, snudda_data=None,
+                 verbose=False, use_cache=True, lazy_loading=False):
 
         self.swc_file = swc_file
         self.snudda_data = snudda_data
         self.verbose = verbose
         self.cache_version = 1.4
 
         self.geometry = None      # x, y, z, r, soma_dist (float)
@@ -181,62 +206,56 @@
 
         self.point_lookup = dict()    # "dend" --> np.array of point_id for dend points
 
         self.rotation = None
         self.position = None
 
         self.parent_tree_info = parent_tree_info     # parent tree, if subtree
-
-        if swc_file is not None:
-            self.load_swc_file(swc_file=swc_file, use_cache=use_cache)
+        self.is_loaded = False
+        
+        if not lazy_loading and self.swc_file is not None:
+            self.load_swc_file(swc_file=self.swc_file, use_cache=use_cache)
 
         self.kd_tree_lookup = dict()
 
-    def section_iterator(self, section_type):
-
-        """ Iterates over all sections of a specific type.
-
-        Args:
-            section_type: 1 = soma, 2 = axon, 3 = dend """
-
-        for section in self.sections[section_type].values():
-            yield section
-
     def section_iterator_selective(self, section_type, section_id):
 
         """ Iterates over all sections of a specific type.
 
         Args:
             section_type: 1 = soma, 2 = axon, 3 = dend
             section_id: ID of sections to iterate over"""
 
         if section_id is None:
             section_id = self.sections[section_type].keys()
 
         for sid in section_id:
             yield self.sections[section_type][sid]
 
-    def load_swc_file(self, swc_file, remapping_types={4: 3}, use_cache=True):
+    def load_swc_file(self, swc_file=None, remapping_types={4: 3}, use_cache=True):
 
         """ Loads SWC morphology, not SNUDDA_DATA aware (file must exist).
 
             Args:
                 swc_file (str): Path to swc file
                 remapping_types (dict): Remapping of compartment types (default: 4 (apical) -> 3 (normal dendrites))
+                use_cache (bool): Save and load neuron morphology to cache
         """
+        if swc_file is None:
+            swc_file = self.swc_file
 
         swc_file = snudda.utils.snudda_parse_path(swc_file, self.snudda_data)
 
         if not os.path.isfile(swc_file):
             raise FileNotFoundError(f"Missing SWC file '{swc_file}'")
 
         if use_cache:
             cache_file, valid_cache = self.get_cache_file()
-
             if valid_cache and self.load_cache():
+                self.is_loaded = True
                 return
 
         data = np.loadtxt(swc_file)
 
         if any(np.diff(data[:, 0]) != 1):
             raise IndexError(f"SWC file has gaps in ID numbering ({swc_file})")
 
@@ -255,19 +274,19 @@
         item, count = np.unique(data[:, 0], return_counts=True)
         if (count > 1).any():
             raise ValueError(f"Duplicate index: {item[count > 1]} ({swc_file})")
 
         if self.parent_tree_info is not None and (data[:, 1] != 2).any():
             raise ValueError(f"Only axonal compartments allowed when subtree of neuron")
 
-        self.geometry = np.zeros((data.shape[0], 5), dtype=float)
+        self.geometry = np.zeros((data.shape[0], 5), dtype=np.single)  # 2023-04-24: float -> single, to save memory
         self.geometry[:, :4] = data[:, 2:6] * 1e-6  # x, y, z, r -- converted to meter
 
         # Store metadata for points
-        self.section_data = np.full((data.shape[0], 4), -1, dtype=int)
+        self.section_data = np.full((data.shape[0], 4), -1, dtype=np.int32)
         self.section_data[:, 2] = data[:, 1]
         self.section_data[0, 3] = -1
         parent_row_id = data[1:, 6].astype(int) - 1
         self.section_data[1:, 3] = parent_row_id
 
         # This remaps apical dendrites to normal dendrites 4 --> 3 (by default)
         for old_key, new_key in remapping_types.items():
@@ -300,15 +319,17 @@
 
         if (self.geometry[1:, 4] < 0).any():
             raise ValueError("Found compartments with 0 or negative distance to soma.")
 
         self.build_tree()
 
         if use_cache:
-            self.save_cache()
+            self.save_cache(skip_check=True)  # skip_check since we have not done any rotations
+
+        self.is_loaded = True
 
     def build_tree(self):
 
         # New sections are triggered when:
         # -- At branch points
         # -- Change of section type
         parent_id, counts = np.unique(self.section_data[:, 3], return_counts=True)
@@ -327,16 +348,14 @@
             parent_id = row[3]
 
             if parent_id == -1 or edge_flag[parent_id]:
 
                 # https://github.com/neuronsimulator/nrn/blob/5038de0b79ddf7da9b536639989da4c10dbae7f7/share/lib/hoc/import3d/read_swc.hoc?fbclid=IwAR2kEJOcWkbze8i6G2t9uUVZn5MfmxdSHtm3yzWdP240guJY9KFCalUMvug#L304
                 if parent_id == 0 and idx in branch_id:
 
-                    # import pdb
-                    # pdb.set_trace()
                     # Special case, parent is soma, and the point itself is a branch point
                     # then mark it as section_type = 0, to not create a one point section
                     self.section_data[idx, 2] = 0
                     section_type = 0
 
                 # Parent point is edge, create new section
                 if section_type not in section_counter:
@@ -393,19 +412,19 @@
                                                                           section_type=section_type,
                                                                           morphology_data=self)
         # Create point lookup
         for section_type in self.sections:
             idx = np.where(self.section_data[:, 2] == section_type)[0]
             self.point_lookup[section_type] = idx
 
-    def save_cache(self):
+    def save_cache(self, skip_check=False):
 
         cache_file, _ = self.get_cache_file()
 
-        if self.rotation is not None or self.position is not None:
+        if not skip_check and (self.rotation is not None or self.position is not None):
             raise ValueError(f"Position and rotation must be None when calling save_cache: {self.swc_file}")
 
         if self.parent_tree_info is not None:
             raise ValueError(f"Parent tree info must be None when calling save_cache: {self.swc_file}")
 
         data = dict()
         data["cache_version"] = self.cache_version
@@ -422,28 +441,29 @@
                 data["sections"][sect_type][sect_key]["section_type"] = sect_value.section_type
 
                 data["sections"][sect_type][sect_key]["parent_point_idx"] = sect_value.parent_point_idx
                 data["sections"][sect_type][sect_key]["parent_section_id"] = sect_value.parent_section_id
                 data["sections"][sect_type][sect_key]["parent_section_type"] = sect_value.parent_section_type
                 data["sections"][sect_type][sect_key]["point_idx"] = sect_value.point_idx
 
-                data["sections"][sect_type][sect_key]["child_section_id"] = dict()
-                for ch_key, ch_value in sect_value.child_section_id.items():
-                    data["sections"][sect_type][sect_key]["child_section_id"][ch_key] = ch_value
+                # data["sections"][sect_type][sect_key]["child_section_id"] = dict()
+                # for ch_key, ch_value in sect_value.child_section_id.items():
+                #     data["sections"][sect_type][sect_key]["child_section_id"][ch_key] = ch_value
+
+                data["sections"][sect_type][sect_key]["child_section_id"] = sect_value.child_section_id
 
         try:
             with open(cache_file, "wb") as f:
                 pickle.dump(data, f)
         except:
             print(f"Unable to save cache file {cache_file} -- do you have write permission?")
 
     def load_cache(self):
 
         cache_file, valid_cache = self.get_cache_file()
-
         cache_loaded = False
 
         if valid_cache:
             try:
                 with open(cache_file, "rb") as f:
                     data = pickle.load(f)
 
@@ -454,29 +474,36 @@
                     raise ValueError(f"Cache mismatch.")
 
                 self.geometry = data["geometry"]
                 self.section_data = data["section_data"]
 
                 self.sections = dict()
                 for sect_type in data["sections"].keys():
-                    assert np.issubdtype(type(sect_type), np.integer), f"sec_type must be int, found {sect_type} ({type(sect_type)})"
+                    assert np.issubdtype(type(sect_type), np.integer), \
+                        f"sec_type must be int, found {sect_type} ({type(sect_type)})"
                     self.sections[sect_type] = dict()
                     for sect_id, sect_val in data["sections"][sect_type].items():
-                        assert np.issubdtype(type(sect_id), np.integer), f"sec_id key must be int, found sec_id = {sect_id} ({type(sect_id)}"
+                        assert np.issubdtype(type(sect_id), np.integer), \
+                            f"sec_id key must be int, found sec_id = {sect_id} ({type(sect_id)}"
                         sec = SectionMetaData(section_id=sect_id, section_type=sect_type,
                                               morphology_data=self, build_section=False)
                         sec.point_idx = sect_val["point_idx"]
-                        sec.parent_point_idx = sect_val["parent_point_idx"]
-                        sec.parent_section_id = sect_val["parent_section_id"]
 
-                        sec.parent_section_type = sect_val["parent_section_type"]
+                        assert sec.point_idx.dtype == np.int32, f"Old format. New format is 32-bit integer"
+
+                        sec.parent_point_idx = int(sect_val["parent_point_idx"])
+                        sec.parent_section_id = int(sect_val["parent_section_id"])
+
+                        sec.parent_section_type = int(sect_val["parent_section_type"])
+
+                        # sec.child_section_id = dict()
+                        # for ch_key, ch_val in sect_val["child_section_id"].items():
+                        #     sec.child_section_id[ch_key] = ch_val
 
-                        sec.child_section_id = dict()
-                        for ch_key, ch_val in sect_val["child_section_id"].items():
-                            sec.child_section_id[ch_key] = ch_val
+                        sec.child_section_id = sect_val["child_section_id"]
 
                         self.sections[sect_type][sect_id] = sec
 
                 cache_loaded = True
 
             except:
                 print(f"Failed to load cache from {cache_file}")
@@ -620,14 +647,15 @@
             # Assuming topology of neuron does not change, these values will be constant
             new_md.section_data = self.section_data
             self.section_data.setflags(write=False)
 
             for p_key, p_value in self.point_lookup.items():
                 new_md.point_lookup[p_key] = p_value
                 p_value.setflags(write=False)
+
         else:
             new_md.section_data = self.section_data.copy()
 
             for p_key, p_value in self.point_lookup.items():
                 new_md.point_lookup[p_key] = p_value.copy()
 
         new_md.sections = dict()
@@ -642,30 +670,15 @@
         new_md.kd_tree_lookup = dict()
         new_md.parent_tree_info = parent_tree_info
 
         new_md.place(position=position, rotation=rotation)
 
         return new_md
 
-    def place(self, position=None, rotation=None, parent_tree_info=None):
-
-        if parent_tree_info is not None:
-            self.parent_tree_info = parent_tree_info  # (MorphologyData, point_idx, arc_factor)
-
-        # Here we assume soma is only a point
-        if 1 in self.point_lookup:
-            soma_position = self.geometry[self.point_lookup[1], :3]
-            if not (soma_position == 0).all():
-                raise ValueError("Soma must be centered at origo before placement.")
-        elif 2 in self.point_lookup:
-            # We have no soma, so it is probably an axonal tree, check that it is centered
-            axon_root_position = self.geometry[self.point_lookup[2][0], :3]
-            if not (axon_root_position == 0).all():
-                raise ValueError("Axon root must be centered at origo before placement.")
-
+    def place(self, position=None, rotation=None, parent_tree_info=None, lazy=False):
         if self.position is not None or self.rotation is not None:
             raise ValueError("Not allowed to rotate or position a neuron that has already been rotated or positioned")
 
         if isinstance(rotation, (list, tuple)):
             rotation = np.array(rotation)
         else:
             rotation = rotation.copy() if rotation is not None else None
@@ -675,37 +688,62 @@
         if isinstance(position, (list, tuple)):
             position = np.array(position)
         else:
             position = position.copy() if position is not None else None
 
         self.position = position
 
+        if lazy:
+            return
+
+        if not self.is_loaded:
+            self.load_swc_file()
+
+        if parent_tree_info is not None:
+            self.parent_tree_info = parent_tree_info  # (MorphologyData, point_idx, arc_factor)
+
+        # Here we assume soma is only a point
+        if 1 in self.point_lookup:
+            soma_position = self.geometry[self.point_lookup[1], :3]
+            if not (soma_position == 0).all():
+                raise ValueError("Soma must be centered at origo before placement.")
+        elif 2 in self.point_lookup:
+            # We have no soma, so it is probably an axonal tree, check that it is centered
+            axon_root_position = self.geometry[self.point_lookup[2][0], :3]
+            if not (axon_root_position == 0).all():
+                raise ValueError("Axon root must be centered at origo before placement.")
+
         if rotation is not None:
             if not np.abs(np.linalg.det(rotation) - 1) < 1e-10 \
                     or not np.abs(np.matmul(rotation, rotation.T) - np.eye(3) < 1e-10).all():
                 raise ValueError(f"Not a valid rotation matrix {rotation}")
 
             self.geometry[:, :3] = np.matmul(self.rotation, self.geometry[:, :3].T).T
 
         if self.position is not None:
             self.geometry[:, :3] += self.position
 
         if self.parent_tree_info is not None:
             # We need to update soma distance for subtree based on distance to parent
-            # self.parent_tree = (MorphologyData, point_idx, arc_factor) -- attachment point
+            # parent_tree_info = (MorphologyData, point_idx, arc_factor) -- attachment point
 
-            parent_object, parent_point_idx, arc_factor = self.parent_tree
-            parent_position = self.parent_object.geometry[parent_point_idx, :3]
-            parent_soma_distance = self.parent_object.geometry[parent_point_idx, 4]
+            parent_object, parent_point_idx, arc_factor = self.parent_tree_info
+            parent_position = parent_object.geometry[parent_point_idx, :3]
+            parent_soma_distance = parent_object.geometry[parent_point_idx, 4]
 
             dist_to_parent = np.linalg.norm(self.position - parent_position)
             self.geometry[:, 4] += parent_soma_distance + dist_to_parent * arc_factor
 
     def section_iterator(self, section_type=None):
 
+        """ Iterates over all sections of a specific type.
+
+        Args:
+            section_type: 1 = soma, 2 = axon, 3 = dend """
+
         if section_type is None:
             for section_dict in self.sections.values():
                 for section in section_dict:
                     yield section
 
         elif section_type in self.sections:
             for section in self.sections[section_type].values():
@@ -775,8 +813,8 @@
 if __name__ == "__main__":
 
     # file_name = "/home/hjorth/HBP/BasalGangliaData/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20211026/morphology/WT-0728MSN01-cor-rep-ax-res3.swc"
     file_name = "/home/hjorth/HBP/BasalGangliaData/Parkinson/20220225/PD0/neurons/striatum/dspn/26/WT-1215MSN03-cor-rep-ax-res3-var8.swc"
     md = MorphologyData(swc_file=file_name)
 
     import pdb
-    pdb.set_trace()
+    pdb.set_trace()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snudda-1.4.0/snudda/neurons/neuron_model_extended.py` & `snudda-1.4.4/snudda/neurons/neuron_model_extended.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neurons/neuron_morphology.py` & `snudda-1.4.4/snudda/neurons/neuron_morphology.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/neurons/neuron_morphology_extended.py` & `snudda-1.4.4/snudda/neurons/neuron_morphology_extended.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.virtual_neuron = virtual_neuron
         self.colour = colour
 
         self.morphology_data = dict()
 
         # Can we remove these:
         self.axon_density_type = None
-        self.dend_density = None
+        # self.dend_density = None
         self.axon_density = None
         self.max_axon_radius = None
         self.axon_density_bounds_xyz = None
         self.voxel_size = 5e6
         self.density_bin_size = 10e-6
         # Or are they required for axon densities?
 
@@ -92,41 +92,42 @@
         self._position = position
 
     @rotation.setter
     def rotation(self, rotation):
         self._rotation = rotation
 
     def add_morphology(self, swc_file, name="neuron", position=None, rotation=None, parent_tree_info=None,
-                       overwrite=False, morphology_data=None):
+                       overwrite=False, morphology_data=None, lazy_loading=False):
 
         """
             MorphologyData
 
             This can hold an entire neuron, or a part of a neuron.
 
             Args:
                 swc_file (str): Path to SWC file
                 name (str): Label of subtree, default "neuron" = main neuron tree
                 position (np.ndarray): x,y,z coordinates
                 rotation (np.ndarray): 3x3 rotation matrix
                 parent_tree_info (tuple, optional): Specify subtree attachment point
                                                     (MorphologyData, parent_label, parent_point_idx, arc_factor)
                 morphology_data (optional): MorphologyData object to use, then swc_file is None
+                lazy_loading (bool) : use lazy loading for morphology data
 
         """
 
         if not overwrite and name in self.morphology_data:
             raise KeyError(f"Error when loading {swc_file}, key {name} already exists in morphology_data")
 
         if morphology_data is None:
             # No cached morphology data, load it from file (slow)
             self.morphology_data[name] = MorphologyData(swc_file=swc_file, parent_tree_info=parent_tree_info,
-                                                        snudda_data=self.snudda_data)
+                                                        snudda_data=self.snudda_data, lazy_loading=lazy_loading)
             if position is not None:
-                self.morphology_data[name].place(position=position, rotation=rotation)
+                self.morphology_data[name].place(position=position, rotation=rotation, lazy=lazy_loading)
 
         else:
             # Use provided morphology data
             self.morphology_data[name] = morphology_data.clone(position=position, rotation=rotation)
 
     def section_iterator(self, section_type=None, subtree=None):
 
@@ -172,17 +173,14 @@
 
             parameter_key (str): Parameter Key for clone
             morphology_key (str): Morphology Key for clone
             modulation_key (str): Modulation Key for clone
 
         """
 
-        # np.set_printoptions(precision=2)
-        # print(f"rot {rotation.flatten()}, place pos {position}")
-
         new_neuron = NeuronMorphologyExtended(name=self.name,
                                               position=None,
                                               rotation=None,
                                               swc_filename=self.swc_filename,
                                               snudda_data=self.snudda_data,
                                               param_data=self.param_data,
                                               mech_filename=self.mech_filename,
@@ -209,21 +207,31 @@
         if parameter_key is not None:
             new_neuron.parameter_key = parameter_key
 
         if modulation_key is not None:
             new_neuron.modulation_key = modulation_key
 
         if morphology_key != self.morphology_key:
-            print("PROBLEM!!")
-            import pdb
-            pdb.set_trace()
             raise ValueError(f"Not allowed to change morphology_key when cloning: {self.morphology_key} -> {morphology_key}")
 
         new_neuron.load_morphology = self.load_morphology
 
+        new_neuron.max_axon_radius = self.max_axon_radius
+
+        if self.axon_density is not None:
+            new_neuron.axon_density = self.axon_density
+
+        new_neuron.voxel_size = self.voxel_size
+
+        if self.axon_density_type is not None:
+            new_neuron.axon_density_type = self.axon_density_type
+
+        if self.axon_density_bounds_xyz is not None:
+            new_neuron.axon_density_bounds_xyz = self.axon_density_bounds_xyz
+
         return new_neuron
 
     def get_section_coordinates(self, section_id, section_x):
 
         if section_id == -1:
             return self.position
 
@@ -349,16 +357,14 @@
                 plt.ion()
                 plt.show()
                 plt.draw()
                 plt.pause(0.001)
 
         return ax
 
-        # raise NotImplementedError("This function will move to separate plot class.")
-
     def get_weighted_synapse_density(self, synapse_density_str):
 
         """ Given synapse_density it returns expected number of synapses in all dendrite compartments """
         section_data = self.morphology_data["neuron"].section_data
         geometry_data = self.morphology_data["neuron"].geometry
 
         # We need to evaluate the synapse density at all dendrites and at soma (since we need all dendrite parents)
```

### Comparing `snudda-1.4.0/snudda/neurons/neuron_prototype.py` & `snudda-1.4.4/snudda/neurons/neuron_prototype.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/create_cube_mesh.py` & `snudda-1.4.4/snudda/place/create_cube_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/create_slice_mesh.py` & `snudda-1.4.4/snudda/place/create_slice_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/place.py` & `snudda-1.4.4/snudda/place/place.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
 from snudda.utils.snudda_path import get_snudda_data
 from snudda.neurons.neuron_prototype import NeuronPrototype
 from snudda.place.region_mesh import RegionMesh
 from snudda.place.rotation import SnuddaRotate
 from snudda.utils.snudda_path import snudda_parse_path, snudda_path_exists, snudda_simplify_path
 
+from snudda.neurons.morphology_data import MorphologyData
+
 ''' This code places all neurons in space, but does not setup their
     connectivity. That is done by detect.py and prune.py '''
 
 
 class SnuddaPlace(object):
     """ Places neurons in 3D space. Use detect to add connections, and prune to remove redundant connections. """
 
@@ -130,16 +132,14 @@
 
         # These are the dimensions of our space, dMin also needs a "padding"
         # region outside the space where fake neurons are placed. This is to
         # avoid boundary effects, without padding we would get too high density
         # at the edges
         self.volume = dict([])
 
-        # self.read_config()  # -- Now called from core.py
-
     def __del__(self):
 
         if self.rc:
             # Cleanup memory on workers
             from snudda.utils import cleanup
             cleanup(self.rc, "place")
 
@@ -286,15 +286,17 @@
             n.axon_density = axon_density
 
             if axon_info is not None and len(axon_info) > 0:
                 for axon_name, axon_position, axon_rotation, axon_swc in axon_info:
                     n.add_morphology(swc_file=axon_swc[idx],
                                      name=axon_name,
                                      position=axon_position[idx, :],
-                                     rotation=axon_rotation[idx, :].reshape((3, 3)))
+                                     rotation=axon_rotation[idx, :].reshape((3, 3)),
+                                     lazy_loading=True
+                                     )
 
             self.neurons.append(n)
 
             # This info is used by workers to speed things up
             if first_added:
                 first_added = False
                 self.neuron_prototypes[n.name] = n
@@ -572,57 +574,101 @@
 
             return axon_info
 
         else:
             # No extra axons for neuron
             return []
 
-    def get_projection_axon_location(self, source_position, proj_info, rng):
-
-        if "proj_file" in proj_info:
-            proj_data = json.load(proj_info["proj_file"])
-            source = np.array(proj_data["source"])*1e-6
-            destination = np.array(proj_data["destination"])*1e-6
-        else:
-            source = np.array(proj_info["source"])*1e-6
-            destination = np.array(proj_info["destination"])*1e-6
-
-        if "rotation_file" in proj_info:
-            rot_data = json.load(proj_info["rotation_file"])
-            rotation = np.array(rot_data["rotation"])
-            rot_position = np.array(rot_data["position"])*1e-6
-        elif "rotation" in proj_info:
-            rotation = np.array(proj_info["rotation"])
-            rot_position = np.array(proj_info["destination"])*1e-6
+    def get_projection_axon_location(self, source_position, proj_info, rng, patch_hull=True):
+        if 'projection' not in proj_info:
+            raise KeyError("No 'projection' entry in the projection config!")
+        
+        proj_cfg = proj_info["projection"]
+        if "file" in proj_cfg and \
+            ("source" in proj_cfg or \
+           "destination" in proj_cfg):
+           raise NotImplementedError("Projections should specify either a file or a mapping!")
+
+        elif "source" in proj_cfg \
+            and "destination" in proj_cfg:
+            source = np.array(proj_cfg["source"])*1e-6
+            destination = np.array(proj_cfg["destination"])*1e-6
+
+        elif "file" in proj_cfg :
+            with open(proj_cfg["file"], 'r') as f:
+                proj_file_data = json.load(f)
+            source = np.array(proj_file_data["source"])*1e-6
+            destination = np.array(proj_file_data["destination"])*1e-6
+            
+        else: 
+            raise NotImplementedError("Unknown projection configuration!")
+
+        # specify the rotations of the termination zones
+        rotation_cfg = proj_info.get("rotation", {})
+        if "rotation" in rotation_cfg:
+            rotation = np.array(rotation_cfg["rotation"])
+            rot_position = destination
+        
+        elif "file" in rotation_cfg:
+            with open(rotation_cfg["file"], 'r') as f:
+                rotation_data = json.load(f)
+            rotation = np.array(rotation_data["rotation"])
+            rot_position = np.array(rotation_data["position"])*1e-6
         else:
             rotation = None
             rot_position = None
 
-        # target_based_rotation = True  # -- TODO: restructure projection
-
-        # Obs we convert from micrometers to meters
         target_centres = griddata(points=source,
                                   values=destination,
-                                  xi=source_position, method="linear")
+                                  xi=source_position,
+                                  method="linear")
+
+        # this checks if there are values outside of the convex hull
+        to_patch = np.where(np.isnan(np.sum(target_centres, axis=1)))[0]
+
+        # and patch missing entries
+        if patch_hull and len(to_patch)>0:
+            self.write_log(f"Patched {len(to_patch)}/{len(target_centres)}")
+            target_centres_patched = griddata(points=source,
+                                              values=destination,
+                                              xi=source_position,
+                                              method="nearest")
+            target_centres[to_patch] = target_centres_patched[to_patch]
+
+        # which coordinates to use for selecting rotation
+        mapping = rotation_cfg.get('mapping', 'target')
+        if mapping == "target":
+            xi = target_centres
+        elif mapping == "source":
+            xi = source_position
+        else:
+            raise NotImplentedError(f"Unknown mapping '{mapping}'!")
 
         if rotation is not None:
-            # TODO: This is probably wrong, we have to handle interpolation between
-            #       rotation matrices in a better way! -- use angles? -- use target_centres, vs
             target_rotation = griddata(points=rot_position,
                                        values=rotation,
-                                       xi=target_centres, method="linear")
+                                       xi=xi, method="linear")
+            # if the rotation is specified as a field of rotation vectors, 
+            # then these need to be converted to matrices.
+            if target_rotation[0].shape == (3,):
+                rotation_matrices = \
+                [SnuddaRotate.rotation_matrix_from_vectors(np.array([0, 0, 1]), rv).flatten()\
+                 for rv in target_rotation] 
+                target_rotation = np.array(rotation_matrices)
+                
         else:
             target_rotation = [None for x in range(source_position.shape[0])]
 
-        num_axons = len(proj_info["axonMorphology"])
+        num_axons = len(proj_info["morphologies"])
         axon_id = rng.choice(num_axons, source_position.shape[0])
-        axon_swc = [proj_info["axonMorphology"][x] for x in axon_id]
+        axon_swc = [proj_info["morphologies"][x] for x in axon_id]
 
         return target_centres, target_rotation, axon_swc
 
+
     ############################################################################
 
     def all_neuron_positions(self):
 
         """ Returns all neuron positions as a n x 3 matrix. """
 
         n_neurons = len(self.neurons)
@@ -681,15 +727,15 @@
 
         return ax_neuron, ax_name, ax_position, ax_rotation, ax_swc
 
     ############################################################################
 
     def write_data(self, file_name=None):
 
-        """ Writes positition data to HDF5 file file_name. """
+        """ Writes position data to HDF5 file file_name. """
 
         if not file_name:
             file_name = self.position_file
 
         assert len(self.neurons) > 0, "No neurons to save!"
 
         self.write_log(f"Writing data to HDF5 file: {file_name}")
@@ -775,43 +821,14 @@
         axon_group.create_dataset("position", data=ax_position)
         axon_group.create_dataset("rotation", data=ax_rotation)
         axon_group.create_dataset("morphology", (len(ax_swc), ), data=ax_swc,
                                   dtype=h5py.special_dtype(vlen=bytes), compression="gzip")
 
         # TODO: Parent tree info, eller motsvarande, måste sparas också!
 
-        # Should not be used anymore, try removing...
-        #
-        # neuron_dend_radius = neuron_group.create_dataset("maxDendRadius",
-        #                                                  (len(self.neurons),),
-        #                                                  "float",
-        #                                                  compression="gzip")
-        #
-        # neuron_axon_radius = neuron_group.create_dataset("maxAxonRadius",
-        #                                                  (len(self.neurons),),
-        #                                                  "float",
-        #                                                  compression="gzip")
-
-        # Obsolete, we now use morphology_key, parameter_key and modulation_key exclusively
-        #
-        # neuron_param_id = neuron_group.create_dataset("parameterID",
-        #                                               (len(self.neurons),),
-        #                                               "int",
-        #                                               compression="gzip")
-        #
-        # neuron_morph_id = neuron_group.create_dataset("morphologyID",
-        #                                               (len(self.neurons),),
-        #                                               "int",
-        #                                               compression="gzip")
-
-        # neuron_modulation_id = neuron_group.create_dataset("modulationID",
-        #                                                    (len(self.neurons),),
-        #                                                    "int",
-        #                                                    compression="gzip")
-
         pk_list = [n.parameter_key.encode("ascii", "ignore")
                    if n.parameter_key is not None else ""
                    for n in self.neurons]
         pk_str_type = 'S' + str(max(1, max([len(x) for x in pk_list])))
 
         mk_list = [n.morphology_key.encode("ascii", "ignore")
                    if n.morphology_key is not None else ""
```

### Comparing `snudda-1.4.0/snudda/place/projection_map_finder.py` & `snudda-1.4.4/snudda/place/projection_map_finder.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/region_mesh.py` & `snudda-1.4.4/snudda/place/region_mesh.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/rotation.py` & `snudda-1.4.4/snudda/place/rotation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/place/volumetric_mapping.py` & `snudda-1.4.4/snudda/place/volumetric_mapping.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/io_mesh_swc/__init__.py` & `snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/__init__.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py` & `snudda-1.4.4/snudda/plotting/Blender/io_mesh_swc/operator_swc_import.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomas.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasRender.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/drawHyperCubeSomasWithLTS.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/makeNeuronCube.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCube.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/makeNeuronCubeSubset.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseCubeOfNeuronsWhiteBackground.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualiseStriatumNeuronsWithSynapses.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_network.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_network_old.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_network_old.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/Blender/visualisation/visualise_touch_detection.py` & `snudda-1.4.4/snudda/plotting/Blender/visualisation/visualise_touch_detection.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plotLTSdensity.py` & `snudda-1.4.4/snudda/plotting/plotLTSdensity.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_cross_correlogram.py` & `snudda-1.4.4/snudda/plotting/plot_cross_correlogram.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_degeneration.py` & `snudda-1.4.4/snudda/plotting/plot_degeneration.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,38 @@
         self.original_plot = SnuddaPlotInputLocations(network_path=original_network_path)
         self.degenerated_plot = SnuddaPlotInputLocations(network_path=degenerated_network_path)
 
         self.fig_path = os.path.join(degenerated_network_path, "figures")
         if not os.path.exists(self.fig_path):
             os.mkdir(self.fig_path)
 
-    def plot_neuron(self, neuron_id, figure_size=None, show_internal_synapses=True):
+    def plot_neuron(self, neuron_id, figure_size=None, show_internal_synapses=True, hide_axis=False):
         import matplotlib.pyplot as plt
         fig = plt.figure(figsize=figure_size)
         ax = fig.add_subplot(111, projection='3d')
         ax = self.original_plot.plot_neuron_inputs(neuron_id=neuron_id,
                                                    neuron_colour=np.array([0.6, 0.6, 0.6]),
                                                    external_colour=np.array([1, 0.5, 0]),
                                                    internal_colour=np.array([0, 0.5, 1]),
                                                    show_internal_synapses=show_internal_synapses,
                                                    ax=ax,
                                                    size=2,
-                                                   save_fig=False, show_figure=False, figure_size=figure_size)
+                                                   save_fig=False,
+                                                   show_figure=False,
+                                                   hide_axis=hide_axis,
+                                                   figure_size=figure_size)
 
         ax = self.degenerated_plot.plot_neuron_inputs(neuron_id=neuron_id,
-                                                 neuron_colour=np.array([0, 0, 0]),
-                                                 show_internal_synapses=show_internal_synapses,
-                                                 ax=ax,
-                                                 size=50,
-                                                 save_fig=True, show_figure=True)
+                                                      neuron_colour=np.array([0, 0, 0]),
+                                                      show_internal_synapses=show_internal_synapses,
+                                                      ax=ax,
+                                                      size=50,
+                                                      save_fig=True,
+                                                      hide_axis=hide_axis,
+                                                      show_figure=True)
 
 
 def cli():
 
     import argparse
     parser = argparse.ArgumentParser("plot_degeneration")
     parser.add_argument("original_network_path", help="Path to original network directory")
```

### Comparing `snudda-1.4.0/snudda/plotting/plot_degeneration_and_growth.py` & `snudda-1.4.4/snudda/plotting/plot_degeneration_and_growth.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_density.py` & `snudda-1.4.4/snudda/plotting/plot_density.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_density_slice.py` & `snudda-1.4.4/snudda/plotting/plot_density_slice.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_distance_statistics.py` & `snudda-1.4.4/snudda/plotting/plot_distance_statistics.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_input.py` & `snudda-1.4.4/snudda/plotting/plot_input.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_input_locations.py` & `snudda-1.4.4/snudda/plotting/plot_input_locations.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,16 @@
                            show_internal_synapses=True,
                            external_colour=None, internal_colour=None,
                            ax=None, neuron_colour=None,
                            size=10,
                            save_fig=True,
                            dpi=300,
                            show_figure=True,
+                           hide_axis=False,
+                           hide_grid=True,
                            figure_size=None):
 
         coords = self.get_input_coords(neuron_id=neuron_id, input_type=input_type)
 
         if external_colour is None:
             external_colour = "r"
 
@@ -115,14 +117,32 @@
             plt.title(f"Input to {neuron_name} ({neuron_id})")
             f_name = f"input-to-{neuron_id}-{neuron_name}{syn_txt}.png"
 
         fig_path = os.path.join(self.network_path, "figures")
         if not os.path.exists(fig_path):
             os.mkdir(fig_path)
 
+        if hide_grid:
+            ax.grid(None)
+
+        if hide_axis:
+            ax.set_axis_off()
+
+        x_labels = [f"{x*1e6:.0f}" for x in ax.get_xticks()]
+        y_labels = [f"{y*1e6:.0f}" for y in ax.get_yticks()]
+        z_labels = [f"{z*1e6:.0f}" for z in ax.get_zticks()]
+
+        ax.set_xticklabels(x_labels)
+        ax.set_yticklabels(y_labels)
+        ax.set_zticklabels(z_labels)
+
+        ax.set_xlabel("μm", fontsize=20)
+        ax.set_ylabel("μm", fontsize=20)
+        ax.set_zlabel("μm", fontsize=20)
+
         if save_fig:
             fig_name = os.path.join(fig_path, f_name)
             plt.savefig(fig_name, dpi=dpi)
             print(f"Figure written: {fig_name}")
 
         if show_figure:
             fig = ax.get_figure()
@@ -179,20 +199,20 @@
 
         max_dist = 0
 
         for nid in neuron_id:
 
             swc_file = snudda_parse_path(self.snudda_load.data["neurons"][nid]["morphology"], self.snudda_data)
             morph = NeuronMorphologyExtended(swc_filename=swc_file)
-            dist_to_soma = morph.dend[:, 4]
+            dist_to_soma = morph.morphology_data["neuron"].geometry[:, 4]
             max_dist = max(np.max(dist_to_soma), max_dist)
 
         return max_dist
 
-    def plot_input_location(self, neuron_type, input_name, n_bins=20):
+    def plot_input_location(self, neuron_type, input_name, n_bins=15):
 
         import numexpr
 
         distance_to_soma = self.get_input_soma_distance_summary(neuron_type=neuron_type, input_name=input_name)
         max_dist = self.get_max_dendrite_distance(neuron_type=neuron_type) + 1e-6
 
         dendrite_density = self.dendrite_density_for_type(neuron_type=neuron_type, max_dist=max_dist, num_bins=n_bins)
@@ -202,17 +222,18 @@
         # divide by bin_width (scaled to micrometers) and divide by dendrite_density
         norm_count = count/np.sum(count)/(max_dist*1e6/n_bins)
 
         fig = plt.figure()
         plt.stairs(norm_count, edges * 1e6, color="black")
 
         plt.xlabel("Distance ($\mu$m)")
-        plt.ylabel("Density")
+        plt.ylabel("Normalised total density")
 
-        if "synapseDensity" in self.input_config[neuron_type][input_name]:
+        if neuron_type in self.input_config and input_name in self.input_config[neuron_type] \
+                and "synapseDensity" in self.input_config[neuron_type][input_name]:
 
             synapse_density = self.input_config[neuron_type][input_name]["synapseDensity"]
             d = np.linspace(0, max_dist, n_bins)
 
             synapse_density = numexpr.evaluate(synapse_density)
             density = np.multiply(synapse_density, dendrite_density)
             norm_density = density / np.sum(density) / (1e6 * (d[1] - d[0]))
@@ -246,26 +267,28 @@
 
         bin_width = max_dist / num_bins
 
         dend_hist = np.zeros((num_bins,))
         morph = NeuronMorphologyExtended(swc_filename=swc_file)
 
         for sec in morph.section_iterator(section_type=3):
-            pos = sec.position
-
-            seg_len = np.linalg.norm(np.diff(sec.position, axis=1), axis=0)
-
-            # 0,1,2: x,y,z  3: radie, 4: dist to soma
-            soma_dist = sec.morphology_data.geometry[sec.point_idx, 4]
+            seg_len = np.linalg.norm(np.diff(sec.position, axis=0), axis=1)
+            soma_dist = sec.soma_distance
 
             for start_dist, end_dist, comp_length in zip(soma_dist[0:-1], soma_dist[1:], seg_len):
                 bin_a = int(start_dist/bin_width)
                 bin_b = int(end_dist/bin_width)
 
-                assert comp_length < bin_width, f"Compartment length {comp_length} > bin width {bin_width}"
+                if comp_length > bin_width:
+                    print("Tell me why")
+                    import pdb
+                    pdb.set_trace()
+
+                assert comp_length < bin_width, f"Compartment length {comp_length} > bin width {bin_width} " \
+                                                f"(try using fewer bins)"
                 assert bin_a <= bin_b, f"Internal error, assume first element in link closer to soma"
 
                 if bin_a == bin_b:
                     dend_hist[bin_a] += comp_length
                 else:
                     frac_a = bin_width - (start_dist % bin_width)
                     frac_b = (end_dist % bin_width)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `snudda-1.4.0/snudda/plotting/plot_network.py` & `snudda-1.4.4/snudda/plotting/plot_network.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_network_simulation.py` & `snudda-1.4.4/snudda/plotting/plot_network_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_node_benchmark.py` & `snudda-1.4.4/snudda/plotting/plot_node_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_period_experiment.py` & `snudda-1.4.4/snudda/plotting/plot_period_experiment.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_size_benchmark.py` & `snudda-1.4.4/snudda/plotting/plot_size_benchmark.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_spike_raster_v2.py` & `snudda-1.4.4/snudda/plotting/plot_spike_raster_v2.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/plotting/plot_traces.py` & `snudda-1.4.4/snudda/plotting/plot_traces.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/model_current_injections.py` & `snudda-1.4.4/snudda/simulate/model_current_injections.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/network_pair_pulse_simulation.py` & `snudda-1.4.4/snudda/simulate/network_pair_pulse_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/nrn_simulator_parallel.py` & `snudda-1.4.4/snudda/simulate/nrn_simulator_parallel.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/pair_recording.py` & `snudda-1.4.4/snudda/simulate/pair_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/save_network_recording.py` & `snudda-1.4.4/snudda/simulate/save_network_recording.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/simulate/simulate.py` & `snudda-1.4.4/snudda/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/ablate_network.py` & `snudda-1.4.4/snudda/utils/ablate_network.py`

 * *Files identical despite different names*

```diff
@@ -408,14 +408,15 @@
                                             compression=data.compression)
             except:
                 import traceback
                 print(traceback.format_exc())
                 import pdb
                 pdb.set_trace()
 
+
 def snudda_ablate_network_cli():
     from argparse import ArgumentParser
 
     # TODO: Fix so ablation can be specified using a json file for more complex ablations
 
     parser = ArgumentParser(description="Modify connections in network.")
     parser.add_argument("original_network", type=str, help="Input network hdf5 file")
```

### Comparing `snudda-1.4.0/snudda/utils/benchmark_logging.py` & `snudda-1.4.4/snudda/utils/benchmark_logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     time.sleep(2)
     bl.stop_timer("test2")
     bl.stop_timer("test")
     bl.write_log()
 
     """
 
-    def __init__(self, network_path, parallel_flag=False, log_file=None, running_neuron=False):
+    def __init__(self, network_path, parallel_flag=False, log_file=None, running_neuron=False,
+                 ipython_profile=None):
 
         """
         Constructor.
 
         Args:
             network_path (str): Path to network
             parallel_flag (bool): Running in parallel, should we determine number of workers?
@@ -41,19 +42,20 @@
         self.network_name = self.get_network_name(network_path)
 
         self.start_time = dict()
         self.end_time = dict()
         self.pc = None  # Used if running neuron
 
         if parallel_flag or running_neuron:
-            self.num_workers = self.get_number_of_workers(running_neuron=running_neuron)
+            self.num_workers = self.get_number_of_workers(running_neuron=running_neuron,
+                                                          ipython_profile=ipython_profile)
         else:
             self.num_workers = 1
 
-    def get_number_of_workers(self, running_neuron):
+    def get_number_of_workers(self, running_neuron, ipython_profile=None):
 
         """
         Returns number of workers.
 
         Args:
             running_neuron (bool) : Are we running NEURON? Used when determining number of workers).
 
@@ -64,28 +66,38 @@
             from mpi4py import MPI   # Import mpi before NEURON for parallel
             from neuron import h
             self.pc = h.ParallelContext()
             return self.pc.nhost()
 
             # Is there a simpler way to get the number of workers?
 
-        ipython_profile = os.getenv('IPYTHON_PROFILE')
+        if ipython_profile is None:
+            ipython_profile = os.getenv('IPYTHON_PROFILE')
+
         if not ipython_profile:
             ipython_profile = "default"
 
         ipython_dir = os.getenv('IPYTHONDIR')
         if not ipython_dir:
             ipython_dir = os.path.join(os.path.abspath(os.getcwd()), ".ipython")
 
         import ipyparallel
         u_file = os.path.join(ipython_dir, f"profile_{ipython_profile}", "security", "ipcontroller-client.json")
-        rc = ipyparallel.Client(url_file=u_file, timeout=120, debug=False)
-        d_view = rc.direct_view(targets='all')  # rc[:] # Direct view into clients
 
-        return len(d_view) + 1  # We also include the master node
+        if os.path.isfile(u_file):
+            print(f"Benchmark reading ipyparallel config file: {u_file}")
+            try:
+                rc = ipyparallel.Client(url_file=u_file, profile=ipython_profile, timeout=120, debug=False)
+                d_view = rc.direct_view(targets='all')  # rc[:] # Direct view into clients
+
+                return len(d_view) + 1  # We also include the master node
+            except:
+                return -1
+        else:
+            return 1
 
     @staticmethod
     def get_network_name(network_path):
 
         """ Returns network name based on network_path. """
 
         if os.path.basename(network_path):
```

### Comparing `snudda-1.4.0/snudda/utils/cleanup.py` & `snudda-1.4.4/snudda/utils/cleanup.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/clone_neurons.py` & `snudda-1.4.4/snudda/utils/clone_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/conv_hurt.py` & `snudda-1.4.4/snudda/utils/conv_hurt.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,73 +9,68 @@
 import numpy as np
 
 
 # TODO: This needs to be updated to match the latest SONATA release.
 
 class ConvHurt(object):
 
-    def __init__(self, simulation_structure, input_structures, base_dir="TEST/"):
+    def __init__(self, simulation_structures, base_dir="TEST/", target_simulator="NEST"):
 
         self.base_dir = base_dir
         self.network_dir = os.path.join(base_dir, 'networks')
+        self.target_simulator = target_simulator
 
         self.h5py_libver = "earliest"  # "latest"
 
-        self.setup_directories(simulation_structure=simulation_structure,
-                               input_structures=input_structures, base_dir=base_dir)
+        self.setup_directories(base_dir=base_dir)
 
-        self.write_main_config(simulation_structure=simulation_structure,
-                               input_structures=input_structures,
-                               base_dir=base_dir)
+        self.write_main_config(simulation_structures=simulation_structures,
+                               base_dir=base_dir, target_simulator=target_simulator)
 
     ############################################################################
 
     @staticmethod
     def create_dir(directory):
 
         if not os.path.exists(directory):
             print(f"Creating directory : {directory}")
             os.makedirs(directory)
 
     ############################################################################
 
     def setup_directories(self,
-                          simulation_structure,
-                          input_structures,
                           base_dir=None):
 
         if base_dir is None:
             base_dir = "."
 
         self.create_dir(base_dir)
 
-        dir_list = ['components', 'components/biophysical_neuron_dynamics', 'components/hoc_templates',
-                    'components/mechanisms', 'components/morphologies', 'components/point_neuron_dynamics',
-                    'components/synapse_dynamics', 'networks', 'inputs', 'output', f"networks/{simulation_structure}"]
-
-        for x in input_structures:
-            dir_list.append(f"networks/{x}")
+        dir_list = ['components',
+                    os.path.join("components", "biophysical_neuron_dynamics"),
+                    os.path.join("components", "hoc_templates"),
+                    os.path.join("components", "mechanisms"),
+                    os.path.join("components", "morphologies"),
+                    os.path.join("components", "point_neuron_dynamics"),
+                    os.path.join("components", "synapse_dynamics"),
+                    'networks', 'inputs', 'output']
 
         for x in dir_list:
-            self.create_dir(f"{base_dir}{x}")
+            self.create_dir(os.path.join(base_dir, x))
 
     ############################################################################
     #
     # Writing the main configuration file, linking everything together
 
     def write_main_config(self,
                           base_dir="TEST/",
                           out_file="circuit_config.json",
-                          simulation_structure="striatum",
-                          input_structures=None,
+                          simulation_structures=[],
                           target_simulator="NEURON"):
 
-        if input_structures is None:
-            input_structures = ["thalamus", "cortex"]
-
         config = OrderedDict([])
 
         config["target_simulator"] = target_simulator
 
         manifest = OrderedDict([("$BASE_DIR", "."),
                                 ("$NETWORK_DIR", "$BASE_DIR/networks"),
                                 ("$COMPONENT_DIR", "$BASE_DIR/components")])
@@ -91,48 +86,38 @@
                                   ("biophysical_neuron_models_dir",
                                    os.path.join("$COMPONENT_DIR", "biophysical_neuron_dynamics")),
                                   ("point_neuron_models_dir", os.path.join("$COMPONENT_DIR", "point_neuron_dynamics")),
                                   ("templates_dir", os.path.join("$COMPONENT_DIR", "hoc_templates"))])
 
         config["components"] = components
 
-        sim_node = os.path.join("$NETWORK_DIR", simulation_structure, f"{simulation_structure}_nodes.hdf5")
-        sim_node_type = os.path.join("$NETWORK_DIR", simulation_structure, f"{simulation_structure}_node_types.csv")
-
-        sim_edge = os.path.join("$NETWORK_DIR", simulation_structure, f"{simulation_structure}_edges.hdf5")
-        sim_edge_type = os.path.join("$NETWORK_DIR", simulation_structure, f"{simulation_structure}_edge_types.csv")
-
-        # We create a list where first element contains the simulated node,
-        # subsequent elements are the inputs (can be more than one)
-
-        node_files = [OrderedDict([("nodes_file", sim_node),
-                                   ("node_types_file", sim_node_type)])]
-        node_files += [OrderedDict([("nodes_file", os.path.join("$NETWORK_DIR", x, f"{x}_nodes.hdf5")),
-                                    ("node_types_file", os.path.join("$NETWORK_DIR", x, f"{x}_node_types.csv"))])
-                       for x in input_structures]
-
-        edge_files = [OrderedDict([("edges_file", sim_edge), ("edge_types_file", sim_edge_type)])]
-        edge_files += [OrderedDict([("edges_file", os.path.join("$NETWORK_DIR", x, f"{x}_edges.hdf5")),
-                                    ("edge_types_file", os.path.join("$NETWORK_DIR", x, f"{x}_edge_types.csv"))])
-                       for x in input_structures]
+        nodes = []
+        edges = []
+        for ss in simulation_structures:
+            node_info = {"nodes_file": os.path.join("$NETWORK_DIR", f"{ss}_nodes.hdf5"),
+                         "node_types_file": os.path.join("$NETWORK_DIR", f"{ss}_node_types.csv") }
+            nodes.append(node_info)
+
+            edge_info = {"edges_file": os.path.join("$NETWORK_DIR", f"{ss}_edges.hdf5"),
+                         "edge_types_file": os.path.join("$NETWORK_DIR", f"{ss}_edge_types.csv") }
+            edges.append(edge_info)
 
-        config["networks"] = OrderedDict([("nodes", node_files),
-                                          ("edges", edge_files)])
+        config["networks"] = OrderedDict([("nodes", nodes), ("edges", edges)])
 
         with open(os.path.join(base_dir, out_file), 'wt') as f:
             json.dump(config, f, indent=4)
 
     ############################################################################
 
     # nodeID - vector with IDs for all neurons
     # nodeTypeID - vector with Type ID for each neuron
-    # nodeGroupID - vector with group memebership for each neuron
+    # nodeGroupID - vector with group membership for each neuron
     # nodeGroupIndex - vector with index of each neuron within the given group
 
-    # data = dictionary with "position", "rotaton_angle_zaxis", ...
+    # data = dictionary with "position", "rotation_angle_zaxis", ...
     #        etc that should be stored
     #        names should match what is in the group data
     def write_nodes(self,
                     node_file,
                     population_name,
                     node_id,
                     node_type_id,
@@ -140,14 +125,16 @@
                     node_group_index,
                     data,
                     model_type=None,
                     model_template=None):
 
         with h5py.File(os.path.join(self.network_dir, node_file), 'w', libver=self.h5py_libver) as f:
 
+            self.add_version(f)
+
             n_group = f.create_group("nodes")
 
             nodes_group = n_group.create_group(population_name)
 
             nodes_group.create_dataset("node_id", data=node_id)
             nodes_group.create_dataset("node_type_id", data=node_type_id)
             nodes_group.create_dataset("node_group_id", data=node_group_id)
@@ -225,88 +212,62 @@
 
                 csv_writer.writerow(row)
 
     ############################################################################
 
     # !!! WHAT HAPPENS IF WE CANT KEEP EVERYTHING IN MEMORY
 
-    def write_edges(self, edge_file,
-                    edge_population_name,
-                    edge_group,
-                    edge_group_index,
+    def write_edges(self,
+                    edge_file,
+                    population_rows,
                     edge_type_id,
                     source_id,
                     target_id,
-                    data,
-                    source_population_name=None,
-                    target_population_name=None, ):
-
-        if source_population_name is None:
-            source_population_name = edge_population_name
-            print(f"No source population name given, using edge_population_name: {edge_population_name}")
-
-        if target_population_name is None:
-            target_population_name = edge_population_name
-            print(f"No source population name given, using edgePopulationName: {edge_population_name}")
+                    data):
 
-            # We need to have the targetID vector sorted
+        # We need to have the targetID vector sorted
         # How should we handle cells that do not have any edges at all?
         sort_idx = np.argsort(target_id)
 
-        # This finds the positions where the sorter targetID increases
-        all_diffs = np.diff(target_id[sort_idx])
-        diff_idx = np.where(all_diffs > 0)[0]
-        index_pointer = np.zeros(len(diff_idx) + 1)
-        index_pointer[1:] = diff_idx + 1
-
-        # import pdb
-        # pdb.set_trace()
-
-        # We assume all neurons has at least one synapse, the diff should
-        # never jump by two
-        if not (all_diffs < 2).all():
-            print("!!! Not all neurons have synapses!")
-
-        # EVERYTHING we write needs to use sortIdx so it is in the right order
+        # EVERYTHING we write needs to use sort_idx (idx) so it is in the right order
         with h5py.File(os.path.join(self.network_dir, edge_file), 'w', libver=self.h5py_libver) as f:
+            self.add_version(f)
+
             edg_group = f.create_group("edges")
-            e_group = edg_group.create_group(edge_population_name)
 
-            e_group.create_dataset("edge_group", data=edge_group[sort_idx])
-            e_group.create_dataset("edge_group_index", data=edge_group_index[sort_idx])
-            e_group.create_dataset("edge_type_id", data=edge_type_id[sort_idx])
-            e_group.create_dataset("index_pointer", data=index_pointer)
-            e_group.create_dataset("source_node_id", data=source_id[sort_idx])
-            e_group.create_dataset("target_node_id", data=target_id[sort_idx])
-
-            e_group["source_node_id"].attrs["node_population"] = source_population_name
-            e_group["target_node_id"].attrs["node_population"] = target_population_name
-            groups = np.unique(edge_group)
+            for pop_name, pop_rows in population_rows.items():
+                source_population_name, target_population_name = pop_name.split("_")
+                n_rows = len(pop_rows)
 
-            for g in groups:
-                idx = np.where(edge_group[sort_idx] == g)
+                e_group = edg_group.create_group(pop_name)
+
+                idx = sort_idx[pop_rows]
+
+                e_group.create_dataset("edge_group_id", data=np.zeros((n_rows,), dtype=int))
+                e_group.create_dataset("edge_group_index", data=np.arange(n_rows), dtype=int)
+                e_group.create_dataset("edge_type_id", data=edge_type_id[idx])
+                e_group.create_dataset("source_node_id", data=source_id[idx])
+                e_group.create_dataset("target_node_id", data=target_id[idx])
 
-                group_group = e_group.create_group(str(g))
+                e_group["source_node_id"].attrs["node_population"] = source_population_name
+                e_group["target_node_id"].attrs["node_population"] = target_population_name
+
+                group_group = e_group.create_group("0")
 
                 for data_type in data.keys():
                     if len(data[data_type].shape) == 1:
-                        group_group.create_dataset(data_type,
-                                                   data=data[data_type][sort_idx][idx])
+                        group_group.create_dataset(data_type, data=data[data_type][idx])
                     elif len(data[data_type].shape) == 2:
-                        group_group.create_dataset(data_type,
-                                                   data=data[data_type][sort_idx, :][idx, :])
+                        group_group.create_dataset(data_type, data=data[data_type][idx, :])
                     else:
                         print("Unsupported width of data column.")
 
-            # We need to create the indices needed by Allen Institute
-            self.create_index(e_group["source_node_id"], e_group, index_source=True)
-            self.create_index(e_group["target_node_id"], e_group, index_source=False)
-            # inGroup = eGroup.create_group("indices")
-            # inGroup.create_group("source_to_target")
-            # inGroup.create_group("target_to_source")
+                # We need to create the indices needed by Allen Institute
+                self.create_index(e_group["source_node_id"], e_group, index_source=True)
+                self.create_index(e_group["target_node_id"], e_group, index_source=False)
 
     ############################################################################
 
     # createIndex provided by Kael Dai from Allen Institute, 2018-11-27
 
     def create_index(self, node_ids_ds, output_grp, index_source=0):
 
@@ -337,17 +298,19 @@
         for node_index, trg_ranges in enumerate(ranges_list):
             if len(trg_ranges) > 0:
                 node_id_to_range[node_index, 0] = range_index
                 for r in trg_ranges:
                     range_to_edge_id[range_index, :] = r
                     range_index += 1
                 node_id_to_range[node_index, 1] = range_index
+            else:
+                node_id_to_range[node_index, :] = -1
 
         output_grp.create_dataset('range_to_edge_id', data=range_to_edge_id, dtype='uint64')
-        output_grp.create_dataset('node_id_to_ranges', data=node_id_to_range, dtype='uint64')
+        output_grp.create_dataset('node_id_to_range', data=node_id_to_range, dtype='uint64')
 
     ############################################################################
 
     def write_edges_csv(self,
                         edge_csv_file,
                         edge_type_id,
                         data):
@@ -388,14 +351,16 @@
             print(f"No spikes specified, not writing {spike_file_name}")
             print("Use python3 Network_input.py yourinput.json yournetwork.hdf5 input-spikes.hdf5")
             return
 
         f_name = os.path.join(self.base_dir, spike_file_name)
 
         with h5py.File(f_name, 'w', libver=self.h5py_libver) as f:
+            self.add_version(f)
+
             print(f"Writing file {f_name}")
 
             s_group = f.create_group("spikes")
             s_group.create_dataset("gids", data=spikes[:, 1])
             s_group.create_dataset("timestamps", data=spikes[:, 0])
 
     ############################################################################
@@ -416,14 +381,19 @@
             f.write("/scatter")
 
             for time, gid in spikes:
                 f.write(f"{time} {gid}")
 
     ############################################################################
 
+    def add_version(self, hdf5_file):
+
+        hdf5_file.attrs["version"] = [0, 1]
+        hdf5_file.attrs["magic"] = 0x0A7A
+
 
 if __name__ == "__main__":
     # ch = ConvHurt()
     # ch = ConvHurt(simulationStructure="cerebellum",
     #              inputStructures=["pons","cortex"])
 
     ch = ConvHurt(simulation_structure="striatum",
@@ -454,15 +424,15 @@
 
     edge_group = np.array([5, 5, 11, 11, 11])
     edge_group_index = np.array([0, 1, 0, 1, 2])
     edge_type_id = np.array([0, 1, 0, 1, 0])
     source_gid = np.array([1, 2, 3, 3, 4])
     target_gid = np.array([2, 3, 4, 0, 1])  # THESE ARE SORTED ... HAHAHA
 
-    # Delay should be in ms (bad bad people, real scientists use SI units)
+    # Delay needs to be in ms (bad bad people, real scientists use SI units)
     edge_data = OrderedDict([("sec_id", np.array([10, 22, 33, 24, 15])),
                              ("sec_x", np.array([0.1, 0.3, 0.5, 0.2, 0])),
                              ("syn_weight", np.array([0.1e-9, 2e-9, 3e-9,
                                                       0.3e-9, 0.1e-9])),
                              ("delay", 1e3 * np.array([1e-3, 4e-3, 2e-3, 5e-3, 1e-3]))])
 
     ch.write_edges(edge_file="striatum_edges.hdf5",
```

### Comparing `snudda-1.4.0/snudda/utils/create_parameter_morphology_input_map.py` & `snudda-1.4.4/snudda/utils/create_parameter_morphology_input_map.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/cut.py` & `snudda-1.4.4/snudda/utils/cut.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                  out_file_name=None,
                  plot_only=False, show_plot=True):
 
         """ Constructor.
 
         Args:
             network_file (str): Path to network file
-            cut_equation (str): Cut equation, e.g. "z>0"
+            cut_equation (str): Cut equation, e.g. "z>0" the neurons fullfilling equation are kept
             out_file_name (str): Path to new network file
             plot_only (bool): Only create a plot of cut
             show_plot (bool): Show plot on screen
         """
 
         self.cut_equation = cut_equation
         self.h5libver = "latest"
@@ -122,18 +122,26 @@
         #       then does cut / ablation, and then verifies that those cells are still connected the same way, if left
         #       + extra unit test, som kollar att inga nya variabler lagts till i load, då vill vi få en krasch
         #       och varning
 
         network_group = self.out_file.create_group("network")
         neuron_group = network_group.create_group("neurons")
 
+        if len(self.in_file["network/neurons/extraAxons/parentNeuron"][()]) > 0:
+            # To implement this we need to only keep the axons that have parent neurons that are still there
+            raise NotImplemented("extraAxons currently not supported by cut.py")
+
         for var_name in self.in_file["network/neurons"]:
 
             data = self.in_file[f"network/neurons/{var_name}"]
 
+            if type(data) == h5py._hl.group.Group:
+                self.in_file.copy(f"network/neurons/{var_name}", neuron_group)
+                continue
+
             if len(data.shape) == 0:
                 # Scalar data, just copy
                 self.in_file.copy(f"network/neurons/{var_name}", neuron_group)
                 continue
 
             elif len(data.shape) == 1:
                 # 1D data, we only keep nSomaKeep of them
```

### Comparing `snudda-1.4.0/snudda/utils/export_connection_matrix.py` & `snudda-1.4.4/snudda/utils/export_connection_matrix.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/export_sonata.py` & `snudda-1.4.4/snudda/utils/export_sonata.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,266 +5,174 @@
 # - Check what axon and dendrite propagation speeds should be
 #
 
 import json
 import os
 import sys
 from collections import OrderedDict
+from shutil import copyfile
+from glob import glob
 
 import h5py
 import numpy as np
 
-from conv_hurt import ConvHurt
-from load import SnuddaLoad
+from snudda.utils import snudda_parse_path
+from snudda.utils.conv_hurt import ConvHurt
+from snudda import SnuddaLoad
 
 
-class ExportSonata(object):
+class ExportSonata:
 
-    def __init__(self, network_file, input_file, out_dir):
+    def __init__(self, network_file, input_file, out_dir, debug_flag=True, target_simulator="NEST"):
 
-        # !!! If inputFile is last, we need to handle that appropriately
-        # and find the corresponding input file
-
-        self.debug = False
+        self.debug = debug_flag
 
         self.out_dir = out_dir
+        self.target_simulator = target_simulator
 
         # Read the data
-        nl = SnuddaLoad(network_file)
-        self.network_file = nl.network_file  # If file was "last", this sets right one
+        self.snudda_load = SnuddaLoad(network_file)
+        self.network_file = self.snudda_load.network_file
+        self.input_file = input_file
 
-        if input_file == "last":
-            self.input_file = os.path.join("save", f"input-spikes-{nl.data['SlurmID']}.hdf5")
-        else:
-            self.input_file = input_file
+        self.network_config = json.loads(self.snudda_load.data["config"])
 
         print(f"Using input file: {self.input_file}")
 
         # This contains data for converting to Neurodamus secID and secX
         self.morph_cache = dict([])
 
+        self.morph_location_lookup = dict([])
+        self.hoc_location_lookup = dict([])
+
         # Write the data in new format using the ConvHurt module
-        ch = ConvHurt(simulation_structure="Striatum",
-                      input_structures=["Cortex", "Thalamus"],
+        # TODO: We need to read structure names from the network-config.json
+        structure_names = [x for x in self.network_config["Volume"]]
+        ch = ConvHurt(simulation_structures=structure_names,
                       base_dir=out_dir)
 
-        self.copy_morphologies(nl)
+        self.copy_morphologies()
         self.copy_mechanisms()
-        self.copy_hoc(nl)
+        self.copy_hoc()
 
         # Convert our rotation matrices to vx,vy,vz rotation angles
         # Neurodamus rotation order is first Z then Y and X.
-        (vx, vy, vz) = self.rot_angles_zyx(nl)
-
-        # Node data is stored in a HDF5 file and a CSV file (CONVERT TO micrometers)
-        node_data = OrderedDict([("x", nl.data["neuronPositions"][:, 0] * 1e6),
-                                 ("y", nl.data["neuronPositions"][:, 1] * 1e6),
-                                 ("z", nl.data["neuronPositions"][:, 2] * 1e6),
-                                 ("rotation_angle_zaxis", vz),
-                                 ("rotation_angle_yaxis", vy),
-                                 ("rotation_angle_xaxis", vx)])
-
-        structure_name = "Striatum"
+        (vx, vy, vz) = self.rot_angles_zyx(self.snudda_load)
 
         # We need to convert the named neuron types to numbers
-        (node_type_id, node_type_i_dlookup) = self.allocate_node_type_id(nl)
-        (node_group_id, group_idx, group_lookup) = self.allocate_node_groups(nl)
+        (node_type_id, node_type_id_lookup) = self.allocate_node_type_id()
+        (node_group_id, group_idx, node_group_lookup) = self.allocate_node_groups()
 
-        node_id_list = np.array([x["neuronID"] for x in nl.data["neurons"] if x["volumeID"] == "Striatum"], dtype=int)
+        volume_id_list = [x["volumeID"] for x in self.snudda_load.data["neurons"]]
+        volume_list = set(volume_id_list)
 
-        ch.write_nodes(node_file='Striatum/Striatum_nodes.hdf5',
-                       population_name=structure_name,
-                       data=node_data,
-                       node_id=node_id_list,
-                       node_type_id=node_type_id[node_id_list],
-                       node_group_id=node_group_id[node_id_list],
-                       node_group_index=group_idx[node_id_list])
-
-        striatum_node_names = [n["name"] for n in nl.data["neurons"] \
-                               if n["volumeID"] == structure_name]
-
-        # This defines the order
-        csv_node_name = [k for k in node_type_i_dlookup if k in striatum_node_names]
-
-        csv_node_type_id = [node_type_i_dlookup[n] for n in csv_node_name]
-        csv_node_location = ['Striatum' for n in csv_node_name]
-
-        (model_template_list, model_type_list, morphology_list) = self.get_node_templates(nl, csv_node_name)
-
-        node_data_csv = OrderedDict([("model_type", model_type_list),
-                                     ("model_template", model_template_list),
-                                     ("location", csv_node_location),
-                                     ("morphology", morphology_list),
-                                     ("model_name", csv_node_name)])
-
-        ch.write_node_csv(node_csv_file='Striatum/Striatum_node_types.csv',
-                          node_type_id=csv_node_type_id,
-                          data=node_data_csv)
+        # node_name_list = [x["name"] for x in self.snudda_load.data["neurons"]]
+        node_name_list = [f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
+                          for n in self.snudda_load.data["neurons"]]
 
         # Edge data is stored in a HDF5 file and a CSV file
-        edge_group_lookup = self.allocate_edge_groups(nl)
+        edge_type_lookup = dict()
+        for (pre_type, post_type), con_data in self.snudda_load.data["connectivityDistributions"].items():
+            for con_type, con_type_data in con_data.items():
+                if con_type == "GapJunction":
+                    # TODO: How do we write gap junctions to SONATA?
+                    continue
+                else:
+                    edge_type_id = con_type_data["channelModelID"]
+
+                    if self.target_simulator == "NEST":
+                        if "nestModelTemplate" in con_type_data["channelParameters"]:
+                            edge_model = con_type_data["channelParameters"]["nestModelTemplate"]
+                        else:
+                            edge_model = "static_synapse"
+                    else:
+                        edge_model = con_type_data["channelParameters"]["modFile"]
+
+                edge_type_lookup[pre_type, post_type, con_type] = (edge_type_id, edge_model)
+
+        for volume_name in volume_list:
+            v_idx = np.where([v == volume_name for v in volume_id_list])[0]
+
+            # Node data is stored in a HDF5 file and a CSV file (CONVERT TO micrometers)
+            node_data = OrderedDict([("x", self.snudda_load.data["neuronPositions"][v_idx, 0] * 1e6),
+                                     ("y", self.snudda_load.data["neuronPositions"][v_idx, 1] * 1e6),
+                                     ("z", self.snudda_load.data["neuronPositions"][v_idx, 2] * 1e6),
+                                     ("rotation_angle_zaxis", vz[v_idx]),
+                                     ("rotation_angle_yaxis", vy[v_idx]),
+                                     ("rotation_angle_xaxis", vx[v_idx])])
+
+            node_id_list = np.array([x["neuronID"] for x in self.snudda_load.data["neurons"]
+                                     if x["volumeID"] == "Striatum"], dtype=int)
+
+            assert (v_idx == node_id_list).all()
+
+            ch.write_nodes(node_file=f"{volume_name}_nodes.hdf5",
+                           population_name=volume_name,
+                           data=node_data,
+                           node_id=node_id_list,
+                           node_type_id=node_type_id[node_id_list],
+                           node_group_id=node_group_id[node_id_list],
+                           node_group_index=group_idx[node_id_list])
+
+            csv_node_names = sorted(list(set([node_name_list[x] for x in v_idx])))
+            csv_node_type_id = [node_type_id_lookup[n] for n in csv_node_names]
+            csv_node_location = [volume_name for n in csv_node_names]
+
+            (model_template_list, model_type_list, morphology_list, dynamic_params) \
+                = self.get_node_templates(csv_node_names)
+
+            # Gather all the NEST models
+            dynamic_params = self.copy_and_rewrite_dynamics_params_files(dynamics_params_list=dynamic_params)
+
+            node_data_csv = OrderedDict([("model_type", model_type_list),
+                                         ("model_template", model_template_list),
+                                         ("location", csv_node_location),
+                                         ("morphology", morphology_list),
+                                         ("model_name", csv_node_names)])
+
+            if dynamic_params is not None and len(dynamic_params) > 0:
+                node_data_csv["dynamics_params"] = dynamic_params
+
+            ch.write_node_csv(node_csv_file=f"{volume_name}_node_types.csv",
+                              node_type_id=csv_node_type_id,
+                              data=node_data_csv)
+
+            edge_population_lookup, edge_population_id_lookup = self.setup_edge_population(node_group_lookup)
 
-        # Here we list all the synapses we might want
-        edge_type_lookup = {("MSD1", "MSD1"): 1,
-                            ("MSD1", "MSD2"): 2,
-                            ("MSD2", "MSD1"): 3,
-                            ("MSD2", "MSD2"): 4,
-                            ("FSN", "MSD1"): 5,
-                            ("FSN", "MSD2"): 6,
-                            ("ChIN", "MSD1"): 7,
-                            ("ChIN", "MSD2"): 8,
-                            ("FSN", "FSN"): 9,
-                            ("MSD1", "FSN"): 10,
-                            ("MSD2", "FSN"): 11,
-                            ("MSD1", "ChIN"): 12,
-                            ("MSD2", "ChIN"): 13,
-                            ("FSN", "ChIN"): 14,
-                            ("ChIN", "FSN"): 15,
-                            ("ThalamusAxon", "MSD1"): 16,
-                            ("ThalamusAxon", "MSD2"): 17,
-                            ("ThalamusAxon", "FSN"): 18,
-                            ("ThalamusAxon", "ChIN"): 19,
-                            ("CortexAxon", "MSD1"): 20,
-                            ("CortexAxon", "MSD2"): 21,
-                            ("CortexAxon", "FSN"): 22,
-                            ("CortexAxon", "ChIN"): 23}
-
-        edge_type_id = np.arange(1, 24)
-
-        # These should match edgeTypeLookup
-        edge_csv_data = OrderedDict([('template',
-                                      ['MSGABA',  # 1
-                                       'MSGABA',  # 2
-                                       'MSGABA',  # 3
-                                       'MSGABA',  # 4
-                                       'FSGABA',  # 5
-                                       'FSGABA',  # 6
-                                       'AChSyn',  # 7
-                                       'AChSyn',  # 8
-                                       'FSGABA',  # 9
-                                       'MSGABA',  # 10
-                                       'MSGABA',  # 11
-                                       'MSGABA',  # 12
-                                       'MSGABA',  # 13
-                                       'FSGABA',  # 14
-                                       'AChSyn',  # 15
-                                       'ThalamusGlu',  # 16
-                                       'ThalamusGlu',  # 17
-                                       'ThalamusGlu',  # 18
-                                       'ThalamusGlu',  # 19
-                                       'CortexGlu',  # 20
-                                       'CortexGlu',  # 21
-                                       'CortexGlu',  # 22
-                                       'CortexGlu',  # 23
-                                       ])])
+            population_rows, edge_type_id, source_gid, target_gid, edge_data = \
+                self.setup_edge_info(edge_population_lookup, node_group_id)
 
-        ch.write_edges_csv(edge_csv_file="Striatum/Striatum_edge_types.csv",
+            ch.write_edges(edge_file=f"{volume_name}_edges.hdf5",
+                           population_rows=population_rows,
                            edge_type_id=edge_type_id,
-                           data=edge_csv_data)
+                           source_id=source_gid,
+                           target_id=target_gid,
+                           data=edge_data)
 
-        (edge_group, edge_group_index, edge_type_id, source_gid, target_gid, edgeData) \
-            = self.setup_edge_info(nl, edge_group_lookup, edge_type_lookup)
+            edge_type_id = [x[0] for x in edge_type_lookup.values()]
 
-        ch.write_edges(edge_file="Striatum/Striatum_edges.hdf5",
-                       edge_population_name="Striatum",
-                       edge_group=edge_group,
-                       edge_group_index=edge_group_index,
-                       edge_type_id=edge_type_id,
-                       source_id=source_gid,
-                       target_id=target_gid,
-                       data=edgeData)
-
-        # Next we need to setup virtual nodes for the cortical and thalamic input
-
-        # !!! Change position to real position?!
-        cortex_node_data = OrderedDict([("x", np.zeros((10,))),
-                                        ("y", np.zeros((10,))),
-                                        ("z", np.zeros((10,)))])
+            edge_data = {"model_template": [x[1] for x in edge_type_lookup.values()]}
 
-        cortex_gid = [x["neuronID"] for x in nl.data["neurons"] if x["type"] == "CortexAxon"]
-        cortex_name = [x["name"] for x in nl.data["neurons"] if x["type"] == "CortexAxon"]
+            ch.write_edges_csv(edge_csv_file=f"{volume_name}_edge_types.csv",
+                               edge_type_id=edge_type_id,
+                               data=edge_data)
 
-        # !!! Check this correct
-        cortex_node_type_id = [node_type_i_dlookup[x] for x in cortex_name]
-        try:
-            cortex_node_group_id = [group_lookup["CortexAxon"] for x in range(0, len(cortex_gid))]
-        except:
-            import traceback
-            tstr = traceback.format_exc()
-            print(tstr)
-            import pdb
-            pdb.set_trace()
+        # !!! WE ALSO NEED TO ADD BACKGROUND INPUT TO THE NEURONS IN THE NETWORK
 
-        cortex_node_group_index = np.arange(0, len(cortex_node_group_id), dtype=int)
-        # cortexModelTypeList = [None for x in range(0,len(cortexNodeGroupID))]
-        # cortexModelTemplateList = [None for x in range(0,len(cortexNodeGroupID))]
-
-        cortex_input = self.sort_input(nl, node_type_i_dlookup, input_name="CortexAxon")
-
-        ch.write_nodes(node_file="Cortex/Cortex_nodes.hdf5",
-                       population_name="Cortex",
-                       data=cortex_node_data,
-                       node_id=cortex_gid,
-                       node_type_id=cortex_node_type_id,
-                       node_group_id=cortex_node_group_id,
-                       node_group_index=cortex_node_group_index)
-        # modelType=cortexModelTypeList,
-        # modelTemplate=cortexModelTemplateList)
-
-        # !!! WRITE CORTEX EDGES
-
-        if False:
-            ch.write_edges(edge_file="Cortex/Cortex_edges.hdf5",
-                           edge_population_name="Cortex",
-                           edge_group=edgeGroupCortex,
-                           edge_type_id=edgeTypeIDCortex,
-                           source_id=sourceGIDCortex,
-                           targetIT=targetGIDCortex,
-                           data=edgeDataCortex)
-
-        # Same for Thalamus
-
-        thalamus_gid = [x["neuronID"] for x in nl.data["neurons"] if x["type"] == "ThalamusAxon"]
-
-        thalamus_name = [x["name"] for x in nl.data["neurons"] if x["type"] == "ThalamusAxon"]
-
-        # !!! Check this correct
-        thalamus_node_type_id = [node_type_i_dlookup[x] for x in thalamus_name]
-        thalamus_node_group_id = [group_lookup["ThalamusAxon"] for x in range(0, len(thalamus_gid))]
-        thalamus_node_group_index = np.arange(0, len(thalamus_node_group_id), dtype=int)
-        # thalamusModelTypeList = [None for x in range(0,len(thalamusNodeGroupID))]
-        # thalamusModelTemplateList =[None for x in range(0,len(thalamusNodeGroupID))]
-
-        # !!! Change to real thalamus positions
-        thalamus_node_data = OrderedDict([("x", np.zeros((10,))),
-                                          ("y", np.zeros((10,))),
-                                          ("z", np.zeros((10,)))])
-
-        thalamus_input = self.sort_input(nl, node_type_i_dlookup, input_name="ThalamusAxon")
-
-        ch.write_nodes(node_file="Thalamus/Thalamus_nodes.hdf5",
-                       population_name="Thalamus",
-                       data=thalamus_node_data,
-                       node_id=thalamus_gid,
-                       node_type_id=thalamus_node_type_id,
-                       node_group_id=thalamus_node_group_id,
-                       node_group_index=thalamus_node_group_index)
-        # modelType=thalamusModelTypeList,
-        # modelTemplate=thalamusModelTemplateList)
+        self.write_simulation_config()
 
-        # !!! WRITE THALAMUS EDGES
+        print(f"SONATA files exported to {out_dir}")
 
-        ch.write_input(spike_file_name="inputs/cortexInput.hdf5", spikes=cortex_input)
-        ch.write_input(spike_file_name="inputs/thalamusInput.hdf5", spikes=thalamus_input)
+    ############################################################################
 
-        # !!! WE ALSO NEED TO ADD BACKGROUND INPUT TO THE NEURONS IN THE NETWORK
+    def get_edge_type_lookup(self):
 
-        self.write_simulation_config()
+        # Read the config file, to find out all possible types of connections
 
-        print("SONATA files exported to " + str(out_dir))
+        pass
 
     ############################################################################
 
     def rot_mat_to_angles_xyz(self, rot_mat):
         # http://nghiaho.com/?page_id=846
 
         # This is for Rz*Ry*Rx
@@ -324,262 +232,234 @@
             y[idx] = ang[1]
             z[idx] = ang[2]
 
         return x, y, z
 
     ############################################################################
 
-    def allocate_node_type_id(self, nl):
+    def allocate_node_type_id(self):
+
+        # Since each neuron directory can have multiple morphology/parameter sets
+        # we need to use the name + morphology_key + parameter_key + modulation_key
 
         node_type_id_lookup = OrderedDict([])
         next_node_type_id = 0
 
-        node_names = [n["name"] for n in nl.data["neurons"]]
+        node_names = [f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
+                      for n in self.snudda_load.data["neurons"]]
 
         for n in node_names:
             if n not in node_type_id_lookup:
                 node_type_id_lookup[n] = next_node_type_id
                 next_node_type_id += 1
 
         node_type_id = np.array([node_type_id_lookup[x] for x in node_names], dtype=int)
 
         return node_type_id, node_type_id_lookup
 
     ############################################################################
 
-    # RT neuron only supports one group, so put everything int he same group
-
-    def allocate_node_groups(self, nl):
-
-        node_group_id = np.zeros(len(nl.data["neurons"]), dtype=int)
-        group_idx = np.arange(0, len(nl.data["neurons"]))
-        group_lookup = dict([])
-
-        neuron_types = [nl.data["neurons"][idx]["type"] for idx in range(0, len(nl.data["neurons"]))]
+    # Comment from 2018, hope they support all now (guess we will find out):
+    #  --> RT neuron only supports one group, so put everything in the same group
 
-        for g in neuron_types:
-            if g not in group_lookup:
-                group_lookup[g] = 0
+    # Snudda neuron type corresponds to SONATA NodeGroup
+    # SONATA NodeType is {Snudda neuron name}_{morphology_key}_{parameter_key}_{modulation_key}
 
-        return node_group_id, group_idx, group_lookup
+    def allocate_node_groups(self):
 
-        ############################################################################
+        node_group_id = np.zeros(len(self.snudda_load.data["neurons"]), dtype=int)
+        group_idx = np.zeros(len(self.snudda_load.data["neurons"]), dtype=int)
+        group_lookup = dict([])
 
-    # So there is a bit of a confusion with the namings. For the neurons in the
-    # network "name" corresponds to SONATA NodeType, while "type" corresponds
-    # to NodeGroup.
+        neuron_types = [n["type"] for n in self.snudda_load.data["neurons"]]
 
-    def allocate_node_groups_OLD(self, nl):
-        group_lookup = OrderedDict([])
+        next_group_idx = dict()
         next_group = 0
 
-        group_names = [nl.data["neurons"][idx]["type"] for idx in range(0, len(nl.data["neurons"]))]
-
-        for g in group_names:
-            if g not in group_lookup:
-                group_lookup[g] = next_group
+        for nt in neuron_types:
+            if nt not in group_lookup:
+                group_lookup[nt] = next_group
                 next_group += 1
+                next_group_idx[nt] = 0
 
-        node_group_id = [group_lookup[g] for g in group_names]
-
-        next_idx = np.zeros(len(group_lookup.keys()), dtype=int)
-
-        group_idx = np.zeros(len(group_names), dtype=int)
-
-        for ig, g in enumerate(group_names):
-            group_idx[ig] = next_idx[group_lookup[g]]
-            next_idx[group_lookup[g]] += 1
+        for idx, nt in enumerate(neuron_types):
+            node_group_id[idx] = group_lookup[nt]
+            group_idx[idx] = next_group_idx[nt]
+            next_group_idx[nt] += 1
 
         return node_group_id, group_idx, group_lookup
 
     ############################################################################
 
-    def get_node_templates(self, nl, csv_node_name):
+    def get_node_templates(self, csv_node_name):
 
         template_dict = dict([])
         model_type_dict = dict([])
         morphology_dict = dict([])
         missing_list = []
 
+        dynamics_params_list = []  # Used by NEST
+
         # First create a lookup
-        for n in nl.data["neurons"]:
+        for n in self.snudda_load.data["neurons"]:
             hoc_file = n["hoc"]
-            name = n["name"]
+            name = f"{n['name']}_{n['morphologyKey']}_{n['parameterKey']}_{n['modulationKey']}"
+
             # It seems that RT neuron requires the filename without .swc at the end
             # Also, they prepend morphology path, but only allows one directory for all morphologies
-
-            morph_file = os.path.splitext(os.path.basename(n["morphology"]))[0]
+            # morph_file = os.path.splitext(os.path.basename(n["morphology"]))[0]
+            morph_file = os.path.basename(n["morphology"])
 
             if hoc_file in self.hoc_location_lookup:
                 # We need to change from old hoc location to the SONATA hoc location
-                hoc_str = "hoc:" + os.path.basename(self.hoc_location_lookup[hoc_file])
+                hoc_str = f"hoc:{os.path.basename(self.hoc_location_lookup[hoc_file])}"
             elif n["virtualNeuron"]:
                 hoc_str = "virtual"
             else:
                 hoc_str = "NULL"
                 if hoc_file not in missing_list:
                     # Only write error ones per file
                     print(f"Missing hoc template: {hoc_file}")
                     missing_list.append(hoc_file)
 
             if name not in morphology_dict:
                 morphology_dict[name] = morph_file
             else:
-                assert morphology_dict[name] == morph_file, \
+                assert os.path.basename(morphology_dict[name]) == os.path.basename(morph_file), \
                     f"Morphology mismatch for {name}: {morphology_dict[name]} vs {morph_file}"
 
             if name not in template_dict:
-                template_dict[name] = hoc_str
-                model_type_dict[name] = "biophysical"
-            else:
+                if self.target_simulator == "NEST":
+                    model_type_dict[name] = "point_neuron"
+                    dynamics_params_list.append(self.get_dynamics_params(n))
+                    template_dict[name] = "aeif_cond_exp"
+                else:
+                    model_type_dict[name] = "biophysical"
+                    template_dict[name] = hoc_str
+
+            elif self.target_simulator is not "NEST":
+
                 assert template_dict[name] == hoc_str, \
                     f"All files named {name} do not share same hoc file: {template_dict[name]} and {hoc_str}"
 
         # Need to put them in the order in csvNodeName
 
         template_list = [template_dict[x] for x in csv_node_name]
         model_type_list = [model_type_dict[x] for x in csv_node_name]
         morph_list = [morphology_dict[x] for x in csv_node_name]
 
-        # import pdb
-        # pdb.set_trace()
-
-        return template_list, model_type_list, morph_list
+        return template_list, model_type_list, morph_list, dynamics_params_list
 
     ############################################################################
 
-    def get_node_templates_for_all(self, nl):
+    def copy_and_rewrite_dynamics_params_files(self, dynamics_params_list):
 
-        print("This should return all the types of neurons, eg. FNS_0,FSN_1, ..., MSD1_0, ...")
-        print("This is fewer than the number of neurons. Check CSV file to make sure it is ok after")
+        dest_path = os.path.join(self.out_dir, "components", "point_neuron_dynamics")
 
-        import pdb
-        pdb.set_trace()
+        new_dynamics_params_list = []
+        copied_files = []
 
-        template_list = []
-        model_type_list = []
-        missing_list = []
+        for file_path in dynamics_params_list:
 
-        for neuron in nl.data["neurons"]:
-            hoc_file = neuron["hoc"]
+            if file_path is None:
+                new_dynamics_params_list.append(None)
+                continue
 
-            model_type_list.append("biophysical".encode())
-
-            if hoc_file in self.hoc_location_lookup:
-                hoc_str = f"hoc:{self.hoc_location_lookup[hoc_file]}"
-                template_list.append(hoc_str.encode())
+            if os.path.basename(file_path) == "dynamics_params.json":
+                dir_name = os.path.basename(os.path.dirname(file_path))
+                new_file = os.path.join(dest_path, f"{dir_name}_dynamics_params.json")
             else:
-                template_list.append("".encode())
-                if hoc_file not in missing_list:
-                    # Only write error ones per file
-                    print(f"Missing hoc template: {hoc_file}")
-                    missing_list.append(hoc_file)
-
-        return template_list, model_type_list
+                new_file = os.path.join(dest_path, os.path.basename(file_path))
 
-    ############################################################################
+            if new_file not in copied_files:
+                copyfile(file_path, new_file)
+                copied_files.append(new_file)
 
-    # !!! A lot of HBP tools only support the first group, so put all in group 0
-    # The old code makes separate groups
+            new_dynamics_params_list.append(os.path.basename(new_file))
 
-    def allocate_edge_groups(self, nl):
+        return new_dynamics_params_list
 
-        # FS->MSD1, FS->MSD2 etc are example of EdgeGroups
-        edge_group_lookup = OrderedDict([])
+    def setup_edge_population(self, node_group_lookup):
 
-        unique_group_names = set([nl.data["neurons"][idx]["name"].split("_")[0]
-                                  for idx in range(0, len(nl.data["neurons"]))])
+        edge_population_lookup = dict()
+        edge_population_id_lookup = dict()
+        next_id = 1
 
-        for g1 in unique_group_names:
-            for g2 in unique_group_names:
-                edge_group_lookup[g1, g2] = 0
+        for pre_node_type, pre_node_group in node_group_lookup.items():
+            for post_node_type, post_node_group in node_group_lookup.items():
+                edge_population_lookup[pre_node_group, post_node_group] = f"{pre_node_type}_{post_node_type}"
+                edge_population_id_lookup[pre_node_group, post_node_group] = next_id
+                next_id += 1
 
-        return edge_group_lookup
-
-    ############################################################################
-
-    # !!! This is old version, that makes separate groups for different sets
-    # of synapses, but HBP tools only support first group currently, Jan 2019.
-    # so made another version of allocateEdgeGroups (see above).
-
-    def allocate_edge_groups_OLD(self, nl):
-
-        # FS->MSD1, FS->MSD2 etc are example of EdgeGroups
-        edge_group_lookup = OrderedDict([])
-
-        unique_group_names = set([nl.data["neurons"][idx]["name"].split("_")[0]
-                                  for idx in range(0, len(nl.data["neurons"]))])
-
-        next_group = 0
-
-        for g1 in unique_group_names:
-            for g2 in unique_group_names:
-                edge_group_lookup[g1, g2] = next_group
-                next_group += 1
-
-        return edge_group_lookup
+        return edge_population_lookup, edge_population_id_lookup
 
     ############################################################################
 
     # This code sets up the info about edges
 
-    def setup_edge_info(self, nl, edge_group_lookup, edge_type_lookup):
+    def setup_edge_info(self, edge_population_lookup, node_group_id):
 
-        n_synapses = nl.data["synapses"].shape[0]
-        edge_group = np.zeros(n_synapses, dtype=int)
-        edge_group_index = np.zeros(n_synapses, dtype=int)
+        n_synapses = self.snudda_load.data["synapses"].shape[0]
         edge_type_id = np.zeros(n_synapses, dtype=int)
         source_gid = np.zeros(n_synapses, dtype=int)
         target_gid = np.zeros(n_synapses, dtype=int)
 
+        population_rows = dict()  # For each population name, list all the synapse rows
+
         sec_id = np.zeros(n_synapses, dtype=int)
         sec_x = np.zeros(n_synapses)
         syn_weight = np.zeros(n_synapses)
         delay = np.zeros(n_synapses)
 
-        edge_group_count = np.zeros(len(edge_group_lookup.keys()))
-
         # Check if these speeds are reasonable?
         axon_speed = 25.0  # 25m/s
         dend_speed = 1.0
 
         # columns in nl.data["synapses"]
         # 0: sourceCellID, 1: sourceComp, 2: destCellID, 3: destComp,
         # 4: locType, 5: synapseType, 6: somaDistDend 7:somaDistAxon
         # somaDist is an int, representing micrometers
 
-        for i_syn, syn_row in enumerate(nl.data["synapses"]):
+        for i_syn, syn_row in enumerate(self.snudda_load.data["synapses"]):
             source_gid[i_syn] = syn_row[0]
             target_gid[i_syn] = syn_row[1]
+
+            source_node_group = node_group_id[syn_row[0]]
+            target_node_group = node_group_id[syn_row[1]]
+
+            population_group = edge_population_lookup[source_node_group, target_node_group]
+
+            if population_group in population_rows:
+                population_rows[population_group].append(i_syn)
+            else:
+                population_rows[population_group] = [i_syn]
+
             sec_id[i_syn] = syn_row[9]
             sec_x[i_syn] = syn_row[10] / 1000.0
+            synapse_type = syn_row[6]
 
-            pre_type = nl.data["neurons"][source_gid[i_syn]]["type"]
-            post_type = nl.data["neurons"][target_gid[i_syn]]["type"]
+            pre_type = self.snudda_load.data["neurons"][source_gid[i_syn]]["type"]
+            post_type = self.snudda_load.data["neurons"][target_gid[i_syn]]["type"]
 
-            edge_group[i_syn] = edge_group_lookup[pre_type, post_type]
-            edge_type_id[i_syn] = edge_type_lookup[pre_type, post_type]
-
-            edge_group_index[i_syn] = edge_group_count[edge_group[i_syn]]
-            edge_group_count[edge_group[i_syn]] += 1
+            edge_type_id[i_syn] = synapse_type
 
             dend_dist = syn_row[6] * 1e-6
             axon_dist = syn_row[7] * 1e-6
             delay[i_syn] = axon_dist / axon_speed + dend_dist / dend_speed
             syn_weight[i_syn] = 1.0  # !!! THIS NEEDS TO BE SET DEPENDING ON CONNECTION TYPE
 
         edge_data = OrderedDict([("sec_id", sec_id),
                                  ("sec_x", sec_x),
                                  ("syn_weight", syn_weight),
                                  ("delay", delay)])
 
-        # Need to set edgeGroup, edgeGroupIndex, edgeType also
+        for pop_name in population_rows.keys():
+            population_rows[pop_name] = np.array(population_rows[pop_name])
 
-        return (edge_group, edge_group_index, edge_type_id,
-                source_gid, target_gid, edge_data)
+        return population_rows, edge_type_id, source_gid, target_gid, edge_data
 
     ############################################################################
 
     # Convert synapse coordinates (in SWC reference frame) to SectionID
     # and section_X (fractional distance along dendritic section)
 
     def conv_synapse_coord_to_section(self, cell_gid, orig_synapse_coord, network_info):
@@ -630,14 +510,40 @@
         # import pdb
         # pdb.set_trace()
 
         return sec_id, sec_x
 
     ############################################################################
 
+    def get_dynamics_params(self, neuron):
+
+        if self.target_simulator == "NEST":
+            # If the dynamics_params.json file exist in the neuron path, then use that
+            neuron_path = os.path.relpath(snudda_parse_path(neuron["neuronPath"], self.snudda_load.data["SnuddaData"]))
+            dynamics_params_path = os.path.join(neuron_path, "dynamics_params.json")
+
+            if os.path.isfile(dynamics_params_path):
+                return dynamics_params_path
+
+            # Otherwise, if there is a default model in the nest/models directory, use that
+            neuron_type = neuron["type"]
+            alt_dynamics_path = os.path.join(self.snudda_load.data["SnuddaData"],
+                                             "nest", "models", f"{neuron_type}.json")
+            if os.path.isfile(alt_dynamics_path):
+
+                print(f"Missing {dynamics_params_path} file, using {alt_dynamics_path}")
+
+                return alt_dynamics_path
+
+            return None
+        else:
+            return None
+
+    ############################################################################
+
     def convert_coordinates(self, morphology):
 
         # Loop through entire SWC morphology, calculate SEC_ID, SEC_X
         # for each vertex.
 
         print("TEST TEST TEST")
         import pdb
@@ -862,87 +768,79 @@
         print(f"Writing {out_conf_file}")
 
         with open(out_conf_file, 'wt') as f:
             json.dump(sim_conf, f, indent=4)
 
     ############################################################################
 
-    def copy_morphologies(self, nl):
+    def copy_morphologies(self):
         from shutil import copyfile
         import os
 
         self.morph_location_lookup = dict([])
 
         print("Copying morphologies")
 
-        # Loop through all the neurons, and copy the morphologies
-        for neuron_id in nl.config:
-            if neuron_id in ["Volume", "Channels"]:
-                continue  # Not cell, skip
+        morph_set = set([n["morphology"] for n in self.snudda_load.data["neurons"]])
 
-            morph_file = nl.config[neuron_id]["morphology"]
+        for morph_path in morph_set:
+            morph_file = snudda_parse_path(morph_path, snudda_data=self.snudda_load.data["SnuddaData"])
             base_name = os.path.basename(morph_file)
-            dest_file = self.out_dir + "components/morphologies/" + base_name
+            dest_file = os.path.join(self.out_dir, "components", "morphologies", base_name)
 
             if self.debug:
-                print("Copying " + morph_file + " to " + dest_file)
+                print(f"Copying {morph_file} to {dest_file}")
 
             copyfile(morph_file, dest_file)
-            self.morph_location_lookup[morph_file] = dest_file
+            self.morph_location_lookup[morph_path] = os.path.relpath(dest_file)
 
     ############################################################################
 
-    def copy_hoc(self, nl):
-        from shutil import copyfile
-        import os
+    def copy_hoc(self):
 
         self.hoc_location_lookup = dict([])
 
         print("Copying hoc files...")
 
         missing_files = []
 
-        # Loop through all the neurons, and copy the hoc
-        for neuron_id in nl.config:
-            if neuron_id in ["Volume", "Channels"]:
-                continue  # Not cell, skip
-
-            hoc_file = nl.config[neuron_id]["hoc"]
+        hoc_set = set([n["hoc"] for n in self.snudda_load.data["neurons"] if n["hoc"]])
 
+        for hoc_path in hoc_set:
+            hoc_file = snudda_parse_path(hoc_path, snudda_data=self.snudda_load.data["SnuddaData"])
             if os.path.isfile(hoc_file):
                 base_name = os.path.basename(hoc_file)
                 dest_file = os.path.join(self.out_dir, "components", "hoc_templates", base_name)
 
                 if self.debug:
                     print(f"Copying {hoc_file} to {dest_file}")
 
-                self.hoc_location_lookup[hoc_file] = dest_file
+                self.hoc_location_lookup[hoc_path] = dest_file
                 copyfile(hoc_file, dest_file)
             else:
-
                 if hoc_file not in missing_files:
                     # Only print same error message ones
-                    print(f"!!! Missing hoc file: {hoc_file}")
+                    print(f"- Missing hoc file: {hoc_file}")
 
                 missing_files.append(hoc_file)
 
-                ############################################################################
+    ############################################################################
 
     def copy_mechanisms(self):
-        from shutil import copyfile
-        from glob import glob
-        import os
 
         print("Copying mechanisms")
+        mech_path = snudda_parse_path(os.path.join("$SNUDDA_DATA", "neurons", "mechanisms"),
+                                      snudda_data=self.snudda_load.data["SnuddaData"])
 
-        for mech in glob("*.mod"):
+        for mech in glob(os.path.join(mech_path, "*.mod")):
             if self.debug:
                 print(f"Copying {mech}")
 
-            copyfile(mech, os.path.join(self.out_dir, "components", "mechanisms", mech))
+            mech_file = os.path.basename(mech)
+            copyfile(mech, os.path.join(self.out_dir, "components", "mechanisms", mech_file))
 
     ############################################################################
 
     def sort_input(self, nl, node_type_id_lookup, input_name=None):
 
         if self.input_file is None or not os.path.isfile(self.input_file):
             print("No input file has been specified!")
```

### Comparing `snudda-1.4.0/snudda/utils/fake_load.py` & `snudda-1.4.4/snudda/utils/fake_load.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/load.py` & `snudda-1.4.4/snudda/utils/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import OrderedDict
 
 import numpy as np
 
 from snudda.neurons.neuron_prototype import NeuronPrototype
 from snudda.utils.numpy_encoder import NumpyEncoder
 import scipy.sparse as sparse
+from scipy.spatial import distance_matrix
 
 
 class SnuddaLoad(object):
     """
     Load data from network-neuron-positions.hdf5 or network-neuron-synapses.hdf5 into python dictionary
     """
 
@@ -329,15 +330,15 @@
                 json.loads(SnuddaLoad.to_str(f["meta/connectivityDistributions"][()]), object_pairs_hook=OrderedDict)
 
             for keys in orig_connectivity_distributions:
                 (pre_type, post_type) = keys.split("$$")
                 data["connectivityDistributions"][pre_type, post_type] \
                     = orig_connectivity_distributions[keys]
 
-        if "synapses" in data:
+        if "synapses" in data and self.verbose:
             if "gapJunctions" in data:
                 print(f"Loading {len(data['neurons'])} neurons with {data['nSynapses']} synapses"
                       f" and {data['nGapJunctions']} gap junctions")
             else:
                 print(f"Loading {len(data['neurons'])} neurons with {data['synapses'].shape[0]} synapses")
 
         if self.verbose:
@@ -925,15 +926,15 @@
         gj_coords = gap_junctions[:, 6:9][:gj_ctr, :] * self.data["voxelSize"] + self.data["simulationOrigo"]
 
         if return_index:
             return gap_junctions[:gj_ctr, :], gj_coords, gj_index_list[:gj_ctr]
         else:
             return gap_junctions[:gj_ctr, :], gj_coords
 
-    def get_centre_neurons_iterator(self, n_neurons=None, neuron_type=None, centre_point=None):
+    def get_centre_neurons_iterator(self, n_neurons=None, neuron_type=None, centre_point=None, max_distance=None):
 
         """ Return neuron id:s, starting from the centre most and moving outwards
 
         Args:
             n_neurons (int) : Number of neurons to return, None = all available
             neuron_type (str) : Type of neurons to return, None = all available
             centre_point (np.array) : x,y,z of centre position, None = auto detect centre
@@ -947,18 +948,23 @@
 
         neuron_ctr = 0
 
         for neuron_id in idx:
             if neuron_type is not None and self.data["neurons"][neuron_id]["type"] != neuron_type:
                 continue
 
+            if max_distance is not None and dist_to_centre[neuron_id] > max_distance:
+                # Stop iterator if max distance is reached
+                return
+
             yield neuron_id, dist_to_centre[neuron_id]
             neuron_ctr += 1
 
             if n_neurons is not None and neuron_ctr >= n_neurons:
+                # Stop iterator if n_neurons are delivered
                 return
 
     ############################################################################
 
     def create_connection_matrix(self, sparse_matrix=True):
 
         if sparse_matrix:
@@ -967,14 +973,36 @@
             connection_matrix = np.zeros((self.data["nNeurons"], self.data["nNeurons"]), dtype=np.ushort)
 
         for syn_row in self.data["synapses"]:
             connection_matrix[syn_row[0], syn_row[1]] += 1
 
         return connection_matrix
 
+    def create_distance_matrix(self, neuron_id=None, pre_id=None, post_id=None):
+
+        if neuron_id is not None and pre_id is not None and post_id is not None:
+            raise ValueError("Specify either neuron_id or the two parameters pre_id and post_id.")
+
+        if (pre_id is None) ^ (post_id is None):
+            raise ValueError("pre_id and post_id must both either be specified, or neither")
+
+        pos = self.data["neuronPositions"]
+
+        if neuron_id is not None:
+            pos = pos[neuron_id, :]
+            dist_matrix = distance_matrix(pos, pos)
+
+        elif pre_id is not None and post_id is not None:
+            dist_matrix = distance_matrix(pos[pre_id, :], pos[post_id, :])
+
+        else:
+            dist_matrix = distance_matrix(pos, pos)
+
+        return dist_matrix
+
     def print_all_synapse_counts_per_type(self):
 
         synapse_types = sorted(list(self.get_neuron_types(return_set=True)))
         connection_matrix = self.create_connection_matrix()
 
         for pre_type in synapse_types:
             for post_type in synapse_types:
@@ -1038,14 +1066,15 @@
             gap_junction_count += np.sum(neuron_id_mask[gap_junctions[:, 0]])
             gap_junction_count += np.sum(neuron_id_mask[gap_junctions[:, 1]])
 
         gap_junction_count /= 2
 
         return synapse_count, gap_junction_count
 
+
 def snudda_load_cli():
     """ Command line parser for SnuddaLoad script """
 
     from argparse import ArgumentParser
 
     parser = ArgumentParser(description="Load snudda network file (hdf5)")
     parser.add_argument("networkFile", help="Network file (hdf5)", type=str)
@@ -1067,15 +1096,15 @@
     args = parser.parse_args()
 
     if args.keepOpen:
         load_synapses = False
     else:
         load_synapses = True
 
-    nl = SnuddaLoad(args.networkFile, load_synapses=load_synapses)
+    nl = SnuddaLoad(args.networkFile, load_synapses=load_synapses, verbose=True)
 
     if args.listN:
         print("Neurons in network: ")
 
         if args.detailed:
             for nid, name, pos, par_key, morph_key, mod_key, neuron_path, pop_id \
                     in [(x["neuronID"], x["name"], x["position"],
```

### Comparing `snudda-1.4.0/snudda/utils/load_network_simulation.py` & `snudda-1.4.4/snudda/utils/load_network_simulation.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/merge_synapse_files.py` & `snudda-1.4.4/snudda/utils/merge_synapse_files.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/numpy_encoder.py` & `snudda-1.4.4/snudda/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/reposition_neurons.py` & `snudda-1.4.4/snudda/utils/reposition_neurons.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/snudda_path.py` & `snudda-1.4.4/snudda/utils/snudda_path.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda/utils/swap_to_degenerated_morphologies.py` & `snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class SwapToDegeneratedMorphologies:
 
     def __init__(self, original_network_file, new_network_file,
                  original_snudda_data_dir, new_snudda_data_dir,
                  original_input_file=None, new_input_file=None,
-                 filter_axon=False):
+                 filter_axon=False, forced_param_key=None):
 
         """ This code replaces the neuron morphologies in the original network with user provided degenerated copies
             of the neurons. The synapses that are on removed dendritic will also be removed.
             The section ID and section X is also updated to match the new degenerated morphologies.
 
             Args:
                 original_network_file (str) : Path to input network-synapses.hdf5
@@ -38,14 +38,15 @@
         self.new_snudda_data_dir = new_snudda_data_dir
 
         assert self.original_snudda_data_dir != self.new_snudda_data_dir, \
             f"SNUDDA_DATA_DIR should be different for WT and degenerated"
 
         self.original_input_file = original_input_file
         self.new_input_file = new_input_file
+        self.forced_param_key = forced_param_key
 
         self.original_network_loader = SnuddaLoad(self.original_network_file, load_synapses=False)
         self.old_hdf5 = self.original_network_loader.hdf5_file
         self.old_data = self.original_network_loader.data
 
         self.morphology_map = dict()
         self.section_lookup = dict()
@@ -92,14 +93,17 @@
         network_group = self.new_hdf5.create_group("network")
         self.old_hdf5.copy(source=self.old_hdf5["network/neurons"], dest=self.new_hdf5["network"])
 
         # Update parameter keys and morphology keys
         for idx, neuron_id in enumerate(self.new_hdf5["network/neurons/neuronID"]):
             assert idx == neuron_id, "There should be no gaps in numbering."
             param_key, morph_key, neuron_path, param_id, morph_id = self.find_morpology(neuron_id)
+
+            if self.forced_param_key:
+                param_key=self.forced_param_key
             self.new_hdf5[f"network/neurons/parameterKey"][idx] = param_key
             self.new_hdf5[f"network/neurons/morphologyKey"][idx] = morph_key
             # self.new_hdf5[f"network/neurons/parameterID"][idx] = param_id
             # self.new_hdf5[f"network/neurons/morphologyID"][idx] = morph_id
 
         self.filter_synapses(filter_axon=self.filter_axon)
         self.filter_gap_junctions()
```

### Comparing `snudda-1.4.0/snudda/utils/swap_to_degenerated_morphologies_extended.py` & `snudda-1.4.4/snudda/utils/swap_to_degenerated_morphologies_extended.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 
         print("Synapse degeneration recovery...")
         # If degenerationRecovery is set in the pruning rules, we will add that fraction of the synapses on the
         # overlapping morphology part back to the network synapses -- and take care not to place synapses
         # exactly where old synapses are already placed
 
         # Get information about synapse degeneration recovery (ie how large a fraction of the synapses
-        # that are in the overlaping part of the dendrites should be kept to recover a little...
+        # that are in the overlaping part of the dendrites should be kept to recover a little...)
         degeneration_recovery, type_lookup = self.get_degeneration_recovery_lookups(network_config=network_config)
 
         if len(degeneration_recovery) > 0:
             p_recovery = np.zeros((synapse_matrix.shape[0],), dtype=float)
 
             for idx, syn_row in enumerate(synapse_matrix):
                 pre_type = type_lookup[syn_row[0]]
```

### Comparing `snudda-1.4.0/snudda/utils/upgrade_old_network_file.py` & `snudda-1.4.4/snudda/utils/upgrade_old_network_file.py`

 * *Files identical despite different names*

### Comparing `snudda-1.4.0/snudda.egg-info/PKG-INFO` & `snudda-1.4.4/snudda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snudda
-Version: 1.4.0
+Version: 1.4.4
 Summary: Create realistic networks of neurons, synapses placed using touch detection between axons and dendrites.
 Home-page: https://github.com/Hjorthmedh/Snudda
 Author: Johannes Hjorth
 Author-email: hjorth@kth.se
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `snudda-1.4.0/snudda.egg-info/SOURCES.txt` & `snudda-1.4.4/snudda.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 snudda/analyse/analyse_input.py
 snudda/analyse/analyse_neuroinformatics2020.py
 snudda/analyse/analyse_spike_trains.py
 snudda/analyse/analyse_striatum.py
 snudda/analyse/analyse_synapse_location.py
 snudda/analyse/analyse_topology.py
 snudda/analyse/analyse_topology_activity.py
+snudda/analyse/spike_time_tiling_coefficient.py
 snudda/data/InputAxons/Cortex/AA0059.swc
 snudda/data/InputAxons/Cortex/Reg10/AA0059-reg10.swc
 snudda/data/InputAxons/Cortex/Reg15/AA0059-reg15.swc
 snudda/data/InputAxons/Cortex/Reg5/AA0059-reg5.swc
 snudda/data/InputAxons/GPe2Striatum/example-projection-config.json
 snudda/data/InputAxons/GPe2Striatum/prototypical-axon.swc
 snudda/data/InputAxons/Thalamus/AA0054.swc
@@ -61,24 +62,29 @@
 snudda/data/input_config/input-tinytest-Channel-Activation.json
 snudda/data/input_config/input-tinytest-channel-1.json
 snudda/data/input_config/input-tinytest-channel-2.json
 snudda/data/input_config/input-tinytest-v7.json
 snudda/data/input_config/input-tinytest-v8.json
 snudda/data/input_config/input-tinytest-v9-freq-vectors.json
 snudda/data/input_config/input-v10-scaled.json
+snudda/data/input_config/input_output_dspn_template_IC.json
 snudda/data/mesh/GPe.obj
 snudda/data/mesh/GPi.obj
 snudda/data/mesh/SNc.obj
 snudda/data/mesh/SNr.obj
 snudda/data/mesh/STN.obj
 snudda/data/mesh/Striatum-d.obj
 snudda/data/mesh/Striatum-dorsal-left-hemisphere.obj
 snudda/data/mesh/Striatum-dorsal-right-hemisphere.obj
 snudda/data/mesh/Striatum-v.obj
 snudda/data/mesh/get_mesh.ipynb
+snudda/data/nest/models/FS.json
+snudda/data/nest/models/dSPN.json
+snudda/data/nest/models/iSPN.json
+snudda/data/neurons/mechanisms/Im_ms.mod
 snudda/data/neurons/mechanisms/Kv3_ch.mod
 snudda/data/neurons/mechanisms/NO.mod
 snudda/data/neurons/mechanisms/bk_ch.mod
 snudda/data/neurons/mechanisms/bk_fs.mod
 snudda/data/neurons/mechanisms/bk_ms.mod
 snudda/data/neurons/mechanisms/ca_ch.mod
 snudda/data/neurons/mechanisms/cadyn_fs.mod
@@ -100,30 +106,33 @@
 snudda/data/neurons/mechanisms/concDA.mod
 snudda/data/neurons/mechanisms/concDAfile.mod
 snudda/data/neurons/mechanisms/hcn12_ch.mod
 snudda/data/neurons/mechanisms/hd_lts.mod
 snudda/data/neurons/mechanisms/im_lts.mod
 snudda/data/neurons/mechanisms/it_lts.mod
 snudda/data/neurons/mechanisms/kaf_fs.mod
+snudda/data/neurons/mechanisms/kaf_lts.mod
 snudda/data/neurons/mechanisms/kaf_ms.mod
 snudda/data/neurons/mechanisms/kas_fs.mod
 snudda/data/neurons/mechanisms/kas_ms.mod
 snudda/data/neurons/mechanisms/kcnq_ch.mod
+snudda/data/neurons/mechanisms/kdb_lts.mod
 snudda/data/neurons/mechanisms/kdr_fs.mod
 snudda/data/neurons/mechanisms/kdr_lts.mod
 snudda/data/neurons/mechanisms/kdr_ms.mod
-snudda/data/neurons/mechanisms/kdrbca1_lts.mod
+snudda/data/neurons/mechanisms/kdrb_lts.mod
+snudda/data/neurons/mechanisms/kir23_ch.mod
 snudda/data/neurons/mechanisms/kir23_lts.mod
 snudda/data/neurons/mechanisms/kir2_ch.mod
 snudda/data/neurons/mechanisms/kir_fs.mod
 snudda/data/neurons/mechanisms/kir_ms.mod
 snudda/data/neurons/mechanisms/kv2_ch.mod
 snudda/data/neurons/mechanisms/kv4_ch.mod
 snudda/data/neurons/mechanisms/na2_ch.mod
-snudda/data/neurons/mechanisms/na3n_lts.mod
+snudda/data/neurons/mechanisms/na3_lts.mod
 snudda/data/neurons/mechanisms/na_ch.mod
 snudda/data/neurons/mechanisms/naf_fs.mod
 snudda/data/neurons/mechanisms/naf_lts.mod
 snudda/data/neurons/mechanisms/naf_ms.mod
 snudda/data/neurons/mechanisms/par_ggap.mod
 snudda/data/neurons/mechanisms/sk_ch.mod
 snudda/data/neurons/mechanisms/sk_fs.mod
@@ -182,83 +191,14 @@
 snudda/data/neurons/mechanisms.OLD/sk_fs.mod
 snudda/data/neurons/mechanisms.OLD/sk_ms.mod
 snudda/data/neurons/mechanisms.OLD/tmampa.mod
 snudda/data/neurons/mechanisms.OLD/tmgabaa.mod
 snudda/data/neurons/mechanisms.OLD/tmglut.mod
 snudda/data/neurons/mechanisms.OLD/tmnmda.mod
 snudda/data/neurons/mechanisms.OLD/vecevent.mod
-snudda/data/neurons/mechanismsWithModulation/#na_ch.mod#
-snudda/data/neurons/mechanismsWithModulation/Kv3_ch.mod
-snudda/data/neurons/mechanismsWithModulation/M4.mod
-snudda/data/neurons/mechanismsWithModulation/NO.mod
-snudda/data/neurons/mechanismsWithModulation/bk_ch.mod
-snudda/data/neurons/mechanismsWithModulation/bk_fs.mod
-snudda/data/neurons/mechanismsWithModulation/bk_ms.mod
-snudda/data/neurons/mechanismsWithModulation/ca_ch.mod
-snudda/data/neurons/mechanismsWithModulation/cadyn_fs.mod
-snudda/data/neurons/mechanismsWithModulation/cadyn_ms.mod
-snudda/data/neurons/mechanismsWithModulation/cal12_ms.mod
-snudda/data/neurons/mechanismsWithModulation/cal12_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/cal13_ms.mod
-snudda/data/neurons/mechanismsWithModulation/cal13_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/cal_ch.mod
-snudda/data/neurons/mechanismsWithModulation/caldyn_ms.mod
-snudda/data/neurons/mechanismsWithModulation/can_fs.mod
-snudda/data/neurons/mechanismsWithModulation/can_ms.mod
-snudda/data/neurons/mechanismsWithModulation/can_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/cap_ch.mod
-snudda/data/neurons/mechanismsWithModulation/caq_fs.mod
-snudda/data/neurons/mechanismsWithModulation/caq_ms.mod
-snudda/data/neurons/mechanismsWithModulation/car_fs.mod
-snudda/data/neurons/mechanismsWithModulation/car_ms.mod
-snudda/data/neurons/mechanismsWithModulation/car_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/cat32_ms.mod
-snudda/data/neurons/mechanismsWithModulation/cat33_ms.mod
-snudda/data/neurons/mechanismsWithModulation/concACh.mod
-snudda/data/neurons/mechanismsWithModulation/concDA.mod
-snudda/data/neurons/mechanismsWithModulation/concDAfile.mod
-snudda/data/neurons/mechanismsWithModulation/hcn12_ch.mod
-snudda/data/neurons/mechanismsWithModulation/hd_lts.mod
-snudda/data/neurons/mechanismsWithModulation/im_lts.mod
-snudda/data/neurons/mechanismsWithModulation/it_lts.mod
-snudda/data/neurons/mechanismsWithModulation/kaf_fs.mod
-snudda/data/neurons/mechanismsWithModulation/kaf_ms.mod
-snudda/data/neurons/mechanismsWithModulation/kaf_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/kas_fs.mod
-snudda/data/neurons/mechanismsWithModulation/kas_ms.mod
-snudda/data/neurons/mechanismsWithModulation/kas_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/kcnq_ch.mod
-snudda/data/neurons/mechanismsWithModulation/kdr_fs.mod
-snudda/data/neurons/mechanismsWithModulation/kdr_lts.mod
-snudda/data/neurons/mechanismsWithModulation/kdr_ms.mod
-snudda/data/neurons/mechanismsWithModulation/kir23_lts.mod
-snudda/data/neurons/mechanismsWithModulation/kir23_lts_mod.mod
-snudda/data/neurons/mechanismsWithModulation/kir2_ch.mod
-snudda/data/neurons/mechanismsWithModulation/kir_fs.mod
-snudda/data/neurons/mechanismsWithModulation/kir_ms.mod
-snudda/data/neurons/mechanismsWithModulation/kir_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/kv2_ch.mod
-snudda/data/neurons/mechanismsWithModulation/kv4_ch.mod
-snudda/data/neurons/mechanismsWithModulation/na2_ch.mod
-snudda/data/neurons/mechanismsWithModulation/na3n_lts.mod
-snudda/data/neurons/mechanismsWithModulation/na_ch.mod
-snudda/data/neurons/mechanismsWithModulation/naf_fs.mod
-snudda/data/neurons/mechanismsWithModulation/naf_lts.mod
-snudda/data/neurons/mechanismsWithModulation/naf_lts_mod.mod
-snudda/data/neurons/mechanismsWithModulation/naf_ms.mod
-snudda/data/neurons/mechanismsWithModulation/naf_ms_mod.mod
-snudda/data/neurons/mechanismsWithModulation/par_ggap.mod
-snudda/data/neurons/mechanismsWithModulation/sk_ch.mod
-snudda/data/neurons/mechanismsWithModulation/sk_fs.mod
-snudda/data/neurons/mechanismsWithModulation/sk_ms.mod
-snudda/data/neurons/mechanismsWithModulation/tmampa.mod
-snudda/data/neurons/mechanismsWithModulation/tmgabaa.mod
-snudda/data/neurons/mechanismsWithModulation/tmglut.mod
-snudda/data/neurons/mechanismsWithModulation/tmnmda.mod
-snudda/data/neurons/mechanismsWithModulation/vecevent.mod
 snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/mechanisms.json
 snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/modulation.json
 snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/optim_chin_morph_renamed2019-11-08.swc
 snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/parameters.json
 snudda/data/neurons/striatum/chin/str-chin-e170614_cell6-m17JUL301751_170614_no6_MD_cell_1_x63-v20190710/protocols.json
 snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/WT-0728MSN01-cor-rep-ax.swc
 snudda/data/neurons/striatum/dspn/str-dspn-e150602_c1_D1-mWT-0728MSN01-v20190508/fix_indexing.py
@@ -406,14 +346,16 @@
 snudda/place/place.py
 snudda/place/projection_map_finder.py
 snudda/place/region_mesh.py
 snudda/place/rotation.py
 snudda/place/volumetric_mapping.py
 snudda/plotting/__init__.py
 snudda/plotting/plotLTSdensity.py
+snudda/plotting/plot_connection_matrix.py
+snudda/plotting/plot_connectivity.py
 snudda/plotting/plot_cross_correlogram.py
 snudda/plotting/plot_degeneration.py
 snudda/plotting/plot_degeneration_and_growth.py
 snudda/plotting/plot_density.py
 snudda/plotting/plot_density_slice.py
 snudda/plotting/plot_distance_statistics.py
 snudda/plotting/plot_input.py
```

