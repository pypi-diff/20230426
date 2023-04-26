# Comparing `tmp/adafruit-circuitpython-imageload-1.17.0.tar.gz` & `tmp/adafruit-circuitpython-imageload-1.17.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-imageload-1.17.0.tar", last modified: Mon Jan  9 15:16:06 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-imageload-1.17.1.tar", last modified: Tue Apr 25 23:21:38 2023, max compression
```

## Comparing `adafruit-circuitpython-imageload-1.17.0.tar` & `adafruit-circuitpython-imageload-1.17.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.398582 adafruit-circuitpython-imageload-1.17.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.382582 adafruit-circuitpython-imageload-1.17.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.386582 adafruit-circuitpython-imageload-1.17.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.386582 adafruit-circuitpython-imageload-1.17.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.386582 adafruit-circuitpython-imageload-1.17.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-01-09 15:16:06.398582 adafruit-circuitpython-imageload-1.17.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.386582 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-01-09 15:16:06.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-01-09 15:16:06.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 15:16:06.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-09 15:16:06.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-09 15:16:06.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.386582 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9850 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/indexed.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/negative_height_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/displayio_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/png.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pbm_ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pbm_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/ppm_ascii.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/ppm_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/tilegrid_inflator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/developing.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.390582 adafruit-circuitpython-imageload-1.17.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_colorwheel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_from_web.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_netpbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_png_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/examples/imageload_tilegrid_inflator_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.394582 adafruit-circuitpython-imageload-1.17.0/examples/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/1bit-not-byte-aligned.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/1bit-not-byte-aligned.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/1bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/1bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/2bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/2bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/4bit.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/4bit.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/4bit_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/4bit_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/8bit_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/8bit_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/castle_spritesheet.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/castle_spritesheet.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)    77880 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel_rle.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel_rle.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/magtag_2x2_test.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/magtag_2x2_test.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p1_mono_ascii.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p1_mono_ascii.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p2_ascii.pgm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p2_ascii.pgm.license
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p3_rgb_ascii.ppm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p3_rgb_ascii.ppm.license
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p4_mono_binary.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p4_mono_binary.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p4_mono_large.pbm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p4_mono_large.pbm.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p5_binary.pgm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p5_binary.pgm.license
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p6_binary.ppm
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p6_binary.ppm.license
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/test_image.png
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/examples/images/test_image.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 15:16:06.398582 adafruit-circuitpython-imageload-1.17.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 15:16:06.398582 adafruit-circuitpython-imageload-1.17.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/__init__.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/displayio_shared_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/displayio_shared_bindings.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_bitmap_c_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_bitmap_c_interface.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_bmp_indexed_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_bmp_indexed_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_palette_c_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_palette_c_interface.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_pbm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_pbm_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_pgm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_pgm_load.py.license
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-01-09 15:15:58.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_ppm_load.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-09 15:15:51.000000 adafruit-circuitpython-imageload-1.17.0/tests/test_ppm_load.py.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.640087 adafruit-circuitpython-imageload-1.17.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.624086 adafruit-circuitpython-imageload-1.17.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.628086 adafruit-circuitpython-imageload-1.17.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.628086 adafruit-circuitpython-imageload-1.17.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.628086 adafruit-circuitpython-imageload-1.17.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-25 23:21:38.640087 adafruit-circuitpython-imageload-1.17.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.628086 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-25 23:21:38.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-25 23:21:38.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 23:21:38.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 23:21:38.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 23:21:38.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.628086 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10096 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/negative_height_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/displayio_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pbm_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pbm_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/ppm_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/ppm_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/tilegrid_inflator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/developing.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.632086 adafruit-circuitpython-imageload-1.17.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_colorwheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_from_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_netpbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_png_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/examples/imageload_tilegrid_inflator_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.640087 adafruit-circuitpython-imageload-1.17.1/examples/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/1bit-not-byte-aligned.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/1bit-not-byte-aligned.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/1bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/1bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/2bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/2bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/4bit.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/4bit.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/4bit_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/4bit_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/8bit_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/8bit_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/castle_spritesheet.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/castle_spritesheet.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    77880 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)    16998 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel_rle.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel_rle.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/magtag_2x2_test.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/magtag_2x2_test.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p1_mono_ascii.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p1_mono_ascii.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p2_ascii.pgm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p2_ascii.pgm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p3_rgb_ascii.ppm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p3_rgb_ascii.ppm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p4_mono_binary.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p4_mono_binary.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p4_mono_large.pbm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p4_mono_large.pbm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p5_binary.pgm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p5_binary.pgm.license
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p6_binary.ppm
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p6_binary.ppm.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/test_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/examples/images/test_image.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 23:21:38.640087 adafruit-circuitpython-imageload-1.17.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 23:21:38.640087 adafruit-circuitpython-imageload-1.17.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/__init__.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/displayio_shared_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/displayio_shared_bindings.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_bitmap_c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_bitmap_c_interface.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_bmp_indexed_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_bmp_indexed_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_palette_c_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_palette_c_interface.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_pbm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_pbm_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_pgm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_pgm_load.py.license
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-25 23:21:29.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_ppm_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-25 23:21:15.000000 adafruit-circuitpython-imageload-1.17.1/tests/test_ppm_load.py.license
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-imageload-1.17.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/.gitignore` & `adafruit-circuitpython-imageload-1.17.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/.pre-commit-config.yaml` & `adafruit-circuitpython-imageload-1.17.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/.pylintrc` & `adafruit-circuitpython-imageload-1.17.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-imageload-1.17.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/LICENSE` & `adafruit-circuitpython-imageload-1.17.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-imageload-1.17.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/LICENSES/MIT.txt` & `adafruit-circuitpython-imageload-1.17.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-imageload-1.17.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/PKG-INFO` & `adafruit-circuitpython-imageload-1.17.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-imageload
-Version: 1.17.0
+Version: 1.17.1
 Summary: Displays text using CircuitPython's displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad
 Keywords: adafruit,blinka,circuitpython,micropython,bitmap,fonts,text,display,tft,lcd,displayio,imageload,image
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/README.rst` & `adafruit-circuitpython-imageload-1.17.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/PKG-INFO` & `adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-imageload
-Version: 1.17.0
+Version: 1.17.1
 Summary: Displays text using CircuitPython's displayio.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad
 Keywords: adafruit,blinka,circuitpython,micropython,bitmap,fonts,text,display,tft,lcd,displayio,imageload,image
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_circuitpython_imageload.egg-info/SOURCES.txt` & `adafruit-circuitpython-imageload-1.17.1/adafruit_circuitpython_imageload.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/__init__.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload`
 ====================================================
 
@@ -25,15 +25,15 @@
     )
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from .displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file_or_filename: Union[str, BufferedReader],
     *,
     bitmap: Optional[BitmapConstructor] = None,
@@ -73,15 +73,20 @@
 
             return bmp.load(file, bitmap=bitmap, palette=palette)
         if header.startswith(b"P"):
             from . import pnm
 
             return pnm.load(file, header, bitmap=bitmap, palette=palette)
         if header.startswith(b"GIF"):
+            if not bitmap:
+                raise RuntimeError("bitmap argument required")
+
             from . import gif
 
             return gif.load(file, bitmap=bitmap, palette=palette)
         if header.startswith(b"\x89PN"):
+            if not bitmap:
+                raise RuntimeError("bitmap argument required")
             from . import png
 
             return png.load(file, bitmap=bitmap, palette=palette)
         raise RuntimeError("Unsupported image format")
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/__init__.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.bmp`
 ====================================================
 
