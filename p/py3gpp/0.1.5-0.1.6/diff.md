# Comparing `tmp/py3gpp-0.1.5.tar.gz` & `tmp/py3gpp-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3gpp-0.1.5.tar", last modified: Tue Feb 28 18:32:59 2023, max compression
+gzip compressed data, was "py3gpp-0.1.6.tar", last modified: Wed Apr 26 07:31:26 2023, max compression
```

## Comparing `py3gpp-0.1.5.tar` & `py3gpp-0.1.6.tar`

### file list

```diff
@@ -1,40 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:32:59.214800 py3gpp-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-28 18:32:44.000000 py3gpp-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-02-28 18:32:59.214800 py3gpp-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-28 18:32:44.000000 py3gpp-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:32:59.210801 py3gpp-0.1.5/py3gpp/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrBCHDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrCRCDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrCRCEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrCarrierConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrChannelEstimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrEqualizeMMSE.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrExtractResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrOFDMDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrOFDMInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrOFDMModulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPBCHDMRS.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPBCHDMRSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPBCHIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPBCHPRBS.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrPolarDecode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrRateRecoverPolar.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrResourceGrid.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrSSS.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrSSSIndices.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrSetResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrSymbolDemodulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-02-28 18:32:44.000000 py3gpp-0.1.5/py3gpp/nrTimingEstimate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 18:32:59.214800 py3gpp-0.1.5/py3gpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-02-28 18:32:59.000000 py3gpp-0.1.5/py3gpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-02-28 18:32:59.000000 py3gpp-0.1.5/py3gpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 18:32:59.000000 py3gpp-0.1.5/py3gpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-28 18:32:59.000000 py3gpp-0.1.5/py3gpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-28 18:32:59.000000 py3gpp-0.1.5/py3gpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-02-28 18:32:44.000000 py3gpp-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 18:32:59.214800 py3gpp-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-28 18:32:44.000000 py3gpp-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.019804 py3gpp-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-26 07:31:09.000000 py3gpp-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 07:31:26.019804 py3gpp-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 07:31:09.000000 py3gpp-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/CommonConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/DMRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/PDSCHConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/PDSCHPTRSConfigBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrCarrierConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrNumerologyConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHDMRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/configs/nrPDSCHPTRSConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrChannelEstimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrEqualizeMMSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrExtractResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrOFDMModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCH.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPBCHPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHPTRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPRBS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrPolarDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrRateRecoverPolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrResourceGrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSSS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSSSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSetResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSymbolDemodulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrSymbolModulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-26 07:31:09.000000 py3gpp-0.1.6/py3gpp/nrTimingEstimate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.015803 py3gpp-0.1.6/py3gpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 07:31:26.000000 py3gpp-0.1.6/py3gpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 07:31:09.000000 py3gpp-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:31:26.019804 py3gpp-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 07:31:09.000000 py3gpp-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:31:26.019804 py3gpp-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18861 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrBCHDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrCRCDecode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrCRCEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHDMRS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHDMRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrPDSCHPTRSIndices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-26 07:31:09.000000 py3gpp-0.1.6/tests/test_nrRateRecoverPolar.py
```

### Comparing `py3gpp-0.1.5/LICENSE` & `py3gpp-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/PKG-INFO` & `py3gpp-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.5/README.md` & `py3gpp-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/helper.py` & `py3gpp-0.1.6/py3gpp/helper.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/nrBCHDecode.py` & `py3gpp-0.1.6/tests/test_nrBCHDecode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,9 @@
 import numpy as np
