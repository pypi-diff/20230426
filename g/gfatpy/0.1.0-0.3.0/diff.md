# Comparing `tmp/gfatpy-0.1.0.tar.gz` & `tmp/gfatpy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gfatpy-0.1.0.tar", max compression
+gzip compressed data, was "gfatpy-0.3.0.tar", max compression
```

## Comparing `gfatpy-0.1.0.tar` & `gfatpy-0.3.0.tar`

### file list

```diff
@@ -1,199 +1,220 @@
--rw-r--r--   0        0        0     1470 2022-09-29 12:34:07.125117 gfatpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     2704 2022-10-24 11:35:53.659111 gfatpy-0.1.0/gfatpy/__init__.py
--rw-r--r--   0        0        0     1077 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/__init__.py
--rw-r--r--   0        0        0      710 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/aeronet4lidar.py
--rw-r--r--   0        0        0     1053 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/aeronet/info.yml
--rw-r--r--   0        0        0    17421 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/plot.py
--rw-r--r--   0        0        0     3965 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/reader.py
--rw-r--r--   0        0        0     8805 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/typing.py
--rw-r--r--   0        0        0    16772 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/aeronet/utils.py
--rw-r--r--   0        0        0    28725 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/assets/LOGO_GFAT_150pp.png
--rw-r--r--   0        0        0        0 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/atmo/__init__.py
--rw-r--r--   0        0        0    20252 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/atmo/atmo.py
--rw-r--r--   0        0        0     4773 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/atmo/ecmwf.py
--rw-r--r--   0        0        0    74896 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/atmo/solar.py
--rw-r--r--   0        0        0     3565 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/cli/lidar/main.py
--rw-r--r--   0        0        0     1183 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/cli/lidar/plot/main.py
--rw-r--r--   0        0        0      896 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/cli/main.py
--rw-r--r--   0        0        0      270 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/cloudnet/__init__.py
--rw-r--r--   0        0        0     8810 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/cloudnet/cloud_model.py
--rw-r--r--   0        0        0       49 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/cloudnet/info.yml
--rw-r--r--   0        0        0     4600 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/cloudnet/plot_deprecated.py
--rw-r--r--   0        0        0     5423 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/cloudnet/reader.py
--rw-r--r--   0        0        0    18059 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/cloudnet/utils.py
--rw-r--r--   0        0        0      928 2022-10-13 07:57:45.247862 gfatpy-0.1.0/gfatpy/config.py
--rw-r--r--   0        0        0       70 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/constants.py
--rw-r--r--   0        0        0      307 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/lidar/__init__.py
--rw-r--r--   0        0        0      174 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
--rw-r--r--   0        0        0      121 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/.hgignore
--rw-r--r--   0        0        0      570 2022-10-24 11:26:56.357627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/.hgtags
--rw-r--r--   0        0        0  2508885 2022-10-24 11:26:56.369627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
--rw-r--r--   0        0        0     2541 2022-10-24 11:26:56.369627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
--rw-r--r--   0        0        0   179833 2022-10-24 11:26:56.373627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
--rw-r--r--   0        0        0   793573 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
--rw-r--r--   0        0        0    13468 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
--rw-r--r--   0        0        0     1628 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/README.md
--rw-r--r--   0        0        0      108 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/requirements.txt
--rw-r--r--   0        0        0        0 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
--rw-r--r--   0        0        0     7453 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
--rw-r--r--   0        0        0     7455 2022-10-24 11:26:56.377627 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
--rw-r--r--   0        0        0     7390 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
--rw-r--r--   0        0        0    11034 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
--rw-r--r--   0        0        0    10931 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
--rw-r--r--   0        0        0    11059 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
--rw-r--r--   0        0        0    11059 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
--rw-r--r--   0        0        0    11059 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
--rw-r--r--   0        0        0     3352 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/tests/datos/MULHACEN/QA/GHK/2022/10/04/output_optic_input_mhc_rot_532x_20220614_GHK_0.9.8h_Py3.7.dat
--rw-r--r--   0        0        0     3191 2022-10-24 11:26:56.353628 gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK.py
--rw-r--r--   0        0        0     8302 2022-10-24 11:26:56.381626 gfatpy-0.1.0/gfatpy/lidar/depolarization/calibration.py
--rw-r--r--   0        0        0     2554 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization.py
--rw-r--r--   0        0        0     1414 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
--rw-r--r--   0        0        0     9744 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
--rw-r--r--   0        0        0      913 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
--rw-r--r--   0        0        0      931 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/io.py
--rw-r--r--   0        0        0     5577 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/lidar_merge.py
--rw-r--r--   0        0        0     5239 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/retrieval.py
--rw-r--r--   0        0        0     1949 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/depolarization/utils.py
--rw-r--r--   0        0        0     8873 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/file_manager.py
--rw-r--r--   0        0        0     3800 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/info.yml
--rw-r--r--   0        0        0     2042 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/lidar/plot/info.yml
--rw-r--r--   0        0        0      168 2022-09-29 12:34:07.125117 gfatpy-0.1.0/gfatpy/lidar/plot/profile.py
--rw-r--r--   0        0        0    20205 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/plot/quicklook.py
--rw-r--r--   0        0        0     2299 2022-10-24 11:26:56.385626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/__init__.py
--rw-r--r--   0        0        0     1931 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
--rw-r--r--   0        0        0     3364 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
--rw-r--r--   0        0        0    11195 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
--rw-r--r--   0        0        0     2958 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
--rw-r--r--   0        0        0    21456 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
--rw-r--r--   0        0        0     3346 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
--rw-r--r--   0        0        0    11823 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
--rw-r--r--   0        0        0    14976 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
--rw-r--r--   0        0        0    31668 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_zerobin_triggerdelay_binshift.py
--rw-r--r--   0        0        0    28048 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/preprocessing/study_dead_time.py
--rw-r--r--   0        0        0     1064 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/common.py
--rw-r--r--   0        0        0        0 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/dark_measurement.py
--rw-r--r--   0        0        0    20617 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/depolarization.py
--rw-r--r--   0        0        0     3314 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/io.py
--rw-r--r--   0        0        0     4953 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/plot.py
--rw-r--r--   0        0        0    13357 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
--rw-r--r--   0        0        0    19932 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/quality_assurance/telecover.py
--rw-r--r--   0        0        0       29 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/.gitignore
--rw-r--r--   0        0        0       96 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/README.md
--rw-r--r--   0        0        0      612 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/raw2l1/__init__.py
--rw-r--r--   0        0        0      111 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_asus.yaml
--rw-r--r--   0        0        0      119 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_asus_test.yaml
--rw-r--r--   0        0        0       78 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_default.yaml
--rw-r--r--   0        0        0      112 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_jaba_workbench.yaml
--rw-r--r--   0        0        0       97 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server.yaml
--rw-r--r--   0        0        0       88 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server_asus.yaml
--rw-r--r--   0        0        0       79 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server_fizhome.yaml
--rw-r--r--   0        0        0       79 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server_fiziista.yaml
--rw-r--r--   0        0        0       97 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server_provisional.yaml
--rw-r--r--   0        0        0      109 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/config/config_server_test.yaml
--rw-r--r--   0        0        0    22413 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/raw2l1/lidar_raw2l1.py
--rw-r--r--   0        0        0     7447 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/CHANGELOG
--rw-r--r--   0        0        0    35141 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/LICENSE
--rw-r--r--   0        0        0     2163 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/README.md
--rw-r--r--   0        0        0     2982 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_jenoptik_chm15k.ini
--rw-r--r--   0        0        0     8100 2022-09-29 12:34:07.129117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_eprofile.ini
--rw-r--r--   0        0        0     8136 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_toprof_netcdf4.ini
--rw-r--r--   0        0        0    13099 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_mhc_prod.ini
--rw-r--r--   0        0        0    10689 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_pd.ini
--rw-r--r--   0        0        0    12848 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_ff.ini
--rw-r--r--   0        0        0    12448 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_nf.ini
--rw-r--r--   0        0        0    12680 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_ff.ini
--rw-r--r--   0        0        0    12304 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_nf.ini
--rw-r--r--   0        0        0     9993 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_MULHACEN.ini
--rw-r--r--   0        0        0     8233 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_VELETA.ini
--rw-r--r--   0        0        0     6934 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l1-tb_toprof_netcdf4.ini
--rw-r--r--   0        0        0     4570 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l2-ta_toprof_netcdf4.ini
--rw-r--r--   0        0        0     7576 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l1-tb_toprof_netcdf4.ini
--rw-r--r--   0        0        0     6101 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-clwvi_toprof_netcdf4.ini
--rw-r--r--   0        0        0     4872 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-hua_toprof_netcdf4.ini
--rw-r--r--   0        0        0     5309 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-prw_toprof_netcdf4.ini
--rw-r--r--   0        0        0     4845 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-ta_toprof_netcdf4.ini
--rw-r--r--   0        0        0     6771 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/Makefile
--rw-r--r--   0        0        0     6710 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/make.bat
--rw-r--r--   0        0        0       84 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/_templates/layout.html
--rw-r--r--   0        0        0    12769 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/conf.py
--rw-r--r--   0        0        0     3435 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/configuration.rst
--rw-r--r--   0        0        0     2047 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/images/logo_sirta_navbar.png
--rw-r--r--   0        0        0     1180 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/index.rst
--rw-r--r--   0        0        0     1979 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/prerequisites.rst
--rw-r--r--   0        0        0       80 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/readers.rst
--rw-r--r--   0        0        0       94 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/running.rst
--rw-r--r--   0        0        0     3170 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/raw2l1.py
--rw-r--r--   0        0        0       24 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/.gitignore
--rw-r--r--   0        0        0       24 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/__init__.py
--rw-r--r--   0        0        0    13305 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/campbellscientific_cs135.py
--rw-r--r--   0        0        0    12353 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10min.py
--rw-r--r--   0        0        0    11741 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10s.py
--rw-r--r--   0        0        0    11983 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_10min.py
--rw-r--r--   0        0        0    12158 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_1s.py
--rw-r--r--   0        0        0        0 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/__init__.py
--rw-r--r--   0        0        0      753 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/libvaisala.py
--rw-r--r--   0        0        0      733 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/libhatpro.py
--rw-r--r--   0        0        0    19875 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus-uk-metoffice.py
--rw-r--r--   0        0        0    24741 2022-09-29 12:34:07.133117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus.py
--rw-r--r--   0        0        0    19006 2022-10-18 10:37:23.936225 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_DMC.py
--rw-r--r--   0        0        0    28598 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh.py
--rw-r--r--   0        0        0    21732 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh_test.py
--rw-r--r--   0        0        0    39567 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_lidar.py
--rw-r--r--   0        0        0    21989 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_mhc.py
--rw-r--r--   0        0        0    19355 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_vlt.py
--rw-r--r--   0        0        0     3564 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_absolute_humidity.py
--rw-r--r--   0        0        0     3453 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp.py
--rw-r--r--   0        0        0     3511 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp_bl.py
--rw-r--r--   0        0        0     7263 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature.py
--rw-r--r--   0        0        0     7158 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature_bl.py
--rw-r--r--   0        0        0     3788 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_clwvi.py
--rw-r--r--   0        0        0     3425 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_prw.py
--rw-r--r--   0        0        0    14613 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/sigmaspace_minimpl.py
--rw-r--r--   0        0        0      302 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/test_reader.py
--rw-r--r--   0        0        0      186 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/run_unittests.sh
--rw-r--r--   0        0        0     2396 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_arg_parser.py
--rw-r--r--   0        0        0     1401 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus-uk-metoffice.py
--rw-r--r--   0        0        0    10780 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus.py
--rw-r--r--   0        0        0     2680 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_cs135.py
--rw-r--r--   0        0        0    13604 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls7.py
--rw-r--r--   0        0        0     5027 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls70.py
--rw-r--r--   0        0        0     2280 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_lidar_reader.py
--rw-r--r--   0        0        0     1111 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_logs.py
--rw-r--r--   0        0        0     1796 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_netcdf4.py
--rw-r--r--   0        0        0     5879 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_rpg_hatpro.py
--rw-r--r--   0        0        0     1694 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_sigmaspace_minimpl.py
--rw-r--r--   0        0        0     2522 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_toprof_format.py
--rw-r--r--   0        0        0     8369 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala.py
--rw-r--r--   0        0        0     8207 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_eprofile.py
--rw-r--r--   0        0        0     1726 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_sirta.py
--rw-r--r--   0        0        0       24 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/__init__.py
--rw-r--r--   0        0        0     5967 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/arg_parser.py
--rw-r--r--   0        0        0     3330 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/check_conf.py
--rw-r--r--   0        0        0      740 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/common.py
--rw-r--r--   0        0        0     1449 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/conf.py
--rw-r--r--   0        0        0    18917 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/create_netcdf.py
--rw-r--r--   0        0        0     4200 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/lidar_reader.py
--rw-r--r--   0        0        0     2287 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/log.py
--rw-r--r--   0        0        0      733 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/read_overlap.py
--rw-r--r--   0        0        0      826 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/utils.py
--rw-r--r--   0        0        0      163 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/requirements.txt
--rw-r--r--   0        0        0      687 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_ASUS.sh
--rw-r--r--   0        0        0      657 2022-09-29 12:34:07.137117 gfatpy-0.1.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_SERVER.sh
--rw-r--r--   0        0        0    10850 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/reader.py
--rw-r--r--   0        0        0        0 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/retrieval/__init__.py
--rw-r--r--   0        0        0     3563 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/retrieval/helper.py
--rw-r--r--   0        0        0     2726 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/retrieval/klett.py
--rw-r--r--   0        0        0     5145 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
--rw-r--r--   0        0        0        0 2022-09-29 12:34:07.141117 gfatpy-0.1.0/gfatpy/lidar/retrieval/number_concentration.py
--rw-r--r--   0        0        0    10584 2022-10-24 11:26:56.389626 gfatpy-0.1.0/gfatpy/lidar/retrieval/raman.py
--rw-r--r--   0        0        0     1488 2022-10-24 11:26:56.393626 gfatpy-0.1.0/gfatpy/lidar/types.py
--rw-r--r--   0        0        0     8966 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/lidar/utils.py
--rw-r--r--   0        0        0       34 2022-09-29 12:34:07.141117 gfatpy-0.1.0/gfatpy/utils/__init__.py
--rw-r--r--   0        0        0     3415 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/utils/calibration.py
--rw-r--r--   0        0        0      253 2022-09-29 12:34:07.141117 gfatpy-0.1.0/gfatpy/utils/io.py
--rw-r--r--   0        0        0     1584 2022-10-24 11:26:56.393626 gfatpy-0.1.0/gfatpy/utils/optimized.py
--rw-r--r--   0        0        0     6664 2022-10-24 11:26:56.393626 gfatpy-0.1.0/gfatpy/utils/plot.py
--rw-r--r--   0        0        0    10252 2022-10-24 11:27:16.064802 gfatpy-0.1.0/gfatpy/utils/utils.py
--rw-r--r--   0        0        0     1291 2022-10-24 11:38:23.348838 gfatpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 gfatpy-0.1.0/setup.py
--rw-r--r--   0        0        0     1415 1970-01-01 00:00:00.000000 gfatpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1470 2023-01-19 15:14:33.615682 gfatpy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2704 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/__init__.py
+-rw-r--r--   0        0        0     1077 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/__init__.py
+-rw-r--r--   0        0        0      710 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/aeronet4lidar.py
+-rw-r--r--   0        0        0     1053 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/info.yml
+-rw-r--r--   0        0        0    17421 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/plot.py
+-rw-r--r--   0        0        0     3965 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/reader.py
+-rw-r--r--   0        0        0     8805 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/aeronet/typing.py
+-rw-r--r--   0        0        0    16772 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/aeronet/utils.py
+-rw-r--r--   0        0        0    28725 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/assets/LOGO_GFAT_150pp.png
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/atmo/__init__.py
+-rw-r--r--   0        0        0    22274 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/atmo/atmo.py
+-rw-r--r--   0        0        0     4984 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/atmo/ecmwf.py
+-rw-r--r--   0        0        0    74896 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/atmo/solar.py
+-rw-r--r--   0        0        0     4466 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/cli/lidar/main.py
+-rw-r--r--   0        0        0     1183 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cli/lidar/plot/main.py
+-rw-r--r--   0        0        0      896 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cli/main.py
+-rw-r--r--   0        0        0      270 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cloudnet/__init__.py
+-rw-r--r--   0        0        0     8810 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cloudnet/cloud_model.py
+-rw-r--r--   0        0        0       49 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cloudnet/info.yml
+-rw-r--r--   0        0        0     4600 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cloudnet/plot_deprecated.py
+-rw-r--r--   0        0        0     5423 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/cloudnet/reader.py
+-rw-r--r--   0        0        0    18059 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/cloudnet/utils.py
+-rw-r--r--   0        0        0     1099 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/config.py
+-rw-r--r--   0        0        0       70 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/constants.py
+-rw-r--r--   0        0        0      333 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/__init__.py
+-rw-r--r--   0        0        0      174 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/.hg_archival.txt
+-rw-r--r--   0        0        0      121 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/.hgignore
+-rw-r--r--   0        0        0      570 2023-01-19 15:14:33.615682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/.hgtags
+-rw-r--r--   0        0        0  2508885 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf
+-rw-r--r--   0        0        0     2541 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md
+-rw-r--r--   0        0        0   179833 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py
+-rw-r--r--   0        0        0   793573 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf
+-rw-r--r--   0        0        0    13468 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/LICENSE.md
+-rw-r--r--   0        0        0     1628 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/README.md
+-rw-r--r--   0        0        0      108 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/requirements.txt
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/__init__.py
+-rw-r--r--   0        0        0     7453 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py
+-rw-r--r--   0        0        0     7455 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py
+-rw-r--r--   0        0        0     7390 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py
+-rw-r--r--   0        0        0    11034 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py
+-rw-r--r--   0        0        0    10931 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py
+-rw-r--r--   0        0        0    11059 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py
+-rw-r--r--   0        0        0     3352 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/tests/datos/MULHACEN/QA/GHK/2022/10/04/output_optic_input_mhc_rot_532x_20220614_GHK_0.9.8h_Py3.7.dat
+-rw-r--r--   0        0        0     3191 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK.py
+-rw-r--r--   0        0        0    13582 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/calibration.py
+-rw-r--r--   0        0        0     1463 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/depolarization_calibration_alh.py
+-rw-r--r--   0        0        0     9744 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py
+-rw-r--r--   0        0        0      913 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py
+-rw-r--r--   0        0        0     1205 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/io.py
+-rw-r--r--   0        0        0     5577 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/old_lidar_merge_2bremoved.py
+-rw-r--r--   0        0        0     4946 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/depolarization/plot.py
+-rw-r--r--   0        0        0    14902 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/retrieval.py
+-rw-r--r--   0        0        0     1949 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/depolarization/utils.py
+-rw-r--r--   0        0        0    10455 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/file_manager.py
+-rw-r--r--   0        0        0     4820 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/info.yml
+-rw-r--r--   0        0        0     3792 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/nc_convert/configs/ALHAMBRA.toml
+-rw-r--r--   0        0        0      837 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/nc_convert/configs/MULHACEN.toml
+-rw-r--r--   0        0        0     8066 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/nc_convert/converter.py
+-rw-r--r--   0        0        0      219 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/nc_convert/types.py
+-rw-r--r--   0        0        0     2042 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/plot/info.yml
+-rw-r--r--   0        0        0      168 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/plot/profile.py
+-rw-r--r--   0        0        0    20385 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/lidar/plot/quicklook.py
+-rw-r--r--   0        0        0     2299 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1931 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py
+-rw-r--r--   0        0        0     3364 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py
+-rw-r--r--   0        0        0     2509 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/preprocessing/gluing_proportional.py
+-rw-r--r--   0        0        0    11195 2023-04-01 21:13:27.762405 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_dead_time.py
+-rw-r--r--   0        0        0     2958 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py
+-rw-r--r--   0        0        0    21456 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py
+-rw-r--r--   0        0        0     3346 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py
+-rw-r--r--   0        0        0    12078 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py
+-rw-r--r--   0        0        0    14976 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py
+-rw-r--r--   0        0        0    31668 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_zerobin_triggerdelay_binshift.py
+-rw-r--r--   0        0        0    28048 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/preprocessing/study_dead_time.py
+-rw-r--r--   0        0        0     1064 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/common.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/dark_measurement.py
+-rw-r--r--   0        0        0    20617 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/depolarization.py
+-rw-r--r--   0        0        0     3314 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/io.py
+-rw-r--r--   0        0        0     5083 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/plot.py
+-rw-r--r--   0        0        0    13385 2023-04-18 20:42:02.824928 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py
+-rw-r--r--   0        0        0    19932 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/quality_assurance/telecover.py
+-rw-r--r--   0        0        0       29 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/.gitignore
+-rw-r--r--   0        0        0       96 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/README.md
+-rw-r--r--   0        0        0      612 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/__init__.py
+-rw-r--r--   0        0        0      111 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_asus.yaml
+-rw-r--r--   0        0        0      119 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_asus_test.yaml
+-rw-r--r--   0        0        0       78 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_default.yaml
+-rw-r--r--   0        0        0      112 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_jaba_workbench.yaml
+-rw-r--r--   0        0        0       97 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server.yaml
+-rw-r--r--   0        0        0       88 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server_asus.yaml
+-rw-r--r--   0        0        0       79 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server_fizhome.yaml
+-rw-r--r--   0        0        0       79 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server_fiziista.yaml
+-rw-r--r--   0        0        0       97 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server_provisional.yaml
+-rw-r--r--   0        0        0      109 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/config/config_server_test.yaml
+-rw-r--r--   0        0        0    22413 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/lidar/raw2l1/lidar_raw2l1.py
+-rw-r--r--   0        0        0     7447 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/CHANGELOG
+-rw-r--r--   0        0        0    35141 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/LICENSE
+-rw-r--r--   0        0        0     2163 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/README.md
+-rw-r--r--   0        0        0     2982 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_jenoptik_chm15k.ini
+-rw-r--r--   0        0        0     8100 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_eprofile.ini
+-rw-r--r--   0        0        0     8136 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_toprof_netcdf4.ini
+-rw-r--r--   0        0        0    13099 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_mhc_prod.ini
+-rw-r--r--   0        0        0    10689 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_pd.ini
+-rw-r--r--   0        0        0    12848 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_ff.ini
+-rw-r--r--   0        0        0    12448 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_nf.ini
+-rw-r--r--   0        0        0    12680 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_ff.ini
+-rw-r--r--   0        0        0    12304 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_nf.ini
+-rw-r--r--   0        0        0     9993 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_MULHACEN.ini
+-rw-r--r--   0        0        0     8233 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_VELETA.ini
+-rw-r--r--   0        0        0     6934 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l1-tb_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     4570 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l2-ta_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     7576 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l1-tb_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     6101 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-clwvi_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     4872 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-hua_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     5309 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-prw_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     4845 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-ta_toprof_netcdf4.ini
+-rw-r--r--   0        0        0     6771 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/Makefile
+-rw-r--r--   0        0        0     6710 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/make.bat
+-rw-r--r--   0        0        0       84 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/_templates/layout.html
+-rw-r--r--   0        0        0    12769 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/conf.py
+-rw-r--r--   0        0        0     3435 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/configuration.rst
+-rw-r--r--   0        0        0     2047 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/images/logo_sirta_navbar.png
+-rw-r--r--   0        0        0     1180 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/index.rst
+-rw-r--r--   0        0        0     1979 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/prerequisites.rst
+-rw-r--r--   0        0        0       80 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/readers.rst
+-rw-r--r--   0        0        0       94 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/running.rst
+-rw-r--r--   0        0        0     3170 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/raw2l1.py
+-rw-r--r--   0        0        0       24 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/.gitignore
+-rw-r--r--   0        0        0       24 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/__init__.py
+-rw-r--r--   0        0        0    13305 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/campbellscientific_cs135.py
+-rw-r--r--   0        0        0    12353 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10min.py
+-rw-r--r--   0        0        0    11741 2023-01-19 15:14:33.625682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10s.py
+-rw-r--r--   0        0        0    11983 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_10min.py
+-rw-r--r--   0        0        0    12158 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_1s.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/__init__.py
+-rw-r--r--   0        0        0      753 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/libvaisala.py
+-rw-r--r--   0        0        0      733 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/libhatpro.py
+-rw-r--r--   0        0        0    19875 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus-uk-metoffice.py
+-rw-r--r--   0        0        0    24741 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus.py
+-rw-r--r--   0        0        0    19006 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_DMC.py
+-rw-r--r--   0        0        0    28598 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh.py
+-rw-r--r--   0        0        0    21732 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh_test.py
+-rw-r--r--   0        0        0    39567 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_lidar.py
+-rw-r--r--   0        0        0    21989 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_mhc.py
+-rw-r--r--   0        0        0    19355 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_vlt.py
+-rw-r--r--   0        0        0     3564 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_absolute_humidity.py
+-rw-r--r--   0        0        0     3453 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp.py
+-rw-r--r--   0        0        0     3511 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp_bl.py
+-rw-r--r--   0        0        0     7263 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature.py
+-rw-r--r--   0        0        0     7158 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature_bl.py
+-rw-r--r--   0        0        0     3788 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_clwvi.py
+-rw-r--r--   0        0        0     3425 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_prw.py
+-rw-r--r--   0        0        0    14613 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/sigmaspace_minimpl.py
+-rw-r--r--   0        0        0      302 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/test_reader.py
+-rw-r--r--   0        0        0      186 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/run_unittests.sh
+-rw-r--r--   0        0        0     2396 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_arg_parser.py
+-rw-r--r--   0        0        0     1401 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus-uk-metoffice.py
+-rw-r--r--   0        0        0    10780 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus.py
+-rw-r--r--   0        0        0     2680 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_cs135.py
+-rw-r--r--   0        0        0    13604 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls7.py
+-rw-r--r--   0        0        0     5027 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls70.py
+-rw-r--r--   0        0        0     2280 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_lidar_reader.py
+-rw-r--r--   0        0        0     1111 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_logs.py
+-rw-r--r--   0        0        0     1796 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_netcdf4.py
+-rw-r--r--   0        0        0     5879 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_rpg_hatpro.py
+-rw-r--r--   0        0        0     1694 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_sigmaspace_minimpl.py
+-rw-r--r--   0        0        0     2522 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_toprof_format.py
+-rw-r--r--   0        0        0     8369 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala.py
+-rw-r--r--   0        0        0     8207 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_eprofile.py
+-rw-r--r--   0        0        0     1726 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_sirta.py
+-rw-r--r--   0        0        0       24 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/__init__.py
+-rw-r--r--   0        0        0     5967 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/arg_parser.py
+-rw-r--r--   0        0        0     3330 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/check_conf.py
+-rw-r--r--   0        0        0      740 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/common.py
+-rw-r--r--   0        0        0     1449 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/conf.py
+-rw-r--r--   0        0        0    18917 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/create_netcdf.py
+-rw-r--r--   0        0        0     4200 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/lidar_reader.py
+-rw-r--r--   0        0        0     2287 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/log.py
+-rw-r--r--   0        0        0      733 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/read_overlap.py
+-rw-r--r--   0        0        0      826 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/utils.py
+-rw-r--r--   0        0        0      163 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/requirements.txt
+-rw-r--r--   0        0        0      687 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_ASUS.sh
+-rw-r--r--   0        0        0      657 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_SERVER.sh
+-rw-r--r--   0        0        0    10850 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/reader.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/retrieval/__init__.py
+-rw-r--r--   0        0        0     3563 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/retrieval/helper.py
+-rw-r--r--   0        0        0     2774 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/lidar/retrieval/klett.py
+-rw-r--r--   0        0        0     5145 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/retrieval/lidar_layer_detection.py
+-rw-r--r--   0        0        0        0 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/lidar/retrieval/number_concentration.py
+-rw-r--r--   0        0        0    10624 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/lidar/retrieval/raman.py
+-rw-r--r--   0        0        0     1559 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/lidar/types.py
+-rw-r--r--   0        0        0     8966 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/lidar/utils.py
+-rw-r--r--   0        0        0      244 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/__init__.py
+-rw-r--r--   0        0        0      101 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/info.yml
+-rw-r--r--   0        0        0        0 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/plot/info.yml
+-rw-r--r--   0        0        0     3013 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/plot/quicklook.py
+-rw-r--r--   0        0        0     2225 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/reader.py
+-rw-r--r--   0        0        0    61357 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/0.C_24.1GHz.csv
+-rw-r--r--   0        0        0    61200 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/0.C_35.5GHz.csv
+-rw-r--r--   0        0        0    60964 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/0.C_94.0GHz.csv
+-rw-r--r--   0        0        0    61372 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/10C_24.1GHz.csv
+-rw-r--r--   0        0        0    61213 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/10C_35.5GHz.csv
+-rw-r--r--   0        0        0    60965 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/10C_94.0GHz.csv
+-rw-r--r--   0        0        0    60528 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/20C_24.1GHz.csv
+-rw-r--r--   0        0        0    61215 2023-04-18 20:35:42.535626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/20C_35.5GHz.csv
+-rw-r--r--   0        0        0    60984 2023-04-18 20:35:42.545626 gfatpy-0.3.0/gfatpy/radar/scattering_databases/20C_94.0GHz.csv
+-rw-r--r--   0        0        0     1305 2023-04-18 20:35:42.545626 gfatpy-0.3.0/gfatpy/radar/types.py
+-rw-r--r--   0        0        0     5853 2023-04-18 20:35:42.545626 gfatpy-0.3.0/gfatpy/radar/utils.py
+-rw-r--r--   0        0        0       34 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/utils/__init__.py
+-rw-r--r--   0        0        0     9654 2023-04-01 21:12:28.922411 gfatpy-0.3.0/gfatpy/utils/calibration.py
+-rw-r--r--   0        0        0     1015 2023-04-18 20:35:42.545626 gfatpy-0.3.0/gfatpy/utils/io.py
+-rw-r--r--   0        0        0     2452 2023-01-21 00:31:29.908872 gfatpy-0.3.0/gfatpy/utils/optimized.py
+-rw-r--r--   0        0        0     6664 2023-01-19 15:14:33.635682 gfatpy-0.3.0/gfatpy/utils/plot.py
+-rw-r--r--   0        0        0    13333 2023-04-18 20:55:26.084565 gfatpy-0.3.0/gfatpy/utils/utils.py
+-rw-r--r--   0        0        0     1472 2023-04-26 04:34:55.939597 gfatpy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2524 1970-01-01 00:00:00.000000 gfatpy-0.3.0/setup.py
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 gfatpy-0.3.0/PKG-INFO
```

### Comparing `gfatpy-0.1.0/LICENSE` & `gfatpy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/__init__.py` & `gfatpy-0.3.0/gfatpy/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/__init__.py` & `gfatpy-0.3.0/gfatpy/aeronet/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/aeronet4lidar.py` & `gfatpy-0.3.0/gfatpy/aeronet/aeronet4lidar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/info.yml` & `gfatpy-0.3.0/gfatpy/aeronet/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/plot.py` & `gfatpy-0.3.0/gfatpy/aeronet/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/reader.py` & `gfatpy-0.3.0/gfatpy/aeronet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/typing.py` & `gfatpy-0.3.0/gfatpy/aeronet/typing.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/aeronet/utils.py` & `gfatpy-0.3.0/gfatpy/aeronet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/assets/LOGO_GFAT_150pp.png` & `gfatpy-0.3.0/gfatpy/assets/LOGO_GFAT_150pp.png`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/atmo/atmo.py` & `gfatpy-0.3.0/gfatpy/atmo/atmo.py`

 * *Files 12% similar despite different names*

