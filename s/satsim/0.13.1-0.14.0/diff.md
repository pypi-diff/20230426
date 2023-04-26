# Comparing `tmp/satsim-0.13.1.tar.gz` & `tmp/satsim-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsim-0.13.1.tar", last modified: Wed Mar 15 09:15:02 2023, max compression
+gzip compressed data, was "satsim-0.14.0.tar", last modified: Thu Apr 13 09:49:43 2023, max compression
```

## Comparing `satsim-0.13.1.tar` & `satsim-0.14.0.tar`

### file list

```diff
@@ -1,153 +1,165 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/
--rw-r--r--   0 root         (0) root         (0)      170 2023-03-15 07:04:27.000000 satsim-0.13.1/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     3255 2023-03-15 07:04:27.000000 satsim-0.13.1/CONTRIBUTING.rst
--rw-r--r--   0 root         (0) root         (0)     6505 2023-03-15 07:36:16.000000 satsim-0.13.1/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)      291 2023-03-15 07:04:28.000000 satsim-0.13.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8130 2023-03-15 09:15:02.892586 satsim-0.13.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-03-15 07:04:38.000000 satsim-0.13.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/
--rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.872586 satsim-0.13.1/docs/_build/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/_static/
--rw-r--r--   0 root         (0) root         (0)    14813 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/_static/css/
--rw-r--r--   0 root         (0) root         (0)     3229 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/badge_only.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 root         (0) root         (0)   165742 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 root         (0) root         (0)   444379 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 root         (0) root         (0)   165548 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 root         (0) root         (0)    98024 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 root         (0) root         (0)    77160 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 root         (0) root         (0)   135235 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 root         (0) root         (0)     4472 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 root         (0) root         (0)      421 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/file.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/_static/js/
--rw-r--r--   0 root         (0) root         (0)      934 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 root         (0) root         (0)     4370 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 root         (0) root         (0)     2734 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 root         (0) root         (0)     5023 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 root         (0) root         (0)     4758 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 root         (0) root         (0)       90 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 root         (0) root         (0)       90 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 root         (0) root         (0)     4846 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 root         (0) root         (0)    18215 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 root         (0) root         (0)     4712 2023-03-15 09:12:10.000000 satsim-0.13.1/docs/_build/html/_static/sphinx_highlight.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/_build/html/api/
--rw-r--r--   0 root         (0) root         (0)    10009 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.dataset.html
--rw-r--r--   0 root         (0) root         (0)     9944 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.generator.html
--rw-r--r--   0 root         (0) root         (0)    59050 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.generator.obs.html
--rw-r--r--   0 root         (0) root         (0)   104847 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.geometry.html
--rw-r--r--   0 root         (0) root         (0)    86632 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.html
--rw-r--r--   0 root         (0) root         (0)    91538 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.image.html
--rw-r--r--   0 root         (0) root         (0)    34513 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.io.html
--rw-r--r--   0 root         (0) root         (0)    33137 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.math.html
--rw-r--r--   0 root         (0) root         (0)    14439 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.pipeline.html
--rw-r--r--   0 root         (0) root         (0)    18154 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.time.html
--rw-r--r--   0 root         (0) root         (0)    24160 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api/satsim.util.html
--rw-r--r--   0 root         (0) root         (0)    48405 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/api.html
--rw-r--r--   0 root         (0) root         (0)     5479 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/authors.html
--rw-r--r--   0 root         (0) root         (0)    13939 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/contributing.html
--rw-r--r--   0 root         (0) root         (0)    43169 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/genindex.html
--rw-r--r--   0 root         (0) root         (0)    17127 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/history.html
--rw-r--r--   0 root         (0) root         (0)     9346 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/index.html
--rw-r--r--   0 root         (0) root         (0)     7750 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/installation.html
--rw-r--r--   0 root         (0) root         (0)    15212 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/py-modindex.html
--rw-r--r--   0 root         (0) root         (0)     4196 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/search.html
--rw-r--r--   0 root         (0) root         (0)    65809 2023-03-15 09:15:02.000000 satsim-0.13.1/docs/_build/html/searchindex.js
--rw-r--r--   0 root         (0) root         (0)    37538 2023-03-15 09:15:01.000000 satsim-0.13.1/docs/_build/html/usage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/docs/api/
--rw-r--r--   0 root         (0) root         (0)      310 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.dataset.rst
--rw-r--r--   0 root         (0) root         (0)     1002 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.generator.obs.rst
--rw-r--r--   0 root         (0) root         (0)      218 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.generator.rst
--rw-r--r--   0 root         (0) root         (0)     1872 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.geometry.rst
--rw-r--r--   0 root         (0) root         (0)     1004 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.image.rst
--rw-r--r--   0 root         (0) root         (0)      673 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.io.rst
--rw-r--r--   0 root         (0) root         (0)      998 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.math.rst
--rw-r--r--   0 root         (0) root         (0)      135 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.pipeline.rst
--rw-r--r--   0 root         (0) root         (0)      712 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.rst
--rw-r--r--   0 root         (0) root         (0)      123 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.time.rst
--rw-r--r--   0 root         (0) root         (0)      572 2023-03-15 09:14:54.000000 satsim-0.13.1/docs/api/satsim.util.rst
--rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/api.rst
--rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/authors.rst
--rw-r--r--   0 root         (0) root         (0)     4906 2023-02-27 00:29:51.000000 satsim-0.13.1/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/history.rst
--rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     1475 2023-02-27 00:29:51.000000 satsim-0.13.1/docs/installation.rst
--rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:33:49.000000 satsim-0.13.1/docs/usage.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.882586 satsim-0.13.1/satsim/
--rw-r--r--   0 root         (0) root         (0)      264 2023-03-15 07:36:16.000000 satsim-0.13.1/satsim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/cli.py
--rw-r--r--   0 root         (0) root         (0)    20530 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/dataset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/dataset/augment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/generator/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/generator/obs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/breakup.py
--rw-r--r--   0 root         (0) root         (0)     2330 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/cso.py
--rw-r--r--   0 root         (0) root         (0)     6239 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/geometry.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/io.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/generator/obs/rpo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/geometry/
--rw-r--r--   0 root         (0) root         (0)       66 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20106 2023-03-15 07:36:16.000000 satsim-0.13.1/satsim/geometry/astrometric.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/csvsc.py
--rw-r--r--   0 root         (0) root         (0)     5268 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/draw.py
--rw-r--r--   0 root         (0) root         (0)     3404 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/ephemeris.py
--rw-r--r--   0 root         (0) root         (0)     1672 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/random.py
--rw-r--r--   0 root         (0) root         (0)     1150 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/sgp4.py
--rw-r--r--   0 root         (0) root         (0)      699 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/sprite.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/sstr7.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/transform.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/twobody.py
--rw-r--r--   0 root         (0) root         (0)     3787 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/geometry/wcs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/image/
--rw-r--r--   0 root         (0) root         (0)       58 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9793 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/augment.py
--rw-r--r--   0 root         (0) root         (0)    16529 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/fpa.py
--rw-r--r--   0 root         (0) root         (0)     5359 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/model.py
--rw-r--r--   0 root         (0) root         (0)     2842 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/noise.py
--rw-r--r--   0 root         (0) root         (0)     6166 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/psf.py
--rw-r--r--   0 root         (0) root         (0)    10401 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/image/render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/io/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11195 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/io/czml.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/io/fits.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 07:36:16.000000 satsim-0.13.1/satsim/io/image.py
--rw-r--r--   0 root         (0) root         (0)     7122 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/io/satnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/math/
--rw-r--r--   0 root         (0) root         (0)       81 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/angle.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/conv.py
--rw-r--r--   0 root         (0) root         (0)     5551 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/fft.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/random.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/math/stats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/pipeline/
--rw-r--r--   0 root         (0) root         (0)     1087 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41367 2023-03-15 07:36:16.000000 satsim-0.13.1/satsim/satsim.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/time/
--rw-r--r--   0 root         (0) root         (0)     4008 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/time/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim/util/
--rw-r--r--   0 root         (0) root         (0)      130 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2542 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/util/system.py
--rw-r--r--   0 root         (0) root         (0)     3271 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     2044 2023-03-15 07:05:07.000000 satsim-0.13.1/satsim/util/timer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/satsim.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8130 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3683 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      327 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-03-15 09:15:02.000000 satsim-0.13.1/satsim.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-15 09:15:02.892586 satsim-0.13.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1796 2023-03-15 07:36:16.000000 satsim-0.13.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-15 09:15:02.892586 satsim-0.13.1/tests/
--rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.13.1/tests/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/
+-rw-r--r--   0 root         (0) root         (0)      170 2022-07-22 19:32:02.000000 satsim-0.14.0/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     3255 2023-02-17 19:27:57.000000 satsim-0.14.0/CONTRIBUTING.rst
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-04-13 09:36:02.000000 satsim-0.14.0/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)      291 2022-07-22 19:32:02.000000 satsim-0.14.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8291 2023-04-13 09:49:43.543551 satsim-0.14.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-04-13 09:42:46.000000 satsim-0.14.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.523551 satsim-0.14.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      608 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.523551 satsim-0.14.0/docs/_build/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/
+-rw-r--r--   0 root         (0) root         (0)    14813 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/css/
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/badge_only.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 root         (0) root         (0)   165742 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 root         (0) root         (0)   444379 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 root         (0) root         (0)   165548 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    98024 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 root         (0) root         (0)    77160 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 root         (0) root         (0)   135235 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 root         (0) root         (0)     4472 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 root         (0) root         (0)      421 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/file.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/_static/js/
+-rw-r--r--   0 root         (0) root         (0)      934 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     2734 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 root         (0) root         (0)     5023 2023-04-13 09:47:10.000000 satsim-0.14.0/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 root         (0) root         (0)     4758 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 root         (0) root         (0)     4846 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 root         (0) root         (0)    18215 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-04-13 09:47:09.000000 satsim-0.14.0/docs/_build/html/_static/sphinx_highlight.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/_build/html/api/
+-rw-r--r--   0 root         (0) root         (0)    10121 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.dataset.html
+-rw-r--r--   0 root         (0) root         (0)    10056 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.generator.html
+-rw-r--r--   0 root         (0) root         (0)    59162 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.generator.obs.html
+-rw-r--r--   0 root         (0) root         (0)   106508 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.geometry.html
+-rw-r--r--   0 root         (0) root         (0)   159519 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.html
+-rw-r--r--   0 root         (0) root         (0)    91650 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.image.html
+-rw-r--r--   0 root         (0) root         (0)    34797 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.io.html
+-rw-r--r--   0 root         (0) root         (0)    33473 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.math.html
+-rw-r--r--   0 root         (0) root         (0)    14551 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.pipeline.html
+-rw-r--r--   0 root         (0) root         (0)    19353 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.time.html
+-rw-r--r--   0 root         (0) root         (0)    24310 2023-04-13 09:49:41.000000 satsim-0.14.0/docs/_build/html/api/satsim.util.html
+-rw-r--r--   0 root         (0) root         (0)   404446 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/api/satsim.vecmath.html
+-rw-r--r--   0 root         (0) root         (0)   122444 2023-04-13 09:49:40.000000 satsim-0.14.0/docs/_build/html/api.html
+-rw-r--r--   0 root         (0) root         (0)     5491 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/authors.html
+-rw-r--r--   0 root         (0) root         (0)    13939 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/contributing.html
+-rw-r--r--   0 root         (0) root         (0)    95348 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/genindex.html
+-rw-r--r--   0 root         (0) root         (0)    17468 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/history.html
+-rw-r--r--   0 root         (0) root         (0)     9440 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/index.html
+-rw-r--r--   0 root         (0) root         (0)     7750 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/installation.html
+-rw-r--r--   0 root         (0) root         (0)    17277 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/py-modindex.html
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/search.html
+-rw-r--r--   0 root         (0) root         (0)   121517 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/searchindex.js
+-rw-r--r--   0 root         (0) root         (0)    37538 2023-04-13 09:49:42.000000 satsim-0.14.0/docs/_build/html/usage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/docs/api/
+-rw-r--r--   0 root         (0) root         (0)      310 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.dataset.rst
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.generator.obs.rst
+-rw-r--r--   0 root         (0) root         (0)      218 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.generator.rst
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.geometry.rst
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.image.rst
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.io.rst
+-rw-r--r--   0 root         (0) root         (0)     1138 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.math.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.pipeline.rst
+-rw-r--r--   0 root         (0) root         (0)      730 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.rst
+-rw-r--r--   0 root         (0) root         (0)      123 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.time.rst
+-rw-r--r--   0 root         (0) root         (0)      572 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.util.rst
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-04-13 09:49:32.000000 satsim-0.14.0/docs/api/satsim.vecmath.rst
+-rw-r--r--   0 root         (0) root         (0)      136 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/api.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/authors.rst
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-04-13 09:36:02.000000 satsim-0.14.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)       33 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       27 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/history.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-02-17 19:27:57.000000 satsim-0.14.0/docs/installation.rst
+-rw-r--r--   0 root         (0) root         (0)      768 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    11419 2022-07-22 19:32:02.000000 satsim-0.14.0/docs/usage.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/
+-rw-r--r--   0 root         (0) root         (0)      264 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/cli.py
+-rw-r--r--   0 root         (0) root         (0)    20530 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/dataset/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/dataset/augment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/generator/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim/generator/obs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/breakup.py
+-rw-r--r--   0 root         (0) root         (0)     2330 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/cso.py
+-rw-r--r--   0 root         (0) root         (0)     6239 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/io.py
+-rw-r--r--   0 root         (0) root         (0)     3703 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/generator/obs/rpo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/geometry/
+-rw-r--r--   0 root         (0) root         (0)       66 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20912 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/geometry/astrometric.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/csvsc.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/draw.py
+-rw-r--r--   0 root         (0) root         (0)     3404 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/ephemeris.py
+-rw-r--r--   0 root         (0) root         (0)     1672 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/random.py
+-rw-r--r--   0 root         (0) root         (0)     1150 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/sgp4.py
+-rw-r--r--   0 root         (0) root         (0)      699 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/sprite.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/sstr7.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/geometry/transform.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/geometry/twobody.py
+-rw-r--r--   0 root         (0) root         (0)     3787 2023-02-17 00:02:42.000000 satsim-0.14.0/satsim/geometry/wcs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/image/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9793 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/augment.py
+-rw-r--r--   0 root         (0) root         (0)    16529 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/image/fpa.py
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/image/model.py
+-rw-r--r--   0 root         (0) root         (0)     2842 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/noise.py
+-rw-r--r--   0 root         (0) root         (0)     6166 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/psf.py
+-rw-r--r--   0 root         (0) root         (0)    10401 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/image/render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13925 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/io/czml.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/fits.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2023-03-15 01:56:05.000000 satsim-0.14.0/satsim/io/image.py
+-rw-r--r--   0 root         (0) root         (0)     7122 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/io/satnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/math/
+-rw-r--r--   0 root         (0) root         (0)       81 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-04-05 08:00:38.000000 satsim-0.14.0/satsim/math/angle.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/math/const.py
+-rw-r--r--   0 root         (0) root         (0)      951 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/conv.py
+-rw-r--r--   0 root         (0) root         (0)     5551 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/fft.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/math/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-02-17 19:27:57.000000 satsim-0.14.0/satsim/math/random.py
+-rw-r--r--   0 root         (0) root         (0)      590 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/math/stats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/pipeline/
+-rw-r--r--   0 root         (0) root         (0)     1087 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41936 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/satsim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/time/
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/time/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/util/
+-rw-r--r--   0 root         (0) root         (0)      130 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/system.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     2044 2022-07-22 19:32:02.000000 satsim-0.14.0/satsim/util/timer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/satsim/vecmath/
+-rw-r--r--   0 root         (0) root         (0)    17668 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian2.py
+-rw-r--r--   0 root         (0) root         (0)    20896 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian3.py
+-rw-r--r--   0 root         (0) root         (0)    18429 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Cartesian4.py
+-rw-r--r--   0 root         (0) root         (0)    21727 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix2.py
+-rw-r--r--   0 root         (0) root         (0)    42567 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix3.py
+-rw-r--r--   0 root         (0) root         (0)    73877 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Matrix4.py
+-rw-r--r--   0 root         (0) root         (0)    25251 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/Quaternion.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-04-13 09:36:02.000000 satsim-0.14.0/satsim/vecmath/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.533551 satsim-0.14.0/satsim.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8291 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      327 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-13 09:49:43.000000 satsim-0.14.0/satsim.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2023-04-13 09:49:43.543551 satsim-0.14.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-04-13 09:36:02.000000 satsim-0.14.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 09:49:43.543551 satsim-0.14.0/tests/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 21:03:12.000000 satsim-0.14.0/tests/README.md
```

### Comparing `satsim-0.13.1/CONTRIBUTING.rst` & `satsim-0.14.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/HISTORY.md` & `satsim-0.14.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 History
 =======
 