-from py3gpp.nrPolarDecode import nrPolarDecode
-from py3gpp.nrRateRecoverPolar import nrRateRecoverPolar
-from py3gpp.nrCRCDecode import nrCRCDecode
-from py3gpp.nrPBCHPRBS import nrPBCHPRBS
-
-
-def nrBCHDecode(softbits, L, lssb=None, ncellid=None):
-    K = 32
-    E = 864
-    L = 8
-    N = 512
-    matched = nrRateRecoverPolar(softbits, K, N, False, False)
-
-    decoded = nrPolarDecode(matched, K, E, L)
-    scrblk, crc_result = nrCRCDecode(decoded, "24C")
-
-    if (lssb is None) or (ncellid is None):
-        return scrblk, crc_result
-
-    # descrambling according to TS38.212 7.1.2
-    # fmt: off
-    G = [16, 23, 18, 17, 8, 30, 10, 6, 24, 7, 0, 5, 3, 2, 1, 4, 9, 11, 12, 13, 14, 15, 19, 20, 21, 22, 25, 26, 27, 28,
-         29, 31]
-    # fmt: on
-    SFN_PAYLOAD_BEGIN = 1
-    SFN_PAYLOAD_LENGTH = 6
-    SFN_2ND_LSB = SFN_PAYLOAD_LENGTH + 2
-    SFN_3RD_LSB = SFN_PAYLOAD_LENGTH + 1
-    v = 2 * scrblk[G[SFN_3RD_LSB]] + scrblk[G[SFN_2ND_LSB]]
-
-    L_max = 8  # TODO: fix this
-    A = 32
-    if L_max in (4, 8):
-        M = A - 3
-    else:
-        M = A - 6
-    n = v * M
-    tmp_seq = nrPBCHPRBS(ncellid, 0, len(scrblk) * 100)
-    scrambling_seq = tmp_seq[n:][:A]
-    scrambling_seq_final = np.zeros(A, "int")
-    j = 0
-    for i in range(A):
-        is_ssb_idx = (i in (G[11], G[12], G[13])) and L_max == 64
-        if is_ssb_idx or i == G[10] or i == G[SFN_2ND_LSB] or i == G[SFN_3RD_LSB]:
-            scrambling_seq_final[i] = 0
-        else:
-            scrambling_seq_final[i] = scrambling_seq[j]
-            j += 1
-    a = np.bitwise_xor(scrambling_seq_final, scrblk)
-
-    # deinterleaving according to TS38.212 7.1.1
-    j_sfn = 0
-    j_other = 14
-    payload = np.empty(24, "int")
-    for i in range(24):
-        if (i >= SFN_PAYLOAD_BEGIN) and (i < (SFN_PAYLOAD_BEGIN + SFN_PAYLOAD_LENGTH)):
-            payload[i] = a[G[j_sfn]]
-            j_sfn += 1
-        else:
-            payload[i] = a[G[j_other]]
-            j_other += 1
-    lsbotfsfn = np.array([a[G[j_sfn]], a[G[j_sfn + 1]], a[G[j_sfn + 2]], a[G[j_sfn + 3]]])
-    hrf = a[G[10]]
-    msbidxoffset = 0  # TODO calculate this
-    return scrblk, crc_result, payload, lsbotfsfn, hrf, msbidxoffset
-
+from py3gpp.nrBCHDecode import nrBCHDecode
 
 def test_nrBCHDecode():
     # 3627MHz, 30720 KSPS
     # fmt: off
     softbits = np.array([98.0994, 100.2936, -100.1615, -111.2452, -101.7249, -101.5950, 78.5901, -77.7265, -76.4686, -81.3223, -115.8069, 89.6047, 85.9367, 104.1048, -98.2053, -106.7203, 83.1207, 88.2861, 83.8204, -109.2175, -124.4919, 94.6728, 91.5959, -89.5352, -101.8143, -123.6915, -103.1579, -108.0879, 100.9417, -95.5231, 122.5312, 99.6845, -78.9441, 115.9421, 65.5815, 90.9532, -88.9573, -85.7132, -83.5216, -78.7969, -54.1358, 75.8672, 84.9239, -89.5731, -92.8101, -76.0732, 72.9594, -74.3997, -68.2989, 93.4047, 95.1260, 79.8283, 80.2065, -89.3344, 68.9841, -77.7767, 95.8681, -79.4709, 62.2583, -63.4266, -91.1614, 81.0331, -83.1753, -95.7477, 93.8353, -80.0016, 83.2706, -104.8245, 75.5381, -89.3799, 86.4390, 84.6055, 43.8157, -100.4702, -79.0332, -89.0215, 109.9606, -99.6110, 111.9779, -101.8772, 79.3811, -78.2227, 109.3239, -70.7376, -90.1096, -93.8385, -83.5296, 79.8664, -107.2777, 86.7808, -83.8104, -89.5405, 83.9844, 88.8928, -114.4005, -81.6010, 68.2572, 100.1189, -94.9682, -106.6306, 94.3960, -75.7935, -80.0656, -80.4422, 80.0088, 78.5461, -101.9442, 101.2641, 79.4489, -82.3328, 85.9272, -93.2934, 96.1777, 88.5216, 84.3977, -82.6021, 84.0117, 95.0405, -86.1691, -74.1916, 108.7456, 86.4657, -75.5564, -99.4773, 74.5251, 98.5329, -83.2432, 70.5688, -68.4671, -79.3403, -62.6724, -60.8476, 67.8379, 91.1800, 87.8499, -101.2957, -69.6481, -74.5603, 70.1766, -99.2101, 101.3056, 57.1986, 87.5917, 84.1423, -76.4349, -65.0490, 66.5703, 77.3265, 70.3819, 58.6750, -61.8244, 94.9379, 68.1455, 80.8718, 71.4065, -89.3790, -42.6856, -64.9363, 76.2369, 69.3416, -66.9824, -62.7680, 60.1339, -78.9674, 65.3749, -64.6940, 50.0190, -89.6008, -59.3167, -63.1129, 61.5982, 48.8499, 65.2957, -44.2573, -67.7464, -87.8192, -64.3863, -64.0232, -58.3138, 79.5344, 67.9879, -79.1206, -79.1714, 60.2715, 72.0637, 87.6743, 87.1759, 81.4093, -74.1212, 100.5560, -82.5535, -56.7645, 73.3080, -55.5333, 61.1872, 83.1372, 72.6622, 56.7458, -90.9942, -99.5641, -62.1492, 75.1305, -67.2248, 82.1078, -71.9184, -96.0142, -82.4769, 63.0060, 90.7906, -100.7988, -64.6227, -98.9736, 89.3586, 78.5604, 99.6034, 55.0377, 83.2926, -72.7276, -98.3970, 71.7933, 61.7939, 67.9014, -69.5731, 73.2906, -78.2155, 88.4656, 78.1025, -62.1181, -66.5374, 74.3818, 84.9285, 65.4854, 60.3368, -59.9013, 62.8409, 45.3090, 58.8132, -90.1745, -80.5019, 76.9129, -70.8013, 63.1397, -52.9220, 80.8111, -76.1652, 76.7023, -66.0006, -52.8898, -67.6308, 85.2930, 78.6230, 75.2349, -75.5770, 61.5977, -82.0592, 56.5244, 53.0226, -60.5902, 68.6878, 71.6496, -79.5789, 68.2251, 69.2261, -57.2262, 67.4926, -56.8821, -78.9174, 54.9742, -77.1147, 72.3281, 45.8284, 74.1518, 73.6083, -91.9549, -48.5210, -68.8685, -87.2434, 55.9644, -90.2183, 76.1801, -85.3346, 66.5699, -93.3345, 46.6941, 74.9255, -85.1393, 65.0381, 59.5640, -96.2469, 74.1641, 71.7959, -84.9770, 75.2968, 43.3046, -75.7478, 79.3113, -67.3357, 83.5540, 88.1043, 92.9397, 60.5756, 96.0108, 68.6091, 56.8510, -65.9826, 84.1422, -68.0985, 74.0803, 66.0246, 83.8283, 78.7515, -80.7086, 52.4481, -66.9362, 56.3773, 65.2047, -60.8237, -76.4423, 79.9544, 76.8582, -81.4292, -84.7288, -61.2944, -77.7179, -74.2870, 73.8435, -68.7351, -50.0336, 55.0304, 84.1329, 68.3470, -42.6786, 51.2943, -66.9083, -66.1926, 79.1121, -76.3870, -74.6423, 50.1182, 43.6267, -69.2405, 65.5949, 78.9524, 64.1765, -55.5729, -64.7979, 61.4107, -74.2137, -74.3217, 62.0394, -74.1537, 69.4664, -59.2044, -69.6405, 89.3530, -68.6773, -78.4004, -57.7046, -56.9396, -56.8815, 84.8120, 85.3458, 72.9297, 90.6085, 110.8704, 81.9232, 78.7975, -75.6312, -96.5727, -98.9427, -77.9188, 81.6283, -92.4196, -81.5016, 116.7946, 111.1792, -104.2775, -102.8753, 105.5464, 73.3699, -121.8863, -83.9218, 99.9105, -76.7338, 71.2199, 84.3709, 123.7199, 78.3144, -110.0666, -102.4246, -94.3307, 82.9367, 96.7602, 97.7912, -85.7501, 88.8595, -71.4018, -73.5545, -58.8523, -103.0843, 97.3005, 78.5062, -109.6570, 85.2691, -91.4737, 87.4685, -87.5806, 106.0338, 76.4113, 112.0384, -78.9545, -67.7884, -70.9985, 84.6570, 98.7297, 91.5841, -83.0778, 108.2129, -94.8490, -87.3756, -111.9341, -86.7001, 95.5885, 115.4110, 72.8125, -106.4446, 80.6854, -90.9581, 87.6573, 68.6028, 103.3637, -92.1900, -74.7351, 68.3605, -64.5109, -86.4599, 92.2079, -62.3135, -47.5140, 74.8112, -55.6607, 72.2295, 98.2756, -54.4462, 104.4787, -76.8929, -84.0509, -87.5470, 73.5025, -53.7392, -64.1919, 106.1772, 79.7842, -69.1110, -79.4048, -98.8703, -57.1228, 62.4514, -93.6077, -45.7700, -68.4287, 71.8675, 66.7427, -63.6768, 88.1545, -38.5373, -73.9172, 86.9245, -65.0378, -62.6790, 76.2379, -54.8815, 70.4215, -64.9437, -64.9268, -78.1091, -52.9684, -53.5112, -67.4531, -47.4951, 54.0182, 62.7692, 47.2771, 64.6934, 62.8590, -63.9107, 52.5923, 69.3743, -64.8862, -76.7852, -60.9050, 51.3035, -61.0244, 75.3462, 66.0729, -50.1459, 61.4202, 80.4490, -65.3638, 65.9481, 66.2290, 68.6534, 48.4402, 76.8827, -88.6572, -102.7420, -94.8729, -128.7776, -122.5039, -111.4672, -105.0354, 107.5132, 103.2147, 78.4791, -91.9850, -118.4194, -89.0634, -99.9338, 68.9210, -113.2486, -88.3158, -77.0076, -84.4593, 114.6763, 96.4872, 78.5846, -65.8721, -113.1152, 103.4743, 124.3876, 74.8503, -111.0042, -115.5840, 75.8457, 107.1602, -101.2862, -89.0443, -131.2639, -95.0169, -101.6776, 106.5587, -78.8672, 92.0872, 105.8629, -109.0139, 50.6957, 105.2203, 100.3173, -83.0163, -97.1313, -102.9198, -86.2367, -100.8920, 86.1522, 104.5341, -74.0529, -89.6591, -101.4711, 98.3851, -92.3188, -59.4171, 86.5606, 95.3560, 76.2519, 86.0034, -75.5908, 89.9902, -103.9601, 84.5431, -83.6168, 96.2207, -84.1777, -80.5586, 106.1140, -76.2755, -92.6383, 108.8716, -95.8761, 80.0378, -67.9769, 65.6445, -116.9681, 85.3114, 109.5884, 91.3763, -90.7064, -61.7081, -79.5426, 89.5249, -81.9820, 70.1122, -97.1048, 71.0162, -72.2081, 70.7452, -68.1885, -78.1658, -64.9691, -88.9413, 70.8800, -73.4284, 67.9446, -79.6382, -91.0749, 77.7375, 68.4846, -82.4107, -79.2529, 81.4335, 72.5728, -89.3588, -78.6540, 92.1629, -65.8376, -76.2695, -83.2549, 80.5638, 94.5750, -60.8127, 73.1588, 77.3830, -64.2280, 87.9001, -50.0027, 74.8442, 77.8280, 84.9365, -70.2339, 64.0379, 57.4044, -59.0314, -88.0455, 72.6950, 98.6087, -71.2674, -94.3452, 73.3607, 71.5727, -75.9903, 80.2090, -50.2199, -75.6587, -86.5366, -103.7038, 70.0617, 90.0493, 89.7471, -88.2946, -54.0257, -87.2369, 104.4625, -101.5353, 75.7854, 68.2742, 80.7305, 77.2729, -83.7552, -90.5382, 70.7754, 67.1356, 88.4907, 89.6675, -83.6852, 56.8200, 83.4220, 49.2676, 80.1260, -67.0996, -100.2257, -62.5562, 75.4357, 91.5392, -83.0123, -80.0729, 88.1559, -55.6654, 58.4997, -59.6680, 59.0821, -54.8626, -62.0851, -75.4294, 80.2651, 95.2739, 56.2296, -84.7247, -84.6150, -88.8262, -89.2111, -75.9162, -82.6932, 103.5515, 77.6816, -80.6825, -64.4125, 94.4056, 85.2704, 69.7562, 71.3295, 82.7432, -94.7477, 78.6021, -70.5708, -84.3440, 61.8713, -63.7839, 78.0555, 72.4840, 87.6374, 80.3411, -73.9080, -70.8911, -65.8246, 86.3262, -61.6859, 82.9255, -84.0396, -82.9138, -77.9931, 89.1368, 91.1653, -58.5482, -83.5073, -91.3116, 81.2495, 72.2874, 50.0016, 78.0471, 75.1215, -56.0254, -74.3332, 71.5110, 73.3624, 88.9567, -75.8943, 79.7566, -78.3273, 64.4678, 69.8261, -79.9440, -71.2289, 75.2226, 86.5812, 57.9802, 87.2199, -81.0658, 65.3986, 86.4986, 69.7224, -61.1344, -105.0467, 69.2449, -70.9433, 83.4344, -66.6032, 45.1522, -79.4094, 100.2277, -78.2417, -56.4543, -73.5083, 69.4708, 78.7618, 81.4791, -70.0314, 62.5427, -71.5135, 80.7320, 90.4718, -52.8129, 63.6561, 73.7117, -78.8202, 79.6381, 53.8892, -93.3015, 73.8935, -52.2579, -60.2833, 73.9423, -54.7339, 84.4312, 56.7623, 71.1906, 89.4435, -49.7766, -80.5811, -55.8977, -58.8677, 65.5685, -59.9771, 65.0678, -81.6615, 90.2745, -74.4305, 63.1864, 83.6006, -61.6714, 90.0837, 48.1648, -84.9140, 78.1148, 71.4074, -57.1791, 67.8951, 68.7683, -70.2009, 83.4573, -74.6282, 77.8962, 59.5611, 97.0689, 64.6330, 78.7713, 97.5969, 69.7465, -43.0201, 48.7812, -49.1213, 82.9030, 83.1607, 68.3046, 54.6260, -102.0873, 50.2760, -89.6055, 94.5197, 79.3946, -75.8153, -67.4159, 67.0226, 77.0560, -53.7410, -77.2953, -72.9407, -71.2448, -42.4205, 56.0560, -60.4946, -76.4592, 54.7078, 56.2773, 59.4870, -65.7878, 73.5729, -55.4234, -85.4392, 48.5772, -81.6894, -49.8058, 65.9435, 76.8729, -44.9569, 75.1489, 80.0595, 63.9259, -54.6950, -72.6381, 47.5685, -70.2114, -36.2244, 61.3018, -57.1606, 48.6657])
     # fmt: on
     L = 8
