# Comparing `tmp/pydevccu-0.1.5.tar.gz` & `tmp/pydevccu-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydevccu-0.1.5.tar", last modified: Thu Jan 26 19:41:35 2023, max compression
+gzip compressed data, was "pydevccu-0.1.6.tar", last modified: Wed Apr 26 19:39:08 2023, max compression
```

## Comparing `pydevccu-0.1.5.tar` & `pydevccu-0.1.6.tar`

### file list

```diff
@@ -1,772 +1,774 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:35.795061 pydevccu-0.1.5/
--rw-rw-rw-   0        0        0      183 2019-12-29 22:52:54.000000 pydevccu-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      615 2023-01-26 19:41:35.795061 pydevccu-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4005 2020-01-01 21:54:21.000000 pydevccu-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:32.822787 pydevccu-0.1.5/pydevccu/
--rw-rw-rw-   0        0        0       39 2019-12-14 01:22:23.000000 pydevccu-0.1.5/pydevccu/__init__.py
--rw-rw-rw-   0        0        0    20446 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/ccu.py
--rw-rw-rw-   0        0        0     1458 2023-01-26 19:39:09.000000 pydevccu-0.1.5/pydevccu/const.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:34.082443 pydevccu-0.1.5/pydevccu/device_descriptions/
--rw-rw-rw-   0        0        0     1114 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_130.json
--rw-rw-rw-   0        0        0     1114 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_131.json
--rw-rw-rw-   0        0        0     1115 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_132.json
--rw-rw-rw-   0        0        0     1967 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_133.json
--rw-rw-rw-   0        0        0     1115 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_134.json
--rw-rw-rw-   0        0        0     1545 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_135.json
--rw-rw-rw-   0        0        0     2007 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_144.json
--rw-rw-rw-   0        0        0     2392 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_145.json
--rw-rw-rw-   0        0        0     1092 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_146.json
--rw-rw-rw-   0        0        0     1092 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_147.json
--rw-rw-rw-   0        0        0     9210 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_155.json
--rw-rw-rw-   0        0        0     1088 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_157.json
--rw-rw-rw-   0        0        0     1088 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_158.json
--rw-rw-rw-   0        0        0     1120 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_160.json
--rw-rw-rw-   0        0        0     1111 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_162.json
--rw-rw-rw-   0        0        0     1107 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/263_167.json
--rw-rw-rw-   0        0        0     6719 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ALPHA-IP-RBG.json
--rw-rw-rw-   0        0        0     1085 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ASH550.json
--rw-rw-rw-   0        0        0     1088 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ASH550I.json
--rw-rw-rw-   0        0        0     2381 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/BRC-H.json
--rw-rw-rw-   0        0        0     2323 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/CMM.json
--rw-rw-rw-   0        0        0     9686 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ELV-SH-BS2.json
--rw-rw-rw-   0        0        0     2050 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Bl1PBU-FM.json
--rw-rw-rw-   0        0        0     2072 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Sw1PBU-FM.json
--rw-rw-rw-   0        0        0     2498 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Sw2PBU-FM.json
--rw-rw-rw-   0        0        0     1115 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sen-PRESS.json
--rw-rw-rw-   0        0        0     3995 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sen-TEMP-DS18B20.json
--rw-rw-rw-   0        0        0     1142 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor-TH-SHT75.json
--rw-rw-rw-   0        0        0     1152 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor-THPD-BME280.json
--rw-rw-rw-   0        0        0     1119 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor1.json
--rw-rw-rw-   0        0        0     1119 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HB-WDS40-THP-O.json
--rw-rw-rw-   0        0        0     7046 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HBW-LC-RGBWW-IN6-DR.json
--rw-rw-rw-   0        0        0     3253 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-RT-DN-BoM.json
--rw-rw-rw-   0        0        0     3223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-RT-DN.json
--rw-rw-rw-   0        0        0     1126 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-SCD.json
--rw-rw-rw-   0        0        0     1948 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-TC.json
--rw-rw-rw-   0        0        0     1116 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-VD.json
--rw-rw-rw-   0        0        0     2692 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-VG-1.json
--rw-rw-rw-   0        0        0     3244 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-DW-WM.json
--rw-rw-rw-   0        0        0     3701 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-EP-WM55.json
--rw-rw-rw-   0        0        0     1136 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-TD-T.json
--rw-rw-rw-   0        0        0     4232 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-WM55.json
--rw-rw-rw-   0        0        0     3200 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-DR.json
--rw-rw-rw-   0        0        0     3248 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R1.json
--rw-rw-rw-   0        0        0     3248 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R2.json
--rw-rw-rw-   0        0        0     3248 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R3.json
--rw-rw-rw-   0        0        0     3248 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R4.json
--rw-rw-rw-   0        0        0     3248 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R5.json
--rw-rw-rw-   0        0        0     3199 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl.json
--rw-rw-rw-   0        0        0     3200 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-SM.json
--rw-rw-rw-   0        0        0     3175 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSwX.json
--rw-rw-rw-   0        0        0     1082 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-TX-WM.json
--rw-rw-rw-   0        0        0     1986 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-AO-SM.json
--rw-rw-rw-   0        0        0     1113 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-FM-2.json
--rw-rw-rw-   0        0        0     1107 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-FM.json
--rw-rw-rw-   0        0        0     1116 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-PB-FM.json
--rw-rw-rw-   0        0        0     1113 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-SM-2.json
--rw-rw-rw-   0        0        0     1107 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-SM.json
--rw-rw-rw-   0        0        0     1116 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1PBU-FM.json
--rw-rw-rw-   0        0        0     1098 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-BlX.json
--rw-rw-rw-   0        0        0     1111 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-DDC1-PCB.json
--rw-rw-rw-   0        0        0     3343 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-DW-WM.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-CV-2.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-CV.json
--rw-rw-rw-   0        0        0     1142 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-2.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-3.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl.json
--rw-rw-rw-   0        0        0     2022 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV-2.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-CV-2.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-CV.json
--rw-rw-rw-   0        0        0     2001 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-DR.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM-2.json
--rw-rw-rw-   0        0        0     1144 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM-LF.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM.json
--rw-rw-rw-   0        0        0     1142 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-2.json
--rw-rw-rw-   0        0        0     2012 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-3.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl.json
--rw-rw-rw-   0        0        0     2027 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM-2.json
--rw-rw-rw-   0        0        0     2017 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM.json
--rw-rw-rw-   0        0        0     1560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-CV.json
--rw-rw-rw-   0        0        0     3309 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-SM-2.json
--rw-rw-rw-   0        0        0     1560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-SM.json
--rw-rw-rw-   0        0        0     3309 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2T-SM-2.json
--rw-rw-rw-   0        0        0     1560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2T-SM.json
--rw-rw-rw-   0        0        0     1119 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Ja1PBU-FM.json
--rw-rw-rw-   0        0        0     1101 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-JaX.json
--rw-rw-rw-   0        0        0     2006 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-RGBW-WM.json
--rw-rw-rw-   0        0        0     1142 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Ba-PCB.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-DR.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-FM-2.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-FM.json
--rw-rw-rw-   0        0        0     1138 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-PB-FM.json
--rw-rw-rw-   0        0        0     1132 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-PCB.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-2.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-3.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R1.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R2.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R3.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R4.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R5.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R1.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R2.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R3.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R4.json
--rw-rw-rw-   0        0        0     1147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R5.json
--rw-rw-rw-   0        0        0     1145 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-OM54.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM-2.json
--rw-rw-rw-   0        0        0     1160 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM-ATmega168.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM.json
--rw-rw-rw-   0        0        0     1138 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1PBU-FM.json
--rw-rw-rw-   0        0        0     1560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-DR-2.json
--rw-rw-rw-   0        0        0     1552 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-DR.json
--rw-rw-rw-   0        0        0     1560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-FM-2.json
--rw-rw-rw-   0        0        0     1552 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-FM.json
--rw-rw-rw-   0        0        0     1564 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-PB-FM.json
--rw-rw-rw-   0        0        0     1552 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-SM.json
--rw-rw-rw-   0        0        0     1564 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2PBU-FM.json
--rw-rw-rw-   0        0        0     2422 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-Ba-PCB.json
--rw-rw-rw-   0        0        0     2410 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-DR-2.json
--rw-rw-rw-   0        0        0     2398 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-DR.json
--rw-rw-rw-   0        0        0     2416 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-PCB-2.json
--rw-rw-rw-   0        0        0     2404 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-PCB.json
--rw-rw-rw-   0        0        0     2410 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM-2.json
--rw-rw-rw-   0        0        0     2459 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM-ATmega168.json
--rw-rw-rw-   0        0        0     2398 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM.json
--rw-rw-rw-   0        0        0     2410 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-WM-2.json
--rw-rw-rw-   0        0        0     2398 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-WM.json
--rw-rw-rw-   0        0        0     1120 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-SwX.json
--rw-rw-rw-   0        0        0     1104 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-MD.json
--rw-rw-rw-   0        0        0     4130 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-EM-8.json
--rw-rw-rw-   0        0        0     2024 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-EM-8Bit.json
--rw-rw-rw-   0        0        0     4080 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-Re-8.json
--rw-rw-rw-   0        0        0     1575 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CF-Pl.json
--rw-rw-rw-   0        0        0     1597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CFM-Pl.json
--rw-rw-rw-   0        0        0     1596 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CFM-TW.json
--rw-rw-rw-   0        0        0     1148 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CM-PCB.json
--rw-rw-rw-   0        0        0     6582 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-LED16.json
--rw-rw-rw-   0        0        0     1059 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-X.json
--rw-rw-rw-   0        0        0     1557 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-FM.json
--rw-rw-rw-   0        0        0     1557 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM.json
--rw-rw-rw-   0        0        0     1573 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM55-2.json
--rw-rw-rw-   0        0        0     1565 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM55.json
--rw-rw-rw-   0        0        0     2411 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4-WM.json
--rw-rw-rw-   0        0        0     9386 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4Dis-WM-2.json
--rw-rw-rw-   0        0        0     9342 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4Dis-WM.json
--rw-rw-rw-   0        0        0     3281 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-6-WM55.json
--rw-rw-rw-   0        0        0     2416 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PBI-4-FM.json
--rw-rw-rw-   0        0        0     1123 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-PBI-X.json
--rw-rw-rw-   0        0        0     5835 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12-B.json
--rw-rw-rw-   0        0        0     5849 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12-SW.json
--rw-rw-rw-   0        0        0     5807 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12.json
--rw-rw-rw-   0        0        0     8304 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19-B.json
--rw-rw-rw-   0        0        0     8324 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19-SW.json
--rw-rw-rw-   0        0        0     8264 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19.json
--rw-rw-rw-   0        0        0     1580 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-2-PBU-FM-2.json
--rw-rw-rw-   0        0        0     1572 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-2-PBU-FM.json
--rw-rw-rw-   0        0        0     2405 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-2.json
--rw-rw-rw-   0        0        0     2417 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-3-D.json
--rw-rw-rw-   0        0        0     2405 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-3.json
--rw-rw-rw-   0        0        0     2405 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-B.json
--rw-rw-rw-   0        0        0     2393 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4.json
--rw-rw-rw-   0        0        0     4089 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-8.json
--rw-rw-rw-   0        0        0     9408 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Dis-H-x-EU.json
--rw-rw-rw-   0        0        0     1994 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key3-B.json
--rw-rw-rw-   0        0        0     1984 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key3.json
--rw-rw-rw-   0        0        0     2377 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key4-2.json
--rw-rw-rw-   0        0        0     2377 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key4-3.json
--rw-rw-rw-   0        0        0     1124 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-P1.json
--rw-rw-rw-   0        0        0     1130 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-SB-X.json
--rw-rw-rw-   0        0        0     1994 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec3-B.json
--rw-rw-rw-   0        0        0     1984 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec3.json
--rw-rw-rw-   0        0        0     2377 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec4-2.json
--rw-rw-rw-   0        0        0     2377 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec4-3.json
--rw-rw-rw-   0        0        0     1121 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-X.json
--rw-rw-rw-   0        0        0    22523 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-RCV-50.json
--rw-rw-rw-   0        0        0     2035 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-ReSC-Win-PCB-xx.json
--rw-rw-rw-   0        0        0     2095 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-SCI-3-FM.json
--rw-rw-rw-   0        0        0     1119 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-Generic.json
--rw-rw-rw-   0        0        0     1101 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-O.json
--rw-rw-rw-   0        0        0     1101 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-S.json
--rw-rw-rw-   0        0        0     1095 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key.json
--rw-rw-rw-   0        0        0     1117 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MD.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR-2.json
--rw-rw-rw-   0        0        0     1129 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR-3.json
--rw-rw-rw-   0        0        0     1123 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR.json
--rw-rw-rw-   0        0        0     2046 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-RHS-2.json
--rw-rw-rw-   0        0        0     2035 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-RHS.json
--rw-rw-rw-   0        0        0     1146 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SC-2.json
--rw-rw-rw-   0        0        0     1139 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SC.json
--rw-rw-rw-   0        0        0     1142 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SCo.json
--rw-rw-rw-   0        0        0     1149 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-2-Generic.json
--rw-rw-rw-   0        0        0     1125 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-2.json
--rw-rw-rw-   0        0        0     1138 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-Generic.json
--rw-rw-rw-   0        0        0     1114 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD.json
--rw-rw-rw-   0        0        0     1140 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SFA-SM.json
--rw-rw-rw-   0        0        0     2425 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Sir-WM.json
--rw-rw-rw-   0        0        0     1115 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-TiS.json
--rw-rw-rw-   0        0        0     1130 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-WDS-2.json
--rw-rw-rw-   0        0        0     1124 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-WDS.json
--rw-rw-rw-   0        0        0     1493 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Win-Generic.json
--rw-rw-rw-   0        0        0     1461 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Win.json
--rw-rw-rw-   0        0        0     1144 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-xx.json
--rw-rw-rw-   0        0        0     1139 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-DB-PCB.json
--rw-rw-rw-   0        0        0     1113 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-EP.json
--rw-rw-rw-   0        0        0     1076 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-LI-O.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O-2.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O-3.json
--rw-rw-rw-   0        0        0     1128 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O.json
--rw-rw-rw-   0        0        0     1131 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-SM.json
--rw-rw-rw-   0        0        0     2003 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-WM55.json
--rw-rw-rw-   0        0        0     1498 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-RD-O.json
--rw-rw-rw-   0        0        0     1128 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-Wa-Od.json
--rw-rw-rw-   0        0        0     1110 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-X.json
--rw-rw-rw-   0        0        0     2027 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-SwI-3-FM.json
--rw-rw-rw-   0        0        0     1136 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-SwI-X.json
--rw-rw-rw-   0        0        0     1081 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sys-sRP-Pl.json
--rw-rw-rw-   0        0        0     2797 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-TC-IT-WM-W-EU.json
--rw-rw-rw-   0        0        0     4804 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDC7000.json
--rw-rw-rw-   0        0        0     1106 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS10-TH-O.json
--rw-rw-rw-   0        0        0     1116 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS100-C6-O-2.json
--rw-rw-rw-   0        0        0     1110 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS100-C6-O.json
--rw-rw-rw-   0        0        0     1106 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS20-TH-O.json
--rw-rw-rw-   0        0        0     2621 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-OT2-SM-2.json
--rw-rw-rw-   0        0        0     2607 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-OT2-SM.json
--rw-rw-rw-   0        0        0     1102 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-T-O.json
--rw-rw-rw-   0        0        0     1112 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS40-TH-I-2.json
--rw-rw-rw-   0        0        0     1106 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS40-TH-I.json
--rw-rw-rw-   0        0        0     5864 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-PS.json
--rw-rw-rw-   0        0        0     7340 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-PSM.json
--rw-rw-rw-   0        0        0     2864 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-SWDO.json
--rw-rw-rw-   0        0        0     2865 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-WRC2.json
--rw-rw-rw-   0        0        0     5479 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-FM.json
--rw-rw-rw-   0        0        0    10812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-Sw14-DR.json
--rw-rw-rw-   0        0        0     8213 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-Sw7-DR.json
--rw-rw-rw-   0        0        0     2288 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-4-FM.json
--rw-rw-rw-   0        0        0     5389 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-SR-FM.json
--rw-rw-rw-   0        0        0     1888 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Bl1-DR-2.json
--rw-rw-rw-   0        0        0     1877 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Bl1-DR.json
--rw-rw-rw-   0        0        0     1889 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Dim1L-DR.json
--rw-rw-rw-   0        0        0     2270 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Sw2-DR.json
--rw-rw-rw-   0        0        0    20525 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-RCV-50.json
--rw-rw-rw-   0        0        0     5211 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-Sen-SC-12-DR.json
--rw-rw-rw-   0        0        0     5211 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HMW-Sen-SC-12-FM.json
--rw-rw-rw-   0        0        0     1111 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HSS-DX.json
--rw-rw-rw-   0        0        0     3646 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-ASIR-2.json
--rw-rw-rw-   0        0        0     3636 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-ASIR.json
--rw-rw-rw-   0        0        0     6610 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BDT.json
--rw-rw-rw-   0        0        0     2861 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BRC2.json
--rw-rw-rw-   0        0        0     6635 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BROLL.json
--rw-rw-rw-   0        0        0    12714 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BSL.json
--rw-rw-rw-   0        0        0     8081 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BSM.json
--rw-rw-rw-   0        0        0    10470 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BWTH.json
--rw-rw-rw-   0        0        0     1376 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-CCU3.json
--rw-rw-rw-   0        0        0     2121 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DBB.json
--rw-rw-rw-   0        0        0     8971 2022-01-13 17:19:05.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DLD.json
--rw-rw-rw-   0        0        0     2857 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DLS.json
--rw-rw-rw-   0        0        0    13649 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRDI3.json
--rw-rw-rw-   0        0        0     5945 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRSI1.json
--rw-rw-rw-   0        0        0    17510 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRSI4.json
--rw-rw-rw-   0        0        0     2188 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DSD-PCB.json
--rw-rw-rw-   0        0        0    12197 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FAL230-C10.json
--rw-rw-rw-   0        0        0     6607 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FBL.json
--rw-rw-rw-   0        0        0     2178 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FCI1.json
--rw-rw-rw-   0        0        0     5136 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FDT.json
--rw-rw-rw-   0        0        0     6636 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FROLL.json
--rw-rw-rw-   0        0        0     5912 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FSI16.json
--rw-rw-rw-   0        0        0     6625 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FSM16.json
--rw-rw-rw-   0        0        0     1390 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HAP.json
--rw-rw-rw-   0        0        0     2872 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HDM1.json
--rw-rw-rw-   0        0        0     2873 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HDM2.json
--rw-rw-rw-   0        0        0     4917 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HEATING.json
--rw-rw-rw-   0        0        0     4342 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-KRC4.json
--rw-rw-rw-   0        0        0     5065 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-KRCA.json
--rw-rw-rw-   0        0        0    38883 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MIO16-PCB.json
--rw-rw-rw-   0        0        0     2941 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-HO.json
--rw-rw-rw-   0        0        0    32607 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-OC8.json
--rw-rw-rw-   0        0        0     7330 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-RC8.json
--rw-rw-rw-   0        0        0     2940 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-TM.json
--rw-rw-rw-   0        0        0     8246 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MP3P.json
--rw-rw-rw-   0        0        0     5919 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS-BAT.json
--rw-rw-rw-   0        0        0     5882 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS.json
--rw-rw-rw-   0        0        0     9690 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS2.json
--rw-rw-rw-   0        0        0     2103 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PMFS.json
--rw-rw-rw-   0        0        0     7287 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RC8.json
--rw-rw-rw-   0        0        0     2123 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RCB1.json
--rw-rw-rw-   0        0        0    38416 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RCV-50.json
--rw-rw-rw-   0        0        0     1378 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RFUSB.json
--rw-rw-rw-   0        0        0     2132 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SAM.json
--rw-rw-rw-   0        0        0     2859 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SCI.json
--rw-rw-rw-   0        0        0    12692 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SCTH230.json
--rw-rw-rw-   0        0        0     5943 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SFD.json
--rw-rw-rw-   0        0        0     3596 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SLO.json
--rw-rw-rw-   0        0        0     3624 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMI.json
--rw-rw-rw-   0        0        0     4391 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMI55.json
--rw-rw-rw-   0        0        0     3635 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO-2.json
--rw-rw-rw-   0        0        0     3634 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO-A.json
--rw-rw-rw-   0        0        0     3625 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO.json
--rw-rw-rw-   0        0        0     5112 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SPDR.json
--rw-rw-rw-   0        0        0     3626 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SPI.json
--rw-rw-rw-   0        0        0     2135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SRD.json
--rw-rw-rw-   0        0        0     2870 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SRH.json
--rw-rw-rw-   0        0        0     3696 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STE2-PCB.json
--rw-rw-rw-   0        0        0     6683 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STH.json
--rw-rw-rw-   0        0        0     6693 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHD.json
--rw-rw-rw-   0        0        0     3608 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHO-A.json
--rw-rw-rw-   0        0        0     3598 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHO.json
--rw-rw-rw-   0        0        0     2856 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STV.json
--rw-rw-rw-   0        0        0     2856 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWD.json
--rw-rw-rw-   0        0        0     2867 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDM-B2.json
--rw-rw-rw-   0        0        0     2855 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDM.json
--rw-rw-rw-   0        0        0     2876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDO-I.json
--rw-rw-rw-   0        0        0     5147 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-B.json
--rw-rw-rw-   0        0        0     6683 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-PL.json
--rw-rw-rw-   0        0        0     7450 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-PR.json
--rw-rw-rw-   0        0        0     2092 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWSD.json
--rw-rw-rw-   0        0        0     7363 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-USBSM.json
--rw-rw-rw-   0        0        0     5161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WGC.json
--rw-rw-rw-   0        0        0     8190 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WHS2.json
--rw-rw-rw-   0        0        0     5815 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRC6.json
--rw-rw-rw-   0        0        0     3583 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRCD.json
--rw-rw-rw-   0        0        0     3623 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRCR.json
--rw-rw-rw-   0        0        0     6704 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WTH-1.json
--rw-rw-rw-   0        0        0     6703 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WTH-2.json
--rw-rw-rw-   0        0        0     6726 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-2 I9F.json
--rw-rw-rw-   0        0        0     6689 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-2.json
--rw-rw-rw-   0        0        0     6714 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-B.json
--rw-rw-rw-   0        0        0     6691 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-B1.json
--rw-rw-rw-   0        0        0     6709 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-C-2.json
--rw-rw-rw-   0        0        0     6692 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-E.json
--rw-rw-rw-   0        0        0     2841 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRAP.json
--rw-rw-rw-   0        0        0    14329 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRBL4.json
--rw-rw-rw-   0        0        0    11264 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRD3.json
--rw-rw-rw-   0        0        0    27565 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRI32.json
--rw-rw-rw-   0        0        0    26574 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRS8.json
--rw-rw-rw-   0        0        0     9118 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FAL230-C6.json
--rw-rw-rw-   0        0        0    13762 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FALMOT-C12.json
--rw-rw-rw-   0        0        0    25954 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FIO6.json
--rw-rw-rw-   0        0        0     5132 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-SMI55.json
--rw-rw-rw-   0        0        0     3640 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-SPI.json
--rw-rw-rw-   0        0        0     6700 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-STH.json
--rw-rw-rw-   0        0        0     6710 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-STHD.json
--rw-rw-rw-   0        0        0    12034 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-WRC6.json
--rw-rw-rw-   0        0        0     6699 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-WTH.json
--rw-rw-rw-   0        0        0     1118 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/IS-WDS-TH-OD-S-R3.json
--rw-rw-rw-   0        0        0     1083 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/KS550.json
--rw-rw-rw-   0        0        0     1089 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/KS550LC.json
--rw-rw-rw-   0        0        0     1095 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/KS550Tech.json
--rw-rw-rw-   0        0        0     1083 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/KS888.json
--rw-rw-rw-   0        0        0     3316 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/OLIGO.smart.iq.HM.json
--rw-rw-rw-   0        0        0     2375 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/RC-H.json
--rw-rw-rw-   0        0        0     1378 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/RPI-RF-MOD.json
--rw-rw-rw-   0        0        0     1084 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/S550IA.json
--rw-rw-rw-   0        0        0     4314 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ST6-SH.json
--rw-rw-rw-   0        0        0     1886 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WDF_solar.json
--rw-rw-rw-   0        0        0     4744 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WS550.json
--rw-rw-rw-   0        0        0     4780 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WS550LCB.json
--rw-rw-rw-   0        0        0     4780 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WS550LCW.json
--rw-rw-rw-   0        0        0     4792 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WS550Tech.json
--rw-rw-rw-   0        0        0     4744 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/WS888.json
--rw-rw-rw-   0        0        0     9430 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_DWT_10.json
--rw-rw-rw-   0        0        0     2056 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FDK.json
--rw-rw-rw-   0        0        0     1128 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FEP_230V.json
--rw-rw-rw-   0        0        0     1155 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FFK.json
--rw-rw-rw-   0        0        0     1134 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FSA.json
--rw-rw-rw-   0        0        0     2062 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FSS_UP3.json
--rw-rw-rw-   0        0        0     2458 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FST_UP4.json
--rw-rw-rw-   0        0        0     2004 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FWT.json
--rw-rw-rw-   0        0        0     1141 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FZS-2.json
--rw-rw-rw-   0        0        0     1135 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FZS.json
--rw-rw-rw-   0        0        0     2441 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_HS_4.json
--rw-rw-rw-   0        0        0     1577 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_WT_2.json
--rw-rw-rw-   0        0        0     1959 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/device_descriptions/atent.json
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:34.084436 pydevccu-0.1.5/pydevccu/device_logic/
--rw-rw-rw-   0        0        0     1306 2019-12-30 23:20:41.000000 pydevccu-0.1.5/pydevccu/device_logic/HM_Sec_SC_2.py
--rw-rw-rw-   0        0        0     1610 2019-12-30 23:25:18.000000 pydevccu-0.1.5/pydevccu/device_logic/HM_Sen_MDIR_WM55.py
--rw-rw-rw-   0        0        0      176 2019-12-30 23:22:53.000000 pydevccu-0.1.5/pydevccu/device_logic/__init__.py
--rw-rw-rw-   0        0        0     3229 2021-04-20 08:03:14.000000 pydevccu-0.1.5/pydevccu/get_device_data.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:35.794060 pydevccu-0.1.5/pydevccu/paramset_descriptions/
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_130.json
--rw-rw-rw-   0        0        0    17446 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_131.json
--rw-rw-rw-   0        0        0    30405 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_132.json
--rw-rw-rw-   0        0        0   112614 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_133.json
--rw-rw-rw-   0        0        0    31140 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_134.json
--rw-rw-rw-   0        0        0     6478 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_135.json
--rw-rw-rw-   0        0        0     5450 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_144.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_145.json
--rw-rw-rw-   0        0        0    27628 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_146.json
--rw-rw-rw-   0        0        0    28081 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_147.json
--rw-rw-rw-   0        0        0    49746 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_155.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_157.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_158.json
--rw-rw-rw-   0        0        0     4627 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_160.json
--rw-rw-rw-   0        0        0     5255 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_162.json
--rw-rw-rw-   0        0        0     2191 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/263_167.json
--rw-rw-rw-   0        0        0   289847 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ALPHA-IP-RBG.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ASH550.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ASH550I.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/BRC-H.json
--rw-rw-rw-   0        0        0     2399 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/CMM.json
--rw-rw-rw-   0        0        0   371150 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ELV-SH-BS2.json
--rw-rw-rw-   0        0        0    36411 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Bl1PBU-FM.json
--rw-rw-rw-   0        0        0     5796 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Sw1PBU-FM.json
--rw-rw-rw-   0        0        0     7175 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Sw2PBU-FM.json
--rw-rw-rw-   0        0        0     2820 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sen-PRESS.json
--rw-rw-rw-   0        0        0     7414 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sen-TEMP-DS18B20.json
--rw-rw-rw-   0        0        0     3015 2022-04-20 21:17:56.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor-TH-SHT75.json
--rw-rw-rw-   0        0        0     6086 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor-THPD-BME280.json
--rw-rw-rw-   0        0        0     4137 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor1.json
--rw-rw-rw-   0        0        0     2859 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-WDS40-THP-O.json
--rw-rw-rw-   0        0        0   188593 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HBW-LC-RGBWW-IN6-DR.json
--rw-rw-rw-   0        0        0    64222 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-RT-DN-BoM.json
--rw-rw-rw-   0        0        0    65656 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-RT-DN.json
--rw-rw-rw-   0        0        0     4627 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-SCD.json
--rw-rw-rw-   0        0        0    86950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-TC.json
--rw-rw-rw-   0        0        0     2646 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-VD.json
--rw-rw-rw-   0        0        0   174821 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-VG-1.json
--rw-rw-rw-   0        0        0   223840 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-DW-WM.json
--rw-rw-rw-   0        0        0    10947 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-EP-WM55.json
--rw-rw-rw-   0        0        0    16751 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-TD-T.json
--rw-rw-rw-   0        0        0    10106 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-WM55.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-DR.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R1.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R2.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R3.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R4.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R5.json
--rw-rw-rw-   0        0        0    32164 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl.json
--rw-rw-rw-   0        0        0    32761 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-SM.json
--rw-rw-rw-   0        0        0    32164 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSwX.json
--rw-rw-rw-   0        0        0     5327 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-TX-WM.json
--rw-rw-rw-   0        0        0   113755 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-AO-SM.json
--rw-rw-rw-   0        0        0    28892 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-FM-2.json
--rw-rw-rw-   0        0        0    27628 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-FM.json
--rw-rw-rw-   0        0        0    27628 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-PB-FM.json
--rw-rw-rw-   0        0        0    28892 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-SM-2.json
--rw-rw-rw-   0        0        0    27628 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-SM.json
--rw-rw-rw-   0        0        0    28081 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1PBU-FM.json
--rw-rw-rw-   0        0        0    27648 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-BlX.json
--rw-rw-rw-   0        0        0    15780 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-DDC1-PCB.json
--rw-rw-rw-   0        0        0   222574 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-DW-WM.json
--rw-rw-rw-   0        0        0   113863 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV-2.json
--rw-rw-rw-   0        0        0    28904 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV.json
--rw-rw-rw-   0        0        0    30405 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-2.json
--rw-rw-rw-   0        0        0   113863 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-3.json
--rw-rw-rw-   0        0        0    28904 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl.json
--rw-rw-rw-   0        0        0   113484 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV-2.json
--rw-rw-rw-   0        0        0   112137 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV.json
--rw-rw-rw-   0        0        0   114025 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV-2.json
--rw-rw-rw-   0        0        0    30321 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV.json
--rw-rw-rw-   0        0        0   114027 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-DR.json
--rw-rw-rw-   0        0        0   114025 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-2.json
--rw-rw-rw-   0        0        0    38429 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-LF.json
--rw-rw-rw-   0        0        0    30321 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM.json
--rw-rw-rw-   0        0        0    31140 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-2.json
--rw-rw-rw-   0        0        0   114025 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-3.json
--rw-rw-rw-   0        0        0    30321 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl.json
--rw-rw-rw-   0        0        0   113734 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM-2.json
--rw-rw-rw-   0        0        0   112614 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM.json
--rw-rw-rw-   0        0        0    56098 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-CV.json
--rw-rw-rw-   0        0        0   224824 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM-2.json
--rw-rw-rw-   0        0        0    56098 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM.json
--rw-rw-rw-   0        0        0   225148 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM-2.json
--rw-rw-rw-   0        0        0    58641 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM.json
--rw-rw-rw-   0        0        0    32227 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Ja1PBU-FM.json
--rw-rw-rw-   0        0        0    32247 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-JaX.json
--rw-rw-rw-   0        0        0    12560 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-RGBW-WM.json
--rw-rw-rw-   0        0        0    16753 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Ba-PCB.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-DR.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-FM-2.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-FM.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-PB-FM.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-PCB.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-2.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-3.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R1.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R2.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R3.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R4.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R5.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R1.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R2.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R3.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R4.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R5.json
--rw-rw-rw-   0        0        0    11839 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-OM54.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl.json
--rw-rw-rw-   0        0        0    18043 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-2.json
--rw-rw-rw-   0        0        0    11839 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-ATmega168.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM.json
--rw-rw-rw-   0        0        0    17446 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1PBU-FM.json
--rw-rw-rw-   0        0        0    32966 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-DR-2.json
--rw-rw-rw-   0        0        0    29901 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-DR.json
--rw-rw-rw-   0        0        0    32966 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-FM-2.json
--rw-rw-rw-   0        0        0    29901 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-FM.json
--rw-rw-rw-   0        0        0    29901 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-PB-FM.json
--rw-rw-rw-   0        0        0    29901 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-SM.json
--rw-rw-rw-   0        0        0    32673 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2PBU-FM.json
--rw-rw-rw-   0        0        0    58625 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-Ba-PCB.json
--rw-rw-rw-   0        0        0    62812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-DR-2.json
--rw-rw-rw-   0        0        0    57661 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-DR.json
--rw-rw-rw-   0        0        0    62812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB-2.json
--rw-rw-rw-   0        0        0    57661 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB.json
--rw-rw-rw-   0        0        0    62812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-2.json
--rw-rw-rw-   0        0        0    42955 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-ATmega168.json
--rw-rw-rw-   0        0        0    57661 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM.json
--rw-rw-rw-   0        0        0    62812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-WM-2.json
--rw-rw-rw-   0        0        0    57661 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-WM.json
--rw-rw-rw-   0        0        0    16041 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-SwX.json
--rw-rw-rw-   0        0        0     4707 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MD.json
--rw-rw-rw-   0        0        0    22333 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-EM-8.json
--rw-rw-rw-   0        0        0    12435 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-EM-8Bit.json
--rw-rw-rw-   0        0        0   114145 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-Re-8.json
--rw-rw-rw-   0        0        0    31793 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CF-Pl.json
--rw-rw-rw-   0        0        0    33812 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CFM-Pl.json
--rw-rw-rw-   0        0        0    34218 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CFM-TW.json
--rw-rw-rw-   0        0        0    18171 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CM-PCB.json
--rw-rw-rw-   0        0        0    24592 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-LED16.json
--rw-rw-rw-   0        0        0     3890 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-X.json
--rw-rw-rw-   0        0        0     7013 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-FM.json
--rw-rw-rw-   0        0        0     6478 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM.json
--rw-rw-rw-   0        0        0     6478 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM55-2.json
--rw-rw-rw-   0        0        0     6478 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM55.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4-WM.json
--rw-rw-rw-   0        0        0    49746 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4Dis-WM-2.json
--rw-rw-rw-   0        0        0    49746 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4Dis-WM.json
--rw-rw-rw-   0        0        0    16762 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-6-WM55.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PBI-4-FM.json
--rw-rw-rw-   0        0        0     4100 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PBI-X.json
--rw-rw-rw-   0        0        0    31161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12-B.json
--rw-rw-rw-   0        0        0    31161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12-SW.json
--rw-rw-rw-   0        0        0    31161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12.json
--rw-rw-rw-   0        0        0    63846 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19-B.json
--rw-rw-rw-   0        0        0    63846 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19-SW.json
--rw-rw-rw-   0        0        0    63846 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19.json
--rw-rw-rw-   0        0        0     6797 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM-2.json
--rw-rw-rw-   0        0        0     6797 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM.json
--rw-rw-rw-   0        0        0    11966 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-2.json
--rw-rw-rw-   0        0        0    11966 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-3-D.json
--rw-rw-rw-   0        0        0    11966 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-3.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-B.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4.json
--rw-rw-rw-   0        0        0    21558 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-8.json
--rw-rw-rw-   0        0        0    50893 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Dis-H-x-EU.json
--rw-rw-rw-   0        0        0     8876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key3-B.json
--rw-rw-rw-   0        0        0     8876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key3.json
--rw-rw-rw-   0        0        0    10182 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key4-2.json
--rw-rw-rw-   0        0        0    10182 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key4-3.json
--rw-rw-rw-   0        0        0     4080 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-P1.json
--rw-rw-rw-   0        0        0     4080 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-SB-X.json
--rw-rw-rw-   0        0        0     8876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec3-B.json
--rw-rw-rw-   0        0        0     8876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec3.json
--rw-rw-rw-   0        0        0    10182 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec4-2.json
--rw-rw-rw-   0        0        0    10182 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec4-3.json
--rw-rw-rw-   0        0        0     4100 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-X.json
--rw-rw-rw-   0        0        0    42669 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RCV-50.json
--rw-rw-rw-   0        0        0    30522 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ReSC-Win-PCB-xx.json
--rw-rw-rw-   0        0        0     9872 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SCI-3-FM.json
--rw-rw-rw-   0        0        0    12597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-Generic.json
--rw-rw-rw-   0        0        0    12597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-O.json
--rw-rw-rw-   0        0        0    12597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-S.json
--rw-rw-rw-   0        0        0    12597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key.json
--rw-rw-rw-   0        0        0     5255 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MD.json
--rw-rw-rw-   0        0        0     5709 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR-2.json
--rw-rw-rw-   0        0        0     5709 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR-3.json
--rw-rw-rw-   0        0        0     5255 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR.json
--rw-rw-rw-   0        0        0    13088 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-RHS-2.json
--rw-rw-rw-   0        0        0    12176 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-RHS.json
--rw-rw-rw-   0        0        0     5486 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SC-2.json
--rw-rw-rw-   0        0        0     5028 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SC.json
--rw-rw-rw-   0        0        0     5952 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SCo.json
--rw-rw-rw-   0        0        0     3596 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-2-Generic.json
--rw-rw-rw-   0        0        0     3596 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-2.json
--rw-rw-rw-   0        0        0     2681 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-Generic.json
--rw-rw-rw-   0        0        0     2681 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD.json
--rw-rw-rw-   0        0        0    20384 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SFA-SM.json
--rw-rw-rw-   0        0        0    70777 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Sir-WM.json
--rw-rw-rw-   0        0        0     4486 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-TiS.json
--rw-rw-rw-   0        0        0     5072 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-WDS-2.json
--rw-rw-rw-   0        0        0     5072 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-WDS.json
--rw-rw-rw-   0        0        0    19422 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Win-Generic.json
--rw-rw-rw-   0        0        0    19422 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Win.json
--rw-rw-rw-   0        0        0     5506 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-xx.json
--rw-rw-rw-   0        0        0     4599 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-DB-PCB.json
--rw-rw-rw-   0        0        0     4397 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-EP.json
--rw-rw-rw-   0        0        0     3892 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-LI-O.json
--rw-rw-rw-   0        0        0     5161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-2.json
--rw-rw-rw-   0        0        0     5161 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-3.json
--rw-rw-rw-   0        0        0     4707 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O.json
--rw-rw-rw-   0        0        0     4707 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-SM.json
--rw-rw-rw-   0        0        0    11107 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-WM55.json
--rw-rw-rw-   0        0        0     5363 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-RD-O.json
--rw-rw-rw-   0        0        0     7183 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-Wa-Od.json
--rw-rw-rw-   0        0        0     4417 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-X.json
--rw-rw-rw-   0        0        0     5450 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SwI-3-FM.json
--rw-rw-rw-   0        0        0     2958 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SwI-X.json
--rw-rw-rw-   0        0        0    61862 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sys-sRP-Pl.json
--rw-rw-rw-   0        0        0   151006 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-TC-IT-WM-W-EU.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDC7000.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS10-TH-O.json
--rw-rw-rw-   0        0        0     5976 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS100-C6-O-2.json
--rw-rw-rw-   0        0        0     4971 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS100-C6-O.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS20-TH-O.json
--rw-rw-rw-   0        0        0     5721 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM-2.json
--rw-rw-rw-   0        0        0     5721 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM.json
--rw-rw-rw-   0        0        0     2009 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-T-O.json
--rw-rw-rw-   0        0        0     2900 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS40-TH-I-2.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS40-TH-I.json
--rw-rw-rw-   0        0        0   406081 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-PS.json
--rw-rw-rw-   0        0        0   415403 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-PSM.json
--rw-rw-rw-   0        0        0    11399 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-SWDO.json
--rw-rw-rw-   0        0        0    13089 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-WRC2.json
--rw-rw-rw-   0        0        0    28906 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-FM.json
--rw-rw-rw-   0        0        0    18542 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-Sw14-DR.json
--rw-rw-rw-   0        0        0    89356 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-Sw7-DR.json
--rw-rw-rw-   0        0        0     9735 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-4-FM.json
--rw-rw-rw-   0        0        0    71842 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-SR-FM.json
--rw-rw-rw-   0        0        0    23301 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR-2.json
--rw-rw-rw-   0        0        0    22640 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR.json
--rw-rw-rw-   0        0        0    22534 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Dim1L-DR.json
--rw-rw-rw-   0        0        0    24051 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Sw2-DR.json
--rw-rw-rw-   0        0        0    29951 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-RCV-50.json
--rw-rw-rw-   0        0        0    10600 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-Sen-SC-12-DR.json
--rw-rw-rw-   0        0        0    10600 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-Sen-SC-12-FM.json
--rw-rw-rw-   0        0        0    28924 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HSS-DX.json
--rw-rw-rw-   0        0        0    37300 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-ASIR-2.json
--rw-rw-rw-   0        0        0    37300 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-ASIR.json
--rw-rw-rw-   0        0        0   394589 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BDT.json
--rw-rw-rw-   0        0        0    12221 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BRC2.json
--rw-rw-rw-   0        0        0   303087 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BROLL.json
--rw-rw-rw-   0        0        0   605344 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BSL.json
--rw-rw-rw-   0        0        0   313597 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BSM.json
--rw-rw-rw-   0        0        0   355786 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BWTH.json
--rw-rw-rw-   0        0        0     3203 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-CCU3.json
--rw-rw-rw-   0        0        0    10543 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DBB.json
--rw-rw-rw-   0        0        0   209377 2022-01-13 17:19:05.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DLD.json
--rw-rw-rw-   0        0        0    12598 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DLS.json
--rw-rw-rw-   0        0        0   649117 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRDI3.json
--rw-rw-rw-   0        0        0   302090 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRSI1.json
--rw-rw-rw-   0        0        0   528162 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRSI4.json
--rw-rw-rw-   0        0        0    11105 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DSD-PCB.json
--rw-rw-rw-   0        0        0    87498 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FAL230-C10.json
--rw-rw-rw-   0        0        0   313284 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FBL.json
--rw-rw-rw-   0        0        0    11557 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FCI1.json
--rw-rw-rw-   0        0        0   389543 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FDT.json
--rw-rw-rw-   0        0        0   302328 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FROLL.json
--rw-rw-rw-   0        0        0   299497 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FSI16.json
--rw-rw-rw-   0        0        0   307261 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FSM16.json
--rw-rw-rw-   0        0        0     8823 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HAP.json
--rw-rw-rw-   0        0        0   208936 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HDM1.json
--rw-rw-rw-   0        0        0   208982 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HDM2.json
--rw-rw-rw-   0        0        0   397000 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HEATING.json
--rw-rw-rw-   0        0        0    19567 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-KRC4.json
--rw-rw-rw-   0        0        0    20983 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-KRCA.json
--rw-rw-rw-   0        0        0   857060 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MIO16-PCB.json
--rw-rw-rw-   0        0        0    26069 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-HO.json
--rw-rw-rw-   0        0        0   784188 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-OC8.json
--rw-rw-rw-   0        0        0    49259 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-RC8.json
--rw-rw-rw-   0        0        0    26069 2023-01-26 19:36:51.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-TM.json
--rw-rw-rw-   0        0        0   789681 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MP3P.json
--rw-rw-rw-   0        0        0   293202 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS-BAT.json
--rw-rw-rw-   0        0        0   404136 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS.json
--rw-rw-rw-   0        0        0   363525 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS2.json
--rw-rw-rw-   0        0        0     8026 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PMFS.json
--rw-rw-rw-   0        0        0    32523 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RC8.json
--rw-rw-rw-   0        0        0    10567 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RCB1.json
--rw-rw-rw-   0        0        0    28801 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RCV-50.json
--rw-rw-rw-   0        0        0     3203 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RFUSB.json
--rw-rw-rw-   0        0        0    12290 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SAM.json
--rw-rw-rw-   0        0        0    11688 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SCI.json
--rw-rw-rw-   0        0        0   485122 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SCTH230.json
--rw-rw-rw-   0        0        0    29787 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SFD.json
--rw-rw-rw-   0        0        0    19026 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SLO.json
--rw-rw-rw-   0        0        0    15501 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMI.json
--rw-rw-rw-   0        0        0    19652 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMI55.json
--rw-rw-rw-   0        0        0    15488 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO-2.json
--rw-rw-rw-   0        0        0    15488 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO-A.json
--rw-rw-rw-   0        0        0    15488 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO.json
--rw-rw-rw-   0        0        0    20635 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SPDR.json
--rw-rw-rw-   0        0        0    16609 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SPI.json
--rw-rw-rw-   0        0        0    10623 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SRD.json
--rw-rw-rw-   0        0        0    11574 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SRH.json
--rw-rw-rw-   0        0        0    19111 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STE2-PCB.json
--rw-rw-rw-   0        0        0   290050 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STH.json
--rw-rw-rw-   0        0        0   290463 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHD.json
--rw-rw-rw-   0        0        0    17840 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHO-A.json
--rw-rw-rw-   0        0        0    17810 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHO.json
--rw-rw-rw-   0        0        0    12404 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STV.json
--rw-rw-rw-   0        0        0    13694 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWD.json
--rw-rw-rw-   0        0        0     9434 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDM-B2.json
--rw-rw-rw-   0        0        0    10567 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDM.json
--rw-rw-rw-   0        0        0    11376 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDO-I.json
--rw-rw-rw-   0        0        0    21639 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-B.json
--rw-rw-rw-   0        0        0    27212 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-PL.json
--rw-rw-rw-   0        0        0    30607 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-PR.json
--rw-rw-rw-   0        0        0    17010 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWSD.json
--rw-rw-rw-   0        0        0   309878 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-USBSM.json
--rw-rw-rw-   0        0        0    72860 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WGC.json
--rw-rw-rw-   0        0        0   366338 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WHS2.json
--rw-rw-rw-   0        0        0    23393 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRC6.json
--rw-rw-rw-   0        0        0    23729 2022-01-07 20:44:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRCD.json
--rw-rw-rw-   0        0        0    14038 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRCR.json
--rw-rw-rw-   0        0        0   290938 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WTH-1.json
--rw-rw-rw-   0        0        0   291149 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WTH-2.json
--rw-rw-rw-   0        0        0   168469 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-2 I9F.json
--rw-rw-rw-   0        0        0   168391 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-2.json
--rw-rw-rw-   0        0        0   167984 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-B.json
--rw-rw-rw-   0        0        0   166773 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-B1.json
--rw-rw-rw-   0        0        0   165736 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-C-2.json
--rw-rw-rw-   0        0        0   168681 2022-01-09 10:38:31.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-E.json
--rw-rw-rw-   0        0        0    17737 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRAP.json
--rw-rw-rw-   0        0        0   665768 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRBL4.json
--rw-rw-rw-   0        0        0   634589 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRD3.json
--rw-rw-rw-   0        0        0   164183 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRI32.json
--rw-rw-rw-   0        0        0   787762 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRS8.json
--rw-rw-rw-   0        0        0    63639 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FAL230-C6.json
--rw-rw-rw-   0        0        0   107331 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FALMOT-C12.json
--rw-rw-rw-   0        0        0   679566 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FIO6.json
--rw-rw-rw-   0        0        0    22570 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-SMI55.json
--rw-rw-rw-   0        0        0    16990 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-SPI.json
--rw-rw-rw-   0        0        0   290356 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-STH.json
--rw-rw-rw-   0        0        0   291115 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-STHD.json
--rw-rw-rw-   0        0        0   604337 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-WRC6.json
--rw-rw-rw-   0        0        0   291823 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-WTH.json
--rw-rw-rw-   0        0        0     2223 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/IS-WDS-TH-OD-S-R3.json
--rw-rw-rw-   0        0        0     4971 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550.json
--rw-rw-rw-   0        0        0     4971 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550LC.json
--rw-rw-rw-   0        0        0     4971 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550Tech.json
--rw-rw-rw-   0        0        0     4971 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/KS888.json
--rw-rw-rw-   0        0        0   220881 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/OLIGO.smart.iq.HM.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/RC-H.json
--rw-rw-rw-   0        0        0     3203 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/RPI-RF-MOD.json
--rw-rw-rw-   0        0        0     2009 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/S550IA.json
--rw-rw-rw-   0        0        0    23916 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ST6-SH.json
--rw-rw-rw-   0        0        0    72078 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WDF_solar.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550LCB.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550LCW.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550Tech.json
--rw-rw-rw-   0        0        0     2950 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/WS888.json
--rw-rw-rw-   0        0        0    49746 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_DWT_10.json
--rw-rw-rw-   0        0        0    13088 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FDK.json
--rw-rw-rw-   0        0        0    27628 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FEP_230V.json
--rw-rw-rw-   0        0        0     5486 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FFK.json
--rw-rw-rw-   0        0        0     2646 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FSA.json
--rw-rw-rw-   0        0        0     5450 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FSS_UP3.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FST_UP4.json
--rw-rw-rw-   0        0        0    87887 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FWT.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS-2.json
--rw-rw-rw-   0        0        0    16021 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS.json
--rw-rw-rw-   0        0        0    11274 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_HS_4.json
--rw-rw-rw-   0        0        0     6478 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_WT_2.json
--rw-rw-rw-   0        0        0     8876 2023-01-03 21:15:18.000000 pydevccu-0.1.5/pydevccu/paramset_descriptions/atent.json
--rw-rw-rw-   0        0        0     1017 2020-01-01 23:05:46.000000 pydevccu-0.1.5/pydevccu/proxy.py
-drwxrwxrwx   0        0        0        0 2023-01-26 19:41:32.836508 pydevccu-0.1.5/pydevccu.egg-info/
--rw-rw-rw-   0        0        0      615 2023-01-26 19:41:32.000000 pydevccu-0.1.5/pydevccu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    36165 2023-01-26 19:41:32.000000 pydevccu-0.1.5/pydevccu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 19:41:32.000000 pydevccu-0.1.5/pydevccu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-12-14 02:26:50.000000 pydevccu-0.1.5/pydevccu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-01-26 19:41:32.000000 pydevccu-0.1.5/pydevccu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-26 19:41:35.795061 pydevccu-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      998 2023-01-26 19:39:18.000000 pydevccu-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:08.064416 pydevccu-0.1.6/
+-rw-rw-rw-   0        0        0      187 2023-04-26 19:37:30.000000 pydevccu-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      615 2023-04-26 19:39:08.064416 pydevccu-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4005 2023-04-26 19:37:30.000000 pydevccu-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:04.230589 pydevccu-0.1.6/pydevccu/
+-rw-rw-rw-   0        0        0       39 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/__init__.py
+-rw-rw-rw-   0        0        0    20446 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/ccu.py
+-rw-rw-rw-   0        0        0     1522 2023-04-26 19:38:33.000000 pydevccu-0.1.6/pydevccu/const.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:05.862421 pydevccu-0.1.6/pydevccu/device_descriptions/
+-rw-rw-rw-   0        0        0     1114 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_130.json
+-rw-rw-rw-   0        0        0     1114 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_131.json
+-rw-rw-rw-   0        0        0     1115 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_132.json
+-rw-rw-rw-   0        0        0     1967 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_133.json
+-rw-rw-rw-   0        0        0     1115 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_134.json
+-rw-rw-rw-   0        0        0     1545 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_135.json
+-rw-rw-rw-   0        0        0     2007 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_144.json
+-rw-rw-rw-   0        0        0     2392 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_145.json
+-rw-rw-rw-   0        0        0     1092 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_146.json
+-rw-rw-rw-   0        0        0     1092 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_147.json
+-rw-rw-rw-   0        0        0     9210 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_155.json
+-rw-rw-rw-   0        0        0     1088 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_157.json
+-rw-rw-rw-   0        0        0     1088 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_158.json
+-rw-rw-rw-   0        0        0     1120 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_160.json
+-rw-rw-rw-   0        0        0     1111 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_162.json
+-rw-rw-rw-   0        0        0     1107 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/263_167.json
+-rw-rw-rw-   0        0        0     6719 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ALPHA-IP-RBG.json
+-rw-rw-rw-   0        0        0     1085 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ASH550.json
+-rw-rw-rw-   0        0        0     1088 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ASH550I.json
+-rw-rw-rw-   0        0        0     2381 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/BRC-H.json
+-rw-rw-rw-   0        0        0     2323 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/CMM.json
+-rw-rw-rw-   0        0        0     9686 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ELV-SH-BS2.json
+-rw-rw-rw-   0        0        0     2050 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Bl1PBU-FM.json
+-rw-rw-rw-   0        0        0     2072 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Sw1PBU-FM.json
+-rw-rw-rw-   0        0        0     2498 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Sw2PBU-FM.json
+-rw-rw-rw-   0        0        0     1115 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sen-PRESS.json
+-rw-rw-rw-   0        0        0     3995 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sen-TEMP-DS18B20.json
+-rw-rw-rw-   0        0        0     1142 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor-TH-SHT75.json
+-rw-rw-rw-   0        0        0     1152 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor-THPD-BME280.json
+-rw-rw-rw-   0        0        0     1119 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor1.json
+-rw-rw-rw-   0        0        0     1119 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HB-WDS40-THP-O.json
+-rw-rw-rw-   0        0        0     7046 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HBW-LC-RGBWW-IN6-DR.json
+-rw-rw-rw-   0        0        0     3253 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-RT-DN-BoM.json
+-rw-rw-rw-   0        0        0     3223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-RT-DN.json
+-rw-rw-rw-   0        0        0     1126 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-SCD.json
+-rw-rw-rw-   0        0        0     1948 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-TC.json
+-rw-rw-rw-   0        0        0     1116 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-VD.json
+-rw-rw-rw-   0        0        0     2692 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-VG-1.json
+-rw-rw-rw-   0        0        0     3244 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-DW-WM.json
+-rw-rw-rw-   0        0        0     3701 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-EP-WM55.json
+-rw-rw-rw-   0        0        0     1136 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-TD-T.json
+-rw-rw-rw-   0        0        0     4232 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-WM55.json
+-rw-rw-rw-   0        0        0     3200 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-DR.json
+-rw-rw-rw-   0        0        0     3248 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R1.json
+-rw-rw-rw-   0        0        0     3248 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R2.json
+-rw-rw-rw-   0        0        0     3248 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R3.json
+-rw-rw-rw-   0        0        0     3248 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R4.json
+-rw-rw-rw-   0        0        0     3248 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R5.json
+-rw-rw-rw-   0        0        0     3199 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl.json
+-rw-rw-rw-   0        0        0     3200 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-SM.json
+-rw-rw-rw-   0        0        0     3175 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSwX.json
+-rw-rw-rw-   0        0        0     1082 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-TX-WM.json
+-rw-rw-rw-   0        0        0     1986 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-AO-SM.json
+-rw-rw-rw-   0        0        0     1113 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-FM-2.json
+-rw-rw-rw-   0        0        0     1107 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-FM.json
+-rw-rw-rw-   0        0        0     1116 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-PB-FM.json
+-rw-rw-rw-   0        0        0     1113 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-SM-2.json
+-rw-rw-rw-   0        0        0     1107 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-SM.json
+-rw-rw-rw-   0        0        0     1116 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1PBU-FM.json
+-rw-rw-rw-   0        0        0     1098 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-BlX.json
+-rw-rw-rw-   0        0        0     1111 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-DDC1-PCB.json
+-rw-rw-rw-   0        0        0     3343 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-DW-WM.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-CV-2.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-CV.json
+-rw-rw-rw-   0        0        0     1142 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-2.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-3.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl.json
+-rw-rw-rw-   0        0        0     2022 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV-2.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-CV-2.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-CV.json
+-rw-rw-rw-   0        0        0     2001 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-DR.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM-2.json
+-rw-rw-rw-   0        0        0     1144 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM-LF.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM.json
+-rw-rw-rw-   0        0        0     1142 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-2.json
+-rw-rw-rw-   0        0        0     2012 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-3.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl.json
+-rw-rw-rw-   0        0        0     2027 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM-2.json
+-rw-rw-rw-   0        0        0     2017 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM.json
+-rw-rw-rw-   0        0        0     1560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-CV.json
+-rw-rw-rw-   0        0        0     3309 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-SM-2.json
+-rw-rw-rw-   0        0        0     1560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-SM.json
+-rw-rw-rw-   0        0        0     3309 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2T-SM-2.json
+-rw-rw-rw-   0        0        0     1560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2T-SM.json
+-rw-rw-rw-   0        0        0     1119 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Ja1PBU-FM.json
+-rw-rw-rw-   0        0        0     1101 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-JaX.json
+-rw-rw-rw-   0        0        0     2006 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-RGBW-WM.json
+-rw-rw-rw-   0        0        0     1142 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Ba-PCB.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-DR.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-FM-2.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-FM.json
+-rw-rw-rw-   0        0        0     1138 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-PB-FM.json
+-rw-rw-rw-   0        0        0     1132 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-PCB.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-2.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-3.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R1.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R2.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R3.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R4.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R5.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R1.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R2.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R3.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R4.json
+-rw-rw-rw-   0        0        0     1147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R5.json
+-rw-rw-rw-   0        0        0     1145 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-OM54.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM-2.json
+-rw-rw-rw-   0        0        0     1160 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM-ATmega168.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM.json
+-rw-rw-rw-   0        0        0     1138 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1PBU-FM.json
+-rw-rw-rw-   0        0        0     1560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-DR-2.json
+-rw-rw-rw-   0        0        0     1552 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-DR.json
+-rw-rw-rw-   0        0        0     1560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-FM-2.json
+-rw-rw-rw-   0        0        0     1552 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-FM.json
+-rw-rw-rw-   0        0        0     1564 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-PB-FM.json
+-rw-rw-rw-   0        0        0     1552 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-SM.json
+-rw-rw-rw-   0        0        0     1564 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2PBU-FM.json
+-rw-rw-rw-   0        0        0     2422 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-Ba-PCB.json
+-rw-rw-rw-   0        0        0     2410 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-DR-2.json
+-rw-rw-rw-   0        0        0     2398 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-DR.json
+-rw-rw-rw-   0        0        0     2416 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-PCB-2.json
+-rw-rw-rw-   0        0        0     2404 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-PCB.json
+-rw-rw-rw-   0        0        0     2410 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM-2.json
+-rw-rw-rw-   0        0        0     2459 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM-ATmega168.json
+-rw-rw-rw-   0        0        0     2398 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM.json
+-rw-rw-rw-   0        0        0     2410 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-WM-2.json
+-rw-rw-rw-   0        0        0     2398 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-WM.json
+-rw-rw-rw-   0        0        0     1120 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-SwX.json
+-rw-rw-rw-   0        0        0     1104 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-MD.json
+-rw-rw-rw-   0        0        0     4130 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-EM-8.json
+-rw-rw-rw-   0        0        0     2024 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-EM-8Bit.json
+-rw-rw-rw-   0        0        0     4080 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-Re-8.json
+-rw-rw-rw-   0        0        0     1575 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CF-Pl.json
+-rw-rw-rw-   0        0        0     1597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CFM-Pl.json
+-rw-rw-rw-   0        0        0     1596 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CFM-TW.json
+-rw-rw-rw-   0        0        0     1148 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CM-PCB.json
+-rw-rw-rw-   0        0        0     6582 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-LED16.json
+-rw-rw-rw-   0        0        0     1059 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-X.json
+-rw-rw-rw-   0        0        0     1557 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-FM.json
+-rw-rw-rw-   0        0        0     1557 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM.json
+-rw-rw-rw-   0        0        0     1573 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM55-2.json
+-rw-rw-rw-   0        0        0     1565 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM55.json
+-rw-rw-rw-   0        0        0     2411 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4-WM.json
+-rw-rw-rw-   0        0        0     9386 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4Dis-WM-2.json
+-rw-rw-rw-   0        0        0     9342 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4Dis-WM.json
+-rw-rw-rw-   0        0        0     3281 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-6-WM55.json
+-rw-rw-rw-   0        0        0     2416 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PBI-4-FM.json
+-rw-rw-rw-   0        0        0     1123 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-PBI-X.json
+-rw-rw-rw-   0        0        0     5835 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12-B.json
+-rw-rw-rw-   0        0        0     5849 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12-SW.json
+-rw-rw-rw-   0        0        0     5807 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12.json
+-rw-rw-rw-   0        0        0     8304 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19-B.json
+-rw-rw-rw-   0        0        0     8324 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19-SW.json
+-rw-rw-rw-   0        0        0     8264 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19.json
+-rw-rw-rw-   0        0        0     1580 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-2-PBU-FM-2.json
+-rw-rw-rw-   0        0        0     1572 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-2-PBU-FM.json
+-rw-rw-rw-   0        0        0     2405 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-2.json
+-rw-rw-rw-   0        0        0     2417 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-3-D.json
+-rw-rw-rw-   0        0        0     2405 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-3.json
+-rw-rw-rw-   0        0        0     2405 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-B.json
+-rw-rw-rw-   0        0        0     2393 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4.json
+-rw-rw-rw-   0        0        0     4089 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-8.json
+-rw-rw-rw-   0        0        0     9408 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Dis-H-x-EU.json
+-rw-rw-rw-   0        0        0     1994 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key3-B.json
+-rw-rw-rw-   0        0        0     1984 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key3.json
+-rw-rw-rw-   0        0        0     2377 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key4-2.json
+-rw-rw-rw-   0        0        0     2377 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key4-3.json
+-rw-rw-rw-   0        0        0     1124 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-P1.json
+-rw-rw-rw-   0        0        0     1130 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-SB-X.json
+-rw-rw-rw-   0        0        0     1994 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec3-B.json
+-rw-rw-rw-   0        0        0     1984 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec3.json
+-rw-rw-rw-   0        0        0     2377 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec4-2.json
+-rw-rw-rw-   0        0        0     2377 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec4-3.json
+-rw-rw-rw-   0        0        0     1121 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-X.json
+-rw-rw-rw-   0        0        0    22523 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-RCV-50.json
+-rw-rw-rw-   0        0        0     2035 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-ReSC-Win-PCB-xx.json
+-rw-rw-rw-   0        0        0     2095 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-SCI-3-FM.json
+-rw-rw-rw-   0        0        0     1119 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-Generic.json
+-rw-rw-rw-   0        0        0     1101 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-O.json
+-rw-rw-rw-   0        0        0     1101 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-S.json
+-rw-rw-rw-   0        0        0     1095 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key.json
+-rw-rw-rw-   0        0        0     1117 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MD.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR-2.json
+-rw-rw-rw-   0        0        0     1129 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR-3.json
+-rw-rw-rw-   0        0        0     1123 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR.json
+-rw-rw-rw-   0        0        0     2046 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-RHS-2.json
+-rw-rw-rw-   0        0        0     2035 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-RHS.json
+-rw-rw-rw-   0        0        0     1146 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SC-2.json
+-rw-rw-rw-   0        0        0     1139 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SC.json
+-rw-rw-rw-   0        0        0     1142 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SCo.json
+-rw-rw-rw-   0        0        0     1149 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-2-Generic.json
+-rw-rw-rw-   0        0        0     1125 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-2.json
+-rw-rw-rw-   0        0        0     1138 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-Generic.json
+-rw-rw-rw-   0        0        0     1114 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD.json
+-rw-rw-rw-   0        0        0     1140 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SFA-SM.json
+-rw-rw-rw-   0        0        0     2425 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Sir-WM.json
+-rw-rw-rw-   0        0        0     1115 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-TiS.json
+-rw-rw-rw-   0        0        0     1130 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-WDS-2.json
+-rw-rw-rw-   0        0        0     1124 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-WDS.json
+-rw-rw-rw-   0        0        0     1493 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Win-Generic.json
+-rw-rw-rw-   0        0        0     1461 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Win.json
+-rw-rw-rw-   0        0        0     1144 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-xx.json
+-rw-rw-rw-   0        0        0     1139 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-DB-PCB.json
+-rw-rw-rw-   0        0        0     1113 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-EP.json
+-rw-rw-rw-   0        0        0     1076 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-LI-O.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O-2.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O-3.json
+-rw-rw-rw-   0        0        0     1128 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O.json
+-rw-rw-rw-   0        0        0     1131 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-SM.json
+-rw-rw-rw-   0        0        0     2003 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-WM55.json
+-rw-rw-rw-   0        0        0     1498 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-RD-O.json
+-rw-rw-rw-   0        0        0     1128 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-Wa-Od.json
+-rw-rw-rw-   0        0        0     1110 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-X.json
+-rw-rw-rw-   0        0        0     2027 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-SwI-3-FM.json
+-rw-rw-rw-   0        0        0     1136 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-SwI-X.json
+-rw-rw-rw-   0        0        0     1081 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sys-sRP-Pl.json
+-rw-rw-rw-   0        0        0     2797 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-TC-IT-WM-W-EU.json
+-rw-rw-rw-   0        0        0     4804 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDC7000.json
+-rw-rw-rw-   0        0        0     1106 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS10-TH-O.json
+-rw-rw-rw-   0        0        0     1116 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS100-C6-O-2.json
+-rw-rw-rw-   0        0        0     1110 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS100-C6-O.json
+-rw-rw-rw-   0        0        0     1106 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS20-TH-O.json
+-rw-rw-rw-   0        0        0     2621 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-OT2-SM-2.json
+-rw-rw-rw-   0        0        0     2607 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-OT2-SM.json
+-rw-rw-rw-   0        0        0     1102 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-T-O.json
+-rw-rw-rw-   0        0        0     1112 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS40-TH-I-2.json
+-rw-rw-rw-   0        0        0     1106 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS40-TH-I.json
+-rw-rw-rw-   0        0        0     5864 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-PS.json
+-rw-rw-rw-   0        0        0     7340 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-PSM.json
+-rw-rw-rw-   0        0        0     2864 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-SWDO.json
+-rw-rw-rw-   0        0        0     2865 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-WRC2.json
+-rw-rw-rw-   0        0        0     5479 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-FM.json
+-rw-rw-rw-   0        0        0    10812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-Sw14-DR.json
+-rw-rw-rw-   0        0        0     8213 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-Sw7-DR.json
+-rw-rw-rw-   0        0        0     2288 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-4-FM.json
+-rw-rw-rw-   0        0        0     5389 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-SR-FM.json
+-rw-rw-rw-   0        0        0     1888 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Bl1-DR-2.json
+-rw-rw-rw-   0        0        0     1877 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Bl1-DR.json
+-rw-rw-rw-   0        0        0     1889 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Dim1L-DR.json
+-rw-rw-rw-   0        0        0     2270 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Sw2-DR.json
+-rw-rw-rw-   0        0        0    20525 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-RCV-50.json
+-rw-rw-rw-   0        0        0     5211 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-Sen-SC-12-DR.json
+-rw-rw-rw-   0        0        0     5211 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HMW-Sen-SC-12-FM.json
+-rw-rw-rw-   0        0        0     1111 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HSS-DX.json
+-rw-rw-rw-   0        0        0     3646 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-ASIR-2.json
+-rw-rw-rw-   0        0        0     3636 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-ASIR.json
+-rw-rw-rw-   0        0        0     6610 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BDT.json
+-rw-rw-rw-   0        0        0     2861 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BRC2.json
+-rw-rw-rw-   0        0        0     6635 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BROLL.json
+-rw-rw-rw-   0        0        0    12714 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BSL.json
+-rw-rw-rw-   0        0        0     8081 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BSM.json
+-rw-rw-rw-   0        0        0    10470 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BWTH.json
+-rw-rw-rw-   0        0        0     1376 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-CCU3.json
+-rw-rw-rw-   0        0        0     2121 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DBB.json
+-rw-rw-rw-   0        0        0     8971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DLD.json
+-rw-rw-rw-   0        0        0     2857 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DLS.json
+-rw-rw-rw-   0        0        0    13649 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRDI3.json
+-rw-rw-rw-   0        0        0     5945 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRSI1.json
+-rw-rw-rw-   0        0        0    17510 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRSI4.json
+-rw-rw-rw-   0        0        0     2188 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DSD-PCB.json
+-rw-rw-rw-   0        0        0    12197 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FAL230-C10.json
+-rw-rw-rw-   0        0        0     6607 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FBL.json
+-rw-rw-rw-   0        0        0     2178 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FCI1.json
+-rw-rw-rw-   0        0        0     5136 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FDT.json
+-rw-rw-rw-   0        0        0     6636 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FROLL.json
+-rw-rw-rw-   0        0        0     5912 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FSI16.json
+-rw-rw-rw-   0        0        0     6625 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FSM16.json
+-rw-rw-rw-   0        0        0     1390 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HAP.json
+-rw-rw-rw-   0        0        0     2872 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HDM1.json
+-rw-rw-rw-   0        0        0     2873 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HDM2.json
+-rw-rw-rw-   0        0        0     4917 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HEATING.json
+-rw-rw-rw-   0        0        0     4342 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-KRC4.json
+-rw-rw-rw-   0        0        0     5065 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-KRCA.json
+-rw-rw-rw-   0        0        0    38883 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MIO16-PCB.json
+-rw-rw-rw-   0        0        0     2941 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-HO.json
+-rw-rw-rw-   0        0        0    32607 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-OC8.json
+-rw-rw-rw-   0        0        0     7330 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-RC8.json
+-rw-rw-rw-   0        0        0     2940 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-TM.json
+-rw-rw-rw-   0        0        0     8246 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MP3P.json
+-rw-rw-rw-   0        0        0     5919 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS-BAT.json
+-rw-rw-rw-   0        0        0     5882 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS.json
+-rw-rw-rw-   0        0        0     9690 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS2.json
+-rw-rw-rw-   0        0        0     2103 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PMFS.json
+-rw-rw-rw-   0        0        0     7287 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RC8.json
+-rw-rw-rw-   0        0        0     2123 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RCB1.json
+-rw-rw-rw-   0        0        0    38416 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RCV-50.json
+-rw-rw-rw-   0        0        0     1378 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RFUSB.json
+-rw-rw-rw-   0        0        0     5224 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RGBW.json
+-rw-rw-rw-   0        0        0     2132 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SAM.json
+-rw-rw-rw-   0        0        0     2859 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SCI.json
+-rw-rw-rw-   0        0        0    12692 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SCTH230.json
+-rw-rw-rw-   0        0        0     5943 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SFD.json
+-rw-rw-rw-   0        0        0     3596 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SLO.json
+-rw-rw-rw-   0        0        0     3624 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMI.json
+-rw-rw-rw-   0        0        0     4391 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMI55.json
+-rw-rw-rw-   0        0        0     3635 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO-2.json
+-rw-rw-rw-   0        0        0     3634 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO-A.json
+-rw-rw-rw-   0        0        0     3625 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO.json
+-rw-rw-rw-   0        0        0     5112 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SPDR.json
+-rw-rw-rw-   0        0        0     3626 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SPI.json
+-rw-rw-rw-   0        0        0     2135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SRD.json
+-rw-rw-rw-   0        0        0     2870 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SRH.json
+-rw-rw-rw-   0        0        0     3696 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STE2-PCB.json
+-rw-rw-rw-   0        0        0     6683 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STH.json
+-rw-rw-rw-   0        0        0     6693 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHD.json
+-rw-rw-rw-   0        0        0     3608 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHO-A.json
+-rw-rw-rw-   0        0        0     3598 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHO.json
+-rw-rw-rw-   0        0        0     2856 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STV.json
+-rw-rw-rw-   0        0        0     2856 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWD.json
+-rw-rw-rw-   0        0        0     2867 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDM-B2.json
+-rw-rw-rw-   0        0        0     2855 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDM.json
+-rw-rw-rw-   0        0        0     2876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDO-I.json
+-rw-rw-rw-   0        0        0     5147 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-B.json
+-rw-rw-rw-   0        0        0     6683 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-PL.json
+-rw-rw-rw-   0        0        0     7450 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-PR.json
+-rw-rw-rw-   0        0        0     2092 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWSD.json
+-rw-rw-rw-   0        0        0     7363 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-USBSM.json
+-rw-rw-rw-   0        0        0     5161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WGC.json
+-rw-rw-rw-   0        0        0     8190 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WHS2.json
+-rw-rw-rw-   0        0        0     5815 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRC6.json
+-rw-rw-rw-   0        0        0     3583 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRCD.json
+-rw-rw-rw-   0        0        0     3623 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRCR.json
+-rw-rw-rw-   0        0        0     6704 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WTH-1.json
+-rw-rw-rw-   0        0        0     6703 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WTH-2.json
+-rw-rw-rw-   0        0        0     6726 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-2 I9F.json
+-rw-rw-rw-   0        0        0     6689 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-2.json
+-rw-rw-rw-   0        0        0     6714 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-B.json
+-rw-rw-rw-   0        0        0     6691 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-B1.json
+-rw-rw-rw-   0        0        0     6709 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-C-2.json
+-rw-rw-rw-   0        0        0     6692 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-E.json
+-rw-rw-rw-   0        0        0     2841 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRAP.json
+-rw-rw-rw-   0        0        0    14329 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRBL4.json
+-rw-rw-rw-   0        0        0    11264 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRD3.json
+-rw-rw-rw-   0        0        0    27565 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRI32.json
+-rw-rw-rw-   0        0        0    26574 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRS8.json
+-rw-rw-rw-   0        0        0     9118 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FAL230-C6.json
+-rw-rw-rw-   0        0        0    13762 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FALMOT-C12.json
+-rw-rw-rw-   0        0        0    25954 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FIO6.json
+-rw-rw-rw-   0        0        0     5132 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-SMI55.json
+-rw-rw-rw-   0        0        0     3640 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-SPI.json
+-rw-rw-rw-   0        0        0     6700 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-STH.json
+-rw-rw-rw-   0        0        0     6710 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-STHD.json
+-rw-rw-rw-   0        0        0    12034 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-WRC6.json
+-rw-rw-rw-   0        0        0     6699 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-WTH.json
+-rw-rw-rw-   0        0        0     1118 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/IS-WDS-TH-OD-S-R3.json
+-rw-rw-rw-   0        0        0     1083 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/KS550.json
+-rw-rw-rw-   0        0        0     1089 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/KS550LC.json
+-rw-rw-rw-   0        0        0     1095 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/KS550Tech.json
+-rw-rw-rw-   0        0        0     1083 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/KS888.json
+-rw-rw-rw-   0        0        0     3316 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/OLIGO.smart.iq.HM.json
+-rw-rw-rw-   0        0        0     2375 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/RC-H.json
+-rw-rw-rw-   0        0        0     1378 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/RPI-RF-MOD.json
+-rw-rw-rw-   0        0        0     1084 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/S550IA.json
+-rw-rw-rw-   0        0        0     4314 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ST6-SH.json
+-rw-rw-rw-   0        0        0     1886 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WDF_solar.json
+-rw-rw-rw-   0        0        0     4744 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WS550.json
+-rw-rw-rw-   0        0        0     4780 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WS550LCB.json
+-rw-rw-rw-   0        0        0     4780 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WS550LCW.json
+-rw-rw-rw-   0        0        0     4792 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WS550Tech.json
+-rw-rw-rw-   0        0        0     4744 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/WS888.json
+-rw-rw-rw-   0        0        0     9430 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_DWT_10.json
+-rw-rw-rw-   0        0        0     2056 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FDK.json
+-rw-rw-rw-   0        0        0     1128 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FEP_230V.json
+-rw-rw-rw-   0        0        0     1155 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FFK.json
+-rw-rw-rw-   0        0        0     1134 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FSA.json
+-rw-rw-rw-   0        0        0     2062 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FSS_UP3.json
+-rw-rw-rw-   0        0        0     2458 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FST_UP4.json
+-rw-rw-rw-   0        0        0     2004 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FWT.json
+-rw-rw-rw-   0        0        0     1141 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FZS-2.json
+-rw-rw-rw-   0        0        0     1135 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FZS.json
+-rw-rw-rw-   0        0        0     2441 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_HS_4.json
+-rw-rw-rw-   0        0        0     1577 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_WT_2.json
+-rw-rw-rw-   0        0        0     1959 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_descriptions/atent.json
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:05.864414 pydevccu-0.1.6/pydevccu/device_logic/
+-rw-rw-rw-   0        0        0     1345 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_logic/HM_Sec_SC_2.py
+-rw-rw-rw-   0        0        0     1652 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_logic/HM_Sen_MDIR_WM55.py
+-rw-rw-rw-   0        0        0      183 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/device_logic/__init__.py
+-rw-rw-rw-   0        0        0     3303 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/get_device_data.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:08.064416 pydevccu-0.1.6/pydevccu/paramset_descriptions/
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_130.json
+-rw-rw-rw-   0        0        0    17446 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_131.json
+-rw-rw-rw-   0        0        0    30405 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_132.json
+-rw-rw-rw-   0        0        0   112614 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_133.json
+-rw-rw-rw-   0        0        0    31140 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_134.json
+-rw-rw-rw-   0        0        0     6478 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_135.json
+-rw-rw-rw-   0        0        0     5450 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_144.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_145.json
+-rw-rw-rw-   0        0        0    27628 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_146.json
+-rw-rw-rw-   0        0        0    28081 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_147.json
+-rw-rw-rw-   0        0        0    49746 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_155.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_157.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_158.json
+-rw-rw-rw-   0        0        0     4627 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_160.json
+-rw-rw-rw-   0        0        0     5255 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_162.json
+-rw-rw-rw-   0        0        0     2191 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/263_167.json
+-rw-rw-rw-   0        0        0   289847 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ALPHA-IP-RBG.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ASH550.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ASH550I.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/BRC-H.json
+-rw-rw-rw-   0        0        0     2399 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/CMM.json
+-rw-rw-rw-   0        0        0   371150 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ELV-SH-BS2.json
+-rw-rw-rw-   0        0        0    36411 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Bl1PBU-FM.json
+-rw-rw-rw-   0        0        0     5796 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Sw1PBU-FM.json
+-rw-rw-rw-   0        0        0     7175 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Sw2PBU-FM.json
+-rw-rw-rw-   0        0        0     2820 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sen-PRESS.json
+-rw-rw-rw-   0        0        0     7414 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sen-TEMP-DS18B20.json
+-rw-rw-rw-   0        0        0     3015 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor-TH-SHT75.json
+-rw-rw-rw-   0        0        0     6086 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor-THPD-BME280.json
+-rw-rw-rw-   0        0        0     4137 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor1.json
+-rw-rw-rw-   0        0        0     2859 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-WDS40-THP-O.json
+-rw-rw-rw-   0        0        0   188593 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HBW-LC-RGBWW-IN6-DR.json
+-rw-rw-rw-   0        0        0    64222 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-RT-DN-BoM.json
+-rw-rw-rw-   0        0        0    65656 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-RT-DN.json
+-rw-rw-rw-   0        0        0     4627 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-SCD.json
+-rw-rw-rw-   0        0        0    86950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-TC.json
+-rw-rw-rw-   0        0        0     2646 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-VD.json
+-rw-rw-rw-   0        0        0   174821 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-VG-1.json
+-rw-rw-rw-   0        0        0   223840 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-DW-WM.json
+-rw-rw-rw-   0        0        0    10947 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-EP-WM55.json
+-rw-rw-rw-   0        0        0    16751 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-TD-T.json
+-rw-rw-rw-   0        0        0    10106 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-WM55.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-DR.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R1.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R2.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R3.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R4.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R5.json
+-rw-rw-rw-   0        0        0    32164 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl.json
+-rw-rw-rw-   0        0        0    32761 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-SM.json
+-rw-rw-rw-   0        0        0    32164 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSwX.json
+-rw-rw-rw-   0        0        0     5327 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-TX-WM.json
+-rw-rw-rw-   0        0        0   113755 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-AO-SM.json
+-rw-rw-rw-   0        0        0    28892 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-FM-2.json
+-rw-rw-rw-   0        0        0    27628 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-FM.json
+-rw-rw-rw-   0        0        0    27628 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-PB-FM.json
+-rw-rw-rw-   0        0        0    28892 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-SM-2.json
+-rw-rw-rw-   0        0        0    27628 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-SM.json
+-rw-rw-rw-   0        0        0    28081 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1PBU-FM.json
+-rw-rw-rw-   0        0        0    27648 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-BlX.json
+-rw-rw-rw-   0        0        0    15780 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-DDC1-PCB.json
+-rw-rw-rw-   0        0        0   222574 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-DW-WM.json
+-rw-rw-rw-   0        0        0   113863 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV-2.json
+-rw-rw-rw-   0        0        0    28904 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV.json
+-rw-rw-rw-   0        0        0    30405 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-2.json
+-rw-rw-rw-   0        0        0   113863 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-3.json
+-rw-rw-rw-   0        0        0    28904 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl.json
+-rw-rw-rw-   0        0        0   113484 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV-2.json
+-rw-rw-rw-   0        0        0   112137 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV.json
+-rw-rw-rw-   0        0        0   114025 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV-2.json
+-rw-rw-rw-   0        0        0    30321 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV.json
+-rw-rw-rw-   0        0        0   114027 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-DR.json
+-rw-rw-rw-   0        0        0   114025 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-2.json
+-rw-rw-rw-   0        0        0    38429 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-LF.json
+-rw-rw-rw-   0        0        0    30321 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM.json
+-rw-rw-rw-   0        0        0    31140 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-2.json
+-rw-rw-rw-   0        0        0   114025 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-3.json
+-rw-rw-rw-   0        0        0    30321 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl.json
+-rw-rw-rw-   0        0        0   113734 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM-2.json
+-rw-rw-rw-   0        0        0   112614 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM.json
+-rw-rw-rw-   0        0        0    56098 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-CV.json
+-rw-rw-rw-   0        0        0   224824 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM-2.json
+-rw-rw-rw-   0        0        0    56098 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM.json
+-rw-rw-rw-   0        0        0   225148 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM-2.json
+-rw-rw-rw-   0        0        0    58641 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM.json
+-rw-rw-rw-   0        0        0    32227 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Ja1PBU-FM.json
+-rw-rw-rw-   0        0        0    32247 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-JaX.json
+-rw-rw-rw-   0        0        0    12560 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-RGBW-WM.json
+-rw-rw-rw-   0        0        0    16753 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Ba-PCB.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-DR.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-FM-2.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-FM.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-PB-FM.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-PCB.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-2.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-3.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R1.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R2.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R3.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R4.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R5.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R1.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R2.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R3.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R4.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R5.json
+-rw-rw-rw-   0        0        0    11839 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-OM54.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl.json
+-rw-rw-rw-   0        0        0    18043 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-2.json
+-rw-rw-rw-   0        0        0    11839 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-ATmega168.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM.json
+-rw-rw-rw-   0        0        0    17446 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1PBU-FM.json
+-rw-rw-rw-   0        0        0    32966 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-DR-2.json
+-rw-rw-rw-   0        0        0    29901 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-DR.json
+-rw-rw-rw-   0        0        0    32966 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-FM-2.json
+-rw-rw-rw-   0        0        0    29901 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-FM.json
+-rw-rw-rw-   0        0        0    29901 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-PB-FM.json
+-rw-rw-rw-   0        0        0    29901 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-SM.json
+-rw-rw-rw-   0        0        0    32673 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2PBU-FM.json
+-rw-rw-rw-   0        0        0    58625 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-Ba-PCB.json
+-rw-rw-rw-   0        0        0    62812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-DR-2.json
+-rw-rw-rw-   0        0        0    57661 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-DR.json
+-rw-rw-rw-   0        0        0    62812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB-2.json
+-rw-rw-rw-   0        0        0    57661 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB.json
+-rw-rw-rw-   0        0        0    62812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-2.json
+-rw-rw-rw-   0        0        0    42955 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-ATmega168.json
+-rw-rw-rw-   0        0        0    57661 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM.json
+-rw-rw-rw-   0        0        0    62812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-WM-2.json
+-rw-rw-rw-   0        0        0    57661 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-WM.json
+-rw-rw-rw-   0        0        0    16041 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-SwX.json
+-rw-rw-rw-   0        0        0     4707 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MD.json
+-rw-rw-rw-   0        0        0    22333 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-EM-8.json
+-rw-rw-rw-   0        0        0    12435 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-EM-8Bit.json
+-rw-rw-rw-   0        0        0   114145 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-Re-8.json
+-rw-rw-rw-   0        0        0    31793 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CF-Pl.json
+-rw-rw-rw-   0        0        0    33812 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CFM-Pl.json
+-rw-rw-rw-   0        0        0    34218 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CFM-TW.json
+-rw-rw-rw-   0        0        0    18171 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CM-PCB.json
+-rw-rw-rw-   0        0        0    24592 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-LED16.json
+-rw-rw-rw-   0        0        0     3890 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-X.json
+-rw-rw-rw-   0        0        0     7013 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-FM.json
+-rw-rw-rw-   0        0        0     6478 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM.json
+-rw-rw-rw-   0        0        0     6478 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM55-2.json
+-rw-rw-rw-   0        0        0     6478 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM55.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4-WM.json
+-rw-rw-rw-   0        0        0    49746 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4Dis-WM-2.json
+-rw-rw-rw-   0        0        0    49746 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4Dis-WM.json
+-rw-rw-rw-   0        0        0    16762 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-6-WM55.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PBI-4-FM.json
+-rw-rw-rw-   0        0        0     4100 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PBI-X.json
+-rw-rw-rw-   0        0        0    31161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12-B.json
+-rw-rw-rw-   0        0        0    31161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12-SW.json
+-rw-rw-rw-   0        0        0    31161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12.json
+-rw-rw-rw-   0        0        0    63846 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19-B.json
+-rw-rw-rw-   0        0        0    63846 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19-SW.json
+-rw-rw-rw-   0        0        0    63846 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19.json
+-rw-rw-rw-   0        0        0     6797 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM-2.json
+-rw-rw-rw-   0        0        0     6797 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM.json
+-rw-rw-rw-   0        0        0    11966 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-2.json
+-rw-rw-rw-   0        0        0    11966 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-3-D.json
+-rw-rw-rw-   0        0        0    11966 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-3.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-B.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4.json
+-rw-rw-rw-   0        0        0    21558 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-8.json
+-rw-rw-rw-   0        0        0    50893 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Dis-H-x-EU.json
+-rw-rw-rw-   0        0        0     8876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key3-B.json
+-rw-rw-rw-   0        0        0     8876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key3.json
+-rw-rw-rw-   0        0        0    10182 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key4-2.json
+-rw-rw-rw-   0        0        0    10182 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key4-3.json
+-rw-rw-rw-   0        0        0     4080 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-P1.json
+-rw-rw-rw-   0        0        0     4080 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-SB-X.json
+-rw-rw-rw-   0        0        0     8876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec3-B.json
+-rw-rw-rw-   0        0        0     8876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec3.json
+-rw-rw-rw-   0        0        0    10182 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec4-2.json
+-rw-rw-rw-   0        0        0    10182 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec4-3.json
+-rw-rw-rw-   0        0        0     4100 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-X.json
+-rw-rw-rw-   0        0        0    42669 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RCV-50.json
+-rw-rw-rw-   0        0        0    30522 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ReSC-Win-PCB-xx.json
+-rw-rw-rw-   0        0        0     9872 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SCI-3-FM.json
+-rw-rw-rw-   0        0        0    12597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-Generic.json
+-rw-rw-rw-   0        0        0    12597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-O.json
+-rw-rw-rw-   0        0        0    12597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-S.json
+-rw-rw-rw-   0        0        0    12597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key.json
+-rw-rw-rw-   0        0        0     5255 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MD.json
+-rw-rw-rw-   0        0        0     5709 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR-2.json
+-rw-rw-rw-   0        0        0     5709 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR-3.json
+-rw-rw-rw-   0        0        0     5255 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR.json
+-rw-rw-rw-   0        0        0    13088 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-RHS-2.json
+-rw-rw-rw-   0        0        0    12176 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-RHS.json
+-rw-rw-rw-   0        0        0     5486 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SC-2.json
+-rw-rw-rw-   0        0        0     5028 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SC.json
+-rw-rw-rw-   0        0        0     5952 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SCo.json
+-rw-rw-rw-   0        0        0     3596 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-2-Generic.json
+-rw-rw-rw-   0        0        0     3596 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-2.json
+-rw-rw-rw-   0        0        0     2681 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-Generic.json
+-rw-rw-rw-   0        0        0     2681 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD.json
+-rw-rw-rw-   0        0        0    20384 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SFA-SM.json
+-rw-rw-rw-   0        0        0    70777 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Sir-WM.json
+-rw-rw-rw-   0        0        0     4486 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-TiS.json
+-rw-rw-rw-   0        0        0     5072 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-WDS-2.json
+-rw-rw-rw-   0        0        0     5072 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-WDS.json
+-rw-rw-rw-   0        0        0    19422 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Win-Generic.json
+-rw-rw-rw-   0        0        0    19422 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Win.json
+-rw-rw-rw-   0        0        0     5506 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-xx.json
+-rw-rw-rw-   0        0        0     4599 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-DB-PCB.json
+-rw-rw-rw-   0        0        0     4397 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-EP.json
+-rw-rw-rw-   0        0        0     3892 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-LI-O.json
+-rw-rw-rw-   0        0        0     5161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-2.json
+-rw-rw-rw-   0        0        0     5161 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-3.json
+-rw-rw-rw-   0        0        0     4707 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O.json
+-rw-rw-rw-   0        0        0     4707 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-SM.json
+-rw-rw-rw-   0        0        0    11107 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-WM55.json
+-rw-rw-rw-   0        0        0     5363 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-RD-O.json
+-rw-rw-rw-   0        0        0     7183 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-Wa-Od.json
+-rw-rw-rw-   0        0        0     4417 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-X.json
+-rw-rw-rw-   0        0        0     5450 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SwI-3-FM.json
+-rw-rw-rw-   0        0        0     2958 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SwI-X.json
+-rw-rw-rw-   0        0        0    61862 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sys-sRP-Pl.json
+-rw-rw-rw-   0        0        0   151006 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-TC-IT-WM-W-EU.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDC7000.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS10-TH-O.json
+-rw-rw-rw-   0        0        0     5976 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS100-C6-O-2.json
+-rw-rw-rw-   0        0        0     4971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS100-C6-O.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS20-TH-O.json
+-rw-rw-rw-   0        0        0     5721 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM-2.json
+-rw-rw-rw-   0        0        0     5721 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM.json
+-rw-rw-rw-   0        0        0     2009 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-T-O.json
+-rw-rw-rw-   0        0        0     2900 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS40-TH-I-2.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS40-TH-I.json
+-rw-rw-rw-   0        0        0   406081 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-PS.json
+-rw-rw-rw-   0        0        0   415403 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-PSM.json
+-rw-rw-rw-   0        0        0    11399 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-SWDO.json
+-rw-rw-rw-   0        0        0    13089 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-WRC2.json
+-rw-rw-rw-   0        0        0    28906 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-FM.json
+-rw-rw-rw-   0        0        0    18542 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-Sw14-DR.json
+-rw-rw-rw-   0        0        0    89356 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-Sw7-DR.json
+-rw-rw-rw-   0        0        0     9735 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-4-FM.json
+-rw-rw-rw-   0        0        0    71842 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-SR-FM.json
+-rw-rw-rw-   0        0        0    23301 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR-2.json
+-rw-rw-rw-   0        0        0    22640 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR.json
+-rw-rw-rw-   0        0        0    22534 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Dim1L-DR.json
+-rw-rw-rw-   0        0        0    24051 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Sw2-DR.json
+-rw-rw-rw-   0        0        0    29951 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-RCV-50.json
+-rw-rw-rw-   0        0        0    10600 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-Sen-SC-12-DR.json
+-rw-rw-rw-   0        0        0    10600 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-Sen-SC-12-FM.json
+-rw-rw-rw-   0        0        0    28924 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HSS-DX.json
+-rw-rw-rw-   0        0        0    37300 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-ASIR-2.json
+-rw-rw-rw-   0        0        0    37300 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-ASIR.json
+-rw-rw-rw-   0        0        0   394589 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BDT.json
+-rw-rw-rw-   0        0        0    12221 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BRC2.json
+-rw-rw-rw-   0        0        0   303087 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BROLL.json
+-rw-rw-rw-   0        0        0   605344 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BSL.json
+-rw-rw-rw-   0        0        0   313597 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BSM.json
+-rw-rw-rw-   0        0        0   355786 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BWTH.json
+-rw-rw-rw-   0        0        0     3203 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-CCU3.json
+-rw-rw-rw-   0        0        0    10543 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DBB.json
+-rw-rw-rw-   0        0        0   209377 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DLD.json
+-rw-rw-rw-   0        0        0    12598 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DLS.json
+-rw-rw-rw-   0        0        0   649117 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRDI3.json
+-rw-rw-rw-   0        0        0   302090 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRSI1.json
+-rw-rw-rw-   0        0        0   528162 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRSI4.json
+-rw-rw-rw-   0        0        0    11105 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DSD-PCB.json
+-rw-rw-rw-   0        0        0    87498 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FAL230-C10.json
+-rw-rw-rw-   0        0        0   313284 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FBL.json
+-rw-rw-rw-   0        0        0    11557 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FCI1.json
+-rw-rw-rw-   0        0        0   389543 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FDT.json
+-rw-rw-rw-   0        0        0   302328 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FROLL.json
+-rw-rw-rw-   0        0        0   299497 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FSI16.json
+-rw-rw-rw-   0        0        0   307261 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FSM16.json
+-rw-rw-rw-   0        0        0     8823 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HAP.json
+-rw-rw-rw-   0        0        0   208936 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HDM1.json
+-rw-rw-rw-   0        0        0   208982 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HDM2.json
+-rw-rw-rw-   0        0        0   397000 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HEATING.json
+-rw-rw-rw-   0        0        0    19567 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-KRC4.json
+-rw-rw-rw-   0        0        0    20983 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-KRCA.json
+-rw-rw-rw-   0        0        0   857060 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MIO16-PCB.json
+-rw-rw-rw-   0        0        0    26069 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-HO.json
+-rw-rw-rw-   0        0        0   784188 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-OC8.json
+-rw-rw-rw-   0        0        0    49259 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-RC8.json
+-rw-rw-rw-   0        0        0    26069 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-TM.json
+-rw-rw-rw-   0        0        0   789681 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MP3P.json
+-rw-rw-rw-   0        0        0   293202 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS-BAT.json
+-rw-rw-rw-   0        0        0   404136 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS.json
+-rw-rw-rw-   0        0        0   363525 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS2.json
+-rw-rw-rw-   0        0        0     8026 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PMFS.json
+-rw-rw-rw-   0        0        0    32523 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RC8.json
+-rw-rw-rw-   0        0        0    10567 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RCB1.json
+-rw-rw-rw-   0        0        0    28801 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RCV-50.json
+-rw-rw-rw-   0        0        0     3203 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RFUSB.json
+-rw-rw-rw-   0        0        0   741153 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RGBW.json
+-rw-rw-rw-   0        0        0    12290 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SAM.json
+-rw-rw-rw-   0        0        0    11688 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SCI.json
+-rw-rw-rw-   0        0        0   485122 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SCTH230.json
+-rw-rw-rw-   0        0        0    29787 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SFD.json
+-rw-rw-rw-   0        0        0    19026 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SLO.json
+-rw-rw-rw-   0        0        0    15501 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMI.json
+-rw-rw-rw-   0        0        0    19652 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMI55.json
+-rw-rw-rw-   0        0        0    15488 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO-2.json
+-rw-rw-rw-   0        0        0    15488 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO-A.json
+-rw-rw-rw-   0        0        0    15488 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO.json
+-rw-rw-rw-   0        0        0    20635 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SPDR.json
+-rw-rw-rw-   0        0        0    16609 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SPI.json
+-rw-rw-rw-   0        0        0    10623 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SRD.json
+-rw-rw-rw-   0        0        0    11574 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SRH.json
+-rw-rw-rw-   0        0        0    19111 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STE2-PCB.json
+-rw-rw-rw-   0        0        0   290050 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STH.json
+-rw-rw-rw-   0        0        0   290463 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHD.json
+-rw-rw-rw-   0        0        0    17840 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHO-A.json
+-rw-rw-rw-   0        0        0    17810 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHO.json
+-rw-rw-rw-   0        0        0    12404 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STV.json
+-rw-rw-rw-   0        0        0    13694 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWD.json
+-rw-rw-rw-   0        0        0     9434 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDM-B2.json
+-rw-rw-rw-   0        0        0    10567 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDM.json
+-rw-rw-rw-   0        0        0    11376 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDO-I.json
+-rw-rw-rw-   0        0        0    21639 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-B.json
+-rw-rw-rw-   0        0        0    27212 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-PL.json
+-rw-rw-rw-   0        0        0    30607 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-PR.json
+-rw-rw-rw-   0        0        0    17010 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWSD.json
+-rw-rw-rw-   0        0        0   309878 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-USBSM.json
+-rw-rw-rw-   0        0        0    72860 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WGC.json
+-rw-rw-rw-   0        0        0   366338 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WHS2.json
+-rw-rw-rw-   0        0        0    23393 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRC6.json
+-rw-rw-rw-   0        0        0    23729 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRCD.json
+-rw-rw-rw-   0        0        0    14038 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRCR.json
+-rw-rw-rw-   0        0        0   290938 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WTH-1.json
+-rw-rw-rw-   0        0        0   291149 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WTH-2.json
+-rw-rw-rw-   0        0        0   168469 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-2 I9F.json
+-rw-rw-rw-   0        0        0   168391 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-2.json
+-rw-rw-rw-   0        0        0   167984 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-B.json
+-rw-rw-rw-   0        0        0   166773 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-B1.json
+-rw-rw-rw-   0        0        0   165736 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-C-2.json
+-rw-rw-rw-   0        0        0   168681 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-E.json
+-rw-rw-rw-   0        0        0    17737 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRAP.json
+-rw-rw-rw-   0        0        0   665768 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRBL4.json
+-rw-rw-rw-   0        0        0   634589 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRD3.json
+-rw-rw-rw-   0        0        0   164183 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRI32.json
+-rw-rw-rw-   0        0        0   787762 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRS8.json
+-rw-rw-rw-   0        0        0    63639 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FAL230-C6.json
+-rw-rw-rw-   0        0        0   107331 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FALMOT-C12.json
+-rw-rw-rw-   0        0        0   679566 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FIO6.json
+-rw-rw-rw-   0        0        0    22570 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-SMI55.json
+-rw-rw-rw-   0        0        0    16990 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-SPI.json
+-rw-rw-rw-   0        0        0   290356 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-STH.json
+-rw-rw-rw-   0        0        0   291115 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-STHD.json
+-rw-rw-rw-   0        0        0   604337 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-WRC6.json
+-rw-rw-rw-   0        0        0   291823 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-WTH.json
+-rw-rw-rw-   0        0        0     2223 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/IS-WDS-TH-OD-S-R3.json
+-rw-rw-rw-   0        0        0     4971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550.json
+-rw-rw-rw-   0        0        0     4971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550LC.json
+-rw-rw-rw-   0        0        0     4971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550Tech.json
+-rw-rw-rw-   0        0        0     4971 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/KS888.json
+-rw-rw-rw-   0        0        0   220881 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/OLIGO.smart.iq.HM.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/RC-H.json
+-rw-rw-rw-   0        0        0     3203 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/RPI-RF-MOD.json
+-rw-rw-rw-   0        0        0     2009 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/S550IA.json
+-rw-rw-rw-   0        0        0    23916 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ST6-SH.json
+-rw-rw-rw-   0        0        0    72078 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WDF_solar.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550LCB.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550LCW.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550Tech.json
+-rw-rw-rw-   0        0        0     2950 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/WS888.json
+-rw-rw-rw-   0        0        0    49746 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_DWT_10.json
+-rw-rw-rw-   0        0        0    13088 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FDK.json
+-rw-rw-rw-   0        0        0    27628 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FEP_230V.json
+-rw-rw-rw-   0        0        0     5486 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FFK.json
+-rw-rw-rw-   0        0        0     2646 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FSA.json
+-rw-rw-rw-   0        0        0     5450 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FSS_UP3.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FST_UP4.json
+-rw-rw-rw-   0        0        0    87887 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FWT.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS-2.json
+-rw-rw-rw-   0        0        0    16021 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS.json
+-rw-rw-rw-   0        0        0    11274 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_HS_4.json
+-rw-rw-rw-   0        0        0     6478 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_WT_2.json
+-rw-rw-rw-   0        0        0     8876 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/paramset_descriptions/atent.json
+-rw-rw-rw-   0        0        0     1054 2023-04-26 19:37:30.000000 pydevccu-0.1.6/pydevccu/proxy.py
+drwxrwxrwx   0        0        0        0 2023-04-26 19:39:04.244578 pydevccu-0.1.6/pydevccu.egg-info/
+-rw-rw-rw-   0        0        0      615 2023-04-26 19:39:04.000000 pydevccu-0.1.6/pydevccu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    36255 2023-04-26 19:39:04.000000 pydevccu-0.1.6/pydevccu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 19:39:04.000000 pydevccu-0.1.6/pydevccu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 19:39:04.000000 pydevccu-0.1.6/pydevccu.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-04-26 19:39:04.000000 pydevccu-0.1.6/pydevccu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 19:39:08.065405 pydevccu-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2023-04-26 19:38:51.000000 pydevccu-0.1.6/setup.py
```

### Comparing `pydevccu-0.1.5/PKG-INFO` & `pydevccu-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pydevccu
-Version: 0.1.5
+Version: 0.1.6
 Summary: Virtual HomeMatic CCU XML-RPC backend
 Home-page: https://github.com/danielperna84/pydevccu
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
-Download-URL: https://github.com/danielperna84/pydevccu/tarball/0.1.5
+Download-URL: https://github.com/danielperna84/pydevccu/tarball/0.1.6
 Description: UNKNOWN
 Keywords: homematic,ccu,xml-rpc
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `pydevccu-0.1.5/README.md` & `pydevccu-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/ccu.py` & `pydevccu-0.1.6/pydevccu/ccu.py`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/const.py` & `pydevccu-0.1.6/pydevccu/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-"""
-Constants used in pydevccu
-"""
-
-VERSION = '0.1.5'
-
-IP_LOCALHOST_V4 = '127.0.0.1'
-IP_LOCALHOST_V6 = '::1'
-IP_ANY_V4 = '0.0.0.0'
-IP_ANY_V6 = '::'
-PORT_ANY = 0
-
-PORT_WIRED = 2000
-PORT_WIRED_TLS = 42000
-PORT_RF = 2001
-PORT_RF_TLS = 42001
-PORT_IP = 2010
-PORT_IP_TLS = 42010
-PORT_GROUPS = 9292
-PORT_GROUPS_TLS = 49292
-
-DEVICE_DESCRIPTIONS = "device_descriptions"
-PARAMSET_DESCRIPTIONS = "paramset_descriptions"
-PARAMSETS_DB = "paramsets_db.json"
-
-ATTR_ADDRESS = 'ADDRESS'
-ATTR_CHILDREN = 'CHILDREN'
-ATTR_NAME = 'NAME'
-ATTR_TYPE = 'TYPE'
-ATTR_PARENT_TYPE = 'PARENT_TYPE'
-ATTR_FLAGS = 'FLAGS'
-ATTR_ERROR = 'ERROR'
-ATTR_PARENT = 'PARENT'
-ATTR_PARENT_TYPE = 'PARENT_TYPE'
-
-PARAMSET_ATTR_MASTER = 'MASTER'
-PARAMSET_ATTR_VALUES = 'VALUES'
-PARAMSET_ATTR_LINK = 'LINK'
-PARAMSET_ATTR_MIN = 'MIN'
-PARAMSET_ATTR_MAX = 'MAX'
-PARAMSET_ATTR_OPERATIONS = 'OPERATIONS'
-PARAMSET_ATTR_DEFAULT = 'DEFAULT'
-PARAMSET_ATTR_VALUE_LIST = 'VALUE_LIST'
-PARAMSET_ATTR_SPECIAL = 'SPECIAL'
-PARAMSET_ATTR_UNIT = 'UNIT'
-PARAMSET_ATTR_CONTROL = 'CONTROL'
-
-PARAMSET_TYPE_FLOAT = 'FLOAT'
-PARAMSET_TYPE_INTEGER = 'INTEGER'
-PARAMSET_TYPE_BOOL = 'BOOL'
-PARAMSET_TYPE_ENUM = 'ENUM'
-PARAMSET_TYPE_STRING = 'STRING'
-PARAMSET_TYPE_ACTION = 'ACTION'
-
-PARAMSET_OPERATIONS_READ = 1
-PARAMSET_OPERATIONS_WRITE = 2
-PARAMSET_OPERATIONS_EVENT = 4
-
-PARAMSET_FLAG_INVISIBLE = 0
-PARAMSET_FLAG_VISIBLE = 1
-PARAMSET_FLAG_INTERNAL = 2
-PARAMSET_FLAG_TRANSFORM = 4
-PARAMSET_FLAG_SERVICE = 8
-PARAMSET_FLAG_STICKY = 10
+"""
+Constants used in pydevccu
+"""
+
+VERSION = '0.1.6'
+
+IP_LOCALHOST_V4 = '127.0.0.1'
+IP_LOCALHOST_V6 = '::1'
+IP_ANY_V4 = '0.0.0.0'
+IP_ANY_V6 = '::'
+PORT_ANY = 0
+
+PORT_WIRED = 2000
+PORT_WIRED_TLS = 42000
+PORT_RF = 2001
+PORT_RF_TLS = 42001
+PORT_IP = 2010
+PORT_IP_TLS = 42010
+PORT_GROUPS = 9292
+PORT_GROUPS_TLS = 49292
+
+DEVICE_DESCRIPTIONS = "device_descriptions"
+PARAMSET_DESCRIPTIONS = "paramset_descriptions"
+PARAMSETS_DB = "paramsets_db.json"
+
+ATTR_ADDRESS = 'ADDRESS'
+ATTR_CHILDREN = 'CHILDREN'
+ATTR_NAME = 'NAME'
+ATTR_TYPE = 'TYPE'
+ATTR_PARENT_TYPE = 'PARENT_TYPE'
+ATTR_FLAGS = 'FLAGS'
+ATTR_ERROR = 'ERROR'
+ATTR_PARENT = 'PARENT'
+ATTR_PARENT_TYPE = 'PARENT_TYPE'
+
+PARAMSET_ATTR_MASTER = 'MASTER'
+PARAMSET_ATTR_VALUES = 'VALUES'
+PARAMSET_ATTR_LINK = 'LINK'
+PARAMSET_ATTR_MIN = 'MIN'
+PARAMSET_ATTR_MAX = 'MAX'
+PARAMSET_ATTR_OPERATIONS = 'OPERATIONS'
+PARAMSET_ATTR_DEFAULT = 'DEFAULT'
+PARAMSET_ATTR_VALUE_LIST = 'VALUE_LIST'
+PARAMSET_ATTR_SPECIAL = 'SPECIAL'
+PARAMSET_ATTR_UNIT = 'UNIT'
+PARAMSET_ATTR_CONTROL = 'CONTROL'
+
+PARAMSET_TYPE_FLOAT = 'FLOAT'
+PARAMSET_TYPE_INTEGER = 'INTEGER'
+PARAMSET_TYPE_BOOL = 'BOOL'
+PARAMSET_TYPE_ENUM = 'ENUM'
+PARAMSET_TYPE_STRING = 'STRING'
+PARAMSET_TYPE_ACTION = 'ACTION'
+
+PARAMSET_OPERATIONS_READ = 1
+PARAMSET_OPERATIONS_WRITE = 2
+PARAMSET_OPERATIONS_EVENT = 4
+
+PARAMSET_FLAG_INVISIBLE = 0
+PARAMSET_FLAG_VISIBLE = 1
+PARAMSET_FLAG_INTERNAL = 2
+PARAMSET_FLAG_TRANSFORM = 4
+PARAMSET_FLAG_SERVICE = 8
+PARAMSET_FLAG_STICKY = 10
```

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_130.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_130.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_131.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_131.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_132.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_132.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_133.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_133.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_134.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_134.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_135.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_135.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_144.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_144.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_145.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_145.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_146.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_146.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_147.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_147.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_155.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_155.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_157.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_157.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_158.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_158.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_160.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_160.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_162.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_162.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/263_167.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/263_167.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ALPHA-IP-RBG.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ALPHA-IP-RBG.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ASH550.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ASH550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ASH550I.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ASH550I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/BRC-H.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/BRC-H.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/CMM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/CMM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ELV-SH-BS2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ELV-SH-BS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Bl1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Bl1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Sw1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Sw1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-LC-Sw2PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-LC-Sw2PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sen-PRESS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sen-PRESS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sen-TEMP-DS18B20.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sen-TEMP-DS18B20.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor-TH-SHT75.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor-TH-SHT75.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor-THPD-BME280.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor-THPD-BME280.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-UNI-Sensor1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-UNI-Sensor1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HB-WDS40-THP-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HB-WDS40-THP-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HBW-LC-RGBWW-IN6-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HBW-LC-RGBWW-IN6-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-RT-DN-BoM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-RT-DN-BoM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-RT-DN.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-RT-DN.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-SCD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-SCD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-TC.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-TC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-VD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-VD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-CC-VG-1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-CC-VG-1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-DW-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-DW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-EP-WM55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-EP-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-TD-T.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-TD-T.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Dis-WM55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Dis-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R5.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl-DN-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSw1-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSw1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-PMSwX.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-PMSwX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ES-TX-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ES-TX-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-AO-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-AO-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-PB-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Bl1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Bl1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-BlX.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-BlX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-DDC1-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-DDC1-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-DW-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-DW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-CV-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-CV.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1L-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1L-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1PWM-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-CV-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-CV.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM-LF.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM-LF.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1T-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1T-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim1TPBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-CV.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2L-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2L-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2T-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2T-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Dim2T-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Dim2T-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Ja1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Ja1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-JaX.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-JaX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-RGBW-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-RGBW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Ba-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Ba-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-PB-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R5.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-CT-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R5.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-DN-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl-OM54.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl-OM54.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM-ATmega168.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM-ATmega168.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-DR-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-PB-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw2PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw2PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-Ba-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-Ba-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-DR-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-PCB-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-PCB-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM-ATmega168.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM-ATmega168.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-WM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-WM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-Sw4-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-Sw4-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-LC-SwX.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-LC-SwX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-MD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-MD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-EM-8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-EM-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-EM-8Bit.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-EM-8Bit.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-MOD-Re-8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-MOD-Re-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CF-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CF-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CFM-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CFM-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CFM-TW.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CFM-TW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-CM-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-CM-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-LED16.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-LED16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-OU-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-OU-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM55-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM55-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-2-WM55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-2-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4Dis-WM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4Dis-WM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-4Dis-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-4Dis-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PB-6-WM55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PB-6-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PBI-4-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PBI-4-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-PBI-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-PBI-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12-SW.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12-SW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-12.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-12.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19-SW.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19-SW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-19.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-19.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-2-PBU-FM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-2-PBU-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-2-PBU-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-2-PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-3-D.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-3-D.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Dis-H-x-EU.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Dis-H-x-EU.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key3-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key3-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key4-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Key4-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Key4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-P1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-P1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-SB-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-SB-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec3-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec3-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec4-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-Sec4-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-Sec4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RC-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RC-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-RCV-50.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-ReSC-Win-PCB-xx.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-ReSC-Win-PCB-xx.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-SCI-3-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-SCI-3-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-Generic.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key-S.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key-S.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Key.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Key.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-MDIR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-MDIR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-RHS-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-RHS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-RHS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-RHS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SC-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SC-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SC.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SCo.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SCo.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-2-Generic.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-2-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD-Generic.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-SFA-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-SFA-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Sir-WM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Sir-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-TiS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-TiS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-WDS-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-WDS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-WDS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-WDS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Win-Generic.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Win-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-Win.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-Win.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sec-xx.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sec-xx.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-DB-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-DB-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-EP.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-EP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-LI-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-LI-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O-3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-MDIR-WM55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-MDIR-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-RD-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-RD-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-Wa-Od.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-Wa-Od.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sen-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sen-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-SwI-3-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-SwI-3-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-SwI-X.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-SwI-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-Sys-sRP-Pl.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-Sys-sRP-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-TC-IT-WM-W-EU.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-TC-IT-WM-W-EU.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDC7000.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDC7000.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS10-TH-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS10-TH-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS100-C6-O-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS100-C6-O-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS100-C6-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS100-C6-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS20-TH-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS20-TH-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-OT2-SM-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-OT2-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-OT2-SM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-OT2-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS30-T-O.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS30-T-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS40-TH-I-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS40-TH-I-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HM-WDS40-TH-I.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HM-WDS40-TH-I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-PS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-PS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-PSM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-PSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-SWDO.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-SWDO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMIP-WRC2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMIP-WRC2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-Sw14-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-Sw14-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-12-Sw7-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-12-Sw7-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-4-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-4-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-IO-SR-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-IO-SR-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Bl1-DR-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Bl1-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Bl1-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Bl1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Dim1L-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Dim1L-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-LC-Sw2-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-LC-Sw2-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-RCV-50.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-Sen-SC-12-DR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-Sen-SC-12-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HMW-Sen-SC-12-FM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HMW-Sen-SC-12-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HSS-DX.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HSS-DX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-ASIR-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-ASIR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-ASIR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-ASIR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BDT.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BDT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BRC2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BRC2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BROLL.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BROLL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BSL.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BSL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BSM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-BWTH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-BWTH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-CCU3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-CCU3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DBB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DBB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DLD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DLD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DLS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DLS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRDI3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRDI3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRSI1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRSI1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DRSI4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DRSI4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-DSD-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-DSD-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FAL230-C10.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FAL230-C10.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FBL.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FBL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FCI1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FCI1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FDT.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FDT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FROLL.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FROLL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FSI16.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FSI16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-FSM16.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-FSM16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HAP.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HAP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HDM1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HDM1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HDM2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HDM2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-HEATING.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-HEATING.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-KRC4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-KRC4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-KRCA.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-KRCA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MIO16-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MIO16-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-HO.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-HO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-OC8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-OC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-RC8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-RC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MOD-TM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MOD-TM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-MP3P.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-MP3P.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS-BAT.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS-BAT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PCBS2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PCBS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-PMFS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-PMFS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RC8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RCB1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RCB1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RCV-50.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-RFUSB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-RFUSB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SAM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SAM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SCI.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SCI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SCTH230.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SCTH230.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SFD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SFD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SLO.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SLO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMI.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMI55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMI55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO-A.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO-A.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SMO.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SMO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SPDR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SPDR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SPI.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SPI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SRD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SRD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SRH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SRH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STE2-PCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STE2-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHO-A.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHO-A.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STHO.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STHO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-STV.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-STV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDM-B2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDM-B2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWDO-I.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWDO-I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-PL.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-PL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWO-PR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWO-PR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-SWSD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-SWSD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-USBSM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-USBSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WGC.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WGC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WHS2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WHS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRC6.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRC6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRCD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRCD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WRCR.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WRCR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WTH-1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WTH-1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-WTH-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-WTH-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-2 I9F.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-2 I9F.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-B.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-B1.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-B1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-C-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-C-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIP-eTRV-E.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIP-eTRV-E.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRAP.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRAP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRBL4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRBL4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRD3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRD3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRI32.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRI32.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-DRS8.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-DRS8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FAL230-C6.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FAL230-C6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FALMOT-C12.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FALMOT-C12.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-FIO6.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-FIO6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-SMI55.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-SMI55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-SPI.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-SPI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-STH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-STH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-STHD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-STHD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-WRC6.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-WRC6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/HmIPW-WTH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/HmIPW-WTH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/IS-WDS-TH-OD-S-R3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/IS-WDS-TH-OD-S-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/KS550.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/KS550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/KS550LC.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/KS550LC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/KS550Tech.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/KS550Tech.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/KS888.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/KS888.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/OLIGO.smart.iq.HM.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/OLIGO.smart.iq.HM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/RC-H.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/RC-H.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/RPI-RF-MOD.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/RPI-RF-MOD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/S550IA.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/S550IA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ST6-SH.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ST6-SH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WDF_solar.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WDF_solar.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WS550.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WS550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WS550LCB.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WS550LCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WS550LCW.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WS550LCW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WS550Tech.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WS550Tech.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/WS888.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/WS888.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_DWT_10.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_DWT_10.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FDK.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FDK.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FEP_230V.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FEP_230V.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FFK.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FFK.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FSA.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FSA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FSS_UP3.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FSS_UP3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FST_UP4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FST_UP4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FWT.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FWT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FZS-2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FZS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_FZS.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_FZS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_HS_4.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_HS_4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/ZEL_STG_RM_WT_2.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/ZEL_STG_RM_WT_2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_descriptions/atent.json` & `pydevccu-0.1.6/pydevccu/device_descriptions/atent.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/device_logic/HM_Sec_SC_2.py` & `pydevccu-0.1.6/pydevccu/device_logic/HM_Sec_SC_2.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-"""
-Logic module for HM-Sec-SC-2 (VCU0000240).
-Switch between open / closed, toggle LOWBAT every 5 events.
-"""
-
-import sys
-import time
-import random
-import logging
-
-LOG = logging.getLogger(__name__)
-if sys.stdout.isatty():
-    logging.basicConfig(level=logging.DEBUG)
-
-class HM_Sec_SC_2(object):
-    def __init__(self, rpcfunctions, startupdelay=5, interval=60):
-        self.rpcfunctions = rpcfunctions
-        self.name = "HM-Sec-SC-2"
-        self.address = "VCU0000240:1"
-        self.active = False
-        self.firstrun = True
-        self.startupdelay = startupdelay
-        self.interval = interval
-        self.lowbat = False
-        self.counter = 1
-
-    def work(self):
-        if self.firstrun:
-            time.sleep(random.randint(0, self.startupdelay))
-        self.firstrun = False
-        while self.active:
-            if self.rpcfunctions.active:
-                current_state = self.rpcfunctions.getValue(self.address, "STATE")
-                if self.counter % 5 == 0:
-                    self.lowbat = not self.lowbat
-                    self.rpcfunctions._fireEvent(self.name, self.address, "LOWBAT", self.lowbat)
-                self.rpcfunctions.setValue(self.address, "STATE", not current_state, force=True)
-                self.counter += 1
-            time.sleep(self.interval)
+"""
+Logic module for HM-Sec-SC-2 (VCU0000240).
+Switch between open / closed, toggle LOWBAT every 5 events.
+"""
+
+import sys
+import time
+import random
+import logging
+
+LOG = logging.getLogger(__name__)
+if sys.stdout.isatty():
+    logging.basicConfig(level=logging.DEBUG)
+
+class HM_Sec_SC_2(object):
+    def __init__(self, rpcfunctions, startupdelay=5, interval=60):
+        self.rpcfunctions = rpcfunctions
+        self.name = "HM-Sec-SC-2"
+        self.address = "VCU0000240:1"
+        self.active = False
+        self.firstrun = True
+        self.startupdelay = startupdelay
+        self.interval = interval
+        self.lowbat = False
+        self.counter = 1
+
+    def work(self):
+        if self.firstrun:
+            time.sleep(random.randint(0, self.startupdelay))
+        self.firstrun = False
+        while self.active:
+            if self.rpcfunctions.active:
+                current_state = self.rpcfunctions.getValue(self.address, "STATE")
+                if self.counter % 5 == 0:
+                    self.lowbat = not self.lowbat
+                    self.rpcfunctions._fireEvent(self.name, self.address, "LOWBAT", self.lowbat)
+                self.rpcfunctions.setValue(self.address, "STATE", not current_state, force=True)
+                self.counter += 1
+            time.sleep(self.interval)
```