@@ -18,24 +18,24 @@
     from typing import Tuple, Optional, Set, List
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     *,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None
-) -> Tuple[Bitmap, Optional[Palette]]:
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None
+) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """Loads a bmp image from the open ``file``.
 
     Returns tuple of bitmap object and palette object.
 
     :param object bitmap: Type to store bitmap data. Must have API similar to `displayio.Bitmap`.
       Will be skipped if None
     :param object palette: Type to store the palette. Must have API similar to
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/bmp/indexed.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/bmp/indexed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.bmp.indexed`
 ====================================================
 
@@ -26,63 +26,68 @@
 
 try:
     from bitmaptools import readinto as _bitmap_readinto
 except ImportError:
     _bitmap_readinto = None  # pylint: disable=invalid-name  # type: Callable
 
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
     data_start: int,
     colors: int,
     color_depth: int,
     compression: int,
     *,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None,
-) -> Tuple[Bitmap, Optional[Palette]]:
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None,
+) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """Loads indexed bitmap data into bitmap and palette objects.
 
     :param file file: The open bmp file
     :param int width: Image width in pixels
     :param int height: Image height in pixels
     :param int data_start: Byte location where the data starts (after headers)
     :param int colors: Number of distinct colors in the image
     :param int color_depth: Number of bits used to store a value