```

### Comparing `py3gpp-0.1.5/py3gpp/nrCRCEncode.py` & `py3gpp-0.1.6/py3gpp/nrCRCEncode.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import sys
 
 
 def nrCRCEncode(blk, poly, mask=0):
     if poly == "6":
         L = 6
         # fmt: off
         crc_coeffs = [6, 5, 0]
@@ -30,16 +29,15 @@
         # fmt: on
     elif poly == "24C":
         L = 24
         # fmt: off
         crc_coeffs = [24, 23, 21, 20, 17, 15, 13, 12, 8, 4, 2, 1, 0]
         # fmt: on
     else:
-        print("Error: invalid CRC polynomial specified!")
-        sys.exit()
+        raise ValueError('invalid CRC polynomial specified!')
     blksrc = np.empty(len(blk) + L, "int")
     blksrc[: len(blk)] = blk
 
     # build crc_poly
     crc_poly = 0
     for crc_coeff in crc_coeffs:
         crc_poly += 2**crc_coeff
@@ -53,16 +51,7 @@
             crc = crc << 1
     crc ^= mask
 
     # append crc LSB first
     for i in range(L):
         blksrc[len(blk) + i] = (crc >> (L - i - 1)) & 1
     return blksrc
-
-
-def test_nrCRCEncode():
-    test = np.zeros(32)
-    test[0] = 1
-    result = nrCRCEncode(test, "24C")
-    # fmt: off
-    assert np.all(result == [1, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 0, 0, 0, 1, 1, 0, 0, 0, 1, 1, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 0])
-    # fmt: on
```

### Comparing `py3gpp-0.1.5/py3gpp/nrChannelEstimate.py` & `py3gpp-0.1.6/py3gpp/nrChannelEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/nrOFDMDemodulate.py` & `py3gpp-0.1.6/py3gpp/nrOFDMDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/nrOFDMModulate.py` & `py3gpp-0.1.6/py3gpp/nrOFDMModulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from py3gpp import nrCarrierConfig
+from py3gpp.configs import nrCarrierConfig
 from py3gpp.nrOFDMInfo import nrOFDMInfo
 
 # TODO: implement windowing
 def nrOFDMModulate(
     carrier=None, grid=None, scs=None, initialNSlot=0, CyclicPrefix="normal", Nfft=None, SampleRate=None, Windowing=None
 ):
     info = {}