```diff
@@ -153,28 +153,66 @@
     532.075: 1.04007,
     710: 1.03919,
     800: 1.03897,
     1064: 1.03863,
     1064.150: 1.03863,
 }
 
+molecular_depolarizationC = {
+    351: 0.004158,
+    354.717: 0.003959,
+    355: 0.003956,
+    400: 0.003825,
+    510.6: 0.003673,
+    532: 0.003656,
+    532.075: 0.003656,
+    710: 0.003575,
+    800: 0.003555,
+    1064: 0.003524,
+    1064.150: 0.003524,
+}
+
+molecular_depolarizationT = {
+    351: 0.01559,
+    354.717: 0.01554,
+    355: 0.01554,
+    400: 0.01507,
+    510.6: 0.01448,
+    532: 0.01441,
+    532.075: 0.01441,
+    710: 0.01410,
+    800: 0.01402,
+    1064: 0.01390,
+    1064.150: 0.01390,
+}
+
 # Create interpolation function once, to avoid re-calculation (does it matter?)
 f_ext = interpolate.interp1d(list(Cs.keys()), list(Cs.values()), kind="cubic")
 f_bst = interpolate.interp1d(list(BsT.keys()), list(BsT.values()), kind="cubic")
 f_bsc = interpolate.interp1d(list(BsC.keys()), list(BsC.values()), kind="cubic")
 f_bsc_parallel = interpolate.interp1d(
     list(BsC_parallel.keys()), list(BsC_parallel.values()), kind="cubic"
 )
 f_bsc_perpendicular = interpolate.interp1d(
     list(BsC_perpendicular.keys()), list(BsC_perpendicular.values()), kind="cubic"
 )
 
 # Splines introduce arifacts due to limited input resolution
 f_kbwt = interpolate.interp1d(list(KbwT.keys()), list(KbwT.values()), kind="linear")
 f_kbwc = interpolate.interp1d(list(KbwC.keys()), list(KbwC.values()), kind="linear")
+f_molt = interpolate.interp1d(
+    list(molecular_depolarizationT.keys()),
+    list(molecular_depolarizationT.values()),
+    kind="linear",
+)
+f_molc = interpolate.interp1d(
+    list(molecular_depolarizationC.keys()),
+    list(molecular_depolarizationC.values()),
+    kind="linear",
+)
 
 
 def standard_atmosphere(
     altitude: float,
     temperature_surface: float = 288.15,
     pressure_surface: float = 101325.0,
 ) -> tuple[float, float, float]:
@@ -398,81 +436,14 @@
     """
 
     delta_height = np.median(np.diff(heights))
     integrated_extinction = scipy.integrate.cumtrapz(alpha, initial=0, dx=delta_height)
     return np.exp(-integrated_extinction)
 
 
-def molecular_properties(
-    wavelength: float,
-    pressure: np.ndarray[Any, np.dtype[np.float64]],
-    temperature: np.ndarray[Any, np.dtype[np.float64]],
-    heights: np.ndarray[Any, np.dtype[np.float64]],
-    times: np.ndarray[Any, np.dtype[np.float64]] | None = None,
-    component: str = "total",
-) -> xr.Dataset:
-    """
-    Molecular Attenuated  Backscatter: beta_mol_att = beta_mol * Transmittance**2
-
-    Parameters
-    ----------
-    wavelength: int, float
-        wavelength of our desired beta molecular attenuated
-    pressure: array
-        pressure profile
-    temperature: array
-        temperature profile
-    heights: array
-        heights profile
-    times: array
-        times profile
-
-    Returns
-    -------
-    beta_molecular_att: array
-        molecular attenuated backscatter profile
-    """
-
-    # molecular backscatter and extinction #
-    beta_mol = molecular_backscatter(
-        wavelength, pressure, temperature, component=component
-    )
-    alfa_mol = molecular_extinction(wavelength, pressure, temperature)
-    lr_mol = molecular_lidar_ratio(wavelength)
-
-    """ transmittance """
-    transmittance_array = transmittance(alfa_mol, heights)
-
-    """ attenuated molecular backscatter """
-    att_beta_mol = attenuated_backscatter(beta_mol, transmittance_array)
-
-    set_trace()
-    if times is None:
-        mol_properties = xr.Dataset(
-            {
-                "molecular_beta": (["range"], beta_mol),
-                "molecular_alpha": (["range"], alfa_mol),
-                "attenuated_molecular_beta": (["range"], att_beta_mol),
-                "molecular_lidar_ratio": lr_mol,
-            },
-            coords={"range": heights},
-        )
-    else:
-        mol_properties = xr.Dataset(
-            {
-                "molecular_beta": (["time", "range"], beta_mol),
-                "molecular_alpha": (["time", "range"], alfa_mol),
-                "attenuated_molecular_beta": (["time", "range"], att_beta_mol),
-                "molecular_lidar_ratio": ([], lr_mol),
-            },
-            coords={"time": times, "range": heights},
-        )
-    return mol_properties
-
-
 def molecular_backscatter(
     wavelength: float,
     pressure: np.ndarray[Any, np.dtype[np.float64]],
     temperature: np.ndarray[Any, np.dtype[np.float64]],
     component: str = "total",
 ) -> np.ndarray[Any, np.dtype[np.float64]]:
     """
@@ -565,14 +536,50 @@
     Kbw = k_function(wavelength)
 
     lidar_ratio_molecular = 8 * np.pi / 3.0 * Kbw
 
     return lidar_ratio_molecular
 
 
+def molecular_depolarization(wavelength: float, component: str = "total") -> float:
+    """
+    Molecular lidar ratio.
+
+    Parameters
+    ----------
+    wavelength : float
+       The wavelength of the radiation in air. From 308 to 1064.15
+    component : str
+       One of 'total' or 'cabannes'.
+
+    Returns
+    -------
+    molecular volume depolarization: float
+
+    References
+    ----------
+    Freudenthaler, V. Rayleigh scattering coefficients and linear depolarization
+    ratios at several EARLINET lidar wavelengths. p.6-7 (2015)
+    """
+
+    if component not in ["total", "cabannes"]:
+        raise ValueError(
+            "Molecular lidar ratio available only for 'total' or 'cabannes' component."
+        )
+
+    if component == "total":
+        moldepo_function = f_molt
+    else:
+        moldepo_function = f_molc
+
+    molecular_depolarization = moldepo_function(wavelength)
+
+    return molecular_depolarization
+
+
 def molecular_extinction(
     wavelength: float,
     pressure: np.ndarray[Any, np.dtype[np.float64]],
     temperature: np.ndarray[Any, np.dtype[np.float64]],
 ) -> np.ndarray[Any, np.dtype[np.float64]]:
     """
     Molecular extinction calculation.
@@ -643,14 +650,84 @@
     # p_pa = pressure * 100.  # Pressure in pascal
 
     n = pressure / (temperature * k_b)
 
     return n
 
 
+def molecular_properties(
+    wavelength: float,
+    pressure: np.ndarray[Any, np.dtype[np.float64]],
+    temperature: np.ndarray[Any, np.dtype[np.float64]],
+    heights: np.ndarray[Any, np.dtype[np.float64]],
+    times: np.ndarray[Any, np.dtype[np.float64]] | None = None,
+    component: str = "total",
+) -> xr.Dataset:
+    """
+    Molecular Attenuated  Backscatter: beta_mol_att = beta_mol * Transmittance**2
+
+    Parameters
+    ----------
+    wavelength: int, float
+        wavelength of our desired beta molecular attenuated
+    pressure: array
+        pressure profile
+    temperature: array
+        temperature profile
+    heights: array
+        heights profile
+    times: array
+        times profile
+
+    Returns
+    -------
+        xarray.dataset: molecular attenuated backscatter profile, molecular backscatter profile, molecular extinction profile, molecular lidar ratio, molecular depolarization ratio
+    """
+
+    # molecular backscatter and extinction #
+    beta_mol = molecular_backscatter(
+        wavelength, pressure, temperature, component=component
+    )
+    alfa_mol = molecular_extinction(wavelength, pressure, temperature)
+    lr_mol = molecular_lidar_ratio(wavelength, component=component)
+
+    depo_mol = molecular_depolarization(wavelength, component=component)
+
+    """ transmittance """
+    transmittance_array = transmittance(alfa_mol, heights)
+
+    """ attenuated molecular backscatter """
+    att_beta_mol = attenuated_backscatter(beta_mol, transmittance_array)
+
+    set_trace()
+    if times is None:
+        mol_properties = xr.Dataset(
+            {
+                "molecular_beta": (["range"], beta_mol),
+                "molecular_alpha": (["range"], alfa_mol),
+                "attenuated_molecular_beta": (["range"], att_beta_mol),
+                "molecular_lidar_ratio": lr_mol,
+                "molecular_depolarization": depo_mol,
+            },
+            coords={"range": heights},
+        )
+    else:
+        mol_properties = xr.Dataset(
+            {
+                "molecular_beta": (["time", "range"], beta_mol),
+                "molecular_alpha": (["time", "range"], alfa_mol),
+                "attenuated_molecular_beta": (["time", "range"], att_beta_mol),
+                "molecular_lidar_ratio": ([], lr_mol),
+                "molecular_depolarization": depo_mol,
+            },
+            coords={"time": times, "range": heights},
+        )
+    return mol_properties
+
+
 def extrapolate_aod(
     wv1: float,
     wv2: float,
     aod2: np.ndarray[Any, np.dtype[np.float64]],
     ae: float,
 ) -> np.ndarray[Any, np.dtype[np.float64]]:
     """_summary_
```