+0.14.0
+---------------------
+
+Add vector math library.
+Add CZML output for sensor visualization.
+Fix objects not updating properly when image renderer is off.
+
+
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
 * Fix incorrect CZML output when image renderer is off.
```

### Comparing `satsim-0.13.1/PKG-INFO` & `satsim-0.14.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.13.1
+Version: 0.14.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,14 +37,22 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.14.0
+---------------------
+
+Add vector math library.
+Add CZML output for sensor visualization.
+Fix objects not updating properly when image renderer is off.
+
+
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
 * Fix incorrect CZML output when image renderer is off.
```

### Comparing `satsim-0.13.1/README.md` & `satsim-0.14.0/README.md`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/Makefile` & `satsim-0.14.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/basic.css` & `satsim-0.14.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/badge_only.css` & `satsim-0.14.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `satsim-0.14.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/css/theme.css` & `satsim-0.14.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/doctools.js` & `satsim-0.14.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/js/badge_only.js` & `satsim-0.14.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `satsim-0.14.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/js/html5shiv.min.js` & `satsim-0.14.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/js/theme.js` & `satsim-0.14.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/language_data.js` & `satsim-0.14.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/pygments.css` & `satsim-0.14.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/searchtools.js` & `satsim-0.14.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/_static/sphinx_highlight.js` & `satsim-0.14.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.dataset.html` & `satsim-0.14.0/docs/_build/html/api/satsim.dataset.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.dataset package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.dataset package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.generator.html` & `satsim-0.14.0/docs/_build/html/api/satsim.generator.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.generator package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.generator.obs.html` & `satsim-0.14.0/docs/_build/html/api/satsim.generator.obs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator.obs package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.generator.obs package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.geometry.html` & `satsim-0.14.0/docs/_build/html/api/satsim.geometry.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.geometry package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.geometry package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
@@ -184,14 +185,32 @@
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>A <cite>Topos</cite> Skyfield object on the planet Earth</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
+<dt class="sig sig-object py" id="satsim.geometry.astrometric.eci_to_ecr">
+<span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">eci_to_ecr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ra</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dec</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">roll</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.eci_to_ecr" title="Permalink to this definition"></a></dt>
+<dd><p>Covert an Earth centered fixed sky coordinates to Earth centered rotating.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>ra</strong> – <cite>float</cite>, right ascension in degrees</p></li>
+<li><p><strong>dec</strong> – <cite>float</cite>, declination in degrees</p></li>
+<li><p><strong>roll</strong> – <cite>float</cite>, field rotation (ignored)</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>float</cite>, ra, dec and roll in degrees</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
 <dt class="sig sig-object py" id="satsim.geometry.astrometric.gen_track">
 <span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">gen_track</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">height</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">width</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">y_fov</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">x_fov</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">observer</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">track</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">satellites</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">brightnesses</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">t0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tt</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rot</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pad_mult</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">track_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'rate'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0,</span> <span class="pre">0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">flipud</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fliplr</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">az</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">el</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.gen_track" title="Permalink to this definition"></a></dt>
 <dd><p>Generates a list of pixel coordinates from the observing focal plane
 array to each satellite in the list, <cite>satellites</cite>. Track mode can be either
 <cite>rate</cite> or <cite>sidereal</cite>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
@@ -78,14 +79,23 @@
       Create a Skyfield topocentric object which represents the location of a
       place on the planet Earth.
         Parameters:
                 * lat âstring or float, latitude in degrees
                 * lon âstring or float, longitude in degrees
         Returns:
             AToposSkyfield object on the planet Earth
+  satsim.geometry.astrometric.eci_to_ecr(time, ra, dec, roll=0)ï
+      Covert an Earth centered fixed sky coordinates to Earth centered
+      rotating.
+        Parameters:
+                * ra âfloat, right ascension in degrees
+                * dec âfloat, declination in degrees
+                * roll âfloat, field rotation (ignored)
+        Returns:
+            Afloat, ra, dec and roll in degrees
   satsim.geometry.astrometric.gen_track(height, width, y_fov, x_fov, observer,
   track, satellites, brightnesses, t0, tt, rot=0, pad_mult=0,
   track_type='rate', offset=[0, 0], flipud=False, fliplr=False, az=None,
   el=None)ï
       Generates a list of pixel coordinates from the observing focal plane
       array to each satellite in the list,satellites. Track mode can be
       eitherrateorsidereal.
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.image.html` & `satsim-0.14.0/docs/_build/html/api/satsim.image.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.image package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.image package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.io.html` & `satsim-0.14.0/docs/_build/html/api/satsim.io.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.io package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.io package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
@@ -110,15 +111,15 @@
 <dl class="py class">
 <dt class="sig sig-object py" id="satsim.io.czml.CZMLExtractor">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">satsim.io.czml.</span></span><span class="sig-name descname"><span class="pre">CZMLExtractor</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">start_epoch</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_epoch</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">multiplier</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">60</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor" title="Permalink to this definition"></a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
 <p>A class for extracting SatSim data to Cesium</p>
 <dl class="py method">
 <dt class="sig sig-object py" id="satsim.io.czml.CZMLExtractor.add_ground_station">
-<span class="sig-name descname"><span class="pre">add_ground_station</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">pos</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_ground_station" title="Permalink to this definition"></a></dt>
+<span class="sig-name descname"><span class="pre">add_ground_station</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">pos</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sensor</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_name</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">id_description</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_fill_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_outline_color</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[255,</span> <span class="pre">255,</span> <span class="pre">0,</span> <span class="pre">255]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_font</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'16pt</span> <span class="pre">Lucida</span> <span class="pre">Console'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_text</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label_show</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.CZMLExtractor.add_ground_station" title="Permalink to this definition"></a></dt>
 <dd><p>Adds a ground station</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>pos</strong> – <cite>list [~astropy.units]</cite>, coordinates of ground station (i.e. latitude, longitude, altitude)</p></li>
 <li><p><strong>id_description</strong> – <cite>str</cite>, Set ground station description</p></li>
 <li><p><strong>label_fill_color</strong> – <cite>list (int)</cite>, Fill Color in rgba format</p></li>
@@ -166,15 +167,15 @@
 </dl>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.czml.save_czml">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.czml.</span></span><span class="sig-name descname"><span class="pre">save_czml</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">obs_cache</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filename</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.save_czml" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.czml.</span></span><span class="sig-name descname"><span class="pre">save_czml</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">ssp</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">obs_cache</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filename</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.czml.save_czml" title="Permalink to this definition"></a></dt>
 <dd><p>Saves scenario as a Cesium czml file.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>ssp</strong> – <cite>dict</cite>, SatSim input configuration.</p></li>
 <li><p><strong>obs_cache</strong> – <cite>list</cite>, list of SatSim Skyfield objects.</p></li>
 <li><p><strong>filename</strong> – <cite>str</cite>, if not None, save czml output. default=None</p></li>
@@ -187,15 +188,15 @@
 </dd></dl>
 
 </section>
 <section id="module-satsim.io.fits">
 <span id="satsim-io-fits-module"></span><h2>satsim.io.fits module<a class="headerlink" href="#module-satsim.io.fits" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.fits.save">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">3,</span> <span class="pre">15,</span> <span class="pre">9,</span> <span class="pre">14,</span> <span class="pre">57,</span> <span class="pre">258170)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2023,</span> <span class="pre">4,</span> <span class="pre">13,</span> <span class="pre">9,</span> <span class="pre">49,</span> <span class="pre">34,</span> <span class="pre">855695)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
 <dd><p>Save a SatNet compatible FITS file.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>filename</strong> – <cite>string</cite>, the FITS filename.</p></li>
 <li><p><strong>fpa</strong> – <cite>np.array</cite>, input image as a 2D numpy array.</p></li>
 <li><p><strong>exposure_time</strong> – <cite>float</cite>, exposure time for header.</p></li>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
@@ -39,15 +40,15 @@
 ****** satsim.io packageï ******
 ***** Submodulesï *****
 
 ***** satsim.io.czml moduleï *****
   classsatsim.io.czml.CZMLExtractor(start_epoch, end_epoch, multiplier=60)ï
       Bases: object
       A class for extracting SatSim data to Cesium
-        add_ground_station(pos, id_name=None, id_description=None,
+        add_ground_station(pos, sensor, id_name=None, id_description=None,
         label_fill_color=[255, 255, 0, 255], label_outline_color=[255, 255, 0,
         255], label_font='16pt Lucida Console', label_text=None,
         label_show=False)ï
             Adds a ground station
               Parameters:
                       * pos âlist [~astropy.units], coordinates of ground
                         station (i.e. latitude, longitude, altitude)
@@ -86,26 +87,26 @@
                       * label_text âstr, Set label text
                       * label_show âbool, Indicates whether the label is
                         visible
         get_document()ï
             Retrieves CZML document.
               Returns:
                   ADocument, the CZML document.
-  satsim.io.czml.save_czml(ssp, obs_cache, filename)ï
+  satsim.io.czml.save_czml(ssp, obs_cache, astrometrics, filename)ï
       Saves scenario as a Cesium czml file.
         Parameters:
                 * ssp âdict, SatSim input configuration.
                 * obs_cache âlist, list of SatSim Skyfield objects.
                 * filename âstr, if not None, save czml output. default=None
         Returns:
             Adict, the CZML output
 
 ***** satsim.io.fits moduleï *****
   satsim.io.fits.save(filename, fpa, exposure_time=0,
-  dt_start=datetime.datetime(2023, 3, 15, 9, 14, 57, 258170), header={},
+  dt_start=datetime.datetime(2023, 4, 13, 9, 49, 34, 855695), header={},
   overwrite=False, dtype='uint16', astrometrics=None)ï
       Save a SatNet compatible FITS file.
         Parameters:
                 * filename âstring, the FITS filename.
                 * fpa ânp.array, input image as a 2D numpy array.
                 * exposure_time âfloat, exposure time for header.
                 * dt_start âdatatime, datetime of start of exposure.
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.math.html` & `satsim-0.14.0/docs/_build/html/api/satsim.math.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.math package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.math package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
@@ -163,14 +164,17 @@
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>A <cite>float</cite>, mean of a0 and a1</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
+<section id="module-satsim.math.const">
+<span id="satsim-math-const-module"></span><h2>satsim.math.const module<a class="headerlink" href="#module-satsim.math.const" title="Permalink to this heading"></a></h2>
+</section>
 <section id="module-satsim.math.conv">
 <span id="satsim-math-conv-module"></span><h2>satsim.math.conv module<a class="headerlink" href="#module-satsim.math.conv" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.math.conv.conv2">
 <span class="sig-prename descclassname"><span class="pre">satsim.math.conv.</span></span><span class="sig-name descname"><span class="pre">conv2</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">x</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">y</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pad</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">32</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">tf.float32</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.math.conv.conv2" title="Permalink to this definition"></a></dt>
 <dd><p>Convolve two 2-dimensional arrays with traditional convolution.</p>
 <dl class="field-list simple">
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
@@ -75,14 +76,16 @@
                 * max_diff âfloat, maximum angle difference before
                   concidering the opposite angle. default=180.
                 * normalize_360 âboolean, normalize angle between 0 and 360.
                   default=True
         Returns:
             Afloat, mean of a0 and a1
 
+***** satsim.math.const moduleï *****
+
 ***** satsim.math.conv moduleï *****
   satsim.math.conv.conv2(x, y, pad=32, dtype=tf.float32)ï
       Convolve two 2-dimensional arrays with traditional convolution.
         Parameters:
                 * x âTensor, input image as a 2D tensor.
                 * y âTensor, input kernel as a 2D tensor.
                 * dtype âdtype,float32,complex64orcomplex128
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.pipeline.html` & `satsim-0.14.0/docs/_build/html/api/satsim.pipeline.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.pipeline package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.pipeline package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.time.html` & `satsim-0.14.0/docs/_build/html/api/satsim.time.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.time package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.time package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.time package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.util.html">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
@@ -154,14 +155,31 @@
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>A <cite>list</cite> of Skyfield times equally spaced between <cite>t0</cite> and <cite>t1</cite>.</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
+<dt class="sig sig-object py" id="satsim.time.mid">
+<span class="sig-prename descclassname"><span class="pre">satsim.time.</span></span><span class="sig-name descname"><span class="pre">mid</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">t1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.time.mid" title="Permalink to this definition"></a></dt>
+<dd><p>Return the mid of two times.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>t0</strong> – <cite>Time</cite>, start Skyfield <cite>Time</cite></p></li>
+<li><p><strong>t1</strong> – <cite>Time</cite>, end Skyfield <cite>Time</cite></p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>Time</cite>, mid Skyfield <cite>Time</cite></p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
 <dt class="sig sig-object py" id="satsim.time.to_astropy">
 <span class="sig-prename descclassname"><span class="pre">satsim.time.</span></span><span class="sig-name descname"><span class="pre">to_astropy</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">t</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.time.to_astropy" title="Permalink to this definition"></a></dt>
 <dd><p>Convert a Skyfield <cite>Time</cite> object to an AstroPy <cite>Time</cite>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><strong>t</strong> – <cite>Time</cite>, a Skyfield <cite>Time</cite></p>
 </dd>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
@@ -55,14 +56,21 @@
       Return evenly spaced Skyfield times over a specified interval.
         Parameters:
                 * t0 âTime, start SkyfieldTime
                 * t1 âTime, end SkyfieldTime
                 * num âint, number of samples to generate. default=50
         Returns:
             Alistof Skyfield times equally spaced betweent0andt1.
+  satsim.time.mid(t0, t1)ï
+      Return the mid of two times.
+        Parameters:
+                * t0 âTime, start SkyfieldTime
+                * t1 âTime, end SkyfieldTime
+        Returns:
+            ATime, mid SkyfieldTime
   satsim.time.to_astropy(t)ï
       Convert a SkyfieldTimeobject to an AstroPyTime.
         Parameters:
             t âTime, a SkyfieldTime
         Returns:
             An AstroPyTimeobject
   satsim.time.to_utc_list(t)ï
```

