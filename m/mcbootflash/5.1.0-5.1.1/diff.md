# Comparing `tmp/mcbootflash-5.1.0.tar.gz` & `tmp/mcbootflash-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbootflash-5.1.0.tar", last modified: Fri Jan 13 09:37:00 2023, max compression
+gzip compressed data, was "mcbootflash-5.1.1.tar", last modified: Wed Apr 26 11:34:49 2023, max compression
```

## Comparing `mcbootflash-5.1.0.tar` & `mcbootflash-5.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      701 2022-11-29 18:35:23.675482 mcbootflash-5.1.0/.github/workflows/codecov.yml
--rw-r--r--   0        0        0      565 2022-11-29 18:35:07.854966 mcbootflash-5.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     3090 2022-06-14 11:40:06.628462 mcbootflash-5.1.0/.gitignore
--rw-r--r--   0        0        0      555 2022-11-29 18:06:08.690320 mcbootflash-5.1.0/.prospector.yaml
--rw-r--r--   0        0        0      120 2022-08-02 08:28:03.082718 mcbootflash-5.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     2201 2023-01-13 09:34:54.447972 mcbootflash-5.1.0/CHANGELOG.txt
--rw-r--r--   0        0        0     1068 2022-06-14 11:40:06.628462 mcbootflash-5.1.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-01-13 07:47:35.627968 mcbootflash-5.1.0/README.md
--rw-r--r--   0        0        0      638 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/Makefile
--rw-r--r--   0        0        0      769 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/make.bat
--rw-r--r--   0        0        0    38336 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/_static/session.gif
--rw-r--r--   0        0        0    22740 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/_static/session.odg
--rw-r--r--   0        0        0     1017 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/api.rst
--rw-r--r--   0        0        0     3357 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/cli.rst
--rw-r--r--   0        0        0     2210 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/conf.py
--rw-r--r--   0        0        0     5352 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/develop.rst
--rw-r--r--   0        0        0      420 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/index.rst
--rw-r--r--   0        0        0     2102 2022-11-29 18:06:08.686320 mcbootflash-5.1.0/docs/source/protocol.rst
--rw-r--r--   0        0        0     2119 2022-12-07 15:48:35.223486 mcbootflash-5.1.0/pyproject.toml
--rw-r--r--   0        0        0      272 2023-01-13 09:27:49.858261 mcbootflash-5.1.0/src/mcbootflash/__init__.py
--rw-r--r--   0        0        0    14606 2023-01-13 09:27:49.858261 mcbootflash-5.1.0/src/mcbootflash/connection.py
--rw-r--r--   0        0        0      981 2022-11-29 18:05:29.833054 mcbootflash-5.1.0/src/mcbootflash/error.py
--rw-r--r--   0        0        0     3690 2022-11-29 18:15:29.508587 mcbootflash-5.1.0/src/mcbootflash/flashing.py
--rw-r--r--   0        0        0     6136 2023-01-13 09:27:49.858261 mcbootflash-5.1.0/src/mcbootflash/protocol.py
--rw-r--r--   0        0        0    24828 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/test_mcbootflash.json
--rw-r--r--   0        0        0     3528 2022-11-29 18:30:00.340951 mcbootflash-5.1.0/tests/test_mcbootflash.py
--rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/testcases/checksum_error/test.hex
--rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/testcases/flash/test.hex
--rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/testcases/flash_empty/test.hex
--rw-r--r--   0        0        0     2932 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/testcases/no_data/test.hex
--rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.0/tests/testcases/no_response/test.hex
--rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 mcbootflash-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0      701 2022-11-29 18:35:23.675482 mcbootflash-5.1.1/.github/workflows/codecov.yml
+-rw-r--r--   0        0        0      565 2022-11-29 18:35:07.854966 mcbootflash-5.1.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3090 2022-06-14 11:40:06.628462 mcbootflash-5.1.1/.gitignore
+-rw-r--r--   0        0        0      555 2022-11-29 18:06:08.690320 mcbootflash-5.1.1/.prospector.yaml
+-rw-r--r--   0        0        0      120 2022-08-02 08:28:03.082718 mcbootflash-5.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     2263 2023-04-26 11:15:11.326518 mcbootflash-5.1.1/CHANGELOG.txt
+-rw-r--r--   0        0        0     1068 2022-06-14 11:40:06.628462 mcbootflash-5.1.1/LICENSE
+-rw-r--r--   0        0        0     1880 2023-02-06 13:47:40.692920 mcbootflash-5.1.1/README.md
+-rw-r--r--   0        0        0      638 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/Makefile
+-rw-r--r--   0        0        0      769 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/make.bat
+-rw-r--r--   0        0        0    38336 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/_static/session.gif
+-rw-r--r--   0        0        0    22740 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/_static/session.odg
+-rw-r--r--   0        0        0     1017 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/api.rst
+-rw-r--r--   0        0        0     3357 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/cli.rst
+-rw-r--r--   0        0        0     2210 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/conf.py
+-rw-r--r--   0        0        0     5352 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/develop.rst
+-rw-r--r--   0        0        0      420 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/index.rst
+-rw-r--r--   0        0        0     2102 2022-11-29 18:06:08.686320 mcbootflash-5.1.1/docs/source/protocol.rst
+-rw-r--r--   0        0        0     2119 2023-04-26 05:39:44.657872 mcbootflash-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0      272 2023-04-26 11:15:11.338519 mcbootflash-5.1.1/src/mcbootflash/__init__.py
+-rw-r--r--   0        0        0    14819 2023-04-26 11:15:11.346519 mcbootflash-5.1.1/src/mcbootflash/connection.py
+-rw-r--r--   0        0        0      981 2022-11-29 18:05:29.833054 mcbootflash-5.1.1/src/mcbootflash/error.py
+-rw-r--r--   0        0        0     3690 2023-04-26 05:39:44.661872 mcbootflash-5.1.1/src/mcbootflash/flashing.py
+-rw-r--r--   0        0        0     6136 2023-01-13 09:27:49.858261 mcbootflash-5.1.1/src/mcbootflash/protocol.py
+-rw-r--r--   0        0        0    24828 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/test_mcbootflash.json
+-rw-r--r--   0        0        0     3528 2022-11-29 18:30:00.340951 mcbootflash-5.1.1/tests/test_mcbootflash.py
+-rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/testcases/checksum_error/test.hex
+-rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/testcases/flash/test.hex
+-rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/testcases/flash_empty/test.hex
+-rw-r--r--   0        0        0     2932 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/testcases/no_data/test.hex
+-rw-r--r--   0        0        0     5628 2022-11-29 18:05:51.941774 mcbootflash-5.1.1/tests/testcases/no_response/test.hex
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 mcbootflash-5.1.1/PKG-INFO
```

### Comparing `mcbootflash-5.1.0/.github/workflows/codecov.yml` & `mcbootflash-5.1.1/.github/workflows/codecov.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/.github/workflows/main.yml` & `mcbootflash-5.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/.gitignore` & `mcbootflash-5.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/.prospector.yaml` & `mcbootflash-5.1.1/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/CHANGELOG.txt` & `mcbootflash-5.1.1/CHANGELOG.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+5.1.1
+
+Bug fixes:
+- Increase timeout during flash erase (#6)
+
 5.1.0
 
 Misc
 - Re-add some logging messages that were removed by mistake
 - Fix some minor docstring mistakes
 - Improve error message when receiving unexpected data
 - Add build status badge
```

### Comparing `mcbootflash-5.1.0/LICENSE` & `mcbootflash-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/README.md` & `mcbootflash-5.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![build](https://github.com/bessman/mcbootflash/actions/workflows/main.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/mcbootflash/badge/?version=latest)](https://mcbootflash.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b0cdb1c0b3b94171866fbfc4489316be)](https://www.codacy.com/gh/bessman/mcbootflash/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bessman/mcbootflash&amp;utm_campaign=Badge_Grade)
 [![Codecov](https://codecov.io/gh/bessman/mcbootflash/branch/main/graph/badge.svg)](https://codecov.io/gh/bessman/mcbootflash)
 
 
-Mcbootflash is a tool for flashing firmware to 16-bit Microchip MCUs and DSPs
+Mcbootflash is a tool for flashing firmware to 16-bit Microchip MCUs and DSCs
 from the PIC24 and dsPIC33 families of devices, which are running a
 [bootloader](https://www.microchip.com/en-us/software-library/16-bit-bootloader)
 generated by the MPLAB Code Configurator tool.
 
 Microchip provides an official GUI tool for this purpose, called the
 Unified Bootloader Host Application. Mcbootflash is intended to be a
 drop-in replacement, with some differences:
@@ -40,8 +40,8 @@
   Flashing firmware.hex
   100%  88.7 KiB |########################################| Elapsed Time: 0:00:05
   Self verify OK
 ```
 
 ## Copyright
 
-MIT License, (C) 2022 Alexander Bessman
+MIT License, (C) 2022-2023 Alexander Bessman
```

### Comparing `mcbootflash-5.1.0/docs/Makefile` & `mcbootflash-5.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/make.bat` & `mcbootflash-5.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/_static/session.gif` & `mcbootflash-5.1.1/docs/source/_static/session.gif`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/_static/session.odg` & `mcbootflash-5.1.1/docs/source/_static/session.odg`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/api.rst` & `mcbootflash-5.1.1/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/cli.rst` & `mcbootflash-5.1.1/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/conf.py` & `mcbootflash-5.1.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/develop.rst` & `mcbootflash-5.1.1/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/docs/source/protocol.rst` & `mcbootflash-5.1.1/docs/source/protocol.rst`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/pyproject.toml` & `mcbootflash-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/src/mcbootflash/connection.py` & `mcbootflash-5.1.1/src/mcbootflash/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,22 +293,28 @@
                 _logger.debug("An application was detected; flash erase failed")
                 _logger.debug("unlock_sequence field may be incorrect")
                 raise BootloaderError("Existing application could not be erased")
             _logger.info("No application detected; flash erase successful")
 
     def _erase_flash(self, start_address: int, end_address: int) -> None:
         _logger.debug(f"Erasing addresses {start_address:#08x}:{end_address:#08x}")
+        normal_timeout = self.interface.timeout
+
+        if self.interface.timeout is not None:
+            self.interface.timeout *= 10  # Erase may take a while.
+
         self._send_and_receive(
             command=Command(
                 command=CommandCode.ERASE_FLASH,
                 data_length=(end_address - start_address) // self._erase_size,
                 unlock_sequence=self._FLASH_UNLOCK_KEY,
                 address=start_address,
             )
         )
+        self.interface.timeout = normal_timeout
 
     def _detect_program(self) -> bool:
         try:
             # Program memory may be empty, which should not be logged as an error.
             _logger.disabled = True
             self._self_verify()
         except VerifyFail:
```

### Comparing `mcbootflash-5.1.0/src/mcbootflash/error.py` & `mcbootflash-5.1.1/src/mcbootflash/error.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/src/mcbootflash/flashing.py` & `mcbootflash-5.1.1/src/mcbootflash/flashing.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/src/mcbootflash/protocol.py` & `mcbootflash-5.1.1/src/mcbootflash/protocol.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/test_mcbootflash.json` & `mcbootflash-5.1.1/tests/test_mcbootflash.json`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/test_mcbootflash.py` & `mcbootflash-5.1.1/tests/test_mcbootflash.py`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/testcases/checksum_error/test.hex` & `mcbootflash-5.1.1/tests/testcases/checksum_error/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/testcases/flash/test.hex` & `mcbootflash-5.1.1/tests/testcases/flash/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/testcases/flash_empty/test.hex` & `mcbootflash-5.1.1/tests/testcases/flash_empty/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/testcases/no_data/test.hex` & `mcbootflash-5.1.1/tests/testcases/no_data/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/tests/testcases/no_response/test.hex` & `mcbootflash-5.1.1/tests/testcases/no_response/test.hex`

 * *Files identical despite different names*

### Comparing `mcbootflash-5.1.0/PKG-INFO` & `mcbootflash-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcbootflash
-Version: 5.1.0
+Version: 5.1.1
 Summary: Flash firmware to devices running Microchip's 16-bit bootloader.
 Keywords: firmware,flashing,bootloader,serial,uart,microchip,pic24,dspic33,16-bit
 Author-email: Alexander Bessman <alexander.bessman@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -26,15 +26,15 @@
 
 ![build](https://github.com/bessman/mcbootflash/actions/workflows/main.yml/badge.svg)
 [![Documentation Status](https://readthedocs.org/projects/mcbootflash/badge/?version=latest)](https://mcbootflash.readthedocs.io/en/latest/?badge=latest)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/b0cdb1c0b3b94171866fbfc4489316be)](https://www.codacy.com/gh/bessman/mcbootflash/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bessman/mcbootflash&amp;utm_campaign=Badge_Grade)
 [![Codecov](https://codecov.io/gh/bessman/mcbootflash/branch/main/graph/badge.svg)](https://codecov.io/gh/bessman/mcbootflash)
 
 
-Mcbootflash is a tool for flashing firmware to 16-bit Microchip MCUs and DSPs
+Mcbootflash is a tool for flashing firmware to 16-bit Microchip MCUs and DSCs
 from the PIC24 and dsPIC33 families of devices, which are running a
 [bootloader](https://www.microchip.com/en-us/software-library/16-bit-bootloader)
 generated by the MPLAB Code Configurator tool.
 
 Microchip provides an official GUI tool for this purpose, called the
 Unified Bootloader Host Application. Mcbootflash is intended to be a
 drop-in replacement, with some differences:
@@ -64,9 +64,9 @@
   Flashing firmware.hex
   100%  88.7 KiB |########################################| Elapsed Time: 0:00:05
   Self verify OK
 ```
 
 ## Copyright
 
-MIT License, (C) 2022 Alexander Bessman
+MIT License, (C) 2022-2023 Alexander Bessman
```

