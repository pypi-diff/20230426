# Comparing `tmp/propeller_design_tools-0.2.8.tar.gz` & `tmp/propeller_design_tools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\tmpe4uek2hs\propeller_design_tools-0.2.8.tar", last modified: Sat Apr 23 18:17:03 2022, max compression
+gzip compressed data, was "C:\Users\Jake\Desktop\Python Projects\propeller_design_tools\dist\tmp_sa74nkw\propeller_design_tools-0.2.9.tar", last modified: Mon Apr 25 20:26:39 2022, max compression
```

## Comparing `propeller_design_tools-0.2.8.tar` & `propeller_design_tools-0.2.9.tar`

### file list

```diff
@@ -1,373 +1,373 @@
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/
--rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7509 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     6611 2022-04-17 04:09:33.000000 propeller_design_tools-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/
--rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.2.8/propeller_design_tools/__init__.py
--rw-rw-rw-   0        0        0    28138 2022-04-15 17:59:25.000000 propeller_design_tools-0.2.8/propeller_design_tools/airfoil.py
--rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.2.8/propeller_design_tools/custom_opengl_classes.py
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag35.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag36.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag37.dat
--rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag38.dat
--rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/arad13.dat
--rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/boe103.dat
--rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/boe106.dat
--rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/clarky.dat
--rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/e855.dat
--rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/hs1606.dat
--rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/mrc-16.dat
--rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_database/xfoil.exe
--rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.2.8/propeller_design_tools/foil_ui_classes.py
--rw-rw-rw-   0        0        0    49655 2022-04-22 04:19:36.000000 propeller_design_tools-0.2.8/propeller_design_tools/funcs.py
--rw-rw-rw-   0        0        0    17857 2022-04-22 04:30:30.000000 propeller_design_tools-0.2.8/propeller_design_tools/helper_ui_classes.py
--rw-rw-rw-   0        0        0    16262 2022-04-17 06:29:47.000000 propeller_design_tools-0.2.8/propeller_design_tools/helper_ui_subclasses.py
--rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.2.8/propeller_design_tools/opt_ui_classes.py
--rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.2.8/propeller_design_tools/optimizations.py
--rw-rw-rw-   0        0        0     9478 2022-04-22 04:38:40.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_analysis_ui_classes.py
--rw-rw-rw-   0        0        0    36995 2022-04-22 17:46:35.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_creation_ui_classes.py
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/
--rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
--rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
--rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
--rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
--rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
--rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
--rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
--rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
--rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
--rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
--rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
--rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
--rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
--rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
--rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
--rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
--rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
--rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
--rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
--rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
--rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
--rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/station_polars/
--rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/
--rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
--rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/station_polars/
--rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/
--rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
--rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
--rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
--rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
--rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
--rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
--rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
--rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
--rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
--rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
--rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
--rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
--rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
--rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
--rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
--rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
--rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
--rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
--rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
--rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/station_polars/
--rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
--rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.2.8/propeller_design_tools/prop_database/xrotor.exe
--rw-rw-rw-   0        0        0    52956 2022-04-22 04:03:02.000000 propeller_design_tools-0.2.8/propeller_design_tools/propeller.py
--rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.2.8/propeller_design_tools/radialstation.py
--rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.2.8/propeller_design_tools/science_spinbox_class.py
--rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.2.8/propeller_design_tools/settings.py
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/
--rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/crosshair_cursor.png
--rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot1.wav
--rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot2.wav
--rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot3.wav
--rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot4.wav
--rw-rw-rw-   0        0        0      236 2022-04-22 17:46:46.000000 propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/user-settings.txt
--rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.2.8/propeller_design_tools/user_interface.py
--rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.2.8/propeller_design_tools/user_io.py
-drwxrwxrwx   0        0        0        0 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools.egg-info/
--rw-rw-rw-   0        0        0     7509 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    26612 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2022-04-23 18:17:02.000000 propeller_design_tools-0.2.8/propeller_design_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.2.8/pyproject.toml
--rw-rw-rw-   0        0        0     1021 2022-04-23 18:17:03.000000 propeller_design_tools-0.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/
+-rw-rw-rw-   0        0        0    35801 2021-08-21 05:57:07.000000 propeller_design_tools-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     1405 2022-04-23 18:14:56.000000 propeller_design_tools-0.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7509 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6611 2022-04-17 04:09:33.000000 propeller_design_tools-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/
+-rw-rw-rw-   0        0        0      479 2022-04-06 00:00:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/__init__.py
+-rw-rw-rw-   0        0        0    28138 2022-04-15 17:59:25.000000 propeller_design_tools-0.2.9/propeller_design_tools/airfoil.py
+-rw-rw-rw-   0        0        0     4871 2022-04-17 06:33:40.000000 propeller_design_tools-0.2.9/propeller_design_tools/custom_opengl_classes.py
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:13:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag35.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:01.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag36.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:08.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag37.dat
+-rw-rw-rw-   0        0        0     4866 2022-03-27 20:14:18.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag38.dat
+-rw-rw-rw-   0        0        0     1132 2021-10-24 06:54:37.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/arad13.dat
+-rw-rw-rw-   0        0        0      816 2022-04-21 23:31:48.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe103.dat
+-rw-rw-rw-   0        0        0      794 2022-04-21 23:06:50.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe106.dat
+-rw-rw-rw-   0        0        0     2730 2021-02-07 20:57:01.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/clarky.dat
+-rw-rw-rw-   0        0        0     1520 2021-10-24 06:55:45.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/e855.dat
+-rw-rw-rw-   0        0        0     2778 2022-03-17 04:23:04.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/hs1606.dat
+-rw-rw-rw-   0        0        0     2768 2021-10-24 06:48:49.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/mrc-16.dat
+-rwxrwxrwx   0        0        0  1002125 2021-01-30 20:37:44.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_database/xfoil.exe
+-rw-rw-rw-   0        0        0    18378 2022-04-21 23:06:28.000000 propeller_design_tools-0.2.9/propeller_design_tools/foil_ui_classes.py
+-rw-rw-rw-   0        0        0    49655 2022-04-22 04:19:36.000000 propeller_design_tools-0.2.9/propeller_design_tools/funcs.py
+-rw-rw-rw-   0        0        0    17861 2022-04-25 18:38:28.000000 propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_classes.py
+-rw-rw-rw-   0        0        0    16262 2022-04-17 06:29:47.000000 propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_subclasses.py
+-rw-rw-rw-   0        0        0      401 2022-03-18 16:03:32.000000 propeller_design_tools-0.2.9/propeller_design_tools/opt_ui_classes.py
+-rw-rw-rw-   0        0        0    11040 2022-04-07 18:47:57.000000 propeller_design_tools-0.2.9/propeller_design_tools/optimizations.py
+-rw-rw-rw-   0        0        0    15622 2022-04-25 20:19:25.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_analysis_ui_classes.py
+-rw-rw-rw-   0        0        0    36995 2022-04-22 17:46:35.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_creation_ui_classes.py
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/
+-rw-rw-rw-   0        0        0    25993 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta
+-rw-rw-rw-   0        0        0     8599 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop
+-rw-rw-rw-   0        0        0     6239 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt
+-rw-rw-rw-   0        0        0     3827 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt
+-rw-rw-rw-   0        0        0     3828 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3804 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3805 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3807 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3806 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt
+-rw-rw-rw-   0        0        0     3808 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt
+-rw-rw-rw-   0        0        0     3809 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt
+-rw-rw-rw-   0        0        0     3810 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3812 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt
+-rw-rw-rw-   0        0        0     3813 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt
+-rw-rw-rw-   0        0        0     3814 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt
+-rw-rw-rw-   0        0        0     3815 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt
+-rw-rw-rw-   0        0        0     3816 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt
+-rw-rw-rw-   0        0        0     3817 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt
+-rw-rw-rw-   0        0        0     3819 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt
+-rw-rw-rw-   0        0        0     3821 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt
+-rw-rw-rw-   0        0        0     3822 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt
+-rw-rw-rw-   0        0        0     3829 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt
+-rw-rw-rw-   0        0        0     3832 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt
+-rw-rw-rw-   0        0        0     3802 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt
+-rw-rw-rw-   0        0        0     3803 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt
+-rw-rw-rw-   0        0        0     3831 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt
+-rw-rw-rw-   0        0        0     3830 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/
+-rw-rw-rw-   0        0        0     4595 2022-04-22 17:47:43.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/
+-rw-rw-rw-   0        0        0    13191 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta
+-rw-rw-rw-   0        0        0     4923 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     2064 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     2062 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     2063 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     2065 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     2066 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/
+-rw-rw-rw-   0        0        0     5160 2022-04-22 04:32:00.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/
+-rw-rw-rw-   0        0        0    13630 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta
+-rw-rw-rw-   0        0        0     4875 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop
+-rw-rw-rw-   0        0        0     3593 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt
+-rw-rw-rw-   0        0        0     3765 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt
+-rw-rw-rw-   0        0        0     3770 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt
+-rw-rw-rw-   0        0        0     3771 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt
+-rw-rw-rw-   0        0        0     3774 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt
+-rw-rw-rw-   0        0        0     3775 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt
+-rw-rw-rw-   0        0        0     3777 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt
+-rw-rw-rw-   0        0        0     3778 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt
+-rw-rw-rw-   0        0        0     3781 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt
+-rw-rw-rw-   0        0        0     3769 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt
+-rw-rw-rw-   0        0        0     3784 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt
+-rw-rw-rw-   0        0        0     3795 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt
+-rw-rw-rw-   0        0        0     3794 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt
+-rw-rw-rw-   0        0        0     3768 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt
+-rw-rw-rw-   0        0        0     3793 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt
+-rw-rw-rw-   0        0        0     3792 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt
+-rw-rw-rw-   0        0        0     3767 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt
+-rw-rw-rw-   0        0        0     3766 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/
+-rw-rw-rw-   0        0        0     6152 2022-04-22 04:32:46.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar
+-rwxrwxrwx   0        0        0  1176521 2021-01-30 22:15:06.000000 propeller_design_tools-0.2.9/propeller_design_tools/prop_database/xrotor.exe
+-rw-rw-rw-   0        0        0    53754 2022-04-25 20:17:44.000000 propeller_design_tools-0.2.9/propeller_design_tools/propeller.py
+-rw-rw-rw-   0        0        0    17617 2022-04-22 04:16:32.000000 propeller_design_tools-0.2.9/propeller_design_tools/radialstation.py
+-rw-rw-rw-   0        0        0     1674 2022-03-17 22:38:26.000000 propeller_design_tools-0.2.9/propeller_design_tools/science_spinbox_class.py
+-rw-rw-rw-   0        0        0     4111 2022-04-10 23:06:53.000000 propeller_design_tools-0.2.9/propeller_design_tools/settings.py
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/
+-rw-rw-rw-   0        0        0     1358 2022-03-17 07:01:27.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/crosshair_cursor.png
+-rw-rw-rw-   0        0        0    10192 2022-03-18 16:44:10.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot1.wav
+-rw-rw-rw-   0        0        0    18704 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot2.wav
+-rw-rw-rw-   0        0        0    23984 2022-03-18 16:44:09.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot3.wav
+-rw-rw-rw-   0        0        0    24784 2022-03-18 16:44:11.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot4.wav
+-rw-rw-rw-   0        0        0      236 2022-04-25 20:19:27.000000 propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/user-settings.txt
+-rw-rw-rw-   0        0        0     5857 2022-04-22 04:28:14.000000 propeller_design_tools-0.2.9/propeller_design_tools/user_interface.py
+-rw-rw-rw-   0        0        0     2839 2022-03-11 21:49:52.000000 propeller_design_tools-0.2.9/propeller_design_tools/user_io.py
+drwxrwxrwx   0        0        0        0 2022-04-25 20:26:38.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/
+-rw-rw-rw-   0        0        0     7509 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    26612 2022-04-25 20:26:37.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2022-04-25 20:26:36.000000 propeller_design_tools-0.2.9/propeller_design_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      274 2022-04-10 09:00:21.000000 propeller_design_tools-0.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1021 2022-04-25 20:26:39.000000 propeller_design_tools-0.2.9/setup.cfg
```

### Comparing `propeller_design_tools-0.2.8/LICENSE` & `propeller_design_tools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/MANIFEST.in` & `propeller_design_tools-0.2.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/PKG-INFO` & `propeller_design_tools-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller_design_tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
 Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Author: Jacob Bronson
 Author-email: jakebronson89@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
 Platform: UNKNOWN