### Comparing `gfatpy-0.1.0/gfatpy/atmo/ecmwf.py` & `gfatpy-0.3.0/gfatpy/atmo/ecmwf.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,26 @@
     Raises:
         FileNotFoundError: There is no available data in the ECMWF data
 
     Returns:
         xr.Dataset: x array dataset with variables: ["pressure", "temperature", "height", "time"]
     """
     _date = parse_datetime(date)
+
     response_filename = requests.get(
         f"{API_URL}/model-files",
         params={**BASE_QUERY_PARAMS, "date": _date.date().isoformat()},
-    ).json()
+    )
+
+    if not response_filename.ok:
+        raise RuntimeError(
+            f"Request returned code {response_filename.status_code}: {response_filename.text}"
+        )
+
+    response_filename = response_filename.json()
 
     if len(response_filename) == 0:
         raise FileNotFoundError("No data found for the given day")
 
     file = requests.get(response_filename[0]["downloadUrl"])
     nc = Dataset("ecmwf.nc", memory=file.content)
     dataset = xr.open_dataset(xr.backends.NetCDF4DataStore(nc))  # type: ignore
```

### Comparing `gfatpy-0.1.0/gfatpy/atmo/solar.py` & `gfatpy-0.3.0/gfatpy/atmo/solar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cli/lidar/main.py` & `gfatpy-0.3.0/gfatpy/cli/lidar/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import pathlib
 from datetime import datetime
 from typing import Optional
 from pathlib import Path
 
 import typer
 
-from gfatpy.lidar.types import LidarName, MeasurementType
+from gfatpy.lidar.types import LidarName, MeasurementType, Telescope
 from gfatpy.lidar.raw2l1.lidar_raw2l1 import lidar_raw2l1
+from gfatpy.lidar.nc_convert.converter import convert_nc_by_date
 from gfatpy.lidar.reader import reader_xarray
 from gfatpy.lidar.quality_assurance.rayleigh_fit import rayleigh_fit_from_date
 
+
 app = typer.Typer(no_args_is_help=True)
 
 
 @app.command(
     help="Converts raw lidar data to l1 data",
     no_args_is_help=True,
 )
@@ -34,14 +36,37 @@
         data_dir,
         measurement_type,
         initial_date,
         final_date,
         overwrite,
     )
 
+@app.command(no_args_is_help=True)
+def nc_convert(
+    lidar_name: LidarName = typer.Option(..., "--lidar", "-l"),
+    initial_date: datetime = typer.Option(..., "--initial-date", "-i"),
+    data_dir: Path = typer.Option(
+        ..., "--data-dir", "-d", readable=True, dir_okay=True, file_okay=False
+    ),
+    measurement_type: Optional[MeasurementType] = typer.Option(
+        None, "--measurement-type", "-t"
+    ),
+    telescope: Optional[Telescope] = typer.Option(
+        Telescope.xf, "--telescope"
+    )
+    
+    # final_date: Optional[datetime] = typer.Option(None, "--final-date", "-f"), TODO: If necessary implement this
+):
+    convert_nc_by_date(
+        lidar_name=lidar_name,
+        date = initial_date,
+        data_dir=data_dir,
+        measurement_type=measurement_type,
+        telescope=telescope
+    )
 
 @app.command(no_args_is_help=True)
 def plot(
     lidar_name: LidarName = typer.Option(..., "--lidar", "-l"),
     initial_date: datetime = typer.Option(..., "--initial-date", "-i"),
     final_date: Optional[datetime] = typer.Option(None, "--final-date", "-f"),
 ):
```

### Comparing `gfatpy-0.1.0/gfatpy/cli/lidar/plot/main.py` & `gfatpy-0.3.0/gfatpy/cli/lidar/plot/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cli/main.py` & `gfatpy-0.3.0/gfatpy/cli/main.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cloudnet/cloud_model.py` & `gfatpy-0.3.0/gfatpy/cloudnet/cloud_model.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cloudnet/plot_deprecated.py` & `gfatpy-0.3.0/gfatpy/cloudnet/plot_deprecated.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cloudnet/reader.py` & `gfatpy-0.3.0/gfatpy/cloudnet/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/cloudnet/utils.py` & `gfatpy-0.3.0/gfatpy/cloudnet/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/config.py` & `gfatpy-0.3.0/gfatpy/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,22 @@
         system_dn = "Y:"
     else:
         system_dn = "/mnt/NASGFAT"
 
     system_dn = Path(system_dn)
     data_dn = Path.joinpath(system_dn, "datos")
 
-    if data_dn.exists():
+    try:
+        data_dn_exist = data_dn.exists()
+    except Exception as e:
+        print(e)
+        FileNotFoundError("Directoy not found.")
+        data_dn_exist = False
+
+    if data_dn_exist:
         return system_dn, data_dn
     else:
         return None, None
 
 
 # Root Directory (in NASGFAT)  according to operative system
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/.hgtags` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/.hgtags`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/About the effects of polarising optics_4b_1L_corr.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/GHK_0.9.8h_Py3.7.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/Improvements_of_the_GHK_script_200529.pdf`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/LICENSE.md` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/README.md` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/README.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_polarizer_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_rotator_casoG_template.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/mulhacen_run.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8e4-PollyXT_Lacros.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_0.9.8h-PollyXT_Cyprus_532_210429_vf_4.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_pol_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20130101.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/system_settings/optic_input_mhc_rot_532x_20220614.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK/tests/datos/MULHACEN/QA/GHK/2022/10/04/output_optic_input_mhc_rot_532x_20220614_GHK_0.9.8h_Py3.7.dat` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK/tests/datos/MULHACEN/QA/GHK/2022/10/04/output_optic_input_mhc_rot_532x_20220614_GHK_0.9.8h_Py3.7.dat`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/GHK.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/GHK.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/calibration.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/calibration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from datetime import datetime
 from pathlib import Path
-from pdb import set_trace
+
 import xarray as xr
-from datetime import datetime
+import numpy as np
 
 from gfatpy import DATA_DN
 from gfatpy.lidar import file_manager
-from gfatpy.lidar.utils import LIDAR_INFO
-
 from gfatpy.lidar.preprocessing.lidar_preprocessing import preprocess
+from gfatpy.lidar.utils import LIDAR_INFO
+from scipy.signal import savgol_filter
 
 
 def retrieve_eta_star_profile(
     signal_T_plus45: xr.DataArray,
     signal_T_minus45: xr.DataArray,
     signal_R_plus45: xr.DataArray,
     signal_R_minus45: xr.DataArray,
@@ -42,18 +43,18 @@
     # Remove effect of the possible extra filter to avoid saturation of the s-channel.
     signal_T_plus45_with_extra_filter = signal_T_plus45
     signal_T_plus45 = signal_T_plus45_with_extra_filter / transmittance_extra_filter
     signal_T_minus45_with_extra_filter = signal_T_minus45
     signal_T_minus45 = signal_T_minus45_with_extra_filter / transmittance_extra_filter
 
     #   Calculate the signal ratio for the +45 position.
-    delta_v45_plus = (signal_T_plus45 / signal_R_plus45).mean("time")
+    delta_v45_plus = signal_R_plus45 / signal_T_plus45
 
     #   Calculate the signal ratio for the -45 position.
-    delta_v45_minus = (signal_T_minus45 / signal_R_minus45).mean("time")
+    delta_v45_minus = signal_R_minus45 / signal_T_minus45
 
     #   Calculate the calibration constant vertical profile.
     v_star_profile = (delta_v45_plus * delta_v45_minus) ** 0.5
     return v_star_profile
 
 
 def eta_star_mean_std(
@@ -95,18 +96,20 @@
 def calibration_factor_files(
     P45_fn: Path,
     N45_fn: Path,
     calib_dir: Path | None,
     min_range: float = 1500,
     max_range: float = 3000,
     transmittance_extra_filter: float = 1.0,
+    epsilon: float | None = None,
+    an_calib_limits: tuple[float, float] = (1500, 3000),
+    pc_calib_limits: tuple[float, float] = (2500, 4000),
 ) -> xr.Dataset:
 
     if not P45_fn.is_file():
-        set_trace()
         raise FileNotFoundError(f"{P45_fn} not found.")
 
     if not N45_fn.is_file():
         raise FileNotFoundError(f"{N45_fn} not found.")
 
     lidar_nick, _, _, _, telescope_, calib_date = file_manager.filename2info(
         P45_fn.name
@@ -142,50 +145,138 @@
                 channel_T not in N45.channel.values
                 or channel_R not in N45.channel.values
             ):
                 continue
 
             calib_dict[telescope_][wavelength_][mode_] = {}
 
-            signal_R_P45 = P45[f"signal_{channel_R}"]
-            signal_T_P45 = P45[f"signal_{channel_T}"]
-            signal_R_N45 = N45[f"signal_{channel_R}"]
-            signal_T_N45 = N45[f"signal_{channel_T}"]
+            signal_T_P45 = xr.apply_ufunc(
+                savgol_filter,
+                P45[f"signal_{channel_T}"].mean("time"),
+                11,
+                3,
+                dask="allowed",
+            )
+            signal_R_P45 = xr.apply_ufunc(
+                savgol_filter,
+                P45[f"signal_{channel_R}"].mean("time"),
+                11,
+                3,
+                dask="allowed",
+            )
+            signal_R_N45 = xr.apply_ufunc(
+                savgol_filter,
+                N45[f"signal_{channel_R}"].mean("time"),
+                11,
+                3,
+                dask="allowed",
+            )
+            signal_T_N45 = xr.apply_ufunc(
+                savgol_filter,
+                N45[f"signal_{channel_T}"].mean("time"),
+                11,
+                3,
+                dask="allowed",
+            )
 
             eta_star_profile = retrieve_eta_star_profile(
                 signal_T_P45,
                 signal_T_N45,
                 signal_R_P45,
                 signal_R_N45,
                 transmittance_extra_filter=transmittance_extra_filter,
             )
             calib_dict[telescope_][wavelength_][mode_]["profile"] = eta_star_profile
-
             eta_star_mean, eta_star_std = eta_star_mean_std(
                 eta_star_profile, min_range=min_range, max_range=max_range
             )
+
+            # Calibrator rotation, epsilon [Freudenthaler, V. (2016)., Eq. 194, 195]
+            # average over calibration height interval
+            gain_ratio_p45 = signal_T_P45 / signal_R_P45
+            gain_ratio_n45 = signal_T_N45 / signal_R_N45
+
+            ranges = P45.range.values
+
+            match mode_:
+                case "a":
+                    idx_avg_ranges = (ranges >= an_calib_limits[0]) & (
+                        ranges <= an_calib_limits[1]
+                    )
+                case "p":
+                    idx_avg_ranges = (ranges >= pc_calib_limits[0]) & (
+                        ranges <= pc_calib_limits[1]
+                    )
+                # case "g":
+                #     ...
+                # TODO: Gluing gna be implemented in the future by receiving extra argument
+                case _:
+                    raise ValueError(f"Mode {mode_} not recognized")
+
+            Y = (gain_ratio_p45 - gain_ratio_n45) / (gain_ratio_p45 + gain_ratio_n45)
+            Y_avg = np.nanmean(Y[idx_avg_ranges])
+            Y_std = np.nanstd(Y[idx_avg_ranges])
+            if epsilon is None:
+                epsilon = (
+                    (180 / np.pi) * 0.5 * np.arcsin(np.tan(0.5 * np.arcsin(Y_avg)))
+                )
+
+            epsilon_err = (
+                (180 / np.pi)
+                * 0.5
+                * abs(
+                    0.5 * np.arcsin(np.tan(0.5 * np.arcsin(Y_avg + Y_std)))
+                    - 0.5 * np.arcsin(np.tan(0.5 * np.arcsin(Y_avg - Y_std)))
+                )
+            )
+
             calib_dict[telescope_][wavelength_][mode_]["values"] = [
                 eta_star_mean,
                 eta_star_std,
+                Y_avg,
+                Y_std,
+                epsilon,
+                epsilon_err,
+            ]
+
+            calib_dict[telescope_][wavelength_][mode_]["signals"] = [
+                signal_T_N45,
+                signal_T_P45,
+                signal_R_P45,
+                signal_R_N45,
+                gain_ratio_p45,
+                gain_ratio_n45,
             ]
 
     # Create dataset
     calib_dataset = xr.Dataset()
+
+    channels = []
+    for wavelength_ in calib_dict[telescope_].keys():
+        for mode_ in calib_dict[telescope_][wavelength_].keys():
+            channels.append(f"{wavelength_}{telescope_[0]}{mode_}")
+
     for wavelength_ in calib_dict[telescope_].keys():
         for mode_ in calib_dict[telescope_][wavelength_].keys():
             key_profile = f"eta_star_profile_{wavelength_}{telescope_[0]}{mode_}"
             calib_dataset[key_profile] = calib_dict[telescope_][wavelength_][mode_][
                 "profile"
             ]
+            # set_trace()
+            (
+                eta_star_mean,
+                eta_star_std,
+                Y_avg,
+                Y_std,
+                epsilon,
+                epsilon_err,
+            ) = calib_dict[telescope_][wavelength_][mode_]["values"]
 
-            eta_star_mean, eta_star_std = calib_dict[telescope_][wavelength_][mode_][
-                "values"
-            ]
             calib_dataset[
-                f"eta_start_mean_{wavelength_}{telescope_[0]}{mode_}"
+                f"eta_start_mean_{wavelength_}{telescope_[0]}{mode_}"  # TODO: Telescope is hardcoded, must iterate over that too
             ] = xr.DataArray(
                 eta_star_mean,
                 dims=[],
                 attrs={
                     "long_name": f"range-average of {key_profile}",
                     "min_range_m": min_range,
                     "max_range_m": max_range,
@@ -199,14 +290,77 @@
                 attrs={
                     "long_name": f"range standard-deviation of {key_profile}",
                     "min_range_m": min_range,
                     "max_range_m": max_range,
                 },
             )
 
+            calib_dataset[
+                f"Y_average_{wavelength_}{telescope_[0]}{mode_}"
+            ] = xr.DataArray(
+                Y_avg,
+                dims=[],
+                attrs={
+                    "long_name": f"range standard-deviation of {key_profile}",
+                    "min_range_m": min_range,
+                    "max_range_m": max_range,
+                },
+            )
+            calib_dataset[
+                f"Y_standard_deviation_{wavelength_}{telescope_[0]}{mode_}"
+            ] = xr.DataArray(
+                Y_std,
+                dims=[],
+                attrs={
+                    "long_name": f"range standard-deviation of {key_profile}",
+                    "min_range_m": min_range,
+                    "max_range_m": max_range,
+                },
+            )
+
+            calib_dataset[
+                f"epsilon_{wavelength_}{telescope_[0]}{mode_}"
+            ] = xr.DataArray(
+                epsilon,
+                dims=[],
+                attrs={
+                    "long_name": f"range standard-deviation of {key_profile}",
+                    "min_range_m": min_range,
+                    "max_range_m": max_range,
+                },
+            )
+
+            calib_dataset[
+                f"epsilon_error_{wavelength_}{telescope_[0]}{mode_}"
+            ] = xr.DataArray(
+                epsilon_err,
+                dims=[],
+                attrs={
+                    "long_name": f"range standard-deviation of {key_profile}",
+                    "min_range_m": min_range,
+                    "max_range_m": max_range,
+                },
+            )
+
+            signals_order = [
+                "signal_T_N45",
+                "signal_T_P45",
+                "signal_R_P45",
+                "signal_R_N45",
+            ]
+            for signal, signal_name in zip(
+                calib_dict[telescope_][wavelength_][mode_]["signals"], signals_order
+            ):
+                calib_dataset[
+                    f"{signal_name}_{wavelength_}{telescope_[0]}{mode_}"
+                ] = signal
+
+    # Channels is not a coordinate yet, just a utility to read the file
+    calib_dataset["channels"] = channels
+
     calib_datetime_str = datetime.strftime(calib_date, "%Y%m%d_%H%M")
     if calib_dir is None:
         if DATA_DN is not None:
             calib_dir = (
                 DATA_DN
                 / lidar_name
                 / "QA"
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/depolarization_calibration_mhc.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/depolarization_calibration_vlt.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/lidar_merge.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/old_lidar_merge_2bremoved.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/depolarization/utils.py` & `gfatpy-0.3.0/gfatpy/lidar/depolarization/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/file_manager.py` & `gfatpy-0.3.0/gfatpy/lidar/file_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,57 +3,68 @@
 
 
 from datetime import datetime
 import numpy as np
 
 from gfatpy import DATA_DN
 from gfatpy.lidar.utils import LIDAR_INFO
+from gfatpy.utils.utils import parse_datetime
 
 
 def channel2info(channel: str) -> tuple[int, str, str | None, str]:
     """`channel_str2info` extracts the information concerning the channel configuration from the string code.
 
     Args:
         channel (str): Chanel string code (e.g., '532xta'.)
 
     Returns:
         tuple[str]: Tuple with following elements: wavelength [int], telescope Options['xf', 'ff', 'nf'], polarization Options['p', 's', 't'], detection Options['a', 'p', 'g'].
     """
 
     channel = channel.split("_")[-1]
     if len(channel) > 5:
-        wave = int(channel[0:-3])
+        wave = int(channel[0:-3], base = 10)
         telescope = f"{channel[-3]}f"
         polarization = channel[-2]
         detection = channel[-1]
     elif len(channel) == 5:
-        wave = int(channel[0:-2])
+        wave = int(channel[0:-2], base = 10)
         telescope = f"{channel[-2]}f"
         polarization = None
         detection = channel[-1]
     else:
         set_trace()
         raise ValueError("Channel format not recognized.")
 
     return wave, telescope, polarization, detection
 
 
 def filename2info(filename: str) -> tuple[str, str, str, str, str, datetime]:
     parts = filename.split("_")
+    
     lidar_nick = parts[0]
     data_level = parts[1]
-    measurement_type = parts[2][-2:]
+    measurement_type = parts[2][1:3]
     signal_type = parts[3]
     telescope = parts[4]
+    
+    if measurement_type in ["tc", "dp"]: #Fallback new format nc for TC and DP
+        signal_type = parts[2][1:3]
+        telescope = parts[3]
+        date_ = parts[4].split(".")[0]
+    else:
+        date_ = parts[5].split(".")[0]
 
-    date_ = parts[5].split(".")[0]
-    if len(parts) == 7:
+    if len(parts) == 7: # has hour
         hour_ = parts[6].split(".")[0]
         date = datetime.strptime(date_ + hour_, "%Y%m%d%H%M")
-    else:
+    elif measurement_type in ["tc", "dp"]:
+        hour_ = parts[5].split(".")[0]
+        date = datetime.strptime(date_ + hour_, "%Y%m%d%H%M")
+    else: # has not hour
         date = datetime.strptime(date_, "%Y%m%d")
 
     return lidar_nick, data_level, measurement_type, signal_type, telescope, date
 
 
 def info2filename(
     channel: str,
@@ -87,17 +98,21 @@
 
     if lidar_nick in LIDAR_INFO["metadata"]["nick2name"].keys():
         _, telescope, _, _ = channel2info(channel)
     else:
         raise NameError("lidar_nick not found in `LIDAR_INFO`.")
 
     date_str = date.strftime("%Y%m%d")
-    filename_ = f"{lidar_nick}_{data_level}_P{measurement_type.lower()}_{signal_type.lower()}_{telescope}_{date_str}"
+    
+    if measurement_type not in ["TC", "DP"]:
+        filename_ = f"{lidar_nick}_{data_level}_P{measurement_type.lower()}_{signal_type.lower()}_{telescope}_{date_str}"
+    else:
+        filename_ = f"{lidar_nick}_{data_level}_P{measurement_type.lower()}-{signal_type}_{telescope}_{date_str}"
 
-    if measurement_type == "DC":
+    if measurement_type in ["DC", "TC", "DP"]:
         if isinstance(date, datetime):
             hour = date.strftime("%H%M")
             filename_ = filename_ + "_" + hour
         else:
             raise TypeError(
                 "Date must be datetime.datetime if `measurement_type` is `DC`."
             )
@@ -217,15 +232,16 @@
         lidar_nick (str): Nick of lidar. Options in `LIDAR_INFO`.
         telescope (str, optional): Telescope type code Options['xf', 'ff', 'nf']
         session_period (tuple[datetime.datetime, datetime.datetime]): Period where the DC is searched. If not found, the nearest is provided.
         force_dc_in_session (bool, optional): Force the DC measurment to be in the period, otherwise it raises an error. Defaults to False.
     Returns:
         Path: Path of the DC measurement.
     """
