# Comparing `tmp/Nuitka-winsvc-1.5.6.tar.gz` & `tmp/Nuitka-winsvc-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nuitka-winsvc-1.5.6.tar", last modified: Thu Apr 13 07:19:04 2023, max compression
+gzip compressed data, was "Nuitka-winsvc-1.5.7.tar", last modified: Wed Apr 26 09:52:44 2023, max compression
```

## Comparing `Nuitka-winsvc-1.5.6.tar` & `Nuitka-winsvc-1.5.7.tar`

### file list

```diff
@@ -1,1792 +1,1792 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.698797 Nuitka-winsvc-1.5.6/
--rw-rw-rw-   0        0        0   801878 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/Changelog.rst
--rw-rw-rw-   0        0        0   152121 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/Developer_Manual.rst
--rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/LICENSE.txt
--rw-rw-rw-   0        0        0     1751 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.910711 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/
--rw-rw-rw-   0        0        0     4626 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    76435 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      308 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 07:19:00.000000 Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4626 2023-04-13 07:19:04.698797 Nuitka-winsvc-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2651 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/README.md
--rw-rw-rw-   0        0        0    73222 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.918712 Nuitka-winsvc-1.5.6/bin/
--rw-rw-rw-   0        0        0     1135 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/autoformat-nuitka-source
--rw-rw-rw-   0        0        0     1136 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/check-nuitka-with-pylint
--rw-rw-rw-   0        0        0     1150 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/compare_with_cpython
--rw-rw-rw-   0        0        0     3079 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/compare_with_xml
--rw-rw-rw-   0        0        0     1163 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/measure-construct-performance
--rw-rw-rw-   0        0        0     1685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/nuitka
--rw-rw-rw-   0        0        0     1685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/bin/nuitka-run
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.766693 Nuitka-winsvc-1.5.6/doc/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.962838 Nuitka-winsvc-1.5.6/doc/Logo/
--rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Horizontal.svg
--rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Symbol.svg
--rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Vertical.svg
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.982330 Nuitka-winsvc-1.5.6/doc/images/
--rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Horizontal.png
--rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Symbol.png
--rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Vertical.png
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.983363 Nuitka-winsvc-1.5.6/lib/
--rw-rw-rw-   0        0        0     4250 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/lib/hints.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.986984 Nuitka-winsvc-1.5.6/misc/
--rwxrwxrwx   0        0        0      901 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/misc/nuitka-run.bat
--rwxrwxrwx   0        0        0     1038 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/misc/nuitka.bat
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.021712 Nuitka-winsvc-1.5.6/nuitka/
--rw-rw-rw-   0        0        0     7236 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/Builtins.py
--rw-rw-rw-   0        0        0     4919 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/BytecodeCaching.py
--rw-rw-rw-   0        0        0     3440 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/Bytecodes.py
--rw-rw-rw-   0        0        0     1884 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/CacheCleanup.py
--rw-rw-rw-   0        0        0    11148 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/Constants.py
--rw-rw-rw-   0        0        0     2447 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/Errors.py
--rw-rw-rw-   0        0        0    36691 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/MainControl.py
--rw-rw-rw-   0        0        0     8064 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/ModuleRegistry.py
--rw-rw-rw-   0        0        0    54557 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/nuitka/OptionParsing.py
--rw-rw-rw-   0        0        0    62842 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/nuitka/Options.py
--rw-rw-rw-   0        0        0     5022 2023-02-14 03:02:21.000000 Nuitka-winsvc-1.5.6/nuitka/OutputDirectories.py
--rw-rw-rw-   0        0        0    14550 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/PostProcessing.py
--rw-rw-rw-   0        0        0     5770 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/Progress.py
--rw-rw-rw-   0        0        0     7472 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/PythonFlavors.py
--rw-rw-rw-   0        0        0     4086 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/PythonOperators.py
--rw-rw-rw-   0        0        0    12083 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/PythonVersions.py
--rw-rw-rw-   0        0        0     4670 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/SourceCodeReferences.py
--rw-rw-rw-   0        0        0    11235 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/Tracing.py
--rw-rw-rw-   0        0        0     3395 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/TreeXML.py
--rw-rw-rw-   0        0        0    15235 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/Variables.py
--rw-rw-rw-   0        0        0     2055 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/Version.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/__init__.py
--rw-rw-rw-   0        0        0     5506 2023-02-22 01:49:06.000000 Nuitka-winsvc-1.5.6/nuitka/__main__.py
--rw-rw-rw-   0        0        0     5143 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/__past__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.042274 Nuitka-winsvc-1.5.6/nuitka/build/
--rw-rw-rw-   0        0        0    33043 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/Backend.scons
--rw-rw-rw-   0        0        0     8314 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/CCompilerVersion.scons
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/DataComposerInterface.py
--rw-rw-rw-   0        0        0    18493 2023-04-13 07:07:54.000000 Nuitka-winsvc-1.5.6/nuitka/build/Onefile.scons
--rw-rw-rw-   0        0        0    15210 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsCaching.py
--rw-rw-rw-   0        0        0    29056 2023-04-13 07:16:35.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsCompilerSettings.py
--rw-rw-rw-   0        0        0     5527 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsHacks.py
--rw-rw-rw-   0        0        0    15532 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsInterface.py
--rw-rw-rw-   0        0        0     2346 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsProgress.py
--rw-rw-rw-   0        0        0    11960 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsSpawn.py
--rw-rw-rw-   0        0        0    24258 2023-03-14 02:12:02.000000 Nuitka-winsvc-1.5.6/nuitka/build/SconsUtils.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.768697 Nuitka-winsvc-1.5.6/nuitka/build/include/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.108366 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/
--rw-rw-rw-   0        0        0     7769 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/allocator.h
--rw-rw-rw-   0        0        0     3423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/builtins.h
--rw-rw-rw-   0        0        0     4460 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/calling.h
--rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/checkers.h
--rw-rw-rw-   0        0        0     1261 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/checksum_tools.h
--rw-rw-rw-   0        0        0     9571 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_asyncgen.h
--rw-rw-rw-   0        0        0     2002 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_cell.h
--rw-rw-rw-   0        0        0     9325 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_coroutine.h
--rw-rw-rw-   0        0        0    16949 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_frame.h
--rw-rw-rw-   0        0        0     5972 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_function.h
--rw-rw-rw-   0        0        0     9136 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_generator.h
--rw-rw-rw-   0        0        0     1838 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_method.h
--rw-rw-rw-   0        0        0     7408 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/constants.h
--rw-rw-rw-   0        0        0     1293 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/constants_blob.h
--rw-rw-rw-   0        0        0    33190 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/exceptions.h
--rw-rw-rw-   0        0        0     3221 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/filesystem_paths.h
--rw-rw-rw-   0        0        0     6253 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/freelists.h
--rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/hedley.h
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.205366 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/
--rw-rw-rw-   0        0        0     3275 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/attributes.h
--rw-rw-rw-   0        0        0     2663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/boolean.h
--rw-rw-rw-   0        0        0     1181 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/bytearrays.h
--rw-rw-rw-   0        0        0     1135 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/bytes.h
--rw-rw-rw-   0        0        0     9335 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/calling_generated.h
--rw-rw-rw-   0        0        0    13140 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_eq.h
--rw-rw-rw-   0        0        0    10616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ge.h
--rw-rw-rw-   0        0        0    10615 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_gt.h
--rw-rw-rw-   0        0        0    13140 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_le.h
--rw-rw-rw-   0        0        0    13139 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_lt.h
--rw-rw-rw-   0        0        0    10616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ne.h
--rw-rw-rw-   0        0        0     1743 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/complex.h
--rw-rw-rw-   0        0        0    13077 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/dictionaries.h
--rw-rw-rw-   0        0        0     1206 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/floats.h
--rw-rw-rw-   0        0        0     3674 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/import_hard.h
--rw-rw-rw-   0        0        0     1798 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/indexes.h
--rw-rw-rw-   0        0        0     2941 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/ints.h
--rw-rw-rw-   0        0        0     9992 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/iterators.h
--rw-rw-rw-   0        0        0     3397 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/lists.h
--rw-rw-rw-   0        0        0     1633 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/lists_generated.h
--rw-rw-rw-   0        0        0     1328 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/mappings.h
--rw-rw-rw-   0        0        0     4573 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations.h
--rw-rw-rw-   0        0        0    12685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_add.h
--rw-rw-rw-   0        0        0     5663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
--rw-rw-rw-   0        0        0     5641 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
--rw-rw-rw-   0        0        0     5663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
--rw-rw-rw-   0        0        0     5422 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
--rw-rw-rw-   0        0        0     5460 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
--rw-rw-rw-   0        0        0     5115 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
--rw-rw-rw-   0        0        0     2799 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
--rw-rw-rw-   0        0        0    15778 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h
--rw-rw-rw-   0        0        0    13210 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h
--rw-rw-rw-   0        0        0     5791 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
--rw-rw-rw-   0        0        0     4714 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h
--rw-rw-rw-   0        0        0     5115 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
--rw-rw-rw-   0        0        0     5824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h
--rw-rw-rw-   0        0        0     5438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
--rw-rw-rw-   0        0        0    15100 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h
--rw-rw-rw-   0        0        0     8670 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h
--rw-rw-rw-   0        0        0     3767 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
--rw-rw-rw-   0        0        0     3753 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
--rw-rw-rw-   0        0        0     3767 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
--rw-rw-rw-   0        0        0     4846 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
--rw-rw-rw-   0        0        0     3011 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
--rw-rw-rw-   0        0        0     2727 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
--rw-rw-rw-   0        0        0    10626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
--rw-rw-rw-   0        0        0     9201 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
--rw-rw-rw-   0        0        0     5147 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
--rw-rw-rw-   0        0        0     4349 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
--rw-rw-rw-   0        0        0     3011 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
--rw-rw-rw-   0        0        0     4975 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
--rw-rw-rw-   0        0        0     4826 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
--rw-rw-rw-   0        0        0     3297 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/raising.h
--rw-rw-rw-   0        0        0     2178 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/rangeobjects.h
--rw-rw-rw-   0        0        0     1146 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/richcomparisons.h
--rw-rw-rw-   0        0        0     1112 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/sequences.h
--rw-rw-rw-   0        0        0     1025 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/sets.h
--rw-rw-rw-   0        0        0     8419 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/slices.h
--rw-rw-rw-   0        0        0     1242 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/strings.h
--rw-rw-rw-   0        0        0    17447 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/subscripts.h
--rw-rw-rw-   0        0        0     5720 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/tuples.h
--rw-rw-rw-   0        0        0    14375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helpers.h
--rw-rw-rw-   0        0        0     5363 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/importing.h
--rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/incbin.h
--rw-rw-rw-   0        0        0    14248 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/prelude.h
--rw-rw-rw-   0        0        0     2870 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/printing.h
--rw-rw-rw-   0        0        0     1761 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/python_pgo.h
--rw-rw-rw-   0        0        0     2119 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/safe_string_ops.h
--rw-rw-rw-   0        0        0     3840 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/threading.h
--rw-rw-rw-   0        0        0     3144 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/tracing.h
--rw-rw-rw-   0        0        0     2830 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/unfreezing.h
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.801911 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.208369 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/appdirs/
--rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/appdirs/LICENSE.txt
--rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/appdirs/appdirs.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.213366 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/atomicwrites/
--rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/atomicwrites/LICENSE
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.214367 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/bin/
--rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/bin/scons.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.772695 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.219371 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/
--rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/LICENSE
--rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/__init__.py
--rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/caching.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.221366 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/
--rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.229367 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/
--rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/__init__.py
--rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansi.py
--rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
--rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/initialise.py
--rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/win32.py
--rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/winterm.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.230366 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/
--rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.235369 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/
--rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/__init__.py
--rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/compat.py
--rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
--rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/impl.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.237366 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/LICENSE.rst
--rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.274812 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/
--rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.277794 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/
--rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
--rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.316801 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
--rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
--rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
--rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
--rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
--rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
--rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
--rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
--rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
--rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
--rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
--rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
--rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
--rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
--rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
--rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
--rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
--rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
--rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
--rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
--rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
--rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
--rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
--rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
--rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.789521 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.779518 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.348394 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
--rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
--rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
--rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.354394 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
--rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.362049 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
--rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
--rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
--rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
--rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
--rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.374524 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
--rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.379066 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.384638 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
--rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
--rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.510514 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
--rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
--rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.525008 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
--rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
--rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
--rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
--rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
--rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.526986 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
--rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
--rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
--rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
--rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
--rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.541742 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.561741 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
--rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
--rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
--rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
--rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
--rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
--rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
--rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.784518 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.630743 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
--rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
--rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
--rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
--rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
--rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
--rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
--rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
--rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
--rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.641743 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
--rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.664742 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
--rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
--rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.676741 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
--rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.681742 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
--rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
--rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.794392 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
--rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.810936 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.811935 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.812934 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
--rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
--rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
--rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.826476 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
--rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
--rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.829882 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
--rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
--rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
--rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.789521 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.862774 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
--rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
--rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
--rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
--rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
--rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
--rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
--rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
--rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
--rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
--rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
--rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
--rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.867932 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
--rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
--rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
--rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
--rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
--rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.889676 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
--rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
--rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
--rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
--rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
--rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
--rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
--rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
--rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
--rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
--rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
--rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
--rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
--rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.902253 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
--rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
--rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
--rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
--rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
--rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:01.913835 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
--rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
--rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
--rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
--rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
--rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
--rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
--rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.022740 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
--rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
--rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.032336 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
--rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
--rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
--rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
--rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
--rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
--rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
--rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
--rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
--rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
--rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
--rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
--rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
--rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
--rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
--rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
--rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
--rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
--rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
--rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
--rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
--rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.033344 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
--rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
--rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
--rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
--rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
--rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
--rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
--rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
--rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
--rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
--rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
--rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
--rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
--rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
--rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
--rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
--rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
--rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
--rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
--rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
--rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
--rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
--rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
--rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.038744 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
--rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
--rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
--rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
--rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
--rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
--rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
--rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
--rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
--rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
--rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
--rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
--rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
--rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
--rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
--rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
--rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
--rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
--rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
--rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
--rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
--rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
--rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
--rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
--rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
--rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
--rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
--rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
--rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
--rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
--rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
--rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
--rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
--rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
--rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.041741 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
--rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
--rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.047751 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
--rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
--rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
--rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
--rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
--rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
--rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
--rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
--rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.051741 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
--rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
--rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
--rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
--rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
--rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
--rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.052740 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/
--rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.059779 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/
--rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
--rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
--rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
--rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.797908 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.061777 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/
--rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
--rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.798907 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.083902 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/
--rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_main.py
--rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
--rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
--rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
--rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
--rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
--rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py
--rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
--rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py
--rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py
--rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
--rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/std.py
--rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py
--rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py
--rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.084902 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.107241 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/
--rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/__init__.py
--rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/composer.py
--rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/constructor.py
--rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/dumper.py
--rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/events.py
--rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/parser.py
--rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/reader.py
--rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/representer.py
--rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/resolver.py
--rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.109253 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.140030 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/
--rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
--rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py
--rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
--rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
--rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
--rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/events.py
--rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
--rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py
--rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py
--rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py
--rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
--rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
--rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.142027 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/
--rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.175206 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/
--rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
--rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py
--rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
--rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
--rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
--rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
--rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/error.py
--rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/events.py
--rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py
--rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
--rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py
--rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py
--rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py
--rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
--rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
--rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
--rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.177178 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/
--rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.201535 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/
--rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/bitstream.h
--rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/compiler.h
--rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/cpu.h
--rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/debug.h
--rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/entropy_common.c
--rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.c
--rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.h
--rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/fse.h
--rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c
--rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/huf.h
--rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/mem.h
--rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.c
--rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.h
--rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_common.c
--rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h
--rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h
--rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.212534 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/
--rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
--rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
--rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
--rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
--rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
--rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
--rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
--rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/zstd.h
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.340850 Nuitka-winsvc-1.5.6/nuitka/build/static_src/
--rw-rw-rw-   0        0        0    82114 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledAsyncgenType.c
--rw-rw-rw-   0        0        0     8250 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCellType.c
--rw-rw-rw-   0        0        0    57572 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCodeHelpers.c
--rw-rw-rw-   0        0        0    70973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCoroutineType.c
--rw-rw-rw-   0        0        0    35865 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledFrameType.c
--rw-rw-rw-   0        0        0    93999 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledFunctionType.c
--rw-rw-rw-   0        0        0    60657 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledGeneratorType.c
--rw-rw-rw-   0        0        0    26221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
--rw-rw-rw-   0        0        0    21493 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledMethodType.c
--rw-rw-rw-   0        0        0    18993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersAllocator.c
--rw-rw-rw-   0        0        0    32656 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersAttributes.c
--rw-rw-rw-   0        0        0    21783 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBuiltin.c
--rw-rw-rw-   0        0        0   107641 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
--rw-rw-rw-   0        0        0     3033 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBytes.c
--rw-rw-rw-   0        0        0    13057 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersCalling.c
--rw-rw-rw-   0        0        0   460993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersCallingGenerated.c
--rw-rw-rw-   0        0        0     1617 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersChecksumTools.c
--rw-rw-rw-   0        0        0     2991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersClasses.c
--rw-rw-rw-   0        0        0   317872 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonEq.c
--rw-rw-rw-   0        0        0     4673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonEqUtils.c
--rw-rw-rw-   0        0        0   313003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonGe.c
--rw-rw-rw-   0        0        0   312414 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonGt.c
--rw-rw-rw-   0        0        0   316217 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonLe.c
--rw-rw-rw-   0        0        0   315628 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonLt.c
--rw-rw-rw-   0        0        0   314618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonNe.c
--rw-rw-rw-   0        0        0    36011 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersConstantsBlob.c
--rw-rw-rw-   0        0        0    19313 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDeepcopy.c
--rw-rw-rw-   0        0        0    38320 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDictionaries.c
--rw-rw-rw-   0        0        0    24294 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDictionariesGenerated.c
--rw-rw-rw-   0        0        0     7035 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersExceptions.c
--rw-rw-rw-   0        0        0     6411 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFiles.c
--rw-rw-rw-   0        0        0    11199 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFilesystemPaths.c
--rw-rw-rw-   0        0        0     2426 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFloats.c
--rw-rw-rw-   0        0        0     1774 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersHeapStorage.c
--rw-rw-rw-   0        0        0    14561 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersImport.c
--rw-rw-rw-   0        0        0    13589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersImportHard.c
--rw-rw-rw-   0        0        0    18391 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersLists.c
--rw-rw-rw-   0        0        0    13915 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersListsGenerated.c
--rw-rw-rw-   0        0        0     1640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersMappings.c
--rw-rw-rw-   0        0        0     3513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersMatching.c
--rw-rw-rw-   0        0        0   181243 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c
--rw-rw-rw-   0        0        0    16700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
--rw-rw-rw-   0        0        0    77943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c
--rw-rw-rw-   0        0        0    77782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c
--rw-rw-rw-   0        0        0    77943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
--rw-rw-rw-   0        0        0    67487 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
--rw-rw-rw-   0        0        0     1236 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
--rw-rw-rw-   0        0        0    68748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
--rw-rw-rw-   0        0        0     6274 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
--rw-rw-rw-   0        0        0    83405 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c
--rw-rw-rw-   0        0        0    13776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
--rw-rw-rw-   0        0        0   183202 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMod.c
--rw-rw-rw-   0        0        0   188514 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMult.c
--rw-rw-rw-   0        0        0     3404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
--rw-rw-rw-   0        0        0    66453 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
--rw-rw-rw-   0        0        0    78891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPow.c
--rw-rw-rw-   0        0        0     1023 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
--rw-rw-rw-   0        0        0    77305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c
--rw-rw-rw-   0        0        0    70465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinarySub.c
--rw-rw-rw-   0        0        0    68005 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
--rw-rw-rw-   0        0        0   149580 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c
--rw-rw-rw-   0        0        0     4071 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
--rw-rw-rw-   0        0        0    53224 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c
--rw-rw-rw-   0        0        0    53122 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c
--rw-rw-rw-   0        0        0    53224 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
--rw-rw-rw-   0        0        0    76512 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
--rw-rw-rw-   0        0        0    47568 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c
--rw-rw-rw-   0        0        0    17742 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
--rw-rw-rw-   0        0        0   136100 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMod.c
--rw-rw-rw-   0        0        0   142211 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMult.c
--rw-rw-rw-   0        0        0    74142 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
--rw-rw-rw-   0        0        0    82669 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplacePow.c
--rw-rw-rw-   0        0        0    45052 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c
--rw-rw-rw-   0        0        0    82842 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceSub.c
--rw-rw-rw-   0        0        0    76343 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
--rw-rw-rw-   0        0        0     3219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersProfiling.c
--rw-rw-rw-   0        0        0     3805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersPythonPgo.c
--rw-rw-rw-   0        0        0    15369 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersRaising.c
--rw-rw-rw-   0        0        0    11094 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSafeStrings.c
--rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSequences.c
--rw-rw-rw-   0        0        0     1946 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSlices.c
--rw-rw-rw-   0        0        0    26642 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersStrings.c
--rw-rw-rw-   0        0        0     4037 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersTuples.c
--rw-rw-rw-   0        0        0     5578 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersTypes.c
--rw-rw-rw-   0        0        0    11945 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/InspectPatcher.c
--rw-rw-rw-   0        0        0    40893 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/MainProgram.c
--rw-rw-rw-   0        0        0    58321 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoader.c
--rw-rw-rw-   0        0        0     3650 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
--rw-rw-rw-   0        0        0     6427 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
--rw-rw-rw-   0        0        0    17065 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
--rw-rw-rw-   0        0        0    35978 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/OnefileBootstrap.c
--rw-rw-rw-   0        0        0     7800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/build/static_src/OnefileSplashScreen.cpp
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.434322 Nuitka-winsvc-1.5.6/nuitka/code_generation/
--rw-rw-rw-   0        0        0     6346 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/AsyncgenCodes.py
--rw-rw-rw-   0        0        0    10153 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/AttributeCodes.py
--rw-rw-rw-   0        0        0    21864 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py
--rw-rw-rw-   0        0        0     2339 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/BranchCodes.py
--rw-rw-rw-   0        0        0    16009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/BuiltinCodes.py
--rw-rw-rw-   0        0        0    35905 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CallCodes.py
--rw-rw-rw-   0        0        0     4896 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ClassCodes.py
--rw-rw-rw-   0        0        0    51024 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeGeneration.py
--rw-rw-rw-   0        0        0     2375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeHelperSelection.py
--rw-rw-rw-   0        0        0    14392 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeHelpers.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeObjectCodes.py
--rw-rw-rw-   0        0        0    16827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ComparisonCodes.py
--rw-rw-rw-   0        0        0     4446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ComparisonHelperDefinitions.py
--rw-rw-rw-   0        0        0     7335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ConditionalCodes.py
--rw-rw-rw-   0        0        0     5879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ConstantCodes.py
--rw-rw-rw-   0        0        0    31196 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/Contexts.py
--rw-rw-rw-   0        0        0     8416 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CoroutineCodes.py
--rw-rw-rw-   0        0        0     1574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/CtypesCodes.py
--rw-rw-rw-   0        0        0    28478 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/DictCodes.py
--rw-rw-rw-   0        0        0     2125 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/Emission.py
--rw-rw-rw-   0        0        0     9325 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ErrorCodes.py
--rw-rw-rw-   0        0        0    12304 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/EvalCodes.py
--rw-rw-rw-   0        0        0     8975 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ExceptionCodes.py
--rw-rw-rw-   0        0        0     7350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
--rw-rw-rw-   0        0        0     2093 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ExpressionCodes.py
--rw-rw-rw-   0        0        0    17725 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/FrameCodes.py
--rw-rw-rw-   0        0        0    27345 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/FunctionCodes.py
--rw-rw-rw-   0        0        0     7622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/GeneratorCodes.py
--rw-rw-rw-   0        0        0     5721 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/GlobalConstants.py
--rw-rw-rw-   0        0        0     6911 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/GlobalsLocalsCodes.py
--rw-rw-rw-   0        0        0     1794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/IdCodes.py
--rw-rw-rw-   0        0        0    13294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ImportCodes.py
--rw-rw-rw-   0        0        0     1396 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/Indentation.py
--rw-rw-rw-   0        0        0     1506 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/IndexCodes.py
--rw-rw-rw-   0        0        0     1033 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/InjectCCodes.py
--rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/IntegerCodes.py
--rw-rw-rw-   0        0        0    12010 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/IteratorCodes.py
--rw-rw-rw-   0        0        0     2022 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/LabelCodes.py
--rw-rw-rw-   0        0        0     2612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/LineNumberCodes.py
--rw-rw-rw-   0        0        0    15892 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ListCodes.py
--rw-rw-rw-   0        0        0     6375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/LoaderCodes.py
--rw-rw-rw-   0        0        0     9951 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/LocalsDictCodes.py
--rw-rw-rw-   0        0        0     3135 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/LoopCodes.py
--rw-rw-rw-   0        0        0     1597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/MatchCodes.py
--rw-rw-rw-   0        0        0     6291 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ModuleCodes.py
--rw-rw-rw-   0        0        0     8118 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/Namify.py
--rw-rw-rw-   0        0        0    12777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/OperationCodes.py
--rw-rw-rw-   0        0        0    28479 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/PackageResourceCodes.py
--rw-rw-rw-   0        0        0     3021 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/PrintCodes.py
--rw-rw-rw-   0        0        0     5474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/PythonAPICodes.py
--rw-rw-rw-   0        0        0    13095 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/RaisingCodes.py
--rw-rw-rw-   0        0        0     3443 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/Reports.py
--rw-rw-rw-   0        0        0     5234 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/ReturnCodes.py
--rw-rw-rw-   0        0        0     6517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/SetCodes.py
--rw-rw-rw-   0        0        0    13949 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/SliceCodes.py
--rw-rw-rw-   0        0        0     9809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/StringCodes.py
--rw-rw-rw-   0        0        0     8188 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/SubscriptCodes.py
--rw-rw-rw-   0        0        0    11176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/TryCodes.py
--rw-rw-rw-   0        0        0     3786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/TupleCodes.py
--rw-rw-rw-   0        0        0    14717 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/VariableCodes.py
--rw-rw-rw-   0        0        0     9121 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/VariableDeclarations.py
--rw-rw-rw-   0        0        0     8099 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/YieldCodes.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.455929 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/
--rw-rw-rw-   0        0        0     6069 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeBases.py
--rw-rw-rw-   0        0        0     3399 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeBooleans.py
--rw-rw-rw-   0        0        0     1804 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeCFloats.py
--rw-rw-rw-   0        0        0     1378 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeCLongs.py
--rw-rw-rw-   0        0        0     3610 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
--rw-rw-rw-   0        0        0     5128 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
--rw-rw-rw-   0        0        0     5211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py
--rw-rw-rw-   0        0        0     4017 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
--rw-rw-rw-   0        0        0    19628 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py
--rw-rw-rw-   0        0        0     2852 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeVoids.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.472927 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/
--rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
--rw-rw-rw-   0        0        0     5747 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesConstants.py
--rw-rw-rw-   0        0        0     2805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
--rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py
--rw-rw-rw-   0        0        0     6339 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesFrames.py
--rw-rw-rw-   0        0        0     3321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesFunction.py
--rw-rw-rw-   0        0        0     3190 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
--rw-rw-rw-   0        0        0     2335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesIterators.py
--rw-rw-rw-   0        0        0     4217 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesLoader.py
--rw-rw-rw-   0        0        0    21441 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesModules.py
--rw-rw-rw-   0        0        0     6640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesVariables.py
--rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/TemplateDebugWrapper.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.516442 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/
--rw-rw-rw-   0        0        0    11231 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
--rw-rw-rw-   0        0        0     5904 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
--rw-rw-rw-   0        0        0    23262 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
--rw-rw-rw-   0        0        0     5238 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
--rw-rw-rw-   0        0        0     1905 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
--rw-rw-rw-   0        0        0     1843 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
--rw-rw-rw-   0        0        0     2817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
--rw-rw-rw-   0        0        0    12818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
--rw-rw-rw-   0        0        0     2044 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2
--rw-rw-rw-   0        0        0     2762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2
--rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
--rw-rw-rw-   0        0        0     7197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
--rw-rw-rw-   0        0        0    12850 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
--rw-rw-rw-   0        0        0     4288 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
--rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
--rw-rw-rw-   0        0        0     2118 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
--rw-rw-rw-   0        0        0     3933 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
--rw-rw-rw-   0        0        0     7407 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
--rw-rw-rw-   0        0        0     4292 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
--rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
--rw-rw-rw-   0        0        0     4487 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
--rw-rw-rw-   0        0        0    11579 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
--rw-rw-rw-   0        0        0    19317 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
--rw-rw-rw-   0        0        0     2843 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
--rw-rw-rw-   0        0        0     3635 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
--rw-rw-rw-   0        0        0    11102 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
--rw-rw-rw-   0        0        0    15380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
--rw-rw-rw-   0        0        0     2979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
--rw-rw-rw-   0        0        0    10421 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
--rw-rw-rw-   0        0        0     2557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
--rw-rw-rw-   0        0        0     3020 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
--rw-rw-rw-   0        0        0     2984 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
--rw-rw-rw-   0        0        0     3173 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.519446 Nuitka-winsvc-1.5.6/nuitka/constants/
--rw-rw-rw-   0        0        0     8524 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/constants/Serialization.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/constants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.526443 Nuitka-winsvc-1.5.6/nuitka/containers/
--rw-rw-rw-   0        0        0     1435 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/containers/Namedtuples.py
--rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/containers/OrderedDicts.py
--rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/containers/OrderedSets.py
--rw-rw-rw-   0        0        0     4397 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/containers/OrderedSetsFallback.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/containers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.529442 Nuitka-winsvc-1.5.6/nuitka/distutils/
--rw-rw-rw-   0        0        0     1964 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/distutils/Build.py
--rw-rw-rw-   0        0        0    12729 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/distutils/DistutilCommands.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/distutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.531443 Nuitka-winsvc-1.5.6/nuitka/finalizations/
--rw-rw-rw-   0        0        0     1224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/finalizations/Finalization.py
--rw-rw-rw-   0        0        0     6110 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/finalizations/FinalizeMarkups.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/finalizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.545443 Nuitka-winsvc-1.5.6/nuitka/freezer/
--rw-rw-rw-   0        0        0     7311 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/DependsExe.py
--rw-rw-rw-   0        0        0     2380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesCommon.py
--rw-rw-rw-   0        0        0    10109 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesMacOS.py
--rw-rw-rw-   0        0        0     7211 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesPosix.py
--rw-rw-rw-   0        0        0     6620 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesWin32.py
--rw-rw-rw-   0        0        0    16587 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/IncludedDataFiles.py
--rw-rw-rw-   0        0        0     9146 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/IncludedEntryPoints.py
--rw-rw-rw-   0        0        0     9795 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/Onefile.py
--rw-rw-rw-   0        0        0    25217 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/Standalone.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/freezer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.556455 Nuitka-winsvc-1.5.6/nuitka/importing/
--rw-rw-rw-   0        0        0    10934 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/IgnoreListing.py
--rw-rw-rw-   0        0        0     2899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/ImportCache.py
--rw-rw-rw-   0        0        0     6455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/ImportResolving.py
--rw-rw-rw-   0        0        0    27820 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/Importing.py
--rw-rw-rw-   0        0        0     4739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/PreloadedPackages.py
--rw-rw-rw-   0        0        0    16375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/importing/Recursion.py
--rw-rw-rw-   0        0        0    10383 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/StandardLibrary.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/importing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.670652 Nuitka-winsvc-1.5.6/nuitka/nodes/
--rw-rw-rw-   0        0        0     3637 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/AsyncgenNodes.py
--rw-rw-rw-   0        0        0     4082 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeLookupNodes.py
--rw-rw-rw-   0        0        0    12004 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeNodes.py
--rw-rw-rw-   0        0        0   378745 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeNodesGenerated.py
--rw-rw-rw-   0        0        0     3823 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinAllNodes.py
--rw-rw-rw-   0        0        0     4098 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinAnyNodes.py
--rw-rw-rw-   0        0        0     2496 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinComplexNodes.py
--rw-rw-rw-   0        0        0     1698 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDecodingNodes.py
--rw-rw-rw-   0        0        0     2727 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDecoratorNodes.py
--rw-rw-rw-   0        0        0     4694 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDictNodes.py
--rw-rw-rw-   0        0        0     4948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinFormatNodes.py
--rw-rw-rw-   0        0        0     2142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinHashNodes.py
--rw-rw-rw-   0        0        0     5334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinIntegerNodes.py
--rw-rw-rw-   0        0        0    12723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinIteratorNodes.py
--rw-rw-rw-   0        0        0     1996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinLenNodes.py
--rw-rw-rw-   0        0        0     3606 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinNextNodes.py
--rw-rw-rw-   0        0        0     3240 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinOpenNodes.py
--rw-rw-rw-   0        0        0   245536 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
--rw-rw-rw-   0        0        0    18589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinRangeNodes.py
--rw-rw-rw-   0        0        0     9067 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinRefNodes.py
--rw-rw-rw-   0        0        0     3307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinSumNodes.py
--rw-rw-rw-   0        0        0    13543 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinTypeNodes.py
--rw-rw-rw-   0        0        0     1573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinVarsNodes.py
--rw-rw-rw-   0        0        0    26113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/BytesNodes.py
--rw-rw-rw-   0        0        0     6478 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/CallNodes.py
--rw-rw-rw-   0        0        0     1550 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/Checkers.py
--rw-rw-rw-   0        0        0   605501 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ChildrenHavingMixins.py
--rw-rw-rw-   0        0        0     8448 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ClassNodes.py
--rw-rw-rw-   0        0        0     6585 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/CodeObjectSpecs.py
--rw-rw-rw-   0        0        0    21683 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ComparisonNodes.py
--rw-rw-rw-   0        0        0    30314 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ConditionalNodes.py
--rw-rw-rw-   0        0        0    46286 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ConstantRefNodes.py
--rw-rw-rw-   0        0        0    12213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ContainerMakingNodes.py
--rw-rw-rw-   0        0        0     2834 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ContainerOperationNodes.py
--rw-rw-rw-   0        0        0     4581 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/CoroutineNodes.py
--rw-rw-rw-   0        0        0     1714 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/CtypesNodes.py
--rw-rw-rw-   0        0        0    50665 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/DictionaryNodes.py
--rw-rw-rw-   0        0        0     7856 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ExceptionNodes.py
--rw-rw-rw-   0        0        0     8044 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ExecEvalNodes.py
--rw-rw-rw-   0        0        0    44996 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionBases.py
--rw-rw-rw-   0        0        0    41307 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionBasesGenerated.py
--rw-rw-rw-   0        0        0    21278 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionShapeMixins.py
--rw-rw-rw-   0        0        0    12156 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/FrameNodes.py
--rw-rw-rw-   0        0        0     3544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/FunctionAttributeNodes.py
--rw-rw-rw-   0        0        0    39726 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/FunctionNodes.py
--rw-rw-rw-   0        0        0     5376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/FutureSpecs.py
--rw-rw-rw-   0        0        0     6256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/GeneratorNodes.py
--rw-rw-rw-   0        0        0     6850 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/GlobalsLocalsNodes.py
--rw-rw-rw-   0        0        0    74177 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/HardImportNodesGenerated.py
--rw-rw-rw-   0        0        0     5491 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ImportHardNodes.py
--rw-rw-rw-   0        0        0    45573 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ImportNodes.py
--rw-rw-rw-   0        0        0     2733 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/IndicatorMixins.py
--rw-rw-rw-   0        0        0     1502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/InjectCNodes.py
--rw-rw-rw-   0        0        0    11228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/IterationHandles.py
--rw-rw-rw-   0        0        0    11002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/KeyValuePairNodes.py
--rw-rw-rw-   0        0        0    16320 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ListOperationNodes.py
--rw-rw-rw-   0        0        0    23094 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/LocalsDictNodes.py
--rw-rw-rw-   0        0        0    14922 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/LocalsScopes.py
--rw-rw-rw-   0        0        0    15581 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/LoopNodes.py
--rw-rw-rw-   0        0        0     1712 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/MatchNodes.py
--rw-rw-rw-   0        0        0     6534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ModuleAttributeNodes.py
--rw-rw-rw-   0        0        0    34414 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ModuleNodes.py
--rw-rw-rw-   0        0        0    24899 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/NodeBases.py
--rw-rw-rw-   0        0        0    15128 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/NodeMakingHelpers.py
--rw-rw-rw-   0        0        0     5618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/NodeMetaClasses.py
--rw-rw-rw-   0        0        0    31894 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/OperatorNodes.py
--rw-rw-rw-   0        0        0     9134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/OperatorNodesUnary.py
--rw-rw-rw-   0        0        0     4202 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/OsSysNodes.py
--rw-rw-rw-   0        0        0    12442 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/OutlineNodes.py
--rw-rw-rw-   0        0        0    31342 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/PackageMetadataNodes.py
--rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/PackageResourceNodes.py
--rw-rw-rw-   0        0        0     3407 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/PrintNodes.py
--rw-rw-rw-   0        0        0     6772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/ReturnNodes.py
--rw-rw-rw-   0        0        0     4309 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/SideEffectNodes.py
--rw-rw-rw-   0        0        0    12501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/SliceNodes.py
--rw-rw-rw-   0        0        0    94880 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/StatementBasesGenerated.py
--rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/StatementNodes.py
--rw-rw-rw-   0        0        0    28658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/StrNodes.py
--rw-rw-rw-   0        0        0     3504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/StringConcatenationNodes.py
--rw-rw-rw-   0        0        0     8640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/SubscriptNodes.py
--rw-rw-rw-   0        0        0    17853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/TryNodes.py
--rw-rw-rw-   0        0        0     2405 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/TypeMatchNodes.py
--rw-rw-rw-   0        0        0     9800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/TypeNodes.py
--rw-rw-rw-   0        0        0    39522 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/VariableAssignNodes.py
--rw-rw-rw-   0        0        0    10746 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/VariableDelNodes.py
--rw-rw-rw-   0        0        0     4574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/VariableNameNodes.py
--rw-rw-rw-   0        0        0    30982 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/VariableRefNodes.py
--rw-rw-rw-   0        0        0     4550 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/VariableReleaseNodes.py
--rw-rw-rw-   0        0        0     3902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/YieldNodes.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.679638 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/
--rw-rw-rw-   0        0        0   156168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/BuiltinTypeShapes.py
--rw-rw-rw-   0        0        0     4387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/ControlFlowDescriptions.py
--rw-rw-rw-   0        0        0     4567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/ShapeMixins.py
--rw-rw-rw-   0        0        0    42374 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/StandardShapes.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.696642 Nuitka-winsvc-1.5.6/nuitka/optimizations/
--rw-rw-rw-   0        0        0     3279 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/BytecodeDemotion.py
--rw-rw-rw-   0        0        0     4038 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/FunctionInlining.py
--rw-rw-rw-   0        0        0     2144 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/Graphs.py
--rw-rw-rw-   0        0        0    10762 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/Optimization.py
--rw-rw-rw-   0        0        0    52154 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/OptimizeBuiltinCalls.py
--rw-rw-rw-   0        0        0     2272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/Tags.py
--rw-rw-rw-   0        0        0    40896 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/TraceCollections.py
--rw-rw-rw-   0        0        0    23977 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/ValueTraces.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/optimizations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.699638 Nuitka-winsvc-1.5.6/nuitka/pgo/
--rw-rw-rw-   0        0        0     4663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/pgo/PGO.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/pgo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.703650 Nuitka-winsvc-1.5.6/nuitka/plugins/
--rw-rw-rw-   0        0        0    39068 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/PluginBase.py
--rw-rw-rw-   0        0        0    52710 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/Plugins.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.745103 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/
--rw-rw-rw-   0        0        0    18092 2023-02-14 03:02:21.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/AntiBloatPlugin.py
--rw-rw-rw-   0        0        0     3460 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
--rw-rw-rw-   0        0        0     9939 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DataFilesPlugin.py
--rw-rw-rw-   0        0        0     4051 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DelvewheelPlugin.py
--rw-rw-rw-   0        0        0     5675 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DillPlugin.py
--rw-rw-rw-   0        0        0    12182 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DllFilesPlugin.py
--rw-rw-rw-   0        0        0     2062 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/EnumPlugin.py
--rw-rw-rw-   0        0        0     1905 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/EventletPlugin.py
--rw-rw-rw-   0        0        0     1880 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GeventPlugin.py
--rw-rw-rw-   0        0        0     3482 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GiPlugin.py
--rw-rw-rw-   0        0        0     5027 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GlfwPlugin.py
--rw-rw-rw-   0        0        0    18758 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/ImplicitImports.py
--rw-rw-rw-   0        0        0     4948 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/KivyPlugin.py
--rw-rw-rw-   0        0        0     7258 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/MatplotlibPlugin.py
--rw-rw-rw-   0        0        0     6750 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/MultiprocessingPlugin.py
--rw-rw-rw-   0        0        0     1187 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/NumpyPlugin.py
--rw-rw-rw-   0        0        0     6554 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/OptionsNannyPlugin.py
--rw-rw-rw-   0        0        0     1917 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PbrPlugin.py
--rw-rw-rw-   0        0        0     4665 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PkgResourcesPlugin.py
--rw-rw-rw-   0        0        0     6992 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PmwPlugin.py
--rw-rw-rw-   0        0        0    49325 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PySidePyQtPlugin.py
--rw-rw-rw-   0        0        0     2933 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PywebViewPlugin.py
--rw-rw-rw-   0        0        0     1160 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TensorflowPlugin.py
--rw-rw-rw-   0        0        0    12180 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TkinterPlugin.py
--rw-rw-rw-   0        0        0     1140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TorchPlugin.py
--rw-rw-rw-   0        0        0     3175 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TrioPlugin.py
--rw-rw-rw-   0        0        0     5553 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/UpxPlugin.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/__init__.py
--rw-rw-rw-   0        0        0   124572 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/standard.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
--rw-rw-rw-   0        0        0     8831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.747694 Nuitka-winsvc-1.5.6/nuitka/reports/
--rw-rw-rw-   0        0        0     2209 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/reports/LicenseReport.rst.j2
--rw-rw-rw-   0        0        0    15558 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/reports/Reports.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/reports/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.759689 Nuitka-winsvc-1.5.6/nuitka/specs/
--rw-rw-rw-   0        0        0     5911 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinBytesOperationSpecs.py
--rw-rw-rw-   0        0        0     2786 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinDictOperationSpecs.py
--rw-rw-rw-   0        0        0     2541 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinListOperationSpecs.py
--rw-rw-rw-   0        0        0    26455 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinParameterSpecs.py
--rw-rw-rw-   0        0        0     6065 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinStrOperationSpecs.py
--rw-rw-rw-   0        0        0     1159 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinTypeOperationSpecs.py
--rw-rw-rw-   0        0        0     4802 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py
--rw-rw-rw-   0        0        0     5133 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/specs/HardImportSpecs.py
--rw-rw-rw-   0        0        0    18781 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/specs/ParameterSpecs.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/specs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.761689 Nuitka-winsvc-1.5.6/nuitka/tools/
--rw-rw-rw-   0        0        0     1603 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/Basics.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.762693 Nuitka-winsvc-1.5.6/nuitka/tools/commercial/
--rw-rw-rw-   0        0        0      815 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/commercial/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.767005 Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/
--rw-rw-rw-   0        0        0    14081 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/DataComposer.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/__init__.py
--rw-rw-rw-   0        0        0     1306 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.772967 Nuitka-winsvc-1.5.6/nuitka/tools/environments/
--rw-rw-rw-   0        0        0     2449 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/environments/CreateEnvironment.py
--rw-rw-rw-   0        0        0     3735 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/environments/Virtualenv.py
--rw-rw-rw-   0        0        0      833 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/environments/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.773967 Nuitka-winsvc-1.5.6/nuitka/tools/general/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/general/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.776809 Nuitka-winsvc-1.5.6/nuitka/tools/general/dll_report/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/general/dll_report/__init__.py
--rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/general/dll_report/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.778806 Nuitka-winsvc-1.5.6/nuitka/tools/general/find_module/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/general/find_module/__init__.py
--rw-rw-rw-   0        0        0     1238 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/general/find_module/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.782806 Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/
--rw-rw-rw-   0        0        0     8869 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/OnefileCompressor.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.785810 Nuitka-winsvc-1.5.6/nuitka/tools/profiler/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/profiler/__init__.py
--rw-rw-rw-   0        0        0     2529 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/profiler/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.790806 Nuitka-winsvc-1.5.6/nuitka/tools/scanning/
--rw-rw-rw-   0        0        0     2369 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/scanning/DisplayPackageDLLs.py
--rw-rw-rw-   0        0        0     2049 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/scanning/DisplayPackageData.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/scanning/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.796526 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/
--rw-rw-rw-   0        0        0    51143 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/CTypeDescriptions.py
--rw-rw-rw-   0        0        0     7685 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/Common.py
--rw-rw-rw-   0        0        0    39625 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/SpecializeC.py
--rw-rw-rw-   0        0        0    33585 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/SpecializePython.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/specialize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.807309 Nuitka-winsvc-1.5.6/nuitka/tools/testing/
--rw-rw-rw-   0        0        0    55189 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/Common.py
--rw-rw-rw-   0        0        0     1483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/Constructs.py
--rw-rw-rw-   0        0        0     8940 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/OutputComparison.py
--rw-rw-rw-   0        0        0     1278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/Pythons.py
--rw-rw-rw-   0        0        0     7888 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/RuntimeTracing.py
--rw-rw-rw-   0        0        0     5371 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/SearchModes.py
--rw-rw-rw-   0        0        0     3375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/Valgrind.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.809306 Nuitka-winsvc-1.5.6/nuitka/tools/testing/check_reference_counts/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/check_reference_counts/__init__.py
--rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/check_reference_counts/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.811306 Nuitka-winsvc-1.5.6/nuitka/tools/testing/compare_with_cpython/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/compare_with_cpython/__init__.py
--rw-rw-rw-   0        0        0    29429 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/compare_with_cpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.813305 Nuitka-winsvc-1.5.6/nuitka/tools/testing/find_sxs_modules/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/find_sxs_modules/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/find_sxs_modules/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.816314 Nuitka-winsvc-1.5.6/nuitka/tools/testing/measure_construct_performance/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/measure_construct_performance/__init__.py
--rw-rw-rw-   0        0        0     8755 2023-02-22 01:49:06.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/measure_construct_performance/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.818324 Nuitka-winsvc-1.5.6/nuitka/tools/testing/run_nuitka_tests/
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/run_nuitka_tests/__init__.py
--rw-rw-rw-   0        0        0    36321 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tools/testing/run_nuitka_tests/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.887983 Nuitka-winsvc-1.5.6/nuitka/tree/
--rw-rw-rw-   0        0        0    46475 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/Building.py
--rw-rw-rw-   0        0        0    75578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ComplexCallHelperFunctions.py
--rw-rw-rw-   0        0        0     1700 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/Extractions.py
--rw-rw-rw-   0        0        0     2572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/InternalModule.py
--rw-rw-rw-   0        0        0     1511 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/Operations.py
--rw-rw-rw-   0        0        0     2807 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationAssertStatements.py
--rw-rw-rw-   0        0        0    42974 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationAssignmentStatements.py
--rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationBooleanExpressions.py
--rw-rw-rw-   0        0        0    11693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationCallExpressions.py
--rw-rw-rw-   0        0        0    15208 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationClasses.py
--rw-rw-rw-   0        0        0    30125 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationClasses3.py
--rw-rw-rw-   0        0        0     6430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationComparisonExpressions.py
--rw-rw-rw-   0        0        0    22111 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationContractionExpressions.py
--rw-rw-rw-   0        0        0    11160 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationDictionaryCreation.py
--rw-rw-rw-   0        0        0    14876 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationExecStatements.py
--rw-rw-rw-   0        0        0     7782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationForLoopStatements.py
--rw-rw-rw-   0        0        0    26211 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationFunctionStatements.py
--rw-rw-rw-   0        0        0    13437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationImportStatements.py
--rw-rw-rw-   0        0        0     6577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationLambdaExpressions.py
--rw-rw-rw-   0        0        0    20962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationMatchStatements.py
--rw-rw-rw-   0        0        0     2409 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationMultidist.py
--rw-rw-rw-   0        0        0     8194 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationNamespacePackages.py
--rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationPrintStatements.py
--rw-rw-rw-   0        0        0    15371 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationSequenceCreation.py
--rw-rw-rw-   0        0        0     4824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationSubscriptExpressions.py
--rw-rw-rw-   0        0        0    14615 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationTryExceptStatements.py
--rw-rw-rw-   0        0        0     6982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationTryFinallyStatements.py
--rw-rw-rw-   0        0        0     5674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationWhileLoopStatements.py
--rw-rw-rw-   0        0        0    14341 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationWithStatements.py
--rw-rw-rw-   0        0        0     3088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationYieldExpressions.py
--rw-rw-rw-   0        0        0     9285 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/SourceHandling.py
--rw-rw-rw-   0        0        0     3757 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/SyntaxErrors.py
--rw-rw-rw-   0        0        0    22973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/TreeHelpers.py
--rw-rw-rw-   0        0        0    20012 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/tree/VariableClosure.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/tree/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.954674 Nuitka-winsvc-1.5.6/nuitka/utils/
--rw-rw-rw-   0        0        0     2542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/AppDirs.py
--rw-rw-rw-   0        0        0     3248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/CStrings.py
--rw-rw-rw-   0        0        0     3653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/CommandLineOptions.py
--rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Distributions.py
--rw-rw-rw-   0        0        0     5794 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Download.py
--rw-rw-rw-   0        0        0    12216 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Execution.py
--rw-rw-rw-   0        0        0    30973 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.6/nuitka/utils/FileOperations.py
--rw-rw-rw-   0        0        0     2885 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Hashing.py
--rw-rw-rw-   0        0        0     2362 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Images.py
--rw-rw-rw-   0        0        0     6665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Importing.py
--rw-rw-rw-   0        0        0     7923 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/utils/InstalledPythons.py
--rw-rw-rw-   0        0        0     2224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/InstanceCounters.py
--rw-rw-rw-   0        0        0     4336 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Jinja2.py
--rw-rw-rw-   0        0        0     1216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Json.py
--rw-rw-rw-   0        0        0     4173 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/MacOSApp.py
--rw-rw-rw-   0        0        0     5040 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/nuitka/utils/MemoryUsage.py
--rw-rw-rw-   0        0        0     9057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/ModuleNames.py
--rw-rw-rw-   0        0        0     4288 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/ReExecute.py
--rw-rw-rw-   0        0        0     3815 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Rest.py
--rw-rw-rw-   0        0        0    21979 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.6/nuitka/utils/SharedLibraries.py
--rw-rw-rw-   0        0        0     3664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Shebang.py
--rw-rw-rw-   0        0        0     2507 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Signing.py
--rw-rw-rw-   0        0        0     6207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/StaticLibraries.py
--rw-rw-rw-   0        0        0     2602 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/ThreadedExecutor.py
--rw-rw-rw-   0        0        0     2772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Timing.py
--rw-rw-rw-   0        0        0    10880 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Utils.py
--rw-rw-rw-   0        0        0    10574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/WindowsFileUsage.py
--rw-rw-rw-   0        0        0    19540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/WindowsResources.py
--rw-rw-rw-   0        0        0     5979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/Yaml.py
--rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/nuitka/utils/__init__.py
--rw-rw-rw-   0        0        0      834 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 07:19:04.699796 Nuitka-winsvc-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0    15023 2023-04-13 07:15:29.000000 Nuitka-winsvc-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:02.957770 Nuitka-winsvc-1.5.6/tests/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.158835 Nuitka-winsvc-1.5.6/tests/basics/
--rw-rw-rw-   0        0        0     1766 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/AssertsTest.py
--rw-rw-rw-   0        0        0     5934 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/AssignmentsTest.py
--rw-rw-rw-   0        0        0     5866 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/AssignmentsTest32.py
--rw-rw-rw-   0        0        0     4055 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/BranchingTest.py
--rw-rw-rw-   0        0        0     1104 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/BuiltinOverload.py
--rw-rw-rw-   0        0        0     3749 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/BuiltinSuperTest.py
--rw-rw-rw-   0        0        0    17079 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/basics/BuiltinsTest.py
--rw-rw-rw-   0        0        0      866 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ClassMinimalTest.py
--rw-rw-rw-   0        0        0     4764 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ClassesTest.py
--rw-rw-rw-   0        0        0     3414 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ClassesTest32.py
--rw-rw-rw-   0        0        0     1406 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ClassesTest34.py
--rw-rw-rw-   0        0        0     4698 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ComparisonChainsTest.py
--rw-rw-rw-   0        0        0     4639 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/basics/ConstantsTest.py
--rw-rw-rw-   0        0        0      995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ConstantsTest27.py
--rw-rw-rw-   0        0        0     1628 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/DecoratorsTest.py
--rw-rw-rw-   0        0        0     2317 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/DefaultParametersTest.py
--rw-rw-rw-   0        0        0     1127 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/DoubleDeletionsTest.py
--rw-rw-rw-   0        0        0      806 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/EmptyModuleTest.py
--rw-rw-rw-   0        0        0    14391 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest.py
--rw-rw-rw-   0        0        0      961 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest32.py
--rw-rw-rw-   0        0        0     1458 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest33.py
--rw-rw-rw-   0        0        0     6745 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ExecEvalTest.py
--rw-rw-rw-   0        0        0     1417 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ExtremeClosureTest.py
--rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/FunctionObjectsTest.py
--rw-rw-rw-   0        0        0    12335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest.py
--rw-rw-rw-   0        0        0     3603 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest32.py
--rw-rw-rw-   0        0        0     2627 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest_2.py
--rw-rw-rw-   0        0        0      890 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/FutureTest32.py
--rw-rw-rw-   0        0        0     5809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/GeneratorExpressionsTest.py
--rw-rw-rw-   0        0        0     1041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/GeneratorExpressionsTest_37.py
--rw-rw-rw-   0        0        0     3824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/GlobalStatementTest.py
--rw-rw-rw-   0        0        0     1286 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/HelloWorldTest_2.py
--rw-rw-rw-   0        0        0     2469 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ImportingTest.py
--rw-rw-rw-   0        0        0     1296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/InplaceOperationsTest.py
--rw-rw-rw-   0        0        0     4227 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/basics/InspectionTest.py
--rw-rw-rw-   0        0        0     1504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/InspectionTest_35.py
--rw-rw-rw-   0        0        0     1618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/InspectionTest_36.py
--rw-rw-rw-   0        0        0     1671 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/LambdasTest.py
--rw-rw-rw-   0        0        0     2731 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/LateClosureAssignmentTest.py
--rw-rw-rw-   0        0        0     2923 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ListContractionsTest.py
--rw-rw-rw-   0        0        0     3329 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/LoopingTest.py
--rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/MainProgramsTest.py
--rw-rw-rw-   0        0        0     1925 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/basics/ModuleAttributesTest.py
--rw-rw-rw-   0        0        0     1988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/OperatorsTest.py
--rw-rw-rw-   0        0        0    14903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/OrderChecksTest.py
--rw-rw-rw-   0        0        0     1827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/OrderChecksTest27.py
--rw-rw-rw-   0        0        0     1452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/OverflowFunctionsTest_2.py
--rw-rw-rw-   0        0        0     5853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ParameterErrorsTest.py
--rw-rw-rw-   0        0        0     1899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ParameterErrorsTest32.py
--rw-rw-rw-   0        0        0      863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/PrintFutureTest.py
--rw-rw-rw-   0        0        0     1413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/PrintingTest_2.py
--rw-rw-rw-   0        0        0      878 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/RecursionTest.py
--rw-rw-rw-   0        0        0    23840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest.py
--rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest27.py
--rw-rw-rw-   0        0        0     7819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest33.py
--rw-rw-rw-   0        0        0     4902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest35.py
--rw-rw-rw-   0        0        0     5092 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest36.py
--rw-rw-rw-   0        0        0     2899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest_2.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/SlotsTest.py
--rw-rw-rw-   0        0        0     1159 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/ThreadedGeneratorsTest.py
--rw-rw-rw-   0        0        0    22965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest32.py
--rw-rw-rw-   0        0        0     1541 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest35.py
--rw-rw-rw-   0        0        0     1788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest_2.py
--rw-rw-rw-   0        0        0     2086 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryContinueFinallyTest.py
--rw-rw-rw-   0        0        0     2212 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryExceptContinueTest.py
--rw-rw-rw-   0        0        0     2275 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryExceptFinallyTest.py
--rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryExceptFramesTest.py
--rw-rw-rw-   0        0        0     2842 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryReturnFinallyTest.py
--rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/TryYieldFinallyTest.py
--rw-rw-rw-   0        0        0     1093 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/UnicodeTest.py
--rw-rw-rw-   0        0        0     1877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/UnpackingTest35.py
--rw-rw-rw-   0        0        0     2095 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/VarargsTest.py
--rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/WithStatementsTest.py
--rw-rw-rw-   0        0        0     3072 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/YieldFromTest33.py
--rw-rw-rw-   0        0        0     3821 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/basics/run_all.py
--rw-rw-rw-   0        0        0     2271 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/basics/run_xml.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.163836 Nuitka-winsvc-1.5.6/tests/onefile/
--rw-rw-rw-   0        0        0      993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/onefile/HelloWorldTest.py
--rw-rw-rw-   0        0        0     1307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/onefile/KeyboardInterruptTest.py
--rw-rw-rw-   0        0        0     5816 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/tests/onefile/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.192837 Nuitka-winsvc-1.5.6/tests/optimizations/
--rw-rw-rw-   0        0        0      958 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/optimizations/ArgumentTypes.py
--rw-rw-rw-   0        0        0     1055 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Attributes.py
--rw-rw-rw-   0        0        0     1021 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Calls.py
--rw-rw-rw-   0        0        0      921 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Conditions.py
--rw-rw-rw-   0        0        0      909 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/optimizations/DecodingOperations.py
--rw-rw-rw-   0        0        0     1212 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/FormatStrings36.py
--rw-rw-rw-   0        0        0     1150 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/HardImports.py
--rw-rw-rw-   0        0        0      974 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/HardImports_2.py
--rw-rw-rw-   0        0        0      918 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Iterations.py
--rw-rw-rw-   0        0        0     1260 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Len.py
--rw-rw-rw-   0        0        0     2262 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Operations.py
--rw-rw-rw-   0        0        0     1333 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/optimizations/Subscripts.py
--rw-rw-rw-   0        0        0     8736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/optimizations/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.193836 Nuitka-winsvc-1.5.6/tests/packages/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.195836 Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/
--rw-rw-rw-   0        0        0     2382 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.199833 Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/variable_package/
--rw-rw-rw-   0        0        0      942 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
--rw-rw-rw-   0        0        0     1168 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py
--rw-rw-rw-   0        0        0     3671 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.828030 Nuitka-winsvc-1.5.6/tests/packages/sub_package/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.207838 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/
--rw-rw-rw-   0        0        0     1230 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/__init__.py
--rw-rw-rw-   0        0        0      908 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/bigkitty.py
--rw-rw-rw-   0        0        0      910 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/smallkitty.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.214835 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/
--rw-rw-rw-   0        0        0      929 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/hello.py
--rw-rw-rw-   0        0        0      966 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/miau.py
--rw-rw-rw-   0        0        0      968 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/purr.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.829029 Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.219835 Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/some_package/
--rw-rw-rw-   0        0        0     2336 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/some_package/__init__.py
--rw-rw-rw-   0        0        0      907 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.223272 Nuitka-winsvc-1.5.6/tests/plugins/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.227270 Nuitka-winsvc-1.5.6/tests/plugins/data_files/
--rw-rw-rw-   0        0        0     1332 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/plugins/data_files/DataFilesMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.230269 Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/
--rw-rw-rw-   0        0        0      924 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/lala.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.232269 Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/sub_dir/
--rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
--rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/plugins/data_files/test_case.nuitka-package.config.yml
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.236271 Nuitka-winsvc-1.5.6/tests/plugins/parameters/
--rw-rw-rw-   0        0        0     1019 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/plugins/parameters/ParametersMain.py
--rw-rw-rw-   0        0        0     2168 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/plugins/parameters/parameter-using-plugin.py
--rw-rw-rw-   0        0        0     3532 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/plugins/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.240271 Nuitka-winsvc-1.5.6/tests/programs/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.242269 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/
--rw-rw-rw-   0        0        0      867 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/AbsoluteImportMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.248271 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/
--rw-rw-rw-   0        0        0      796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/foobar.py
--rw-rw-rw-   0        0        0      879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/local.py
--rw-rw-rw-   0        0        0      860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/util.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.249270 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/
--rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.251271 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/
--rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.253273 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.256278 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/
--rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.258268 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/some_package/
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.259269 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/
--rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:03.260272 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.353867 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/some_package/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.355868 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/
--rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.356873 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/Some_Package/
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.357868 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/
--rw-rw-rw-   0        0        0     1075 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/CasedImportingMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.358868 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/
--rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.359868 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.362873 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/
--rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/Some_Module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.364501 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/Some_Package/
--rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/Some_Package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.365496 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/
--rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/CyclicImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.368977 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/
--rw-rw-rw-   0        0        0      875 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
--rw-rw-rw-   0        0        0      875 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
--rw-rw-rw-   0        0        0      842 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.372994 Nuitka-winsvc-1.5.6/tests/programs/dash_import/
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dash_import/DashImportMain.py
--rw-rw-rw-   0        0        0      817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dash_import/dash-module.py
--rw-rw-rw-   0        0        0      817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dash_import/plus+module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.373990 Nuitka-winsvc-1.5.6/tests/programs/dash_main/
--rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dash_main/Dash-Main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.375468 Nuitka-winsvc-1.5.6/tests/programs/deep/
--rw-rw-rw-   0        0        0      898 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/DeepProgramMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.378652 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/
--rw-rw-rw-   0        0        0      980 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/DeepBrother.py
--rw-rw-rw-   0        0        0      909 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/DeepChild.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.380663 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/deep_package/
--rw-rw-rw-   0        0        0      876 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
--rw-rw-rw-   0        0        0      952 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/deep_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.381654 Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/
--rw-rw-rw-   0        0        0      794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.382653 Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/package/
--rw-rw-rw-   0        0        0      797 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/package/SubModule.py
--rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.383655 Nuitka-winsvc-1.5.6/tests/programs/import_variants/
--rw-rw-rw-   0        0        0     1005 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/import_variants/ImportVariationsMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.390659 Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/
--rw-rw-rw-   0        0        0      946 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child1.py
--rw-rw-rw-   0        0        0     1098 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child2.py
--rw-rw-rw-   0        0        0      822 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child3.py
--rw-rw-rw-   0        0        0      994 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.392654 Nuitka-winsvc-1.5.6/tests/programs/main_raises/
--rw-rw-rw-   0        0        0      911 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/main_raises/ErrorMain.py
--rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/main_raises/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.395664 Nuitka-winsvc-1.5.6/tests/programs/main_raises2/
--rw-rw-rw-   0        0        0     1080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/main_raises2/ErrorInFunctionMain.py
--rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/main_raises2/ErrorRaising.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.396654 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/
--rw-rw-rw-   0        0        0     1529 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/ModuleAttributesMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.397653 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/
--rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/Nearby1.py
--rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.399655 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/
--rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
--rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.401654 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/
--rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
--rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.404657 Nuitka-winsvc-1.5.6/tests/programs/module_exits/
--rw-rw-rw-   0        0        0      869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/module_exits/ErrorExitingModule.py
--rw-rw-rw-   0        0        0      867 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/module_exits/Main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.406880 Nuitka-winsvc-1.5.6/tests/programs/module_object_replacing/
--rw-rw-rw-   0        0        0     1078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
--rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/module_object_replacing/SelfReplacingModule.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.407981 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/
--rw-rw-rw-   0        0        0      990 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.413869 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/__init__.py
--rw-rw-rw-   0        0        0      836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/__main__.py
--rw-rw-rw-   0        0        0     1758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/entry.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.414466 Nuitka-winsvc-1.5.6/tests/programs/named_imports/
--rw-rw-rw-   0        0        0      846 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/named_imports/NamedImportsMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.416526 Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.417526 Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/sub_package/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.418525 Nuitka-winsvc-1.5.6/tests/programs/package_code/
--rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_code/PackageInitCodeMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.421885 Nuitka-winsvc-1.5.6/tests/programs/package_code/some_package/
--rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_code/some_package/SomeModule.py
--rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_code/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.424920 Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/
--rw-rw-rw-   0        0        0      789 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/PackageContainsMain.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/__init__.py
--rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/local.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.426888 Nuitka-winsvc-1.5.6/tests/programs/package_init_import/
--rw-rw-rw-   0        0        0      823 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_import/PackageInitImportMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.429892 Nuitka-winsvc-1.5.6/tests/programs/package_init_import/some_package/
--rw-rw-rw-   0        0        0     1008 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_import/some_package/PackageLocal.py
--rw-rw-rw-   0        0        0     1169 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_import/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.430882 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/
--rw-rw-rw-   0        0        0      789 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/PackageInitIssueMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.431892 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/
--rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.433897 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/child_package/
--rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
--rw-rw-rw-   0        0        0      795 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/child_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.434882 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/
--rw-rw-rw-   0        0        0      926 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/PackageMissingInitMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.435892 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/
--rw-rw-rw-   0        0        0      965 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.436881 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/sub_package/
--rw-rw-rw-   0        0        0      977 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.440227 Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/
--rw-rw-rw-   0        0        0      901 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.442234 Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/Something/
--rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/Something/__init__.py
--rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/something.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.443228 Nuitka-winsvc-1.5.6/tests/programs/package_overload/
--rw-rw-rw-   0        0        0      852 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_overload/Main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.447179 Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/__init__.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/bar.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/bar2.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.448177 Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/
--rw-rw-rw-   0        0        0     2972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.450178 Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/some_package/
--rw-rw-rw-   0        0        0     1078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/some_package/__init__.py
--rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:00.860422 Nuitka-winsvc-1.5.6/tests/programs/package_program/
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.452177 Nuitka-winsvc-1.5.6/tests/programs/package_program/PackageAsMain/
--rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_program/PackageAsMain/__init__.py
--rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/package_program/PackageAsMain/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.453189 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/
--rw-rw-rw-   0        0        0     1728 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.486276 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.492283 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.496343 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.497630 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/
--rw-rw-rw-   0        0        0     1261 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.501641 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
--rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
--rw-rw-rw-   0        0        0     1553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.502641 Nuitka-winsvc-1.5.6/tests/programs/plugin_import/
--rw-rw-rw-   0        0        0      859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/plugin_import/PluginImportMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.505644 Nuitka-winsvc-1.5.6/tests/programs/plugin_import/some_package/
--rw-rw-rw-   0        0        0      771 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/plugin_import/some_package/__init__.py
--rw-rw-rw-   0        0        0      781 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/plugin_import/some_package/some_module.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.507162 Nuitka-winsvc-1.5.6/tests/programs/reimport_main_dynamic/
--rw-rw-rw-   0        0        0      911 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.510161 Nuitka-winsvc-1.5.6/tests/programs/reimport_main_static/
--rw-rw-rw-   0        0        0      898 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.513170 Nuitka-winsvc-1.5.6/tests/programs/relative_import/
--rw-rw-rw-   0        0        0      842 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/relative_import/RelativeImportMain.py
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/relative_import/dircache.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.514160 Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/
--rw-rw-rw-   0        0        0     1169 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/ResourceReaderMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.517040 Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/some_package/
--rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/some_package/DATA_FILE.txt
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/some_package/__init__.py
--rw-rw-rw-   0        0        0     6615 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/tests/programs/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.520592 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/
--rw-rw-rw-   0        0        0     1171 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/StdlibOverloadMain.py
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/pyexpat.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.527591 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/
--rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/__init__.py
--rw-rw-rw-   0        0        0      909 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/normal_importing.py
--rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/pyexpat.py
--rw-rw-rw-   0        0        0     1236 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/star_importing.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.533624 Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/
--rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/IndentationErroring.py
--rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/SyntaxErroring.py
--rw-rw-rw-   0        0        0     1079 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/SyntaxErrorsMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.539143 Nuitka-winsvc-1.5.6/tests/programs/unicode_bom/
--rw-rw-rw-   0        0        0      963 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/unicode_bom/UnicodeBomMain.py
--rw-rw-rw-   0        0        0      846 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/unicode_bom/unicode_bom.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.542133 Nuitka-winsvc-1.5.6/tests/programs/with space/
--rw-rw-rw-   0        0        0      826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/programs/with space/Space Main.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.544894 Nuitka-winsvc-1.5.6/tests/reflected/
--rw-rw-rw-   0        0        0    14085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/reflected/compile_itself.py
--rw-rw-rw-   0        0        0     1243 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/run-tests
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.651638 Nuitka-winsvc-1.5.6/tests/standalone/
--rw-rw-rw-   0        0        0     1058 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/BrotliUsing.py
--rw-rw-rw-   0        0        0     2554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/CtypesUsing.py
--rw-rw-rw-   0        0        0     1136 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/FlaskUsing.py
--rw-rw-rw-   0        0        0      990 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/GlfwUsing.py
--rw-rw-rw-   0        0        0     1184 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/GtkUsing.py
--rw-rw-rw-   0        0        0     1025 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/HexEncodingTest_2.py
--rw-rw-rw-   0        0        0     1086 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/IdnaUsing.py
--rw-rw-rw-   0        0        0     1151 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/LxmlUsing.py
--rw-rw-rw-   0        0        0     1431 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/MatplotlibUsing.py
--rw-rw-rw-   0        0        0     2538 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/MetadataPackagesUsing.py
--rw-rw-rw-   0        0        0     1727 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/NumpyUsing.py
--rw-rw-rw-   0        0        0      947 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/OpenGLUsing.py
--rw-rw-rw-   0        0        0     1379 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PandasUsing.py
--rw-rw-rw-   0        0        0     1066 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/PasslibUsing.py
--rw-rw-rw-   0        0        0     1151 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PendulumUsing.py
--rw-rw-rw-   0        0        0     2074 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PkgResourcesRequiresUsing.py
--rw-rw-rw-   0        0        0     1067 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PmwUsing.py
--rw-rw-rw-   0        0        0     1085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/PyQt5Plugins.py
--rw-rw-rw-   0        0        0     1105 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/PyQt5SSLSupport.py
--rw-rw-rw-   0        0        0     2050 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PyQt5Using.py
--rw-rw-rw-   0        0        0     2050 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/PyQt6Using.py
--rw-rw-rw-   0        0        0     1757 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/PySide6Using.py
--rw-rw-rw-   0        0        0     1323 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/RsaUsing.py
--rw-rw-rw-   0        0        0      973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/ShlibUsing.py
--rw-rw-rw-   0        0        0     1504 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/SocketUsing.py
--rw-rw-rw-   0        0        0     1941 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/TkInterUsing.py
--rw-rw-rw-   0        0        0     3228 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/Urllib3Using.py
--rw-rw-rw-   0        0        0     1200 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/standalone/Win32ComUsing.py
--rw-rw-rw-   0        0        0     9531 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.6/tests/standalone/run_all.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.653638 Nuitka-winsvc-1.5.6/tests/standalone/zip_importer/
--rw-rw-rw-   0        0        0     1264 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/standalone/zip_importer/ZipImporterMain.py
-drwxrwxrwx   0        0        0        0 2023-04-13 07:19:04.697295 Nuitka-winsvc-1.5.6/tests/syntax/
--rw-rw-rw-   0        0        0      811 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/AsyncgenReturn36.py
--rw-rw-rw-   0        0        0      868 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/BreakWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/ClassReturn.py
--rw-rw-rw-   0        0        0      970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/ClosureDel_2.py
--rw-rw-rw-   0        0        0      849 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/ContinueWithoutLoop.py
--rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/DuplicateArgument.py
--rw-rw-rw-   0        0        0     1111 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/ExecWithNesting_2.py
--rw-rw-rw-   0        0        0      826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/FutureBraces.py
--rw-rw-rw-   0        0        0      805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/FutureUnknown.py
--rw-rw-rw-   0        0        0     1041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/GeneratorExpressions38.py
--rw-rw-rw-   0        0        0      879 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/GeneratorReturn_2.py
--rw-rw-rw-   0        0        0      792 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/GlobalForParameter.py
--rw-rw-rw-   0        0        0      995 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/Importing32.py
--rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/IndentationError.py
--rw-rw-rw-   0        0        0      915 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/LateFutureImport.py
--rw-rw-rw-   0        0        0      841 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/MisplacedFutureImport.py
--rw-rw-rw-   0        0        0      800 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/ModuleReturn.py
--rw-rw-rw-   0        0        0      883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/NonAsciiWithoutEncoding_2.py
--rw-rw-rw-   0        0        0      794 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/NonlocalForParameter32.py
--rw-rw-rw-   0        0        0      868 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/NonlocalNotFound32.py
--rw-rw-rw-   0        0        0      908 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/StarImportExtra.py
--rw-rw-rw-   0        0        0      869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/SyntaxError.py
--rw-rw-rw-   0        0        0      874 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/TryExceptAllNotLast.py
--rw-rw-rw-   0        0        0      875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/TryFinallyContinue_37.py
--rw-rw-rw-   0        0        0      776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/UnpackNoTuple.py
--rw-rw-rw-   0        0        0      809 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/UnpackTwoStars32.py
--rw-rw-rw-   0        0        0      793 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/YieldFromInModule.py
--rw-rw-rw-   0        0        0      804 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/YieldInAsync35.py
--rw-rw-rw-   0        0        0      923 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/YieldInGenexp38.py
--rw-rw-rw-   0        0        0      781 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.6/tests/syntax/YieldInModule.py
--rw-rw-rw-   0        0        0     2203 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.6/tests/syntax/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.344764 Nuitka-winsvc-1.5.7/
+-rw-rw-rw-   0        0        0   801878 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/Changelog.rst
+-rw-rw-rw-   0        0        0   152121 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/Developer_Manual.rst
+-rw-rw-rw-   0        0        0    11348 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     1751 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.574296 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/
+-rw-rw-rw-   0        0        0     4626 2023-04-26 09:52:39.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    76435 2023-04-26 09:52:40.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:52:39.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      308 2023-04-26 09:52:39.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-03-28 09:21:19.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-04-26 09:52:39.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 09:52:39.000000 Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4626 2023-04-26 09:52:44.344764 Nuitka-winsvc-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2651 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/README.md
+-rw-rw-rw-   0        0        0    73222 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.675377 Nuitka-winsvc-1.5.7/bin/
+-rw-rw-rw-   0        0        0     1135 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/autoformat-nuitka-source
+-rw-rw-rw-   0        0        0     1136 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/check-nuitka-with-pylint
+-rw-rw-rw-   0        0        0     1150 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/compare_with_cpython
+-rw-rw-rw-   0        0        0     3079 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/compare_with_xml
+-rw-rw-rw-   0        0        0     1163 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/measure-construct-performance
+-rw-rw-rw-   0        0        0     1685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/nuitka
+-rw-rw-rw-   0        0        0     1685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/bin/nuitka-run
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.244223 Nuitka-winsvc-1.5.7/doc/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.724420 Nuitka-winsvc-1.5.7/doc/Logo/
+-rw-rw-rw-   0        0        0     7321 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Horizontal.svg
+-rw-rw-rw-   0        0        0     7401 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Symbol.svg
+-rw-rw-rw-   0        0        0    17917 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Vertical.svg
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.756565 Nuitka-winsvc-1.5.7/doc/images/
+-rw-rw-rw-   0        0        0     7585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Horizontal.png
+-rw-rw-rw-   0        0        0     4452 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Symbol.png
+-rw-rw-rw-   0        0        0     9828 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Vertical.png
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.758506 Nuitka-winsvc-1.5.7/lib/
+-rw-rw-rw-   0        0        0     4250 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/lib/hints.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.799791 Nuitka-winsvc-1.5.7/misc/
+-rwxrwxrwx   0        0        0      901 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/misc/nuitka-run.bat
+-rwxrwxrwx   0        0        0     1038 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/misc/nuitka.bat
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.852164 Nuitka-winsvc-1.5.7/nuitka/
+-rw-rw-rw-   0        0        0     7236 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/Builtins.py
+-rw-rw-rw-   0        0        0     5437 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/BytecodeCaching.py
+-rw-rw-rw-   0        0        0     3440 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/Bytecodes.py
+-rw-rw-rw-   0        0        0     1884 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/CacheCleanup.py
+-rw-rw-rw-   0        0        0    11148 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/Constants.py
+-rw-rw-rw-   0        0        0     2447 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/Errors.py
+-rw-rw-rw-   0        0        0    36691 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/nuitka/MainControl.py
+-rw-rw-rw-   0        0        0     8064 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/ModuleRegistry.py
+-rw-rw-rw-   0        0        0    54557 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/OptionParsing.py
+-rw-rw-rw-   0        0        0    62842 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/Options.py
+-rw-rw-rw-   0        0        0     5022 2023-02-14 03:02:21.000000 Nuitka-winsvc-1.5.7/nuitka/OutputDirectories.py
+-rw-rw-rw-   0        0        0    14550 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/PostProcessing.py
+-rw-rw-rw-   0        0        0     5770 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/Progress.py
+-rw-rw-rw-   0        0        0     7472 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/PythonFlavors.py
+-rw-rw-rw-   0        0        0     4061 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/PythonOperators.py
+-rw-rw-rw-   0        0        0    12083 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/PythonVersions.py
+-rw-rw-rw-   0        0        0     4670 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/SourceCodeReferences.py
+-rw-rw-rw-   0        0        0    11235 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/Tracing.py
+-rw-rw-rw-   0        0        0     3395 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/TreeXML.py
+-rw-rw-rw-   0        0        0    15235 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/Variables.py
+-rw-rw-rw-   0        0        0     2055 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/Version.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/__init__.py
+-rw-rw-rw-   0        0        0     5506 2023-02-22 01:49:06.000000 Nuitka-winsvc-1.5.7/nuitka/__main__.py
+-rw-rw-rw-   0        0        0     5143 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/__past__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.881447 Nuitka-winsvc-1.5.7/nuitka/build/
+-rw-rw-rw-   0        0        0    33043 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/Backend.scons
+-rw-rw-rw-   0        0        0     8314 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/CCompilerVersion.scons
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/DataComposerInterface.py
+-rw-rw-rw-   0        0        0    18530 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/build/Onefile.scons
+-rw-rw-rw-   0        0        0    15210 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsCaching.py
+-rw-rw-rw-   0        0        0    29056 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsCompilerSettings.py
+-rw-rw-rw-   0        0        0     5527 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsHacks.py
+-rw-rw-rw-   0        0        0    15532 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsInterface.py
+-rw-rw-rw-   0        0        0     2346 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsProgress.py
+-rw-rw-rw-   0        0        0    11960 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsSpawn.py
+-rw-rw-rw-   0        0        0    24258 2023-03-14 02:12:02.000000 Nuitka-winsvc-1.5.7/nuitka/build/SconsUtils.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.246985 Nuitka-winsvc-1.5.7/nuitka/build/include/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.936200 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/
+-rw-rw-rw-   0        0        0     7769 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/allocator.h
+-rw-rw-rw-   0        0        0     3423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/builtins.h
+-rw-rw-rw-   0        0        0     4460 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/calling.h
+-rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/checkers.h
+-rw-rw-rw-   0        0        0     1261 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/checksum_tools.h
+-rw-rw-rw-   0        0        0     9571 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_asyncgen.h
+-rw-rw-rw-   0        0        0     2002 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_cell.h
+-rw-rw-rw-   0        0        0     9325 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_coroutine.h
+-rw-rw-rw-   0        0        0    16949 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_frame.h
+-rw-rw-rw-   0        0        0     5972 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_function.h
+-rw-rw-rw-   0        0        0     9136 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_generator.h
+-rw-rw-rw-   0        0        0     1838 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_method.h
+-rw-rw-rw-   0        0        0     7408 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/constants.h
+-rw-rw-rw-   0        0        0     1293 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/constants_blob.h
+-rw-rw-rw-   0        0        0    33190 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/exceptions.h
+-rw-rw-rw-   0        0        0     3221 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/filesystem_paths.h
+-rw-rw-rw-   0        0        0     6253 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/freelists.h
+-rw-rw-rw-   0        0        0    86326 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/hedley.h
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.056458 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/
+-rw-rw-rw-   0        0        0     3275 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/attributes.h
+-rw-rw-rw-   0        0        0     2663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/boolean.h
+-rw-rw-rw-   0        0        0     1181 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/bytearrays.h
+-rw-rw-rw-   0        0        0     1135 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/bytes.h
+-rw-rw-rw-   0        0        0     9335 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/calling_generated.h
+-rw-rw-rw-   0        0        0    13140 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_eq.h
+-rw-rw-rw-   0        0        0    10616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ge.h
+-rw-rw-rw-   0        0        0    10615 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_gt.h
+-rw-rw-rw-   0        0        0    13140 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_le.h
+-rw-rw-rw-   0        0        0    13139 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_lt.h
+-rw-rw-rw-   0        0        0    10616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ne.h
+-rw-rw-rw-   0        0        0     1743 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/complex.h
+-rw-rw-rw-   0        0        0    13077 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/dictionaries.h
+-rw-rw-rw-   0        0        0     1206 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/floats.h
+-rw-rw-rw-   0        0        0     3674 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/import_hard.h
+-rw-rw-rw-   0        0        0     1798 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/indexes.h
+-rw-rw-rw-   0        0        0     2941 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/ints.h
+-rw-rw-rw-   0        0        0     9992 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/iterators.h
+-rw-rw-rw-   0        0        0     3397 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/lists.h
+-rw-rw-rw-   0        0        0     1633 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/lists_generated.h
+-rw-rw-rw-   0        0        0     1328 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/mappings.h
+-rw-rw-rw-   0        0        0     4573 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations.h
+-rw-rw-rw-   0        0        0    12685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_add.h
+-rw-rw-rw-   0        0        0     5663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitand.h
+-rw-rw-rw-   0        0        0     5641 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitor.h
+-rw-rw-rw-   0        0        0     5663 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h
+-rw-rw-rw-   0        0        0     5422 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_divmod.h
+-rw-rw-rw-   0        0        0     5460 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h
+-rw-rw-rw-   0        0        0     5115 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_lshift.h
+-rw-rw-rw-   0        0        0     2799 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_matmult.h
+-rw-rw-rw-   0        0        0    15778 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mod.h
+-rw-rw-rw-   0        0        0    13210 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mult.h
+-rw-rw-rw-   0        0        0     5791 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h
+-rw-rw-rw-   0        0        0     4714 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_pow.h
+-rw-rw-rw-   0        0        0     5115 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_rshift.h
+-rw-rw-rw-   0        0        0     5824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_sub.h
+-rw-rw-rw-   0        0        0     5438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_truediv.h
+-rw-rw-rw-   0        0        0    15100 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_builtin_types.h
+-rw-rw-rw-   0        0        0     8670 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_add.h
+-rw-rw-rw-   0        0        0     3767 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h
+-rw-rw-rw-   0        0        0     3753 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h
+-rw-rw-rw-   0        0        0     3767 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h
+-rw-rw-rw-   0        0        0     4846 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h
+-rw-rw-rw-   0        0        0     3011 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h
+-rw-rw-rw-   0        0        0     2727 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h
+-rw-rw-rw-   0        0        0    10626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mod.h
+-rw-rw-rw-   0        0        0     9201 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mult.h
+-rw-rw-rw-   0        0        0     5147 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h
+-rw-rw-rw-   0        0        0     4349 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_pow.h
+-rw-rw-rw-   0        0        0     3011 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h
+-rw-rw-rw-   0        0        0     4975 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_sub.h
+-rw-rw-rw-   0        0        0     4826 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h
+-rw-rw-rw-   0        0        0     3297 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/raising.h
+-rw-rw-rw-   0        0        0     2178 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/rangeobjects.h
+-rw-rw-rw-   0        0        0     1146 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/richcomparisons.h
+-rw-rw-rw-   0        0        0     1112 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/sequences.h
+-rw-rw-rw-   0        0        0     1025 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/sets.h
+-rw-rw-rw-   0        0        0     8419 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/slices.h
+-rw-rw-rw-   0        0        0     1242 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/strings.h
+-rw-rw-rw-   0        0        0    17447 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/subscripts.h
+-rw-rw-rw-   0        0        0     5720 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/tuples.h
+-rw-rw-rw-   0        0        0    14375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helpers.h
+-rw-rw-rw-   0        0        0     5363 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/importing.h
+-rw-rw-rw-   0        0        0    12979 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/incbin.h
+-rw-rw-rw-   0        0        0    14248 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/prelude.h
+-rw-rw-rw-   0        0        0     2870 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/printing.h
+-rw-rw-rw-   0        0        0     1761 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/python_pgo.h
+-rw-rw-rw-   0        0        0     2119 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/safe_string_ops.h
+-rw-rw-rw-   0        0        0     3840 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/threading.h
+-rw-rw-rw-   0        0        0     3144 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/tracing.h
+-rw-rw-rw-   0        0        0     2830 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/unfreezing.h
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.288701 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.065249 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/appdirs/
+-rw-rw-rw-   0        0        0     1097 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/appdirs/LICENSE.txt
+-rw-rw-rw-   0        0        0    24824 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/appdirs/appdirs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.076966 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/atomicwrites/
+-rw-rw-rw-   0        0        0     1069 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/atomicwrites/LICENSE
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/atomicwrites/atomicwrites.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.078919 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/bin/
+-rw-rw-rw-   0        0        0     1331 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/bin/scons.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.251866 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.089661 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/
+-rw-rw-rw-   0        0        0     1585 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/__init__.py
+-rw-rw-rw-   0        0        0    65424 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/caching.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.102984 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/
+-rw-rw-rw-   0        0        0     1491 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.115241 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/
+-rw-rw-rw-   0        0        0      243 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/__init__.py
+-rw-rw-rw-   0        0        0     2522 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansi.py
+-rw-rw-rw-   0        0        0    10517 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py
+-rw-rw-rw-   0        0        0     1915 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/initialise.py
+-rw-rw-rw-   0        0        0     5404 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/win32.py
+-rw-rw-rw-   0        0        0     6438 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/winterm.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.130916 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/
+-rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.142154 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/
+-rw-rw-rw-   0        0        0       82 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/__init__.py
+-rw-rw-rw-   0        0        0     6859 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/compat.py
+-rw-rw-rw-   0        0        0     4463 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/fnmatch.py
+-rw-rw-rw-   0        0        0     8304 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/impl.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.162310 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/LICENSE.rst
+-rw-rw-rw-   0        0        0       85 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.214721 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/
+-rw-rw-rw-   0        0        0     2423 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17473 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.246357 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/
+-rw-rw-rw-   0        0        0     1466 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/LICENSE.rst
+-rw-rw-rw-   0        0        0       84 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.294930 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py
+-rw-rw-rw-   0        0        0     2685 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py
+-rw-rw-rw-   0        0        0     1726 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py
+-rw-rw-rw-   0        0        0    12719 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py
+-rw-rw-rw-   0        0        0    65386 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py
+-rw-rw-rw-   0        0        0     1626 2023-02-13 06:36:03.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py
+-rw-rw-rw-   0        0        0    12281 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py
+-rw-rw-rw-   0        0        0     1400 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py
+-rw-rw-rw-   0        0        0    50849 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py
+-rw-rw-rw-   0        0        0     4428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py
+-rw-rw-rw-   0        0        0    24500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py
+-rw-rw-rw-   0        0        0    36528 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py
+-rw-rw-rw-   0        0        0     9197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py
+-rw-rw-rw-   0        0        0    28559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py
+-rw-rw-rw-   0        0        0    17474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py
+-rw-rw-rw-   0        0        0     4340 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py
+-rw-rw-rw-   0        0        0     7308 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py
+-rw-rw-rw-   0        0        0    30853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py
+-rw-rw-rw-   0        0        0     1722 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py
+-rw-rw-rw-   0        0        0    35875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py
+-rw-rw-rw-   0        0        0    27644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py
+-rw-rw-rw-   0        0        0    17080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py
+-rw-rw-rw-   0        0        0     4214 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py
+-rw-rw-rw-   0        0        0    20501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py
+-rw-rw-rw-   0        0        0     3316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.274186 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.259542 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.332289 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/
+-rw-rw-rw-   0        0        0    47844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    33996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0     8083 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     6938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    17622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7358 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16000 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.341089 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/
+-rw-rw-rw-   0        0        0     4197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   121420 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     4164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    49503 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.348087 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py
+-rw-rw-rw-   0        0        0     1950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py
+-rw-rw-rw-   0        0        0     1965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py
+-rw-rw-rw-   0        0        0     2736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py
+-rw-rw-rw-   0        0        0     2614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py
+-rw-rw-rw-   0        0        0     8467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.366968 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/
+-rw-rw-rw-   0        0        0     9314 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3131 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     1989 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1718 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1605 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     2170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4179 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1882 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0    14948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    39700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    12950 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.376360 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3233 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2011 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    14663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.383191 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/
+-rw-rw-rw-   0        0        0    14029 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    52665 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    40719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    24133 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py
+-rw-rw-rw-   0        0        0    34903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    40510 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.524897 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2166 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py
+-rw-rw-rw-   0        0        0     2859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py
+-rw-rw-rw-   0        0        0    18084 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.543125 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2004 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0     9248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    14869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    19499 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    20832 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py
+-rw-rw-rw-   0        0        0     5149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py
+-rw-rw-rw-   0        0        0     2657 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py
+-rw-rw-rw-   0        0        0    31283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     2379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2267 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py
+-rw-rw-rw-   0        0        0     2720 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     2796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2147 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2936 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2935 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     2777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0      142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/dmd.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.545072 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3428 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     2681 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     2433 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py
+-rw-rw-rw-   0        0        0     1844 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     4782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py
+-rw-rw-rw-   0        0        0     2025 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py
+-rw-rw-rw-   0        0        0     2256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py
+-rw-rw-rw-   0        0        0     2460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2077 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    18600 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     3328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py
+-rw-rw-rw-   0        0        0     8394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     3953 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2309 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2945 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     6919 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4381 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2168 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    13881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1804 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    11380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    72761 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6841 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     4695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1927 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     2349 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     5992 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13016 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3415 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    48938 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.559723 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3007 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11034 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.587471 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/
+-rw-rw-rw-   0        0        0     8120 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     3596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py
+-rw-rw-rw-   0        0        0     1818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py
+-rw-rw-rw-   0        0        0     1742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     2465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py
+-rw-rw-rw-   0        0        0     1776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py
+-rw-rw-rw-   0        0        0    19253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py
+-rw-rw-rw-   0        0        0    44500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py
+-rw-rw-rw-   0        0        0    19664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     7509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.266153 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.640781 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/
+-rw-rw-rw-   0        0        0    53545 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py
+-rw-rw-rw-   0        0        0    34985 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py
+-rw-rw-rw-   0        0        0    13596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    28403 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py
+-rw-rw-rw-   0        0        0    20988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    96818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py
+-rw-rw-rw-   0        0        0     7752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py
+-rw-rw-rw-   0        0        0    22350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16068 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py
+-rw-rw-rw-   0        0        0     9565 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.646630 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/
+-rw-rw-rw-   0        0        0     5239 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   135413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     5758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8354 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.672024 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/
+-rw-rw-rw-   0        0        0    11500 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2227 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1767 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1654 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1460 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4476 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     4003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    16962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41186 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py
+-rw-rw-rw-   0        0        0    13880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.680809 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/
+-rw-rw-rw-   0        0        0     4853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     3812 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15053 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.691551 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/
+-rw-rw-rw-   0        0        0    13779 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53260 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    39394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14489 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    35863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py
+-rw-rw-rw-   0        0        0    42204 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.831910 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/
+-rw-rw-rw-   0        0        0     2211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    18207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.843614 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2152 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     2057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    10674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    33537 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    21762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    50660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1667 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2316 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     8618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2226 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     2978 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3389 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.845106 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      313 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3631 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3444 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     8494 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.846083 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/
+-rw-rw-rw-   0        0        0    29765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py
+-rw-rw-rw-   0        0        0     3472 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1977 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3686 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2580 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1645 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2765 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2189 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1944 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     2123 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     2085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    15791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    26195 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0    13924 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py
+-rw-rw-rw-   0        0        0     4041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2351 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2987 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     7808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4956 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     5235 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14751 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1847 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    82939 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2660 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4904 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1868 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     5335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6756 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3773 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    13982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     3201 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    53803 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.855606 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/
+-rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4459 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3643 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5579 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    11655 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py
+-rw-rw-rw-   0        0        0     1647 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.857799 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/
+-rw-rw-rw-   0        0        0     6869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0    19816 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2149 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.275154 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.891528 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/
+-rw-rw-rw-   0        0        0    56578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py
+-rw-rw-rw-   0        0        0    35213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py
+-rw-rw-rw-   0        0        0    11061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py
+-rw-rw-rw-   0        0        0    27408 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py
+-rw-rw-rw-   0        0        0     7884 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py
+-rw-rw-rw-   0        0        0    21423 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py
+-rw-rw-rw-   0        0        0    97269 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py
+-rw-rw-rw-   0        0        0     3979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py
+-rw-rw-rw-   0        0        0     7515 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py
+-rw-rw-rw-   0        0        0    21937 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py
+-rw-rw-rw-   0        0        0    16583 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py
+-rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.895424 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/
+-rw-rw-rw-   0        0        0     5126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py
+-rw-rw-rw-   0        0        0   136271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py
+-rw-rw-rw-   0        0        0     6167 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py
+-rw-rw-rw-   0        0        0    63768 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py
+-rw-rw-rw-   0        0        0     8183 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.913001 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/
+-rw-rw-rw-   0        0        0    12836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py
+-rw-rw-rw-   0        0        0     3087 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py
+-rw-rw-rw-   0        0        0     2107 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py
+-rw-rw-rw-   0        0        0     2630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py
+-rw-rw-rw-   0        0        0     1674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py
+-rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py
+-rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py
+-rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py
+-rw-rw-rw-   0        0        0     4356 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py
+-rw-rw-rw-   0        0        0     1805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py
+-rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py
+-rw-rw-rw-   0        0        0    14831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py
+-rw-rw-rw-   0        0        0    41983 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py
+-rw-rw-rw-   0        0        0    14673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.922767 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/
+-rw-rw-rw-   0        0        0     7394 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py
+-rw-rw-rw-   0        0        0     4357 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py
+-rw-rw-rw-   0        0        0     3546 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py
+-rw-rw-rw-   0        0        0     1972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py
+-rw-rw-rw-   0        0        0    15577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:41.929602 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/
+-rw-rw-rw-   0        0        0    13597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py
+-rw-rw-rw-   0        0        0    53509 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py
+-rw-rw-rw-   0        0        0    42760 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py
+-rw-rw-rw-   0        0        0    26676 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py
+-rw-rw-rw-   0        0        0    14272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py
+-rw-rw-rw-   0        0        0    36753 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py
+-rw-rw-rw-   0        0        0    41191 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.046211 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/
+-rw-rw-rw-   0        0        0     2122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py
+-rw-rw-rw-   0        0        0    15570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.059473 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/
+-rw-rw-rw-   0        0        0     2014 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py
+-rw-rw-rw-   0        0        0     1943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py
+-rw-rw-rw-   0        0        0    13182 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py
+-rw-rw-rw-   0        0        0     2734 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py
+-rw-rw-rw-   0        0        0    15027 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py
+-rw-rw-rw-   0        0        0    38783 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py
+-rw-rw-rw-   0        0        0    22570 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py
+-rw-rw-rw-   0        0        0     4368 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py
+-rw-rw-rw-   0        0        0    32724 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py
+-rw-rw-rw-   0        0        0     2228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py
+-rw-rw-rw-   0        0        0     2386 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py
+-rw-rw-rw-   0        0        0     2616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py
+-rw-rw-rw-   0        0        0     7993 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py
+-rw-rw-rw-   0        0        0     2141 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py
+-rw-rw-rw-   0        0        0     1661 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py
+-rw-rw-rw-   0        0        0     2893 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py
+-rw-rw-rw-   0        0        0     2889 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py
+-rw-rw-rw-   0        0        0     1567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py
+-rw-rw-rw-   0        0        0     3742 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py
+-rw-rw-rw-   0        0        0     3296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.060448 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/
+-rw-rw-rw-   0        0        0      343 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangCommon/__init__.py
+-rw-rw-rw-   0        0        0     3534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py
+-rw-rw-rw-   0        0        0     3259 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py
+-rw-rw-rw-   0        0        0     7461 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py
+-rw-rw-rw-   0        0        0     1663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py
+-rw-rw-rw-   0        0        0     3379 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py
+-rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py
+-rw-rw-rw-   0        0        0     1891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py
+-rw-rw-rw-   0        0        0     3616 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py
+-rw-rw-rw-   0        0        0     2377 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py
+-rw-rw-rw-   0        0        0     2437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py
+-rw-rw-rw-   0        0        0     2526 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py
+-rw-rw-rw-   0        0        0     1557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py
+-rw-rw-rw-   0        0        0     1772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py
+-rw-rw-rw-   0        0        0     2677 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py
+-rw-rw-rw-   0        0        0     2206 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py
+-rw-rw-rw-   0        0        0     2096 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py
+-rw-rw-rw-   0        0        0     1851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py
+-rw-rw-rw-   0        0        0     1954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py
+-rw-rw-rw-   0        0        0     1995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py
+-rw-rw-rw-   0        0        0    19180 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py
+-rw-rw-rw-   0        0        0    25826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py
+-rw-rw-rw-   0        0        0     2588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.064354 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/
+-rw-rw-rw-   0        0        0     4649 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py
+-rw-rw-rw-   0        0        0     7652 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py
+-rw-rw-rw-   0        0        0     6064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py
+-rw-rw-rw-   0        0        0     3931 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py
+-rw-rw-rw-   0        0        0     2266 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py
+-rw-rw-rw-   0        0        0     2900 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py
+-rw-rw-rw-   0        0        0     8622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py
+-rw-rw-rw-   0        0        0     4577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py
+-rw-rw-rw-   0        0        0     4517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py
+-rw-rw-rw-   0        0        0     4113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py
+-rw-rw-rw-   0        0        0     2387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py
+-rw-rw-rw-   0        0        0    14473 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py
+-rw-rw-rw-   0        0        0     1752 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py
+-rw-rw-rw-   0        0        0    12902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py
+-rw-rw-rw-   0        0        0    84784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py
+-rw-rw-rw-   0        0        0     6788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py
+-rw-rw-rw-   0        0        0     3576 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py
+-rw-rw-rw-   0        0        0     4817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py
+-rw-rw-rw-   0        0        0     2788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py
+-rw-rw-rw-   0        0        0     2479 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py
+-rw-rw-rw-   0        0        0     1563 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py
+-rw-rw-rw-   0        0        0     1780 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py
+-rw-rw-rw-   0        0        0     1999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py
+-rw-rw-rw-   0        0        0     2006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py
+-rw-rw-rw-   0        0        0     2271 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py
+-rw-rw-rw-   0        0        0     1569 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py
+-rw-rw-rw-   0        0        0     1888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py
+-rw-rw-rw-   0        0        0     2419 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py
+-rw-rw-rw-   0        0        0     2429 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py
+-rw-rw-rw-   0        0        0     6412 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py
+-rw-rw-rw-   0        0        0     1786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py
+-rw-rw-rw-   0        0        0    12548 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py
+-rw-rw-rw-   0        0        0     4076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py
+-rw-rw-rw-   0        0        0    71693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.072163 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/
+-rw-rw-rw-   0        0        0     6632 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/__init__.py
+-rw-rw-rw-   0        0        0    15278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.080954 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/
+-rw-rw-rw-   0        0        0     3134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py
+-rw-rw-rw-   0        0        0     3896 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py
+-rw-rw-rw-   0        0        0     4672 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py
+-rw-rw-rw-   0        0        0     3536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py
+-rw-rw-rw-   0        0        0     5588 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py
+-rw-rw-rw-   0        0        0    12708 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py
+-rw-rw-rw-   0        0        0     6785 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py
+-rw-rw-rw-   0        0        0      353 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.088767 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/
+-rw-rw-rw-   0        0        0     4307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py
+-rw-rw-rw-   0        0        0     1644 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py
+-rw-rw-rw-   0        0        0     3395 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py
+-rw-rw-rw-   0        0        0    21614 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py
+-rw-rw-rw-   0        0        0     9295 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py
+-rw-rw-rw-   0        0        0     2032 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.109846 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/
+-rw-rw-rw-   0        0        0     1467 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/LICENSE.rst
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.113752 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/
+-rw-rw-rw-   0        0        0    10126 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py
+-rw-rw-rw-   0        0        0     4690 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py
+-rw-rw-rw-   0        0        0     1873 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.282675 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.117215 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/
+-rw-rw-rw-   0        0        0   107452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py
+-rw-rw-rw-   0        0        0      538 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.284161 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.143198 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/
+-rw-rw-rw-   0        0        0     1591 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/__init__.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_main.py
+-rw-rw-rw-   0        0        0     3687 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py
+-rw-rw-rw-   0        0        0      283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm.py
+-rw-rw-rw-   0        0        0      287 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_gui.py
+-rw-rw-rw-   0        0        0      307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_notebook.py
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py
+-rw-rw-rw-   0        0        0      596 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_utils.py
+-rw-rw-rw-   0        0        0     1106 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/auto.py
+-rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py
+-rw-rw-rw-   0        0        0     1376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/dask.py
+-rw-rw-rw-   0        0        0     5943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/gui.py
+-rw-rw-rw-   0        0        0    10790 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/notebook.py
+-rw-rw-rw-   0        0        0    57572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/std.py
+-rw-rw-rw-   0        0        0     6948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/tk.py
+-rw-rw-rw-   0        0        0     9533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/utils.py
+-rw-rw-rw-   0        0        0      333 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/version.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.159806 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.187107 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/
+-rw-rw-rw-   0        0        0    13170 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/composer.py
+-rw-rw-rw-   0        0        0    28639 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3851 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2837 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43006 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/events.py
+-rw-rw-rw-   0        0        0     2061 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/parser.py
+-rw-rw-rw-   0        0        0     6794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/reader.py
+-rw-rw-rw-   0        0        0    14184 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/representer.py
+-rw-rw-rw-   0        0        0     8999 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51277 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.194453 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.224456 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/
+-rw-rw-rw-   0        0        0     9776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4921 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/composer.py
+-rw-rw-rw-   0        0        0    25145 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2719 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/dumper.py
+-rw-rw-rw-   0        0        0    43298 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2559 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/events.py
+-rw-rw-rw-   0        0        0     1132 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25542 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/parser.py
+-rw-rw-rw-   0        0        0     6746 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/reader.py
+-rw-rw-rw-   0        0        0    17711 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/representer.py
+-rw-rw-rw-   0        0        0     9122 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/resolver.py
+-rw-rw-rw-   0        0        0    52446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4171 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.528116 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/
+-rw-rw-rw-   0        0        0     1101 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/LICENSE
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.556557 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/
+-rw-rw-rw-   0        0        0     9607 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/__init__.py
+-rw-rw-rw-   0        0        0     4881 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/composer.py
+-rw-rw-rw-   0        0        0    25554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/constructor.py
+-rw-rw-rw-   0        0        0     3294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py
+-rw-rw-rw-   0        0        0     2723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/dumper.py
+-rw-rw-rw-   0        0        0    42954 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/emitter.py
+-rw-rw-rw-   0        0        0     2533 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/error.py
+-rw-rw-rw-   0        0        0     2445 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/events.py
+-rw-rw-rw-   0        0        0     1138 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/loader.py
+-rw-rw-rw-   0        0        0     1440 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/nodes.py
+-rw-rw-rw-   0        0        0    25495 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/parser.py
+-rw-rw-rw-   0        0        0     6854 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/reader.py
+-rw-rw-rw-   0        0        0    14097 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/representer.py
+-rw-rw-rw-   0        0        0     8970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/resolver.py
+-rw-rw-rw-   0        0        0    51695 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/scanner.py
+-rw-rw-rw-   0        0        0     4165 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/serializer.py
+-rw-rw-rw-   0        0        0     2573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/tokens.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.568969 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/
+-rw-rw-rw-   0        0        0     1530 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.604292 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/
+-rw-rw-rw-   0        0        0    18198 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/bitstream.h
+-rw-rw-rw-   0        0        0    10157 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/compiler.h
+-rw-rw-rw-   0        0        0     4455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/cpu.h
+-rw-rw-rw-   0        0        0     3763 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/debug.h
+-rw-rw-rw-   0        0        0    13662 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/entropy_common.c
+-rw-rw-rw-   0        0        0     3009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.c
+-rw-rw-rw-   0        0        0     2441 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.h
+-rw-rw-rw-   0        0        0    34422 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/fse.h
+-rw-rw-rw-   0        0        0    14748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/fse_decompress.c
+-rw-rw-rw-   0        0        0    20216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/huf.h
+-rw-rw-rw-   0        0        0    13930 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/mem.h
+-rw-rw-rw-   0        0        0    26976 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.c
+-rw-rw-rw-   0        0        0    11706 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.h
+-rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_common.c
+-rw-rw-rw-   0        0        0     2497 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_deps.h
+-rw-rw-rw-   0        0        0     3828 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_errors.h
+-rw-rw-rw-   0        0        0    15880 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_internal.h
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.614351 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/
+-rw-rw-rw-   0        0        0    54982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c
+-rw-rw-rw-   0        0        0     9164 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c
+-rw-rw-rw-   0        0        0     1321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h
+-rw-rw-rw-   0        0        0    80283 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c
+-rw-rw-rw-   0        0        0    66784 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c
+-rw-rw-rw-   0        0        0     2253 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h
+-rw-rw-rw-   0        0        0     7906 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h
+-rw-rw-rw-   0        0        0   138334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/zstd.h
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.750195 Nuitka-winsvc-1.5.7/nuitka/build/static_src/
+-rw-rw-rw-   0        0        0    82114 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledAsyncgenType.c
+-rw-rw-rw-   0        0        0     8250 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCellType.c
+-rw-rw-rw-   0        0        0    57572 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCodeHelpers.c
+-rw-rw-rw-   0        0        0    70973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCoroutineType.c
+-rw-rw-rw-   0        0        0    35865 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledFrameType.c
+-rw-rw-rw-   0        0        0    93999 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledFunctionType.c
+-rw-rw-rw-   0        0        0    60657 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledGeneratorType.c
+-rw-rw-rw-   0        0        0    26221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c
+-rw-rw-rw-   0        0        0    21493 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledMethodType.c
+-rw-rw-rw-   0        0        0    18993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersAllocator.c
+-rw-rw-rw-   0        0        0    32656 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersAttributes.c
+-rw-rw-rw-   0        0        0    21783 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBuiltin.c
+-rw-rw-rw-   0        0        0   107641 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBuiltinTypeMethods.c
+-rw-rw-rw-   0        0        0     3033 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBytes.c
+-rw-rw-rw-   0        0        0    13057 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersCalling.c
+-rw-rw-rw-   0        0        0   460993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersCallingGenerated.c
+-rw-rw-rw-   0        0        0     1617 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersChecksumTools.c
+-rw-rw-rw-   0        0        0     2991 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersClasses.c
+-rw-rw-rw-   0        0        0   317872 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonEq.c
+-rw-rw-rw-   0        0        0     4673 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonEqUtils.c
+-rw-rw-rw-   0        0        0   313003 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonGe.c
+-rw-rw-rw-   0        0        0   312414 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonGt.c
+-rw-rw-rw-   0        0        0   316217 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonLe.c
+-rw-rw-rw-   0        0        0   315628 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonLt.c
+-rw-rw-rw-   0        0        0   314618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonNe.c
+-rw-rw-rw-   0        0        0    36011 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersConstantsBlob.c
+-rw-rw-rw-   0        0        0    19313 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDeepcopy.c
+-rw-rw-rw-   0        0        0    38320 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDictionaries.c
+-rw-rw-rw-   0        0        0    24294 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDictionariesGenerated.c
+-rw-rw-rw-   0        0        0     7035 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersExceptions.c
+-rw-rw-rw-   0        0        0     6411 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFiles.c
+-rw-rw-rw-   0        0        0    11199 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFilesystemPaths.c
+-rw-rw-rw-   0        0        0     2426 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFloats.c
+-rw-rw-rw-   0        0        0     1774 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersHeapStorage.c
+-rw-rw-rw-   0        0        0    14561 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersImport.c
+-rw-rw-rw-   0        0        0    13589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersImportHard.c
+-rw-rw-rw-   0        0        0    18391 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersLists.c
+-rw-rw-rw-   0        0        0    13915 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersListsGenerated.c
+-rw-rw-rw-   0        0        0     1640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersMappings.c
+-rw-rw-rw-   0        0        0     3513 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersMatching.c
+-rw-rw-rw-   0        0        0   181243 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAdd.c
+-rw-rw-rw-   0        0        0    16700 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c
+-rw-rw-rw-   0        0        0    77943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitand.c
+-rw-rw-rw-   0        0        0    77782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitor.c
+-rw-rw-rw-   0        0        0    77943 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitxor.c
+-rw-rw-rw-   0        0        0    67487 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmod.c
+-rw-rw-rw-   0        0        0     1236 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c
+-rw-rw-rw-   0        0        0    68748 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c
+-rw-rw-rw-   0        0        0     6274 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c
+-rw-rw-rw-   0        0        0    83405 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryLshift.c
+-rw-rw-rw-   0        0        0    13776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMatmult.c
+-rw-rw-rw-   0        0        0   183202 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMod.c
+-rw-rw-rw-   0        0        0   188514 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMult.c
+-rw-rw-rw-   0        0        0     3404 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c
+-rw-rw-rw-   0        0        0    66453 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c
+-rw-rw-rw-   0        0        0    78891 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPow.c
+-rw-rw-rw-   0        0        0     1023 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c
+-rw-rw-rw-   0        0        0    77305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryRshift.c
+-rw-rw-rw-   0        0        0    70465 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinarySub.c
+-rw-rw-rw-   0        0        0    68005 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryTruediv.c
+-rw-rw-rw-   0        0        0   149580 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAdd.c
+-rw-rw-rw-   0        0        0     4071 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c
+-rw-rw-rw-   0        0        0    53224 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitand.c
+-rw-rw-rw-   0        0        0    53122 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitor.c
+-rw-rw-rw-   0        0        0    53224 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitxor.c
+-rw-rw-rw-   0        0        0    76512 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c
+-rw-rw-rw-   0        0        0    47568 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceLshift.c
+-rw-rw-rw-   0        0        0    17742 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMatmult.c
+-rw-rw-rw-   0        0        0   136100 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMod.c
+-rw-rw-rw-   0        0        0   142211 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMult.c
+-rw-rw-rw-   0        0        0    74142 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c
+-rw-rw-rw-   0        0        0    82669 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplacePow.c
+-rw-rw-rw-   0        0        0    45052 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceRshift.c
+-rw-rw-rw-   0        0        0    82842 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceSub.c
+-rw-rw-rw-   0        0        0    76343 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceTruediv.c
+-rw-rw-rw-   0        0        0     3219 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersProfiling.c
+-rw-rw-rw-   0        0        0     3805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersPythonPgo.c
+-rw-rw-rw-   0        0        0    15369 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersRaising.c
+-rw-rw-rw-   0        0        0    11094 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSafeStrings.c
+-rw-rw-rw-   0        0        0     3730 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSequences.c
+-rw-rw-rw-   0        0        0     1946 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSlices.c
+-rw-rw-rw-   0        0        0    26642 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersStrings.c
+-rw-rw-rw-   0        0        0     4037 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersTuples.c
+-rw-rw-rw-   0        0        0     5578 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersTypes.c
+-rw-rw-rw-   0        0        0    11945 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/InspectPatcher.c
+-rw-rw-rw-   0        0        0    40884 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/MainProgram.c
+-rw-rw-rw-   0        0        0    58321 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoader.c
+-rw-rw-rw-   0        0        0     3650 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c
+-rw-rw-rw-   0        0        0     6427 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c
+-rw-rw-rw-   0        0        0    17065 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c
+-rw-rw-rw-   0        0        0    35924 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/OnefileBootstrap.c
+-rw-rw-rw-   0        0        0     7891 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/build/static_src/OnefileSplashScreen.cpp
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.841095 Nuitka-winsvc-1.5.7/nuitka/code_generation/
+-rw-rw-rw-   0        0        0     6346 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/AsyncgenCodes.py
+-rw-rw-rw-   0        0        0    10153 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/AttributeCodes.py
+-rw-rw-rw-   0        0        0    21864 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/BinaryOperationHelperDefinitions.py
+-rw-rw-rw-   0        0        0     2339 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/BranchCodes.py
+-rw-rw-rw-   0        0        0    16009 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/BuiltinCodes.py
+-rw-rw-rw-   0        0        0    35905 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CallCodes.py
+-rw-rw-rw-   0        0        0     4896 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ClassCodes.py
+-rw-rw-rw-   0        0        0    51024 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeGeneration.py
+-rw-rw-rw-   0        0        0     2375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeHelperSelection.py
+-rw-rw-rw-   0        0        0    14392 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeHelpers.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeObjectCodes.py
+-rw-rw-rw-   0        0        0    16827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ComparisonCodes.py
+-rw-rw-rw-   0        0        0     4446 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ComparisonHelperDefinitions.py
+-rw-rw-rw-   0        0        0     7335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ConditionalCodes.py
+-rw-rw-rw-   0        0        0     5879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ConstantCodes.py
+-rw-rw-rw-   0        0        0    31196 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/Contexts.py
+-rw-rw-rw-   0        0        0     8416 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CoroutineCodes.py
+-rw-rw-rw-   0        0        0     1574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/CtypesCodes.py
+-rw-rw-rw-   0        0        0    28478 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/DictCodes.py
+-rw-rw-rw-   0        0        0     2125 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/Emission.py
+-rw-rw-rw-   0        0        0     9325 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ErrorCodes.py
+-rw-rw-rw-   0        0        0    12304 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/EvalCodes.py
+-rw-rw-rw-   0        0        0     8975 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ExceptionCodes.py
+-rw-rw-rw-   0        0        0     7350 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py
+-rw-rw-rw-   0        0        0     2093 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ExpressionCodes.py
+-rw-rw-rw-   0        0        0    17725 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/FrameCodes.py
+-rw-rw-rw-   0        0        0    27345 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/FunctionCodes.py
+-rw-rw-rw-   0        0        0     7622 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/GeneratorCodes.py
+-rw-rw-rw-   0        0        0     5721 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/GlobalConstants.py
+-rw-rw-rw-   0        0        0     6911 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/GlobalsLocalsCodes.py
+-rw-rw-rw-   0        0        0     1794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/IdCodes.py
+-rw-rw-rw-   0        0        0    13294 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ImportCodes.py
+-rw-rw-rw-   0        0        0     1396 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/Indentation.py
+-rw-rw-rw-   0        0        0     1506 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/IndexCodes.py
+-rw-rw-rw-   0        0        0     1033 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/InjectCCodes.py
+-rw-rw-rw-   0        0        0     3432 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/IntegerCodes.py
+-rw-rw-rw-   0        0        0    12010 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/IteratorCodes.py
+-rw-rw-rw-   0        0        0     2022 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/LabelCodes.py
+-rw-rw-rw-   0        0        0     2612 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/LineNumberCodes.py
+-rw-rw-rw-   0        0        0    15892 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ListCodes.py
+-rw-rw-rw-   0        0        0     6375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/LoaderCodes.py
+-rw-rw-rw-   0        0        0     9951 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/LocalsDictCodes.py
+-rw-rw-rw-   0        0        0     3135 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/LoopCodes.py
+-rw-rw-rw-   0        0        0     1597 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/MatchCodes.py
+-rw-rw-rw-   0        0        0     6291 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ModuleCodes.py
+-rw-rw-rw-   0        0        0     8118 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/Namify.py
+-rw-rw-rw-   0        0        0    12777 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/OperationCodes.py
+-rw-rw-rw-   0        0        0    28479 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/PackageResourceCodes.py
+-rw-rw-rw-   0        0        0     3021 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/PrintCodes.py
+-rw-rw-rw-   0        0        0     5474 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/PythonAPICodes.py
+-rw-rw-rw-   0        0        0    13095 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/RaisingCodes.py
+-rw-rw-rw-   0        0        0     3443 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/Reports.py
+-rw-rw-rw-   0        0        0     5234 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/ReturnCodes.py
+-rw-rw-rw-   0        0        0     6517 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/SetCodes.py
+-rw-rw-rw-   0        0        0    13949 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/SliceCodes.py
+-rw-rw-rw-   0        0        0     9809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/StringCodes.py
+-rw-rw-rw-   0        0        0     8188 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/SubscriptCodes.py
+-rw-rw-rw-   0        0        0    11176 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/TryCodes.py
+-rw-rw-rw-   0        0        0     3786 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/TupleCodes.py
+-rw-rw-rw-   0        0        0    14717 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/VariableCodes.py
+-rw-rw-rw-   0        0        0     9121 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/VariableDeclarations.py
+-rw-rw-rw-   0        0        0     8099 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/YieldCodes.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.860423 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/
+-rw-rw-rw-   0        0        0     6069 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeBases.py
+-rw-rw-rw-   0        0        0     3399 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeBooleans.py
+-rw-rw-rw-   0        0        0     1804 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeCFloats.py
+-rw-rw-rw-   0        0        0     1378 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeCLongs.py
+-rw-rw-rw-   0        0        0     3610 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeModuleDictVariables.py
+-rw-rw-rw-   0        0        0     5128 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py
+-rw-rw-rw-   0        0        0     5211 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaInts.py
+-rw-rw-rw-   0        0        0     3955 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaVoids.py
+-rw-rw-rw-   0        0        0    19628 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypePyObjectPointers.py
+-rw-rw-rw-   0        0        0     2852 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeVoids.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:42.893654 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/
+-rw-rw-rw-   0        0        0     2728 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py
+-rw-rw-rw-   0        0        0     5747 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesConstants.py
+-rw-rw-rw-   0        0        0     2805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesCoroutines.py
+-rw-rw-rw-   0        0        0     2290 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesExceptions.py
+-rw-rw-rw-   0        0        0     6339 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesFrames.py
+-rw-rw-rw-   0        0        0     3321 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesFunction.py
+-rw-rw-rw-   0        0        0     3190 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py
+-rw-rw-rw-   0        0        0     2335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesIterators.py
+-rw-rw-rw-   0        0        0     4217 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesLoader.py
+-rw-rw-rw-   0        0        0    21441 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesModules.py
+-rw-rw-rw-   0        0        0     6640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesVariables.py
+-rw-rw-rw-   0        0        0     2475 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/TemplateDebugWrapper.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.323068 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/
+-rw-rw-rw-   0        0        0    11231 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2
+-rw-rw-rw-   0        0        0     5904 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2
+-rw-rw-rw-   0        0        0    23262 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2
+-rw-rw-rw-   0        0        0     5238 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2
+-rw-rw-rw-   0        0        0     1905 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2
+-rw-rw-rw-   0        0        0     1843 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2
+-rw-rw-rw-   0        0        0     2817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2
+-rw-rw-rw-   0        0        0    12818 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2
+-rw-rw-rw-   0        0        0     2044 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperImportHard.c.j2
+-rw-rw-rw-   0        0        0     2762 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperLongTools.c.j2
+-rw-rw-rw-   0        0        0     1544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperObjectTools.c.j2
+-rw-rw-rw-   0        0        0     7197 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2
+-rw-rw-rw-   0        0        0    12850 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2
+-rw-rw-rw-   0        0        0     4288 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2
+-rw-rw-rw-   0        0        0     2088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2
+-rw-rw-rw-   0        0        0     2118 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2
+-rw-rw-rw-   0        0        0     3933 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2
+-rw-rw-rw-   0        0        0     7407 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2
+-rw-rw-rw-   0        0        0     4292 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2
+-rw-rw-rw-   0        0        0     3860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2
+-rw-rw-rw-   0        0        0     4487 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2
+-rw-rw-rw-   0        0        0    11579 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2
+-rw-rw-rw-   0        0        0    19317 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2
+-rw-rw-rw-   0        0        0     2843 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2
+-rw-rw-rw-   0        0        0     3635 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2
+-rw-rw-rw-   0        0        0    11102 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2
+-rw-rw-rw-   0        0        0    15380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2
+-rw-rw-rw-   0        0        0     2979 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsList.c.j2
+-rw-rw-rw-   0        0        0    10421 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2
+-rw-rw-rw-   0        0        0     2557 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2
+-rw-rw-rw-   0        0        0     3020 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2
+-rw-rw-rw-   0        0        0     2984 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2
+-rw-rw-rw-   0        0        0     3173 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.325997 Nuitka-winsvc-1.5.7/nuitka/constants/
+-rw-rw-rw-   0        0        0     8524 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/constants/Serialization.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/constants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.330879 Nuitka-winsvc-1.5.7/nuitka/containers/
+-rw-rw-rw-   0        0        0     1435 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/containers/Namedtuples.py
+-rw-rw-rw-   0        0        0     6553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/containers/OrderedDicts.py
+-rw-rw-rw-   0        0        0      554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/containers/OrderedSets.py
+-rw-rw-rw-   0        0        0     4397 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/containers/OrderedSetsFallback.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/containers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.334786 Nuitka-winsvc-1.5.7/nuitka/distutils/
+-rw-rw-rw-   0        0        0     1964 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/distutils/Build.py
+-rw-rw-rw-   0        0        0    14107 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/distutils/DistutilCommands.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/distutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.338692 Nuitka-winsvc-1.5.7/nuitka/finalizations/
+-rw-rw-rw-   0        0        0     1224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/finalizations/Finalization.py
+-rw-rw-rw-   0        0        0     6110 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/finalizations/FinalizeMarkups.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/finalizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.363108 Nuitka-winsvc-1.5.7/nuitka/freezer/
+-rw-rw-rw-   0        0        0     7311 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/DependsExe.py
+-rw-rw-rw-   0        0        0     2380 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesCommon.py
+-rw-rw-rw-   0        0        0    10109 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesMacOS.py
+-rw-rw-rw-   0        0        0     7211 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesPosix.py
+-rw-rw-rw-   0        0        0     6620 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesWin32.py
+-rw-rw-rw-   0        0        0    16587 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/IncludedDataFiles.py
+-rw-rw-rw-   0        0        0     9146 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/IncludedEntryPoints.py
+-rw-rw-rw-   0        0        0     9795 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/Onefile.py
+-rw-rw-rw-   0        0        0    25368 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/Standalone.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/freezer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.381660 Nuitka-winsvc-1.5.7/nuitka/importing/
+-rw-rw-rw-   0        0        0    10934 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/IgnoreListing.py
+-rw-rw-rw-   0        0        0     2899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/ImportCache.py
+-rw-rw-rw-   0        0        0     6455 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/ImportResolving.py
+-rw-rw-rw-   0        0        0    28248 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/importing/Importing.py
+-rw-rw-rw-   0        0        0     4739 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/PreloadedPackages.py
+-rw-rw-rw-   0        0        0    16375 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/importing/Recursion.py
+-rw-rw-rw-   0        0        0    10383 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/StandardLibrary.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/importing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.517007 Nuitka-winsvc-1.5.7/nuitka/nodes/
+-rw-rw-rw-   0        0        0     3637 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/AsyncgenNodes.py
+-rw-rw-rw-   0        0        0     4082 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeLookupNodes.py
+-rw-rw-rw-   0        0        0    12004 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeNodes.py
+-rw-rw-rw-   0        0        0   378745 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeNodesGenerated.py
+-rw-rw-rw-   0        0        0     3823 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinAllNodes.py
+-rw-rw-rw-   0        0        0     4098 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinAnyNodes.py
+-rw-rw-rw-   0        0        0     2496 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinComplexNodes.py
+-rw-rw-rw-   0        0        0     1698 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDecodingNodes.py
+-rw-rw-rw-   0        0        0     2727 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDecoratorNodes.py
+-rw-rw-rw-   0        0        0     4694 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDictNodes.py
+-rw-rw-rw-   0        0        0     4948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinFormatNodes.py
+-rw-rw-rw-   0        0        0     2142 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinHashNodes.py
+-rw-rw-rw-   0        0        0     5334 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinIntegerNodes.py
+-rw-rw-rw-   0        0        0    12723 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinIteratorNodes.py
+-rw-rw-rw-   0        0        0     1996 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinLenNodes.py
+-rw-rw-rw-   0        0        0     3606 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinNextNodes.py
+-rw-rw-rw-   0        0        0     3240 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinOpenNodes.py
+-rw-rw-rw-   0        0        0   245536 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py
+-rw-rw-rw-   0        0        0    18589 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinRangeNodes.py
+-rw-rw-rw-   0        0        0     9067 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinRefNodes.py
+-rw-rw-rw-   0        0        0     3307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinSumNodes.py
+-rw-rw-rw-   0        0        0    13543 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinTypeNodes.py
+-rw-rw-rw-   0        0        0     1573 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinVarsNodes.py
+-rw-rw-rw-   0        0        0    26113 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/BytesNodes.py
+-rw-rw-rw-   0        0        0     6478 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/CallNodes.py
+-rw-rw-rw-   0        0        0     1550 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/Checkers.py
+-rw-rw-rw-   0        0        0   605501 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ChildrenHavingMixins.py
+-rw-rw-rw-   0        0        0     8448 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ClassNodes.py
+-rw-rw-rw-   0        0        0     6585 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/CodeObjectSpecs.py
+-rw-rw-rw-   0        0        0    21683 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ComparisonNodes.py
+-rw-rw-rw-   0        0        0    30314 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ConditionalNodes.py
+-rw-rw-rw-   0        0        0    46286 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ConstantRefNodes.py
+-rw-rw-rw-   0        0        0    12213 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ContainerMakingNodes.py
+-rw-rw-rw-   0        0        0     2834 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ContainerOperationNodes.py
+-rw-rw-rw-   0        0        0     4581 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/CoroutineNodes.py
+-rw-rw-rw-   0        0        0     1714 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/CtypesNodes.py
+-rw-rw-rw-   0        0        0    51021 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/DictionaryNodes.py
+-rw-rw-rw-   0        0        0     7856 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ExceptionNodes.py
+-rw-rw-rw-   0        0        0     8044 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ExecEvalNodes.py
+-rw-rw-rw-   0        0        0    44996 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionBases.py
+-rw-rw-rw-   0        0        0    41307 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionBasesGenerated.py
+-rw-rw-rw-   0        0        0    21278 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionShapeMixins.py
+-rw-rw-rw-   0        0        0    12156 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/FrameNodes.py
+-rw-rw-rw-   0        0        0     3544 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/FunctionAttributeNodes.py
+-rw-rw-rw-   0        0        0    39803 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/FunctionNodes.py
+-rw-rw-rw-   0        0        0     5376 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/FutureSpecs.py
+-rw-rw-rw-   0        0        0     6256 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/GeneratorNodes.py
+-rw-rw-rw-   0        0        0     6850 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/GlobalsLocalsNodes.py
+-rw-rw-rw-   0        0        0    74177 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/HardImportNodesGenerated.py
+-rw-rw-rw-   0        0        0     5491 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ImportHardNodes.py
+-rw-rw-rw-   0        0        0    45573 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ImportNodes.py
+-rw-rw-rw-   0        0        0     2733 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/IndicatorMixins.py
+-rw-rw-rw-   0        0        0     1502 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/InjectCNodes.py
+-rw-rw-rw-   0        0        0    11228 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/IterationHandles.py
+-rw-rw-rw-   0        0        0    11002 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/KeyValuePairNodes.py
+-rw-rw-rw-   0        0        0    16320 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ListOperationNodes.py
+-rw-rw-rw-   0        0        0    23094 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/LocalsDictNodes.py
+-rw-rw-rw-   0        0        0    14922 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/LocalsScopes.py
+-rw-rw-rw-   0        0        0    15581 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/LoopNodes.py
+-rw-rw-rw-   0        0        0     1712 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/MatchNodes.py
+-rw-rw-rw-   0        0        0     6534 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ModuleAttributeNodes.py
+-rw-rw-rw-   0        0        0    34377 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ModuleNodes.py
+-rw-rw-rw-   0        0        0    24899 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/NodeBases.py
+-rw-rw-rw-   0        0        0    15128 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/NodeMakingHelpers.py
+-rw-rw-rw-   0        0        0     5550 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/NodeMetaClasses.py
+-rw-rw-rw-   0        0        0    31894 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/OperatorNodes.py
+-rw-rw-rw-   0        0        0     9134 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/OperatorNodesUnary.py
+-rw-rw-rw-   0        0        0     4202 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/OsSysNodes.py
+-rw-rw-rw-   0        0        0    12442 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/OutlineNodes.py
+-rw-rw-rw-   0        0        0    31342 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/PackageMetadataNodes.py
+-rw-rw-rw-   0        0        0     4464 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/PackageResourceNodes.py
+-rw-rw-rw-   0        0        0     3407 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/PrintNodes.py
+-rw-rw-rw-   0        0        0     6772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/ReturnNodes.py
+-rw-rw-rw-   0        0        0     4309 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/SideEffectNodes.py
+-rw-rw-rw-   0        0        0    12501 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/SliceNodes.py
+-rw-rw-rw-   0        0        0    94880 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/StatementBasesGenerated.py
+-rw-rw-rw-   0        0        0     9430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/StatementNodes.py
+-rw-rw-rw-   0        0        0    28658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/StrNodes.py
+-rw-rw-rw-   0        0        0     3504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/StringConcatenationNodes.py
+-rw-rw-rw-   0        0        0     8640 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/SubscriptNodes.py
+-rw-rw-rw-   0        0        0    17853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/TryNodes.py
+-rw-rw-rw-   0        0        0     2405 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/TypeMatchNodes.py
+-rw-rw-rw-   0        0        0     9800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/TypeNodes.py
+-rw-rw-rw-   0        0        0    39522 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/VariableAssignNodes.py
+-rw-rw-rw-   0        0        0    10746 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/VariableDelNodes.py
+-rw-rw-rw-   0        0        0     4574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/VariableNameNodes.py
+-rw-rw-rw-   0        0        0    30982 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/VariableRefNodes.py
+-rw-rw-rw-   0        0        0     4550 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/VariableReleaseNodes.py
+-rw-rw-rw-   0        0        0     3902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/YieldNodes.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.525394 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/
+-rw-rw-rw-   0        0        0   156243 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/BuiltinTypeShapes.py
+-rw-rw-rw-   0        0        0     4387 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/ControlFlowDescriptions.py
+-rw-rw-rw-   0        0        0     4567 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/ShapeMixins.py
+-rw-rw-rw-   0        0        0    42374 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/StandardShapes.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.539065 Nuitka-winsvc-1.5.7/nuitka/optimizations/
+-rw-rw-rw-   0        0        0     3279 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/BytecodeDemotion.py
+-rw-rw-rw-   0        0        0     4038 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/FunctionInlining.py
+-rw-rw-rw-   0        0        0     2144 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/Graphs.py
+-rw-rw-rw-   0        0        0    10762 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/Optimization.py
+-rw-rw-rw-   0        0        0    52154 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/OptimizeBuiltinCalls.py
+-rw-rw-rw-   0        0        0     2272 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/Tags.py
+-rw-rw-rw-   0        0        0    40896 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/TraceCollections.py
+-rw-rw-rw-   0        0        0    23977 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/ValueTraces.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/optimizations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.542972 Nuitka-winsvc-1.5.7/nuitka/pgo/
+-rw-rw-rw-   0        0        0     4663 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/pgo/PGO.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/pgo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.546875 Nuitka-winsvc-1.5.7/nuitka/plugins/
+-rw-rw-rw-   0        0        0    39068 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/PluginBase.py
+-rw-rw-rw-   0        0        0    52902 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/Plugins.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.596680 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/
+-rw-rw-rw-   0        0        0    18092 2023-02-14 03:02:21.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/AntiBloatPlugin.py
+-rw-rw-rw-   0        0        0     3460 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py
+-rw-rw-rw-   0        0        0     9939 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DataFilesPlugin.py
+-rw-rw-rw-   0        0        0     4051 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DelvewheelPlugin.py
+-rw-rw-rw-   0        0        0     5675 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DillPlugin.py
+-rw-rw-rw-   0        0        0    12182 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DllFilesPlugin.py
+-rw-rw-rw-   0        0        0     2062 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/EnumPlugin.py
+-rw-rw-rw-   0        0        0     1905 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/EventletPlugin.py
+-rw-rw-rw-   0        0        0     1880 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GeventPlugin.py
+-rw-rw-rw-   0        0        0     3482 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GiPlugin.py
+-rw-rw-rw-   0        0        0     5027 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GlfwPlugin.py
+-rw-rw-rw-   0        0        0    18758 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/ImplicitImports.py
+-rw-rw-rw-   0        0        0     4948 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/KivyPlugin.py
+-rw-rw-rw-   0        0        0     7258 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/MatplotlibPlugin.py
+-rw-rw-rw-   0        0        0     6750 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/MultiprocessingPlugin.py
+-rw-rw-rw-   0        0        0     1187 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/NumpyPlugin.py
+-rw-rw-rw-   0        0        0     6554 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/OptionsNannyPlugin.py
+-rw-rw-rw-   0        0        0     1917 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PbrPlugin.py
+-rw-rw-rw-   0        0        0     4665 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PkgResourcesPlugin.py
+-rw-rw-rw-   0        0        0     6992 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PmwPlugin.py
+-rw-rw-rw-   0        0        0    49324 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PySidePyQtPlugin.py
+-rw-rw-rw-   0        0        0     2933 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PywebViewPlugin.py
+-rw-rw-rw-   0        0        0     1160 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TensorflowPlugin.py
+-rw-rw-rw-   0        0        0    12180 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TkinterPlugin.py
+-rw-rw-rw-   0        0        0     1140 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TorchPlugin.py
+-rw-rw-rw-   0        0        0     3175 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TrioPlugin.py
+-rw-rw-rw-   0        0        0     5553 2023-03-28 09:14:06.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/UpxPlugin.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/__init__.py
+-rw-rw-rw-   0        0        0   127647 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/standard.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     2221 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml
+-rw-rw-rw-   0        0        0     8831 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.644131 Nuitka-winsvc-1.5.7/nuitka/reports/
+-rw-rw-rw-   0        0        0     2209 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/reports/LicenseReport.rst.j2
+-rw-rw-rw-   0        0        0    15558 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/reports/Reports.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/reports/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.661698 Nuitka-winsvc-1.5.7/nuitka/specs/
+-rw-rw-rw-   0        0        0     5911 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinBytesOperationSpecs.py
+-rw-rw-rw-   0        0        0     2786 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinDictOperationSpecs.py
+-rw-rw-rw-   0        0        0     2541 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinListOperationSpecs.py
+-rw-rw-rw-   0        0        0    26455 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinParameterSpecs.py
+-rw-rw-rw-   0        0        0     6065 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinStrOperationSpecs.py
+-rw-rw-rw-   0        0        0     1159 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinTypeOperationSpecs.py
+-rw-rw-rw-   0        0        0     4802 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinUnicodeOperationSpecs.py
+-rw-rw-rw-   0        0        0     5133 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/specs/HardImportSpecs.py
+-rw-rw-rw-   0        0        0    18740 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/specs/ParameterSpecs.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/specs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.665605 Nuitka-winsvc-1.5.7/nuitka/tools/
+-rw-rw-rw-   0        0        0     1603 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/Basics.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.667557 Nuitka-winsvc-1.5.7/nuitka/tools/commercial/
+-rw-rw-rw-   0        0        0      815 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/commercial/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.674401 Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/
+-rw-rw-rw-   0        0        0    14081 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/DataComposer.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/__init__.py
+-rw-rw-rw-   0        0        0     1306 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.680251 Nuitka-winsvc-1.5.7/nuitka/tools/environments/
+-rw-rw-rw-   0        0        0     2449 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/environments/CreateEnvironment.py
+-rw-rw-rw-   0        0        0     3735 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/environments/Virtualenv.py
+-rw-rw-rw-   0        0        0      833 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/environments/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.682204 Nuitka-winsvc-1.5.7/nuitka/tools/general/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/general/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.687106 Nuitka-winsvc-1.5.7/nuitka/tools/general/dll_report/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/general/dll_report/__init__.py
+-rw-rw-rw-   0        0        0     2366 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/general/dll_report/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.691975 Nuitka-winsvc-1.5.7/nuitka/tools/general/find_module/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/general/find_module/__init__.py
+-rw-rw-rw-   0        0        0     1238 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/general/find_module/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.698391 Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/
+-rw-rw-rw-   0        0        0     8869 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/OnefileCompressor.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.701320 Nuitka-winsvc-1.5.7/nuitka/tools/profiler/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/profiler/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/profiler/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.710108 Nuitka-winsvc-1.5.7/nuitka/tools/scanning/
+-rw-rw-rw-   0        0        0     2369 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/scanning/DisplayPackageDLLs.py
+-rw-rw-rw-   0        0        0     2049 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/scanning/DisplayPackageData.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/scanning/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.723777 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/
+-rw-rw-rw-   0        0        0    51143 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/CTypeDescriptions.py
+-rw-rw-rw-   0        0        0     7685 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/Common.py
+-rw-rw-rw-   0        0        0    39625 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/SpecializeC.py
+-rw-rw-rw-   0        0        0    33585 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/SpecializePython.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/specialize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.745259 Nuitka-winsvc-1.5.7/nuitka/tools/testing/
+-rw-rw-rw-   0        0        0    55189 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/Common.py
+-rw-rw-rw-   0        0        0     1483 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/Constructs.py
+-rw-rw-rw-   0        0        0     8940 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/OutputComparison.py
+-rw-rw-rw-   0        0        0     1278 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/Pythons.py
+-rw-rw-rw-   0        0        0     7888 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/RuntimeTracing.py
+-rw-rw-rw-   0        0        0     5371 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/SearchModes.py
+-rw-rw-rw-   0        0        0     3375 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/Valgrind.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.748190 Nuitka-winsvc-1.5.7/nuitka/tools/testing/check_reference_counts/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/check_reference_counts/__init__.py
+-rw-rw-rw-   0        0        0     3064 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/check_reference_counts/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.754053 Nuitka-winsvc-1.5.7/nuitka/tools/testing/compare_with_cpython/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/compare_with_cpython/__init__.py
+-rw-rw-rw-   0        0        0    29429 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/compare_with_cpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.758937 Nuitka-winsvc-1.5.7/nuitka/tools/testing/find_sxs_modules/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/find_sxs_modules/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/find_sxs_modules/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.762385 Nuitka-winsvc-1.5.7/nuitka/tools/testing/measure_construct_performance/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/measure_construct_performance/__init__.py
+-rw-rw-rw-   0        0        0     8755 2023-02-22 01:49:06.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/measure_construct_performance/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.764339 Nuitka-winsvc-1.5.7/nuitka/tools/testing/run_nuitka_tests/
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/run_nuitka_tests/__init__.py
+-rw-rw-rw-   0        0        0    36321 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tools/testing/run_nuitka_tests/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.828915 Nuitka-winsvc-1.5.7/nuitka/tree/
+-rw-rw-rw-   0        0        0    46475 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/Building.py
+-rw-rw-rw-   0        0        0    75578 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ComplexCallHelperFunctions.py
+-rw-rw-rw-   0        0        0     1700 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/Extractions.py
+-rw-rw-rw-   0        0        0     2572 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/InternalModule.py
+-rw-rw-rw-   0        0        0     1511 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/Operations.py
+-rw-rw-rw-   0        0        0     2807 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationAssertStatements.py
+-rw-rw-rw-   0        0        0    42974 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationAssignmentStatements.py
+-rw-rw-rw-   0        0        0     2948 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationBooleanExpressions.py
+-rw-rw-rw-   0        0        0    11693 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationCallExpressions.py
+-rw-rw-rw-   0        0        0    15208 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationClasses.py
+-rw-rw-rw-   0        0        0    30125 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationClasses3.py
+-rw-rw-rw-   0        0        0     6430 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationComparisonExpressions.py
+-rw-rw-rw-   0        0        0    22111 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationContractionExpressions.py
+-rw-rw-rw-   0        0        0    11160 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationDictionaryCreation.py
+-rw-rw-rw-   0        0        0    14876 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationExecStatements.py
+-rw-rw-rw-   0        0        0     7782 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationForLoopStatements.py
+-rw-rw-rw-   0        0        0    26211 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationFunctionStatements.py
+-rw-rw-rw-   0        0        0    13437 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationImportStatements.py
+-rw-rw-rw-   0        0        0     6577 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationLambdaExpressions.py
+-rw-rw-rw-   0        0        0    20962 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationMatchStatements.py
+-rw-rw-rw-   0        0        0     2409 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationMultidist.py
+-rw-rw-rw-   0        0        0     8194 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationNamespacePackages.py
+-rw-rw-rw-   0        0        0     4658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationPrintStatements.py
+-rw-rw-rw-   0        0        0    15371 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationSequenceCreation.py
+-rw-rw-rw-   0        0        0     4824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationSubscriptExpressions.py
+-rw-rw-rw-   0        0        0    14615 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationTryExceptStatements.py
+-rw-rw-rw-   0        0        0     6982 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationTryFinallyStatements.py
+-rw-rw-rw-   0        0        0     5674 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationWhileLoopStatements.py
+-rw-rw-rw-   0        0        0    14341 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationWithStatements.py
+-rw-rw-rw-   0        0        0     3088 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationYieldExpressions.py
+-rw-rw-rw-   0        0        0     9285 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/SourceHandling.py
+-rw-rw-rw-   0        0        0     3757 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/SyntaxErrors.py
+-rw-rw-rw-   0        0        0    22973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/TreeHelpers.py
+-rw-rw-rw-   0        0        0    20012 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/tree/VariableClosure.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/tree/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.874420 Nuitka-winsvc-1.5.7/nuitka/utils/
+-rw-rw-rw-   0        0        0     2484 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/utils/AppDirs.py
+-rw-rw-rw-   0        0        0     3248 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/CStrings.py
+-rw-rw-rw-   0        0        0     3653 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/CommandLineOptions.py
+-rw-rw-rw-   0        0        0     2855 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Distributions.py
+-rw-rw-rw-   0        0        0     5794 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Download.py
+-rw-rw-rw-   0        0        0    12216 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Execution.py
+-rw-rw-rw-   0        0        0    30973 2023-04-06 02:35:44.000000 Nuitka-winsvc-1.5.7/nuitka/utils/FileOperations.py
+-rw-rw-rw-   0        0        0     2885 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Hashing.py
+-rw-rw-rw-   0        0        0     2362 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Images.py
+-rw-rw-rw-   0        0        0     6816 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Importing.py
+-rw-rw-rw-   0        0        0     7923 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/utils/InstalledPythons.py
+-rw-rw-rw-   0        0        0     2224 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/InstanceCounters.py
+-rw-rw-rw-   0        0        0     4336 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Jinja2.py
+-rw-rw-rw-   0        0        0     1216 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Json.py
+-rw-rw-rw-   0        0        0     4173 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/MacOSApp.py
+-rw-rw-rw-   0        0        0     5040 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/nuitka/utils/MemoryUsage.py
+-rw-rw-rw-   0        0        0     9057 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/ModuleNames.py
+-rw-rw-rw-   0        0        0     4246 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/utils/ReExecute.py
+-rw-rw-rw-   0        0        0     3815 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Rest.py
+-rw-rw-rw-   0        0        0    21979 2023-03-20 05:44:19.000000 Nuitka-winsvc-1.5.7/nuitka/utils/SharedLibraries.py
+-rw-rw-rw-   0        0        0     3664 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Shebang.py
+-rw-rw-rw-   0        0        0     2507 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Signing.py
+-rw-rw-rw-   0        0        0     6207 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/StaticLibraries.py
+-rw-rw-rw-   0        0        0     2602 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/ThreadedExecutor.py
+-rw-rw-rw-   0        0        0     2772 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Timing.py
+-rw-rw-rw-   0        0        0    10826 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Utils.py
+-rw-rw-rw-   0        0        0    10574 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/WindowsFileUsage.py
+-rw-rw-rw-   0        0        0    19540 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/WindowsResources.py
+-rw-rw-rw-   0        0        0     6084 2023-04-26 09:34:14.000000 Nuitka-winsvc-1.5.7/nuitka/utils/Yaml.py
+-rw-rw-rw-   0        0        0      833 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/nuitka/utils/__init__.py
+-rw-rw-rw-   0        0        0      834 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:52:44.345741 Nuitka-winsvc-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0    14957 2023-04-26 09:36:57.000000 Nuitka-winsvc-1.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.881265 Nuitka-winsvc-1.5.7/tests/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.996622 Nuitka-winsvc-1.5.7/tests/basics/
+-rw-rw-rw-   0        0        0     1766 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/AssertsTest.py
+-rw-rw-rw-   0        0        0     5934 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/AssignmentsTest.py
+-rw-rw-rw-   0        0        0     5866 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/AssignmentsTest32.py
+-rw-rw-rw-   0        0        0     4055 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/BranchingTest.py
+-rw-rw-rw-   0        0        0     1104 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/BuiltinOverload.py
+-rw-rw-rw-   0        0        0     3749 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/BuiltinSuperTest.py
+-rw-rw-rw-   0        0        0    17079 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/basics/BuiltinsTest.py
+-rw-rw-rw-   0        0        0      866 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ClassMinimalTest.py
+-rw-rw-rw-   0        0        0     4764 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ClassesTest.py
+-rw-rw-rw-   0        0        0     3414 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ClassesTest32.py
+-rw-rw-rw-   0        0        0     1406 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ClassesTest34.py
+-rw-rw-rw-   0        0        0     4698 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ComparisonChainsTest.py
+-rw-rw-rw-   0        0        0     4639 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/basics/ConstantsTest.py
+-rw-rw-rw-   0        0        0      995 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ConstantsTest27.py
+-rw-rw-rw-   0        0        0     1628 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/DecoratorsTest.py
+-rw-rw-rw-   0        0        0     2317 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/DefaultParametersTest.py
+-rw-rw-rw-   0        0        0     1127 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/DoubleDeletionsTest.py
+-rw-rw-rw-   0        0        0      806 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/EmptyModuleTest.py
+-rw-rw-rw-   0        0        0    14391 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest.py
+-rw-rw-rw-   0        0        0      961 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest32.py
+-rw-rw-rw-   0        0        0     1458 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest33.py
+-rw-rw-rw-   0        0        0     6745 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ExecEvalTest.py
+-rw-rw-rw-   0        0        0     1417 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ExtremeClosureTest.py
+-rw-rw-rw-   0        0        0     1658 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/FunctionObjectsTest.py
+-rw-rw-rw-   0        0        0    12335 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest.py
+-rw-rw-rw-   0        0        0     3603 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest32.py
+-rw-rw-rw-   0        0        0     2627 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest_2.py
+-rw-rw-rw-   0        0        0      890 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/FutureTest32.py
+-rw-rw-rw-   0        0        0     5809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/GeneratorExpressionsTest.py
+-rw-rw-rw-   0        0        0     1041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/GeneratorExpressionsTest_37.py
+-rw-rw-rw-   0        0        0     3824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/GlobalStatementTest.py
+-rw-rw-rw-   0        0        0     1286 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/HelloWorldTest_2.py
+-rw-rw-rw-   0        0        0     2469 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ImportingTest.py
+-rw-rw-rw-   0        0        0     1296 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/InplaceOperationsTest.py
+-rw-rw-rw-   0        0        0     4227 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/basics/InspectionTest.py
+-rw-rw-rw-   0        0        0     1504 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/InspectionTest_35.py
+-rw-rw-rw-   0        0        0     1618 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/InspectionTest_36.py
+-rw-rw-rw-   0        0        0     1671 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/LambdasTest.py
+-rw-rw-rw-   0        0        0     2731 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/LateClosureAssignmentTest.py
+-rw-rw-rw-   0        0        0     2923 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ListContractionsTest.py
+-rw-rw-rw-   0        0        0     3329 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/LoopingTest.py
+-rw-rw-rw-   0        0        0     1536 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/MainProgramsTest.py
+-rw-rw-rw-   0        0        0     1925 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/basics/ModuleAttributesTest.py
+-rw-rw-rw-   0        0        0     1988 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/OperatorsTest.py
+-rw-rw-rw-   0        0        0    14903 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/OrderChecksTest.py
+-rw-rw-rw-   0        0        0     1827 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/OrderChecksTest27.py
+-rw-rw-rw-   0        0        0     1452 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/OverflowFunctionsTest_2.py
+-rw-rw-rw-   0        0        0     5853 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ParameterErrorsTest.py
+-rw-rw-rw-   0        0        0     1899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ParameterErrorsTest32.py
+-rw-rw-rw-   0        0        0      863 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/PrintFutureTest.py
+-rw-rw-rw-   0        0        0     1413 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/PrintingTest_2.py
+-rw-rw-rw-   0        0        0      878 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/RecursionTest.py
+-rw-rw-rw-   0        0        0    23840 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest.py
+-rw-rw-rw-   0        0        0     2076 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest27.py
+-rw-rw-rw-   0        0        0     7819 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest33.py
+-rw-rw-rw-   0        0        0     4902 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest35.py
+-rw-rw-rw-   0        0        0     5092 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest36.py
+-rw-rw-rw-   0        0        0     2899 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest_2.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/SlotsTest.py
+-rw-rw-rw-   0        0        0     1159 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/ThreadedGeneratorsTest.py
+-rw-rw-rw-   0        0        0    22965 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest32.py
+-rw-rw-rw-   0        0        0     1541 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest35.py
+-rw-rw-rw-   0        0        0     1788 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest_2.py
+-rw-rw-rw-   0        0        0     2086 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryContinueFinallyTest.py
+-rw-rw-rw-   0        0        0     2212 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryExceptContinueTest.py
+-rw-rw-rw-   0        0        0     2275 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryExceptFinallyTest.py
+-rw-rw-rw-   0        0        0     2305 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryExceptFramesTest.py
+-rw-rw-rw-   0        0        0     2842 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryReturnFinallyTest.py
+-rw-rw-rw-   0        0        0     2328 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/TryYieldFinallyTest.py
+-rw-rw-rw-   0        0        0     1093 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/UnicodeTest.py
+-rw-rw-rw-   0        0        0     1877 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/UnpackingTest35.py
+-rw-rw-rw-   0        0        0     2095 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/VarargsTest.py
+-rw-rw-rw-   0        0        0     4879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/WithStatementsTest.py
+-rw-rw-rw-   0        0        0     3072 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/YieldFromTest33.py
+-rw-rw-rw-   0        0        0     3821 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/basics/run_all.py
+-rw-rw-rw-   0        0        0     2271 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/basics/run_xml.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:43.999552 Nuitka-winsvc-1.5.7/tests/onefile/
+-rw-rw-rw-   0        0        0      993 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/onefile/HelloWorldTest.py
+-rw-rw-rw-   0        0        0     1307 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/onefile/KeyboardInterruptTest.py
+-rw-rw-rw-   0        0        0     5816 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/tests/onefile/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.026534 Nuitka-winsvc-1.5.7/tests/optimizations/
+-rw-rw-rw-   0        0        0      958 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/optimizations/ArgumentTypes.py
+-rw-rw-rw-   0        0        0     1055 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Attributes.py
+-rw-rw-rw-   0        0        0     1021 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Calls.py
+-rw-rw-rw-   0        0        0      921 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Conditions.py
+-rw-rw-rw-   0        0        0      909 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/optimizations/DecodingOperations.py
+-rw-rw-rw-   0        0        0     1212 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/FormatStrings36.py
+-rw-rw-rw-   0        0        0     1150 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/HardImports.py
+-rw-rw-rw-   0        0        0      974 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/HardImports_2.py
+-rw-rw-rw-   0        0        0      918 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Iterations.py
+-rw-rw-rw-   0        0        0     1260 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Len.py
+-rw-rw-rw-   0        0        0     2262 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Operations.py
+-rw-rw-rw-   0        0        0     1333 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/optimizations/Subscripts.py
+-rw-rw-rw-   0        0        0     8736 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/optimizations/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.027511 Nuitka-winsvc-1.5.7/tests/packages/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.028488 Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/
+-rw-rw-rw-   0        0        0     2382 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.030440 Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/variable_package/
+-rw-rw-rw-   0        0        0      942 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py
+-rw-rw-rw-   0        0        0     1168 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/variable_package/__init__.py
+-rw-rw-rw-   0        0        0     3671 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.320269 Nuitka-winsvc-1.5.7/tests/packages/sub_package/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.034348 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/
+-rw-rw-rw-   0        0        0     1230 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/__init__.py
+-rw-rw-rw-   0        0        0      908 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/bigkitty.py
+-rw-rw-rw-   0        0        0      910 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/smallkitty.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.041735 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/
+-rw-rw-rw-   0        0        0      929 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/hello.py
+-rw-rw-rw-   0        0        0      966 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/miau.py
+-rw-rw-rw-   0        0        0      968 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/purr.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.323195 Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.044667 Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/some_package/
+-rw-rw-rw-   0        0        0     2336 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/some_package/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.045642 Nuitka-winsvc-1.5.7/tests/plugins/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.054436 Nuitka-winsvc-1.5.7/tests/plugins/data_files/
+-rw-rw-rw-   0        0        0     1332 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/plugins/data_files/DataFilesMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.057362 Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/
+-rw-rw-rw-   0        0        0      924 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/lala.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.058336 Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/sub_dir/
+-rw-rw-rw-   0        0        0        0 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/sub_dir/lulu.txt
+-rw-rw-rw-   0        0        0      255 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/plugins/data_files/test_case.nuitka-package.config.yml
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.060289 Nuitka-winsvc-1.5.7/tests/plugins/parameters/
+-rw-rw-rw-   0        0        0     1019 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/plugins/parameters/ParametersMain.py
+-rw-rw-rw-   0        0        0     2168 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/plugins/parameters/parameter-using-plugin.py
+-rw-rw-rw-   0        0        0     3532 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/plugins/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.061266 Nuitka-winsvc-1.5.7/tests/programs/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.062243 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/
+-rw-rw-rw-   0        0        0      867 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/AbsoluteImportMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.067125 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/
+-rw-rw-rw-   0        0        0      796 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/foobar.py
+-rw-rw-rw-   0        0        0      879 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/local.py
+-rw-rw-rw-   0        0        0      860 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/util.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.068103 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/
+-rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.071035 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/
+-rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.072988 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.073962 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/
+-rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.075771 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/some_package/
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.075914 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/
+-rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.076890 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.078843 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/some_package/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.079820 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/
+-rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.080798 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/Some_Package/
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.081773 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/
+-rw-rw-rw-   0        0        0     1075 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/CasedImportingMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.082749 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/
+-rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.083727 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.086661 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/
+-rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/Some_Module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.088610 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/Some_Package/
+-rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/Some_Package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.090568 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/
+-rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/CyclicImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.094469 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/
+-rw-rw-rw-   0        0        0      875 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py
+-rw-rw-rw-   0        0        0      875 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py
+-rw-rw-rw-   0        0        0      842 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.097397 Nuitka-winsvc-1.5.7/tests/programs/dash_import/
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dash_import/DashImportMain.py
+-rw-rw-rw-   0        0        0      817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dash_import/dash-module.py
+-rw-rw-rw-   0        0        0      817 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dash_import/plus+module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.098373 Nuitka-winsvc-1.5.7/tests/programs/dash_main/
+-rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dash_main/Dash-Main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.099349 Nuitka-winsvc-1.5.7/tests/programs/deep/
+-rw-rw-rw-   0        0        0      898 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/DeepProgramMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.103806 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/
+-rw-rw-rw-   0        0        0      980 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/DeepBrother.py
+-rw-rw-rw-   0        0        0      909 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/DeepChild.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.106736 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/deep_package/
+-rw-rw-rw-   0        0        0      876 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/deep_package/DeepDeepChild.py
+-rw-rw-rw-   0        0        0      952 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/deep_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.108689 Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/
+-rw-rw-rw-   0        0        0      794 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/DunderInitImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.110642 Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/package/
+-rw-rw-rw-   0        0        0      797 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/package/SubModule.py
+-rw-rw-rw-   0        0        0      857 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.111618 Nuitka-winsvc-1.5.7/tests/programs/import_variants/
+-rw-rw-rw-   0        0        0     1005 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/import_variants/ImportVariationsMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.115527 Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/
+-rw-rw-rw-   0        0        0      946 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child1.py
+-rw-rw-rw-   0        0        0     1098 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child2.py
+-rw-rw-rw-   0        0        0      822 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child3.py
+-rw-rw-rw-   0        0        0      994 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.117478 Nuitka-winsvc-1.5.7/tests/programs/main_raises/
+-rw-rw-rw-   0        0        0      911 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/main_raises/ErrorMain.py
+-rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/main_raises/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.121393 Nuitka-winsvc-1.5.7/tests/programs/main_raises2/
+-rw-rw-rw-   0        0        0     1080 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/main_raises2/ErrorInFunctionMain.py
+-rw-rw-rw-   0        0        0      808 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/main_raises2/ErrorRaising.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.122908 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/
+-rw-rw-rw-   0        0        0     1529 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/ModuleAttributesMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.125377 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/
+-rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/Nearby1.py
+-rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.127330 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/
+-rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py
+-rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.130262 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/
+-rw-rw-rw-   0        0        0     1744 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py
+-rw-rw-rw-   0        0        0     1611 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.132213 Nuitka-winsvc-1.5.7/tests/programs/module_exits/
+-rw-rw-rw-   0        0        0      869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/module_exits/ErrorExitingModule.py
+-rw-rw-rw-   0        0        0      867 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/module_exits/Main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.136126 Nuitka-winsvc-1.5.7/tests/programs/module_object_replacing/
+-rw-rw-rw-   0        0        0     1078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py
+-rw-rw-rw-   0        0        0     1359 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/module_object_replacing/SelfReplacingModule.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.138073 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/
+-rw-rw-rw-   0        0        0      990 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.141979 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/__main__.py
+-rw-rw-rw-   0        0        0     1758 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/entry.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.144908 Nuitka-winsvc-1.5.7/tests/programs/named_imports/
+-rw-rw-rw-   0        0        0      846 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/named_imports/NamedImportsMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.146863 Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      824 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.147838 Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/sub_package/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/sub_package/SomeModule.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.148814 Nuitka-winsvc-1.5.7/tests/programs/package_code/
+-rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_code/PackageInitCodeMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.150766 Nuitka-winsvc-1.5.7/tests/programs/package_code/some_package/
+-rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_code/some_package/SomeModule.py
+-rw-rw-rw-   0        0        0      809 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_code/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.158579 Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/
+-rw-rw-rw-   0        0        0      789 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/PackageContainsMain.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/local.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.159556 Nuitka-winsvc-1.5.7/tests/programs/package_init_import/
+-rw-rw-rw-   0        0        0      823 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_import/PackageInitImportMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.161507 Nuitka-winsvc-1.5.7/tests/programs/package_init_import/some_package/
+-rw-rw-rw-   0        0        0     1008 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_import/some_package/PackageLocal.py
+-rw-rw-rw-   0        0        0     1169 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_import/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.162484 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/
+-rw-rw-rw-   0        0        0      789 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/PackageInitIssueMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.163461 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/
+-rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.165413 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/child_package/
+-rw-rw-rw-   0        0        0      798 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/child_package/SomeModule.py
+-rw-rw-rw-   0        0        0      795 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/child_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.166390 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/
+-rw-rw-rw-   0        0        0      926 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/PackageMissingInitMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.168347 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/
+-rw-rw-rw-   0        0        0      965 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.170298 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/sub_package/
+-rw-rw-rw-   0        0        0      977 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.173227 Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/
+-rw-rw-rw-   0        0        0      901 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.175102 Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/Something/
+-rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/Something/__init__.py
+-rw-rw-rw-   0        0        0      801 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/something.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.175697 Nuitka-winsvc-1.5.7/tests/programs/package_overload/
+-rw-rw-rw-   0        0        0      852 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_overload/Main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.178626 Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/__init__.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/bar.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/bar2.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.179603 Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/
+-rw-rw-rw-   0        0        0     2972 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.181556 Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/some_package/
+-rw-rw-rw-   0        0        0     1078 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/some_package/__init__.py
+-rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:40.360539 Nuitka-winsvc-1.5.7/tests/programs/package_program/
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.183509 Nuitka-winsvc-1.5.7/tests/programs/package_program/PackageAsMain/
+-rw-rw-rw-   0        0        0      888 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_program/PackageAsMain/__init__.py
+-rw-rw-rw-   0        0        0     1630 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/package_program/PackageAsMain/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.185987 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/
+-rw-rw-rw-   0        0        0     1728 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.187938 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.191843 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.195367 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.196265 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/
+-rw-rw-rw-   0        0        0     1261 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/PkgUtilUsageMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.215793 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE2.txt
+-rw-rw-rw-   0        0        0       14 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/DATA_FILE3.txt
+-rw-rw-rw-   0        0        0     1553 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.216771 Nuitka-winsvc-1.5.7/tests/programs/plugin_import/
+-rw-rw-rw-   0        0        0      859 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/plugin_import/PluginImportMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.220682 Nuitka-winsvc-1.5.7/tests/programs/plugin_import/some_package/
+-rw-rw-rw-   0        0        0      771 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/plugin_import/some_package/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/plugin_import/some_package/some_module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.222631 Nuitka-winsvc-1.5.7/tests/programs/reimport_main_dynamic/
+-rw-rw-rw-   0        0        0      911 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.224187 Nuitka-winsvc-1.5.7/tests/programs/reimport_main_static/
+-rw-rw-rw-   0        0        0      898 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/reimport_main_static/ImportItselfStaticMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.227067 Nuitka-winsvc-1.5.7/tests/programs/relative_import/
+-rw-rw-rw-   0        0        0      842 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/relative_import/RelativeImportMain.py
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/relative_import/dircache.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.228043 Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/
+-rw-rw-rw-   0        0        0     1169 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/ResourceReaderMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.230970 Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/some_package/
+-rw-rw-rw-   0        0        0       13 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/some_package/DATA_FILE.txt
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/some_package/__init__.py
+-rw-rw-rw-   0        0        0     6615 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/tests/programs/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.232924 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/
+-rw-rw-rw-   0        0        0     1171 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/StdlibOverloadMain.py
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/pyexpat.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.239763 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/
+-rw-rw-rw-   0        0        0      769 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/__init__.py
+-rw-rw-rw-   0        0        0      909 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/normal_importing.py
+-rw-rw-rw-   0        0        0      810 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/pyexpat.py
+-rw-rw-rw-   0        0        0     1236 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/star_importing.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.242690 Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/
+-rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/IndentationErroring.py
+-rw-rw-rw-   0        0        0      800 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/SyntaxErroring.py
+-rw-rw-rw-   0        0        0     1079 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/SyntaxErrorsMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.246597 Nuitka-winsvc-1.5.7/tests/programs/unicode_bom/
+-rw-rw-rw-   0        0        0      963 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/unicode_bom/UnicodeBomMain.py
+-rw-rw-rw-   0        0        0      846 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/unicode_bom/unicode_bom.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.247577 Nuitka-winsvc-1.5.7/tests/programs/with space/
+-rw-rw-rw-   0        0        0      826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/programs/with space/Space Main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.249525 Nuitka-winsvc-1.5.7/tests/reflected/
+-rw-rw-rw-   0        0        0    14085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/reflected/compile_itself.py
+-rw-rw-rw-   0        0        0     1243 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/run-tests
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.298869 Nuitka-winsvc-1.5.7/tests/standalone/
+-rw-rw-rw-   0        0        0     1058 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/BrotliUsing.py
+-rw-rw-rw-   0        0        0     2554 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/CtypesUsing.py
+-rw-rw-rw-   0        0        0     1136 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/FlaskUsing.py
+-rw-rw-rw-   0        0        0      990 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/GlfwUsing.py
+-rw-rw-rw-   0        0        0     1184 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/GtkUsing.py
+-rw-rw-rw-   0        0        0     1025 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/HexEncodingTest_2.py
+-rw-rw-rw-   0        0        0     1086 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/IdnaUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/LxmlUsing.py
+-rw-rw-rw-   0        0        0     1431 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/MatplotlibUsing.py
+-rw-rw-rw-   0        0        0     2538 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/MetadataPackagesUsing.py
+-rw-rw-rw-   0        0        0     1727 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/NumpyUsing.py
+-rw-rw-rw-   0        0        0      947 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/OpenGLUsing.py
+-rw-rw-rw-   0        0        0     1379 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PandasUsing.py
+-rw-rw-rw-   0        0        0     1066 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/PasslibUsing.py
+-rw-rw-rw-   0        0        0     1151 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PendulumUsing.py
+-rw-rw-rw-   0        0        0     2074 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PkgResourcesRequiresUsing.py
+-rw-rw-rw-   0        0        0     1067 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PmwUsing.py
+-rw-rw-rw-   0        0        0     1085 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/PyQt5Plugins.py
+-rw-rw-rw-   0        0        0     1105 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/PyQt5SSLSupport.py
+-rw-rw-rw-   0        0        0     2050 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PyQt5Using.py
+-rw-rw-rw-   0        0        0     2050 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/PyQt6Using.py
+-rw-rw-rw-   0        0        0     1757 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/PySide6Using.py
+-rw-rw-rw-   0        0        0     1323 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/RsaUsing.py
+-rw-rw-rw-   0        0        0      973 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/ShlibUsing.py
+-rw-rw-rw-   0        0        0     1504 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/SocketUsing.py
+-rw-rw-rw-   0        0        0     1941 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/TkInterUsing.py
+-rw-rw-rw-   0        0        0     3228 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/Urllib3Using.py
+-rw-rw-rw-   0        0        0     1200 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/standalone/Win32ComUsing.py
+-rw-rw-rw-   0        0        0     9531 2023-04-13 07:04:12.000000 Nuitka-winsvc-1.5.7/tests/standalone/run_all.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.299846 Nuitka-winsvc-1.5.7/tests/standalone/zip_importer/
+-rw-rw-rw-   0        0        0     1264 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/standalone/zip_importer/ZipImporterMain.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:52:44.343788 Nuitka-winsvc-1.5.7/tests/syntax/
+-rw-rw-rw-   0        0        0      811 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/AsyncgenReturn36.py
+-rw-rw-rw-   0        0        0      868 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/BreakWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/ClassReturn.py
+-rw-rw-rw-   0        0        0      970 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/ClosureDel_2.py
+-rw-rw-rw-   0        0        0      849 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/ContinueWithoutLoop.py
+-rw-rw-rw-   0        0        0      791 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/DuplicateArgument.py
+-rw-rw-rw-   0        0        0     1111 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/ExecWithNesting_2.py
+-rw-rw-rw-   0        0        0      826 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/FutureBraces.py
+-rw-rw-rw-   0        0        0      805 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/FutureUnknown.py
+-rw-rw-rw-   0        0        0     1041 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/GeneratorExpressions38.py
+-rw-rw-rw-   0        0        0      879 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/GeneratorReturn_2.py
+-rw-rw-rw-   0        0        0      792 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/GlobalForParameter.py
+-rw-rw-rw-   0        0        0      995 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/Importing32.py
+-rw-rw-rw-   0        0        0      799 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/IndentationError.py
+-rw-rw-rw-   0        0        0      915 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/LateFutureImport.py
+-rw-rw-rw-   0        0        0      841 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/MisplacedFutureImport.py
+-rw-rw-rw-   0        0        0      800 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/ModuleReturn.py
+-rw-rw-rw-   0        0        0      883 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/NonAsciiWithoutEncoding_2.py
+-rw-rw-rw-   0        0        0      794 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/NonlocalForParameter32.py
+-rw-rw-rw-   0        0        0      868 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/NonlocalNotFound32.py
+-rw-rw-rw-   0        0        0      908 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/StarImportExtra.py
+-rw-rw-rw-   0        0        0      869 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/SyntaxError.py
+-rw-rw-rw-   0        0        0      874 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/TryExceptAllNotLast.py
+-rw-rw-rw-   0        0        0      875 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/TryFinallyContinue_37.py
+-rw-rw-rw-   0        0        0      776 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/UnpackNoTuple.py
+-rw-rw-rw-   0        0        0      809 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/UnpackTwoStars32.py
+-rw-rw-rw-   0        0        0      793 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/YieldFromInModule.py
+-rw-rw-rw-   0        0        0      804 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/YieldInAsync35.py
+-rw-rw-rw-   0        0        0      923 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/YieldInGenexp38.py
+-rw-rw-rw-   0        0        0      781 2023-03-14 02:09:13.000000 Nuitka-winsvc-1.5.7/tests/syntax/YieldInModule.py
+-rw-rw-rw-   0        0        0     2203 2023-02-13 06:36:04.000000 Nuitka-winsvc-1.5.7/tests/syntax/run_all.py
```

### Comparing `Nuitka-winsvc-1.5.6/Changelog.rst` & `Nuitka-winsvc-1.5.7/Changelog.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/Developer_Manual.rst` & `Nuitka-winsvc-1.5.7/Developer_Manual.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/LICENSE.txt` & `Nuitka-winsvc-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/MANIFEST.in` & `Nuitka-winsvc-1.5.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/PKG-INFO` & `Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.5.6
+Version: 1.5.7
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.5.6/Nuitka_winsvc.egg-info/SOURCES.txt` & `Nuitka-winsvc-1.5.7/Nuitka_winsvc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/PKG-INFO` & `Nuitka-winsvc-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Nuitka-winsvc
-Version: 1.5.6
+Version: 1.5.7
 Summary: Nuitka but support compile as Windows service
 Home-page: https://github.com/tabris17/Nuitka-winsvc
 Author: tabris17
 Author-email: tabris17.cn@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/tabris17/Nuitka-winsvc
 Keywords: windows service,compiler,python,nuitka