### Comparing `satsim-0.13.1/docs/_build/html/api/satsim.util.html` & `satsim-0.14.0/docs/_build/html/api/satsim.util.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.util package &mdash; SatSim 0.13.0 documentation</title>
+  <title>satsim.util package &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
         <script src="../_static/doctools.js"></script>
         <script src="../_static/sphinx_highlight.js"></script>
     <script src="../_static/js/theme.js"></script>
     <link rel="index" title="Index" href="../genindex.html" />
     <link rel="search" title="Search" href="../search.html" />
-    <link rel="next" title="Credits" href="../authors.html" />
+    <link rel="next" title="satsim.vecmath package" href="satsim.vecmath.html" />
     <link rel="prev" title="satsim.time package" href="satsim.time.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -56,14 +56,15 @@
 <li class="toctree-l4"><a class="reference internal" href="satsim.geometry.html">satsim.geometry package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.image.html">satsim.image package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.io.html">satsim.io package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.math.html">satsim.math package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.pipeline.html">satsim.pipeline package</a></li>
 <li class="toctree-l4"><a class="reference internal" href="satsim.time.html">satsim.time package</a></li>
 <li class="toctree-l4 current"><a class="current reference internal" href="#">satsim.util package</a></li>
+<li class="toctree-l4"><a class="reference internal" href="satsim.vecmath.html">satsim.vecmath package</a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#submodules">Submodules</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.cli">satsim.cli module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.config">satsim.config module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.html#module-satsim.satsim">satsim.satsim module</a></li>
 </ul>