-    candidates = list(rs_path.parent.glob("*1a_Pdc_*"))
+    telescope = filename2info(rs_path.name)[4]
+    candidates = list(rs_path.parent.glob(f"*1a_Pdc_*{telescope}*"))
 
     for dc_path in candidates:
         dc_npdate = np.datetime64(filename2info(dc_path.name)[-1])
         if (session_period[0] <= dc_npdate) and (dc_npdate <= session_period[1]):
             return dc_path
 
     if force_dc_in_session:
@@ -272,7 +288,46 @@
         list(
             map(
                 lambda p: np.datetime64(p.name.split(".")[0].split("_")[-1]), candidates
             )
         )
     )
     return candidates, dates
+
+
+def info2general_path(
+    lidar_name: str,
+    date: datetime | str,
+    data_level: str,
+    data_dir: Path | None = None,
+) -> Path:
+    """Similar to info2path but can take only lidar name, data level and dates as only args
+
+    Args:
+        lidar_name (str): _description_
+        date (datetime | str): _description_
+        data_level (str): _description_
+
+    Returns:
+        Path: _description_
+    """
+
+    date = parse_datetime(date)
+
+    if data_dir is None:
+        if DATA_DN is None:
+            raise ValueError("DATA_DN is None.")
+        else:
+            data_dir = DATA_DN
+    else:
+        if not data_dir.exists():
+            set_trace()
+            raise NotADirectoryError("data_dir not found.")
+
+    return (
+        data_dir
+        / lidar_name
+        / data_level
+        / f"{date.year}"
+        / f"{date.month:02}"
+        / f"{date.day:02}"
+    )
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/info.yml` & `gfatpy-0.3.0/gfatpy/lidar/info.yml`

 * *Files 22% similar despite different names*

```diff
@@ -89,47 +89,112 @@
         - 355xsp
     GHK_channels:
       - 355x
   ALHAMBRA:
     modules:
       - nf
       - ff