### Comparing `pydevccu-0.1.5/pydevccu/device_logic/HM_Sen_MDIR_WM55.py` & `pydevccu-0.1.6/pydevccu/device_logic/HM_Sen_MDIR_WM55.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-"""
-Logic module for HM-Sen-MDIR-WM55 (VCU0000274).
-Switch between motion, toggle LOWBAT every 5 events,
-random brightness from 60 to 90, press on channel 1.
-"""
-
-import sys
-import time
-import random
-import logging
-
-LOG = logging.getLogger(__name__)
-if sys.stdout.isatty():
-    logging.basicConfig(level=logging.DEBUG)
-
-class HM_Sen_MDIR_WM55(object):
-    def __init__(self, rpcfunctions, startupdelay=5, interval=60):
-        self.rpcfunctions = rpcfunctions
-        self.name = "HM-Sen-MDIR-WM55"
-        self.address = "VCU0000274"
-        self.active = False
-        self.firstrun = True
-        self.startupdelay = startupdelay
-        self.interval = interval
-        self.lowbat = False
-        self.counter = 1
-
-    def work(self):
-        if self.firstrun:
-            time.sleep(random.randint(0, self.startupdelay))
-        self.firstrun = False
-        while self.active:
-            if self.rpcfunctions.active:
-                current_state = self.rpcfunctions.getValue("%s:3" % self.address, "MOTION")
-                if self.counter % 5 == 0:
-                    self.lowbat = not self.lowbat
-                    self.rpcfunctions._fireEvent(self.name, "%s:0" % self.address, "LOWBAT", self.lowbat)
-                self.rpcfunctions.setValue("%s:3" % self.address, "MOTION", not current_state, force=True)
-                self.rpcfunctions.setValue("%s:3" % self.address, "BRIGHTNESS", random.randint(60, 90), force=True)
-                self.rpcfunctions._fireEvent(self.name, "%s:1" % self.address, "PRESS_SHORT", True)
-                self.counter += 1
-            time.sleep(self.interval)
+"""
+Logic module for HM-Sen-MDIR-WM55 (VCU0000274).
+Switch between motion, toggle LOWBAT every 5 events,
+random brightness from 60 to 90, press on channel 1.
+"""
+
+import sys
+import time
+import random
+import logging
+
+LOG = logging.getLogger(__name__)
+if sys.stdout.isatty():
+    logging.basicConfig(level=logging.DEBUG)
+
+class HM_Sen_MDIR_WM55(object):
+    def __init__(self, rpcfunctions, startupdelay=5, interval=60):
+        self.rpcfunctions = rpcfunctions
+        self.name = "HM-Sen-MDIR-WM55"
+        self.address = "VCU0000274"
+        self.active = False
+        self.firstrun = True
+        self.startupdelay = startupdelay
+        self.interval = interval
+        self.lowbat = False
+        self.counter = 1
+
+    def work(self):
+        if self.firstrun:
+            time.sleep(random.randint(0, self.startupdelay))
+        self.firstrun = False
+        while self.active:
+            if self.rpcfunctions.active:
+                current_state = self.rpcfunctions.getValue("%s:3" % self.address, "MOTION")
+                if self.counter % 5 == 0:
+                    self.lowbat = not self.lowbat
+                    self.rpcfunctions._fireEvent(self.name, "%s:0" % self.address, "LOWBAT", self.lowbat)
+                self.rpcfunctions.setValue("%s:3" % self.address, "MOTION", not current_state, force=True)
+                self.rpcfunctions.setValue("%s:3" % self.address, "BRIGHTNESS", random.randint(60, 90), force=True)
+                self.rpcfunctions._fireEvent(self.name, "%s:1" % self.address, "PRESS_SHORT", True)
+                self.counter += 1
+            time.sleep(self.interval)
```

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_130.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_130.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_131.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_131.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_132.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_132.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_133.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_133.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_134.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_134.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_135.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_135.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_144.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_144.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_145.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_145.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_146.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_146.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_147.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_147.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_155.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_155.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_157.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_157.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_158.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_158.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_160.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_160.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_162.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_162.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/263_167.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/263_167.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ALPHA-IP-RBG.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ALPHA-IP-RBG.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ASH550.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ASH550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ASH550I.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ASH550I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/BRC-H.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/BRC-H.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/CMM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/CMM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ELV-SH-BS2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ELV-SH-BS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Bl1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Bl1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Sw1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Sw1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-LC-Sw2PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-LC-Sw2PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sen-PRESS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sen-PRESS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sen-TEMP-DS18B20.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sen-TEMP-DS18B20.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor-TH-SHT75.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor-TH-SHT75.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor-THPD-BME280.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor-THPD-BME280.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-UNI-Sensor1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-UNI-Sensor1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HB-WDS40-THP-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HB-WDS40-THP-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HBW-LC-RGBWW-IN6-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HBW-LC-RGBWW-IN6-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-RT-DN-BoM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-RT-DN-BoM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-RT-DN.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-RT-DN.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-SCD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-SCD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-TC.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-TC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-VD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-VD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-CC-VG-1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-CC-VG-1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-DW-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-DW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-EP-WM55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-EP-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-TD-T.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-TD-T.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Dis-WM55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Dis-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R5.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl-DN-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSw1-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSw1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-PMSwX.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-PMSwX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ES-TX-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ES-TX-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-AO-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-AO-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-PB-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Bl1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Bl1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-BlX.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-BlX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-DDC1-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-DDC1-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-DW-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-DW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1L-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1PWM-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-LF.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM-LF.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1T-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim1TPBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-CV.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-CV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2L-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Dim2T-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Ja1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Ja1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-JaX.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-JaX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-RGBW-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-RGBW-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Ba-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Ba-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-PB-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R5.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-CT-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R5.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-DN-R5.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-OM54.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl-OM54.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-ATmega168.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM-ATmega168.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw1PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw1PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-DR-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-PB-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-PB-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw2PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw2PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-Ba-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-Ba-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-DR-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-ATmega168.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM-ATmega168.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-WM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-WM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-Sw4-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-Sw4-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-LC-SwX.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-LC-SwX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-EM-8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-EM-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-EM-8Bit.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-EM-8Bit.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-MOD-Re-8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-MOD-Re-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CF-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CF-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CFM-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CFM-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CFM-TW.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CFM-TW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-CM-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-CM-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-LED16.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-LED16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-OU-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-OU-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM55-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM55-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-2-WM55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-2-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4Dis-WM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4Dis-WM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-4Dis-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-4Dis-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PB-6-WM55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PB-6-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PBI-4-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PBI-4-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-PBI-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-PBI-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12-SW.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12-SW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-12.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-12.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19-SW.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19-SW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-19.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-19.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-2-PBU-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-3-D.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-3-D.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Dis-H-x-EU.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Dis-H-x-EU.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key3-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key3-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key4-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Key4-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Key4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-P1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-P1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-SB-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-SB-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec3-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec3-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec4-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec4-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-Sec4-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-Sec4-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RC-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RC-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-RCV-50.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-ReSC-Win-PCB-xx.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-ReSC-Win-PCB-xx.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SCI-3-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SCI-3-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-Generic.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key-S.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key-S.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Key.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Key.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-MDIR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-MDIR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-RHS-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-RHS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-RHS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-RHS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SC-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SC-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SC.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SCo.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SCo.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-2-Generic.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-2-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD-Generic.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-SFA-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-SFA-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Sir-WM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Sir-WM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-TiS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-TiS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-WDS-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-WDS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-WDS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-WDS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Win-Generic.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Win-Generic.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-Win.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-Win.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sec-xx.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sec-xx.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-DB-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-DB-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-EP.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-EP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-LI-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-LI-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O-3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-MDIR-WM55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-MDIR-WM55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-RD-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-RD-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-Wa-Od.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-Wa-Od.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sen-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sen-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SwI-3-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SwI-3-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-SwI-X.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-SwI-X.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-Sys-sRP-Pl.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-Sys-sRP-Pl.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-TC-IT-WM-W-EU.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-TC-IT-WM-W-EU.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDC7000.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDC7000.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS10-TH-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS10-TH-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS100-C6-O-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS100-C6-O-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS100-C6-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS100-C6-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS20-TH-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS20-TH-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-OT2-SM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS30-T-O.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS30-T-O.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS40-TH-I-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS40-TH-I-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HM-WDS40-TH-I.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HM-WDS40-TH-I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-PS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-PS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-PSM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-PSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-SWDO.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-SWDO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMIP-WRC2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMIP-WRC2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-Sw14-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-Sw14-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-12-Sw7-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-12-Sw7-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-4-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-4-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-IO-SR-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-IO-SR-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Bl1-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Dim1L-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Dim1L-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-LC-Sw2-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-LC-Sw2-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-RCV-50.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-Sen-SC-12-DR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-Sen-SC-12-DR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HMW-Sen-SC-12-FM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HMW-Sen-SC-12-FM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HSS-DX.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HSS-DX.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-ASIR-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-ASIR-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-ASIR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-ASIR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BDT.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BDT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BRC2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BRC2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BROLL.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BROLL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BSL.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BSL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BSM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-BWTH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-BWTH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-CCU3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-CCU3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DBB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DBB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DLD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DLD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DLS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DLS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRDI3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRDI3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRSI1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRSI1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DRSI4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DRSI4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-DSD-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-DSD-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FAL230-C10.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FAL230-C10.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FBL.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FBL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FCI1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FCI1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FDT.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FDT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FROLL.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FROLL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FSI16.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FSI16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-FSM16.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-FSM16.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HAP.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HAP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HDM1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HDM1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HDM2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HDM2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-HEATING.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-HEATING.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-KRC4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-KRC4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-KRCA.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-KRCA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MIO16-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MIO16-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-HO.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-HO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-OC8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-OC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-RC8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-RC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MOD-TM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MOD-TM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-MP3P.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-MP3P.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS-BAT.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS-BAT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PCBS2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PCBS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-PMFS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-PMFS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RC8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RC8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RCB1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RCB1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RCV-50.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RCV-50.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-RFUSB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-RFUSB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SAM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SAM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SCI.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SCI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SCTH230.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SCTH230.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SFD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SFD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SLO.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SLO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMI.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMI55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMI55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO-A.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO-A.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SMO.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SMO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SPDR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SPDR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SPI.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SPI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SRD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SRD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SRH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SRH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STE2-PCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STE2-PCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHO-A.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHO-A.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STHO.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STHO.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-STV.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-STV.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDM-B2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDM-B2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWDO-I.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWDO-I.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-PL.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-PL.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWO-PR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWO-PR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-SWSD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-SWSD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-USBSM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-USBSM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WGC.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WGC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WHS2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WHS2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRC6.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRC6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRCD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRCD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WRCR.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WRCR.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WTH-1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WTH-1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-WTH-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-WTH-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-2 I9F.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-2 I9F.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-B.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-B.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-B1.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-B1.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-C-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-C-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIP-eTRV-E.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIP-eTRV-E.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRAP.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRAP.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRBL4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRBL4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRD3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRD3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRI32.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRI32.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-DRS8.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-DRS8.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FAL230-C6.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FAL230-C6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FALMOT-C12.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FALMOT-C12.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-FIO6.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-FIO6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-SMI55.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-SMI55.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-SPI.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-SPI.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-STH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-STH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-STHD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-STHD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-WRC6.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-WRC6.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/HmIPW-WTH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/HmIPW-WTH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/IS-WDS-TH-OD-S-R3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/IS-WDS-TH-OD-S-R3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550LC.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550LC.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/KS550Tech.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/KS550Tech.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/KS888.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/KS888.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/OLIGO.smart.iq.HM.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/OLIGO.smart.iq.HM.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/RC-H.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/RC-H.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/RPI-RF-MOD.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/RPI-RF-MOD.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/S550IA.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/S550IA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ST6-SH.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ST6-SH.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WDF_solar.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WDF_solar.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550LCB.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550LCB.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550LCW.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550LCW.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WS550Tech.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WS550Tech.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/WS888.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/WS888.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_DWT_10.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_DWT_10.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FDK.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FDK.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FEP_230V.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FEP_230V.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FFK.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FFK.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FSA.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FSA.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FSS_UP3.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FSS_UP3.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FST_UP4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FST_UP4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FWT.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FWT.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS-2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS-2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_FZS.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_HS_4.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_HS_4.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/ZEL_STG_RM_WT_2.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/ZEL_STG_RM_WT_2.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu/paramset_descriptions/atent.json` & `pydevccu-0.1.6/pydevccu/paramset_descriptions/atent.json`

 * *Files identical despite different names*

### Comparing `pydevccu-0.1.5/pydevccu.egg-info/PKG-INFO` & `pydevccu-0.1.6/pydevccu.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: pydevccu
-Version: 0.1.5
+Version: 0.1.6
 Summary: Virtual HomeMatic CCU XML-RPC backend
 Home-page: https://github.com/danielperna84/pydevccu
 Author: Daniel Perna
 Author-email: danielperna84@gmail.com
 License: MIT License
-Download-URL: https://github.com/danielperna84/pydevccu/tarball/0.1.5
+Download-URL: https://github.com/danielperna84/pydevccu/tarball/0.1.6
 Description: UNKNOWN
 Keywords: homematic,ccu,xml-rpc
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `pydevccu-0.1.5/pydevccu.egg-info/SOURCES.txt` & `pydevccu-0.1.6/pydevccu.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
 pydevccu/device_descriptions/HmIP-PCBS.json
 pydevccu/device_descriptions/HmIP-PCBS2.json
 pydevccu/device_descriptions/HmIP-PMFS.json
 pydevccu/device_descriptions/HmIP-RC8.json
 pydevccu/device_descriptions/HmIP-RCB1.json
 pydevccu/device_descriptions/HmIP-RCV-50.json
 pydevccu/device_descriptions/HmIP-RFUSB.json
+pydevccu/device_descriptions/HmIP-RGBW.json
 pydevccu/device_descriptions/HmIP-SAM.json
 pydevccu/device_descriptions/HmIP-SCI.json
 pydevccu/device_descriptions/HmIP-SCTH230.json
 pydevccu/device_descriptions/HmIP-SFD.json
 pydevccu/device_descriptions/HmIP-SLO.json
 pydevccu/device_descriptions/HmIP-SMI.json
 pydevccu/device_descriptions/HmIP-SMI55.json
@@ -673,14 +674,15 @@
 pydevccu/paramset_descriptions/HmIP-PCBS.json
 pydevccu/paramset_descriptions/HmIP-PCBS2.json
 pydevccu/paramset_descriptions/HmIP-PMFS.json
 pydevccu/paramset_descriptions/HmIP-RC8.json
 pydevccu/paramset_descriptions/HmIP-RCB1.json
 pydevccu/paramset_descriptions/HmIP-RCV-50.json
 pydevccu/paramset_descriptions/HmIP-RFUSB.json
+pydevccu/paramset_descriptions/HmIP-RGBW.json
 pydevccu/paramset_descriptions/HmIP-SAM.json
 pydevccu/paramset_descriptions/HmIP-SCI.json
 pydevccu/paramset_descriptions/HmIP-SCTH230.json
 pydevccu/paramset_descriptions/HmIP-SFD.json
 pydevccu/paramset_descriptions/HmIP-SLO.json
 pydevccu/paramset_descriptions/HmIP-SMI.json
 pydevccu/paramset_descriptions/HmIP-SMI55.json
```