```

### Comparing `py3gpp-0.1.5/py3gpp/nrPBCHDMRSIndices.py` & `py3gpp-0.1.6/py3gpp/nrPBCHDMRSIndices.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,9 +10,9 @@
             (1 * np.ones(len(indices_sym1_3)), 2 * np.ones(len(indices_sym2)), 3 * np.ones(len(indices_sym1_3)))
         ).astype("int")
         return (tuple(indices), tuple(symbol_idx))
     elif style == "matlab":
         indices = np.concatenate((indices_sym1_3 + 240, indices_sym2 + 2 * 240, indices_sym1_3 + 3 * 240))
         return indices
     else:
-        print("Error: Unknown style!")
+        raise ValueError("Unknown style!")
         return
```

### Comparing `py3gpp-0.1.5/py3gpp/nrPolarDecode.py` & `py3gpp-0.1.6/py3gpp/nrPolarDecode.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/nrSSS.py` & `py3gpp-0.1.6/py3gpp/nrSSS.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import numpy as np
 from py3gpp.helper import _calc_m_seq
 
-def _gold(N_id_1, N_id_2):
+
+def nrSSSm0(ncellid):
+    n1 = ncellid // 3
+    n2 = ncellid % 3
+    return 15*(n1 // 112) + 5*n2
+
+
+def nrSSSm1(ncellid):
+    n1 = ncellid // 3
+    return n1 % 112
+
+
+def _gold(ncellid):
     N = 7
     c = [1, 0, 0, 0, 0, 0, 0]
     taps_0 = [0, 4]
     taps_1 = [0, 1]
     mseq_0 = _calc_m_seq(N, c, taps_0)
     mseq_1 = _calc_m_seq(N, c, taps_1)
-    m_0 = 15 * int((N_id_1 / 112)) + 5 * N_id_2
-    m_1 = N_id_1 % 112
+    m_0 = nrSSSm0(ncellid)
+    m_1 = nrSSSm1(ncellid)
     d_SSS = (1 - 2 * np.roll(mseq_0, -m_0)) * (1 - 2 * np.roll(mseq_1, -m_1))
     return d_SSS
 
 
 def nrSSS(ncellid):
-    N_id_2 = ncellid % 3
-    N_id_1 = (ncellid - N_id_2) // 3
-    return _gold(N_id_1, N_id_2)
+    assert ncellid >= 0 and ncellid <= 1007, "invalid ncellid"
+    return _gold(ncellid)
+
```

### Comparing `py3gpp-0.1.5/py3gpp/nrSymbolDemodulate.py` & `py3gpp-0.1.6/py3gpp/nrSymbolDemodulate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp/nrTimingEstimate.py` & `py3gpp-0.1.6/py3gpp/nrTimingEstimate.py`

 * *Files identical despite different names*

### Comparing `py3gpp-0.1.5/py3gpp.egg-info/PKG-INFO` & `py3gpp-0.1.6/py3gpp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3gpp
-Version: 0.1.5
+Version: 0.1.6
 Summary: Functions for 5G NR signal processing
 Author-email: Benjamin Menküc <benjamin@menkuec.de>
 Project-URL: Homepage, https://github.com/catkira/py3gpp
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `py3gpp-0.1.5/pyproject.toml` & `py3gpp-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     {name = "Benjamin Menküc", email = "benjamin@menkuec.de"},
 ]
 description = "Functions for 5G NR signal processing"
 name = "py3gpp"
 readme = "README.md"
 requires-python = ">=3.8"
```