```

### Comparing `Nuitka-winsvc-1.5.6/README.md` & `Nuitka-winsvc-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/README.rst` & `Nuitka-winsvc-1.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/autoformat-nuitka-source` & `Nuitka-winsvc-1.5.7/bin/autoformat-nuitka-source`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/check-nuitka-with-pylint` & `Nuitka-winsvc-1.5.7/bin/check-nuitka-with-pylint`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/compare_with_cpython` & `Nuitka-winsvc-1.5.7/bin/compare_with_cpython`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/compare_with_xml` & `Nuitka-winsvc-1.5.7/bin/compare_with_xml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/measure-construct-performance` & `Nuitka-winsvc-1.5.7/bin/measure-construct-performance`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/nuitka` & `Nuitka-winsvc-1.5.7/bin/nuitka`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/bin/nuitka-run` & `Nuitka-winsvc-1.5.7/bin/nuitka-run`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Horizontal.svg` & `Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Horizontal.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Symbol.svg` & `Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Symbol.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/Logo/Nuitka-Logo-Vertical.svg` & `Nuitka-winsvc-1.5.7/doc/Logo/Nuitka-Logo-Vertical.svg`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Horizontal.png` & `Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Horizontal.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Symbol.png` & `Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Symbol.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/doc/images/Nuitka-Logo-Vertical.png` & `Nuitka-winsvc-1.5.7/doc/images/Nuitka-Logo-Vertical.png`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/lib/hints.py` & `Nuitka-winsvc-1.5.7/lib/hints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/misc/nuitka-run.bat` & `Nuitka-winsvc-1.5.7/misc/nuitka-run.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/misc/nuitka.bat` & `Nuitka-winsvc-1.5.7/misc/nuitka.bat`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Builtins.py` & `Nuitka-winsvc-1.5.7/nuitka/Builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/BytecodeCaching.py` & `Nuitka-winsvc-1.5.7/nuitka/BytecodeCaching.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,35 +84,47 @@
         return None
 
     if data["module_name"] != module_name:
         return None
 
     result = OrderedSet()
 
-    for module in data["modules_used"]:
-        module_name = ModuleName(module["module_name"])
+    for module_used in data["modules_used"]:
+        used_module_name = ModuleName(module_used["module_name"])
 
-        # Retry the module scan.
-        _module_name, filename, module_kind, finding = locateModule(
-            module_name=module_name, parent_package=None, level=0
-        )
+        # Retry the module scan to see if it still gives same result
+        if module_used["finding"] == "relative":
+            _used_module_name, filename, module_kind, finding = locateModule(
+                module_name=used_module_name.getBasename(),
+                parent_package=used_module_name.getPackageName(),
+                level=1,
+            )
+        else:
+            _used_module_name, filename, module_kind, finding = locateModule(
+                module_name=used_module_name, parent_package=None, level=0
+            )
+
+        if (
+            finding != module_used["finding"]
+            or module_kind != module_used["module_kind"]
+        ):
+            assert module_name != "email._header_value_parser", finding
 
-        if finding != module["finding"] or module_kind != module["module_kind"]:
             return None
 
         result.add(
             makeModuleUsageAttempt(
-                module_name=module_name,
+                module_name=used_module_name,
                 filename=filename,
-                finding=module["finding"],
-                module_kind=module["module_kind"],
+                finding=module_used["finding"],
+                module_kind=module_used["module_kind"],
                 # TODO: Level might have to be dropped.
                 level=0,
                 # We store only the line number, so this cheats it to at full one.
-                source_ref=source_ref.atLineNumber(module["source_ref_line"]),
+                source_ref=source_ref.atLineNumber(module_used["source_ref_line"]),
             )
         )
 
     return result
 
 
 def writeImportedModulesNamesToCache(module_name, source_code, used_modules):
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Bytecodes.py` & `Nuitka-winsvc-1.5.7/nuitka/Bytecodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/CacheCleanup.py` & `Nuitka-winsvc-1.5.7/nuitka/CacheCleanup.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Constants.py` & `Nuitka-winsvc-1.5.7/nuitka/Constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Errors.py` & `Nuitka-winsvc-1.5.7/nuitka/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/MainControl.py` & `Nuitka-winsvc-1.5.7/nuitka/MainControl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/ModuleRegistry.py` & `Nuitka-winsvc-1.5.7/nuitka/ModuleRegistry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/OptionParsing.py` & `Nuitka-winsvc-1.5.7/nuitka/OptionParsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Options.py` & `Nuitka-winsvc-1.5.7/nuitka/Options.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/OutputDirectories.py` & `Nuitka-winsvc-1.5.7/nuitka/OutputDirectories.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/PostProcessing.py` & `Nuitka-winsvc-1.5.7/nuitka/PostProcessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         splash_data = getFileContents(splash_screen_filename, mode="rb")
 
         addResourceToFile(
             target_filename=result_filename,
             data=splash_data,
             resource_kind=RT_RCDATA,
             lang_id=0,
-            res_name=27,
+            res_name=28,
             logger=postprocessing_logger,
         )
 
 
 def executePostProcessing():
     """Postprocessing of the resulting binary.
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Progress.py` & `Nuitka-winsvc-1.5.7/nuitka/Progress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/PythonFlavors.py` & `Nuitka-winsvc-1.5.7/nuitka/PythonFlavors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/PythonOperators.py` & `Nuitka-winsvc-1.5.7/nuitka/PythonOperators.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,29 +118,28 @@
 
 
 all_comparison_functions = dict(rich_comparison_functions)
 all_comparison_functions.update(other_comparison_functions)
 
 
 def matchException(left, right):
+    # This doesn't yet work, make it error exit and silence PyLint for now.
+    # pylint: disable=unused-argument
+
     if python_version >= 0x300:
         if type(right) is tuple:
             for element in right:
                 if not isinstance(BaseException, element):
                     raise TypeError(
                         "catching classes that do not inherit from BaseException is not allowed"
                     )
         elif not isinstance(BaseException, right):
             raise TypeError(
                 "catching classes that do not inherit from BaseException is not allowed"
             )
 
-    # This doesn't yet work, make it error exit. and silence PyLint for now.
-    # pylint: disable=protected-access
     import os
 
     os._exit(16)
 
-    assert False, left
-
 
 all_comparison_functions["exception_match"] = matchException
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/PythonVersions.py` & `Nuitka-winsvc-1.5.7/nuitka/PythonVersions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/SourceCodeReferences.py` & `Nuitka-winsvc-1.5.7/nuitka/SourceCodeReferences.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Tracing.py` & `Nuitka-winsvc-1.5.7/nuitka/Tracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/TreeXML.py` & `Nuitka-winsvc-1.5.7/nuitka/TreeXML.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Variables.py` & `Nuitka-winsvc-1.5.7/nuitka/Variables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/Version.py` & `Nuitka-winsvc-1.5.7/nuitka/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #     limitations under the License.
 #
 """ Nuitka version related stuff.
 
 """
 
 version_string = """\
-Nuitka V1.5.6
+Nuitka V1.5.7
 Copyright (C) 2022 Kay Hayen."""
 
 
 def getNuitkaVersion():
     """Return Nuitka version as a string.
 
     This should not be used for >= comparisons directly.
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/__past__.py` & `Nuitka-winsvc-1.5.7/nuitka/__past__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/Backend.scons` & `Nuitka-winsvc-1.5.7/nuitka/build/Backend.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/CCompilerVersion.scons` & `Nuitka-winsvc-1.5.7/nuitka/build/CCompilerVersion.scons`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/DataComposerInterface.py` & `Nuitka-winsvc-1.5.7/nuitka/build/DataComposerInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/Onefile.scons` & `Nuitka-winsvc-1.5.7/nuitka/build/Onefile.scons`

 * *Files 0% similar despite different names*

```diff
@@ -346,14 +346,15 @@
     # With Clang on Windows, there is also an linker to use.
     env.Append(
         CCFLAGS=[
             "/EHsc",  # No C++ exception handling code.
             "/J",  # default char type is unsigned.
             "/Gd",  # Use C calling convention by default.
             "/bigobj",  # Product object files with larger internal limits.
+            "/source-charset:utf-8",
         ]
     )
 
     # No incremental linking.
     env.Append(LINKFLAGS=["/INCREMENTAL:NO"])
 
 if debug_mode:
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsCaching.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsCaching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsCompilerSettings.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsCompilerSettings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsHacks.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsHacks.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsInterface.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsInterface.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsProgress.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsProgress.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsSpawn.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsSpawn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/SconsUtils.py` & `Nuitka-winsvc-1.5.7/nuitka/build/SconsUtils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/allocator.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/allocator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/builtins.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/builtins.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/calling.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/calling.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/checkers.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/checkers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/checksum_tools.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/checksum_tools.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_asyncgen.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_asyncgen.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_cell.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_cell.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_coroutine.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_coroutine.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_frame.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_frame.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_function.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_function.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_generator.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_generator.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/compiled_method.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/compiled_method.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/constants.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/constants.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/constants_blob.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/constants_blob.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/exceptions.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/exceptions.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/filesystem_paths.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/filesystem_paths.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/freelists.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/freelists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/hedley.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/hedley.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/attributes.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/attributes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/boolean.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/boolean.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/bytearrays.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/bytearrays.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/bytes.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/bytes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/calling_generated.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/calling_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_eq.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_eq.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ge.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ge.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_gt.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_gt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_le.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_le.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_lt.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_lt.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/comparisons_ne.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/comparisons_ne.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/complex.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/complex.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/dictionaries.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/dictionaries.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/floats.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/floats.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/import_hard.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/import_hard.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/indexes.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/indexes.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/ints.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/ints.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/iterators.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/iterators.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/lists.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/lists.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/lists_generated.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/lists_generated.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/mappings.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/mappings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_add.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitand.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitor.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_divmod.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_divmod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_lshift.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_matmult.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mod.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_mult.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_pow.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_rshift.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_sub.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_binary_truediv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_binary_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_builtin_types.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_builtin_types.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_add.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_add.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitand.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_bitxor.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_floordiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_lshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_matmult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mod.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mod.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_mult.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_mult.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_olddiv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_pow.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_pow.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_rshift.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_sub.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_sub.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/operations_inplace_truediv.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/raising.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/raising.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/rangeobjects.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/rangeobjects.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/richcomparisons.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/richcomparisons.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/sequences.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/sequences.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/sets.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/sets.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/slices.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/slices.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/strings.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/strings.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/subscripts.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/subscripts.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helper/tuples.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helper/tuples.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/helpers.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/helpers.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/importing.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/importing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/incbin.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/incbin.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/prelude.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/prelude.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/printing.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/printing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/python_pgo.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/python_pgo.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/safe_string_ops.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/safe_string_ops.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/threading.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/threading.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/tracing.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/tracing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/include/nuitka/unfreezing.h` & `Nuitka-winsvc-1.5.7/nuitka/build/include/nuitka/unfreezing.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/appdirs/LICENSE.txt` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/appdirs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/appdirs/appdirs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/appdirs/appdirs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/atomicwrites/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/atomicwrites/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/atomicwrites/atomicwrites.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/atomicwrites/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/bin/scons.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/bin/scons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/clcache/clcache/caching.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/clcache/clcache/caching.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/LICENSE.txt` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansi.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/initialise.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/win32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/colorama/colorama/winterm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/colorama/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/compat.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/fnmatch.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/fnmatch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/glob2/glob2/impl.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/glob2/glob2/impl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/LICENSE.rst` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_compat.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/bccache.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/compiler.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/constants.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/debug.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/defaults.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/environment.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/ext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/filters.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/lexer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/loaders.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/meta.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/nodes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/parser.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/runtime.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/tests.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/utils.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2/jinja2/visitor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/LICENSE.rst` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/_identifier.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/bccache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/compiler.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/exceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/ext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/filters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/idtracking.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/lexer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/loaders.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/meta.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nativetypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/optimizer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/runtime.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/sandbox.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/tests.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/jinja2_35/jinja2/visitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/BoolOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/EnumOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/ListOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PackageOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/PathOption.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Options/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Sig.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/BitKeeper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/CVS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Perforce.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/RCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/SCCS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/Subversion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixf77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/g77.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gdc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gfortran.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/lex.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_builtins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_collections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_hashlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_io.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_sets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/compat/_scons_subprocess.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-2.3.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/docbook/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-3.1.2/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Action.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Builder.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/CacheDir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Conftest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Debug.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Defaults.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Environment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/EnvironmentValues.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Errors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Executor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Job.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Memoize.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Alias.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/FS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/Python.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Node/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/PathList.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/aix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/cygwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/darwin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/hpux.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/irix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/os2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/posix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/sunos.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Platform/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConf.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/SConsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/C.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Dir.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/Prog.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/RC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Interactive.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConsOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/SConscript.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Script/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Subst.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Taskmaster.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/386asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/GettextCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/arch.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/netframework.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/sdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/MSCommon/vs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/PharLapCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/aixlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/applelink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/as.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/asm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/bcc32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/c++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/clangxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/cyglink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/default.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/filesystem.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/g++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gettext_tool.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gnulink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/gxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hpcxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/hplink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/icl.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/ilink32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/install.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/intelc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/link.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/LoadableModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/SharedLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkCommon/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/linkloc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/m4.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/masm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mingw.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgfmt.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msginit.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msgmerge.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mslink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mssdk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/msvs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwcc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/mwld.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/nasm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rmic.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/rpcgen.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgiar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgic++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgicxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sgilink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunc++.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncc.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/suncxx.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/sunlink.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/textfile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/tlib.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/wix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/xgettext.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Tool/zip.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/ConfigureCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Utilities/sconsign.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/BoolVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/EnumVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/ListVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PackageVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/PathVariable.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Variables/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/Warnings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/_scons_dbm.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/compat/win32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/cpp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/dblite.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/lib/scons-4.3.0/SCons/exitfuncs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/LICENSE.rst` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_constants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/markupsafe/markupsafe/_native.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/pkg_resources/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_monitor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_tqdm_pandas.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/_utils.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/_utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/auto.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/auto.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/autonotebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/dask.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/dask.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/gui.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/gui.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/notebook.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/notebook.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/std.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/std.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/tk.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/tk.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/tqdm/tqdm/utils.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/tqdm/tqdm/utils.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/composer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/constructor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/cyaml.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/dumper.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/emitter.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/error.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/events.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/loader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/nodes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/parser.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/reader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/representer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/resolver.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/scanner.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/serializer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml/yaml/tokens.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/composer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/constructor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/dumper.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/emitter.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/error.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/events.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/loader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/nodes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/parser.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/reader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/representer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/resolver.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/scanner.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/serializer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_27/yaml/tokens.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_27/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/LICENSE` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/LICENSE`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/composer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/composer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/constructor.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/constructor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/cyaml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/dumper.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/dumper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/emitter.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/emitter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/error.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/error.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/events.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/events.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/loader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/loader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/nodes.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/parser.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/parser.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/reader.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/reader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/representer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/representer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/resolver.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/resolver.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/scanner.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/scanner.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/serializer.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/serializer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/yaml_35/yaml/tokens.py` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/yaml_35/yaml/tokens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/LICENSE.txt` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/bitstream.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/bitstream.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/compiler.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/compiler.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/cpu.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/cpu.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/debug.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/debug.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/entropy_common.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/entropy_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/error_private.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/error_private.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/fse.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/fse.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/fse_decompress.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/huf.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/huf.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/mem.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/mem.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/xxhash.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/xxhash.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_common.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_common.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_deps.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_deps.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_errors.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_errors.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/common/zstd_internal.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/common/zstd_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_ddict.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_block.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/decompress/zstd_decompress_internal.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/inline_copy/zstd/zstd.h` & `Nuitka-winsvc-1.5.7/nuitka/build/inline_copy/zstd/zstd.h`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledAsyncgenType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledAsyncgenType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCellType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCellType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCodeHelpers.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCodeHelpers.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledCoroutineType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledCoroutineType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledFrameType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledFrameType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledFunctionType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledFunctionType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledGeneratorType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledGeneratorType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledGeneratorTypeUncompiledIntegration.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/CompiledMethodType.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/CompiledMethodType.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersAllocator.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersAllocator.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersAttributes.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersAttributes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBuiltin.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBuiltin.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBuiltinTypeMethods.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBuiltinTypeMethods.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersBytes.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersBytes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersCalling.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersCalling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersCallingGenerated.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersCallingGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersChecksumTools.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersChecksumTools.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersClasses.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersClasses.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonEq.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonEq.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonEqUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonEqUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonGe.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonGe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonGt.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonGt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonLe.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonLe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonLt.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonLt.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersComparisonNe.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersComparisonNe.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersConstantsBlob.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersConstantsBlob.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDeepcopy.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDeepcopy.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDictionaries.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDictionaries.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersDictionariesGenerated.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersDictionariesGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersExceptions.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersExceptions.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFiles.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFilesystemPaths.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFilesystemPaths.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersFloats.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersFloats.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersHeapStorage.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersHeapStorage.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersImport.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersImport.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersImportHard.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersImportHard.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersLists.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersLists.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersListsGenerated.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersListsGenerated.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersMappings.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersMappings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersMatching.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersMatching.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAdd.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitand.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitor.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryBitxor.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmod.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryDivmodUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryLshift.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMatmult.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMod.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMult.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryMultUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPow.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryPowUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryRshift.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinarySub.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinarySub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationBinaryTruediv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationBinaryTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAdd.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAdd.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceAddUtils.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitand.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitand.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitor.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceBitxor.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceBitxor.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceFloordiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceLshift.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceLshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMatmult.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMatmult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMod.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMod.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceMult.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceMult.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceOlddiv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplacePow.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplacePow.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceRshift.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceRshift.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceSub.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceSub.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersOperationInplaceTruediv.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersOperationInplaceTruediv.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersProfiling.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersProfiling.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersPythonPgo.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersPythonPgo.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersRaising.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersRaising.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSafeStrings.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSafeStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSequences.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSequences.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersSlices.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersSlices.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersStrings.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersStrings.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersTuples.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersTuples.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/HelpersTypes.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/HelpersTypes.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/InspectPatcher.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/InspectPatcher.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/MainProgram.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/MainProgram.c`

 * *Files 3% similar despite different names*

```diff
@@ -102,70 +102,80 @@
 #endif
 
 #if SYSFLAG_NO_RANDOMIZATION == 1 || SYSFLAG_UNBUFFERED == 1 || defined(_NUITKA_STANDALONE)
 
 #if defined(_WIN32)
 #define environment_char_t wchar_t
 