-    channels: [
-      1064fta, 1061fta,
-      532fta,  532ftp,
-      531fta,  531ftp,
-      355fpa,  355fpp,  355fsa,  355fsp,
-      354fta,  354ftp,
-      408fta,  408ftp,
-      1064nta, 1064nta,
-      532npa,  532npa,  532npp, 532npp,
-      532nsa,  532nsa,  532nsp, 532nsp,
-      355npa,  355npa,  355npp, 355npp,
-      355nsa,  355nsa,  355nsp, 355nsp,
-      387nta,  387nta,  387ntp, 387ntp,
-      607nta,  607nta
-    ]
+    channels:
+      1064fta:
+        bin_zero: 5
+      1061fta:
+        bin_zero: 5
+      532fta:
+        bin_zero: 5
+      532ftp:
+        bin_zero: -2
+        dead_time_ns: 4
+      531fta:
+        bin_zero: 5
+      531ftp:
+        bin_zero: -2
+        dead_time_ns: 4
+      355fpa:
+        bin_zero: 5
+      355fpp:
+        bin_zero: -2
+        dead_time_ns: 4
+      355fsa:
+        bin_zero: 5
+      355fsp:
+        bin_zero: -2
+        dead_time_ns: 4
+      354fta:
+        bin_zero: 5
+      354ftp:
+        bin_zero: -2
+        dead_time_ns: 4
+      408fta:
+        bin_zero: 5
+      408ftp:
+        bin_zero: -2
+        dead_time_ns: 4
+      1064nta:
+        bin_zero: 5
+      532npa:
+        bin_zero: 5
+      532npp:
+        bin_zero: -2
+        dead_time_ns: 4
+      532nsa:
+        bin_zero: 5
+      532nsp:
+        bin_zero: -2
+        dead_time_ns: 4
+      355npa:
+        bin_zero: 5
+      355npp:
+        bin_zero: -2
+        dead_time_ns: 4
+      355nsa:
+        bin_zero: 5
+      355nsp:
+        bin_zero: -2
+        dead_time_ns: 4
+      387nta:
+        bin_zero: 5
+      387ntp:
+        bin_zero: -2
+        dead_time_ns: 4
+      607nta:
+        bin_zero: 5
     polarized_channels:
-      ff:
-        355:
-        355fpa: Tan
-        355fpp: Tpc
-        355fsa: Ran
-        355fsp: Rpc
       nf:
         355:
-          355npa: Tan
-          355npp: Tpc
-          355nsa: Ran
-          355nsp: Rpc
+          a: 
+            T: 355nsa
+            R: 355npa
+          p:
+            T: 355nsp
+            R: 355npp
+          g:
+            T: 355nsg
+            R: 355npg
         532:
-          532npa: Tan
-          532npp: Tpc
-          532nsa: Ran
-          532nsp: Rpc
+          a: 
+            T: 532nsa
+            R: 532npa
+          p:
+            T: 532nsp
+            R: 532npp
+          g:
+            T: 532nsg
+            R: 532npg
+      ff:
+        355:
+          a: 
+            T: 355fsa
+            R: 355fpa
+          p:
+            T: 355fsp
+            R: 355fpp
+          g:
+            T: 355fsg
+            R: 355fpg
+        
     product_channels:
       355fta:
         - 355fpa
         - 355fsa
       lvd_355fa:
         - 355fpa
         - 355fpa
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/plot/info.yml` & `gfatpy-0.3.0/gfatpy/lidar/plot/info.yml`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/plot/quicklook.py` & `gfatpy-0.3.0/gfatpy/lidar/plot/quicklook.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pathlib
+from typing import Literal
 
 import matplotlib
 import numpy as np
 import xarray as xr
 import pandas as pd
 import datetime as dt
 from loguru import logger
@@ -471,26 +472,32 @@
 #     hours = mdates.HourLocator(interval = 1)
 #     h_fmt = mdates.DateFormatter('%H:%M')
 #     axes.xaxis.set_major_locator(hours)
 #     axes.xaxis.set_major_formatter(h_fmt)
 #     plt.fill_between([min(time),max(time)], [0,0], [z_station,z_station], alpha = 0.7, color = 'black')
 #     plt.show()
 
+BoundsType = tuple[float, float] | Literal["auto", "limits"]
+
 
 def get_norm(
     rcs: np.ndarray,
-    scale_bounds: tuple[float, float] | None = None,
+    scale_bounds: BoundsType,
     color_resolution: int = 128,
 ) -> matplotlib.colors.BoundaryNorm:
-    if scale_bounds is not None:
-        bounds = np.linspace(*scale_bounds, 128)
-    else:
-        bounds = np.linspace(0, rcs.max() * 0.6, 128)
 
-    norm = matplotlib.colors.BoundaryNorm(boundaries=bounds, ncolors=2**8)
+    match scale_bounds:
+        case "auto":
+            bounds = np.linspace(0, rcs.max() * 0.6, 128)
+        case "limits":
+            bounds = np.linspace(rcs.min(), rcs.max(), 128)
+        case _:
+            bounds = np.linspace(*scale_bounds, 128)
+
+    norm = matplotlib.colors.BoundaryNorm(boundaries=bounds, ncolors=2**8, clip=False)
     logger.debug(f"Color bounds min - max: {bounds.min()} - {bounds.max()}")
 
     return norm
 
 
 def apply_labels(ax: matplotlib.axes.Axes, data_array: xr.DataArray) -> None:  # type: ignore
     # TODO: Other titles will later be added with config param
@@ -524,16 +531,17 @@
         "#c7c7c7",
     )
 
 
 # TODO: this should be the default implemetation rather than filelist argument
 def quicklook_xarray(
     data_array: xr.DataArray,
-    scale_bounds: tuple[float, float] | None = None,
+    /,
     is_rcs: bool = True,
+    scale_bounds: BoundsType = "auto",
     color_resolution: int = 128,
     colormap: str | matplotlib.colors.Colormap = "jet",
 ) -> tuple[Figure, Axes]:
 
     if is_rcs:
         rcs = data_array.values
     else:
@@ -543,15 +551,15 @@
     norm = get_norm(rcs, scale_bounds)
 
     q = ax.pcolormesh(
         data_array.time, data_array.range, rcs.T, cmap=colormap, norm=norm
     )
 
     ax.set_xlabel(r"Time, $[UTC]$")
-    ax.set_ylabel(r"Height, $[km, \, agl]$")
+    ax.set_ylabel(r"Height, $[m, \, agl]$")
     ax.set_ylim(0)
 
     apply_labels(ax, data_array=data_array)
     apply_gap_size(ax, data_array=data_array)
 
     fig.colorbar(q)
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/__init__.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/gluing_de_la_rosa_slope.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_dead_time.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_dead_time.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_gluing_bravo_aranda.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_gluing_damico.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_linear_response_region.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # from curses import set_tabsize
 from pathlib import Path
+from pdb import set_trace
 
 import numpy as np
 import xarray as xr
 
 from gfatpy.lidar.file_manager import filename2path, search_dc
 
 # from gfatpy.lidar.preprocessing.lidar_gluing_bravo_aranda import gluing
-from gfatpy.lidar.preprocessing.gluing_de_la_rosa import gluing
+from gfatpy.lidar.preprocessing.gluing_proportional import gluing
 from gfatpy.lidar.utils import LIDAR_INFO
 from gfatpy.utils import calibration
 
 # from .lidar_merge import apply_polarization_merge
 # from .lidar_preprocessing_tools import *  # TODO: Remove wildcard importations within modules
 
 # warnings.filterwarnings("ignore")
@@ -72,15 +73,16 @@
     if not _p.exists():
         print("File not found. Searching in DATA_DN.")
         filename = _p.name
         _p = filename2path(filename)
         if not _p.exists:
             raise ValueError("File not found.")
 
-    dataset = xr.load_dataset(_p)
+    with xr.open_dataset(_p, chunks={}) as _nc:
+        dataset = _nc
     dataset = drop_unwanted_channels(dataset, channels=channels)
 
     if apply_dc:
         dataset = apply_dark_current_correction(
             dataset,
             rs_path=_p,
             save_dc=save_dc,
@@ -125,15 +127,17 @@
     return dataset
 
 
 def apply_dark_current_correction(
     dataset: xr.Dataset, rs_path: Path, save_dc: bool = False, force_dc_in_session=False
 ) -> xr.Dataset:
     groups = calibration.split_continous_measurements(dataset.time.values)
-    analog_channels = list(filter(lambda c: c.endswith("a"), dataset.channel.values))
+    channels = dataset.channel.values
+
+    analog_channels: list[str] = list(filter(lambda c: c.endswith("a"), channels))
 
     for group in groups:
         dc_path = search_dc(
             rs_path,
             session_period=group[[0, -1]],
             force_dc_in_session=force_dc_in_session,
         )
@@ -176,15 +180,15 @@
                 if value.get("dead_time_ns", False)
             }
         except Exception:
             raise ValueError(
                 f"No dead time value defined in LIDAR_INFO->{lidar_name}]."
             )
 
-    photocounting_channels = list(
+    photocounting_channels: list[str] = list(
         filter(lambda c: c.endswith("p"), dataset.channel.values)
     )
 
     for channel in photocounting_channels:
         # tau from ns to us
         tau_us = dt_dict[channel] * 1e-3
 
@@ -217,18 +221,21 @@
 
     if background_ranges[1] <= background_ranges[0]:
         raise ValueError("background_ranges should be in order (min, max)")
 
     ranges_between = (background_ranges[0] < dataset.range) & (
         dataset.range < background_ranges[1]
     )
-
-    for channel in dataset.channel:
+    channels: list[str] = dataset.channel.values
+    for channel in channels:
         signal_str = f"signal_{channel}"
-        background = dataset[signal_str].loc[:, ranges_between].mean(axis=1)
+        try:
+            background = dataset[signal_str].loc[:, ranges_between].mean(axis=1)
+        except:
+            background = np.ones(1)
         dataset[signal_str] -= background
 
         if save_bg:
             dataset[f"bg_{channel}"] = background
 
     dataset.attrs["bg_corrected"] = True
 
@@ -244,17 +251,18 @@
         lidar_name = dataset.attrs["system"].upper()
         try:
             bz_dict = {
                 key: value["bin_zero"]
                 for (key, value) in LIDAR_INFO["lidars"][lidar_name]["channels"].items()
             }
         except Exception:
-            raise ValueError(f"No bin zero value defined in LIDAR_INFO->{lidar_name}].")
+            raise ValueError(f"No bin zero value defined in LIDAR_INFO->{lidar_name}.")
 
-    for channel in dataset.channel.values:
+    channels: list[str] = dataset.channel.values
+    for channel in channels:
         signal_str = f"signal_{channel}"
         # set_trace()
         dataset[signal_str] = dataset[signal_str].shift(
             range=-bz_dict[channel], fill_value=0.0
         )
 
     dataset.attrs["bz_corrected"] = True
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_preprocessing_tools.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/lidar_zerobin_triggerdelay_binshift.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/lidar_zerobin_triggerdelay_binshift.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/preprocessing/study_dead_time.py` & `gfatpy-0.3.0/gfatpy/lidar/preprocessing/study_dead_time.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/common.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/common.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/depolarization.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/depolarization.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/io.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/io.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/plot.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 from gfatpy.lidar.file_manager import channel2info
 
 
 def plot_rayleigh_fit(
     filepath: Path | list[Path],
     output_dir: Path | None = None,
     save_fig: bool = False,
-) -> tuple[list[Figure | None], list[Figure | None]]:
+) -> tuple[
+    list[Figure | None], list[Figure | None]
+]:  # FIXME: warning message due to more than 20 figures open. Consider remove output figure/axes handles.
 
     if isinstance(filepath, Path):
         files = [filepath]
     elif isinstance(filepath, list):
         files = filepath
     else:
         raise ValueError("filepath must be Path or list[Path]")
@@ -127,8 +129,9 @@
 
             plt.tight_layout()
             plt.savefig(fig_fn, dpi=300, bbox_inches="tight")
         else:
             fig, ax = None, None
         figures.append(fig)
         axes.append(ax)
+        plt.close()
     return figures, axes
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/rayleigh_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime as dt
 from pathlib import Path
 from typing import Any
-
+from pdb import set_trace
 import numpy as np
 import pandas as pd
 import xarray as xr
 from scipy.signal import savgol_filter
 
 from gfatpy import DATA_DN
 from gfatpy.utils import utils
@@ -308,16 +308,15 @@
     # Lidar preprocess
     lidar_ds = preprocess(
         filepath,
         channels=channels,
         crop_ranges=crop_ranges,
         save_dc=True,
         save_bg=True,
-    )
-
+    )    
     # time in array
     times = lidar_ds["time"].values
     times = np.array([utils.numpy_to_datetime(xx) for xx in times])
 
     # ranges in array
     range = lidar_ds["range"].values
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/quality_assurance/telecover.py` & `gfatpy-0.3.0/gfatpy/lidar/quality_assurance/telecover.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/__init__.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/__init__.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/lidar_raw2l1.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/lidar_raw2l1.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/CHANGELOG` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/CHANGELOG`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/LICENSE` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/LICENSE`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/README.md` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/README.md`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_jenoptik_chm15k.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_jenoptik_chm15k.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_eprofile.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_eprofile.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_lufft_chm15k-nimbus_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_mhc_prod.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_mhc_prod.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_pd.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_pd.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_ff.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_ff.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_nf.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_rs_nf.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_ff.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_ff.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_nf.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_ALHAMBRA_sd_nf.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_MULHACEN.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_MULHACEN.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_VELETA.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_prod_VELETA.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l1-tb_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l1-tb_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l2-ta_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_bl00-l2-ta_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l1-tb_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l1-tb_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-clwvi_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-clwvi_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-hua_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-hua_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-prw_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-prw_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-ta_toprof_netcdf4.ini` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/conf/conf_rpg_hatpro_l2-ta_toprof_netcdf4.ini`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/Makefile` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/make.bat` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/conf.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/configuration.rst` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/images/logo_sirta_navbar.png` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/images/logo_sirta_navbar.png`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/index.rst` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/prerequisites.rst` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/doc/source/prerequisites.rst`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/raw2l1.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/raw2l1.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/campbellscientific_cs135.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/campbellscientific_cs135.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10min.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10min.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10s.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls70_10s.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_10min.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_10min.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_1s.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/leosphere_wls7_1s.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/libvaisala.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lib/libvaisala.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/libhatpro.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/libhatpro.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus-uk-metoffice.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus-uk-metoffice.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/lufft_chm15k_nimbus.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_DMC.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_DMC.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh_test.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_alh_test.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_lidar.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_lidar.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_mhc.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_mhc.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_vlt.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/reader_vlt.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_absolute_humidity.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_absolute_humidity.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp_bl.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_air_temp_bl.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature_bl.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_brightness_temperature_bl.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_clwvi.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_clwvi.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_prw.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/rpg_hatpro_prw.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/sigmaspace_minimpl.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/reader/sigmaspace_minimpl.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_arg_parser.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_arg_parser.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus-uk-metoffice.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus-uk-metoffice.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_chm15k_nimbus.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_cs135.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_cs135.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls7.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls7.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls70.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_leosphere_wls70.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_lidar_reader.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_lidar_reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_logs.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_logs.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_netcdf4.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_netcdf4.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_rpg_hatpro.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_rpg_hatpro.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_sigmaspace_minimpl.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_sigmaspace_minimpl.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_toprof_format.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_toprof_format.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_eprofile.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_eprofile.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_sirta.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/test/_test_vaisala_sirta.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/arg_parser.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/arg_parser.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/check_conf.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/check_conf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/common.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/common.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/conf.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/conf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/create_netcdf.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/create_netcdf.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/lidar_reader.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/lidar_reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/log.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/log.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/read_overlap.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/read_overlap.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/utils.py` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/raw2l1_gfat/raw2l1/tools/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_ASUS.sh` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_ASUS.sh`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_SERVER.sh` & `gfatpy-0.3.0/gfatpy/lidar/raw2l1/run_raw2l1_EXAMPLE_SERVER.sh`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/reader.py` & `gfatpy-0.3.0/gfatpy/lidar/reader.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/retrieval/helper.py` & `gfatpy-0.3.0/gfatpy/lidar/retrieval/helper.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/retrieval/klett.py` & `gfatpy-0.3.0/gfatpy/lidar/retrieval/klett.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,31 +29,31 @@
     Returns:
         np.ndarray: Aerosol backscattering (beta)
     """
     particle_beta = np.zeros(len(range_profile))
 
     ytop = (np.abs(range_profile - ymax)).argmin()
 
-    range_resolution = np.median(np.diff(range_profile))
+    range_resolution = np.median(np.diff(range_profile))  # type: ignore
 
     idx_ref = np.logical_and(range_profile >= ymin, range_profile <= ymax)
 
     if idx_ref.any():
         calib = np.nanmean(
             rcs_profile[idx_ref] / (beta_mol_profile[idx_ref] + beta_aer_ref)
         )
         # Calculo de backscatter cuando i<Z0
         # integer1 = np.flip(-cumtrapz(np.flip(beta_mol_profile[:ytop]),dx=range_resolution,initial=0))
         integer1 = np.flip(
-            -cumtrapz(np.flip(beta_mol_profile[:ytop]), dx=range_resolution, initial=0)
+            -cumtrapz(np.flip(beta_mol_profile[:ytop]), dx=range_resolution, initial=0)  # type: ignore
         )
         integrando = rcs_profile[:ytop] * np.exp(-2 * (lr_aer - lr_mol) * integer1)
         # integer3 = np.flip(-cumtrapz(np.flip(integrando),dx=range_resolution,initial=0))
         integer3 = np.flip(
-            -cumtrapz(np.flip(integrando), dx=range_resolution, initial=0)
+            -cumtrapz(np.flip(integrando), dx=range_resolution, initial=0)  # type: ignore
         )
         particle_beta[:ytop] = (
             rcs_profile[:ytop] * np.exp(-2 * (lr_aer - lr_mol) * integer1)
         ) / (calib - 2 * lr_aer * integer3) - beta_mol_profile[:ytop]
 
     else:
         logger.error("Range [ymin,ymax] out of rcs size.")
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/retrieval/lidar_layer_detection.py` & `gfatpy-0.3.0/gfatpy/lidar/retrieval/lidar_layer_detection.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/lidar/retrieval/raman.py` & `gfatpy-0.3.0/gfatpy/lidar/retrieval/raman.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Retrievals of backscatter and extinction based on Raman measurements
 
 .. warning::
    These functions have not been tested!
 """
 import numpy as np
-
 from scipy.integrate import cumtrapz
 from scipy.signal import savgol_filter
 
 from gfatpy.atmo.atmo import molecular_extinction, number_density_at_pt
 
 
 def _integrate_from_reference(integral_argument, index_reference, bin_length):
@@ -90,17 +89,17 @@
     alpha_aer : arrays
        The aerosol extinction coefficient [m-1]
 
     Notes:
     The aerosol extinction coefficient is given by the formula:
 
     .. math::
-       \alpha_{aer}(R,\lambda_0) = \frac{\frac{d}{dR}ln[\frac{N_{Ra}(R)}
-       {S(R,\lambda_{Ra})}] - \alpha_{mol}(R,\lambda_0) - \alpha_{mol}(R,\lambda_{Ra})}
-       {[1 + (\frac{\lambda_0}{\lambda_{Ra}})^{\alpha(R)}]}
+       \\alpha_{aer}(R,\\lambda_0) = \\frac{\\frac{d}{dR}ln[\\frac{N_{Ra}(R)}
+       {S(R,\\lambda_{Ra})}] - \\alpha_{mol}(R,\\lambda_0) - \\alpha_{mol}(R,\\lambda_{Ra})}
+       {[1 + (\\frac{\\lambda_0}{\\lambda_{Ra}})^{\\alpha(R)}]}
 
     References
     ----------
     Ansmann, A. et al. Independent measurement of extinction and backscatter profiles
     in cirrus clouds by using a combined Raman elastic-backscatter lidar.
     Applied Optics Vol. 31, Issue 33, pp. 7113-7131 (1992)
     """
@@ -178,15 +177,14 @@
 
     # Ratio to apply derivative
     number_density = number_density.astype(float)
     signal = signal.astype(float)
     valid_idx = np.logical_and(number_density > 0, signal > 0)
     ratio = np.nan * np.ones(len(signal))
     ratio[valid_idx] = np.ma.log(number_density[valid_idx] / signal[valid_idx])
-
     window_size_bin = np.floor(window_size_m / dz).astype(int)
     derivative = savgol_filter(
         ratio, window_size_bin, order, deriv=1, delta=dz, mode="nearest", cval=np.nan
     )  # Calculate 1st derivative
     alpha_aer = (derivative - alpha_molecular_emission - alpha_molecular_raman) / (
         1 + (emission_wavelength / float(raman_wavelength)) ** angstrom_aerosol
     )
@@ -246,18 +244,18 @@
         The aerosol  backscatter coefficient [m-1]
 
     Notes
     -----
     The aerosol backscatter coefficient is given by the formula:
 
     .. math::
-       \beta_{aer}(R,\lambda_0) = [\beta_{aer}(R_0,\lambda_0) + \beta_{mol}(R_0,\lambda_0)]
-       \cdot \frac{P(R_0,\lambda_{Ra}) \cdot P(R,\lambda_0)}{P(R_0,\lambda_0) \cdot P(R,\lambda_{Ra})}
-       \cdot \frac{e^{-\int_{R_0}^{R} [\alpha_{aer}(r,\lambda_{Ra}) + \alpha_{mol}(r,\lambda_{Ra})]dr}}
-       {e^{-\int_{R_0}^{R} [\alpha_{aer}(r,\lambda_0) + \alpha_{mol}(r,\lambda_0)]dr}} - \beta_{mol}(R,\lambda_0)
+       \\beta_{aer}(R,\\lambda_0) = [\\beta_{aer}(R_0,\\lambda_0) + \\beta_{mol}(R_0,\\lambda_0)]
+       \\cdot \\frac{P(R_0,\\lambda_{Ra}) \\cdot P(R,\\lambda_0)}{P(R_0,\\lambda_0) \\cdot P(R,\\lambda_{Ra})}
+       \\cdot \\frac{e^{-\\int_{R_0}^{R} [\\alpha_{aer}(r,\\lambda_{Ra}) + \\alpha_{mol}(r,\\lambda_{Ra})]dr}}
+       {e^{-\\int_{R_0}^{R} [\\alpha_{aer}(r,\\lambda_0) + \\alpha_{mol}(r,\\lambda_0)]dr}} - \\beta_{mol}(R,\\lambda_0)
 
     References
     ----------
     Ansmann, A. et al. Independent measurement of extinction and backscatter profiles
     in cirrus clouds by using a combined Raman elastic-backscatter lidar.
     Applied Optics Vol. 31, Issue 33, pp. 7113-7131 (1992)
     """
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/types.py` & `gfatpy-0.3.0/gfatpy/lidar/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     HF = "HF"
     DC = "DC"
     TC = "TC"
     DP = "DP"
     OT = "OT"
 
 
+class Telescope(str, Enum):
+    xf = "xf"
+    ff = "ff"
+    nf = "nf"
+
 class _LidarInfo(TypedDict):
     MULHACEN: dict
     ALHAMBRA: dict
     VELETA: dict
 
 
 class _LidarMetadata(TypedDict):
```