@@ -325,15 +326,15 @@
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
         <a href="satsim.time.html" class="btn btn-neutral float-left" title="satsim.time package" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="../authors.html" class="btn btn-neutral float-right" title="Credits" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+        <a href="satsim.vecmath.html" class="btn btn-neutral float-right" title="satsim.vecmath package" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Space Force.</p>
   </div>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
           o satsim_package
@@ -20,14 +20,15 @@
                       # satsim.geometry_package
                       # satsim.image_package
                       # satsim.io_package
                       # satsim.math_package
                       # satsim.pipeline_package
                       # satsim.time_package
                       # satsim.util_package
+                      # satsim.vecmath_package
                 # Submodules
                 # satsim.cli_module
                 # satsim.config_module
                 # satsim.satsim_module
     * Credits
     * History
    SatSim
```

### Comparing `satsim-0.13.1/docs/_build/html/authors.html` & `satsim-0.14.0/docs/_build/html/authors.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Credits &mdash; SatSim 0.13.0 documentation</title>
+  <title>Credits &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="History" href="history.html" />
-    <link rel="prev" title="satsim.util package" href="api/satsim.util.html" /> 
+    <link rel="prev" title="satsim.vecmath package" href="api/satsim.vecmath.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
         <div class="wy-side-nav-search" >
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -95,15 +95,15 @@
 </section>
 </section>
 
 
            </div>
           </div>
           <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="api/satsim.util.html" class="btn btn-neutral float-left" title="satsim.util package" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="api/satsim.vecmath.html" class="btn btn-neutral float-left" title="satsim.vecmath package" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
         <a href="history.html" class="btn btn-neutral float-right" title="History" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023, Space Force.</p>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.13.1/docs/_build/html/contributing.html` & `satsim-0.14.0/docs/_build/html/contributing.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Contributing &mdash; SatSim 0.13.0 documentation</title>
+  <title>Contributing &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
           o Getting_Started_for_Developers
           o Merge_Request_Guidelines
```

### Comparing `satsim-0.13.1/docs/_build/html/history.html` & `satsim-0.14.0/docs/_build/html/history.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>History &mdash; SatSim 0.13.0 documentation</title>
+  <title>History &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -46,36 +46,37 @@
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="contributing.html">Contributing</a></li>
 <li class="toctree-l1"><a class="reference internal" href="api.html">API Documentation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#id1">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id2">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id3">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id4">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id5">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id6">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id7">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id8">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id9">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id10">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id12">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id13">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id14">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id15">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id16">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id17">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id18">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id19">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id20">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id21">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id22">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id1">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id2">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id3">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id4">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id5">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id6">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id7">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id8">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id9">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id10">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id11">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id12">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id13">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id14">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id15">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id16">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id17">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id18">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id19">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id20">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id21">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id22">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id23">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -99,212 +100,218 @@
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="history">
 <h1>History<a class="headerlink" href="#history" title="Permalink to this heading"></a></h1>
 <section id="id1">
-<h2>0.13.1<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<h2>0.14.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<p>Add vector math library.
+Add CZML output for sensor visualization.
+Fix objects not updating properly when image renderer is off.</p>
+</section>
+<section id="id2">
+<h2>0.13.1<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add argument to set folder name in <cite>gen_multi</cite>.</p></li>
 <li><p>Add environment variable, <cite>SATSIM_SKYFIELD_LOAD_DIR</cite>, to specify location of Skyfield ephemeris files.</p></li>
 <li><p>Fix incorrect CZML output when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id2">
-<h2>0.13.0<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
+<section id="id3">
+<h2>0.13.0<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add ephemeris objects that are propagated with the Lagrange interpolator.</p></li>
 <li><p>Add Cesium CZML output. Set sim option <cite>save_czml</cite> to <cite>false</cite> to disable.</p></li>
 <li><p>Add CSV text file star catalog loader. This feature is useful for small catalogs such as Hipparcos and simulating wide FOV sensors.</p></li>
 <li><p>Add multiplier and clipping for radial cosine.</p></li>
 <li><p>Add option to skip image rendering. Set sim option <cite>mode</cite> to <cite>none</cite> to bypass image rendering.</p></li>
 <li><p>Update interfaces for newest version of Skyfield, Poliastro, POPPY, and AstroPy.</p></li>
 <li><p>Fix star renderer issue removing stars in field of view for non-square arrays.</p></li>
 </ul>
 </section>
-<section id="id3">
-<h2>0.12.0<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
+<section id="id4">
+<h2>0.12.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add augmentation of SatNet <cite>tf.data.Dataset</cite>. This feature allows injecting synthetic targets into real data during training.</p></li>
 <li><p>Add FFT convolution to <cite>add_patch</cite> sprite render and <cite>scatter_shift</cite> image augmenter for speed improvement.</p></li>
 <li><p>Add cache last PSF FFT to <cite>fftconv2p</cite> for speed improvement for static PSFs.</p></li>
 <li><p>Add two-body state vector as a trackable target.</p></li>
 <li><p>Add moon and sun model and misc methods to calculate phase angle and target brightness.</p></li>
 </ul>
 </section>
-<section id="id4">
-<h2>0.11.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
+<section id="id5">
+<h2>0.11.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to render star motion with FFT. Set sim option <cite>star_render_mode</cite> to <cite>fft</cite>.</p></li>
 <li><p>Add option to sample photon noise multiple times. Set sim option <cite>num_shot_noise_samples</cite> to integer number.</p></li>
 <li><p>Add support to render a satellite as a sprite. Set <cite>model</cite> option in obs.</p></li>
 <li><p>Add support to load and augment sprite model with <cite>$pipeline</cite> operator.</p></li>
 <li><p>Add cropped POPPY PSF generation.</p></li>
 <li><p>Fix GreatCircle propagator tracking offset.</p></li>
 <li><p>Fix runtime exception when site and track_mode are not defined.</p></li>
 <li><p>Add TensorFlow 2.6 and update TensorFlow 2.2 and 2.4 Docker build file.</p></li>
 </ul>
 </section>
-<section id="id5">
-<h2>0.10.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
+<section id="id6">
+<h2>0.10.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for piecewise rendering. Set sim option <cite>render_size</cite> to enable. For example, [256, 256].</p></li>
 <li><p>Add <cite>fixed</cite> tracking mode with mount azimuth and elevation.</p></li>
 <li><p>Add great circle propagator for targets.</p></li>
 <li><p>Add in-memory image generation. See generator function <cite>image_generator</cite>.</p></li>
 <li><p>Fix missing stars when FOV crosses zero degree RA.</p></li>
 <li><p>Add curved targets using bezier curve raster. Enabled by default. Set sim option <cite>num_target_samples</cite> to 2 to enable linear raster.</p></li>
 <li><p>Add LRU cache to star catalog reader.</p></li>
 <li><p>Add option to turn off SNR calculation. Set sim option <cite>calculate_snr</cite> to false will render targets and stars together.</p></li>
 <li><p>Handle unstable SGP4 TLEs.</p></li>
 <li><p>Add TensorFlow 2.4 Docker build file.</p></li>
 <li><p>Add debug output for pristine images of targets and stars.</p></li>
 </ul>
 </section>
-<section id="id6">
-<h2>0.9.1<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
+<section id="id7">
+<h2>0.9.1<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Calculate POPPY input wavefront resolution to avoid PSF aliasing.</p></li>
 <li><p>Add support for additional FITS image data types (<cite>int16</cite>, <cite>uint16</cite>, <cite>int32</cite>, <cite>uint32</cite>, <cite>float32</cite>).</p></li>
 <li><p>Add batch processing to <cite>transform_and_add_counts</cite> to support batch processing of stars.</p></li>
 <li><p>Add <cite>auto</cite> option to calculate temporal oversample factor based on star velocities.</p></li>
 <li><p>Add option to turn off serializing config data to pickle file (<cite>save_pickle</cite>).</p></li>
 <li><p>Add option to turn off png movie output (<cite>save_movie</cite>).</p></li>
 <li><p>Add <cite>crop_and_resize</cite> and <cite>flip</cite> image augmentation.</p></li>
 <li><p>Set pixels with values beyond the pixel data type’s capacity to the maximum value for that data type.</p></li>
 <li><p>Add <cite>lognormal</cite> function to generate a distribution with a true target mean.</p></li>
 <li><p>Fix issue with sidereal track.</p></li>
 <li><p>Fix issue with fragment velocity not being randomly sampled.</p></li>
 </ul>
 </section>