-static environment_char_t const *getEnvironmentVariable(environment_char_t const *name) {
+static environment_char_t const *getEnvironmentVariable(char const *name) {
     // Max size for environment variables according to docs.
     wchar_t buffer[32768];
     buffer[0] = 0;
 
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
     // Size must be in bytes apparently, not in characters. Cannot be larger anyway.
-    DWORD res = GetEnvironmentVariableW(name, buffer, 65536);
+    DWORD res = GetEnvironmentVariableW(name_wide, buffer, 65536);
 
     if (res == 0 || res > sizeof(buffer)) {
         return NULL;
     }
 
     return wcsdup(buffer);
 }
 
-static void setEnvironmentVariable(environment_char_t const *name, environment_char_t const *value) {
-    DWORD res = SetEnvironmentVariableW(name, value);
+static void setEnvironmentVariable(char const *name, environment_char_t const *value) {
+    assert(name != NULL);
+    assert(value != NULL);
+
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
+    DWORD res = SetEnvironmentVariableW(name_wide, value);
+    assert(wcscmp(getEnvironmentVariable(name), value) == 0);
 
     assert(res != 0);
 }
 
-static void unsetEnvironmentVariable(environment_char_t const *name) {
-    DWORD res = SetEnvironmentVariableW(name, NULL);
+static void unsetEnvironmentVariable(char const *name) {
+    wchar_t name_wide[20];
+    name_wide[0] = 0;
+    appendStringSafeW(name_wide, name, sizeof(name_wide) / sizeof(wchar_t));
+
+    DWORD res = SetEnvironmentVariableW(name_wide, NULL);
 
     assert(res != 0);
 }
 
 #define makeEnvironmentLiteral(x) L##x
 
 #else
 #define environment_char_t char
 
 #define makeEnvironmentLiteral(x) x
 
-static environment_char_t const *getEnvironmentVariable(environment_char_t const *name) { return getenv(name); }
+static environment_char_t const *getEnvironmentVariable(char const *name) { return getenv(name); }
 
-static void setEnvironmentVariable(environment_char_t const *name, environment_char_t const *value) {
-    setenv(name, value, 1);
-}
+static void setEnvironmentVariable(char const *name, environment_char_t const *value) { setenv(name, value, 1); }
 
-static void unsetEnvironmentVariable(environment_char_t const *name) { unsetenv(name); }
+static void unsetEnvironmentVariable(char const *name) { unsetenv(name); }
 
 #endif
 
-static void undoEnvironmentVariable(environment_char_t const *variable_name, environment_char_t const *old_value) {
+static void undoEnvironmentVariable(char const *variable_name, environment_char_t const *old_value) {
     PyObject *os_module = IMPORT_HARD_OS();
     CHECK_OBJECT(os_module);
 
     PyObject *os_environ = PyObject_GetAttrString(os_module, "environ");
     CHECK_OBJECT(os_environ);
 
-#ifdef _WIN32
-    PyObject *variable_name_str = NuitkaUnicode_FromWideChar(variable_name, -1);
-#else
     PyObject *variable_name_str = Nuitka_String_FromString(variable_name);
-#endif
     CHECK_OBJECT(variable_name_str);
 
     if (old_value) {
         setEnvironmentVariable(variable_name, old_value);
 
 #ifdef _WIN32
         PyObject *env_value = NuitkaUnicode_FromWideChar(old_value, -1);
@@ -184,16 +194,15 @@
         Py_DECREF(env_value);
     } else {
         unsetEnvironmentVariable(variable_name);
 
         int res = PyObject_DelItem(os_environ, variable_name_str);
 
         if (unlikely(res != 0)) {
-            PyErr_PrintEx(1);
-            Py_Exit(1);
+            DROP_ERROR_OCCURRED();
         }
     }
 
     Py_DECREF(variable_name_str);
     Py_DECREF(os_environ);
 }
 #endif
@@ -206,24 +215,23 @@
 static environment_char_t const *old_env_pythonhome;
 
 static void prepareStandaloneEnvironment(void) {
     /* Setup environment variables to tell CPython that we would like it to use
      * the provided binary directory as the place to look for DLLs and for
      * extension modules.
      */
-    old_env_path = getEnvironmentVariable(makeEnvironmentLiteral("PATH"));
+    old_env_path = getEnvironmentVariable("PATH");
     // Remove the PATH during Python init, so it won't pick up stuff from there.
-    setEnvironmentVariable(makeEnvironmentLiteral("PATH"), makeEnvironmentLiteral("/"));
-
-    old_env_pythonhome = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"));
+    setEnvironmentVariable("PATH", makeEnvironmentLiteral("/"));
 
+    old_env_pythonhome = getEnvironmentVariable("PYTHONHOME");
 #if defined(_WIN32)
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"), getBinaryDirectoryWideChars());
+    setEnvironmentVariable("PYTHONHOME", getBinaryDirectoryWideChars());
 #else
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHOME"), getBinaryDirectoryHostEncoded());
+    setEnvironmentVariable("PYTHONHOME", getBinaryDirectoryHostEncoded());
 #endif
 
 #if defined(_WIN32)
     SetDllDirectoryW(getBinaryDirectoryWideChars());
 #endif
 
 #if PYTHON_VERSION < 0x300
@@ -926,16 +934,16 @@
 
 #if SYSFLAG_UNBUFFERED == 1
     setbuf(stdin, (char *)NULL);
     setbuf(stdout, (char *)NULL);
     setbuf(stderr, (char *)NULL);
 
 #if PYTHON_VERSION >= 0x300
-    environment_char_t const *old_env_unbuffered = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"));
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"), makeEnvironmentLiteral("1"));
+    environment_char_t const *old_env_unbuffered = getEnvironmentVariable("PYTHONUNBUFFERED");
+    setEnvironmentVariable("PYTHONUNBUFFERED", makeEnvironmentLiteral("1"));
 #endif
 #endif
 
 #ifdef __FreeBSD__
     /* FP exceptions run in "no stop" mode by default */
 
     fp_except_t m;
@@ -1035,16 +1043,16 @@
     Py_SetPythonHome(L"" PYTHON_HOME_PATH);
     // Make sure the above Py_SetPythonHome call has effect already.
     Py_GetPath();
 #endif
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_NO_RANDOMIZATION == 1
-    environment_char_t const *old_env_hash_seed = getEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"));
-    setEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"), makeEnvironmentLiteral("0"));
+    environment_char_t const *old_env_hash_seed = getEnvironmentVariable("PYTHONHASHSEED");
+    setEnvironmentVariable("PYTHONHASHSEED", makeEnvironmentLiteral("0"));
 #endif
 
     /* Disable CPython warnings if requested to. */
 #if NO_PYTHON_WARNINGS
     NUITKA_PRINT_TRACE("main(): Disabling Python warnings.");
     {
 #if PYTHON_VERSION >= 0x300
@@ -1205,27 +1213,27 @@
 #if PYTHON_VERSION >= 0x300
     NUITKA_PRINT_TRACE("main(): Calling patchInspectModule().");
     patchInspectModule();
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_NO_RANDOMIZATION == 1
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PYTHONHASHSEED' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PYTHONHASHSEED"), old_env_hash_seed);
+    undoEnvironmentVariable("PYTHONHASHSEED", old_env_hash_seed);
 #endif
 
 #if PYTHON_VERSION >= 0x300 && SYSFLAG_UNBUFFERED == 1
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PYTHONUNBUFFERED' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PYTHONUNBUFFERED"), old_env_unbuffered);
+    undoEnvironmentVariable("PYTHONUNBUFFERED", old_env_unbuffered);
 #endif
 
 #ifdef _NUITKA_STANDALONE
     // Restore the PATH, so the program can use it.
     NUITKA_PRINT_TRACE("main(): Reverting to initial 'PATH' value.");
-    undoEnvironmentVariable(makeEnvironmentLiteral("PATH"), old_env_path);
-    // undoEnvironmentVariable("PYTHONHOME", old_env_pythonhome);
+    undoEnvironmentVariable("PATH", old_env_path);
+    undoEnvironmentVariable("PYTHONHOME", old_env_pythonhome);
 #endif
 
 #if _NUITKA_PROFILE
     // Profiling with "vmprof" if enabled.
     startProfiling();
 #endif
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoader.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderImportlibMetadataDistribution.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReader.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/MetaPathBasedLoaderResourceReaderFiles.c`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/OnefileBootstrap.c` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/OnefileBootstrap.c`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
 #if _NUITKA_ONEFILE_COMPRESSION_BOOL == 1
 
 static ZSTD_DCtx *dest_ctx = NULL;
 static ZSTD_inBuffer input = {NULL, 0, 0};
 static ZSTD_outBuffer output = {NULL, 0, 0};
 
 static void initZSTD(void) {
-    size_t const input_buffer_size = ZSTD_DStreamInSize();
     input.src = NULL;
 
     size_t const output_buffer_size = ZSTD_DStreamOutSize();
     output.dst = malloc(output_buffer_size);
     if (output.dst == NULL) {
         fatalErrorMemory();
     }
@@ -1064,15 +1063,15 @@
         fatalErrorHeaderAttachedData();
     }
 #endif
 
     static filename_char_t first_filename[1024] = {0};
 
 #if _NUITKA_ONEFILE_SPLASH_SCREEN
-    NUITKA_PRINT_TIMING("ONEFILE: Splash screen.");
+    NUITKA_PRINT_TIMING("ONEFILE: Init splash screen.");
 
     initSplashScreen();
 #endif
 
     NUITKA_PRINT_TIMING("ONEFILE: Entering decompression.");
 
 #if _NUITKA_ONEFILE_TEMP_BOOL == 1
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/build/static_src/OnefileSplashScreen.cpp` & `Nuitka-winsvc-1.5.7/nuitka/build/static_src/OnefileSplashScreen.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,29 @@
 //     See the License for the specific language governing permissions and
 //     limitations under the License.
 //
 // Creates a stream object initialized with the data from an executable resource.
 
 #ifdef __IDE_ONLY__
 #include "HelpersSafeStrings.c"
+#include "nuitka/tracing.h"
 #include <windows.h>
 #endif
 
 #include <assert.h>
 #include <wincodec.h>
 
 #ifdef __MINGW32__
 #error "No support for splash screens with MinGW64 yet, only works with MSVC. Somebody please make it portable."
 #endif
 
 IStream *createImageStream(void) {
 
     // Load the resource with image data
-    HRSRC res_handle = FindResource(NULL, MAKEINTRESOURCE(27), RT_RCDATA);
+    HRSRC res_handle = FindResource(NULL, MAKEINTRESOURCE(28), RT_RCDATA);
     if (res_handle == NULL) {
         return NULL;
     }
     DWORD resource_size = SizeofResource(NULL, res_handle);
     HGLOBAL image_handle = LoadResource(NULL, res_handle);
     if (image_handle == NULL) {
         return NULL;
@@ -217,14 +218,16 @@
     }
 
     HANDLE handle_splash_file =
         CreateFileW(splash_indicator_path, GENERIC_WRITE, FILE_SHARE_WRITE, NULL, CREATE_ALWAYS, 0, NULL);
     CloseHandle(handle_splash_file);
 
     splash_active = true;
+
+    NUITKA_PRINT_TIMING("ONEFILE: Done with splash screen.");
 }
 
 static void closeSplashScreen(void) {
     if (splash_window) {
         DestroyWindow(splash_window);
         splash_window = 0;
     }
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/AsyncgenCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/AsyncgenCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/AttributeCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/AttributeCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/BinaryOperationHelperDefinitions.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/BinaryOperationHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/BranchCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/BranchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/BuiltinCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/BuiltinCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CallCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CallCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ClassCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ClassCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeGeneration.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeGeneration.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeHelperSelection.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeHelperSelection.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeHelpers.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CodeObjectCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CodeObjectCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ComparisonCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ComparisonCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ComparisonHelperDefinitions.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ComparisonHelperDefinitions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ConditionalCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ConditionalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ConstantCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ConstantCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/Contexts.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/Contexts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CoroutineCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CoroutineCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/CtypesCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/CtypesCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/DictCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/DictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/Emission.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/Emission.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ErrorCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ErrorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/EvalCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/EvalCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ExceptionCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ExceptionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ExpressionCTypeSelectionHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ExpressionCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ExpressionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/FrameCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/FrameCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/FunctionCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/FunctionCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/GeneratorCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/GeneratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/GlobalConstants.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/GlobalConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/GlobalsLocalsCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/GlobalsLocalsCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/IdCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/IdCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ImportCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ImportCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/Indentation.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/Indentation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/IndexCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/IndexCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/InjectCCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/InjectCCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/IntegerCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/IntegerCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/IteratorCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/IteratorCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/LabelCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/LabelCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/LineNumberCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/LineNumberCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ListCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ListCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/LoaderCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/LoaderCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/LocalsDictCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/LocalsDictCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/LoopCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/LoopCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/MatchCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/MatchCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ModuleCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ModuleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/Namify.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/Namify.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/OperationCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/OperationCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/PackageResourceCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/PackageResourceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/PrintCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/PrintCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/PythonAPICodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/PythonAPICodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/RaisingCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/RaisingCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/Reports.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/ReturnCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/ReturnCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/SetCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/SetCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/SliceCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/SliceCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/StringCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/StringCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/SubscriptCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/SubscriptCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/TryCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/TryCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/TupleCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/TupleCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/VariableCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/VariableCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/VariableDeclarations.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/VariableDeclarations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/YieldCodes.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/YieldCodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeBases.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeBooleans.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeCFloats.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeCFloats.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeCLongs.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeCLongs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeModuleDictVariables.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeModuleDictVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaBooleans.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaInts.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaInts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeNuitkaVoids.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeNuitkaVoids.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,14 @@
         if Options.is_debug:
             emit("%s = NUITKA_VOID_OK;" % to_name)
 
     @classmethod
     def emitAssignmentCodeFromConstant(
         cls, to_name, constant, may_escape, emit, context
     ):
-        # No context needed, pylint: disable=unused-argument
-
         # Everything else expresses missed compiled time optimization.
         assert constant is None
 
         # The only possible value, and in this case never read, but the compiler hates
         # it being defined which is hard for us to know ahead of time.
         if Options.is_debug:
             emit("%s = NUITKA_VOID_OK;" % to_name)
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypePyObjectPointers.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypePyObjectPointers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/CTypeVoids.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/CTypeVoids.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/c_types/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/c_types/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesAsyncgens.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesConstants.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesConstants.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesCoroutines.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesCoroutines.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesExceptions.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesExceptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesFrames.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesFrames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesFunction.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesGeneratorFunction.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesIterators.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesIterators.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesLoader.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesLoader.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesModules.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesModules.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/CodeTemplatesVariables.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/CodeTemplatesVariables.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/TemplateDebugWrapper.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/TemplateDebugWrapper.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMethodPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsMixed.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositional.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateCallsPositionalMethodDescr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListHinted.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/CodeTemplateMakeListSmall.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperBuiltinMethodOperation.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperDictionaryCopy.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperImportHard.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperImportHard.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperLongTools.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperLongTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperObjectTools.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperObjectTools.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparison.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationComparisonUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperOperationInplace.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBinary.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsBytes.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsCommon.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsFloat.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsInt.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsList.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsList.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsLong.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsSet.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsStr.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsTuple.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2` & `Nuitka-winsvc-1.5.7/nuitka/code_generation/templates_c/HelperSlotsUnicode.c.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/constants/Serialization.py` & `Nuitka-winsvc-1.5.7/nuitka/constants/Serialization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/constants/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/containers/Namedtuples.py` & `Nuitka-winsvc-1.5.7/nuitka/containers/Namedtuples.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/containers/OrderedDicts.py` & `Nuitka-winsvc-1.5.7/nuitka/containers/OrderedDicts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/containers/OrderedSets.py` & `Nuitka-winsvc-1.5.7/nuitka/containers/OrderedSets.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/containers/OrderedSetsFallback.py` & `Nuitka-winsvc-1.5.7/nuitka/containers/OrderedSetsFallback.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/containers/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/distutils/Build.py` & `Nuitka-winsvc-1.5.7/nuitka/distutils/Build.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/distutils/DistutilCommands.py` & `Nuitka-winsvc-1.5.7/nuitka/distutils/DistutilCommands.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,20 @@
 import wheel.bdist_wheel  # pylint: disable=I0021,import-error,no-name-in-module
 
 from nuitka.__past__ import Iterable, unicode
 from nuitka.containers.OrderedSets import OrderedSet
 from nuitka.importing.Importing import (
     addMainScriptDirectory,
     decideModuleSourceRef,
+    flushImportCache,
     locateModule,
 )
 from nuitka.Tracing import wheel_logger
 from nuitka.utils.Execution import check_call
+from nuitka.utils.FileOperations import deleteFile, renameFile
 from nuitka.utils.ModuleNames import ModuleName
 
 
 def setupNuitkaDistutilsCommands(dist, keyword, value):
     # If the user project setup.py includes the key "build_with_nuitka=True" all
     # build operations (build, bdist_wheel, install etc) will run via Nuitka.
     # pylint: disable=unused-argument
@@ -108,15 +110,15 @@
             )
 
         # Python2 does not allow super on this old style class.
         distutils.command.build.build.run(self)
 
         self._build(os.path.abspath(self.build_lib))
 
-    def _findBuildTasks(self):
+    def _findBuildTasks2(self):
         """
         Helper for _build
         Returns list containing bool (is_package) and module_names
 
         Algorithm for finding distinct packages:
         1) Take minimum package
         2) Find related packages that start with this name
@@ -177,14 +179,50 @@
             py_packages = [
                 p for p in py_packages if not p.hasNamespace(current_package)
             ]
             builds.append((True, current_package))
 
         return builds
 
+    def _findBuildTasks(self):
+        builds = self._findBuildTasks2()
+        result = []
+
+        for _is_package, module_name_orig in builds:
+            _module_name, main_filename, module_kind, finding = locateModule(
+                module_name=module_name_orig,
+                parent_package=None,
+                level=0,
+            )
+
+            # Handle extension modules already compiled. They are either to be replaced, or
+            # they are included as they are, because there is no source, then the task can
+            # be skipped.
+            if module_kind == "extension":
+                main_filename_away = main_filename + ".away"
+                renameFile(main_filename, main_filename_away)
+
+                flushImportCache()
+
+                _module_name, main_filename, module_kind, finding = locateModule(
+                    module_name=module_name_orig,
+                    parent_package=None,
+                    level=0,
+                )
+
+                if finding != "not-found":
+                    deleteFile(main_filename_away, must_exist=True)
+                else:
+                    renameFile(main_filename_away, main_filename)
+                    continue
+
+            result.append((_is_package, module_name_orig))
+
+        return result
+
     @staticmethod
     def _parseOptionsEntry(option, value):
         option = "--" + option.lstrip("-")
 
         if type(value) is tuple and len(value) == 2 and value[0] == "setup.py":
             value = value[1]
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/distutils/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/finalizations/Finalization.py` & `Nuitka-winsvc-1.5.7/nuitka/finalizations/Finalization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/finalizations/FinalizeMarkups.py` & `Nuitka-winsvc-1.5.7/nuitka/finalizations/FinalizeMarkups.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/finalizations/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/finalizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/DependsExe.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/DependsExe.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesCommon.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesCommon.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesMacOS.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesMacOS.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesPosix.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesPosix.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/DllDependenciesWin32.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/DllDependenciesWin32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/IncludedDataFiles.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/IncludedDataFiles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/IncludedEntryPoints.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/IncludedEntryPoints.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/Onefile.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/Onefile.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/Standalone.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/Standalone.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,19 @@
                 if package_name is not None:
                     problem_modules.add(package_name)
                 else:
                     problem_modules.add(module_name)
 
     else:
         checkModulePath = None
+        message = None
+        mnemonic = None
 
+    # We intend for other platforms to join, e.g. Fedora, etc. but currently
+    # only Debian is done.
     if checkModulePath is not None:
         for module in ModuleRegistry.getDoneModules():
             checkModulePath(module)
 
     if problem_modules:
         general.info("Using Debian packages for '%s'." % ",".join(problem_modules))
         general.warning(message=message, mnemonic=mnemonic)
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/freezer/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/freezer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/IgnoreListing.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/IgnoreListing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/ImportCache.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/ImportCache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/ImportResolving.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/ImportResolving.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/Importing.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/Importing.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 
 from nuitka import Options, SourceCodeReferences
 from nuitka.__past__ import iter_modules
 from nuitka.containers.Namedtuples import makeNamedtupleClass
 from nuitka.containers.OrderedSets import OrderedSet
 from nuitka.importing import StandardLibrary
 from nuitka.plugins.Plugins import Plugins
+from nuitka.PythonFlavors import isNuitkaPython
 from nuitka.PythonVersions import python_version
 from nuitka.Tracing import my_print, recursion_logger
 from nuitka.tree.ReformulationMultidist import locateMultidistModule
 from nuitka.utils.AppDirs import getCacheDir
 from nuitka.utils.FileOperations import listDir, removeDirectory
 from nuitka.utils.Importing import getSharedLibrarySuffixes
 from nuitka.utils.ModuleNames import ModuleName
@@ -160,14 +161,17 @@
     if os.path.isdir(module_filename):
         return ModuleName(os.path.basename(module_filename)), "py"
 
     return None, None
 
 
 def isIgnoreListedImportMaker(source_ref):
+    if isNuitkaPython():
+        return True
+
     return StandardLibrary.isStandardLibraryPath(source_ref.getFilename())
 
 
 def warnAbout(importing, module_name, level, source_ref):
     # This probably should not be dealt with here
     if module_name == "":
         return
@@ -402,14 +406,25 @@
 
     if path not in _list_dir_cache:
         _list_dir_cache[path] = tuple(listDir(path))
 
     return _list_dir_cache[path]
 
 
+def flushImportCache():
+    """Clear import related caches.
+
+    In some situations, e.g. during package rebuild, we scan and then decide to remove
+    files and scan again. This allows that. Nothing in standard Nuitka should do it,
+    as it throws away so much.
+    """
+    _list_dir_cache.clear()
+    module_search_cache.clear()
+
+
 def _findModuleInPath2(package_name, module_name, search_path):
     """This is out own module finding low level implementation.
 
     Just the full module name and search path are given. This is then
     tasked to raise "ImportError" or return a path if it finds it, or
     None, if it is a built-in.
     """
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/PreloadedPackages.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/PreloadedPackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/Recursion.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/Recursion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/StandardLibrary.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/StandardLibrary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/importing/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/AsyncgenNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/AsyncgenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeLookupNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeLookupNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/AttributeNodesGenerated.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/AttributeNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinAllNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinAllNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinAnyNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinAnyNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinComplexNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinComplexNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDecodingNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDecodingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDecoratorNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDecoratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinDictNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinFormatNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinFormatNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinHashNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinHashNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinIntegerNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinIntegerNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinIteratorNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinIteratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinLenNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinLenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinNextNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinNextNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinOpenNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinOpenNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinOperationNodeBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinRangeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinRangeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinRefNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinSumNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinSumNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinTypeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinTypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BuiltinVarsNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BuiltinVarsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/BytesNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/BytesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/CallNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/CallNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/Checkers.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/Checkers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ChildrenHavingMixins.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ChildrenHavingMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ClassNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ClassNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/CodeObjectSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/CodeObjectSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ComparisonNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ComparisonNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ConditionalNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ConditionalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ConstantRefNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ConstantRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ContainerMakingNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ContainerMakingNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ContainerOperationNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ContainerOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/CoroutineNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/CoroutineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/CtypesNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/CtypesNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/DictionaryNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/DictionaryNodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1410,14 +1410,15 @@
     def computeExpression(self, trace_collection):
         if self.mayRaiseExceptionOperation():
             trace_collection.onExceptionRaiseExit(BaseException)
 
         if self.subnode_iterable.isCompileTimeConstant():
             # TODO: Could be assert against it being None with a compile time constant,
             # we will usually be able to tell?
+            # This is actually OK to use like this, pylint: disable=bad-chained-comparison
             if None is not self.subnode_iterable.getIterationLength() < 256:
                 return trace_collection.getCompileTimeComputationResult(
                     node=self,
                     computation=lambda: dict.fromkeys(
                         self.subnode_iterable.getCompileTimeConstant()
                     ),
                     description="Computed 'dict.fromkeys' with constant value.",
@@ -1428,14 +1429,15 @@
     def mayRaiseException(self, exception_type):
         return (
             self.subnode_iterable.mayRaiseException(exception_type)
             or self.mayRaiseExceptionOperation()
         )
 
     def mayRaiseExceptionOperation(self):
+        # This is actually OK to use like this, pylint: disable=bad-chained-comparison
         return None is not self.subnode_iterable.getIterationLength() < 256
 
 
 class ExpressionDictOperationFromkeys3(ExpressionDictOperationFromkeys3Base):
     kind = "EXPRESSION_DICT_OPERATION_FROMKEYS3"
 
     def computeExpression(self, trace_collection):
@@ -1444,14 +1446,15 @@
 
         if (
             self.subnode_iterable.isCompileTimeConstant()
             and self.subnode_value.isCompileTimeConstant()
         ):
             # TODO: Could be assert against it being None with a compile time constant,
             # we will usually be able to tell?
+            # This is actually OK to use like this, pylint: disable=bad-chained-comparison
             if None is not self.subnode_iterable.getIterationLength() < 256:
                 return trace_collection.getCompileTimeComputationResult(
                     node=self,
                     computation=lambda: dict.fromkeys(
                         self.subnode_iterable.getCompileTimeConstant(),
                         self.subnode_value.getCompileTimeConstant(),
                     ),
@@ -1464,14 +1467,15 @@
         return (
             self.subnode_iterable.mayRaiseException(exception_type)
             or self.subnode_value.mayRaiseException(exception_type)
             or self.mayRaiseExceptionOperation()
         )
 
     def mayRaiseExceptionOperation(self):
+        # This is actually OK to use like this, pylint: disable=bad-chained-comparison
         return None is not self.subnode_iterable.getIterationLength() < 256
 
 
 class ExpressionDictOperationFromkeysRef(ExpressionNoSideEffectsMixin, ExpressionBase):
     kind = "EXPRESSION_DICT_OPERATION_FROMKEYS_REF"
 
     def finalize(self):
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ExceptionNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ExceptionNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ExecEvalNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ExecEvalNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionBases.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionBasesGenerated.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ExpressionShapeMixins.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ExpressionShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/FrameNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/FrameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/FunctionAttributeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/FunctionAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/FunctionNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/FunctionNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -564,17 +564,19 @@
 
 
 class ExpressionFunctionBody(
     ExpressionNoSideEffectsMixin,
     MarkUnoptimizedFunctionIndicatorMixin,
     ExpressionFunctionEntryPointBase,
 ):
+    # TODO: There should be more special ones than this general type in order to
+    # not cover exec ones in the same object. pylint: disable=too-many-instance-attributes
+
     kind = "EXPRESSION_FUNCTION_BODY"
 
-    # TODO: These should be more special than the general type in order to not cover exec ones.
     __slots__ = (
         "unoptimized_locals",
         "unqualified_exec",
         "doc",
         "return_exception",
         "needs_creation",
         "needs_direct",
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/FutureSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/FutureSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/GeneratorNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/GeneratorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/GlobalsLocalsNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/GlobalsLocalsNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/HardImportNodesGenerated.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/HardImportNodesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ImportHardNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ImportHardNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ImportNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ImportNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/IndicatorMixins.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/IndicatorMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/InjectCNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/InjectCNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/IterationHandles.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/IterationHandles.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/KeyValuePairNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/KeyValuePairNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ListOperationNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ListOperationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/LocalsDictNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/LocalsDictNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/LocalsScopes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/LocalsScopes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/LoopNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/LoopNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/MatchNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/MatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ModuleAttributeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ModuleAttributeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ModuleNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ModuleNodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -827,16 +827,15 @@
             "module_name": self.module_name,
             "main_added": self.main_added,
             "mode": self.mode,
         }
 
     @classmethod
     def fromXML(cls, provider, source_ref, **args):
-        if "code_flags" in args:
-            future_spec = fromFlags(args["code_flags"])
+        future_spec = fromFlags(args["code_flags"])
 
         result = cls(
             main_added=args["main_added"] == "True",
             mode=args["mode"],
             module_name=ModuleName(args["module_name"]),
             future_spec=future_spec,
             source_ref=source_ref,
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/NodeBases.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/NodeBases.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/NodeMakingHelpers.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/NodeMakingHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/NodeMetaClasses.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/NodeMetaClasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         if base is not object and "__slots__" not in base.__dict__:
             raise NuitkaNodeDesignError(name, "All bases must have __slots__.", base)
 
 
 class NodeCheckMetaClass(ABCMeta):
     kinds = {}
 
-    def __new__(cls, name, bases, dictionary):  # pylint: disable=I0021,arguments-differ
+    def __new__(mcs, name, bases, dictionary):  # pylint: disable=I0021,arguments-differ
         _checkBases(name, bases)
 
         if "__slots__" not in dictionary:
             dictionary["__slots__"] = ()
 
         if "named_children" in dictionary:
             assert type(dictionary["named_children"]) is tuple
@@ -99,16 +99,15 @@
 
                 dictionary["__init__"] = __init__
 
         # Not a method:
         if "checker" in dictionary:
             dictionary["checker"] = staticmethod(dictionary["checker"])
 
-        # false alarm, pylint: disable=I0021,too-many-function-args
-        return ABCMeta.__new__(cls, name, bases, dictionary)
+        return ABCMeta.__new__(mcs, name, bases, dictionary)
 
     def __init__(cls, name, bases, dictionary):
 
         if not name.endswith(("Base", "Mixin")):
             if "kind" not in dictionary:
                 raise NuitkaNodeDesignError(name, "Must provide class variable 'kind'")
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/OperatorNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/OperatorNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/OperatorNodesUnary.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/OperatorNodesUnary.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/OsSysNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/OsSysNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/OutlineNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/OutlineNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/PackageMetadataNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/PackageMetadataNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/PackageResourceNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/PackageResourceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/PrintNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/PrintNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/ReturnNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/ReturnNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/SideEffectNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/SideEffectNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/SliceNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/SliceNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/StatementBasesGenerated.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/StatementBasesGenerated.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/StatementNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/StatementNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/StrNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/StrNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/StringConcatenationNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/StringConcatenationNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/SubscriptNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/SubscriptNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/TryNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/TryNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/TypeMatchNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/TypeMatchNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/TypeNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/TypeNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/VariableAssignNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/VariableAssignNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/VariableDelNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/VariableDelNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/VariableNameNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/VariableNameNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/VariableRefNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/VariableRefNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/VariableReleaseNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/VariableReleaseNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/YieldNodes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/YieldNodes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/BuiltinTypeShapes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/BuiltinTypeShapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -4088,14 +4088,15 @@
         if value is value2:
             r[key] = value
         elif value[0] is tshape_str_or_unicode and value2[0] is tshape_unicode:
             assert value[1] is value2[1]
 
             r[key] = value
         elif value[0] is tshape_str and value2[0] is tshape_unicode:
+            # Actually as intended, pylint: disable=bad-chained-comparison
             assert (
                 value[1]
                 is value2[1]
                 in (
                     operation_result_strorunicode_noescape[1],
                     ControlFlowDescriptionFormatError,
                 )
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/ControlFlowDescriptions.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/ControlFlowDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/ShapeMixins.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/ShapeMixins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/StandardShapes.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/StandardShapes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/nodes/shapes/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/nodes/shapes/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/BytecodeDemotion.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/BytecodeDemotion.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/FunctionInlining.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/FunctionInlining.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/Graphs.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/Graphs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/Optimization.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/Optimization.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/OptimizeBuiltinCalls.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/OptimizeBuiltinCalls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/Tags.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/Tags.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/TraceCollections.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/TraceCollections.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/ValueTraces.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/ValueTraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/optimizations/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/optimizations/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/pgo/PGO.py` & `Nuitka-winsvc-1.5.7/nuitka/pgo/PGO.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/pgo/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/pgo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/PluginBase.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/PluginBase.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/Plugins.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/Plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,15 +438,15 @@
         with withPluginModuleNameProblemReporting(plugin, package_name):
             for path in plugin.getPackageExtraScanPaths(package_name, package_dir):
                 if os.path.isdir(path):
                     yield path
 
     @classmethod
     def getPackageExtraScanPaths(cls, package_name, package_dir):
-        key = package_name
+        key = package_name, package_dir
 
         if key not in cls.extra_scan_paths_cache:
             cls.extra_scan_paths_cache[key] = ()
 
             for plugin in getActivePlugins():
                 cls.extra_scan_paths_cache[key] += tuple(
                     cls._getPackageExtraScanPaths(
@@ -741,28 +741,29 @@
                 source_code=code,
                 is_top=False,
                 is_main=False,
                 is_extension=False,
                 is_fake=module_name,
                 hide_syntax_error=False,
             )
-        except SyntaxError:
+        except SyntaxError as e:
             plugins_logger.sysexit(
-                "SyntaxError in plugin provided source code for '%s'." % module_name
+                "SyntaxError in plugin provided source code for '%s': %s."
+                % (module_name, e)
             )
 
         if trigger_module.getCompilationMode() == "bytecode":
             trigger_module.setSourceCode(code)
 
         return trigger_module
 
     @classmethod
     def onModuleDiscovered(cls, module):
         # We offer plugins many ways to provide extra stuff
-        # pylint: disable=too-many-branches,too-many-locals,too-many-statements
+        # pylint: disable=too-many-locals,too-many-statements
 
         full_name = module.getFullName()
 
         def _untangleLoadDescription(description):
             if description and inspect.isgenerator(description):
                 description = tuple(description)
 
@@ -812,58 +813,64 @@
                     description=plugin.createPostModuleLoadCode(module)
                 )
             )
             fake_module_descriptions.extend(
                 _untangleFakeDesc(description=plugin.createFakeModuleDependency(module))
             )
 
-        if pre_module_load_descriptions:
-            total_code = []
+        def combineLoadCodes(module_load_descriptions, mode):
+            future_imports_code = []
+            normal_code_code = []
             total_flags = OrderedSet()
             reasons = []
 
-            for plugin, pre_code, reason, flags in pre_module_load_descriptions:
-                if pre_code:
+            for plugin, code, reason, flags in module_load_descriptions:
+                if code:
                     plugin.info(
-                        "Injecting pre-module load code for module '%s':" % full_name
+                        "Injecting %s-module load code for module '%s':"
+                        % (mode, full_name)
                     )
                     for line in reason.split("\n"):
                         plugin.info("    " + line)
 
-                    total_code.append(pre_code)
+                    for line in code.splitlines():
+                        line = line + "\n"
+
+                        if line.startswith("from __future__"):
+                            future_imports_code.append(line)
+                        else:
+                            normal_code_code.append(line)
+
                     total_flags.update(flags)
                     reasons.append(reason)
 
+            total_code = future_imports_code + normal_code_code
+
+            return total_code, reasons, total_flags
+
+        if pre_module_load_descriptions:
+            total_code, reasons, total_flags = combineLoadCodes(
+                module_load_descriptions=pre_module_load_descriptions, mode="pre"
+            )
+
             if total_code:
                 assert full_name not in pre_modules
 
                 pre_modules[full_name] = cls._createTriggerLoadedModule(
                     module=module,
                     trigger_name=pre_module_load_trigger_name,
                     code="\n\n".join(total_code),
                     flags=total_flags,
                 )
                 pre_modules_reasons[full_name] = tuple(reasons)
 
         if post_module_load_descriptions:
-            total_code = []
-            total_flags = OrderedSet()
-            reasons = []
-
-            for plugin, post_code, reason, flags in post_module_load_descriptions:
-                if post_code:
-                    plugin.info(
-                        "Injecting post-module load code for module '%s':" % full_name
-                    )
-                    for line in reason.split("\n"):
-                        plugin.info("    " + line)
-
-                    total_code.append(post_code)
-                    total_flags.update(flags)
-                    reasons.append(reason)
+            total_code, reasons, total_flags = combineLoadCodes(
+                module_load_descriptions=post_module_load_descriptions, mode="post"
+            )
 
             if total_code:
                 assert full_name not in post_modules
 
                 post_modules[full_name] = cls._createTriggerLoadedModule(
                     module=module,
                     trigger_name=post_module_load_trigger_name,
@@ -959,15 +966,14 @@
 
             if type(must_recurse) is not tuple and must_recurse not in (True, False):
                 plugin.sysexit(
                     "Error, onModuleEncounter code failed to return a None or tuple(bool, reason) result."
                 )
 
             if result is not None:
-                # false alarm, pylint: disable=unsubscriptable-object
                 if result[0] != must_recurse[0]:
                     plugin.sysexit(
                         "Error, decision %s does not match other plugin '%s' decision."
                         % (must_recurse[0], ".".join(deciding_plugins))
                     )
 
             deciding_plugins.append(plugin.plugin_name)
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/AntiBloatPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/AntiBloatPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/ConsiderPyLintAnnotationsPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DataFilesPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DataFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DelvewheelPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DelvewheelPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DillPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DillPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/DllFilesPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/DllFilesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/EnumPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/EnumPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/EventletPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/EventletPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GeventPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GeventPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GiPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GiPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/GlfwPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/GlfwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/ImplicitImports.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/ImplicitImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/KivyPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/KivyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/MatplotlibPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/MatplotlibPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/MultiprocessingPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/MultiprocessingPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/NumpyPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/NumpyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/OptionsNannyPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/OptionsNannyPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PbrPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PbrPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PkgResourcesPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PkgResourcesPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PmwPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PmwPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PySidePyQtPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PySidePyQtPlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,14 @@
     ]
 )
 
 os.environ["QML2_IMPORT_PATH"] = os.path.join(
     os.path.dirname(__file__),
     "qml"
 )
-
 """ % {
                 "package_name": full_name
             }
 
             yield (
                 code,
                 """\
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/PywebViewPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/PywebViewPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TensorflowPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TensorflowPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TkinterPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TkinterPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TorchPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TorchPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/TrioPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/TrioPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/UpxPlugin.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/UpxPlugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/standard.nuitka-package.config.yml` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/standard.nuitka-package.config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -199,16 +199,16 @@
         'compile': 'un-callable'
         'distutils_extension': 'un-callable'
       when: 'not use_cffi_recompiler'
 
 - module-name: 'cffi.ffiplatform'
   anti-bloat:
     - description: 'disable distutils hacks'
-      replacements:
-        'import setuptools': "'pass'"
+      replacements_plain:
+        'import setuptools': 'pass'
     - description: 'disable distutils hacks'
       change_function:
         'get_extension': 'un-callable'
         '_build': 'un-callable'
       when: 'not use_cffi_recompiler'
 
 - module-name: 'chainer'
@@ -412,17 +412,17 @@
     patterns:
       - 'distributed.yaml'
 
 - module-name: 'distributed.scheduler'
   anti-bloat:
     - description: 'remove cython support'
       # TODO: We should replace this with a nuitkarize in Cython maybe.
-      replacements:
-        'from cython import compiled': "'raise ImportError'"
-        'if compiled:': "'if False:'"
+      replacements_plain:
+        'from cython import compiled': 'raise ImportError'
+        'if compiled:': 'if False:'
 
 - module-name: 'dns.rdtypes'
   implicit-imports:
     - depends:
         - '.IN.A'
         - '.CH.A'
 
@@ -448,16 +448,16 @@
   data-files:
     patterns:
       - 'eel.js'
 
 - module-name: 'eliot._traceback'
   anti-bloat:
     - description: 'avoid useless duplication of traceback module'
-      replacements:
-        'load_module(str("_traceback_no_io"), traceback)': "'__import__(\"traceback\")'"
+      replacements_plain:
+        'load_module(str("_traceback_no_io"), traceback)': '__import__("traceback")'
 
 - module-name: 'enchant'
   data-files:
     dirs:
       - 'data'
 
 - module-name: 'engineio'
@@ -1125,31 +1125,59 @@
         "imp.find_module('pytest')": "'None'"
 
 - module-name: 'mozilla-ca'
   data-files:
     patterns:
       - '*.pem'
 
+- module-name: 'mpmath'
+  anti-bloat:
+    - description: 'remove pytest reference'
+      change_function:
+        'doctests': 'un-callable'
+        'runtests': 'un-callable'
+      when: 'not use_pytest'
+
 - module-name: 'nacl._sodium'
   implicit-imports:
     - depends:
         - '_cffi_backend'
 
 - module-name: 'networkx'
   anti-bloat:
     - description: 'remove networkx.testing usage'
       replacements_plain:
         'from networkx.testing.test import run as test': 'test = None'
 
+- module-name: 'networkx.classes.backends'
+  anti-bloat:
+    - description: 'remove pytest reference'
+      replacements_plain:
+        'os.environ.get("NETWORKX_GRAPH_CONVERT")': 'None'
+      when: 'not use_pytest'
+
 - module-name: 'networkx.utils.decorators'
   anti-bloat:
     - description: 'required for decorator compatibility'
       replacements_plain:
         'func.__defaults__ = f.__defaults__': ''
         'real_func = func.__argmap__.compile(func.__wrapped__)': 'return func'
+        '    return argmap(_not_implemented_for, 0)': |
+          #
+              import functools
+              def inner(func):
+                  @functools.wraps(func)
+                  def _not_implemented_for(g):
+                      if (mval is None or mval == g.is_multigraph()) and (
+                          dval is None or dval == g.is_directed()
+                      ):
+                          raise nx.NetworkXNotImplemented(errmsg)
+                      return func(g)
+                  return _not_implemented_for
+              return inner
 
 - module-name: 'nose.core'
   data-files:
     patterns:
       - 'usage.txt'
 
 - module-name: 'numba'
@@ -1384,14 +1412,20 @@
         - 'numpy'
 
 - module-name: 'openapi_spec_validator'
   data-files:
     dirs:
       - 'resources/schemas'
 
+- module-name: 'opentele.utils'
+  anti-bloat:
+    - description: 'workaround compiled function decorator issues'
+      replacements_plain:
+        'bases = func.__class__.__bases__': 'bases = func.__class__.__bases__ if bases != (FunctionType,) else (object,)'
+
 - module-name: 'openvino'
   data-files:
     dirs:
       - 'libs'
 
 - module-name: 'openvino.inference_engine'
   dlls:
@@ -1671,14 +1705,15 @@
 
 - module-name: 'patsy.util'
   anti-bloat:
     - description: 'remove pytest reference'
       change_function:
         'test_pandas_friendly_reshape': 'un-callable'
         'test_wide_dtype_for_and_widen': 'un-callable'
+      when: 'not use_pytest'
 
 - module-name: 'pendulum'
   data-files:
     empty_dir_structures:
       - 'locales'
 
 - module-name: 'pendulum.locales'
@@ -1879,14 +1914,19 @@
         'from ._common import NETBSD': "'NETBSD = %r' % + psutil.NETBSD"
         'from ._common import OPENBSD': "'OPENBSD = %r' % + psutil.OPENBSD"
         'from ._common import OSX': "'OSX = %r' % psutil.OSX"
         'from ._common import POSIX': "'POSIX = %r' % psutil.POSIX"
         'from ._common import SUNOS': "'SUNOS = %r' % psutil.SUNOS"
         'from ._common import WINDOWS': "'WINDOWS = %r' % psutil.WINDOWS"
 
+- module-name: 'pyarrow.lib'
+  implicit-imports:
+    - depends:
+        - 'pyarrow.vendored.version'
+
 - module-name: 'pyarrow.vendored.docscrape'
   anti-bloat:
     - description: 'remove sphinx reference'
       replacements_plain:
         "if 'sphinx' in sys.modules:": 'if False:'
     - description: 'workaround for MSVC bug with scipy docscrape 1.8.x'
       replacements_plain:
@@ -2152,15 +2192,32 @@
       - description: 'PySide2 cannot be signed unless onefile'
         macos_bundle_as_onefile: 'yes'
         when: 'macos and plugin("pyside2")'
   import-hacks:
     - find-dlls-near-module:
         - 'shiboken2'
 
-- module-name: 'PySide6'
+- module-name: 'PySide6.QtCore'
+  implicit-imports:
+    - depends:
+        - 'PySide6.support.deprecated'
+    - post-import-code:
+        - |
+          def myconnect(self, func):
+              if hasattr(func, "im_func"):
+                  if hasattr(func.im_func, "__compiled__"):
+                      myconnect._protected = getattr(myconnect, "_protected", set())
+                      myconnect._protected.add(func)
+
+              return orig_connect(self, func)
+
+          from PySide6 import QtCore
+          orig_connect = QtCore.SignalInstance.connect
+          QtCore.SignalInstance.connect = myconnect
+
   options:
     checks:
       - description: 'PySide6 is a GUI framework'
         console: 'recommend'
         when: 'plugin("pyside6")'
   import-hacks:
     - find-dlls-near-module:
@@ -3260,14 +3317,34 @@
       - 'sv.tcl'
 
 - module-name: 'swagger_ui_bundle'
   data-files:
     dirs:
       - 'vendor'
 
+- module-name: 'sympy.interactive.printing'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'import IPython': 'raise ImportError'
+        'from IPython import get_ipython': 'raise ImportError'
+        'from IPython.terminal.interactiveshell import TerminalInteractiveShell': 'raise ImportError'
+        'from IPython.frontend.terminal.interactiveshell import TerminalInteractiveShell': 'raise ImportError'
+        'from IPython.lib.latextools import latex_to_png': 'raise ImportError'
+        'from IPython.core.interactiveshell import InteractiveShell': 'raise ImportError'
+      when: 'not use_ipython'
+
+- module-name: 'sympy.interactive.session'
+  anti-bloat:
+    - description: 'remove IPython reference'
+      replacements_plain:
+        'import IPython': 'raise ImportError'
+        'from IPython import get_ipython': 'raise ImportError'
+      when: 'not use_ipython'
+
 - module-name: 'tables'
   anti-bloat:
     - description: 'remove tables.tests usage'
       replacements_plain:
         'from .tests import print_versions, test': ''
 
 - module-name: 'tables.filters'
@@ -3999,14 +4076,21 @@
 - module-name: 'trio._core._multierror'
   anti-bloat:
     - description: 'remove IPython reference'
       replacements_plain:
         '"IPython" in sys.modules': 'False'
       when: 'not use_ipython'
 
+- module-name: 'triton.compiler'
+  anti-bloat:
+    - description: 'remove setuptools usage'
+      replacements_plain:
+        'import setuptools': ''
+      when: 'not use_setuptools'
+
 - module-name: 'tzdata'
   data-files:
     dirs:
       - 'zones'
 
 - module-name: 'tzdata.zoneinfo'
   data-files:
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/stdlib2.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml` & `Nuitka-winsvc-1.5.7/nuitka/plugins/standard/stdlib3.nuitka-package.config.yml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/reports/LicenseReport.rst.j2` & `Nuitka-winsvc-1.5.7/nuitka/reports/LicenseReport.rst.j2`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/reports/Reports.py` & `Nuitka-winsvc-1.5.7/nuitka/reports/Reports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/reports/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinBytesOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinBytesOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinDictOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinDictOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinListOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinListOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinParameterSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinParameterSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinStrOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinStrOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinTypeOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinTypeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/BuiltinUnicodeOperationSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/BuiltinUnicodeOperationSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/HardImportSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/HardImportSpecs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/ParameterSpecs.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/ParameterSpecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,22 +413,22 @@
                 else:
                     message = (
                         "'%s' is an invalid keyword argument for this function"
                         % pair[0]
                     )
 
                 raise TooManyArguments(TypeError(message))
-            else:
-                if arg_index < num_pos_only:
-                    message = "'%s' is an invalid keyword argument for %s()" % (
-                        pair[0],
-                        func_name,
-                    )
 
-                    raise TooManyArguments(TypeError(message))
+            if arg_index < num_pos_only:
+                message = "'%s' is an invalid keyword argument for %s()" % (
+                    pair[0],
+                    func_name,
+                )
+
+                raise TooManyArguments(TypeError(message))
 
     if star_list_arg:
         if num_pos > num_args:
             value = positional[-(num_pos - num_args) :]
             assign(star_list_arg, value)
 
             if star_list_single_arg:
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/specs/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/Basics.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/Basics.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/commercial/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/commercial/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/DataComposer.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/DataComposer.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/data_composer/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/data_composer/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/environments/CreateEnvironment.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/environments/CreateEnvironment.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/environments/Virtualenv.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/environments/Virtualenv.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/environments/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/general/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/general/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/general/dll_report/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/general/dll_report/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/general/dll_report/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/general/dll_report/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/general/find_module/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/general/find_module/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/general/find_module/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/general/find_module/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/OnefileCompressor.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/OnefileCompressor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/onefile_compressor/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/onefile_compressor/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/profiler/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/profiler/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/scanning/DisplayPackageDLLs.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/scanning/DisplayPackageDLLs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/scanning/DisplayPackageData.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/scanning/DisplayPackageData.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/scanning/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/specialize/CTypeDescriptions.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/specialize/CTypeDescriptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/specialize/Common.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/specialize/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/specialize/SpecializeC.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/specialize/SpecializeC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/specialize/SpecializePython.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/specialize/SpecializePython.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/specialize/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/specialize/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/Common.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/Common.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/Constructs.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/Constructs.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/OutputComparison.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/OutputComparison.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/Pythons.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/Pythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/RuntimeTracing.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/RuntimeTracing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/SearchModes.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/SearchModes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/Valgrind.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/Valgrind.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/check_reference_counts/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/check_reference_counts/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/check_reference_counts/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/check_reference_counts/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/compare_with_cpython/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/compare_with_cpython/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/compare_with_cpython/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/compare_with_cpython/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/find_sxs_modules/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/find_sxs_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/find_sxs_modules/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/find_sxs_modules/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/measure_construct_performance/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/measure_construct_performance/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/measure_construct_performance/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/measure_construct_performance/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/run_nuitka_tests/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/run_nuitka_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tools/testing/run_nuitka_tests/__main__.py` & `Nuitka-winsvc-1.5.7/nuitka/tools/testing/run_nuitka_tests/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/Building.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/Building.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ComplexCallHelperFunctions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ComplexCallHelperFunctions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/Extractions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/Extractions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/InternalModule.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/InternalModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/Operations.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationAssertStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationAssertStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationAssignmentStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationAssignmentStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationBooleanExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationBooleanExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationCallExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationCallExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationClasses.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationClasses.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationClasses3.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationClasses3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationComparisonExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationComparisonExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationContractionExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationContractionExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationDictionaryCreation.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationDictionaryCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationExecStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationExecStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationForLoopStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationForLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationFunctionStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationFunctionStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationImportStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationImportStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationLambdaExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationLambdaExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationMatchStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationMatchStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationMultidist.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationMultidist.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationNamespacePackages.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationNamespacePackages.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationPrintStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationPrintStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationSequenceCreation.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationSequenceCreation.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationSubscriptExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationSubscriptExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationTryExceptStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationTryExceptStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationTryFinallyStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationTryFinallyStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationWhileLoopStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationWhileLoopStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationWithStatements.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationWithStatements.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/ReformulationYieldExpressions.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/ReformulationYieldExpressions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/SourceHandling.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/SourceHandling.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/SyntaxErrors.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/SyntaxErrors.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/TreeHelpers.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/TreeHelpers.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/VariableClosure.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/VariableClosure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/tree/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/AppDirs.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/AppDirs.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,18 @@
 import tempfile
 
 from nuitka.Tracing import general
 
 from .FileOperations import makePath
 from .Importing import importFromInlineCopy
 
-try:
+appdirs = importFromInlineCopy("appdirs", must_exist=False)
+
+if appdirs is None:
     import appdirs  # pylint: disable=I0021,import-error
-except ImportError:
-    # We handle the case without inline copy too.
-    appdirs = importFromInlineCopy("appdirs", must_exist=False)
 
 _cache_dir = None
 
 
 def getCacheDir():
     global _cache_dir  # singleton, pylint: disable=global-statement
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/CStrings.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/CStrings.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/CommandLineOptions.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/CommandLineOptions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Distributions.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Distributions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Download.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Download.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Execution.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Execution.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/FileOperations.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/FileOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Hashing.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Hashing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Images.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Images.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Importing.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Importing.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,19 @@
 
             for suffix, _mode, module_type in imp.get_suffixes():
                 if module_type == imp.C_EXTENSION:
                     _shared_library_suffixes.append(suffix)
         else:
             import importlib.machinery  # pylint: disable=I0021,import-error,no-name-in-module
 
-            _shared_library_suffixes = importlib.machinery.EXTENSION_SUFFIXES
+            _shared_library_suffixes = list(importlib.machinery.EXTENSION_SUFFIXES)
+
+        # Nuitka-Python on Windows has that
+        if "" in _shared_library_suffixes:
+            _shared_library_suffixes.remove("")
 
         _shared_library_suffixes = tuple(_shared_library_suffixes)
 
     return _shared_library_suffixes
 
 
 def getSharedLibrarySuffix(preferred):
@@ -136,15 +140,15 @@
             del sys.modules[module_name]
 
     # Temporarily add the inline path of the module to the import path.
     sys.path.insert(0, path)
 
     # Handle case without inline copy too.
     try:
-        return __import__(module_name)
+        return __import__(module_name, level=0)
     except (ImportError, SyntaxError, RuntimeError) as e:
         if not must_exist:
             return None
 
         exit_message = (
             "Error, expected inline copy of '%s' to be in '%s', error was: %r."
             % (module_name, path, e)
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/InstalledPythons.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/InstalledPythons.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/InstanceCounters.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/InstanceCounters.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Jinja2.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Jinja2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Json.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Json.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/MacOSApp.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/MacOSApp.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/MemoryUsage.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/MemoryUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/ModuleNames.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/ModuleNames.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/ReExecute.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/ReExecute.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,24 +45,24 @@
         args = list(args)
         del args[1]
 
         try:
             # Context manager is not available on all Python versions, pylint: disable=consider-using-with
             process = subprocess.Popen(args=args)
             process.communicate()
-            # No point in cleaning up, pylint: disable=protected-access
+            # No point in cleaning up, just exit the hard way.
             try:
                 os._exit(process.returncode)
             except OverflowError:
                 # Seems negative values go wrong otherwise,
                 # see https://bugs.python.org/issue28474
                 os._exit(process.returncode - 2**32)
         except KeyboardInterrupt:
             # There was a more relevant stack trace already, so abort this
-            # right here, pylint: disable=protected-access
+            # right here.
             os._exit(2)
     else:
         # The star arguments is the API of execl
         os.execl(*args)
 
 
 def reExecuteNuitka(pgo_filename):
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Rest.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Rest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/SharedLibraries.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/SharedLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Shebang.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Shebang.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Signing.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Signing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/StaticLibraries.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/StaticLibraries.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/ThreadedExecutor.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/ThreadedExecutor.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Timing.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Timing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Utils.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,14 @@
 
     return platform.release()
 
 
 def isDebianBasedLinux():
     dist_name, base, _dist_version = getLinuxDistribution()
 
-    # False alarm, pylint: disable=superfluous-parens
     return (base or dist_name) in ("Debian", "Ubuntu")
 
 
 def isFedoraBasedLinux():
     dist_name, base, _dist_version = getLinuxDistribution()
 
     return (base or dist_name) == "Fedora"
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/WindowsFileUsage.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/WindowsFileUsage.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/WindowsResources.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/WindowsResources.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/Yaml.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/Yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 what library to use for what Python. We have an inline copy of PyYAML that
 still does 2.6, on other Pythons, we expect the system to have it installed.
 
 Also we put loading for specific packages in here and a few helpers to work
 with these config files.
 """
 
+# Otherwise "Yaml" and "yaml" collide on case insensitive setups
+from __future__ import absolute_import
+
 import os
 import pkgutil
 
 from nuitka.containers.OrderedDicts import OrderedDict
 from nuitka.Options import getUserProvidedYamlFiles
 from nuitka.Tracing import general
```

### Comparing `Nuitka-winsvc-1.5.6/nuitka/utils/__init__.py` & `Nuitka-winsvc-1.5.7/nuitka/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/pyproject.toml` & `Nuitka-winsvc-1.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/setup.py` & `Nuitka-winsvc-1.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,17 +248,15 @@
 
     for type_ in "console", "gui":
         group = type_ + "_scripts"
 
         for name, _ep in dist.get_entry_map(group).items():
             script_text = runner_script_template
 
-            args = cls._get_script_args(  # pylint: disable=protected-access
-                type_, name, header, script_text
-            )
+            args = cls._get_script_args(type_, name, header, script_text)
             for res in args:
                 yield res
 
 
 try:
     easy_install.ScriptWriter.get_args = get_args
 except AttributeError:
```

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/AssertsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/AssertsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/AssignmentsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/AssignmentsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/AssignmentsTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/AssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/BranchingTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/BranchingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/BuiltinOverload.py` & `Nuitka-winsvc-1.5.7/tests/basics/BuiltinOverload.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/BuiltinSuperTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/BuiltinSuperTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/BuiltinsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/BuiltinsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ClassMinimalTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ClassMinimalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ClassesTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ClassesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ClassesTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/ClassesTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ClassesTest34.py` & `Nuitka-winsvc-1.5.7/tests/basics/ClassesTest34.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ComparisonChainsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ComparisonChainsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ConstantsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ConstantsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ConstantsTest27.py` & `Nuitka-winsvc-1.5.7/tests/basics/ConstantsTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/DecoratorsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/DecoratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/DefaultParametersTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/DefaultParametersTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/DoubleDeletionsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/DoubleDeletionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/EmptyModuleTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/EmptyModuleTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ExceptionRaisingTest33.py` & `Nuitka-winsvc-1.5.7/tests/basics/ExceptionRaisingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ExecEvalTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ExecEvalTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ExtremeClosureTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ExtremeClosureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/FunctionObjectsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/FunctionObjectsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/FunctionsTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/FunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/FutureTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/FutureTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/GeneratorExpressionsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/GeneratorExpressionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/GeneratorExpressionsTest_37.py` & `Nuitka-winsvc-1.5.7/tests/basics/GeneratorExpressionsTest_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/GlobalStatementTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/GlobalStatementTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/HelloWorldTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/HelloWorldTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ImportingTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ImportingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/InplaceOperationsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/InplaceOperationsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/InspectionTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/InspectionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/InspectionTest_35.py` & `Nuitka-winsvc-1.5.7/tests/basics/InspectionTest_35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/InspectionTest_36.py` & `Nuitka-winsvc-1.5.7/tests/basics/InspectionTest_36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/LambdasTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/LambdasTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/LateClosureAssignmentTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/LateClosureAssignmentTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ListContractionsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ListContractionsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/LoopingTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/LoopingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/MainProgramsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/MainProgramsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ModuleAttributesTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ModuleAttributesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/OperatorsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/OperatorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/OrderChecksTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/OrderChecksTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/OrderChecksTest27.py` & `Nuitka-winsvc-1.5.7/tests/basics/OrderChecksTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/OverflowFunctionsTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/OverflowFunctionsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ParameterErrorsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ParameterErrorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ParameterErrorsTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/ParameterErrorsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/PrintFutureTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/PrintFutureTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/PrintingTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/PrintingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/RecursionTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/RecursionTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest27.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest27.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest33.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest35.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest36.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ReferencingTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/ReferencingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/SlotsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/SlotsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/ThreadedGeneratorsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/ThreadedGeneratorsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest32.py` & `Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest35.py` & `Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TrickAssignmentsTest_2.py` & `Nuitka-winsvc-1.5.7/tests/basics/TrickAssignmentsTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryContinueFinallyTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryContinueFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryExceptContinueTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryExceptContinueTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryExceptFinallyTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryExceptFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryExceptFramesTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryExceptFramesTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryReturnFinallyTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryReturnFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/TryYieldFinallyTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/TryYieldFinallyTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/UnicodeTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/UnicodeTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/UnpackingTest35.py` & `Nuitka-winsvc-1.5.7/tests/basics/UnpackingTest35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/VarargsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/VarargsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/WithStatementsTest.py` & `Nuitka-winsvc-1.5.7/tests/basics/WithStatementsTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/YieldFromTest33.py` & `Nuitka-winsvc-1.5.7/tests/basics/YieldFromTest33.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/run_all.py` & `Nuitka-winsvc-1.5.7/tests/basics/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/basics/run_xml.py` & `Nuitka-winsvc-1.5.7/tests/basics/run_xml.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/onefile/HelloWorldTest.py` & `Nuitka-winsvc-1.5.7/tests/onefile/HelloWorldTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/onefile/KeyboardInterruptTest.py` & `Nuitka-winsvc-1.5.7/tests/onefile/KeyboardInterruptTest.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/onefile/run_all.py` & `Nuitka-winsvc-1.5.7/tests/onefile/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/ArgumentTypes.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/ArgumentTypes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Attributes.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Attributes.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Calls.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Calls.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Conditions.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Conditions.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/DecodingOperations.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/DecodingOperations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/FormatStrings36.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/FormatStrings36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/HardImports.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/HardImports.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/HardImports_2.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/HardImports_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Iterations.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Iterations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Len.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Len.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Operations.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Operations.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/Subscripts.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/Subscripts.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/optimizations/run_all.py` & `Nuitka-winsvc-1.5.7/tests/optimizations/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py` & `Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/PackageImportSuccessAfterFailure.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py` & `Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/variable_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/package_import_success_after_failure/variable_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/packages/package_import_success_after_failure/variable_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/run_all.py` & `Nuitka-winsvc-1.5.7/tests/packages/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/__init__.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/bigkitty.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/bigkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/smallkitty.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/smallkitty.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/__init__.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/hello.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/hello.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/miau.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/miau.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/sub_package/kitty/speak/purr.py` & `Nuitka-winsvc-1.5.7/tests/packages/sub_package/kitty/speak/purr.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/packages/top_level_attributes_3/some_package/some_module.py` & `Nuitka-winsvc-1.5.7/tests/packages/top_level_attributes_3/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/plugins/data_files/DataFilesMain.py` & `Nuitka-winsvc-1.5.7/tests/plugins/data_files/DataFilesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/plugins/data_files/data_files_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/plugins/data_files/data_files_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/plugins/parameters/ParametersMain.py` & `Nuitka-winsvc-1.5.7/tests/plugins/parameters/ParametersMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/plugins/parameters/parameter-using-plugin.py` & `Nuitka-winsvc-1.5.7/tests/plugins/parameters/parameter-using-plugin.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/plugins/run_all.py` & `Nuitka-winsvc-1.5.7/tests/plugins/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/absolute_import/AbsoluteImportMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/absolute_import/AbsoluteImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/foobar.py` & `Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/foobar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/local.py` & `Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/absolute_import/foobar/util.py` & `Nuitka-winsvc-1.5.7/tests/programs/absolute_import/foobar/util.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports1/CasedImportingMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports1/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/Some_Module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/some_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports1/path2/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports1/path2/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports2/CasedImportingMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports2/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/some_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path1/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path1/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/Some_Module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports2/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports2/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports3/CasedImportingMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports3/CasedImportingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/Some_Module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path1/Some_Package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path1/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/Some_Module.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/Some_Module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/case_imports3/path2/Some_Package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/case_imports3/path2/Some_Package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/CyclicImportsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/CyclicImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py` & `Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py` & `Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/cyclic_imports/cyclic_importing_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dash_import/DashImportMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/dash_import/DashImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dash_import/dash-module.py` & `Nuitka-winsvc-1.5.7/tests/programs/dash_import/dash-module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dash_import/plus+module.py` & `Nuitka-winsvc-1.5.7/tests/programs/dash_import/plus+module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dash_main/Dash-Main.py` & `Nuitka-winsvc-1.5.7/tests/programs/dash_main/Dash-Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/DeepProgramMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/DeepProgramMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/DeepBrother.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/DeepBrother.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/DeepChild.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/DeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/deep_package/DeepDeepChild.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/deep_package/DeepDeepChild.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/deep/some_package/deep_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/deep/some_package/deep_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/DunderInitImportsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/DunderInitImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/package/SubModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/package/SubModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/dunderinit_imports/package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/dunderinit_imports/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/import_variants/ImportVariationsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/import_variants/ImportVariationsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child1.py` & `Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child2.py` & `Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/Child3.py` & `Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/Child3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/import_variants/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/import_variants/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/main_raises/ErrorMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/main_raises/ErrorMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/main_raises/ErrorRaising.py` & `Nuitka-winsvc-1.5.7/tests/programs/main_raises/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/main_raises2/ErrorInFunctionMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/main_raises2/ErrorInFunctionMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/main_raises2/ErrorRaising.py` & `Nuitka-winsvc-1.5.7/tests/programs/main_raises2/ErrorRaising.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/ModuleAttributesMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/ModuleAttributesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/Nearby1.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/Nearby1.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/Nearby2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/Nearby3.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_attributes/package_level1/package_level2/package_level3/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_exits/ErrorExitingModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_exits/ErrorExitingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_exits/Main.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_exits/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_object_replacing/ModuleObjectReplacingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/module_object_replacing/SelfReplacingModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/module_object_replacing/SelfReplacingModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/MultiprocessingUsingMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/__main__.py` & `Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/multiprocessing_using/foo/entry.py` & `Nuitka-winsvc-1.5.7/tests/programs/multiprocessing_using/foo/entry.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/named_imports/NamedImportsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/named_imports/NamedImportsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/SomeModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/named_imports/some_package/sub_package/SomeModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/named_imports/some_package/sub_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_code/PackageInitCodeMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_code/PackageInitCodeMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_code/some_package/SomeModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_code/some_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_code/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_code/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/PackageContainsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/PackageContainsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_contains_main/local.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_contains_main/local.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_import/PackageInitImportMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_import/PackageInitImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_import/some_package/PackageLocal.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_import/some_package/PackageLocal.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_import/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/PackageInitIssueMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/PackageInitIssueMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/child_package/SomeModule.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/child_package/SomeModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_init_issue/some_package/child_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_init_issue/some_package/child_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/PackageMissingInitMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/PackageMissingInitMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/some_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_missing_init/some_package/sub_package/some_sub_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/PackageAndModuleNamedSameMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/Something/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/Something/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_module_collision/something.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_module_collision/something.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_overload/Main.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_overload/Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/bar.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/bar.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_overload/foo/bar2.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_overload/foo/bar2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/PackagePreventsSubmoduleMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_prevents_submodule/some_package/some_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_prevents_submodule/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_program/PackageAsMain/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_program/PackageAsMain/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/package_program/PackageAsMain/__main__.py` & `Nuitka-winsvc-1.5.7/tests/programs/package_program/PackageAsMain/__main__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/PkgUtilIterModulesMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleC.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/SomeModuleD.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package1/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleA.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/SomeModuleB.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_itermodules/some_package/sub_package2/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/PkgUtilUsageMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/PkgUtilUsageMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/pkgutil_usage/package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/pkgutil_usage/package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/plugin_import/PluginImportMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/plugin_import/PluginImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/plugin_import/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/plugin_import/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/plugin_import/some_package/some_module.py` & `Nuitka-winsvc-1.5.7/tests/programs/plugin_import/some_package/some_module.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/reimport_main_dynamic/ImportItselfDynamicMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/reimport_main_static/ImportItselfStaticMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/reimport_main_static/ImportItselfStaticMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/relative_import/RelativeImportMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/relative_import/RelativeImportMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/relative_import/dircache.py` & `Nuitka-winsvc-1.5.7/tests/programs/relative_import/dircache.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/ResourceReaderMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/ResourceReaderMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/resource_reader37/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/resource_reader37/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/run_all.py` & `Nuitka-winsvc-1.5.7/tests/programs/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/StdlibOverloadMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/StdlibOverloadMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/pyexpat.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/__init__.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/__init__.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/normal_importing.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/normal_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/pyexpat.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/pyexpat.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/stdlib_overload/some_package/star_importing.py` & `Nuitka-winsvc-1.5.7/tests/programs/stdlib_overload/some_package/star_importing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/IndentationErroring.py` & `Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/IndentationErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/SyntaxErroring.py` & `Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/SyntaxErroring.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/syntax_errors/SyntaxErrorsMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/syntax_errors/SyntaxErrorsMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/unicode_bom/UnicodeBomMain.py` & `Nuitka-winsvc-1.5.7/tests/programs/unicode_bom/UnicodeBomMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/unicode_bom/unicode_bom.py` & `Nuitka-winsvc-1.5.7/tests/programs/unicode_bom/unicode_bom.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/programs/with space/Space Main.py` & `Nuitka-winsvc-1.5.7/tests/programs/with space/Space Main.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/reflected/compile_itself.py` & `Nuitka-winsvc-1.5.7/tests/reflected/compile_itself.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/run-tests` & `Nuitka-winsvc-1.5.7/tests/run-tests`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/BrotliUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/BrotliUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/CtypesUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/CtypesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/FlaskUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/FlaskUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/GlfwUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/GlfwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/GtkUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/GtkUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/HexEncodingTest_2.py` & `Nuitka-winsvc-1.5.7/tests/standalone/HexEncodingTest_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/IdnaUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/IdnaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/LxmlUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/LxmlUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/MatplotlibUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/MatplotlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/MetadataPackagesUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/MetadataPackagesUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/NumpyUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/NumpyUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/OpenGLUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/OpenGLUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PandasUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PandasUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PasslibUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PasslibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PendulumUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PendulumUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PkgResourcesRequiresUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PkgResourcesRequiresUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PmwUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PmwUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PyQt5Plugins.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PyQt5Plugins.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PyQt5SSLSupport.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PyQt5SSLSupport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PyQt5Using.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PyQt5Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PyQt6Using.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PyQt6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/PySide6Using.py` & `Nuitka-winsvc-1.5.7/tests/standalone/PySide6Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/RsaUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/RsaUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/ShlibUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/ShlibUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/SocketUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/SocketUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/TkInterUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/TkInterUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/Urllib3Using.py` & `Nuitka-winsvc-1.5.7/tests/standalone/Urllib3Using.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/Win32ComUsing.py` & `Nuitka-winsvc-1.5.7/tests/standalone/Win32ComUsing.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/run_all.py` & `Nuitka-winsvc-1.5.7/tests/standalone/run_all.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/standalone/zip_importer/ZipImporterMain.py` & `Nuitka-winsvc-1.5.7/tests/standalone/zip_importer/ZipImporterMain.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/AsyncgenReturn36.py` & `Nuitka-winsvc-1.5.7/tests/syntax/AsyncgenReturn36.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/BreakWithoutLoop.py` & `Nuitka-winsvc-1.5.7/tests/syntax/BreakWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/ClassReturn.py` & `Nuitka-winsvc-1.5.7/tests/syntax/ClassReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/ClosureDel_2.py` & `Nuitka-winsvc-1.5.7/tests/syntax/ClosureDel_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/ContinueWithoutLoop.py` & `Nuitka-winsvc-1.5.7/tests/syntax/ContinueWithoutLoop.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/DuplicateArgument.py` & `Nuitka-winsvc-1.5.7/tests/syntax/DuplicateArgument.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/ExecWithNesting_2.py` & `Nuitka-winsvc-1.5.7/tests/syntax/ExecWithNesting_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/FutureBraces.py` & `Nuitka-winsvc-1.5.7/tests/syntax/FutureBraces.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/FutureUnknown.py` & `Nuitka-winsvc-1.5.7/tests/syntax/FutureUnknown.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/GeneratorExpressions38.py` & `Nuitka-winsvc-1.5.7/tests/syntax/GeneratorExpressions38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/GeneratorReturn_2.py` & `Nuitka-winsvc-1.5.7/tests/syntax/GeneratorReturn_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/GlobalForParameter.py` & `Nuitka-winsvc-1.5.7/tests/syntax/GlobalForParameter.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/Importing32.py` & `Nuitka-winsvc-1.5.7/tests/syntax/Importing32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/IndentationError.py` & `Nuitka-winsvc-1.5.7/tests/syntax/IndentationError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/LateFutureImport.py` & `Nuitka-winsvc-1.5.7/tests/syntax/LateFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/MisplacedFutureImport.py` & `Nuitka-winsvc-1.5.7/tests/syntax/MisplacedFutureImport.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/ModuleReturn.py` & `Nuitka-winsvc-1.5.7/tests/syntax/ModuleReturn.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/NonAsciiWithoutEncoding_2.py` & `Nuitka-winsvc-1.5.7/tests/syntax/NonAsciiWithoutEncoding_2.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/NonlocalForParameter32.py` & `Nuitka-winsvc-1.5.7/tests/syntax/NonlocalForParameter32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/NonlocalNotFound32.py` & `Nuitka-winsvc-1.5.7/tests/syntax/NonlocalNotFound32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/StarImportExtra.py` & `Nuitka-winsvc-1.5.7/tests/syntax/StarImportExtra.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/SyntaxError.py` & `Nuitka-winsvc-1.5.7/tests/syntax/SyntaxError.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/TryExceptAllNotLast.py` & `Nuitka-winsvc-1.5.7/tests/syntax/TryExceptAllNotLast.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/TryFinallyContinue_37.py` & `Nuitka-winsvc-1.5.7/tests/syntax/TryFinallyContinue_37.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/UnpackNoTuple.py` & `Nuitka-winsvc-1.5.7/tests/syntax/UnpackNoTuple.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/UnpackTwoStars32.py` & `Nuitka-winsvc-1.5.7/tests/syntax/UnpackTwoStars32.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/YieldFromInModule.py` & `Nuitka-winsvc-1.5.7/tests/syntax/YieldFromInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/YieldInAsync35.py` & `Nuitka-winsvc-1.5.7/tests/syntax/YieldInAsync35.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/YieldInGenexp38.py` & `Nuitka-winsvc-1.5.7/tests/syntax/YieldInGenexp38.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/YieldInModule.py` & `Nuitka-winsvc-1.5.7/tests/syntax/YieldInModule.py`

 * *Files identical despite different names*

### Comparing `Nuitka-winsvc-1.5.6/tests/syntax/run_all.py` & `Nuitka-winsvc-1.5.7/tests/syntax/run_all.py`

 * *Files identical despite different names*