### Comparing `gfatpy-0.1.0/gfatpy/lidar/utils.py` & `gfatpy-0.3.0/gfatpy/lidar/utils.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/utils/optimized.py` & `gfatpy-0.3.0/gfatpy/utils/optimized.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,73 @@
 import numpy as np
 from numpy.polynomial.polynomial import polyfit
 
-
 import numba
 
 
 def best_slope_fit(mat1: np.ndarray, mat2: np.ndarray, window: int) -> np.ndarray:
 
     assert mat1.shape == mat2.shape, "Matrices shape must match"
     assert isinstance(window, int), "Window argument must be an integer"
 
     x = np.arange(window)
     res = np.array([])
 
     # Iter in first dimension, equivalent to time in lidar case
     for idx in range(mat1.shape[0]):
-        windowed1 = _rolling(mat1[idx], window)
-        windowed2 = _rolling(mat2[idx], window)
+        windowed1 = rolling(mat1[idx], window)
+        windowed2 = rolling(mat2[idx], window)
 
         slopes1 = polyfit(x, windowed1.T, 1)[0]
         slopes2 = polyfit(x, windowed2.T, 1)[0]
         chosen_group = np.argmin(np.abs(slopes1 - slopes2) / slopes1)
         res = np.hstack([res, chosen_group + np.floor(window / 2)])  # Append chosen bin
 
     return res.astype(int)
 
 
 @numba.njit(parallel=True)
 def windowed_corrcoefs(arr1: np.ndarray, arr2: np.ndarray, w_size: int):
     range_shape = arr1.shape[1] - (w_size - 1)
     _corrcoefs = np.empty((arr1.shape[0], range_shape))
     for t_idx in numba.prange(arr1.shape[0]):