-<section id="id7">
-<h2>0.9.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
+<section id="id8">
+<h2>0.9.0<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add Physical Optics Propagation in Python (POPPY) PSF generation.</p></li>
 <li><p>Add PSF augmentation with <cite>$pipeline</cite> replacement key.</p></li>
 <li><p>Add <cite>$function</cite> and <cite>$compound</cite> replacement key.</p></li>
 <li><p>Add ability to generate stray light from a <cite>$function</cite> replacement key.</p></li>
 <li><p>Add built-in 2D polynomial image generator for stray light, <cite>polygrid2d</cite>.</p></li>
 <li><p>Add built-in cosine fourth image generator for irradiance falloff, <cite>radial_cos2d</cite>.</p></li>
 <li><p>Add built-in sine wave image generator for fix pattern noise, <cite>sin2d</cite>.</p></li>
 <li><p>Add built-in image generator from AstroPy model, <cite>astropy_model2d</cite>.</p></li>
 <li><p>Add built-in image augmentation, <cite>scatter_shift</cite> and <cite>scatter_shift_polar</cite>.</p></li>
 <li><p>Add <cite>$cache</cite> replacement key (caching works for PSF and <cite>$function</cite>).</p></li>
 </ul>
 </section>
-<section id="id8">
-<h2>0.8.3<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
+<section id="id9">
+<h2>0.8.3<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix new Skyfield incompatibility.</p></li>
 </ul>
 </section>
-<section id="id9">
-<h2>0.8.2<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
+<section id="id10">
+<h2>0.8.2<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Prefix replacement keys with <cite>$</cite> in SatSim configuration file.</p></li>
 <li><p>Add option to scale collision fragments by cosine of the exit angle.</p></li>
 </ul>
 </section>
-<section id="id10">
-<h2>0.8.1<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
+<section id="id11">
+<h2>0.8.1<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add astrometric metadata into FITS header</p></li>
 <li><p>Refactor WCS library</p></li>
 <li><p>Add option to flip images about x or y axis</p></li>
 <li><p>Add option to refresh stars for each frame</p></li>
 <li><p>Add RPO from TLE generator</p></li>
 </ul>
 </section>
-<section id="id11">
-<h2>0.8.0<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
+<section id="id12">
+<h2>0.8.0<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add two body propagator</p></li>
 <li><p>Add object <cite>create</cite>, <cite>delete</cite>, and <cite>update</cite> events</p></li>
 <li><p>Add collision generator</p></li>
 <li><p>Add breakup generator</p></li>
 <li><p>Add <cite>ref</cite> keyword to configuration</p></li>
 <li><p>Add <cite>key</cite> keyword to <cite>import</cite> configuration</p></li>
 <li><p>Refactor astrometric library</p></li>
 </ul>
 </section>
-<section id="id12">
-<h2>0.7.2<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
+<section id="id13">
+<h2>0.7.2<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to specify star and obs velocity in polar coordinates</p></li>
 </ul>
 </section>
-<section id="id13">
-<h2>0.7.1<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
+<section id="id14">
+<h2>0.7.1<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to turn off shot noise: <cite>sim.enable_shot_noise: true</cite></p></li>
 <li><p>Add option to turn off annotation boxes in image: <cite>sim.show_obs_boxes: true</cite></p></li>
 <li><p>Add option to specify velocity in arcseconds: <cite>sim.velocity_units: arcsec</cite></p></li>
 <li><p>Fix PNG output threading issue</p></li>
 </ul>
 </section>
-<section id="id14">
-<h2>0.7.0<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
+<section id="id15">
+<h2>0.7.0<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add function pipelines to support variable target brightness</p></li>
 </ul>
 </section>
-<section id="id15">
-<h2>0.6.1<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
+<section id="id16">
+<h2>0.6.1<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix built-in generators not included in distribution</p></li>
 <li><p>Add dockerfile</p></li>
 </ul>
 </section>
-<section id="id16">
-<h2>0.6.0<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
+<section id="id17">
+<h2>0.6.0<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add configuration import.</p></li>
 <li><p>Add configuration generator functions.</p></li>
 <li><p>Add built-in generator for breakups.</p></li>
 <li><p>Add built-in generator for CSOs.</p></li>
 <li><p>Add built-in generator for loading TLE files.</p></li>
 </ul>
 </section>
-<section id="id17">
-<h2>0.5.0<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
+<section id="id18">
+<h2>0.5.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Runtime optimization.</p></li>
 <li><p>Add parallel processing and multi-gpu utilization.</p></li>
 <li><p>Add option to limit gpu memory usage.</p></li>
 </ul>
 </section>
-<section id="id18">
-<h2>0.4.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
+<section id="id19">
+<h2>0.4.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add signal to noise calculation for target pixels.</p></li>
 </ul>
 </section>
-<section id="id19">
-<h2>0.3.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
+<section id="id20">
+<h2>0.3.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for two line element set SGP4 satellite propagator.</p></li>
 <li><p>Add support for rate and sidereal track from topocentric site.</p></li>
 </ul>
 </section>
-<section id="id20">
-<h2>0.2.0<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
+<section id="id21">
+<h2>0.2.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for SSTR7 star catalog.</p></li>
 </ul>
 </section>
-<section id="id21">
-<h2>0.1.1<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
+<section id="id22">
+<h2>0.1.1<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add target position to annotation file.</p></li>
 <li><p>Updates to run GitLab CI.</p></li>
 </ul>
 </section>
-<section id="id22">
-<h2>0.1.0<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
+<section id="id23">
+<h2>0.1.0<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>First release.</p></li>
 </ul>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
     * History
+          o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
           o 0.9.1
           o 0.9.0
@@ -37,14 +38,18 @@
           o 0.1.1
           o 0.1.0
    SatSim
     * History
     * View_page_source
 ===============================================================================
 ****** Historyï ******
+***** 0.14.0ï *****
+Add vector math library. Add CZML output for sensor visualization. Fix objects
+not updating properly when image renderer is off.
+
 ***** 0.13.1ï *****
     * Add argument to set folder name ingen_multi.
     * Add environment variable,SATSIM_SKYFIELD_LOAD_DIR, to specify location of
       Skyfield ephemeris files.
     * Fix incorrect CZML output when image renderer is off.
 
 ***** 0.13.0ï *****
```

### Comparing `satsim-0.13.1/docs/_build/html/index.html` & `satsim-0.14.0/docs/_build/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Documentation for SatSim &mdash; SatSim 0.13.0 documentation</title>
+  <title>Documentation for SatSim &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -106,36 +106,37 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#development-lead">Development Lead</a></li>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#contributors">Contributors</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
@@ -35,14 +35,15 @@
           o Other_Ways_of_Contributing
     * API_Documentation
           o satsim_package
     * Credits
           o Development_Lead
           o Contributors
     * History
+          o 0.14.0
           o 0.13.1
           o 0.13.0
           o 0.12.0
           o 0.11.0
           o 0.10.0
           o 0.9.1
           o 0.9.0
```

### Comparing `satsim-0.13.1/docs/_build/html/installation.html` & `satsim-0.14.0/docs/_build/html/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; SatSim 0.13.0 documentation</title>
+  <title>Installation &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
           o Stable_Release
           o From_Sources
     * Usage
     * Contributing
```

### Comparing `satsim-0.13.1/docs/_build/html/py-modindex.html` & `satsim-0.14.0/docs/_build/html/py-modindex.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; SatSim 0.13.0 documentation</title>
+  <title>Python Module Index &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -277,14 +277,19 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.math.html#module-satsim.math.angle"><code class="xref">satsim.math.angle</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="api/satsim.math.html#module-satsim.math.const"><code class="xref">satsim.math.const</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="api/satsim.math.html#module-satsim.math.conv"><code class="xref">satsim.math.conv</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.math.html#module-satsim.math.fft"><code class="xref">satsim.math.fft</code></a></td><td>
        <em></em></td></tr>
@@ -334,14 +339,54 @@
        <a href="api/satsim.util.html#module-satsim.util.thread"><code class="xref">satsim.util.thread</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.util.html#module-satsim.util.timer"><code class="xref">satsim.util.timer</code></a></td><td>
        <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath"><code class="xref">satsim.vecmath</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Cartesian2"><code class="xref">satsim.vecmath.Cartesian2</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Cartesian3"><code class="xref">satsim.vecmath.Cartesian3</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Cartesian4"><code class="xref">satsim.vecmath.Cartesian4</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Matrix2"><code class="xref">satsim.vecmath.Matrix2</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Matrix3"><code class="xref">satsim.vecmath.Matrix3</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Matrix4"><code class="xref">satsim.vecmath.Matrix4</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
+       <a href="api/satsim.vecmath.html#module-satsim.vecmath.Quaternion"><code class="xref">satsim.vecmath.Quaternion</code></a></td><td>
+       <em></em></td></tr>
    </table>
 
 
            </div>
           </div>
           <footer>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
@@ -54,23 +54,32 @@
         satsim.io
         satsim.io.czml
         satsim.io.fits
         satsim.io.image
         satsim.io.satnet
         satsim.math
         satsim.math.angle
+        satsim.math.const
         satsim.math.conv
         satsim.math.fft
         satsim.math.interpolate
         satsim.math.random
         satsim.math.stats
         satsim.pipeline
         satsim.satsim
         satsim.time
         satsim.util
         satsim.util.system
         satsim.util.thread
         satsim.util.timer
+        satsim.vecmath
+        satsim.vecmath.Cartesian2
+        satsim.vecmath.Cartesian3
+        satsim.vecmath.Cartesian4
+        satsim.vecmath.Matrix2
+        satsim.vecmath.Matrix3
+        satsim.vecmath.Matrix4
+        satsim.vecmath.Quaternion
 
 ===============================================================================
 © Copyright 2023, Space Force.
 Built with Sphinx using a theme provided by Read_the_Docs.