```

### Comparing `propeller_design_tools-0.2.8/README.md` & `propeller_design_tools-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/airfoil.py` & `propeller_design_tools-0.2.9/propeller_design_tools/airfoil.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/custom_opengl_classes.py` & `propeller_design_tools-0.2.9/propeller_design_tools/custom_opengl_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag35.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag35.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag36.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag36.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag37.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag37.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/ag38.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/ag38.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/arad13.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/arad13.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/boe103.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe103.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/boe106.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/boe106.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/clarky.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/clarky.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/e855.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/e855.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/hs1606.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/hs1606.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/mrc-16.dat` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/mrc-16.dat`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_database/xfoil.exe` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_database/xfoil.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/foil_ui_classes.py` & `propeller_design_tools-0.2.9/propeller_design_tools/foil_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/funcs.py` & `propeller_design_tools-0.2.9/propeller_design_tools/funcs.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/helper_ui_classes.py` & `propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,15 @@
 
         lay.addWidget(self.left_box)
         lay.addWidget(PDT_Label('->', font_size=12))
         lay.addWidget(self.right_box)
         lay.addWidget(PDT_Label('by'))
 
         if spin_double_science == 'double':
-            self.step_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=[0, 10],
+            self.step_box = PDT_DoubleSpinBox(font_size=12, width=80, box_range=[0, np.inf],
                                               box_single_step=0.01, default_str=self.step_default)
         elif spin_double_science == 'spin':
             self.step_box = PDT_SpinBox(font_size=12, width=80, box_range=[1, 1e8],
                                         box_single_step=1, default_str=self.step_default)
         else:  # spin_double_science == 'science'
             self.step_box = PDT_ScienceSpinBox(font_size=12, width=80, default_str=self.step_default, box_range=[1e3, 1e9])
```

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/helper_ui_subclasses.py` & `propeller_design_tools-0.2.9/propeller_design_tools/helper_ui_subclasses.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/optimizations.py` & `propeller_design_tools-0.2.9/propeller_design_tools/optimizations.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_analysis_ui_classes.py` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_analysis_ui_classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import numpy as np
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-import pyqtgraph as pg
 import pyqtgraph.opengl as gl
 from propeller_design_tools.settings import VALID_OPER_PLOT_PARAMS
 from propeller_design_tools.funcs import get_all_propeller_dirs
 from propeller_design_tools.propeller import Propeller
 try:
     from PyQt5 import QtWidgets, QtCore
     from propeller_design_tools.helper_ui_subclasses import PDT_Label, PDT_GroupBox, PDT_ComboBox, PDT_PushButton, \
         PDT_CheckBox
     from propeller_design_tools.helper_ui_classes import SingleAxCanvas, PropellerCreationPanelCanvas, \
-        CheckColumnWidget, AxesComboBoxWidget
+        CheckColumnWidget, AxesComboBoxWidget, RangeLineEditWidget, Capturing
 except:
     pass
 
 
 class PropellerSweepWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
         super(PropellerSweepWidget, self).__init__()
@@ -23,41 +23,74 @@
         center_lay = QtWidgets.QVBoxLayout()
         left_lay = QtWidgets.QVBoxLayout()
         main_lay.addLayout(left_lay)
         main_lay.addLayout(center_lay)
 
         # left
         self.select_prop_widg = select_prop_widg = PropellerSweepSelectPropWidget(main_win=main_win)
+        select_prop_widg.selectedPropChanged.connect(self.propeller_changed)
         left_lay.addWidget(select_prop_widg)
 
         # center layout
         center_lay.addStretch()
-        self.exist_data_widg = exist_data_widg = CheckColumnWidget(title='Existing Data (plot controls)', title_font_size=14,
+        self.exist_data_widg = exist_data_widg = CheckColumnWidget(title='Existing Data (plot controls):', title_font_size=14,
                                                                    title_bold=True)
         center_lay.addWidget(exist_data_widg)
         center_lay.addStretch()
-        add_data_grp = PDT_GroupBox('Add Data Points By Range')
-        add_data_grp.setMinimumSize(400, 250)
-        add_data_grp.setLayout(QtWidgets.QVBoxLayout())
-        center_lay.addWidget(add_data_grp)
+        self.add_data_widg = add_data_widg = PropellerSweepAddDataWidget(main_win=main_win)
+        add_data_widg.dataChanged.connect(self.add_data_widg_data_changed)
+        center_lay.addWidget(add_data_widg)
         center_lay.addStretch()
 
         # right layout
         self.metric_plot_widget = PropellerSweepMetricPlotWidget(main_win=main_win)
         main_lay.addWidget(self.metric_plot_widget)
 
         # connecting those signals
         self.exist_data_widg.checkboxClicked.connect(self.metric_plot_widget.update_data)
 
     @property
     def prop(self):
         return self.select_prop_widg.prop
 
+    def add_data_widg_data_changed(self):
+        self.update_exist_data_widg()
+        self.update_plot_widg()
+
+    def propeller_changed(self):
+        self.update_exist_data_widg()
+        self.update_plot_widg()
+
+    def update_plot_widg(self):
+        self.metric_plot_widget.update_data()
+
+    def update_exist_data_widg(self):
+        self.exist_data_widg.clear()
+
+        if self.prop is None:
+            return
+
+        if len(self.prop.oper_data) == 0:
+            return
+
+        params = self.prop.oper_data.get_swept_params()
+        if len(params) == 0:
+            return
+
+        self.exist_data_widg.col_groups = params
+        for param in params:
+            uniq_vals = self.prop.oper_data.get_unique_param(param=param)
+            for val in uniq_vals:
+                self.exist_data_widg.add_checkbox(lbl='{}'.format(val), colname=param, chkd=True)
+
 
 class PropellerSweepSelectPropWidget(QtWidgets.QWidget):
+
+    selectedPropChanged = QtCore.pyqtSignal()
+
     def __init__(self, main_win: 'InterfaceMainWindow'):
         super(PropellerSweepSelectPropWidget, self).__init__()
         self.main_win = main_win
         self.prop = None
 
         layout = QtWidgets.QVBoxLayout()
         self.setLayout(layout)
@@ -70,89 +103,180 @@
         top_lay.addStretch()
         top_lay.addWidget(PDT_Label('Select Propeller:', font_size=14, bold=True))
         top_lay.addWidget(select_prop_cb)
         top_lay.addStretch()
         layout.addLayout(top_lay)
 
         layout.addStretch()
-        grp = PDT_GroupBox('Velocity Vectors', width=200)
-        grp_lay = QtWidgets.QVBoxLayout()
-        grp.setLayout(grp_lay)
-        self.tot_vel_chk = tot_vel_chk = PDT_CheckBox('Total')
-        tot_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        grp_lay.addWidget(tot_vel_chk)
-        self.ax_vel_chk = ax_vel_chk = PDT_CheckBox('Axial (thrust)')
-        ax_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        grp_lay.addWidget(ax_vel_chk)
-        self.tan_vel_chk = tan_vel_chk = PDT_CheckBox('Tangential (swirl)')
-        tan_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
-        grp_lay.addWidget(tan_vel_chk)
-        layout.addWidget(grp)
-        layout.setAlignment(grp, QtCore.Qt.AlignHCenter)
+        self.vel_vec_widg = vel_vec_widg = VelocityVectorWidget()
+        vel_vec_widg.checkboxClicked.connect(self.vel_vec_chk_clicked)
+        layout.addWidget(vel_vec_widg)
+        layout.setAlignment(vel_vec_widg, QtCore.Qt.AlignHCenter)
 
         layout.addStretch()
         bot_lay = QtWidgets.QHBoxLayout()
         bot_lay.addStretch()
         self.wvel_3d_view = wvel_3d_view = gl.GLViewWidget()
         wvel_3d_view.setFixedSize(450, 450)
         bot_lay.addWidget(wvel_3d_view)
         bot_lay.addStretch()
         layout.addLayout(bot_lay)
         layout.addStretch()
 
-    def tot_ax_tan_chk_clicked(self):
+    def vel_vec_chk_clicked(self):
         center = self.wvel_3d_view.opts['center']
         distance = self.wvel_3d_view.opts['distance']
         elevation = self.wvel_3d_view.opts['elevation']
         azimuth = self.wvel_3d_view.opts['azimuth']
 
         self.plot_prop_wvel()
         self.wvel_3d_view.setCameraPosition(pos=center, distance=distance, elevation=elevation, azimuth=azimuth)
 
     def pop_select_prop_cb(self):
         self.select_prop_cb.clear()
         item_txts = ['None'] + get_all_propeller_dirs()
         self.select_prop_cb.addItems(item_txts)
 
     def select_prop_cb_changed(self):
-        self.main_win.prop_sweep_widg.exist_data_widg.clear()
-        if self.select_prop_cb.currentText().strip() == '':
-            return
-
         if self.select_prop_cb.currentText() == 'None':
             self.prop = None
             self.wvel_3d_view.clear()
-            self.main_win.prop_sweep_widg.metric_plot_widget.axes.clear()
-            self.main_win.prop_sweep_widg.metric_plot_widget.plot_canvas.draw()
         else:
             self.prop = Propeller(self.select_prop_cb.currentText())
             self.plot_prop_wvel()
-            self.main_win.prop_sweep_widg.metric_plot_widget.update_data()
-
-            if len(self.prop.oper_data) == 0:
-                return
-
-            params = self.prop.oper_data.get_swept_params()
-            if len(params) == 0:
-                return
 
-            self.main_win.prop_sweep_widg.exist_data_widg.col_groups = params
-            for param in params:
-                uniq_vals = self.prop.oper_data.get_unique_param(param=param)
-                for val in uniq_vals:
-                    self.main_win.prop_sweep_widg.exist_data_widg.add_checkbox(lbl='{}'.format(val), colname=param, chkd=True)
+        self.selectedPropChanged.emit()
 
     def plot_prop_wvel(self):
         self.wvel_3d_view.clear()
-        total = self.tot_vel_chk.isChecked()
-        axial = self.ax_vel_chk.isChecked()
-        tang = self.tan_vel_chk.isChecked()
+        total = self.vel_vec_widg.tot_vel_chk.isChecked()
+        axial = self.vel_vec_widg.ax_vel_chk.isChecked()
+        tang = self.vel_vec_widg.tan_vel_chk.isChecked()
         self.prop.plot_gl3d_wvel_data(total=total, axial=axial, tangential=tang, view=self.wvel_3d_view)
 
 
+class VelocityVectorWidget(PDT_GroupBox):
+
+    checkboxClicked = QtCore.pyqtSignal()
+
+    def __init__(self):
+        super(VelocityVectorWidget, self).__init__('Velocity Vectors', width=200)
+
+        lay = QtWidgets.QHBoxLayout()
+        self.setLayout(lay)
+        lay.addStretch()
+
+        self.pt_select_lay = pt_select_lay = QtWidgets.QVBoxLayout()
+        lay.addLayout(pt_select_lay)
+        lay.addStretch()
+
+        velvec_lay = QtWidgets.QVBoxLayout()
+        self.tot_vel_chk = tot_vel_chk = PDT_CheckBox('Total')
+        tot_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(tot_vel_chk)
+        self.ax_vel_chk = ax_vel_chk = PDT_CheckBox('Axial (thrust)')
+        ax_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(ax_vel_chk)
+        self.tan_vel_chk = tan_vel_chk = PDT_CheckBox('Tangential (swirl)')
+        tan_vel_chk.clicked.connect(self.tot_ax_tan_chk_clicked)
+        velvec_lay.addWidget(tan_vel_chk)
+        lay.addLayout(velvec_lay)
+        lay.addStretch()
+
+    def tot_ax_tan_chk_clicked(self):
+        self.checkboxClicked.emit()
+
+    def pop_pt_select_lay(self):
+        pass
+
+
+class PropellerSweepAddDataWidget(QtWidgets.QWidget):
+
+    dataChanged = QtCore.pyqtSignal()
+
+    def __init__(self, main_win: 'InterfaceMainWindow'):
+        super(PropellerSweepAddDataWidget, self).__init__()
+        self.main_win = main_win
+
+        lay = QtWidgets.QVBoxLayout()
+        self.setLayout(lay)
+        lay.addWidget(PDT_Label('Add Data Points By Range:', font_size=14, bold=True))
+
+        opts_lay = QtWidgets.QFormLayout()
+        self.vorform_cb = vorform_cb = PDT_ComboBox(width=150)
+        vorform_cb.addItems(['grad', 'pot', 'vrtx'])
+        vorform_cb.setCurrentIndex(1)
+        opts_lay.addRow(PDT_Label('Vortex Formulation:', font_size=12), vorform_cb)
+        self.vel_rle = vel_rle = RangeLineEditWidget(box_range=[0, 1000], box_single_step=1,
+                                                      default_strs=['5.0', '30.0', '5.0'], spin_double_science='double')
+        opts_lay.addRow(PDT_Label('Speeds:', font_size=12), vel_rle)
+        self.valid_sweep_params = ['adva', 'rpm', 'thrust', 'power', 'torque']
+        self.sweep_param_cb = sweep_param_cb = PDT_ComboBox(width=150)
+        sweep_param_cb.addItems(self.valid_sweep_params)
+        opts_lay.addRow(PDT_Label('Sweep Param:', font_size=12), sweep_param_cb)
+        self.sweep_vals_rle = sweep_vals_rle = RangeLineEditWidget(box_range=[0, np.Inf], box_single_step=1,
+                                                                   default_strs=['0.1', '1.0', '0.1'],
+                                                                   spin_double_science='double')
+        opts_lay.addRow(PDT_Label('Sweep Values:', font_size=12), sweep_vals_rle)
+        lay.addLayout(opts_lay)
+
+        self.add_btn = add_btn = PDT_PushButton('Sweep (overwrites)', font_size=12, width=150)
+        add_btn.clicked.connect(self.add_btn_clicked)
+        lay.addWidget(add_btn)
+
+    @property
+    def prop(self):
+        return self.main_win.prop_sweep_widg.prop
+
+    def add_btn_clicked(self):
+        min_vel, max_vel, vel_step = self.vel_rle.get_start_stop_step()
+        velos = list(np.arange(min_vel, max_vel, vel_step))
+        param = self.sweep_param_cb.currentText()
+        min_val, max_val, val_step = self.sweep_vals_rle.get_start_stop_step()
+        vals = list(np.arange(min_val, max_val, val_step))
+        vor = self.vorform_cb.currentText()
+
+        if self.prop is None:
+            msgbox = QtWidgets.QMessageBox()
+            msgbox.about(self, 'Error', 'Must Select a Propeller() first!')
+            return
+
+        self.prop.clear_sweep_data()
+        self.thread = QtCore.QThread()
+        self.prop_sweep_worker = PropellerSweepWorker(prop=self.prop, velos=velos, param2sweep=param, sweep_vals=vals,
+                                                      vorform=vor)
+        self.prop_sweep_worker.moveToThread(self.thread)
+        self.thread.started.connect(self.prop_sweep_worker.run)
+        self.prop_sweep_worker.finished.connect(self.thread.quit)
+        self.prop_sweep_worker.finished.connect(self.prop_sweep_worker.deleteLater)
+        self.prop_sweep_worker.finished.connect(self.on_sweep_worker_finish)
+        self.thread.finished.connect(self.thread.deleteLater)
+        self.prop_sweep_worker.progress.connect(self.update_sweep_worker_progress)
+
+        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(False)
+        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(False)
+        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(False)
+        self.setEnabled(False)
+        self.thread.start()
+
+    def on_sweep_worker_finish(self):
+        self.main_win.prop_sweep_widg.exist_data_widg.setEnabled(True)
+        self.main_win.prop_sweep_widg.metric_plot_widget.setEnabled(True)
+        self.main_win.prop_sweep_widg.select_prop_widg.vel_vec_widg.setEnabled(True)
+        self.setEnabled(True)
+        self.main_win.prog_bar.setValue(0)
+        self.dataChanged.emit()
+
+    def update_sweep_worker_progress(self, pcnt: float, strs: list):
+        if pcnt is not None and isinstance(pcnt, float):
+            self.main_win.prog_bar.setValue(pcnt)
+        if strs is not None and isinstance(strs, list):
+            self.main_win.print(strs)
+
+
 class PropellerSweepMetricPlotWidget(QtWidgets.QWidget):
     def __init__(self, main_win: 'InterfaceMainWindow'):
         self.main_win = main_win
         super(PropellerSweepMetricPlotWidget, self).__init__()
         main_lay = QtWidgets.QVBoxLayout()
         self.setLayout(main_lay)
         self.creation_panel_canvas = None
@@ -194,35 +318,59 @@
         self.axes = self.plot_canvas.axes
         main_lay.addWidget(self.plot_canvas)
         toolbar = NavigationToolbar(self.plot_canvas, self)
         main_lay.addWidget(toolbar)
         main_lay.setAlignment(toolbar, QtCore.Qt.AlignHCenter)
         main_lay.addStretch()
 
+    @property
+    def prop(self):
+        return self.main_win.prop_sweep_widg.prop
+
     def update_data(self, *args):
         self.plot_canvas.clear_axes()
 
-        yax_txt = self.yax_cb.currentText()
-        xax_txt = self.xax_cb.currentText()
-        if yax_txt == 'y-axis' or xax_txt == 'x-axis':
-            return
-        prop = self.main_win.prop_sweep_widg.prop
-        if prop is None:
-            return
+        if self.prop is not None:
+            yax_txt = self.yax_cb.currentText()
+            xax_txt = self.xax_cb.currentText()
+            if yax_txt == 'y-axis' or xax_txt == 'x-axis':
+                return
+            prop = self.main_win.prop_sweep_widg.prop
+            if prop is None:
+                return
 
-        fam_txt = self.fam_cb.currentText()
-        if fam_txt.lower() == 'none':
-            fam_txt = None
-
-        iso_txt = self.iso_cb.currentText()
-        if iso_txt.lower() == 'none':
-            iso_txt = None
-
-        # need to filter out the unchecked boxes and not plot that data
-        if len(args) > 0:
-            print(isinstance(args[0], dict))
-            print(args[0])
+            fam_txt = self.fam_cb.currentText()
+            if fam_txt.lower() == 'none':
+                fam_txt = None
+
+            iso_txt = self.iso_cb.currentText()
+            if iso_txt.lower() == 'none':
+                iso_txt = None
+
+            # need to filter out the unchecked boxes and not plot that data
+            if len(args) > 0:
+                print(isinstance(args[0], dict))
+                print(args[0])
 
-        prop.oper_data.plot(x_param=xax_txt, y_param=yax_txt, family_param=fam_txt, iso_param=iso_txt,
-                            fig=self.plot_canvas.figure)
+            prop.oper_data.plot(x_param=xax_txt, y_param=yax_txt, family_param=fam_txt, iso_param=iso_txt,
+                                fig=self.plot_canvas.figure)
 
         self.plot_canvas.draw()
+
+
+class PropellerSweepWorker(QtCore.QObject):
+
+    progress = QtCore.pyqtSignal(object, object)
+    finished = QtCore.pyqtSignal()
+
+    def __init__(self, prop: Propeller, velos: list, param2sweep: str, sweep_vals: list, vorform: str):
+        super(PropellerSweepWorker, self).__init__()
+        self.prop = prop
+        self.velos = velos
+        self.param2sweep = param2sweep
+        self.sweep_vals = sweep_vals
+        self.vorform = vorform
+
+    def run(self):
+        self.prop.analyze_sweep(velo_vals=self.velos, sweep_param=self.param2sweep, sweep_vals=self.sweep_vals,
+                                verbose=True, xrotor_verbose=False, vorform=self.vorform, prog_signal=self.progress)
+        self.finished.emit()
```

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_creation_ui_classes.py` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_creation_ui_classes.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/MyPropeller.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_100.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_101.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_102.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_103.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_104.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_105.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_106.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_107.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_108.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_109.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_110.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_111.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_112.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_113.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_114.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_115.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_116.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_117.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_118.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_119.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_120.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_121.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_122.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_123.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_124.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_125.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_126.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_127.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_128.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_129.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_130.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_131.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_132.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_133.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_134.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_135.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_136.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_137.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_138.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_139.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_140.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_141.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_142.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_143.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_144.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_145.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_146.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_147.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_148.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_149.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_150.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_151.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_152.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_153.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_154.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_155.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_156.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_157.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_158.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_159.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_160.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_161.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_162.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_163.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_164.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_165.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_166.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_167.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_168.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_169.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_170.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_171.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_172.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_173.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_174.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_175.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_176.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_177.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_178.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_179.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_180.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_181.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_182.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_183.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_184.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_185.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_186.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_187.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_188.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_189.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_190.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_191.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_192.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_193.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_194.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_195.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_196.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_197.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_198.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_199.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_50.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_51.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_52.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_53.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_54.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_55.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_56.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_57.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_58.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_59.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_60.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_61.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_62.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_63.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_64.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_65.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_66.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_67.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_68.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_69.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_70.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_71.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_72.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_73.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_74.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_75.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_76.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_77.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_78.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_79.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_80.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_81.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_82.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_83.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_84.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_85.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_86.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_87.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_88.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_89.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_90.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_91.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_92.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_93.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_94.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_95.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_96.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_97.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_98.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/blade_profiles/profile_99.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller/station_polars/0.75_clarky.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/MyPropeller2.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller2/station_polars/0.75_e855.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.meta`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrop`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/MyPropeller3.xrr`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_0.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_1.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_10.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_11.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_12.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_13.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_14.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_15.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_16.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_17.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_18.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_19.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_2.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_20.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_21.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_22.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_23.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_24.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_25.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_26.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_27.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_28.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_29.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_3.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_30.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_31.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_32.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_33.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_34.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_35.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_36.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_37.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_38.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_39.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_4.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_40.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_41.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_42.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_43.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_44.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_45.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_46.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_47.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_48.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_49.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_5.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_6.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_7.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_8.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/blade_profiles/profile_9.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/MyPropeller3/station_polars/0.75_mrc-16.dat.polar`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/prop_database/xrotor.exe` & `propeller_design_tools-0.2.9/propeller_design_tools/prop_database/xrotor.exe`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/propeller.py` & `propeller_design_tools-0.2.9/propeller_design_tools/propeller.py`

 * *Files 2% similar despite different names*

```diff
@@ -962,40 +962,55 @@
     def analyze_operating_point(self, velo: float = None, adva: float = None, rpm: float = None, thrust: float = None,
                                 power: float = None, torque: float = None, xrotor_verbose: bool = False):
 
         funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=self.design_vorform, adva=adva, rpm=rpm, thrust=thrust,
                               torque=torque, power=power, velo=velo, xrotor_verbose=xrotor_verbose)
 
     def analyze_sweep(self, velo_vals: list, sweep_param: str, sweep_vals: list, verbose: bool = True,
-                      xrotor_verbose: bool = False, vorform: str = None):
+                      xrotor_verbose: bool = False, vorform: str = None, prog_signal=None):
         if sweep_param not in ['adva', 'rpm', 'thrust', 'power', 'torque']:
             raise Error('"sweep_param" must be one of ("adva", "rpm", "thrust", "power", "torque")')
 
         vorform = self.design_vorform if vorform is None else vorform
 
         total_pnts = len(velo_vals) * len(sweep_vals)
         if verbose:
-            Info('Analyzing "{}" across a sweep of {} operating points'.format(self.name, total_pnts))
+            info_str = 'Analyzing "{}" across a sweep of {} operating points'.format(self.name, total_pnts)
+            if prog_signal is not None:
+                prog_signal.emit(0, [info_str])
+            else:
+                Info(info_str)
         count = 0
         for velo_val in velo_vals:
             for v, val in enumerate(sweep_vals):
                 count += 1
                 if verbose:
-                    Info('Analyzing sweep point # {} / {}'.format(count, total_pnts))
+                    info_str = 'Analyzing sweep point # {} / {}'.format(count, total_pnts)
+                    if prog_signal is not None:
+                        prog_signal.emit(count / total_pnts * 100, [info_str])
+                    else:
+                        Info(info_str)
                 try:
-                    funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=vorform, velo=velo_val,
+                    funcs.run_xrotor_oper(xrr_file=self.xrr_file, vorform=vorform, velo=velo_val, verbose=False,
                                           xrotor_verbose=xrotor_verbose, **{sweep_param: val})
                 except Error as e:
-                    Warning('Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param, val, e))
-                    pass
+                    warn_str = 'Failed to get XROTOR oper results for vel={}, {}={}\n{}'.format(velo_val, sweep_param, val, e)
+                    if prog_signal is not None:
+                        prog_signal.emit(None, [warn_str])
+                    else:
+                        Warning(warn_str)
+                        pass
 
         self.oper_data.load_oper_sweep_results()
         self.wvel_data.load_wvel_sweep_results()
         if verbose:
-            Info('Done!')
+            if prog_signal is not None:
+                prog_signal.emit(0, 'Done!')
+            else:
+                Info('Done!')
 
     def clear_sweep_data(self):
         if os.path.exists(self.oper_data_dir):
             shutil.rmtree(self.oper_data_dir)
             Info('Removed {} and its contents'.format(self.oper_data_dir))
         if os.path.exists(self.wvel_data_dir):
             shutil.rmtree(self.wvel_data_dir)
@@ -1010,20 +1025,23 @@
 
     def __len__(self):
         return len(self.datapoints)
 
     def get_swept_params(self):
         valid_params = VALID_OPER_PLOT_PARAMS
         swept_params = []
+        avoid_params = []
         for param in valid_params:
             for dp in self.datapoints.values():
                 if param not in swept_params:
                     pts = self.get_datapoints_by_paramval(param=param, val=dp[param])
-                    if len(pts) > 2 and len(pts) < len(self.datapoints):
+                    if 2 < len(pts) < len(self.datapoints) and param not in avoid_params:
                         swept_params.append(param)
+                    else:
+                        avoid_params.append(param)
 
         return swept_params
 
     def get_oper_files(self, fullpath: bool = True):
         if os.path.exists(self.directory):
             if fullpath:
                 return [os.path.join(self.directory, name) for name in os.listdir(self.directory) if name.endswith('.oper')]
```

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/radialstation.py` & `propeller_design_tools-0.2.9/propeller_design_tools/radialstation.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/science_spinbox_class.py` & `propeller_design_tools-0.2.9/propeller_design_tools/science_spinbox_class.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/settings.py` & `propeller_design_tools-0.2.9/propeller_design_tools/settings.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/crosshair_cursor.png` & `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/crosshair_cursor.png`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot1.wav` & `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot1.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot2.wav` & `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot2.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot3.wav` & `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot3.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/supporting_files/gunshot4.wav` & `propeller_design_tools-0.2.9/propeller_design_tools/supporting_files/gunshot4.wav`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/user_interface.py` & `propeller_design_tools-0.2.9/propeller_design_tools/user_interface.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools/user_io.py` & `propeller_design_tools-0.2.9/propeller_design_tools/user_io.py`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools.egg-info/PKG-INFO` & `propeller_design_tools-0.2.9/propeller_design_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: propeller-design-tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools, for propeller design (automates usage of XFOIL and XROTOR executables).
 Home-page: https://github.com/helloDestroyerOfWorlds/propeller_design_tools.git
 Author: Jacob Bronson
 Author-email: jakebronson89@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/helloDestroyerOfWorlds/propeller_design_tools/issues
 Platform: UNKNOWN
```

### Comparing `propeller_design_tools-0.2.8/propeller_design_tools.egg-info/SOURCES.txt` & `propeller_design_tools-0.2.9/propeller_design_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `propeller_design_tools-0.2.8/setup.cfg` & `propeller_design_tools-0.2.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 726f 7065 6c6c 6572 5f64 6573   = propeller_des
 00000020: 6967 6e5f 746f 6f6c 730d 0a76 6572 7369  ign_tools..versi
-00000030: 6f6e 203d 2030 2e32 2e38 0d0a 6175 7468  on = 0.2.8..auth
+00000030: 6f6e 203d 2030 2e32 2e39 0d0a 6175 7468  on = 0.2.9..auth
 00000040: 6f72 203d 204a 6163 6f62 2042 726f 6e73  or = Jacob Brons
 00000050: 6f6e 0d0a 6175 7468 6f72 5f65 6d61 696c  on..author_email
 00000060: 203d 206a 616b 6562 726f 6e73 6f6e 3839   = jakebronson89
 00000070: 4067 6d61 696c 2e63 6f6d 0d0a 6465 7363  @gmail.com..desc
 00000080: 7269 7074 696f 6e20 3d20 546f 6f6c 732c  ription = Tools,
 00000090: 2066 6f72 2070 726f 7065 6c6c 6572 2064   for propeller d
 000000a0: 6573 6967 6e20 2861 7574 6f6d 6174 6573  esign (automates
```