-    :param int compression: 0 - none, 1 - 8bit RLE, 2 - 4bit RLE"""
+    :param int compression: 0 - none, 1 - 8bit RLE, 2 - 4bit RLE
+    :param BitmapConstructor bitmap: a function that returns a displayio.Bitmap
+    :param PaletteConstructor palette: a function that returns a displayio.Palette
+    """
     # pylint: disable=too-many-arguments,too-many-locals,too-many-branches
+    palette_obj = None
     if palette:
-        palette = palette(colors)  # type: Palette
+        palette_obj = palette(colors)
 
         file.seek(data_start - colors * 4)
         for value in range(colors):
             c_bytes = file.read(4)
             # Need to swap red & blue bytes (bytes 0 and 2)
-            palette[value] = bytes(
+            palette_obj[value] = bytes(
                 b"".join([c_bytes[2:3], c_bytes[1:2], c_bytes[0:1], c_bytes[3:1]])
             )
 
+    bitmap_obj = None
     if bitmap:
         minimum_color_depth = 1
         while colors > 2**minimum_color_depth:
             minimum_color_depth *= 2
 
         if sys.maxsize > 1073741823:
             # pylint: disable=import-outside-toplevel, relative-beyond-top-level
             from .negative_height_check import negative_height_check
 
             # convert unsigned int to signed int when height is negative
             height = negative_height_check(height)
-        bitmap = bitmap(width, abs(height), colors)  # type: Bitmap
+        bitmap_obj = bitmap(width, abs(height), colors)
         file.seek(data_start)
         line_size = width // (8 // color_depth)
         if width % (8 // color_depth) != 0:
             line_size += 1
         if line_size % 4 != 0:
             line_size += 4 - line_size % 4
 
@@ -93,18 +98,17 @@
             range3 = -1
         else:
             range1 = 0
             range2 = abs(height)
             range3 = 1
 
         if compression == 0:
-
             if _bitmap_readinto:
                 _bitmap_readinto(
-                    bitmap,
+                    bitmap_obj,
                     file,
                     bits_per_pixel=color_depth,
                     element_size=4,
                     reverse_pixels_in_element=True,
                     reverse_rows=True,
                 )
 
@@ -116,25 +120,25 @@
                     offset = y * width
 
                     for x in range(width):
                         i = x // pixels_per_byte
                         pixel = (
                             chunk[i] >> (8 - color_depth * (x % pixels_per_byte + 1))
                         ) & mask
-                        bitmap[offset + x] = pixel
+                        bitmap_obj[offset + x] = pixel
         elif compression in (1, 2):
             decode_rle(
-                bitmap=bitmap,
+                bitmap=bitmap_obj,
                 file=file,
                 compression=compression,
                 y_range=(range1, range2, range3),
                 width=width,
             )
 
-    return bitmap, palette
+    return bitmap_obj, palette_obj
 
 
 def decode_rle(
     bitmap: Bitmap,
     file: BufferedReader,
     compression: int,
     y_range: Tuple[int, int, int],
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/displayio_types.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/displayio_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,9 @@
     from displayio import Palette, Bitmap
 
     PaletteConstructor = Callable[[int], Palette]
     BitmapConstructor = Callable[[int, int, int], Bitmap]
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/gif.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/gif.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2019 Radomir Dopieralski for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.gif`
 ====================================================
 
@@ -20,23 +20,23 @@
     from typing import Tuple, Iterator, Optional, List
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from .displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     *,
     bitmap: BitmapConstructor,
-    palette: PaletteConstructor = None
+    palette: Optional[PaletteConstructor] = None
 ) -> Tuple[Bitmap, Optional[Palette]]:
     """Loads a GIF image from the open ``file``.
 
     Returns tuple of bitmap object and palette object.
 
     :param BufferedReader file: The *.gif file being loaded
     :param object bitmap: Type to store bitmap data. Must have API similar to `displayio.Bitmap`.
@@ -46,14 +46,16 @@
     header = file.read(6)
     if header not in {b"GIF87a", b"GIF89a"}:
         raise ValueError("Not a GIF file")
     width, height, flags, _, _ = struct.unpack(  # pylint: disable=no-member
         "<HHBBB", file.read(7)
     )
     if (flags & 0x80) != 0:
+        if not palette:
+            raise RuntimeError("palette argument required")
         palette_size = 1 << ((flags & 0x07) + 1)
         palette_obj = palette(palette_size)
         for i in range(palette_size):
             palette_obj[i] = file.read(3)
     else:
         palette_obj = None
     color_bits = ((flags & 0x70) >> 4) + 1
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/png.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/png.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 # SPDX-FileCopyrightText: 2022 Radomir Dopieralski
+# SPDX-FileCopyrightText: 2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.png`
 ====================================================
 
 Load pixel values (indices or colors) into a bitmap and colors into a palette
 from a PNG file.
 
-* Author(s): Radomir Dopieralski
+* Author(s): Radomir Dopieralski, Matt Land
 
 """
 
 try:
-    # pylint: disable=unused-import
-    import typing
+    from io import BufferedReader
+    from typing import Optional, Tuple
+    from displayio import Palette, Bitmap
     from .displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
 import struct
 import zlib
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
-    file: str, *, bitmap: BitmapConstructor, palette: PaletteConstructor = None
-):  # pylint: disable=too-many-locals,too-many-branches
-    """Loads a PNG image from the open ``file``.
+    file: BufferedReader,
+    *,
+    bitmap: BitmapConstructor,
+    palette: Optional[PaletteConstructor] = None
+) -> Tuple[Bitmap, Optional[Palette]]:
+    """
+    Loads a PNG image from the open ``file``.
 
     Returns tuple of bitmap object and palette object.
 
     :param file: The *.png file being loaded
     :param object bitmap: Type to store bitmap data. Must have API similar to
       `displayio.Bitmap`.
     :param object palette: Type to store the palette. Must have API similar to
-      `displayio.Palette`. Will be skipped if None"""
+      `displayio.Palette`. Will be skipped if None
+    """
+    # pylint: disable=too-many-locals,too-many-branches
     header = file.read(8)
     if header != b"\x89PNG\r\n\x1a\n":
         raise ValueError("Not a PNG file")
     del header
     data = bytearray()
     pal = None
     mode = None
-    depth = None
+    depth = 0
+    width = 0
+    height = 0
     while True:
         size, chunk = struct.unpack(">I4s", file.read(8))
         if chunk == b"IHDR":
             (
                 width,
                 height,
                 depth,
@@ -77,20 +87,20 @@
         elif chunk == b"IDAT":
             data.extend(file.read(size))
         elif chunk == b"IEND":
             break
         else:
             file.seek(size, 1)  # skip unknown chunks
         file.seek(4, 1)  # skip CRC
-    data = zlib.decompress(data)
+    data_bytes = zlib.decompress(data)
     bmp = bitmap(width, height, 1 << depth)
     scanline = (width * depth + 7) // 8
     mem = memoryview(bmp)
     for y in range(height):
         dst = y * scanline
         src = y * (scanline + 1) + 1
-        filter_ = data[src - 1]
+        filter_ = data_bytes[src - 1]
         if filter_ == 0:
-            mem[dst : dst + scanline] = data[src : src + scanline]
+            mem[dst : dst + scanline] = data_bytes[src : src + scanline]
         else:
             raise NotImplementedError("Filters not supported")
     return bmp, pal
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/__init__.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm`
@@ -28,24 +28,24 @@
     )
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     header: bytes,
     *,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """
     Scan for netpbm format info, skip over comments, and delegate to a submodule
     to do the actual data loading.
     Formats P1, P4 have two space padded pieces of information: width and height.
     All other formats have three: width, height, and max color value.
     This load function will move the file stream pointer to the start of data in all cases.
@@ -88,37 +88,42 @@
                     pnm_header[0],
                     pnm_header[1],
                     bitmap=bitmap,
                     palette=palette,
                 )
 
         if len(pnm_header) == 2 and magic_number in [b"P1", b"P4"]:
-            bitmap = bitmap(pnm_header[0], pnm_header[1], 1)  # type: Bitmap
+            if not bitmap:
+                raise RuntimeError(
+                    "A bitmap constructor is required for this type of pnm format file"
+                )
+            bitmap_obj = bitmap(pnm_header[0], pnm_header[1], 1)
+            palette_obj = None
             if palette:
-                palette = palette(1)  # type: Palette
-                palette[0] = b"\xFF\xFF\xFF"
+                palette_obj = palette(1)
+                palette_obj[0] = b"\xFF\xFF\xFF"
             if magic_number.startswith(b"P1"):
                 from . import pbm_ascii
 
                 return pbm_ascii.load(
                     file,
                     pnm_header[0],
                     pnm_header[1],
-                    bitmap=bitmap,
-                    palette=palette,
+                    bitmap=bitmap_obj,
+                    palette=palette_obj,
                 )
 
             from . import pbm_binary
 
             return pbm_binary.load(
                 file,
                 pnm_header[0],
                 pnm_header[1],
-                bitmap=bitmap,
-                palette=palette,
+                bitmap=bitmap_obj,
+                palette=palette_obj,
             )
 
         next_byte = file.read(1)
         if next_byte == b"":
             raise RuntimeError("Unsupported image format {!r}".format(magic_number))
         if next_byte == b"#":  # comment found, seek until a newline or EOF is found
             while file.read(1) not in [b"", b"\n"]:  # EOF or NL
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pbm_ascii.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pbm_ascii.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.pbm_ascii`
@@ -19,24 +19,24 @@
 try:
     from typing import Tuple, Optional
     from io import BufferedReader
     from displayio import Palette, Bitmap
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
     bitmap: Bitmap,
-    palette: Palette = None,
+    palette: Optional[Palette] = None,
 ) -> Tuple[Bitmap, Optional[Palette]]:
     """
     Load a P1 'PBM' ascii image into the displayio.Bitmap
     """
     next_byte = b"1"  # just to start the iterator
     for y in range(height):
         x = 0
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pbm_binary.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pbm_binary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.pbm_binary`
@@ -18,24 +18,24 @@
 try:
     from typing import Tuple, Optional, Iterator
     from io import BufferedReader
     from displayio import Palette, Bitmap
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
     bitmap: Bitmap,
-    palette: Palette = None,
+    palette: Optional[Palette] = None,
 ) -> Tuple[Bitmap, Optional[Palette]]:
     """
     Load a P4 'PBM' binary image into the Bitmap
     """
     x = 0
     y = 0
     while True:
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/__init__.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.pgm`
@@ -25,16 +25,16 @@
 
 
 def load(
     file: BufferedReader,
     magic_number: bytes,
     header: List[int],
     *,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """
     Perform the load of Netpbm greyscale images (P2, P5)
     """
     if header[2] > 256:
         raise NotImplementedError("16 bit files are not supported")
     width = header[0]
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/ascii.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/ascii.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.pgm.ascii`
@@ -23,16 +23,16 @@
     pass
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None,
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None,
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """
     Load a PGM ascii file (P2)
     """
     data_start = file.tell()  # keep this so we can rewind
     _palette_colors = set()
     pixel = bytearray()