```

### Comparing `satsim-0.13.1/docs/_build/html/search.html` & `satsim-0.14.0/docs/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; SatSim 0.13.0 documentation</title>
+  <title>Search &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
     * Contributing
     * API_Documentation
     * Credits
```

### Comparing `satsim-0.13.1/docs/_build/html/usage.html` & `satsim-0.14.0/docs/_build/html/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Usage &mdash; SatSim 0.13.0 documentation</title>
+  <title>Usage &mdash; SatSim 0.14.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.13.0
+                0.14.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 
 
 
 SatSim
-0.13.0
+0.14.0
 [q                   ]
 Contents:
     * Installation
     * Usage
           o Python_Module
           o Command_Line_Interface
           o Parameters_and_Configuration
```

### Comparing `satsim-0.13.1/docs/api/satsim.generator.obs.rst` & `satsim-0.14.0/docs/api/satsim.generator.obs.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/api/satsim.geometry.rst` & `satsim-0.14.0/docs/api/satsim.geometry.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/api/satsim.image.rst` & `satsim-0.14.0/docs/api/satsim.image.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/api/satsim.io.rst` & `satsim-0.14.0/docs/api/satsim.io.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/api/satsim.math.rst` & `satsim-0.14.0/docs/api/satsim.math.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 ------------------------
 
 .. automodule:: satsim.math.angle
    :members:
    :undoc-members:
    :show-inheritance:
 
+satsim.math.const module
+------------------------
+
+.. automodule:: satsim.math.const
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 satsim.math.conv module
 -----------------------
 
 .. automodule:: satsim.math.conv
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `satsim-0.13.1/docs/api/satsim.rst` & `satsim-0.14.0/docs/api/satsim.rst`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
    satsim.geometry
    satsim.image
    satsim.io
    satsim.math
    satsim.pipeline
    satsim.time
    satsim.util
+   satsim.vecmath
 
 Submodules
 ----------
 
 satsim.cli module
 -----------------
```

### Comparing `satsim-0.13.1/docs/api/satsim.util.rst` & `satsim-0.14.0/docs/api/satsim.util.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/conf.py` & `satsim-0.14.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 author = u"Alex Cabello"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '0.13.0'
+version = '0.14.0'
 # The full version, including alpha/beta/rc tags.
-release = '0.13.0'
+release = '0.14.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `satsim-0.13.1/docs/installation.rst` & `satsim-0.14.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/make.bat` & `satsim-0.14.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/docs/usage.rst` & `satsim-0.14.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/cli.py` & `satsim-0.14.0/satsim/cli.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/config.py` & `satsim-0.14.0/satsim/config.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/dataset/augment.py` & `satsim-0.14.0/satsim/dataset/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/generator/obs/breakup.py` & `satsim-0.14.0/satsim/generator/obs/breakup.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/generator/obs/cso.py` & `satsim-0.14.0/satsim/generator/obs/cso.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/generator/obs/geometry.py` & `satsim-0.14.0/satsim/generator/obs/geometry.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/generator/obs/io.py` & `satsim-0.14.0/satsim/generator/obs/io.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/generator/obs/rpo.py` & `satsim-0.14.0/satsim/generator/obs/rpo.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/astrometric.py` & `satsim-0.14.0/satsim/geometry/astrometric.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
 if 'SATSIM_SKYFIELD_LOAD_DIR' in os.environ:
     from skyfield.api import Loader
     load = Loader(os.environ['SATSIM_SKYFIELD_LOAD_DIR'])
 else:
     from skyfield.api import load
 
+from astropy.coordinates import SkyCoord, ICRS, ITRS
+from astropy.time import Time
+from astropy.coordinates import cartesian_to_spherical
+from astropy import units as u
+
 from satsim.geometry.wcs import get_min_max_ra_dec, get_wcs
 
 
 SATSIM_EARTH = None
 SATSIM_MOON = None
 SATSIM_SUN = None
 
@@ -178,15 +183,15 @@
             target_au, observer_gcrs_au)
         include_earth_deflection = nadir_angle >= 0.8
 
     if deflection:
         add_deflection(target_au, bcrs_position,
                        p._ephemeris, t, include_earth_deflection)
 
-    if aberration:
+    if aberration and p.light_time is not None:
         add_aberration(target_au, bcrs_velocity, p.light_time)
 
     apparent = Apparent(target_au, None, t, p.center, p.target)
     apparent.center_barycentric = p.center_barycentric
     apparent._observer_gcrs_au = observer_gcrs_au
     return apparent
 
@@ -551,7 +556,29 @@
     phase_factor = np.sin(phase_angle) + (np.pi - phase_angle) * np.cos(phase_angle)
     intensity = phase_factor * (2 * albedo * (radius * radius)) / (3 * np.pi * (distance * distance))
 
     # Convert intensities to magnitudes
     mvVector = mv_sun - 2.5 * np.log10(intensity)
 
     return mvVector
+
+
+def eci_to_ecr(time, ra, dec, roll=0):
+    """Covert an Earth centered fixed sky coordinates to Earth centered rotating.
+
+    Args:
+        ra: `float`, right ascension in degrees
+        dec: `float`, declination in degrees
+        roll: `float`, field rotation (ignored)
+
+    Returns:
+        A `float`, ra, dec and roll in degrees
+    """
+    sc = SkyCoord(ra=ra, dec=dec, unit='deg', frame=ICRS)
+    sc2 = sc.transform_to(ITRS(obstime=Time(time)))
+    sc3 = SkyCoord(sc2)
+
+    _, dec, ra = cartesian_to_spherical(sc3.x, sc3.y, sc3.z)
+    dec = dec + 270 * u.deg
+    ra = -ra
+
+    return ra, dec, roll
```

### Comparing `satsim-0.13.1/satsim/geometry/csvsc.py` & `satsim-0.14.0/satsim/geometry/csvsc.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/draw.py` & `satsim-0.14.0/satsim/geometry/draw.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/ephemeris.py` & `satsim-0.14.0/satsim/geometry/ephemeris.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/random.py` & `satsim-0.14.0/satsim/geometry/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/sgp4.py` & `satsim-0.14.0/satsim/geometry/sgp4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/sprite.py` & `satsim-0.14.0/satsim/geometry/sprite.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/sstr7.py` & `satsim-0.14.0/satsim/geometry/sstr7.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/transform.py` & `satsim-0.14.0/satsim/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/twobody.py` & `satsim-0.14.0/satsim/geometry/twobody.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/geometry/wcs.py` & `satsim-0.14.0/satsim/geometry/wcs.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/augment.py` & `satsim-0.14.0/satsim/image/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/fpa.py` & `satsim-0.14.0/satsim/image/fpa.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/model.py` & `satsim-0.14.0/satsim/image/model.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/noise.py` & `satsim-0.14.0/satsim/image/noise.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/psf.py` & `satsim-0.14.0/satsim/image/psf.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/image/render.py` & `satsim-0.14.0/satsim/image/render.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/io/czml.py` & `satsim-0.14.0/satsim/io/czml.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,37 @@
 from astropy import units as u
 
 from skyfield.constants import AU_KM
 from skyfield.units import _ltude
 from skyfield.vectorlib import VectorFunction
 
 from satsim import time
-from satsim.geometry.astrometric import load_earth
+from satsim.geometry.astrometric import load_earth, eci_to_ecr
+from satsim.vecmath import Quaternion
 
 from czmlpy.core import Document, Packet, Preamble
-from czmlpy.enums import InterpolationAlgorithms, ReferenceFrames
+from czmlpy.enums import InterpolationAlgorithms, ReferenceFrames, ExtrapolationTypes
 from czmlpy.properties import (
     Billboard,
     Clock,
     Color,
     Label,
     Material,
     Path,
     Position,
     SolidColorMaterial,
+    RectangularSensor,
+    Orientation,
+    Double,
 )
 from czmlpy.types import IntervalValue, TimeInterval
 from erfa import gd2gc
 
 
-def save_czml(ssp, obs_cache, filename):
+def save_czml(ssp, obs_cache, astrometrics, filename):
     """Saves scenario as a Cesium czml file.
 
     Args:
         ssp: `dict`, SatSim input configuration.
         obs_cache: `list`, list of SatSim Skyfield objects.
         filename: `str`, if not None, save czml output. default=None
 
@@ -67,15 +71,24 @@
         alt = site['alt'] * u.m
 
         name = site['name'] if 'name' in site else None
         label_show = False
 
         if 'czml' in site:
             label_show = site['czml'].get('path_show', label_show)
-        extractor.add_ground_station([latitude, longitude, alt], label_text=name, label_show=label_show)
+
+        sensor = {
+            'y_fov': astrometrics[0]['y_fov'],
+            'x_fov': astrometrics[0]['x_fov'],
+            'time': [x['time'] for x in astrometrics],
+            'quat': [list(_equatorial_to_ecr_quaternion(x['ra'], x['dec'], 0.0, x['time'])) for x in astrometrics],
+            'range': [x['range'] for x in astrometrics],
+        }
+
+        extractor.add_ground_station([latitude, longitude, alt], sensor, label_text=name, label_show=label_show)
 
     # extract objects data
     for i, o in enumerate(ssp['geometry']['obs']['list']):
 
         ts_start_ob = t0
         ts_end_ob = t2
         if 'events' in o:
@@ -135,14 +148,29 @@
     "hPrZDRDcMgDAU9GqN0lIzijw6SUbJJygUeNQgSqepJTyHG91LVVpwDdfxM3T9TSl1EXZvDwi"
     "i471fivK73cBFFQNTT/d2KoGpfGOpSIkhUpgUMxq9DFEsWv4IXhlyCnhBFnZcFEEuYqbiUlN"
     "wWgMTdrZ3JbQFoEVG53rd8ztG9aPJMnBUQf/VFraBJeWnLS0RfjbKyLJA8FkT5seDYS1Qwyv"
     "8t0B/5C2ZmH2/eTGNNBgMmAAAAAElFTkSuQmCC"
 )
 
 
+def _equatorial_to_ecr_quaternion(ra, dec, roll=0.0, time=None):
+    """ Converts ECI RA/Dec to ECR Quaternion """
+    ra, dec, roll = eci_to_ecr(time, ra, dec, roll)
+
+    hpr = {
+        'pitch': dec.to(u.rad).value,
+        'heading': ra.to(u.rad).value,
+        'roll': roll
+    }
+
+    q = Quaternion.fromHeadingPitchRoll(hpr)
+
+    return [q.x, q.y, q.z, q.w]
+
+
 class CZMLExtractor:
     """A class for extracting SatSim data to Cesium"""
 
     def __init__(self, start_epoch, end_epoch, multiplier=60):
         """
         Orbital constructor
 