-        w1 = _rolling(arr1[t_idx], w_size)
-        w2 = _rolling(arr2[t_idx], w_size)
+        w1 = rolling(arr1[t_idx], w_size)
+        w2 = rolling(arr2[t_idx], w_size)
         for idx in numba.prange(range_shape):
             _w1 = w1[idx]
             _w2 = w2[idx]
             coeff = np.corrcoef(_w1, _w2)[1, 0]
             _corrcoefs[t_idx][idx] = coeff
     return _corrcoefs
 
 
+@numba.njit(parallel=True)
+def windowed_proportional(arr1: np.ndarray, arr2: np.ndarray, /, *, w_size: int):
+
+    assert arr1.shape == arr2.shape, "Matrices shape must match"
+    # assert isinstance(w_size, int), "Window argument must be an integer"
+
+    range_shape = arr1.shape[1] - (w_size - 1)
+    _proportional = np.full((arr1.shape[0], range_shape), np.nan)
+    _factor = np.full((arr1.shape[0], range_shape), np.nan)
+
+    for t_idx in numba.prange(arr1.shape[0]):
+        w1 = rolling(arr1[t_idx], w_size)
+        w2 = rolling(arr2[t_idx], w_size)
+
+        for idx in numba.prange(range_shape):
+            _w1 = w1[idx]
+            _w2 = w2[idx]
+
+            ratio = np.mean(_w2 / _w1)
+            adj = _w1 * ratio
+            _factor[t_idx][idx] = ratio
+            _proportional[t_idx][idx] = (np.abs(adj - _w2) / _w2).mean()
+
+    return _factor, _proportional
+
+
 @numba.njit()
-def _rolling(a, window):
+def rolling(a, window):
     shape = (a.size - window + 1, window)
     strides = (a.itemsize, a.itemsize)
     return np.lib.stride_tricks.as_strided(a, shape=shape, strides=strides)
```

### Comparing `gfatpy-0.1.0/gfatpy/utils/plot.py` & `gfatpy-0.3.0/gfatpy/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gfatpy-0.1.0/gfatpy/utils/utils.py` & `gfatpy-0.3.0/gfatpy/utils/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from __future__ import absolute_import
 
 import re
 import os
 import sys
 from typing import Callable
 
-
 import scipy as sp
 import numpy as np
 import pandas as pd
 import datetime as dt
 from scipy import stats
 from loguru import logger
 
@@ -395,7 +394,103 @@
         return np.interp(_x, x, y)
 
     return interpolator
 
 
 def moving_average(a: np.ndarray, window_size: int = 3) -> np.ndarray:
     return sp.ndimage.uniform_filter(a, size=(window_size, 1), mode="nearest")
+
+
+def leapyear(year: int)-> bool:
+        """
+        determines whether a given year is a leap year or not
+        True iff the year is a leap year
+        """
+        return year % 4 == 0 and year % 100 != 0 or year % 400 == 0
+
+
+def zellerGregorian(d: int, m: int, a: int) -> str:
+    """determines the day of the week corresponding to a temporary
+    milestone according to the Gregorian calendar
+    """
+    # cfr. https://en.wikipedia.org/wiki/Zeller%27s_congruence
+    # cfr. https://es.wikipedia.org/wiki/Congruencia_de_Zeller
+    if m in [1,2]:
+        m += 12
+        a -= 1
+    q, m, a = d,m,a
+    J, K  = divmod(a,100)
+    c1,r1 = divmod((m+1)*26,10)
+    c2,r2 = divmod(K,4)
+    c3,r3 = divmod(J,4)
+    r = (q+c1+K+c2+c3-2*J) % 7
+    return ['sat','sun','mon','tue','wed','thu','fri'][r]
+
+
+def zellerJulian(d: int, m: int, a: int) -> str:
+    """determines the day of the week corresponding to a temporary
+    milestone according to the Julian calendar
+    """
+    # cfr https://www.timeanddate.com/calendar/?country=23
+    if m in [1,2]:
+        m += 12
+        a -= 1
+    q, m, a = d,m,a
+    J, K = divmod(a,100)
+    c1,r1 = divmod((m+1)*26,10)
+    c2,r2 = divmod(K,4)
+    r = (q+c1+K+c2+5-J) % 7
+    return ['sat','sun','mon','tue','wed','thu','fri'][r]
+
+def weekDay(s: str) -> bool:
+        weekValue = {'sat':False,
+                'sun':False,
+                'mon':True,
+                'tue':True,
+                'wed':True,
+                'thu':True,
+                'fri':True
+                }
+        return weekValue[s]
+
+
+def holyday(s: str) -> bool:
+        """
+        holyday('dd/mm/aaaa') gives 'True' iff dd/mm/ isn't in any list
+        """
+        # Dates given by: https://www.enforex.com/espanol/fiesta-espana.html
+        holydaysNat = ['01/01',
+                       '06/01',
+                       '01/05',
+                       '15/08',
+                       '12/10',
+                       '01/11',
+                       '06/12',
+                       '07/12',
+                       '08/12',
+                       '25/12']
+        holydaysReg = ['28/02']
+        holydaysLoc = ['02/11',
+                       '28/02',
+                       '15/09']
+        t = '/'.join(s.split('/')[:-1])
+        return not (t in holydaysNat or t in holydaysReg or t in holydaysLoc)
+
+def yearHolyday(s: str) -> bool:
+        """
+        We must have, and thus trust that it is, the "d/m/a" format.
+        warning('dd/mm/aa') gives True sii dd/mm/aa is weekend day 
+        or holiday
+        """
+        yearHolyday=['09/04/2020','10/04/2020','11/06/2020']
+        return not (s in yearHolyday)
+
+def warning_not_working_date(date: str) -> bool:
+        """
+        We must have, and thus trust that it is, the "dd/mm/aaaa" format.
+        warning('dd/mm/aaaa') gives True sii dd/mm/aa is weekend day 
+        or holiday
+        """
+        d,m,a = date.split('/')
+        d,m,a = int(d), int(m), int(a)
+        lyr   = d == 29 and leapyear(a) or d != 29
+        return lyr and weekDay(zellerGregorian(d,m,a)) and holyday(date) and yearHolyday(date)
```

### Comparing `gfatpy-0.1.0/pyproject.toml` & `gfatpy-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gfatpy"
-version = "0.1.0"
+version = "0.3.0"
 description = "A python package for GFAT utilities"
 # Can be extended to multiple authors
 authors = [
     "Juan Diego De la Rosa <jdidelarc@gmail.com>"
 ]
 classifiers = [
     "Intended Audience :: Science/Research",
@@ -12,41 +12,47 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
     "Development Status :: 1 - Planning"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.10,<3.12"
 numpy = "^1.23.1"
 matplotlib = "^3.5.2"
 scipy = "^1.9.0"
 scikit-learn = "^1.1.1"
 xarray = {extras = ["h5netcdf"], version = "^2022.6.0"}
 dask = "^2022.7.1"
 typer = {extras = ["all"], version = "^0.6.1"}
 PyYAML = "^6.0"
 requests = "^2.28.1"
-netCDF4 = "~1.5.7"
+netCDF4 = "^1.6.2"
 loguru = "^0.6.0"
-cloudnetpy = "^1.36.2"
+# cloudnetpy = "^1.36.2"
 pdoc = {version = "^12.0.2", optional = true }
+notebook = {version = "^6.4.12", optional = true}
+ipywidgets = {version = "^8.0.2", optional = true}
 typing-extensions = "^4.3.0"
 seaborn = "^0.12.0"
 numba = "^0.56.2"
+scikit-image = "^0.19.3"
+linc = "^1.4.0"
+pdfminer = "^20191125"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.6.0"
 pytest = "^7.1.2"
 notebook = "^6.4.12"
 pre-commit = "^2.20.0"
 ipywidgets = "^8.0.2"
 
 [tool.poetry.extras]
 docs = ["pdoc"]
+jupyter = []
 
 [tool.poetry.scripts]
 gfatpy = "gfatpy.cli.main:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gfatpy-0.1.0/setup.py` & `gfatpy-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,46 +9,53 @@
  'gfatpy.cli.lidar',
  'gfatpy.cli.lidar.plot',
  'gfatpy.cloudnet',
  'gfatpy.lidar',
  'gfatpy.lidar.depolarization',
  'gfatpy.lidar.depolarization.GHK',
  'gfatpy.lidar.depolarization.GHK.system_settings',
+ 'gfatpy.lidar.nc_convert',
  'gfatpy.lidar.plot',
  'gfatpy.lidar.preprocessing',
  'gfatpy.lidar.quality_assurance',
  'gfatpy.lidar.raw2l1',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.doc.source',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.reader',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.reader.lib',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.test',
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.tools',
  'gfatpy.lidar.retrieval',
+ 'gfatpy.radar',
+ 'gfatpy.radar.plot',
  'gfatpy.utils']
 
 package_data = \
 {'': ['*'],
  'gfatpy': ['assets/*'],
  'gfatpy.lidar.depolarization.GHK': ['tests/datos/MULHACEN/QA/GHK/2022/10/04/*'],
+ 'gfatpy.lidar.nc_convert': ['configs/*'],
  'gfatpy.lidar.raw2l1': ['config/*', 'raw2l1_gfat/*'],
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1': ['conf/*', 'doc/*'],
  'gfatpy.lidar.raw2l1.raw2l1_gfat.raw2l1.doc.source': ['_templates/*',
-                                                       'images/*']}
+                                                       'images/*'],
+ 'gfatpy.radar': ['scattering_databases/*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
- 'cloudnetpy>=1.36.2,<2.0.0',
  'dask>=2022.7.1,<2023.0.0',
+ 'linc>=1.4.0,<2.0.0',
  'loguru>=0.6.0,<0.7.0',
  'matplotlib>=3.5.2,<4.0.0',
- 'netCDF4>=1.5.7,<1.6.0',
+ 'netCDF4>=1.6.2,<2.0.0',
  'numba>=0.56.2,<0.57.0',
  'numpy>=1.23.1,<2.0.0',
+ 'pdfminer>=20191125,<20191126',
  'requests>=2.28.1,<3.0.0',
+ 'scikit-image>=0.19.3,<0.20.0',
  'scikit-learn>=1.1.1,<2.0.0',
  'scipy>=1.9.0,<2.0.0',
  'seaborn>=0.12.0,<0.13.0',
  'typer[all]>=0.6.1,<0.7.0',
  'typing-extensions>=4.3.0,<5.0.0',
  'xarray[h5netcdf]>=2022.6.0,<2023.0.0']
 
@@ -56,25 +63,25 @@
 {'docs': ['pdoc>=12.0.2,<13.0.0']}
 
 entry_points = \
 {'console_scripts': ['gfatpy = gfatpy.cli.main:app']}
 
 setup_kwargs = {
     'name': 'gfatpy',
-    'version': '0.1.0',
+    'version': '0.3.0',
     'description': 'A python package for GFAT utilities',
     'long_description': 'None',
     'author': 'Juan Diego De la Rosa',
     'author_email': 'jdidelarc@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.10,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `gfatpy-0.1.0/PKG-INFO` & `gfatpy-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 Metadata-Version: 2.1
 Name: gfatpy
-Version: 0.1.0
+Version: 0.3.0
 Summary: A python package for GFAT utilities
 Author: Juan Diego De la Rosa
 Author-email: jdidelarc@gmail.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Atmospheric Science
 Provides-Extra: docs
+Provides-Extra: jupyter
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: cloudnetpy (>=1.36.2,<2.0.0)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
+Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
+Requires-Dist: linc (>=1.4.0,<2.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
-Requires-Dist: netCDF4 (>=1.5.7,<1.6.0)
+Requires-Dist: netCDF4 (>=1.6.2,<2.0.0)
+Requires-Dist: notebook (>=6.4.12,<7.0.0)
 Requires-Dist: numba (>=0.56.2,<0.57.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: pdoc (>=12.0.2,<13.0.0); extra == "docs"
+Requires-Dist: pdfminer (>=20191125,<20191126)
+Requires-Dist: pdoc (>=12.0.2,<13.0.0) ; extra == "docs"
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: scikit-image (>=0.19.3,<0.20.0)
 Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
 Requires-Dist: xarray[h5netcdf] (>=2022.6.0,<2023.0.0)
```

