# Comparing `tmp/types-Pillow-9.5.0.1.tar.gz` & `tmp/types-Pillow-9.5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Pillow-9.5.0.1.tar", last modified: Mon Apr 17 12:30:45 2023, max compression
+gzip compressed data, was "types-Pillow-9.5.0.2.tar", last modified: Wed Apr 26 18:18:47 2023, max compression
```

## Comparing `types-Pillow-9.5.0.1.tar` & `types-Pillow-9.5.0.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/PIL-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BdfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BlpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BmpImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/BufrStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ContainerIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/CurImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/DcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/DdsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/EpsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ExifTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FitsStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FliImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FpxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/FtexImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GbrImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GdImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GifImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GimpGradientFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GimpPaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/GribStubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Hdf5StubImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IcnsImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IcoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11469 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageChops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageCms.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageColor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageDraw2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageEnhance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFilter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageFont.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageGrab.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageMorph.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageOps.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImagePalette.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImagePath.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageQt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageSequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageShow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageStat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageTk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageTransform.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImageWin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/ImtImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/IptcImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/Jpeg2KImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/JpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/JpegPresets.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/PIL-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/McIdasImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MicImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MpegImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MpoImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/MspImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PSDraw.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PaletteFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PalmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcfFontFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PcxImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PdfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PdfParser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PixarImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PngImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PsdImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/PyAccess.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SgiImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SpiderImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/SunImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TarIO.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TgaImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TiffImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/TiffTags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WalImageFile.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WebPImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/WmfImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XVThumbImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XbmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/XpmImagePlugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_imaging.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_tkinter_finder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-17 12:30:30.000000 types-Pillow-9.5.0.1/PIL-stubs/features.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-17 12:30:44.000000 types-Pillow-9.5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 12:30:45.848385 types-Pillow-9.5.0.1/types_Pillow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-17 12:30:45.000000 types-Pillow-9.5.0.1/types_Pillow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/PIL-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BdfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BlpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BmpImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/BufrStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ContainerIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/CurImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/DcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/DdsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/EpsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ExifTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FitsStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FliImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FpxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/FtexImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GbrImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GdImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GifImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GimpGradientFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GimpPaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/GribStubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Hdf5StubImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IcnsImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IcoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageChops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageCms.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageColor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageDraw2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageEnhance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFilter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageFont.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageGrab.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageMorph.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageOps.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImagePalette.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImagePath.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageQt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageSequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageShow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageStat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageTk.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageTransform.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImageWin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/ImtImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/IptcImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/Jpeg2KImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/JpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/JpegPresets.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/PIL-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/McIdasImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MicImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MpegImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MpoImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/MspImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PSDraw.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PaletteFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PalmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcfFontFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PcxImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PdfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PdfParser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PixarImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PngImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PsdImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/PyAccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SgiImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SpiderImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/SunImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TarIO.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TgaImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TiffImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/TiffTags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WalImageFile.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WebPImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/WmfImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XVThumbImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XbmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/XpmImagePlugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_imaging.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_tkinter_finder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-26 18:18:26.000000 types-Pillow-9.5.0.2/PIL-stubs/features.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-26 18:18:43.000000 types-Pillow-9.5.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:18:47.026572 types-Pillow-9.5.0.2/types_Pillow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 18:18:46.000000 types-Pillow-9.5.0.2/types_Pillow.egg-info/top_level.txt
```

### Comparing `types-Pillow-9.5.0.1/CHANGELOG.md` & `types-Pillow-9.5.0.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 9.5.0.2 (2023-04-26)
+
+Add a return type for `PIL.Image.load` (#9466)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 9.5.0.1 (2023-04-17)
 
 [Pillow] Add Base and GPS enums in PIL.ExifTags (#10051)
 
 ## 9.5.0.0 (2023-04-14)
 
 Bump Pillow to 9.5.* (#10046)
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/BlpImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/BlpImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/DdsImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/DdsImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/EpsImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/EpsImagePlugin.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
+from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 split: Any
 field: Any
 gs_windows_binary: Any
 
 def has_ghostscript(): ...
@@ -20,9 +21,9 @@
 class EpsImageFile(ImageFile):
     format: ClassVar[Literal["EPS"]]
     format_description: ClassVar[str]
     mode_map: Any
     im: Any
     mode: Any
     tile: Any
-    def load(self, scale: int = 1, transparency: bool = False) -> None: ...
+    def load(self, scale: int = 1, transparency: bool = False) -> _PixelAccessor: ...
     def load_seek(self, *args, **kwargs) -> None: ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ExifTags.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ExifTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/FpxImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/FpxImagePlugin.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from _typeshed import Incomplete
 from typing import Any, ClassVar
 from typing_extensions import Literal, TypeAlias
 
+from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 _OleFileIO: TypeAlias = Any  # olefile.OleFileIO
 _OleStream: TypeAlias = Any  # olefile.OleStream
 
 MODES: dict[tuple[int, ...], tuple[str, str]]
 
@@ -15,8 +16,8 @@
     format_description: ClassVar[str]
     fp: _OleStream | None
     maxid: int
     rawmode: str
     jpeg: dict[int, Incomplete]
     tile_prefix: Incomplete
     stream: list[str]
-    def load(self): ...
+    def load(self) -> _PixelAccessor: ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/GifImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/GifImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/IcnsImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/IcnsImagePlugin.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from _typeshed import Incomplete
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
+from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 enable_jpeg2k: Any
 HEADERSIZE: int
 
 def nextheader(fobj): ...
 def read_32t(fobj, start_length, size): ...
@@ -29,8 +30,8 @@
     @property
     def size(self): ...
     @size.setter
     def size(self, value) -> None: ...
     best_size: Any
     im: Any
     mode: Any
-    def load(self) -> None: ...
+    def load(self) -> _PixelAccessor: ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/IcoImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/IcoImagePlugin.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
+from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 class IcoFile:
     buf: Any
     entry: Any
     nb_items: Any
     def __init__(self, buf): ...
@@ -18,9 +19,9 @@
     format_description: ClassVar[str]
     @property
     def size(self): ...
     @size.setter
     def size(self, value) -> None: ...
     im: Any
     mode: Any
-    def load(self) -> None: ...
+    def load(self) -> _PixelAccessor: ...
     def load_seek(self) -> None: ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/Image.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/Image.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from ._imaging import (
     DEFAULT_STRATEGY as DEFAULT_STRATEGY,
     FILTERED as FILTERED,
     FIXED as FIXED,
     HUFFMAN_ONLY as HUFFMAN_ONLY,
     RLE as RLE,
+    _PixelAccessor,
 )
 from .ImageFilter import Filter
 from .ImagePalette import ImagePalette
 
 _Mode: TypeAlias = str
 _Resample: TypeAlias = Literal[0, 1, 2, 3, 4, 5]
 _Size: TypeAlias = tuple[int, int]
@@ -176,15 +177,15 @@
     def close(self) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __getstate__(self) -> _ImageState: ...
     def __setstate__(self, state: _ImageState) -> None: ...
     def tobytes(self, encoder_name: str = "raw", *args) -> bytes: ...
     def tobitmap(self, name: str = "image") -> bytes: ...
     def frombytes(self, data: bytes, decoder_name: str = "raw", *args) -> None: ...
-    def load(self) -> None: ...
+    def load(self) -> _PixelAccessor: ...
     def verify(self) -> None: ...
     def convert(
         self,
         mode: _Mode | None = None,
         matrix: _ConversionMatrix | None = None,
         dither: int | None = None,
         palette: Palette | Literal[0, 1] = ...,
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageChops.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageChops.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageCms.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageCms.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageDraw.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageDraw2.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageDraw2.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageEnhance.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageEnhance.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageFile.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageFile.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from _typeshed import Incomplete, Unused
 from typing import Any, NoReturn
 from typing_extensions import Self
 
+from ._imaging import _PixelAccessor
 from .Image import Image
 
 MAXBLOCK: int
 SAFEBLOCK: Any
 LOAD_TRUNCATED_IMAGES: bool
 ERRORS: Any
 
@@ -20,20 +21,20 @@
     fp: Any
     filename: Any
     def __init__(self, fp: Incomplete | None = None, filename: Incomplete | None = None) -> None: ...
     def get_format_mimetype(self): ...
     def verify(self) -> None: ...
     map: Any
     im: Any
-    def load(self): ...
+    def load(self) -> _PixelAccessor: ...
     def load_prepare(self) -> None: ...
     def load_end(self) -> None: ...
 
 class StubImageFile(ImageFile):
-    def load(self) -> None: ...
+    def load(self) -> _PixelAccessor: ...
 
 class Parser:
     incremental: Incomplete | None
     image: Incomplete | None
     data: Incomplete | None
     decoder: Incomplete | None
     offset: int
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageFilter.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageFilter.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageFont.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageFont.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageMath.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageMath.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageMorph.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageMorph.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageOps.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageOps.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImagePalette.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImagePalette.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageQt.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageQt.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageShow.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageShow.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageTk.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageTk.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/ImageWin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/ImageWin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/JpegImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/JpegImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/MicImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/MicImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/PSDraw.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/PSDraw.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/PdfParser.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/PdfParser.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/PngImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/PngImagePlugin.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     def seek(self, frame) -> None: ...
     def tell(self): ...
     decoderconfig: Any
     def load_prepare(self) -> None: ...
     def load_read(self, read_bytes): ...
     png: Any
     im: Any
-    pyaccess: Any
     def load_end(self) -> None: ...
     def getexif(self): ...
 
 def putchunk(fp, cid, *data) -> None: ...
 
 class _idat:
     fp: Any
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/PyAccess.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/PyAccess.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from logging import Logger
 from typing import Any
 
+from PIL._imaging import _PixelAccessor
+
 ffi: Any
 logger: Logger
 
-class PyAccess:
+class PyAccess(_PixelAccessor):
     readonly: Any
     image8: Any
     image32: Any
     image: Any
     def __init__(self, img, readonly: bool = False) -> None: ...
-    def __setitem__(self, xy, color) -> None: ...
-    def __getitem__(self, xy): ...
-    putpixel: Any
-    getpixel: Any
-    def check_xy(self, xy): ...
+    def __setitem__(self, xy: tuple[int, int], color) -> None: ...
+    def __getitem__(self, xy: tuple[int, int]) -> Any: ...
+    def putpixel(self, xy: tuple[int, int], color) -> None: ...
+    def getpixel(self, xy: tuple[int, int]) -> Any: ...
+    def check_xy(self, xy: tuple[int, int]): ...
 
 class _PyAccess32_2(PyAccess):
     def get_pixel(self, x, y): ...
     def set_pixel(self, x, y, color) -> None: ...
 
 class _PyAccess32_3(PyAccess):
     def get_pixel(self, x, y): ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/SpiderImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/SpiderImagePlugin.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/TiffImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/TiffImagePlugin.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from _typeshed import Incomplete
 from collections.abc import MutableMapping
 from numbers import Rational
 from types import TracebackType
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
+from ._imaging import _PixelAccessor
 from .ImageFile import ImageFile
 
 logger: Any
 READ_LIBTIFF: bool
 WRITE_LIBTIFF: bool
 IFD_LEGACY_API: bool
 II: bytes
@@ -149,15 +150,15 @@
     tag: Any
     def __init__(self, fp: Incomplete | None = None, filename: Incomplete | None = None) -> None: ...
     @property
     def n_frames(self): ...
     im: Any
     def seek(self, frame) -> None: ...
     def tell(self): ...
-    def load(self): ...
+    def load(self) -> _PixelAccessor: ...
     def load_end(self) -> None: ...
 
 SAVE_INFO: Any
 
 class AppendingTiffWriter:
     fieldSizes: Any
     Tags: Any
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/TiffTags.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/TiffTags.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/WmfImagePlugin.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/WmfImagePlugin.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 from _typeshed import Incomplete
 from typing import Any, ClassVar
 from typing_extensions import Literal
 
+from ._imaging import _PixelAccessor
 from .ImageFile import StubImageFile
 
 def register_handler(handler) -> None: ...
 
 if sys.platform == "win32":
     class WmfHandler:
         bbox: Any
         def open(self, im) -> None: ...
         def load(self, im): ...
 
 class WmfStubImageFile(StubImageFile):
     format: ClassVar[Literal["WMF"]]
     format_description: ClassVar[str]
-    def load(self, dpi: Incomplete | None = None) -> None: ...
+    def load(self, dpi: Incomplete | None = None) -> _PixelAccessor: ...
```

### Comparing `types-Pillow-9.5.0.1/PIL-stubs/features.pyi` & `types-Pillow-9.5.0.2/PIL-stubs/features.pyi`

 * *Files identical despite different names*

### Comparing `types-Pillow-9.5.0.1/PKG-INFO` & `types-Pillow-9.5.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.1
+Version: 9.5.0.2
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
```

### Comparing `types-Pillow-9.5.0.1/setup.py` & `types-Pillow-9.5.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
 '''.lstrip()
 
 setup(name=name,
-      version="9.5.0.1",
+      version="9.5.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md",
```

### Comparing `types-Pillow-9.5.0.1/types_Pillow.egg-info/PKG-INFO` & `types-Pillow-9.5.0.2/types_Pillow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Pillow
-Version: 9.5.0.1
+Version: 9.5.0.2
 Summary: Typing stubs for Pillow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Pillow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Pillow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Pillow. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fd188fa67e404350873c736bd45335fcf601548a`.
+This package was generated from typeshed commit `f7443a748e87e1bf4ab675b3d0a56f0ba44a21ce`.
```

### Comparing `types-Pillow-9.5.0.1/types_Pillow.egg-info/SOURCES.txt` & `types-Pillow-9.5.0.2/types_Pillow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