@@ -169,14 +197,15 @@
             ),
         )
         self.packets.append(pckt)
 
     def add_ground_station(
         self,
         pos,
+        sensor,
         id_name=None,
         id_description=None,
         label_fill_color=[255, 255, 0, 255],
         label_outline_color=[255, 255, 0, 255],
         label_font="16pt Lucida Console",
         label_text=None,
         label_show=False
@@ -192,33 +221,73 @@
             label_font: `str`, Set label font style and size (CSS syntax)
             label_text: `str`, Set label text
             label_show: `bool`, Indicates whether the label is visible
         """
         lat, lon, alt = pos
         pos = list(gd2gc(1, lon.to_value(u.rad), lat.to_value(u.rad), alt.to_value(u.m)))
 
+        gs_id = "GS" + str(self.num_gs)
         pckt = Packet(
-            id="GS" + str(self.num_gs),
+            id=gs_id,
             name=id_name,
             description=id_description,
             availability=TimeInterval(start=self.start_epoch, end=self.end_epoch),
             position=Position(cartesian=pos),
             label=Label(
-                show=label_show,
-                text=label_text,
-                font=label_font,
-                fillColor=Color(rgba=label_fill_color),
-                outlineColor=Color(rgba=label_outline_color),
+                show=True,
             ),
             billboard=Billboard(image=PIC_GROUNDSTATION, show=True),
         )
 
         self.packets.append(pckt)
         self.num_gs += 1
 
+        N = len(sensor['quat'])
+        quat = []
+        radius = []
+        for i, t, q, r in zip(range(N), sensor['time'], sensor['quat'], sensor['range']):
+            s = (Time(t) - self.start_epoch).to(u.second).value
+            quat += [s, q[0], q[1], q[2], q[3]]
+            radius += [s, r * 1000]
+
+        # test add sensor
+        pckt = Packet(
+            id=gs_id + "_FOV",
+            parent=gs_id,
+            position=Position(reference=gs_id + "#position"),
+            orientation=Orientation(
+                unitQuaternion=quat,
+                interpolationDegree=1,
+                interpolationAlgorithm=InterpolationAlgorithms.LINEAR,
+                epoch=self.start_epoch.datetime.replace(tzinfo=timezone.utc),
+                forwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE,
+                backwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE
+            ),
+            agi_rectangularSensor=RectangularSensor(
+                show=True,
+                showIntersection=False,
+                intersectionColor=Color(rgba=[255, 255, 255, 255]),
+                intersectionWidth=2,
+                portionToDisplay="COMPLETE",
+                lateralSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=[255, 255, 0, 128]))),
+                domeSurfaceMaterial=Material(solidColor=SolidColorMaterial(color=Color(rgba=[255, 255, 0, 128]))),
+                xHalfAngle=np.radians(sensor['x_fov'] / 2),
+                yHalfAngle=np.radians(sensor['y_fov'] / 2),
+                radius=Double(
+                    number=radius,
+                    interpolationDegree=1,
+                    interpolationAlgorithm=InterpolationAlgorithms.LINEAR,
+                    epoch=self.start_epoch.datetime.replace(tzinfo=timezone.utc),
+                    forwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE,
+                    backwardExtrapolationType=ExtrapolationTypes.EXTRAPOLATE
+                )
+            )
+        )
+        self.packets.append(pckt)
+
     def add_object(
         self,
         sat,
         N=10,
         id_name=None,
         id_description=None,
         path_width=None,
```

### Comparing `satsim-0.13.1/satsim/io/fits.py` & `satsim-0.14.0/satsim/io/fits.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/io/image.py` & `satsim-0.14.0/satsim/io/image.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/io/satnet.py` & `satsim-0.14.0/satsim/io/satnet.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/angle.py` & `satsim-0.14.0/satsim/math/angle.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/conv.py` & `satsim-0.14.0/satsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/fft.py` & `satsim-0.14.0/satsim/math/fft.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/interpolate.py` & `satsim-0.14.0/satsim/math/interpolate.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/random.py` & `satsim-0.14.0/satsim/math/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/math/stats.py` & `satsim-0.14.0/satsim/math/stats.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/pipeline/__init__.py` & `satsim-0.14.0/satsim/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/satsim.py` & `satsim-0.14.0/satsim/satsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,15 +148,17 @@
         'dir.name',
         ['{}.{:04d}.json'.format(set_name,x) for x in range(num_frames)],
         ssp['fpa']['height'],
         ssp['fpa']['width'],
         y_ifov,
         x_ifov)
 
+    astrometrics_list = []
     for fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, num_shot_noise_samples, obs_cache in image_generator(ssp, output_dir, output_debug, dir_debug, with_meta=True, num_sets=1):
+        astrometrics_list.append(astrometrics)
         if fpa_digital is not None:
             snr = signal_to_noise_ratio(fpa_conv_targ, fpa_conv_star + bg_tf + dc_tf, rn_tf)
             if num_shot_noise_samples is not None:
                 snr = snr * np.sqrt(num_shot_noise_samples)
             meta_data = set_frame_annotation(meta_data, frame_num, h_fpa_os, w_fpa_os, obs_os_pix, [20 * s_osf, 20 * s_osf], snr=snr)
             if queue is not None:
                 queue.task(write_frame, {
@@ -165,15 +167,15 @@
                     'fpa_digital': fpa_digital.numpy(),
                     'meta_data': copy.deepcopy(meta_data),
                     'frame_num': frame_num,
                     'exposure_time': exposure_time,
                     'time_stamp': dt,
                     'ssp': ssp_orig,
                     'show_obs_boxes': ssp['sim']['show_obs_boxes'],
-                    'astrometrics': astrometrics.copy(),
+                    'astrometrics': astrometrics,
                     'save_pickle': ssp['sim']['save_pickle'],
                     'dtype': a2d_dtype,
                     'save_jpeg': ssp['sim']['save_jpeg'],
                 }, tag=dir_name)
             if output_debug:
                 with open(os.path.join(dir_debug, 'metadata_{}.json'.format(frame_num)), 'w') as jsonfile:
                     json.dump(meta_data, jsonfile, indent=2)
@@ -193,15 +195,15 @@
                 sleep(0.1)
             else:
                 if ssp['sim']['save_movie']:
                     logger.debug('Saving PNG movie.')
                     save_apng(dirname=os.path.join(dir_name,'AnnotatedImages'), filename='movie.png')
                 if ssp['sim']['save_czml']:
                     logger.debug('Saving CZML.')
-                    save_czml(ssp, obs_cache, os.path.join(dir_name,'satsim.czml'))
+                    save_czml(ssp, obs_cache, astrometrics_list, os.path.join(dir_name,'satsim.czml'))
                 return
 
     if queue is not None:
         queue.task(wait_and_run, {})
 
     return dir_name
 
@@ -483,23 +485,27 @@
 
             [rr0, rr1], [cc0, cc1], drr, dcc, _ = gen_track(h_fpa_pad_os, w_fpa_pad_os, y_fov_pad, x_fov_pad, observer, track, track_target, [0], t0, [t_start, t_end], star_rot, 1, track_mode, flipud=ssp['fpa']['flip_up_down'], fliplr=ssp['fpa']['flip_left_right'], az=az, el=el)
             star_tran_os = [-drr, -dcc]  # stars move in the opposite direction of target
             star_rot_rate = 0  # TODO
 
             astrometrics['ra'] = mean_degrees(star_ra0, star_ra1)
             astrometrics['dec'] = (star_dec0 + star_dec1) / 2
+            astrometrics['range'] = (dis0 + dis1) / 2
+            astrometrics['roll'] = star_rot
             astrometrics['ra_rate'] = diff_degrees(star_ra1, star_ra0) / exposure_time * 3600
             astrometrics['dec_rate'] = (star_dec1 - star_dec0) / exposure_time * 3600
             astrometrics['az'] = mean_degrees(az0, az1)
             astrometrics['el'] = (el0 + el1) / 2
-            astrometrics['time'] = t_start.utc_datetime()
+            astrometrics['time'] = time.mid(t_start, t_end).utc_datetime()
             astrometrics['x_ifov'] = x_ifov
             astrometrics['y_ifov'] = y_ifov
+            astrometrics['x_fov'] = x_fov
+            astrometrics['y_fov'] = y_fov
 
-            logger.debug('Boresight RA, Dec, Az, El: {}, {}, {}, {}.'.format(astrometrics['ra'], astrometrics['dec'], astrometrics['az'], astrometrics['el']))
+            logger.debug('Boresight RA, Dec, Roll, Az, El: {}, {}, {}, {}, {}.'.format(astrometrics['ra'], astrometrics['dec'], astrometrics['roll'], astrometrics['az'], astrometrics['el']))
 
             return star_ra0, star_dec0, star_tran_os, star_rot_rate
 
         # site
         if 'site' in ssp['geometry']:
 
             # note: stars will track horizontally where zenith is pointed up. focal plane rotation is simulated with the `rotation` variable
@@ -556,26 +562,27 @@
         if star_mode == 'bins':
             r_stars_os, c_stars_os, pe_stars_os = gen_random_points(h_fpa_pad_os, w_fpa_pad_os, y_fov_pad, x_fov_pad, star_pe, star_dn, pad_mult=star_pad)
         else:
             r_stars_os, c_stars_os, m_stars_os = [], [], []
             pe_stars_os = []
 
         # gen psf
-        if not isinstance(ssp['fpa']['psf'], dict):  # loaded from config
-            psf_os = ssp['fpa']['psf']
-            psf_os = tf.cast(psf_os, tf.float32)
-        elif ssp['fpa']['psf']['mode'] == 'gaussian':
-            eod = ssp['fpa']['psf']['eod']
-            sigma = eod_to_sigma(eod, s_osf)
-            psf_os = gen_gaussian(h_sub_pad_os, w_sub_pad_os, sigma)
-            save_cache(ssp['fpa']['psf'], psf_os)
-        elif ssp['fpa']['psf']['mode'] == 'poppy':
-            psf_os = gen_from_poppy_configuration(h_sub_pad_os / s_osf, w_sub_pad_os / s_osf, y_ifov, x_ifov, s_osf, ssp['fpa']['psf'])
-            save_cache(ssp['fpa']['psf'], psf_os)
-            psf_os = tf.cast(psf_os, tf.float32)
+        if ssp['sim']['mode'] != 'none':
+            if not isinstance(ssp['fpa']['psf'], dict):  # loaded from config
+                psf_os = ssp['fpa']['psf']
+                psf_os = tf.cast(psf_os, tf.float32)
+            elif ssp['fpa']['psf']['mode'] == 'gaussian':
+                eod = ssp['fpa']['psf']['eod']
+                sigma = eod_to_sigma(eod, s_osf)
+                psf_os = gen_gaussian(h_sub_pad_os, w_sub_pad_os, sigma)
+                save_cache(ssp['fpa']['psf'], psf_os)
+            elif ssp['fpa']['psf']['mode'] == 'poppy':
+                psf_os = gen_from_poppy_configuration(h_sub_pad_os / s_osf, w_sub_pad_os / s_osf, y_ifov, x_ifov, s_osf, ssp['fpa']['psf'])
+                save_cache(ssp['fpa']['psf'], psf_os)
+                psf_os = tf.cast(psf_os, tf.float32)
 
         if pydash.objects.has(ssp, 'augment.background.stray'):
             bg = ssp['augment']['background']['stray'](bg)
             bg = tf.cast(bg, tf.float32)
             bg = tf.where(tf.math.is_nan(bg), tf.zeros_like(bg), bg)
 
         logger.debug('Exposure time {}.'.format(exposure_time))
@@ -746,20 +753,21 @@
                 ts_end = time.utc_from_list(tt, t_end)
                 t_start_star = t_start
                 t_end_star = t_end
 
                 # if image rendering is disabled, then propagate objects and return
                 if ssp['sim']['mode'] == 'none':
                     r_obs_os, c_obs_os, pe_obs_os, obs_os_pix, obs_model = gen_objects(obs, t_start, t_end)
-                    logger.debug('Number of objects {}.'.format(len(obs_os_pix)))
-
+                    if track_mode is not None:
+                        star_ra, star_dec, star_tran_os, star_rot_rate = calculate_star_position_and_motion(ts_start, ts_end, star_rot, track_mode)
                     if with_meta:
-                        yield None, frame_num, None, None, None, None, None, None, None, None, obs_cache
+                        yield None, frame_num, astrometrics.copy(), None, None, None, None, None, None, None, obs_cache
                     else:
                         yield None
+                    continue
 
                 # refresh catalog stars
                 # TODO should save stars and transform to FPA again on every frame
                 if (star_mode == 'sstr7' or star_mode == 'csv') and (ssp['sim']['star_catalog_query_mode'] == 'frame' or frame_num == 0):
                     if track_mode is not None:
                         star_ra, star_dec, star_tran_os, star_rot_rate = calculate_star_position_and_motion(ts_start, ts_end, star_rot, track_mode)
                     if star_mode == 'sstr7':
@@ -846,10 +854,10 @@
                         pickle.dump(fpa.numpy(), picklefile)
                     with open(os.path.join(dir_debug, 'fpa_digital_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                         pickle.dump(fpa_digital.numpy(), picklefile)
                     with open(os.path.join(dir_debug, 'stars_os_{}.pickle'.format(frame_num)), 'wb') as picklefile:
                         pickle.dump([r_stars_os.numpy(), c_stars_os.numpy(), pe_stars_os.numpy(), t_start_star, t_end_star, t_osf, star_rot_rate, star_tran_os], picklefile)
 
                 if with_meta:
-                    yield fpa_digital, frame_num, astrometrics, obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, ssp['sim']['num_shot_noise_samples'], obs_cache
+                    yield fpa_digital, frame_num, astrometrics.copy(), obs_os_pix, fpa_conv_star, fpa_conv_targ, bg_tf, dc_tf, rn_tf, ssp['sim']['num_shot_noise_samples'], obs_cache
                 else:
                     yield fpa_digital
```

### Comparing `satsim-0.13.1/satsim/time/__init__.py` & `satsim-0.14.0/satsim/time/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -138,14 +138,30 @@
     frac1 = t1.tt_fraction
     return Time(
         _ts,
         np.linspace(whole0, whole1, num),
         np.linspace(frac0, frac1, num),
     )
 
+
 def delta_sec(t0, t1):
     """ Subtract t0 and t1. (t0 - t1)
 
     Returns:
         A `float` in seconds.
     """
-    return (t0 - t1) * 86400
+    return (t0 - t1) * 86400
+
+
+def mid(t0, t1):
+    """ Return the mid of two times.
+
+    Args:
+        t0: `Time`, start Skyfield `Time`
+        t1: `Time`, end Skyfield `Time`
+
+    Returns:
+        A `Time`, mid Skyfield `Time`
+    """
+    d = t1 - t0
+
+    return t0 + d * 0.5
```

### Comparing `satsim-0.13.1/satsim/util/system.py` & `satsim-0.14.0/satsim/util/system.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/util/thread.py` & `satsim-0.14.0/satsim/util/thread.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim/util/timer.py` & `satsim-0.14.0/satsim/util/timer.py`

 * *Files identical despite different names*

### Comparing `satsim-0.13.1/satsim.egg-info/PKG-INFO` & `satsim-0.14.0/satsim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.13.1
+Version: 0.14.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
 License: UNKNOWN
 Keywords: satsim
 Platform: UNKNOWN
@@ -37,14 +37,22 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.14.0
+---------------------
+
+Add vector math library.
+Add CZML output for sensor visualization.
+Fix objects not updating properly when image renderer is off.
+
+
 0.13.1
 ---------------------
 
 * Add argument to set folder name in `gen_multi`.
 * Add environment variable, `SATSIM_SKYFIELD_LOAD_DIR`, to specify location of Skyfield ephemeris files.
 * Fix incorrect CZML output when image renderer is off.
```

### Comparing `satsim-0.13.1/satsim.egg-info/SOURCES.txt` & `satsim-0.14.0/satsim.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -54,25 +54,27 @@
 docs/_build/html/api/satsim.html
 docs/_build/html/api/satsim.image.html
 docs/_build/html/api/satsim.io.html
 docs/_build/html/api/satsim.math.html
 docs/_build/html/api/satsim.pipeline.html
 docs/_build/html/api/satsim.time.html
 docs/_build/html/api/satsim.util.html
+docs/_build/html/api/satsim.vecmath.html
 docs/api/satsim.dataset.rst
 docs/api/satsim.generator.obs.rst
 docs/api/satsim.generator.rst
 docs/api/satsim.geometry.rst
 docs/api/satsim.image.rst
 docs/api/satsim.io.rst
 docs/api/satsim.math.rst
 docs/api/satsim.pipeline.rst
 docs/api/satsim.rst
 docs/api/satsim.time.rst
 docs/api/satsim.util.rst
+docs/api/satsim.vecmath.rst
 satsim/__init__.py
 satsim/cli.py
 satsim/config.py
 satsim/satsim.py
 satsim.egg-info/PKG-INFO
 satsim.egg-info/SOURCES.txt
 satsim.egg-info/dependency_links.txt
@@ -111,19 +113,28 @@
 satsim/io/__init__.py
 satsim/io/czml.py
 satsim/io/fits.py
 satsim/io/image.py
 satsim/io/satnet.py
 satsim/math/__init__.py
 satsim/math/angle.py
+satsim/math/const.py
 satsim/math/conv.py
 satsim/math/fft.py
 satsim/math/interpolate.py
 satsim/math/random.py
 satsim/math/stats.py
 satsim/pipeline/__init__.py
 satsim/time/__init__.py
 satsim/util/__init__.py
 satsim/util/system.py
 satsim/util/thread.py
 satsim/util/timer.py
+satsim/vecmath/Cartesian2.py
+satsim/vecmath/Cartesian3.py
+satsim/vecmath/Cartesian4.py
+satsim/vecmath/Matrix2.py
+satsim/vecmath/Matrix3.py
+satsim/vecmath/Matrix4.py
+satsim/vecmath/Quaternion.py
+satsim/vecmath/__init__.py
 tests/README.md
```

### Comparing `satsim-0.13.1/setup.cfg` & `satsim-0.14.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.13.1
+current_version = 0.14.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
 
@@ -12,15 +12,15 @@
 replace = __version__ = '{new_version}'
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = docs, __init__.py, satsim/experimental
-ignore = E501, E231, E222, E201, E402, E275
+ignore = E501, E231, E222, E201, E402, E275, W503, W504
 
 [aliases]
 test = pytest
 
 [tool:pytest]
 collect_ignore = ['setup.py']
```

### Comparing `satsim-0.13.1/setup.py` & `satsim-0.14.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     'poppy==1.0.3',
     'diskcache==5.0.3',
     'pydash~=4.9.0',
     'asdf==2.14.3',
     'pygc==1.3.0',
     'numba~=0.56.0',
     'pooch~=1.6.0',
-    'czmlpy~=0.8.0',
+    'czmlpy~=0.9.0',
 ]
 
 setup_requirements = ['pytest-runner', ]
 
 test_requirements = ['pytest', ]
 
 setup(
@@ -63,10 +63,10 @@
     keywords='satsim',
     name='satsim',
     packages=find_packages(include=['satsim', 'satsim.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ssc-ai/satsim',
-    version='0.13.1',
+    version='0.14.0',
     zip_safe=False,
 )
```