@@ -42,31 +42,32 @@
         if byte == b"":
             break
         if not byte.isdigit():
             int_pixel = int("".join(["%c" % char for char in pixel]))
             _palette_colors.add(int_pixel)
             pixel = bytearray()
         pixel += byte
+    palette_obj = None
     if palette:
-        palette = build_palette(palette, _palette_colors)  # type: Palette
+        palette_obj = build_palette(palette, _palette_colors)
+    bitmap_obj = None
     if bitmap:
-        bitmap = bitmap(width, height, len(_palette_colors))  # type: Bitmap
-        _palette_colors = list(_palette_colors)
+        bitmap_obj = bitmap(width, height, len(_palette_colors))
         file.seek(data_start)
         for y in range(height):
             for x in range(width):
                 pixel = bytearray()
                 while True:
                     byte = file.read(1)
                     if not byte.isdigit():
                         break
                     pixel += byte
                 int_pixel = int("".join(["%c" % char for char in pixel]))
-                bitmap[x, y] = _palette_colors.index(int_pixel)
-    return bitmap, palette
+                bitmap_obj[x, y] = list(_palette_colors).index(int_pixel)
+    return bitmap_obj, palette_obj
 
 
 def build_palette(
     palette_class: PaletteConstructor, palette_colors: Set[int]
 ) -> Palette:  # pylint: disable=duplicate-code
     """
     construct the Palette, and populate it with the set of palette_colors
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/pgm/binary.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/pgm/binary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.pgm.binary`
@@ -11,50 +11,51 @@
 
 Load pixel values (indices or colors) into a bitmap and colors into a palette.
 
 * Author(s): Matt Land, Brooke Storm, Sam McGahan
 
 """
 try:
-    from typing import Tuple, Optional, Set, List
+    from typing import Tuple, Optional, Set
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ...displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None,
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None,
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """
     Load a P5 format file (binary), handle PGM (greyscale)
     """
     palette_colors = set()  # type: Set[int]
     data_start = file.tell()
     for y in range(height):
         data_line = iter(bytes(file.read(width)))
         for pixel in data_line:
             palette_colors.add(pixel)
 
+    palette_obj = None
     if palette:
-        palette = build_palette(palette, palette_colors)  # type: Palette
+        palette_obj = build_palette(palette, palette_colors)
+    bitmap_obj = None
     if bitmap:
-        bitmap = bitmap(width, height, len(palette_colors))  # type: Bitmap
-        palette_colors = list(palette_colors)  # type: List[int]
+        bitmap_obj = bitmap(width, height, len(palette_colors))
         file.seek(data_start)
         for y in range(height):
             data_line = iter(bytes(file.read(width)))
             for x, pixel in enumerate(data_line):
-                bitmap[x, y] = palette_colors.index(pixel)
-    return bitmap, palette
+                bitmap_obj[x, y] = list(palette_colors).index(pixel)
+    return bitmap_obj, palette_obj
 
 
 def build_palette(
     palette_class: PaletteConstructor, palette_colors: Set[int]
 ) -> Palette:
     """
     construct the Palette, and populate it with the set of palette_colors
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/ppm_ascii.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/ppm_ascii.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.ppm_ascii`
@@ -12,15 +12,15 @@
 Load pixel values (indices or colors) into a bitmap and for an ascii ppm,
 return None for pallet.
 
 * Author(s):  Matt Land, Brooke Storm, Sam McGahan
 
 """
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 try:
     from typing import (
         Tuple,
         Iterator,
         Optional,
@@ -34,16 +34,16 @@
     pass
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None,
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None,
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
     """
     :param stream file: infile with the position set at start of data
     :param int width:
     :param int height:
     :param int max_colors: color space of file
     :param bitmap: displayio.Bitmap class
@@ -51,35 +51,36 @@
     :return tuple:
     """
     palette_colors = set()  # type: Set[bytes]
     data_start = file.tell()
     for triplet in read_three_colors(file):
         palette_colors.add(triplet)
 
+    palette_obj = None
     if palette:
-        palette = palette(len(palette_colors))  # type: Palette
+        palette_obj = palette(len(palette_colors))
         for counter, color in enumerate(palette_colors):
-            palette[counter] = color
+            palette_obj[counter] = color
+    bitmap_obj = None
     if bitmap:
         file.seek(data_start)
-        bitmap = bitmap(width, height, len(palette_colors))  # type: Bitmap
-        palette_colors = list(palette_colors)  # type: List[bytes]
+        bitmap_obj = bitmap(width, height, len(palette_colors))
         for y in range(height):
             for x in range(width):
                 for color in read_three_colors(file):
-                    bitmap[x, y] = palette_colors.index(color)
+                    bitmap_obj[x, y] = list(palette_colors).index(color)
                     break  # exit the inner generator
-    return bitmap, palette
+    return bitmap_obj, palette_obj
 
 
 def read_three_colors(file: BufferedReader) -> Iterator[bytes]:
     """
     Generator to read integer values from file, in groups of three.
     Each value can be len 1-3, for values 0 - 255, space padded.
-    :return tuple[int]:
+    :return Iterator[bytes]:
     """
     triplet = []  # type: List[int]
     color = bytearray()
     while True:
         this_byte = file.read(1)
         if this_byte.isdigit():
             color += this_byte
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/pnm/ppm_binary.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/pnm/ppm_binary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2018 Scott Shawcroft for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 # SPDX-FileCopyrightText: Brooke Storm
 # SPDX-FileCopyrightText: Sam McGahan
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.pnm.ppm_binary`
@@ -19,50 +19,54 @@
     from typing import Tuple, Optional, List, Set
     from io import BufferedReader
     from displayio import Palette, Bitmap
     from ..displayio_types import PaletteConstructor, BitmapConstructor
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def load(
     file: BufferedReader,
     width: int,
     height: int,
-    bitmap: BitmapConstructor = None,
-    palette: PaletteConstructor = None,
+    bitmap: Optional[BitmapConstructor] = None,
+    palette: Optional[PaletteConstructor] = None,
 ) -> Tuple[Optional[Bitmap], Optional[Palette]]:
-    """Load pixel values (indices or colors) into a bitmap and for a binary
-    ppm, return None for pallet."""
+    """
+    Load pixel values (indices or colors) into a bitmap and for a binary
+    ppm, return None for pallet.
+    """
+    # pylint: disable=too-many-locals
 
     data_start = file.tell()
     palette_colors = set()  # type: Set[Tuple[int, int, int]]
     line_size = width * 3
 
     for y in range(height):
         data_line = iter(bytes(file.read(line_size)))
         for red in data_line:
             # red, green, blue
             palette_colors.add((red, next(data_line), next(data_line)))
 
+    palette_obj = None
     if palette:
-        palette = palette(len(palette_colors))  # type: Palette
+        palette_obj = palette(len(palette_colors))
         for counter, color in enumerate(palette_colors):
-            palette[counter] = bytes(color)
+            palette_obj[counter] = bytes(color)
+    bitmap_obj = None
     if bitmap:
-        bitmap = bitmap(width, height, len(palette_colors))  # type: Bitmap
+        bitmap_obj = bitmap(width, height, len(palette_colors))
         file.seek(data_start)
-        palette_colors = list(palette_colors)  # type: List[Tuple[int, int, int]]
         for y in range(height):
             x = 0
             data_line = iter(bytes(file.read(line_size)))
             for red in data_line:
                 # red, green, blue
-                bitmap[x, y] = palette_colors.index(
+                bitmap_obj[x, y] = list(palette_colors).index(
                     (red, next(data_line), next(data_line))
                 )
                 x += 1
 
-    return bitmap, palette
+    return bitmap_obj, palette_obj
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/adafruit_imageload/tilegrid_inflator.py` & `adafruit-circuitpython-imageload-1.17.1/adafruit_imageload/tilegrid_inflator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-FileCopyrightText: 2022 Tim Cocks for Adafruit Industries
-# SPDX-FileCopyrightText: 2022 Matt Land
+# SPDX-FileCopyrightText: 2022-2023 Matt Land
 #
 # SPDX-License-Identifier: MIT
 
 """
 `adafruit_imageload.tilegrid_inflator`
 ====================================================
 
@@ -18,33 +18,33 @@
 
 try:
     from typing import Tuple, Optional, List, Union
     from displayio import Palette, Bitmap, OnDiskBitmap, TileGrid
 except ImportError:
     pass
 
-__version__ = "1.17.0"
+__version__ = "1.17.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad.git"
 
 
 def inflate_tilegrid(
-    bmp_path: str = None,
+    bmp_path: Optional[str] = None,
     target_size: Tuple[int, int] = (3, 3),
-    tile_size: List[int] = None,
+    tile_size: Optional[List[int]] = None,
     transparent_index: Optional[Union[tuple, int]] = None,
     bmp_obj: Optional[OnDiskBitmap] = None,
     bmp_palette: Optional[Palette] = None,
 ) -> TileGrid:
     """
     inflate a TileGrid of ``target_size`` in tiles from a 3x3 spritesheet by duplicating
     the center rows and columns.
 
     :param Optional[str] bmp_path: filepath to the 3x3 spritesheet bitmap file
-    :param Optional[tuple] target_size: desired size in tiles (target_width, target_height)
-    :param Optional[tuple] tile_size: size of the tiles in the 3x3 spritesheet. If
+    :param tuple[int, int] target_size: desired size in tiles (target_width, target_height)
+    :param Optional[List[int]] tile_size: size of the tiles in the 3x3 spritesheet. If
       None is used it will equally divide the width and height of the Bitmap by 3.
     :param Optional[Union[tuple, int]] transparent_index: a single index within the palette to
       make transparent, or a tuple of multiple indexes to make transparent
     :param Optional[OnDiskBitmap] bmp_obj: Already loaded 3x3 spritesheet in an OnDiskBitmap
     :param Optional[Palette] bmp_palette: Already loaded spritesheet Palette
     """
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/docs/_static/favicon.ico` & `adafruit-circuitpython-imageload-1.17.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/docs/conf.py` & `adafruit-circuitpython-imageload-1.17.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/docs/developing.rst` & `adafruit-circuitpython-imageload-1.17.1/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/docs/examples.rst` & `adafruit-circuitpython-imageload-1.17.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/docs/index.rst` & `adafruit-circuitpython-imageload-1.17.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/imageload_from_web.py` & `adafruit-circuitpython-imageload-1.17.1/examples/imageload_from_web.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/imageload_magtag_simpletest.py` & `adafruit-circuitpython-imageload-1.17.1/examples/imageload_magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/imageload_netpbm.py` & `adafruit-circuitpython-imageload-1.17.1/examples/imageload_netpbm.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/imageload_png_simpletest.py` & `adafruit-circuitpython-imageload-1.17.1/examples/imageload_png_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/1bit-not-byte-aligned.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/1bit-not-byte-aligned.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/8bit_rle.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/8bit_rle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/castle_spritesheet.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/castle_spritesheet.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/color_wheel_rle.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/color_wheel_rle.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/magtag_2x2_test.bmp` & `adafruit-circuitpython-imageload-1.17.1/examples/images/magtag_2x2_test.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p1_mono_ascii.pbm` & `adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p1_mono_ascii.pbm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p3_rgb_ascii.ppm` & `adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p3_rgb_ascii.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p4_mono_large.pbm` & `adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p4_mono_large.pbm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/netpbm_p6_binary.ppm` & `adafruit-circuitpython-imageload-1.17.1/examples/images/netpbm_p6_binary.ppm`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/examples/images/test_image.png` & `adafruit-circuitpython-imageload-1.17.1/examples/images/test_image.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/pyproject.toml` & `adafruit-circuitpython-imageload-1.17.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-imageload"
 description = "Displays text using CircuitPython's displayio."
-version = "1.17.0"
+version = "1.17.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ImageLoad"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/__init__.py` & `adafruit-circuitpython-imageload-1.17.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/displayio_shared_bindings.py` & `adafruit-circuitpython-imageload-1.17.1/tests/displayio_shared_bindings.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_bitmap_c_interface.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_bitmap_c_interface.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_bmp_indexed_load.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_bmp_indexed_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_palette_c_interface.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_palette_c_interface.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_pbm_load.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_pbm_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_pgm_load.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_pgm_load.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-imageload-1.17.0/tests/test_ppm_load.py` & `adafruit-circuitpython-imageload-1.17.1/tests/test_ppm_load.py`

 * *Files identical despite different names*

