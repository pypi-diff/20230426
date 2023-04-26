# Comparing `tmp/visiomode-0.5.1.tar.gz` & `tmp/visiomode-0.5.2.tar.gz`

## Comparing `visiomode-0.5.1.tar` & `visiomode-0.5.2.tar`

### file list

```diff
@@ -1,122 +1,124 @@
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 visiomode-0.5.1/.coveragerc
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 visiomode-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 visiomode-0.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 visiomode-0.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 visiomode-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visiomode-0.5.1/MANIFEST.in
--rw-r--r--   0        0        0   529374 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.icns
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 visiomode-0.5.1/pylintrc
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 visiomode-0.5.1/tox.ini
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 visiomode-0.5.1/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 visiomode-0.5.1/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 visiomode-0.5.1/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0   276154 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_1024x1024.png
--rw-r--r--   0        0        0    12448 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_128x128.png
--rw-r--r--   0        0        0    27717 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_128x128@2x.png
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_16x16.png
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_16x16@2x.png
--rw-r--r--   0        0        0    27717 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_256x256.png
--rw-r--r--   0        0        0    88924 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_256x256@2x.png
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_32x32.png
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_32x32@2x.png
--rw-r--r--   0        0        0    88924 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_512x512.png
--rw-r--r--   0        0        0   276154 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_512x512@2x.png
--rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_64x64.png
--rw-r--r--   0        0        0    12448 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_64x64@2x.png
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 visiomode-0.5.1/icon.iconset/icon_8x8@2x.png
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 visiomode-0.5.1/microcontrollers/leverpush/leverpush.ino
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 visiomode-0.5.1/microcontrollers/watercontrol/watercontrol.ino
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 visiomode-0.5.1/microcontrollers/waterservo/waterservo.ino
--rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/banner.png
--rw-r--r--   0        0        0    70254 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/logo_blackandwhite.png
--rw-r--r--   0        0        0   184766 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/sidb.jpg
--rw-r--r--   0        0        0    94408 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/visiomode_logo.png
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/visiomode_logo.svg
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/visiomode_logo_blackandwhite.svg
--rw-r--r--   0        0        0    69823 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/visiomode_logo_icon.png
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 visiomode-0.5.1/resources/visiomode_logo_icon.svg
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/__about__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/__init__.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/config.py
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/core.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/mixins.py
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/models.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/plugins.py
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/devices/__init__.py
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/devices/lever_push.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/devices/touchscreen.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/devices/water_reward.py
--rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/protocols/__init__.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/protocols/gonogo.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/protocols/tafc.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/protocols/target_only.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/res/__init__.py
--rw-r--r--   0        0        0    84551 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/res/icon.png
--rw-r--r--   0        0        0    70254 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/res/loading.png
--rw-r--r--   0        0        0   141955 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/res/target.jpg
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/__init__.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/grating.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/isoluminant_gray.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/moving_grating.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/solid_colour.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/variable_contrast_grating.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/stimuli/variable_contrast_moving_grating.py
--rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/__init__.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/api.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/export.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/favicon.ico
--rw-r--r--   0        0        0   164761 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0    78643 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/css/styles.min.css
--rw-r--r--   0        0        0   125320 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.eot
--rw-r--r--   0        0        0   662941 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.svg
--rw-r--r--   0        0        0   125016 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    84568 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.woff
--rw-r--r--   0        0        0    72148 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34388 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.eot
--rw-r--r--   0        0        0   145174 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.svg
--rw-r--r--   0        0        0    34092 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13608 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   186512 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.eot
--rw-r--r--   0        0        0   819802 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.svg
--rw-r--r--   0        0        0   186228 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    96248 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.woff
--rw-r--r--   0        0        0    74320 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    54242 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fontawesome-all.min.css
--rw-r--r--   0        0        0    69823 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/visiomode_logo_icon.png
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar1.jpeg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar2.jpeg
--rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar3.jpeg
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar4.jpeg
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar5.jpeg
--rw-r--r--   0        0        0   203483 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/js/chart.min.js
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/js/history.js
--rw-r--r--   0        0        0    88147 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/js/jquery.min.js
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/js/script.min.js
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/static/js/session.js
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/404.html
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/about.html
--rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/base.html
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/help.html
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/history.html
--rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/index.html
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/settings.html
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/README.md
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/gonogo.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/protocol.html
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/tafc.html
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/target_only.html
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/task.html
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/README.md
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/grating.html
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/moving_grating.html
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/solid_colour.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/stimulus.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 visiomode-0.5.1/tests/test_launch.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 visiomode-0.5.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 visiomode-0.5.1/LICENSE
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 visiomode-0.5.1/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 visiomode-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 visiomode-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 visiomode-0.5.2/.coveragerc
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 visiomode-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 visiomode-0.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 visiomode-0.5.2/CITATION.cff
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 visiomode-0.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 visiomode-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 visiomode-0.5.2/MANIFEST.in
+-rw-r--r--   0        0        0   529374 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.icns
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 visiomode-0.5.2/pylintrc
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 visiomode-0.5.2/tox.ini
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 visiomode-0.5.2/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 visiomode-0.5.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 visiomode-0.5.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0   276154 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_1024x1024.png
+-rw-r--r--   0        0        0    12448 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_128x128.png
+-rw-r--r--   0        0        0    27717 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_128x128@2x.png
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_16x16.png
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_16x16@2x.png
+-rw-r--r--   0        0        0    27717 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_256x256.png
+-rw-r--r--   0        0        0    88924 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_256x256@2x.png
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_32x32.png
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_32x32@2x.png
+-rw-r--r--   0        0        0    88924 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_512x512.png
+-rw-r--r--   0        0        0   276154 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_512x512@2x.png
+-rw-r--r--   0        0        0     6327 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_64x64.png
+-rw-r--r--   0        0        0    12448 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_64x64@2x.png
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 visiomode-0.5.2/icon.iconset/icon_8x8@2x.png
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 visiomode-0.5.2/microcontrollers/leverpush/leverpush.ino
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 visiomode-0.5.2/microcontrollers/watercontrol/watercontrol.ino
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 visiomode-0.5.2/microcontrollers/waterservo/waterservo.ino
+-rw-r--r--   0        0        0    26199 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/banner.png
+-rw-r--r--   0        0        0    70254 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/logo_blackandwhite.png
+-rw-r--r--   0        0        0   184766 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/sidb.jpg
+-rw-r--r--   0        0        0    94408 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/visiomode_logo.png
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/visiomode_logo.svg
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/visiomode_logo_blackandwhite.svg
+-rw-r--r--   0        0        0    69823 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/visiomode_logo_icon.png
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 visiomode-0.5.2/resources/visiomode_logo_icon.svg
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/__about__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/config.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/core.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/mixins.py
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/models.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/plugins.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/devices/__init__.py
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/devices/lever_push.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/devices/touchscreen.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/devices/water_reward.py
+-rw-r--r--   0        0        0    10250 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/protocols/__init__.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/protocols/gonogo.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/protocols/tafc.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/protocols/target_only.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/res/__init__.py
+-rw-r--r--   0        0        0    84551 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/res/icon.png
+-rw-r--r--   0        0        0    70254 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/res/loading.png
+-rw-r--r--   0        0        0   141955 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/res/target.jpg
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/__init__.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/grating.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/isoluminant_gray.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/moving_grating.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/solid_colour.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/variable_contrast_grating.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/stimuli/variable_contrast_moving_grating.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/__init__.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/api.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/export.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/favicon.ico
+-rw-r--r--   0        0        0   164761 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0    78643 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/css/styles.min.css
+-rw-r--r--   0        0        0   125320 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   662941 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   125016 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    84568 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    72148 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34388 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   145174 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    34092 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16812 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13608 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   186512 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   819802 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   186228 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    96248 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    74320 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    54242 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fontawesome-all.min.css
+-rw-r--r--   0        0        0    69823 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/visiomode_logo_icon.png
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar1.jpeg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar2.jpeg
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar3.jpeg
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar4.jpeg
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar5.jpeg
+-rw-r--r--   0        0        0   203484 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/chart.min.js
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/history.js
+-rw-r--r--   0        0        0    88147 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/jquery.min.js
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/script.min.js
+-rw-r--r--   0        0        0     8165 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/session.js
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/static/js/settings.js
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/404.html
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/about.html
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/base.html
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/help.html
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/history.html
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/index.html
+-rw-r--r--   0        0        0    11043 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/settings.html
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/README.md
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/gonogo.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/protocol.html
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/tafc.html
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/target_only.html
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/task.html
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/README.md
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/grating.html
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/moving_grating.html
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/solid_colour.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/stimulus.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 visiomode-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 visiomode-0.5.2/tests/test_launch.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 visiomode-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 visiomode-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 visiomode-0.5.2/README.md
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 visiomode-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 visiomode-0.5.2/PKG-INFO
```

### Comparing `visiomode-0.5.1/CHANGELOG.md` & `visiomode-0.5.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,37 @@
 
 Versions follow [Semantic Versioning](https://semver.org) (`<major>.<minor>.<patch>`).
 
 ## [Unreleased]
 
 ### Added
 
+- Cache directory for intermittent export files.
+- Session data export in NWB and CSV format.
+- CITATION.cff file.
+
+### Changed
+
+- App configuration is now stored in a JSON relative to where the app was launched.
+- Help sidebar option redirects to documentation at readthedocs.
+
+### Fixed
+
+- Fix loading external configuration files ([#118](https://github.com/DuguidLab/visiomode/issues/118)).
+
+## [0.5.1] - 2023-03-02
+
+### Fixed
+
+- Target-only paradigm crash.
+
+## [0.5.0] - 2023-02-24
+
+### Added
+
 - Trial outcome counter chart in session "Overview" panel.
 - Favicon for web interface.
 - Version details in session file.
 - Signal detection theory classification per trial.
 - Added response identifier to Response object.
 - Stimulus info now returns common name and identifier.
 
@@ -84,15 +107,14 @@
 
 ## [0.3.3] - 2022-03-22
 
 ### Changed
 
 - Use pygame version 2.0.1.
 
-
 ## [0.3.2] - 2022-03-22
 
 ### Changed
 
 - Various build system improvements.
 
 ## [0.3.1] - 2022-03-22
@@ -174,15 +196,17 @@
 - CLI-based task monitoring.
 - Grating and isoluminant gray stimuli.
 - Single-target and 2AFC paradigms.
 - Initial JSON file format for storing session data.
 - Redis-based syncing between behaviour & web interface components.
 - SocketIO reads Redis updates for web interface.
 
-[unreleased]: https://github.com/DuguidLab/visiomode/compare/v0.4.1...HEAD
+[unreleased]: https://github.com/DuguidLab/visiomode/compare/v0.5.1...HEAD
+[0.5.1]: https://github.com/DuguidLab/visiomode/compare/v0.5.0...v0.5.1
+[0.5.0]: https://github.com/DuguidLab/visiomode/compare/v0.4.1...v0.5.0
 [0.4.1]: https://github.com/DuguidLab/visiomode/compare/v0.4.0...v0.4.1
 [0.4.0]: https://github.com/DuguidLab/visiomode/compare/v0.3.5...v0.4.0
 [0.3.5]: https://github.com/DuguidLab/visiomode/compare/v0.3.4...v0.3.5
 [0.3.4]: https://github.com/DuguidLab/visiomode/compare/v0.3.3...v0.3.4
 [0.3.3]: https://github.com/DuguidLab/visiomode/compare/v0.3.2...v0.3.3
 [0.3.2]: https://github.com/DuguidLab/visiomode/compare/v0.3.1...v0.3.2
 [0.3.1]: https://github.com/DuguidLab/visiomode/compare/v0.3.0...v0.3.1
```

### Comparing `visiomode-0.5.1/CODE_OF_CONDUCT.md` & `visiomode-0.5.2/CODE_OF_CONDUCT.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-
-# Contributor Covenant Code of Conduct
-
-## Our Pledge
-
-We as members, contributors, and leaders pledge to make participation in our
-community a harassment-free experience for everyone, regardless of age, body
-size, visible or invisible disability, ethnicity, sex characteristics, gender
-identity and expression, level of experience, education, socio-economic status,
-nationality, personal appearance, race, caste, color, religion, or sexual
-identity and orientation.
-
-We pledge to act and interact in ways that contribute to an open, welcoming,
-diverse, inclusive, and healthy community.
-
-## Our Standards
-
-Examples of behaviour that contributes to a positive environment for our
-community include:
-
-* Demonstrating empathy and kindness toward other people
-* Being respectful of differing opinions, viewpoints, and experiences
-* Giving and gracefully accepting constructive feedback
-* Accepting responsibility and apologizing to those affected by our mistakes,
-  and learning from the experience
-* Focusing on what is best not just for us as individuals, but for the overall
-  community
-
-Examples of unacceptable behaviour include:
-
-* The use of sexualized language or imagery, and sexual attention or advances of
-  any kind
-* Trolling, insulting or derogatory comments, and personal or political attacks
-* Public or private harassment
-* Publishing others' private information, such as a physical or email address,
-  without their explicit permission
-* Other conduct which could reasonably be considered inappropriate in a
-  professional setting
-
-## Enforcement Responsibilities
-
-Community leaders are responsible for clarifying and enforcing our standards of
-acceptable behaviour and will take appropriate and fair corrective action in
-response to any behaviour that they deem inappropriate, threatening, offensive,
-or harmful.
-
-Community leaders have the right and responsibility to remove, edit, or reject
-comments, commits, code, wiki edits, issues, and other contributions that are
-not aligned to this Code of Conduct, and will communicate reasons for moderation
-decisions when appropriate.
-
-## Scope
-
-This Code of Conduct applies within all community spaces, and also applies when
-an individual is officially representing the community in public spaces.
-Examples of representing our community include using an official e-mail address,
-posting via an official social media account, or acting as an appointed
-representative at an online or offline event.
-
-## Enforcement
-
-Instances of abusive, harassing, or otherwise unacceptable behaviour may be
-reported to the community leaders responsible for enforcement at
-`Constantinos.Eleftheriou at ed.ac.uk`.
-All complaints will be reviewed and investigated promptly and fairly.
-
-All community leaders are obligated to respect the privacy and security of the
-reporter of any incident.
-
-## Enforcement Guidelines
-
-Community leaders will follow these Community Impact Guidelines in determining
-the consequences for any action they deem in violation of this Code of Conduct:
-
-### 1. Correction
-
-**Community Impact**: Use of inappropriate language or other behaviour deemed
-unprofessional or unwelcome in the community.
-
-**Consequence**: A private, written warning from community leaders, providing
-clarity around the nature of the violation and an explanation of why the
-behaviour was inappropriate. A public apology may be requested.
-
-### 2. Warning
-
-**Community Impact**: A violation through a single incident or series of
-actions.
-
-**Consequence**: A warning with consequences for continued behaviour. No
-interaction with the people involved, including unsolicited interaction with
-those enforcing the Code of Conduct, for a specified period of time. This
-includes avoiding interactions in community spaces as well as external channels
-like social media. Violating these terms may lead to a temporary or permanent
-ban.
-
-### 3. Temporary Ban
-
-**Community Impact**: A serious violation of community standards, including
-sustained inappropriate behaviour.
-
-**Consequence**: A temporary ban from any sort of interaction or public
-communication with the community for a specified period of time. No public or
-private interaction with the people involved, including unsolicited interaction
-with those enforcing the Code of Conduct, is allowed during this period.
-Violating these terms may lead to a permanent ban.
-
-### 4. Permanent Ban
-
-**Community Impact**: Demonstrating a pattern of violation of community
-standards, including sustained inappropriate behaviour, harassment of an
-individual, or aggression toward or disparagement of classes of individuals.
-
-**Consequence**: A permanent ban from any sort of public interaction within the
-community.
-
-## Attribution
-
-This Code of Conduct is adapted from the [Contributor Covenant][homepage],
-version 2.1, available at
-[https://www.contributor-covenant.org/version/2/1/code_of_conduct.html][v2.1].
-
-Community Impact Guidelines were inspired by
-[Mozilla's code of conduct enforcement ladder][Mozilla CoC].
-
-For answers to common questions about this code of conduct, see the FAQ at
-[https://www.contributor-covenant.org/faq][FAQ]. Translations are available at
-[https://www.contributor-covenant.org/translations][translations].
-
-[homepage]: https://www.contributor-covenant.org
-[v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
-[Mozilla CoC]: https://github.com/mozilla/diversity
-[FAQ]: https://www.contributor-covenant.org/faq
-[translations]: https://www.contributor-covenant.org/translations
+
+# Contributor Covenant Code of Conduct
+
+## Our Pledge
+
+We as members, contributors, and leaders pledge to make participation in our
+community a harassment-free experience for everyone, regardless of age, body
+size, visible or invisible disability, ethnicity, sex characteristics, gender
+identity and expression, level of experience, education, socio-economic status,
+nationality, personal appearance, race, caste, color, religion, or sexual
+identity and orientation.
+
+We pledge to act and interact in ways that contribute to an open, welcoming,
+diverse, inclusive, and healthy community.
+
+## Our Standards
+
+Examples of behaviour that contributes to a positive environment for our
+community include:
+
+* Demonstrating empathy and kindness toward other people
+* Being respectful of differing opinions, viewpoints, and experiences
+* Giving and gracefully accepting constructive feedback
+* Accepting responsibility and apologizing to those affected by our mistakes,
+  and learning from the experience
+* Focusing on what is best not just for us as individuals, but for the overall
+  community
+
+Examples of unacceptable behaviour include:
+
+* The use of sexualized language or imagery, and sexual attention or advances of
+  any kind
+* Trolling, insulting or derogatory comments, and personal or political attacks
+* Public or private harassment
+* Publishing others' private information, such as a physical or email address,
+  without their explicit permission
+* Other conduct which could reasonably be considered inappropriate in a
+  professional setting
+
+## Enforcement Responsibilities
+
+Community leaders are responsible for clarifying and enforcing our standards of
+acceptable behaviour and will take appropriate and fair corrective action in
+response to any behaviour that they deem inappropriate, threatening, offensive,
+or harmful.
+
+Community leaders have the right and responsibility to remove, edit, or reject
+comments, commits, code, wiki edits, issues, and other contributions that are
+not aligned to this Code of Conduct, and will communicate reasons for moderation
+decisions when appropriate.
+
+## Scope
+
+This Code of Conduct applies within all community spaces, and also applies when
+an individual is officially representing the community in public spaces.
+Examples of representing our community include using an official e-mail address,
+posting via an official social media account, or acting as an appointed
+representative at an online or offline event.
+
+## Enforcement
+
+Instances of abusive, harassing, or otherwise unacceptable behaviour may be
+reported to the community leaders responsible for enforcement at
+`Constantinos.Eleftheriou at ed.ac.uk`.
+All complaints will be reviewed and investigated promptly and fairly.
+
+All community leaders are obligated to respect the privacy and security of the
+reporter of any incident.
+
+## Enforcement Guidelines
+
+Community leaders will follow these Community Impact Guidelines in determining
+the consequences for any action they deem in violation of this Code of Conduct:
+
+### 1. Correction
+
+**Community Impact**: Use of inappropriate language or other behaviour deemed
+unprofessional or unwelcome in the community.
+
+**Consequence**: A private, written warning from community leaders, providing
+clarity around the nature of the violation and an explanation of why the
+behaviour was inappropriate. A public apology may be requested.
+
+### 2. Warning
+
+**Community Impact**: A violation through a single incident or series of
+actions.
+
+**Consequence**: A warning with consequences for continued behaviour. No
+interaction with the people involved, including unsolicited interaction with
+those enforcing the Code of Conduct, for a specified period of time. This
+includes avoiding interactions in community spaces as well as external channels
+like social media. Violating these terms may lead to a temporary or permanent
+ban.
+
+### 3. Temporary Ban
+
+**Community Impact**: A serious violation of community standards, including
+sustained inappropriate behaviour.
+
+**Consequence**: A temporary ban from any sort of interaction or public
+communication with the community for a specified period of time. No public or
+private interaction with the people involved, including unsolicited interaction
+with those enforcing the Code of Conduct, is allowed during this period.
+Violating these terms may lead to a permanent ban.
+
+### 4. Permanent Ban
+
+**Community Impact**: Demonstrating a pattern of violation of community
+standards, including sustained inappropriate behaviour, harassment of an
+individual, or aggression toward or disparagement of classes of individuals.
+
+**Consequence**: A permanent ban from any sort of public interaction within the
+community.
+
+## Attribution
+
+This Code of Conduct is adapted from the [Contributor Covenant][homepage],
+version 2.1, available at
+[https://www.contributor-covenant.org/version/2/1/code_of_conduct.html][v2.1].
+
+Community Impact Guidelines were inspired by
+[Mozilla's code of conduct enforcement ladder][Mozilla CoC].
+
+For answers to common questions about this code of conduct, see the FAQ at
+[https://www.contributor-covenant.org/faq][FAQ]. Translations are available at
+[https://www.contributor-covenant.org/translations][translations].
+
+[homepage]: https://www.contributor-covenant.org
+[v2.1]: https://www.contributor-covenant.org/version/2/1/code_of_conduct.html
+[Mozilla CoC]: https://github.com/mozilla/diversity
+[FAQ]: https://www.contributor-covenant.org/faq
+[translations]: https://www.contributor-covenant.org/translations
```

### Comparing `visiomode-0.5.1/CONTRIBUTING.md` & `visiomode-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.icns` & `visiomode-0.5.2/icon.icns`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/pylintrc` & `visiomode-0.5.2/pylintrc`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/tox.ini` & `visiomode-0.5.2/tox.ini`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_1024x1024.png` & `visiomode-0.5.2/icon.iconset/icon_1024x1024.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_128x128.png` & `visiomode-0.5.2/icon.iconset/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_128x128@2x.png` & `visiomode-0.5.2/icon.iconset/icon_128x128@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_16x16.png` & `visiomode-0.5.2/icon.iconset/icon_16x16.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_16x16@2x.png` & `visiomode-0.5.2/icon.iconset/icon_16x16@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_256x256.png` & `visiomode-0.5.2/icon.iconset/icon_256x256.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_256x256@2x.png` & `visiomode-0.5.2/icon.iconset/icon_256x256@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_32x32.png` & `visiomode-0.5.2/icon.iconset/icon_32x32.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_32x32@2x.png` & `visiomode-0.5.2/icon.iconset/icon_32x32@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_512x512.png` & `visiomode-0.5.2/icon.iconset/icon_512x512.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_512x512@2x.png` & `visiomode-0.5.2/icon.iconset/icon_512x512@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_64x64.png` & `visiomode-0.5.2/icon.iconset/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_64x64@2x.png` & `visiomode-0.5.2/icon.iconset/icon_64x64@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/icon.iconset/icon_8x8@2x.png` & `visiomode-0.5.2/icon.iconset/icon_8x8@2x.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/microcontrollers/leverpush/leverpush.ino` & `visiomode-0.5.2/microcontrollers/leverpush/leverpush.ino`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/microcontrollers/watercontrol/watercontrol.ino` & `visiomode-0.5.2/microcontrollers/watercontrol/watercontrol.ino`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/banner.png` & `visiomode-0.5.2/resources/banner.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/logo_blackandwhite.png` & `visiomode-0.5.2/resources/logo_blackandwhite.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/sidb.jpg` & `visiomode-0.5.2/resources/sidb.jpg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/visiomode_logo.png` & `visiomode-0.5.2/resources/visiomode_logo.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/visiomode_logo.svg` & `visiomode-0.5.2/resources/visiomode_logo.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/visiomode_logo_blackandwhite.svg` & `visiomode-0.5.2/resources/visiomode_logo_blackandwhite.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/visiomode_logo_icon.png` & `visiomode-0.5.2/resources/visiomode_logo_icon.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/resources/visiomode_logo_icon.svg` & `visiomode-0.5.2/resources/visiomode_logo_icon.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/core.py` & `visiomode-0.5.2/src/visiomode/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 import visiomode.models as models
 import visiomode.webpanel as webpanel
 import visiomode.protocols as protocols
 
 # Register mouse events as touch events - useful for debugging.
 os.environ["SDL_MOUSE_TOUCH_EVENTS"] = "1"
 
-logging.basicConfig(level=logging.DEBUG)
-
 
 class Visiomode:
     def __init__(self):
         self.clock = pg.time.Clock()
         self.config = conf.Config()
 
         self.action_q = queue.Queue()  # Queue for action messages
```

### Comparing `visiomode-0.5.1/src/visiomode/mixins.py` & `visiomode-0.5.2/src/visiomode/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,87 @@
-"""Useful Mixins for class code reuse"""
+"""App configuration loader"""
+
 #  This file is part of visiomode.
 #  Copyright (c) 2020 Constantinos Eleftheriou <Constantinos.Eleftheriou@ed.ac.uk>
 #  Distributed under the terms of the MIT Licence.
+
 import os
-import re
-import yaml
+import json
 import logging
 
+logging.basicConfig(level=logging.INFO)
 
-class BaseClassMixin:
-    """Provides convenience methods for identifying and tracking the progeny of Base classes."""
-
-    @classmethod
-    def get_children(cls):
-        """Return all inheriting children as a list."""
-        for child in cls.__subclasses__():
-            yield from child.get_children()
-            yield child
-
-    @classmethod
-    def get_child(cls, child_id):
-        children = cls.get_children()
-        for child in children:
-            if child.get_identifier() == child_id:
-                return child
-
-    @classmethod
-    def get_identifier(cls):
-        """Generate lowercase identifier for the class."""
-        return cls.__name__.lower()
 
-    @classmethod
-    def get_common_name(cls):
-        """ "Return the human-readable, space-separated name for the class."""
-        return re.sub(r"((?<=[a-z])[A-Z]|(?<!\A)[A-Z](?=[a-z]))", r" \1", cls.__name__)
+CONFIG_PATH = ".visiomode.json"
 
+DEFAULT_CONFIG = {
+    "debug": True,
+    "flask_key": "dev",
+    "data_dir": "visiomode_data",
+    "cache_dir": "visiomode_data/cache",
+    "fps": 60,
+    "width": 400,
+    "height": 800,
+    "fullscreen": False,
+    "devices": "devices/",
+}
+
+
+class Config:
+    """App configuration loader."""
+
+    debug: bool
+    flask_key: str
+    data_dir: str
+    cache_dir: str
+    fps: int
+    width: int
+    height: int
+    fullscreen: bool
+    devices: str
 
-class WebFormMixin:
-    """Webform UI for class parameters."""
+    def __init__(self):
+        """Initialises Config with a path to a configuration file.
 
-    form_path: str
-
-    @classmethod
-    def get_form(cls):
-        return cls.form_path
-
-
-class YamlAttributesMixin:
-    """Load and save class attributes as YAML files."""
-
-    def load_yaml(self, path):
-        """Loads YAML file parameters as class attributes.
+        If a valid configuration file exists, the program assumes it is NOT in debug mode, unless the config file
+        specifies otherwise.
 
         Args:
-            path: Path to config YAML.
+            path: Path to config YAML, defaults to DEFAULT_PATH. Only used if it exists.
         """
-        if not path or not os.path.exists(path):
-            return
-        with open(path) as f:
-            attrs = yaml.safe_load(f)
-            for key, value in attrs.items():
-                if key not in self.__dict__.keys():
-                    logging.info(
-                        "{} is not a valid config parameter, skipping...".format(key)
-                    )
-                    continue
-                setattr(self, key, value)
+        if os.path.exists(CONFIG_PATH):
+            logging.info(f"Loading config from {CONFIG_PATH}")
+            self._load_config(CONFIG_PATH)
+        else:
+            logging.warning("No config file found, using defaults")
+            self._set_defaults()
+            self.save()
+
+        os.makedirs(self.data_dir, exist_ok=True)
+        os.makedirs(self.cache_dir, exist_ok=True)
+
+    def save(self, path=CONFIG_PATH):
+        with open(path, "w") as f:
+            json.dump(self.__dict__, f, indent=4)
 
-    def save_yaml(self, path, exclude=None):
-        """Save class attributes as a YAML file."""
-        pass
+    def to_dict(self):
+        return self.__dict__
 
+    def _load_config(self, path):
+        """Loads config from a JSON file.
 
-class ProtocolEventsMixin:
-    """Interface declarations for methods handling protocol events."""
-
-    def on_protocol_start(self):
-        pass
-
-    def on_trial_start(self):
-        pass
-
-    def on_stimulus_start(self):
-        pass
-
-    def on_trial_end(self):
-        pass
-
-    def on_protocol_end(self):
-        pass
-
-    def on_correct(self):
-        pass
-
-    def on_incorrect(self):
-        pass
+        Args:
+            path: Path to config JSON file.
+        """
+        with open(path, "r") as f:
+            config = json.load(f)
 
-    def on_no_response(self):
-        pass
+        for key, value in config.items():
+            if key in DEFAULT_CONFIG:
+                setattr(self, key, value)
+            else:
+                logging.warning("Unknown config key: {}".format(key))
 
-    def on_precued(self):
-        pass
+    def _set_defaults(self):
+        """Sets config to default values."""
+        for key, value in DEFAULT_CONFIG.items():
+            setattr(self, key, value)
```

### Comparing `visiomode-0.5.1/src/visiomode/models.py` & `visiomode-0.5.2/src/visiomode/models.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/plugins.py` & `visiomode-0.5.2/src/visiomode/plugins.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/devices/__init__.py` & `visiomode-0.5.2/src/visiomode/devices/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,23 +35,20 @@
 
     try:
         InputDevice.get_child(profile_id)(address).test()
     except TypeError:
         logging.error("Not an input device!")
 
 
-class Device(
-    mixins.BaseClassMixin, mixins.YamlAttributesMixin, mixins.ProtocolEventsMixin
-):
+class Device(mixins.BaseClassMixin, mixins.ProtocolEventsMixin):
     def __init__(self, address=None, profile_path=None):
         self.profile_path = profile_path or (
             conf.Config().devices + os.sep + self.get_identifier() + ".yml"
         )
         self.address = address
-        self.load_yaml(self.profile_path)
 
     def test(self):
         raise NotImplementedError
 
     def __repr__(self):
         return "<{} device at {}>".format(self.get_common_name(), self.address)
```

### Comparing `visiomode-0.5.1/src/visiomode/devices/lever_push.py` & `visiomode-0.5.2/src/visiomode/devices/lever_push.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/devices/touchscreen.py` & `visiomode-0.5.2/src/visiomode/devices/touchscreen.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/devices/water_reward.py` & `visiomode-0.5.2/src/visiomode/devices/water_reward.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/protocols/__init__.py` & `visiomode-0.5.2/src/visiomode/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/protocols/gonogo.py` & `visiomode-0.5.2/src/visiomode/protocols/gonogo.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/protocols/tafc.py` & `visiomode-0.5.2/src/visiomode/protocols/tafc.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/protocols/target_only.py` & `visiomode-0.5.2/src/visiomode/protocols/target_only.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/res/icon.png` & `visiomode-0.5.2/src/visiomode/res/icon.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/res/loading.png` & `visiomode-0.5.2/src/visiomode/res/loading.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/res/target.jpg` & `visiomode-0.5.2/src/visiomode/res/target.jpg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/__init__.py` & `visiomode-0.5.2/src/visiomode/stimuli/__init__.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/grating.py` & `visiomode-0.5.2/src/visiomode/stimuli/grating.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/moving_grating.py` & `visiomode-0.5.2/src/visiomode/stimuli/moving_grating.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/solid_colour.py` & `visiomode-0.5.2/src/visiomode/stimuli/solid_colour.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/variable_contrast_grating.py` & `visiomode-0.5.2/src/visiomode/stimuli/variable_contrast_grating.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/stimuli/variable_contrast_moving_grating.py` & `visiomode-0.5.2/src/visiomode/stimuli/variable_contrast_moving_grating.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/__init__.py` & `visiomode-0.5.2/src/visiomode/webpanel/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,14 +105,20 @@
 
     app.add_url_rule(
         "/api/download/<filetype>/<filename>",
         view_func=api.DownloadAPI.as_view("download_api"),
         methods=["GET"],
     )
 
+    app.add_url_rule(
+        "/api/settings",
+        view_func=api.SettingsAPI.as_view("settings_api"),
+        methods=["GET", "POST"],
+    )
+
     return app
 
 
 def runserver(action_q, log_q, threaded=False):
     """Runs the flask app in an integrated server."""
     app = create_app(action_q, log_q)
     if threaded:
```

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/api.py` & `visiomode-0.5.2/src/visiomode/webpanel/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import glob
 import flask
 import flask.views
 import visiomode.config as cfg
 import visiomode.devices as devices
 import visiomode.protocols as protocols
 import visiomode.stimuli as stimuli
+import visiomode.webpanel.export as export
 
 
 class DeviceAPI(flask.views.MethodView):
     def post(self):
         request = json.loads(flask.request.data.decode("utf8"))
         devices.check_device_profile(request["profile"], request["address"])
         return "OK"
@@ -71,16 +72,15 @@
         return socket.gethostname()
 
 
 class HistoryAPI(flask.views.MethodView):
     """Session history API."""
 
     def get(self):
-        """Get stored session data.
-        """
+        """Get stored session data."""
         config = cfg.Config()
         session_files = glob.glob(config.data_dir + os.sep + "*.json")
         sessions = []
         for session_file in session_files:
             with open(session_file) as f:
                 try:
                     session = json.load(f)
@@ -100,11 +100,41 @@
 
 class DownloadAPI(flask.views.MethodView):
     """Download session data in whatever format the user wants."""
 
     def get(self, filetype, filename):
         config = cfg.Config()
         sessions_dir = os.path.abspath(config.data_dir)
+        cache_dir = os.path.abspath(config.cache_dir)
         if filetype == "json":
             return flask.send_from_directory(sessions_dir, filename, as_attachment=True)
+        elif filetype == "nwb":
+            nwb_fname = export.to_nwb(sessions_dir + os.sep + filename)
+            return flask.send_from_directory(cache_dir, nwb_fname, as_attachment=True)
+        elif filetype == "csv":
+            csv_fname = export.to_csv(sessions_dir + os.sep + filename)
+            return flask.send_from_directory(cache_dir, csv_fname, as_attachment=True)
         else:
             return "File format {} is not supported (yet)".format(filetype)
+
+
+class SettingsAPI(flask.views.MethodView):
+    """API for saving and loading settings."""
+
+    def get(self):
+        """Get settings."""
+        config = cfg.Config()
+        return config.to_dict()
+
+    def post(self):
+        """Save settings."""
+        request = flask.request.json
+        config = cfg.Config()
+        print(request)
+        config.width = request.get("width", config.width)
+        config.height = request.get("height", config.height)
+        config.fps = request.get("fps", config.fps)
+        config.fullscreen = request.get("fullscreen", config.fullscreen)
+        config.data_dir = request.get("data_dir", config.data_dir)
+        config.save()
+        return "OK"
+
```

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/favicon.ico` & `visiomode-0.5.2/src/visiomode/webpanel/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/bootstrap/css/bootstrap.min.css` & `visiomode-0.5.2/src/visiomode/webpanel/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/bootstrap/js/bootstrap.min.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/css/styles.min.css` & `visiomode-0.5.2/src/visiomode/webpanel/static/css/styles.min.css`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.eot` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.svg` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.ttf` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.woff` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-brands-400.woff2` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.eot` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.svg` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.ttf` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.woff` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-regular-400.woff2` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.eot` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.svg` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.ttf` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.woff` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fa-solid-900.woff2` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/fonts/fontawesome-all.min.css` & `visiomode-0.5.2/src/visiomode/webpanel/static/fonts/fontawesome-all.min.css`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/visiomode_logo_icon.png` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/visiomode_logo_icon.png`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar1.jpeg` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar1.jpeg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar2.jpeg` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar2.jpeg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar3.jpeg` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar3.jpeg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar4.jpeg` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar4.jpeg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/img/avatars/avatar5.jpeg` & `visiomode-0.5.2/src/visiomode/webpanel/static/img/avatars/avatar5.jpeg`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/js/chart.min.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/js/chart.min.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with very long lines (57044), with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -12711,8 +12711,8 @@
 00031a60: 2877 6e2c 566e 2c7a 6f2c 6f6f 2c74 2c4d  (wn,Vn,zo,oo,t,M
 00031a70: 7329 2c77 6e2e 4368 6172 743d 776e 2c22  s),wn.Chart=wn,"
 00031a80: 756e 6465 6669 6e65 6422 213d 7479 7065  undefined"!=type
 00031a90: 6f66 2077 696e 646f 7726 2628 7769 6e64  of window&&(wind
 00031aa0: 6f77 2e43 6861 7274 3d77 6e29 2c77 6e7d  ow.Chart=wn),wn}
 00031ab0: 2929 3b0d 0a2f 2f23 2073 6f75 7263 654d  ));..//# sourceM
 00031ac0: 6170 7069 6e67 5552 4c3d 6368 6172 742e  appingURL=chart.
-00031ad0: 756d 642e 6a73 2e6d 6170 0a              umd.js.map.
+00031ad0: 756d 642e 6a73 2e6d 6170 0d0a            umd.js.map..
```

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/js/history.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/js/history.js`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/js/jquery.min.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/js/script.min.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/js/script.min.js`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/static/js/session.js` & `visiomode-0.5.2/src/visiomode/webpanel/static/js/session.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text, with CRLF line terminators*

 * *Files 0% similar despite different names*

```diff
@@ -51,460 +51,461 @@
 00000320: 7373 696f 6e0d 0a20 2020 2020 2020 206c  ssion..        l
 00000330: 6574 2066 6965 6c64 7320 3d20 5b2e 2e2e  et fields = [...
 00000340: 666f 726d 2e67 6574 456c 656d 656e 7473  form.getElements
 00000350: 4279 436c 6173 734e 616d 6528 2766 6f72  ByClassName('for
 00000360: 6d2d 636f 6e74 726f 6c27 295d 3b0d 0a20  m-control')];.. 
 00000370: 2020 2020 2020 206c 6574 2072 6571 7565         let reque
 00000380: 7374 203d 2066 6965 6c64 732e 7265 6475  st = fields.redu
-00000390: 6365 2828 5f2c 2078 2920 3d3e 2028 7b2e  ce((_, x) => ({.
-000003a0: 2e2e 5f2c 205b 782e 6964 5d3a 2078 2e76  .._, [x.id]: x.v
-000003b0: 616c 7565 7d29 2c20 7b7d 293b 0d0a 2020  alue}), {});..  
-000003c0: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
-000003d0: 6728 4a53 4f4e 2e73 7472 696e 6769 6679  g(JSON.stringify
-000003e0: 2872 6571 7565 7374 2929 0d0a 0d0a 2020  (request))....  
-000003f0: 2020 2020 2020 242e 616a 6178 287b 0d0a        $.ajax({..
-00000400: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00000410: 3a20 2750 4f53 5427 2c0d 0a20 2020 2020  : 'POST',..     
-00000420: 2020 2020 2020 2075 726c 3a20 222f 6170         url: "/ap
-00000430: 692f 7365 7373 696f 6e22 2c0d 0a20 2020  i/session",..   
-00000440: 2020 2020 2020 2020 2064 6174 613a 204a           data: J
-00000450: 534f 4e2e 7374 7269 6e67 6966 7928 7b0d  SON.stringify({.
-00000460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000470: 2074 7970 653a 2022 7374 6172 7422 2c0d   type: "start",.
-00000480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000490: 2064 6174 613a 2072 6571 7565 7374 2c0d   data: request,.
-000004a0: 0a20 2020 2020 2020 2020 2020 207d 292c  .            }),
-000004b0: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-000004c0: 7461 5479 7065 3a20 226a 736f 6e22 2c0d  taType: "json",.
-000004d0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000004e0: 7465 6e74 5479 7065 3a20 2261 7070 6c69  tentType: "appli
-000004f0: 6361 7469 6f6e 2f6a 736f 6e22 0d0a 2020  cation/json"..  
-00000500: 2020 2020 2020 7d29 3b0d 0a0d 0a20 2020        });....   
-00000510: 2020 2020 2063 6f6e 736f 6c65 2e6c 6f67       console.log
-00000520: 2827 7365 7373 696f 6e20 7374 6172 7420  ('session start 
-00000530: 7265 7175 6573 7427 293b 0d0a 0d0a 2020  request');....  
-00000540: 2020 2020 2020 7365 7453 7461 7475 7357        setStatusW
-00000550: 6169 7469 6e67 2829 3b0d 0a0d 0a20 2020  aiting();....   
-00000560: 2020 2020 2073 6574 5469 6d65 6f75 7428       setTimeout(
-00000570: 6765 7453 7461 7475 732c 2031 3030 290d  getStatus, 100).
-00000580: 0a20 2020 207d 2065 6c73 6520 6966 2028  .    } else if (
-00000590: 7365 7373 696f 6e5f 7374 6174 7573 203d  session_status =
-000005a0: 3d3d 2022 6163 7469 7665 2229 207b 0d0a  == "active") {..
-000005b0: 2020 2020 2020 2020 2f2f 2053 746f 7020          // Stop 
-000005c0: 7365 7373 696f 6e0d 0a20 2020 2020 2020  session..       
-000005d0: 2024 2e61 6a61 7828 7b0d 0a20 2020 2020   $.ajax({..     
-000005e0: 2020 2020 2020 2074 7970 653a 2022 504f         type: "PO
-000005f0: 5354 222c 0d0a 2020 2020 2020 2020 2020  ST",..          
-00000600: 2020 7572 6c3a 2022 2f61 7069 2f73 6573    url: "/api/ses
-00000610: 7369 6f6e 222c 0d0a 2020 2020 2020 2020  sion",..        
-00000620: 2020 2020 6461 7461 3a20 4a53 4f4e 2e73      data: JSON.s
-00000630: 7472 696e 6769 6679 287b 0d0a 2020 2020  tringify({..    
-00000640: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00000650: 3a20 2273 746f 7022 0d0a 2020 2020 2020  : "stop"..      
-00000660: 2020 2020 2020 7d29 2c0d 0a20 2020 2020        }),..     
-00000670: 2020 2020 2020 2064 6174 6154 7970 653a         dataType:
-00000680: 2022 6a73 6f6e 222c 0d0a 2020 2020 2020   "json",..      
-00000690: 2020 2020 2020 636f 6e74 656e 7454 7970        contentTyp
-000006a0: 653a 2022 6170 706c 6963 6174 696f 6e2f  e: "application/
-000006b0: 6a73 6f6e 220d 0a20 2020 2020 2020 207d  json"..        }
-000006c0: 290d 0a0d 0a20 2020 2020 2020 2063 6f6e  )....        con
-000006d0: 736f 6c65 2e6c 6f67 2827 7365 7373 696f  sole.log('sessio
-000006e0: 6e20 7374 6f70 2072 6571 7565 7374 2729  n stop request')
-000006f0: 3b0d 0a0d 0a20 2020 2020 2020 2073 6574  ;....        set
-00000700: 5374 6174 7573 5761 6974 696e 6728 293b  StatusWaiting();
-00000710: 0d0a 0d0a 2020 2020 2020 2020 6c65 7420  ....        let 
-00000720: 6e6f 7720 3d20 6e65 7720 4461 7465 2844  now = new Date(D
-00000730: 6174 652e 6e6f 7728 2929 2e74 6f49 534f  ate.now()).toISO
-00000740: 5374 7269 6e67 2829 3b0d 0a20 2020 2020  String();..     
-00000750: 2020 206c 6574 2073 746f 7054 696d 6545     let stopTimeE
-00000760: 7665 6e74 203d 2064 6f63 756d 656e 742e  vent = document.
-00000770: 6372 6561 7465 456c 656d 656e 7428 276c  createElement('l
-00000780: 6927 293b 0d0a 2020 2020 2020 2020 7374  i');..        st
-00000790: 6f70 5469 6d65 4576 656e 742e 696e 6e65  opTimeEvent.inne
-000007a0: 7248 544d 4c20 3d20 2253 6573 7369 6f6e  rHTML = "Session
-000007b0: 2073 746f 7070 6564 2061 7420 2220 2b20   stopped at " + 
-000007c0: 6e6f 773b 0d0a 2020 2020 2020 2020 6c6f  now;..        lo
-000007d0: 674c 6973 742e 7072 6570 656e 6428 7374  gList.prepend(st
-000007e0: 6f70 5469 6d65 4576 656e 7429 3b0d 0a0d  opTimeEvent);...
-000007f0: 0a20 2020 2020 2020 2073 6574 5469 6d65  .        setTime
-00000800: 6f75 7428 6765 7453 7461 7475 732c 2032  out(getStatus, 2
-00000810: 3030 290d 0a20 2020 207d 0d0a 2020 2020  00)..    }..    
-00000820: 7265 7475 726e 2066 616c 7365 3b0d 0a7d  return false;..}
-00000830: 3b0d 0a0d 0a66 756e 6374 696f 6e20 6765  ;....function ge
-00000840: 7453 7461 7475 7328 2920 7b0d 0a20 2020  tStatus() {..   
-00000850: 2024 2e67 6574 2822 2f61 7069 2f73 6573   $.get("/api/ses
-00000860: 7369 6f6e 222c 2066 756e 6374 696f 6e20  sion", function 
-00000870: 2864 6174 6129 207b 0d0a 2020 2020 2020  (data) {..      
-00000880: 2020 7365 7373 696f 6e5f 7374 6174 7573    session_status
-00000890: 203d 2064 6174 612e 7374 6174 7573 3b0d   = data.status;.
-000008a0: 0a20 2020 2020 2020 2069 6620 2873 6573  .        if (ses
-000008b0: 7369 6f6e 5f73 7461 7475 7320 3d3d 3d20  sion_status === 
-000008c0: 2261 6374 6976 6522 2920 7b0d 0a20 2020  "active") {..   
-000008d0: 2020 2020 2020 2020 206c 6574 2073 6573           let ses
-000008e0: 7369 6f6e 5f64 6174 6120 3d20 4a53 4f4e  sion_data = JSON
-000008f0: 2e70 6172 7365 2864 6174 612e 6461 7461  .parse(data.data
-00000900: 293b 0d0a 2020 2020 2020 2020 2020 2020  );..            
-00000910: 7365 7453 7461 7475 7341 6374 6976 6528  setStatusActive(
-00000920: 293b 0d0a 0d0a 2020 2020 2020 2020 2020  );....          
-00000930: 2020 636f 6e73 6f6c 652e 6c6f 6728 7365    console.log(se
-00000940: 7373 696f 6e5f 6461 7461 290d 0a0d 0a20  ssion_data).... 
-00000950: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-00000960: 6543 6861 7274 285b 0d0a 2020 2020 2020  eChart([..      
-00000970: 2020 2020 2020 2020 2020 7365 7373 696f            sessio
-00000980: 6e5f 6461 7461 2e74 7269 616c 732e 6669  n_data.trials.fi
-00000990: 6c74 6572 2828 6f62 6a29 203d 3e20 6f62  lter((obj) => ob
-000009a0: 6a2e 6f75 7463 6f6d 6520 3d3d 3d20 2763  j.outcome === 'c
-000009b0: 6f72 7265 6374 2729 2e6c 656e 6774 682c  orrect').length,
-000009c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000009d0: 2020 7365 7373 696f 6e5f 6461 7461 2e74    session_data.t
-000009e0: 7269 616c 732e 6669 6c74 6572 2828 6f62  rials.filter((ob
-000009f0: 6a29 203d 3e20 6f62 6a2e 6f75 7463 6f6d  j) => obj.outcom
-00000a00: 6520 3d3d 3d20 2769 6e63 6f72 7265 6374  e === 'incorrect
-00000a10: 2729 2e6c 656e 6774 682c 0d0a 2020 2020  ').length,..    
-00000a20: 2020 2020 2020 2020 2020 2020 7365 7373              sess
-00000a30: 696f 6e5f 6461 7461 2e74 7269 616c 732e  ion_data.trials.
-00000a40: 6669 6c74 6572 2828 6f62 6a29 203d 3e20  filter((obj) => 
-00000a50: 6f62 6a2e 6f75 7463 6f6d 6520 3d3d 3d20  obj.outcome === 
-00000a60: 2770 7265 6375 6564 2729 2e6c 656e 6774  'precued').lengt
-00000a70: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
-00000a80: 2020 2020 7365 7373 696f 6e5f 6461 7461      session_data
-00000a90: 2e74 7269 616c 732e 6669 6c74 6572 2828  .trials.filter((
-00000aa0: 6f62 6a29 203d 3e20 6f62 6a2e 6f75 7463  obj) => obj.outc
-00000ab0: 6f6d 6520 3d3d 3d20 276e 6f5f 7265 7370  ome === 'no_resp
-00000ac0: 6f6e 7365 2729 2e6c 656e 6774 680d 0a20  onse').length.. 
-00000ad0: 2020 2020 2020 2020 2020 205d 290d 0a0d             ])...
-00000ae0: 0a20 2020 2020 2020 2020 2020 2064 6f63  .            doc
-00000af0: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
-00000b00: 4279 4964 2827 616e 696d 616c 5f69 6427  ById('animal_id'
-00000b10: 292e 7661 6c75 6520 3d20 7365 7373 696f  ).value = sessio
-00000b20: 6e5f 6461 7461 2e61 6e69 6d61 6c5f 6964  n_data.animal_id
-00000b30: 3b0d 0a20 2020 2020 2020 2020 2020 2064  ;..            d
-00000b40: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
-00000b50: 6e74 4279 4964 2827 6578 7065 7269 6d65  ntById('experime
-00000b60: 6e74 2729 2e76 616c 7565 203d 2073 6573  nt').value = ses
-00000b70: 7369 6f6e 5f64 6174 612e 6578 7065 7269  sion_data.experi
-00000b80: 6d65 6e74 3b0d 0a20 2020 2020 2020 2020  ment;..         
-00000b90: 2020 2064 6f63 756d 656e 742e 6765 7445     document.getE
-00000ba0: 6c65 6d65 6e74 4279 4964 2827 7072 6f74  lementById('prot
-00000bb0: 6f63 6f6c 2729 2e76 616c 7565 203d 2073  ocol').value = s
-00000bc0: 6573 7369 6f6e 5f64 6174 612e 7072 6f74  ession_data.prot
-00000bd0: 6f63 6f6c 3b0d 0a20 2020 2020 2020 2020  ocol;..         
-00000be0: 2020 2064 6f63 756d 656e 742e 6765 7445     document.getE
-00000bf0: 6c65 6d65 6e74 4279 4964 2827 6475 7261  lementById('dura
-00000c00: 7469 6f6e 2729 2e76 616c 7565 203d 2073  tion').value = s
-00000c10: 6573 7369 6f6e 5f64 6174 612e 6475 7261  ession_data.dura
-00000c20: 7469 6f6e 3b0d 0a0d 0a20 2020 2020 2020  tion;....       
-00000c30: 2020 2020 206c 6f67 4c69 7374 2e69 6e6e       logList.inn
-00000c40: 6572 4854 4d4c 203d 2022 2220 2f2f 2043  erHTML = "" // C
-00000c50: 6c65 6172 2063 6f6e 7465 6e74 730d 0a20  lear contents.. 
-00000c60: 2020 2020 2020 2020 2020 2066 6f72 2028             for (
-00000c70: 6c65 7420 6920 3d20 7365 7373 696f 6e5f  let i = session_
-00000c80: 6461 7461 2e74 7269 616c 732e 6c65 6e67  data.trials.leng
-00000c90: 7468 202d 2031 3b20 6920 3e3d 2030 3b20  th - 1; i >= 0; 
-00000ca0: 692d 2d29 207b 0d0a 2020 2020 2020 2020  i--) {..        
-00000cb0: 2020 2020 2020 2020 6c65 7420 6576 656e          let even
-00000cc0: 7420 3d20 646f 6375 6d65 6e74 2e63 7265  t = document.cre
-00000cd0: 6174 6545 6c65 6d65 6e74 2827 6c69 2729  ateElement('li')
-00000ce0: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
-00000cf0: 2020 2065 7665 6e74 2e69 6e6e 6572 4854     event.innerHT
-00000d00: 4d4c 203d 2022 3c65 6d3e 2220 2b20 7365  ML = "<em>" + se
-00000d10: 7373 696f 6e5f 6461 7461 2e74 7269 616c  ssion_data.trial
-00000d20: 735b 695d 2e74 696d 6573 7461 6d70 202b  s[i].timestamp +
-00000d30: 2022 3a20 3c2f 656d 3e22 202b 2073 6573   ": </em>" + ses
-00000d40: 7369 6f6e 5f64 6174 612e 7472 6961 6c73  sion_data.trials
-00000d50: 5b69 5d2e 6f75 7463 6f6d 653b 0d0a 2020  [i].outcome;..  
-00000d60: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00000d70: 674c 6973 742e 6170 7065 6e64 4368 696c  gList.appendChil
-00000d80: 6428 6576 656e 7429 3b0d 0a20 2020 2020  d(event);..     
-00000d90: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
-00000da0: 2020 2020 2020 6c6f 674c 6973 742e 6170        logList.ap
-00000db0: 7065 6e64 2864 6f63 756d 656e 742e 6372  pend(document.cr
-00000dc0: 6561 7465 456c 656d 656e 7428 276c 6927  eateElement('li'
-00000dd0: 292e 696e 6e65 7248 544d 4c20 3d20 2253  ).innerHTML = "S
-00000de0: 6573 7369 6f6e 2073 7461 7274 6564 2061  ession started a
-00000df0: 7420 2220 2b20 7365 7373 696f 6e5f 6461  t " + session_da
-00000e00: 7461 2e74 696d 6573 7461 6d70 293b 0d0a  ta.timestamp);..
-00000e10: 0d0a 2020 2020 2020 2020 2020 2020 2f2f  ..            //
-00000e20: 2075 7064 6174 6520 7072 6f67 7265 7373   update progress
-00000e30: 2062 6172 0d0a 2020 2020 2020 2020 2020   bar..          
-00000e40: 2020 746f 7461 6c54 696d 654d 7320 3d20    totalTimeMs = 
-00000e50: 2870 6172 7365 496e 7428 7365 7373 696f  (parseInt(sessio
-00000e60: 6e5f 6461 7461 2e64 7572 6174 696f 6e29  n_data.duration)
-00000e70: 202a 2036 3030 3030 293b 0d0a 2020 2020   * 60000);..    
-00000e80: 2020 2020 2020 2020 7469 6d65 4c65 6674          timeLeft
-00000e90: 4d73 203d 2074 6f74 616c 5469 6d65 4d73  Ms = totalTimeMs
-00000ea0: 202d 2028 4461 7465 2e6e 6f77 2829 202d   - (Date.now() -
-00000eb0: 2044 6174 652e 7061 7273 6528 7365 7373   Date.parse(sess
-00000ec0: 696f 6e5f 6461 7461 2e74 696d 6573 7461  ion_data.timesta
-00000ed0: 6d70 2929 3b0d 0a20 2020 2020 2020 2020  mp));..         
-00000ee0: 2020 2074 696d 654c 6566 744d 696e 203d     timeLeftMin =
-00000ef0: 2074 696d 654c 6566 744d 7320 2f20 3630   timeLeftMs / 60
-00000f00: 3030 303b 0d0a 2020 2020 2020 2020 2020  000;..          
-00000f10: 2020 7072 6f67 7265 7373 4261 7257 6964    progressBarWid
-00000f20: 7468 203d 2028 3120 2d20 2874 696d 654c  th = (1 - (timeL
-00000f30: 6566 744d 7320 2f20 746f 7461 6c54 696d  eftMs / totalTim
-00000f40: 654d 7329 2920 2a20 3130 303b 0d0a 2020  eMs)) * 100;..  
-00000f50: 2020 2020 2020 2020 2020 636f 6e73 6f6c            consol
-00000f60: 652e 6c6f 6728 7072 6f67 7265 7373 4261  e.log(progressBa
-00000f70: 7257 6964 7468 293b 0d0a 2020 2020 2020  rWidth);..      
-00000f80: 2020 2020 2020 636f 6e73 6f6c 652e 6c6f        console.lo
-00000f90: 6728 7072 6f67 7265 7373 4261 7229 3b0d  g(progressBar);.
-00000fa0: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000fb0: 6772 6573 7342 6172 2e73 7479 6c65 2e77  gressBar.style.w
-00000fc0: 6964 7468 203d 2070 726f 6772 6573 7342  idth = progressB
-00000fd0: 6172 5769 6474 682e 746f 5374 7269 6e67  arWidth.toString
-00000fe0: 2829 202b 2022 2522 3b0d 0a20 2020 2020  () + "%";..     
-00000ff0: 2020 2020 2020 2070 726f 6772 6573 7342         progressB
-00001000: 6172 2e69 6e6e 6572 4854 4d4c 203d 2074  ar.innerHTML = t
-00001010: 696d 654c 6566 744d 696e 2e74 6f46 6978  imeLeftMin.toFix
-00001020: 6564 2831 292e 746f 5374 7269 6e67 2829  ed(1).toString()
-00001030: 202b 2022 206d 696e 206c 6566 7422 3b0d   + " min left";.
-00001040: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-00001050: 6620 2874 696d 654c 6566 744d 696e 203c  f (timeLeftMin <
-00001060: 3d20 3029 207b 0d0a 2020 2020 2020 2020  = 0) {..        
-00001070: 2020 2020 2020 2020 6c65 7420 6e6f 7720          let now 
-00001080: 3d20 6e65 7720 4461 7465 2844 6174 652e  = new Date(Date.
-00001090: 6e6f 7728 2929 2e74 6f49 534f 5374 7269  now()).toISOStri
-000010a0: 6e67 2829 3b0d 0a20 2020 2020 2020 2020  ng();..         
-000010b0: 2020 2020 2020 206c 6574 2066 696e 6973         let finis
-000010c0: 6854 696d 6545 7665 6e74 203d 2064 6f63  hTimeEvent = doc
-000010d0: 756d 656e 742e 6372 6561 7465 456c 656d  ument.createElem
-000010e0: 656e 7428 276c 6927 293b 0d0a 2020 2020  ent('li');..    
-000010f0: 2020 2020 2020 2020 2020 2020 6669 6e69              fini
-00001100: 7368 5469 6d65 4576 656e 742e 696e 6e65  shTimeEvent.inne
-00001110: 7248 544d 4c20 3d20 2253 6573 7369 6f6e  rHTML = "Session
-00001120: 2073 746f 7070 6564 2061 7420 2220 2b20   stopped at " + 
-00001130: 6e6f 773b 0d0a 2020 2020 2020 2020 2020  now;..          
-00001140: 2020 2020 2020 6c6f 674c 6973 742e 7072        logList.pr
-00001150: 6570 656e 6428 6669 6e69 7368 5469 6d65  epend(finishTime
-00001160: 4576 656e 7429 3b0d 0a20 2020 2020 2020  Event);..       
-00001170: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
-00001180: 2020 7d20 656c 7365 2069 6620 2873 6573    } else if (ses
-00001190: 7369 6f6e 5f73 7461 7475 7320 3d3d 3d20  sion_status === 
-000011a0: 2269 6e61 6374 6976 6522 2920 7b0d 0a20  "inactive") {.. 
-000011b0: 2020 2020 2020 2020 2020 2073 6574 5374             setSt
-000011c0: 6174 7573 496e 6163 7469 7665 2829 3b0d  atusInactive();.
-000011d0: 0a0d 0a20 2020 2020 2020 207d 2065 6c73  ...        } els
-000011e0: 6520 7b0d 0a20 2020 2020 2020 2020 2020  e {..           
-000011f0: 2073 6574 5374 6174 7573 5761 6974 696e   setStatusWaitin
-00001200: 6728 293b 0d0a 2020 2020 2020 2020 7d0d  g();..        }.
-00001210: 0a20 2020 207d 290d 0a7d 0d0a 0d0a 6c65  .    })..}....le
-00001220: 7420 7374 6174 7573 5f69 6e74 6572 7661  t status_interva
-00001230: 6c20 3d20 7365 7449 6e74 6572 7661 6c28  l = setInterval(
-00001240: 6765 7453 7461 7475 732c 2034 3030 3029  getStatus, 4000)
-00001250: 3b0d 0a0d 0a66 756e 6374 696f 6e20 7365  ;....function se
-00001260: 7453 7461 7475 7341 6374 6976 6528 2920  tStatusActive() 
-00001270: 7b0d 0a20 2020 2073 6573 7369 6f6e 5f62  {..    session_b
-00001280: 7574 746f 6e2e 636c 6173 734e 616d 6520  utton.className 
-00001290: 3d20 2262 746e 2062 746e 2d64 616e 6765  = "btn btn-dange
-000012a0: 7220 6274 6e2d 626c 6f63 6b20 6274 6e2d  r btn-block btn-
-000012b0: 6c67 223b 0d0a 2020 2020 7365 7373 696f  lg";..    sessio
-000012c0: 6e5f 6275 7474 6f6e 2e74 6578 7443 6f6e  n_button.textCon
-000012d0: 7465 6e74 203d 2022 5374 6f70 223b 0d0a  tent = "Stop";..
-000012e0: 0d0a 2020 2020 7374 6174 7573 5f69 636f  ..    status_ico
-000012f0: 6e2e 636c 6173 734e 616d 6520 3d20 2266  n.className = "f
-00001300: 6173 2066 612d 6369 7263 6c65 2074 6578  as fa-circle tex
-00001310: 742d 7375 6363 6573 7322 3b0d 0a20 2020  t-success";..   
-00001320: 2073 7461 7475 735f 7465 7874 2e63 6869   status_text.chi
-00001330: 6c64 4e6f 6465 735b 325d 2e6e 6f64 6556  ldNodes[2].nodeV
-00001340: 616c 7565 203d 2022 2052 756e 6e69 6e67  alue = " Running
-00001350: 223b 0d0a 0d0a 2020 2020 2f2f 2064 6973  ";....    // dis
-00001360: 6162 6c65 2069 6e70 7574 2066 6965 6c64  able input field
-00001370: 730d 0a20 2020 206c 6574 2066 6965 6c64  s..    let field
-00001380: 7320 3d20 666f 726d 2e67 6574 456c 656d  s = form.getElem
-00001390: 656e 7473 4279 436c 6173 734e 616d 6528  entsByClassName(
-000013a0: 2766 6f72 6d2d 636f 6e74 726f 6c27 293b  'form-control');
-000013b0: 0d0a 2020 2020 666f 7220 286c 6574 2069  ..    for (let i
-000013c0: 203d 2030 3b20 6920 3c20 6669 656c 6473   = 0; i < fields
-000013d0: 2e6c 656e 6774 683b 2069 2b2b 2920 7b0d  .length; i++) {.
-000013e0: 0a20 2020 2020 2020 2066 6965 6c64 735b  .        fields[
-000013f0: 695d 2e64 6973 6162 6c65 6420 3d20 7472  i].disabled = tr
-00001400: 7565 3b0d 0a20 2020 207d 0d0a 7d0d 0a0d  ue;..    }..}...
-00001410: 0a0d 0a66 756e 6374 696f 6e20 7365 7453  ...function setS
-00001420: 7461 7475 7349 6e61 6374 6976 6528 2920  tatusInactive() 
-00001430: 7b0d 0a20 2020 2073 6573 7369 6f6e 5f62  {..    session_b
-00001440: 7574 746f 6e2e 636c 6173 734e 616d 6520  utton.className 
-00001450: 3d20 2262 746e 2062 746e 2d73 7563 6365  = "btn btn-succe
-00001460: 7373 2062 746e 2d62 6c6f 636b 2062 746e  ss btn-block btn
-00001470: 2d6c 6722 3b0d 0a20 2020 2073 6573 7369  -lg";..    sessi
-00001480: 6f6e 5f62 7574 746f 6e2e 7465 7874 436f  on_button.textCo
-00001490: 6e74 656e 7420 3d20 2253 7461 7274 223b  ntent = "Start";
-000014a0: 0d0a 0d0a 2020 2020 7374 6174 7573 5f69  ....    status_i
-000014b0: 636f 6e2e 636c 6173 734e 616d 6520 3d20  con.className = 
-000014c0: 2266 6173 2066 612d 6369 7263 6c65 2074  "fas fa-circle t
-000014d0: 6578 742d 6461 6e67 6572 223b 0d0a 2020  ext-danger";..  
-000014e0: 2020 7374 6174 7573 5f74 6578 742e 6368    status_text.ch
-000014f0: 696c 644e 6f64 6573 5b32 5d2e 6e6f 6465  ildNodes[2].node
-00001500: 5661 6c75 6520 3d20 2220 4e6f 7420 5275  Value = " Not Ru
-00001510: 6e6e 696e 6722 3b0d 0a0d 0a20 2020 2070  nning";....    p
-00001520: 726f 6772 6573 7342 6172 2e73 7479 6c65  rogressBar.style
-00001530: 2e77 6964 7468 203d 2022 3025 223b 0d0a  .width = "0%";..
-00001540: 2020 2020 7072 6f67 7265 7373 4261 722e      progressBar.
-00001550: 696e 6e65 7248 544d 4c20 3d20 2222 3b0d  innerHTML = "";.
-00001560: 0a0d 0a0d 0a20 2020 202f 2f20 656e 6162  .....    // enab
-00001570: 6c65 2069 6e70 7574 2066 6965 6c64 730d  le input fields.
-00001580: 0a20 2020 206c 6574 2066 6965 6c64 7320  .    let fields 
-00001590: 3d20 666f 726d 2e67 6574 456c 656d 656e  = form.getElemen
-000015a0: 7473 4279 436c 6173 734e 616d 6528 2766  tsByClassName('f
-000015b0: 6f72 6d2d 636f 6e74 726f 6c27 293b 0d0a  orm-control');..
-000015c0: 2020 2020 666f 7220 286c 6574 2069 203d      for (let i =
-000015d0: 2030 3b20 6920 3c20 6669 656c 6473 2e6c   0; i < fields.l
-000015e0: 656e 6774 683b 2069 2b2b 2920 7b0d 0a20  ength; i++) {.. 
-000015f0: 2020 2020 2020 2066 6965 6c64 735b 695d         fields[i]
-00001600: 2e64 6973 6162 6c65 6420 3d20 6661 6c73  .disabled = fals
-00001610: 653b 0d0a 2020 2020 7d0d 0a7d 0d0a 0d0a  e;..    }..}....
-00001620: 0d0a 6675 6e63 7469 6f6e 2073 6574 5374  ..function setSt
-00001630: 6174 7573 5761 6974 696e 6728 2920 7b0d  atusWaiting() {.
-00001640: 0a20 2020 2073 6573 7369 6f6e 5f62 7574  .    session_but
-00001650: 746f 6e2e 636c 6173 734e 616d 6520 3d20  ton.className = 
-00001660: 2262 746e 2062 746e 2d6c 6967 6874 2062  "btn btn-light b
-00001670: 746e 2d62 6c6f 636b 2062 746e 2d6c 6722  tn-block btn-lg"
-00001680: 3b0d 0a20 2020 2073 6573 7369 6f6e 5f62  ;..    session_b
-00001690: 7574 746f 6e2e 7465 7874 436f 6e74 656e  utton.textConten
-000016a0: 7420 3d20 2257 6169 7469 6e67 2e2e 2e22  t = "Waiting..."
-000016b0: 3b0d 0a0d 0a20 2020 2073 7461 7475 735f  ;....    status_
-000016c0: 6963 6f6e 2e63 6c61 7373 4e61 6d65 203d  icon.className =
-000016d0: 2022 6661 7320 6661 2d63 6972 636c 6520   "fas fa-circle 
-000016e0: 7465 7874 2d77 6172 6e69 6e67 223b 0d0a  text-warning";..
-000016f0: 2020 2020 7374 6174 7573 5f74 6578 742e      status_text.
-00001700: 6368 696c 644e 6f64 6573 5b32 5d2e 6e6f  childNodes[2].no
-00001710: 6465 5661 6c75 6520 3d20 2220 5761 6974  deValue = " Wait
-00001720: 696e 6722 3b0d 0a0d 0a20 2020 202f 2f20  ing";....    // 
-00001730: 656e 6162 6c65 2069 6e70 7574 2066 6965  enable input fie
-00001740: 6c64 730d 0a20 2020 206c 6574 2066 6965  lds..    let fie
-00001750: 6c64 7320 3d20 666f 726d 2e67 6574 456c  lds = form.getEl
-00001760: 656d 656e 7473 4279 436c 6173 734e 616d  ementsByClassNam
-00001770: 6528 2766 6f72 6d2d 636f 6e74 726f 6c27  e('form-control'
-00001780: 293b 0d0a 2020 2020 666f 7220 286c 6574  );..    for (let
-00001790: 2069 203d 2030 3b20 6920 3c20 6669 656c   i = 0; i < fiel
-000017a0: 6473 2e6c 656e 6774 683b 2069 2b2b 2920  ds.length; i++) 
-000017b0: 7b0d 0a20 2020 2020 2020 2066 6965 6c64  {..        field
-000017c0: 735b 695d 2e64 6973 6162 6c65 6420 3d20  s[i].disabled = 
-000017d0: 7472 7565 3b0d 0a20 2020 207d 0d0a 7d0d  true;..    }..}.
-000017e0: 0a0d 0a2f 2f2f 2043 6861 7274 0d0a 0d0a  .../// Chart....
-000017f0: 6675 6e63 7469 6f6e 2075 7064 6174 6543  function updateC
-00001800: 6861 7274 2864 6174 6129 207b 0d0a 2020  hart(data) {..  
-00001810: 2020 6966 2028 6973 4361 6e76 6173 426c    if (isCanvasBl
-00001820: 616e 6b28 6374 7829 2920 7b0d 0a20 2020  ank(ctx)) {..   
-00001830: 2020 2020 2074 7269 616c 7343 6861 7274       trialsChart
-00001840: 203d 2063 7265 6174 6543 6861 7274 2864   = createChart(d
-00001850: 6174 6129 3b0d 0a20 2020 207d 0d0a 2020  ata);..    }..  
-00001860: 2020 656c 7365 207b 0d0a 2020 2020 2020    else {..      
-00001870: 2020 7472 6961 6c73 4368 6172 742e 6461    trialsChart.da
-00001880: 7461 2e64 6174 6173 6574 732e 666f 7245  ta.datasets.forE
-00001890: 6163 6828 2864 6174 6173 6574 2920 3d3e  ach((dataset) =>
-000018a0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000018b0: 6461 7461 7365 742e 6461 7461 203d 2064  dataset.data = d
-000018c0: 6174 613b 0d0a 2020 2020 2020 2020 7d29  ata;..        })
-000018d0: 3b0d 0a20 2020 2020 2020 2074 7269 616c  ;..        trial
-000018e0: 7343 6861 7274 2e75 7064 6174 6528 293b  sChart.update();
-000018f0: 0d0a 2020 2020 7d0d 0a7d 0d0a 0d0a 6675  ..    }..}....fu
-00001900: 6e63 7469 6f6e 2063 7265 6174 6543 6861  nction createCha
-00001910: 7274 2864 6174 6129 207b 0d0a 2020 2020  rt(data) {..    
-00001920: 6c65 7420 6e65 7743 6861 7274 203d 206e  let newChart = n
-00001930: 6577 2043 6861 7274 2863 7478 2c20 7b0d  ew Chart(ctx, {.
-00001940: 0a20 2020 2020 2020 2074 7970 653a 2027  .        type: '
-00001950: 646f 7567 686e 7574 272c 0d0a 2020 2020  doughnut',..    
-00001960: 2020 2020 6461 7461 3a20 7b0d 0a20 2020      data: {..   
-00001970: 2020 2020 2020 2020 206c 6162 656c 733a           labels:
-00001980: 205b 2743 6f72 7265 6374 272c 2027 496e   ['Correct', 'In
-00001990: 636f 7272 6563 7427 2c20 2750 7265 6375  correct', 'Precu
-000019a0: 6564 272c 2027 4e6f 2052 6573 706f 6e73  ed', 'No Respons
-000019b0: 6527 5d2c 0d0a 2020 2020 2020 2020 2020  e'],..          
-000019c0: 2020 6461 7461 7365 7473 3a20 5b7b 0d0a    datasets: [{..
-000019d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019e0: 6c61 6265 6c3a 2027 2320 6f66 2054 7269  label: '# of Tri
-000019f0: 616c 7327 2c0d 0a20 2020 2020 2020 2020  als',..         
-00001a00: 2020 2020 2020 2064 6174 613a 2064 6174         data: dat
-00001a10: 612c 0d0a 2020 2020 2020 2020 2020 2020  a,..            
-00001a20: 2020 2020 626f 7264 6572 5769 6474 683a      borderWidth:
-00001a30: 2031 0d0a 2020 2020 2020 2020 2020 2020   1..            
-00001a40: 7d5d 0d0a 2020 2020 2020 2020 7d2c 0d0a  }]..        },..
-00001a50: 2020 2020 2020 2020 6f70 7469 6f6e 733a          options:
-00001a60: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00001a70: 6465 7669 6365 5069 7865 6c52 6174 696f  devicePixelRatio
-00001a80: 3a20 332c 0d0a 2020 2020 2020 2020 2020  : 3,..          
-00001a90: 2020 7265 7370 6f6e 7369 7665 3a20 7472    responsive: tr
-00001aa0: 7565 2c0d 0a20 2020 2020 2020 2020 2020  ue,..           
-00001ab0: 2070 6c75 6769 6e73 3a20 7b0d 0a20 2020   plugins: {..   
-00001ac0: 2020 2020 2020 2020 2020 2020 206c 6567               leg
-00001ad0: 656e 643a 207b 0d0a 2020 2020 2020 2020  end: {..        
-00001ae0: 2020 2020 2020 2020 2020 2020 6469 7370              disp
-00001af0: 6c61 793a 2074 7275 652c 0d0a 2020 2020  lay: true,..    
+00000390: 6365 2828 5f2c 2078 2920 3d3e 2028 7b20  ce((_, x) => ({ 
+000003a0: 2e2e 2e5f 2c20 5b78 2e69 645d 3a20 782e  ..._, [x.id]: x.
+000003b0: 7661 6c75 6520 7d29 2c20 7b7d 293b 0d0a  value }), {});..
+000003c0: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+000003d0: 6c6f 6728 4a53 4f4e 2e73 7472 696e 6769  log(JSON.stringi
+000003e0: 6679 2872 6571 7565 7374 2929 0d0a 0d0a  fy(request))....
+000003f0: 2020 2020 2020 2020 242e 616a 6178 287b          $.ajax({
+00000400: 0d0a 2020 2020 2020 2020 2020 2020 7479  ..            ty
+00000410: 7065 3a20 2750 4f53 5427 2c0d 0a20 2020  pe: 'POST',..   
+00000420: 2020 2020 2020 2020 2075 726c 3a20 222f           url: "/
+00000430: 6170 692f 7365 7373 696f 6e22 2c0d 0a20  api/session",.. 
+00000440: 2020 2020 2020 2020 2020 2064 6174 613a             data:
+00000450: 204a 534f 4e2e 7374 7269 6e67 6966 7928   JSON.stringify(
+00000460: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
+00000470: 2020 2074 7970 653a 2022 7374 6172 7422     type: "start"
+00000480: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000490: 2020 2064 6174 613a 2072 6571 7565 7374     data: request
+000004a0: 2c0d 0a20 2020 2020 2020 2020 2020 207d  ,..            }
+000004b0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+000004c0: 6461 7461 5479 7065 3a20 226a 736f 6e22  dataType: "json"
+000004d0: 2c0d 0a20 2020 2020 2020 2020 2020 2063  ,..            c
+000004e0: 6f6e 7465 6e74 5479 7065 3a20 2261 7070  ontentType: "app
+000004f0: 6c69 6361 7469 6f6e 2f6a 736f 6e22 0d0a  lication/json"..
+00000500: 2020 2020 2020 2020 7d29 3b0d 0a0d 0a20          });.... 
+00000510: 2020 2020 2020 2063 6f6e 736f 6c65 2e6c         console.l
+00000520: 6f67 2827 7365 7373 696f 6e20 7374 6172  og('session star
+00000530: 7420 7265 7175 6573 7427 293b 0d0a 0d0a  t request');....
+00000540: 2020 2020 2020 2020 7365 7453 7461 7475          setStatu
+00000550: 7357 6169 7469 6e67 2829 3b0d 0a0d 0a20  sWaiting();.... 
+00000560: 2020 2020 2020 2073 6574 5469 6d65 6f75         setTimeou
+00000570: 7428 6765 7453 7461 7475 732c 2031 3030  t(getStatus, 100
+00000580: 290d 0a20 2020 207d 2065 6c73 6520 6966  )..    } else if
+00000590: 2028 7365 7373 696f 6e5f 7374 6174 7573   (session_status
+000005a0: 203d 3d3d 2022 6163 7469 7665 2229 207b   === "active") {
+000005b0: 0d0a 2020 2020 2020 2020 2f2f 2053 746f  ..        // Sto
+000005c0: 7020 7365 7373 696f 6e0d 0a20 2020 2020  p session..     
+000005d0: 2020 2024 2e61 6a61 7828 7b0d 0a20 2020     $.ajax({..   
+000005e0: 2020 2020 2020 2020 2074 7970 653a 2022           type: "
+000005f0: 504f 5354 222c 0d0a 2020 2020 2020 2020  POST",..        
+00000600: 2020 2020 7572 6c3a 2022 2f61 7069 2f73      url: "/api/s
+00000610: 6573 7369 6f6e 222c 0d0a 2020 2020 2020  ession",..      
+00000620: 2020 2020 2020 6461 7461 3a20 4a53 4f4e        data: JSON
+00000630: 2e73 7472 696e 6769 6679 287b 0d0a 2020  .stringify({..  
+00000640: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00000650: 7065 3a20 2273 746f 7022 0d0a 2020 2020  pe: "stop"..    
+00000660: 2020 2020 2020 2020 7d29 2c0d 0a20 2020          }),..   
+00000670: 2020 2020 2020 2020 2064 6174 6154 7970           dataTyp
+00000680: 653a 2022 6a73 6f6e 222c 0d0a 2020 2020  e: "json",..    
+00000690: 2020 2020 2020 2020 636f 6e74 656e 7454          contentT
+000006a0: 7970 653a 2022 6170 706c 6963 6174 696f  ype: "applicatio
+000006b0: 6e2f 6a73 6f6e 220d 0a20 2020 2020 2020  n/json"..       
+000006c0: 207d 290d 0a0d 0a20 2020 2020 2020 2063   })....        c
+000006d0: 6f6e 736f 6c65 2e6c 6f67 2827 7365 7373  onsole.log('sess
+000006e0: 696f 6e20 7374 6f70 2072 6571 7565 7374  ion stop request
+000006f0: 2729 3b0d 0a0d 0a20 2020 2020 2020 2073  ');....        s
+00000700: 6574 5374 6174 7573 5761 6974 696e 6728  etStatusWaiting(
+00000710: 293b 0d0a 0d0a 2020 2020 2020 2020 6c65  );....        le
+00000720: 7420 6e6f 7720 3d20 6e65 7720 4461 7465  t now = new Date
+00000730: 2844 6174 652e 6e6f 7728 2929 2e74 6f49  (Date.now()).toI
+00000740: 534f 5374 7269 6e67 2829 3b0d 0a20 2020  SOString();..   
+00000750: 2020 2020 206c 6574 2073 746f 7054 696d       let stopTim
+00000760: 6545 7665 6e74 203d 2064 6f63 756d 656e  eEvent = documen
+00000770: 742e 6372 6561 7465 456c 656d 656e 7428  t.createElement(
+00000780: 276c 6927 293b 0d0a 2020 2020 2020 2020  'li');..        
+00000790: 7374 6f70 5469 6d65 4576 656e 742e 696e  stopTimeEvent.in
+000007a0: 6e65 7248 544d 4c20 3d20 2253 6573 7369  nerHTML = "Sessi
+000007b0: 6f6e 2073 746f 7070 6564 2061 7420 2220  on stopped at " 
+000007c0: 2b20 6e6f 773b 0d0a 2020 2020 2020 2020  + now;..        
+000007d0: 6c6f 674c 6973 742e 7072 6570 656e 6428  logList.prepend(
+000007e0: 7374 6f70 5469 6d65 4576 656e 7429 3b0d  stopTimeEvent);.
+000007f0: 0a0d 0a20 2020 2020 2020 2073 6574 5469  ...        setTi
+00000800: 6d65 6f75 7428 6765 7453 7461 7475 732c  meout(getStatus,
+00000810: 2032 3030 290d 0a20 2020 207d 0d0a 2020   200)..    }..  
+00000820: 2020 7265 7475 726e 2066 616c 7365 3b0d    return false;.
+00000830: 0a7d 3b0d 0a0d 0a66 756e 6374 696f 6e20  .};....function 
+00000840: 6765 7453 7461 7475 7328 2920 7b0d 0a20  getStatus() {.. 
+00000850: 2020 2024 2e67 6574 2822 2f61 7069 2f73     $.get("/api/s
+00000860: 6573 7369 6f6e 222c 2066 756e 6374 696f  ession", functio
+00000870: 6e20 2864 6174 6129 207b 0d0a 2020 2020  n (data) {..    
+00000880: 2020 2020 7365 7373 696f 6e5f 7374 6174      session_stat
+00000890: 7573 203d 2064 6174 612e 7374 6174 7573  us = data.status
+000008a0: 3b0d 0a20 2020 2020 2020 2069 6620 2873  ;..        if (s
+000008b0: 6573 7369 6f6e 5f73 7461 7475 7320 3d3d  ession_status ==
+000008c0: 3d20 2261 6374 6976 6522 2920 7b0d 0a20  = "active") {.. 
+000008d0: 2020 2020 2020 2020 2020 206c 6574 2073             let s
+000008e0: 6573 7369 6f6e 5f64 6174 6120 3d20 4a53  ession_data = JS
+000008f0: 4f4e 2e70 6172 7365 2864 6174 612e 6461  ON.parse(data.da
+00000900: 7461 293b 0d0a 2020 2020 2020 2020 2020  ta);..          
+00000910: 2020 7365 7453 7461 7475 7341 6374 6976    setStatusActiv
+00000920: 6528 293b 0d0a 0d0a 2020 2020 2020 2020  e();....        
+00000930: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00000940: 7365 7373 696f 6e5f 6461 7461 290d 0a0d  session_data)...
+00000950: 0a20 2020 2020 2020 2020 2020 2075 7064  .            upd
+00000960: 6174 6543 6861 7274 285b 0d0a 2020 2020  ateChart([..    
+00000970: 2020 2020 2020 2020 2020 2020 7365 7373              sess
+00000980: 696f 6e5f 6461 7461 2e74 7269 616c 732e  ion_data.trials.
+00000990: 6669 6c74 6572 2828 6f62 6a29 203d 3e20  filter((obj) => 
+000009a0: 6f62 6a2e 6f75 7463 6f6d 6520 3d3d 3d20  obj.outcome === 
+000009b0: 2763 6f72 7265 6374 2729 2e6c 656e 6774  'correct').lengt
+000009c0: 682c 0d0a 2020 2020 2020 2020 2020 2020  h,..            
+000009d0: 2020 2020 7365 7373 696f 6e5f 6461 7461      session_data
+000009e0: 2e74 7269 616c 732e 6669 6c74 6572 2828  .trials.filter((
+000009f0: 6f62 6a29 203d 3e20 6f62 6a2e 6f75 7463  obj) => obj.outc
+00000a00: 6f6d 6520 3d3d 3d20 2769 6e63 6f72 7265  ome === 'incorre
+00000a10: 6374 2729 2e6c 656e 6774 682c 0d0a 2020  ct').length,..  
+00000a20: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00000a30: 7373 696f 6e5f 6461 7461 2e74 7269 616c  ssion_data.trial
+00000a40: 732e 6669 6c74 6572 2828 6f62 6a29 203d  s.filter((obj) =
+00000a50: 3e20 6f62 6a2e 6f75 7463 6f6d 6520 3d3d  > obj.outcome ==
+00000a60: 3d20 2770 7265 6375 6564 2729 2e6c 656e  = 'precued').len
+00000a70: 6774 682c 0d0a 2020 2020 2020 2020 2020  gth,..          
+00000a80: 2020 2020 2020 7365 7373 696f 6e5f 6461        session_da
+00000a90: 7461 2e74 7269 616c 732e 6669 6c74 6572  ta.trials.filter
+00000aa0: 2828 6f62 6a29 203d 3e20 6f62 6a2e 6f75  ((obj) => obj.ou
+00000ab0: 7463 6f6d 6520 3d3d 3d20 276e 6f5f 7265  tcome === 'no_re
+00000ac0: 7370 6f6e 7365 2729 2e6c 656e 6774 680d  sponse').length.
+00000ad0: 0a20 2020 2020 2020 2020 2020 205d 290d  .            ]).
+00000ae0: 0a0d 0a20 2020 2020 2020 2020 2020 2064  ...            d
+00000af0: 6f63 756d 656e 742e 6765 7445 6c65 6d65  ocument.getEleme
+00000b00: 6e74 4279 4964 2827 616e 696d 616c 5f69  ntById('animal_i
+00000b10: 6427 292e 7661 6c75 6520 3d20 7365 7373  d').value = sess
+00000b20: 696f 6e5f 6461 7461 2e61 6e69 6d61 6c5f  ion_data.animal_
+00000b30: 6964 3b0d 0a20 2020 2020 2020 2020 2020  id;..           
+00000b40: 2064 6f63 756d 656e 742e 6765 7445 6c65   document.getEle
+00000b50: 6d65 6e74 4279 4964 2827 6578 7065 7269  mentById('experi
+00000b60: 6d65 6e74 2729 2e76 616c 7565 203d 2073  ment').value = s
+00000b70: 6573 7369 6f6e 5f64 6174 612e 6578 7065  ession_data.expe
+00000b80: 7269 6d65 6e74 3b0d 0a20 2020 2020 2020  riment;..       
+00000b90: 2020 2020 2064 6f63 756d 656e 742e 6765       document.ge
+00000ba0: 7445 6c65 6d65 6e74 4279 4964 2827 7072  tElementById('pr
+00000bb0: 6f74 6f63 6f6c 2729 2e76 616c 7565 203d  otocol').value =
+00000bc0: 2073 6573 7369 6f6e 5f64 6174 612e 7072   session_data.pr
+00000bd0: 6f74 6f63 6f6c 3b0d 0a20 2020 2020 2020  otocol;..       
+00000be0: 2020 2020 2064 6f63 756d 656e 742e 6765       document.ge
+00000bf0: 7445 6c65 6d65 6e74 4279 4964 2827 6475  tElementById('du
+00000c00: 7261 7469 6f6e 2729 2e76 616c 7565 203d  ration').value =
+00000c10: 2073 6573 7369 6f6e 5f64 6174 612e 6475   session_data.du
+00000c20: 7261 7469 6f6e 3b0d 0a0d 0a20 2020 2020  ration;....     
+00000c30: 2020 2020 2020 206c 6f67 4c69 7374 2e69         logList.i
+00000c40: 6e6e 6572 4854 4d4c 203d 2022 2220 2f2f  nnerHTML = "" //
+00000c50: 2043 6c65 6172 2063 6f6e 7465 6e74 730d   Clear contents.
+00000c60: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00000c70: 2028 6c65 7420 6920 3d20 7365 7373 696f   (let i = sessio
+00000c80: 6e5f 6461 7461 2e74 7269 616c 732e 6c65  n_data.trials.le
+00000c90: 6e67 7468 202d 2031 3b20 6920 3e3d 2030  ngth - 1; i >= 0
+00000ca0: 3b20 692d 2d29 207b 0d0a 2020 2020 2020  ; i--) {..      
+00000cb0: 2020 2020 2020 2020 2020 6c65 7420 6576            let ev
+00000cc0: 656e 7420 3d20 646f 6375 6d65 6e74 2e63  ent = document.c
+00000cd0: 7265 6174 6545 6c65 6d65 6e74 2827 6c69  reateElement('li
+00000ce0: 2729 3b0d 0a20 2020 2020 2020 2020 2020  ');..           
+00000cf0: 2020 2020 2065 7665 6e74 2e69 6e6e 6572       event.inner
+00000d00: 4854 4d4c 203d 2022 3c65 6d3e 2220 2b20  HTML = "<em>" + 
+00000d10: 7365 7373 696f 6e5f 6461 7461 2e74 7269  session_data.tri
+00000d20: 616c 735b 695d 2e74 696d 6573 7461 6d70  als[i].timestamp
+00000d30: 202b 2022 3a20 3c2f 656d 3e22 202b 2073   + ": </em>" + s
+00000d40: 6573 7369 6f6e 5f64 6174 612e 7472 6961  ession_data.tria
+00000d50: 6c73 5b69 5d2e 6f75 7463 6f6d 653b 0d0a  ls[i].outcome;..
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 6c6f 674c 6973 742e 6170 7065 6e64 4368  logList.appendCh
+00000d80: 696c 6428 6576 656e 7429 3b0d 0a20 2020  ild(event);..   
+00000d90: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00000da0: 2020 2020 2020 2020 6c6f 674c 6973 742e          logList.
+00000db0: 6170 7065 6e64 2864 6f63 756d 656e 742e  append(document.
+00000dc0: 6372 6561 7465 456c 656d 656e 7428 276c  createElement('l
+00000dd0: 6927 292e 696e 6e65 7248 544d 4c20 3d20  i').innerHTML = 
+00000de0: 2253 6573 7369 6f6e 2073 7461 7274 6564  "Session started
+00000df0: 2061 7420 2220 2b20 7365 7373 696f 6e5f   at " + session_
+00000e00: 6461 7461 2e74 696d 6573 7461 6d70 293b  data.timestamp);
+00000e10: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00000e20: 2f2f 2075 7064 6174 6520 7072 6f67 7265  // update progre
+00000e30: 7373 2062 6172 0d0a 2020 2020 2020 2020  ss bar..        
+00000e40: 2020 2020 746f 7461 6c54 696d 654d 7320      totalTimeMs 
+00000e50: 3d20 2870 6172 7365 496e 7428 7365 7373  = (parseInt(sess
+00000e60: 696f 6e5f 6461 7461 2e64 7572 6174 696f  ion_data.duratio
+00000e70: 6e29 202a 2036 3030 3030 293b 0d0a 2020  n) * 60000);..  
+00000e80: 2020 2020 2020 2020 2020 7469 6d65 4c65            timeLe
+00000e90: 6674 4d73 203d 2074 6f74 616c 5469 6d65  ftMs = totalTime
+00000ea0: 4d73 202d 2028 4461 7465 2e6e 6f77 2829  Ms - (Date.now()
+00000eb0: 202d 2044 6174 652e 7061 7273 6528 7365   - Date.parse(se
+00000ec0: 7373 696f 6e5f 6461 7461 2e74 696d 6573  ssion_data.times
+00000ed0: 7461 6d70 2929 3b0d 0a20 2020 2020 2020  tamp));..       
+00000ee0: 2020 2020 2074 696d 654c 6566 744d 696e       timeLeftMin
+00000ef0: 203d 2074 696d 654c 6566 744d 7320 2f20   = timeLeftMs / 
+00000f00: 3630 3030 303b 0d0a 2020 2020 2020 2020  60000;..        
+00000f10: 2020 2020 7072 6f67 7265 7373 4261 7257      progressBarW
+00000f20: 6964 7468 203d 2028 3120 2d20 2874 696d  idth = (1 - (tim
+00000f30: 654c 6566 744d 7320 2f20 746f 7461 6c54  eLeftMs / totalT
+00000f40: 696d 654d 7329 2920 2a20 3130 303b 0d0a  imeMs)) * 100;..
+00000f50: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000f60: 6f6c 652e 6c6f 6728 7072 6f67 7265 7373  ole.log(progress
+00000f70: 4261 7257 6964 7468 293b 0d0a 2020 2020  BarWidth);..    
+00000f80: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00000f90: 6c6f 6728 7072 6f67 7265 7373 4261 7229  log(progressBar)
+00000fa0: 3b0d 0a20 2020 2020 2020 2020 2020 2070  ;..            p
+00000fb0: 726f 6772 6573 7342 6172 2e73 7479 6c65  rogressBar.style
+00000fc0: 2e77 6964 7468 203d 2070 726f 6772 6573  .width = progres
+00000fd0: 7342 6172 5769 6474 682e 746f 5374 7269  sBarWidth.toStri
+00000fe0: 6e67 2829 202b 2022 2522 3b0d 0a20 2020  ng() + "%";..   
+00000ff0: 2020 2020 2020 2020 2070 726f 6772 6573           progres
+00001000: 7342 6172 2e69 6e6e 6572 4854 4d4c 203d  sBar.innerHTML =
+00001010: 2074 696d 654c 6566 744d 696e 2e74 6f46   timeLeftMin.toF
+00001020: 6978 6564 2831 292e 746f 5374 7269 6e67  ixed(1).toString
+00001030: 2829 202b 2022 206d 696e 206c 6566 7422  () + " min left"
+00001040: 3b0d 0a0d 0a20 2020 2020 2020 2020 2020  ;....           
+00001050: 2069 6620 2874 696d 654c 6566 744d 696e   if (timeLeftMin
+00001060: 203c 3d20 3029 207b 0d0a 2020 2020 2020   <= 0) {..      
+00001070: 2020 2020 2020 2020 2020 6c65 7420 6e6f            let no
+00001080: 7720 3d20 6e65 7720 4461 7465 2844 6174  w = new Date(Dat
+00001090: 652e 6e6f 7728 2929 2e74 6f49 534f 5374  e.now()).toISOSt
+000010a0: 7269 6e67 2829 3b0d 0a20 2020 2020 2020  ring();..       
+000010b0: 2020 2020 2020 2020 206c 6574 2066 696e           let fin
+000010c0: 6973 6854 696d 6545 7665 6e74 203d 2064  ishTimeEvent = d
+000010d0: 6f63 756d 656e 742e 6372 6561 7465 456c  ocument.createEl
+000010e0: 656d 656e 7428 276c 6927 293b 0d0a 2020  ement('li');..  
+000010f0: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+00001100: 6e69 7368 5469 6d65 4576 656e 742e 696e  nishTimeEvent.in
+00001110: 6e65 7248 544d 4c20 3d20 2253 6573 7369  nerHTML = "Sessi
+00001120: 6f6e 2073 746f 7070 6564 2061 7420 2220  on stopped at " 
+00001130: 2b20 6e6f 773b 0d0a 2020 2020 2020 2020  + now;..        
+00001140: 2020 2020 2020 2020 6c6f 674c 6973 742e          logList.
+00001150: 7072 6570 656e 6428 6669 6e69 7368 5469  prepend(finishTi
+00001160: 6d65 4576 656e 7429 3b0d 0a20 2020 2020  meEvent);..     
+00001170: 2020 2020 2020 207d 0d0a 0d0a 2020 2020         }....    
+00001180: 2020 2020 7d20 656c 7365 2069 6620 2873      } else if (s
+00001190: 6573 7369 6f6e 5f73 7461 7475 7320 3d3d  ession_status ==
+000011a0: 3d20 2269 6e61 6374 6976 6522 2920 7b0d  = "inactive") {.
+000011b0: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
+000011c0: 5374 6174 7573 496e 6163 7469 7665 2829  StatusInactive()
+000011d0: 3b0d 0a0d 0a20 2020 2020 2020 207d 2065  ;....        } e
+000011e0: 6c73 6520 7b0d 0a20 2020 2020 2020 2020  lse {..         
+000011f0: 2020 2073 6574 5374 6174 7573 5761 6974     setStatusWait
+00001200: 696e 6728 293b 0d0a 2020 2020 2020 2020  ing();..        
+00001210: 7d0d 0a20 2020 207d 290d 0a7d 0d0a 0d0a  }..    })..}....
+00001220: 6c65 7420 7374 6174 7573 5f69 6e74 6572  let status_inter
+00001230: 7661 6c20 3d20 7365 7449 6e74 6572 7661  val = setInterva
+00001240: 6c28 6765 7453 7461 7475 732c 2034 3030  l(getStatus, 400
+00001250: 3029 3b0d 0a0d 0a66 756e 6374 696f 6e20  0);....function 
+00001260: 7365 7453 7461 7475 7341 6374 6976 6528  setStatusActive(
+00001270: 2920 7b0d 0a20 2020 2073 6573 7369 6f6e  ) {..    session
+00001280: 5f62 7574 746f 6e2e 636c 6173 734e 616d  _button.classNam
+00001290: 6520 3d20 2262 746e 2062 746e 2d64 616e  e = "btn btn-dan
+000012a0: 6765 7220 6274 6e2d 626c 6f63 6b20 6274  ger btn-block bt
+000012b0: 6e2d 6c67 223b 0d0a 2020 2020 7365 7373  n-lg";..    sess
+000012c0: 696f 6e5f 6275 7474 6f6e 2e74 6578 7443  ion_button.textC
+000012d0: 6f6e 7465 6e74 203d 2022 5374 6f70 223b  ontent = "Stop";
+000012e0: 0d0a 0d0a 2020 2020 7374 6174 7573 5f69  ....    status_i
+000012f0: 636f 6e2e 636c 6173 734e 616d 6520 3d20  con.className = 
+00001300: 2266 6173 2066 612d 6369 7263 6c65 2074  "fas fa-circle t
+00001310: 6578 742d 7375 6363 6573 7322 3b0d 0a20  ext-success";.. 
+00001320: 2020 2073 7461 7475 735f 7465 7874 2e63     status_text.c
+00001330: 6869 6c64 4e6f 6465 735b 325d 2e6e 6f64  hildNodes[2].nod
+00001340: 6556 616c 7565 203d 2022 2052 756e 6e69  eValue = " Runni
+00001350: 6e67 223b 0d0a 0d0a 2020 2020 2f2f 2064  ng";....    // d
+00001360: 6973 6162 6c65 2069 6e70 7574 2066 6965  isable input fie
+00001370: 6c64 730d 0a20 2020 206c 6574 2066 6965  lds..    let fie
+00001380: 6c64 7320 3d20 666f 726d 2e67 6574 456c  lds = form.getEl
+00001390: 656d 656e 7473 4279 436c 6173 734e 616d  ementsByClassNam
+000013a0: 6528 2766 6f72 6d2d 636f 6e74 726f 6c27  e('form-control'
+000013b0: 293b 0d0a 2020 2020 666f 7220 286c 6574  );..    for (let
+000013c0: 2069 203d 2030 3b20 6920 3c20 6669 656c   i = 0; i < fiel
+000013d0: 6473 2e6c 656e 6774 683b 2069 2b2b 2920  ds.length; i++) 
+000013e0: 7b0d 0a20 2020 2020 2020 2066 6965 6c64  {..        field
+000013f0: 735b 695d 2e64 6973 6162 6c65 6420 3d20  s[i].disabled = 
+00001400: 7472 7565 3b0d 0a20 2020 207d 0d0a 7d0d  true;..    }..}.
+00001410: 0a0d 0a0d 0a66 756e 6374 696f 6e20 7365  .....function se
+00001420: 7453 7461 7475 7349 6e61 6374 6976 6528  tStatusInactive(
+00001430: 2920 7b0d 0a20 2020 2073 6573 7369 6f6e  ) {..    session
+00001440: 5f62 7574 746f 6e2e 636c 6173 734e 616d  _button.classNam
+00001450: 6520 3d20 2262 746e 2062 746e 2d73 7563  e = "btn btn-suc
+00001460: 6365 7373 2062 746e 2d62 6c6f 636b 2062  cess btn-block b
+00001470: 746e 2d6c 6722 3b0d 0a20 2020 2073 6573  tn-lg";..    ses
+00001480: 7369 6f6e 5f62 7574 746f 6e2e 7465 7874  sion_button.text
+00001490: 436f 6e74 656e 7420 3d20 2253 7461 7274  Content = "Start
+000014a0: 223b 0d0a 0d0a 2020 2020 7374 6174 7573  ";....    status
+000014b0: 5f69 636f 6e2e 636c 6173 734e 616d 6520  _icon.className 
+000014c0: 3d20 2266 6173 2066 612d 6369 7263 6c65  = "fas fa-circle
+000014d0: 2074 6578 742d 6461 6e67 6572 223b 0d0a   text-danger";..
+000014e0: 2020 2020 7374 6174 7573 5f74 6578 742e      status_text.
+000014f0: 6368 696c 644e 6f64 6573 5b32 5d2e 6e6f  childNodes[2].no
+00001500: 6465 5661 6c75 6520 3d20 2220 4e6f 7420  deValue = " Not 
+00001510: 5275 6e6e 696e 6722 3b0d 0a0d 0a20 2020  Running";....   
+00001520: 2070 726f 6772 6573 7342 6172 2e73 7479   progressBar.sty
+00001530: 6c65 2e77 6964 7468 203d 2022 3025 223b  le.width = "0%";
+00001540: 0d0a 2020 2020 7072 6f67 7265 7373 4261  ..    progressBa
+00001550: 722e 696e 6e65 7248 544d 4c20 3d20 2222  r.innerHTML = ""
+00001560: 3b0d 0a0d 0a0d 0a20 2020 202f 2f20 656e  ;......    // en
+00001570: 6162 6c65 2069 6e70 7574 2066 6965 6c64  able input field
+00001580: 730d 0a20 2020 206c 6574 2066 6965 6c64  s..    let field
+00001590: 7320 3d20 666f 726d 2e67 6574 456c 656d  s = form.getElem
+000015a0: 656e 7473 4279 436c 6173 734e 616d 6528  entsByClassName(
+000015b0: 2766 6f72 6d2d 636f 6e74 726f 6c27 293b  'form-control');
+000015c0: 0d0a 2020 2020 666f 7220 286c 6574 2069  ..    for (let i
+000015d0: 203d 2030 3b20 6920 3c20 6669 656c 6473   = 0; i < fields
+000015e0: 2e6c 656e 6774 683b 2069 2b2b 2920 7b0d  .length; i++) {.
+000015f0: 0a20 2020 2020 2020 2066 6965 6c64 735b  .        fields[
+00001600: 695d 2e64 6973 6162 6c65 6420 3d20 6661  i].disabled = fa
+00001610: 6c73 653b 0d0a 2020 2020 7d0d 0a7d 0d0a  lse;..    }..}..
+00001620: 0d0a 0d0a 6675 6e63 7469 6f6e 2073 6574  ....function set
+00001630: 5374 6174 7573 5761 6974 696e 6728 2920  StatusWaiting() 
+00001640: 7b0d 0a20 2020 2073 6573 7369 6f6e 5f62  {..    session_b
+00001650: 7574 746f 6e2e 636c 6173 734e 616d 6520  utton.className 
+00001660: 3d20 2262 746e 2062 746e 2d6c 6967 6874  = "btn btn-light
+00001670: 2062 746e 2d62 6c6f 636b 2062 746e 2d6c   btn-block btn-l
+00001680: 6722 3b0d 0a20 2020 2073 6573 7369 6f6e  g";..    session
+00001690: 5f62 7574 746f 6e2e 7465 7874 436f 6e74  _button.textCont
+000016a0: 656e 7420 3d20 2257 6169 7469 6e67 2e2e  ent = "Waiting..
+000016b0: 2e22 3b0d 0a0d 0a20 2020 2073 7461 7475  .";....    statu
+000016c0: 735f 6963 6f6e 2e63 6c61 7373 4e61 6d65  s_icon.className
+000016d0: 203d 2022 6661 7320 6661 2d63 6972 636c   = "fas fa-circl
+000016e0: 6520 7465 7874 2d77 6172 6e69 6e67 223b  e text-warning";
+000016f0: 0d0a 2020 2020 7374 6174 7573 5f74 6578  ..    status_tex
+00001700: 742e 6368 696c 644e 6f64 6573 5b32 5d2e  t.childNodes[2].
+00001710: 6e6f 6465 5661 6c75 6520 3d20 2220 5761  nodeValue = " Wa
+00001720: 6974 696e 6722 3b0d 0a0d 0a20 2020 202f  iting";....    /
+00001730: 2f20 656e 6162 6c65 2069 6e70 7574 2066  / enable input f
+00001740: 6965 6c64 730d 0a20 2020 206c 6574 2066  ields..    let f
+00001750: 6965 6c64 7320 3d20 666f 726d 2e67 6574  ields = form.get
+00001760: 456c 656d 656e 7473 4279 436c 6173 734e  ElementsByClassN
+00001770: 616d 6528 2766 6f72 6d2d 636f 6e74 726f  ame('form-contro
+00001780: 6c27 293b 0d0a 2020 2020 666f 7220 286c  l');..    for (l
+00001790: 6574 2069 203d 2030 3b20 6920 3c20 6669  et i = 0; i < fi
+000017a0: 656c 6473 2e6c 656e 6774 683b 2069 2b2b  elds.length; i++
+000017b0: 2920 7b0d 0a20 2020 2020 2020 2066 6965  ) {..        fie
+000017c0: 6c64 735b 695d 2e64 6973 6162 6c65 6420  lds[i].disabled 
+000017d0: 3d20 7472 7565 3b0d 0a20 2020 207d 0d0a  = true;..    }..
+000017e0: 7d0d 0a0d 0a2f 2f2f 2043 6861 7274 0d0a  }..../// Chart..
+000017f0: 0d0a 6675 6e63 7469 6f6e 2075 7064 6174  ..function updat
+00001800: 6543 6861 7274 2864 6174 6129 207b 0d0a  eChart(data) {..
+00001810: 2020 2020 6966 2028 6973 4361 6e76 6173      if (isCanvas
+00001820: 426c 616e 6b28 6374 7829 2920 7b0d 0a20  Blank(ctx)) {.. 
+00001830: 2020 2020 2020 2074 7269 616c 7343 6861         trialsCha
+00001840: 7274 203d 2063 7265 6174 6543 6861 7274  rt = createChart
+00001850: 2864 6174 6129 3b0d 0a20 2020 207d 0d0a  (data);..    }..
+00001860: 2020 2020 656c 7365 207b 0d0a 2020 2020      else {..    
+00001870: 2020 2020 7472 6961 6c73 4368 6172 742e      trialsChart.
+00001880: 6461 7461 2e64 6174 6173 6574 732e 666f  data.datasets.fo
+00001890: 7245 6163 6828 2864 6174 6173 6574 2920  rEach((dataset) 
+000018a0: 3d3e 207b 0d0a 2020 2020 2020 2020 2020  => {..          
+000018b0: 2020 6461 7461 7365 742e 6461 7461 203d    dataset.data =
+000018c0: 2064 6174 613b 0d0a 2020 2020 2020 2020   data;..        
+000018d0: 7d29 3b0d 0a20 2020 2020 2020 2074 7269  });..        tri
+000018e0: 616c 7343 6861 7274 2e75 7064 6174 6528  alsChart.update(
+000018f0: 293b 0d0a 2020 2020 7d0d 0a7d 0d0a 0d0a  );..    }..}....
+00001900: 6675 6e63 7469 6f6e 2063 7265 6174 6543  function createC
+00001910: 6861 7274 2864 6174 6129 207b 0d0a 2020  hart(data) {..  
+00001920: 2020 6c65 7420 6e65 7743 6861 7274 203d    let newChart =
+00001930: 206e 6577 2043 6861 7274 2863 7478 2c20   new Chart(ctx, 
+00001940: 7b0d 0a20 2020 2020 2020 2074 7970 653a  {..        type:
+00001950: 2027 646f 7567 686e 7574 272c 0d0a 2020   'doughnut',..  
+00001960: 2020 2020 2020 6461 7461 3a20 7b0d 0a20        data: {.. 
+00001970: 2020 2020 2020 2020 2020 206c 6162 656c             label
+00001980: 733a 205b 2743 6f72 7265 6374 272c 2027  s: ['Correct', '
+00001990: 496e 636f 7272 6563 7427 2c20 2750 7265  Incorrect', 'Pre
+000019a0: 6375 6564 272c 2027 4e6f 2052 6573 706f  cued', 'No Respo
+000019b0: 6e73 6527 5d2c 0d0a 2020 2020 2020 2020  nse'],..        
+000019c0: 2020 2020 6461 7461 7365 7473 3a20 5b7b      datasets: [{
+000019d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000019e0: 2020 6c61 6265 6c3a 2027 2320 6f66 2054    label: '# of T
+000019f0: 7269 616c 7327 2c0d 0a20 2020 2020 2020  rials',..       
+00001a00: 2020 2020 2020 2020 2064 6174 613a 2064           data: d
+00001a10: 6174 612c 0d0a 2020 2020 2020 2020 2020  ata,..          
+00001a20: 2020 2020 2020 626f 7264 6572 5769 6474        borderWidt
+00001a30: 683a 2031 0d0a 2020 2020 2020 2020 2020  h: 1..          
+00001a40: 2020 7d5d 0d0a 2020 2020 2020 2020 7d2c    }]..        },
+00001a50: 0d0a 2020 2020 2020 2020 6f70 7469 6f6e  ..        option
+00001a60: 733a 207b 0d0a 2020 2020 2020 2020 2020  s: {..          
+00001a70: 2020 6465 7669 6365 5069 7865 6c52 6174    devicePixelRat
+00001a80: 696f 3a20 332c 0d0a 2020 2020 2020 2020  io: 3,..        
+00001a90: 2020 2020 7265 7370 6f6e 7369 7665 3a20      responsive: 
+00001aa0: 7472 7565 2c0d 0a20 2020 2020 2020 2020  true,..         
+00001ab0: 2020 2070 6c75 6769 6e73 3a20 7b0d 0a20     plugins: {.. 
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00001ad0: 6567 656e 643a 207b 0d0a 2020 2020 2020  egend: {..      
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001af0: 7370 6c61 793a 2074 7275 652c 0d0a 2020  splay: true,..  
 00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 706f 7369 7469 6f6e 3a20 2772 6967 6874  position: 'right
-00001b20: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00001b30: 2020 2020 2020 2020 6c61 6265 6c73 3a20          labels: 
-00001b40: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00001b50: 2020 2020 2020 2020 2020 2066 6f6e 743a             font:
-00001b60: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001b10: 2020 706f 7369 7469 6f6e 3a20 2772 6967    position: 'rig
+00001b20: 6874 272c 0d0a 2020 2020 2020 2020 2020  ht',..          
+00001b30: 2020 2020 2020 2020 2020 6c61 6265 6c73            labels
+00001b40: 3a20 7b0d 0a20 2020 2020 2020 2020 2020  : {..           
+00001b50: 2020 2020 2020 2020 2020 2020 2066 6f6e               fon
+00001b60: 743a 207b 0d0a 2020 2020 2020 2020 2020  t: {..          
 00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 7369 7a65 3a20 3134 0d0a 2020 2020 2020  size: 14..      
+00001b80: 2020 7369 7a65 3a20 3134 0d0a 2020 2020    size: 14..    
 00001b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ba0: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
-00001bb0: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00001bc0: 2020 2020 2020 2020 2020 2020 7d2c 0d0a              },..
-00001bd0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-00001be0: 2020 2020 2020 207d 2c0d 0a20 2020 207d         },..    }
-00001bf0: 293b 0d0a 2020 2020 7265 7475 726e 206e  );..    return n
-00001c00: 6577 4368 6172 743b 0d0a 7d0d 0a0d 0a2f  ewChart;..}..../
-00001c10: 2f20 7265 7475 726e 7320 7472 7565 2069  / returns true i
-00001c20: 6620 616c 6c20 636f 6c6f 7220 6368 616e  f all color chan
-00001c30: 6e65 6c73 2069 6e20 6561 6368 2070 6978  nels in each pix
-00001c40: 656c 2061 7265 2030 2028 6f72 2022 626c  el are 0 (or "bl
-00001c50: 616e 6b22 290d 0a66 756e 6374 696f 6e20  ank")..function 
-00001c60: 6973 4361 6e76 6173 426c 616e 6b28 6361  isCanvasBlank(ca
-00001c70: 6e76 6173 2920 7b0d 0a20 2020 2072 6574  nvas) {..    ret
-00001c80: 7572 6e20 2163 616e 7661 732e 6765 7443  urn !canvas.getC
-00001c90: 6f6e 7465 7874 2827 3264 2729 0d0a 2020  ontext('2d')..  
-00001ca0: 2020 2020 2e67 6574 496d 6167 6544 6174      .getImageDat
-00001cb0: 6128 302c 2030 2c20 6361 6e76 6173 2e77  a(0, 0, canvas.w
-00001cc0: 6964 7468 2c20 6361 6e76 6173 2e68 6569  idth, canvas.hei
-00001cd0: 6768 7429 2e64 6174 610d 0a20 2020 2020  ght).data..     
-00001ce0: 202e 736f 6d65 2863 6861 6e6e 656c 203d   .some(channel =
-00001cf0: 3e20 6368 616e 6e65 6c20 213d 3d20 3029  > channel !== 0)
-00001d00: 3b0d 0a7d 0d0a 0d0a 2f2f 206e 6577 2043  ;..}....// new C
-00001d10: 6861 7274 2863 7478 2c20 7b0d 0a2f 2f20  hart(ctx, {..// 
-00001d20: 2020 2020 7479 7065 3a20 2764 6f75 6768      type: 'dough
-00001d30: 6e75 7427 2c0d 0a2f 2f20 2020 2020 6461  nut',..//     da
-00001d40: 7461 3a20 7b0d 0a2f 2f20 2020 2020 2020  ta: {..//       
-00001d50: 2020 6461 7461 7365 7473 3a20 5b7b 0d0a    datasets: [{..
-00001d60: 2f2f 2020 2020 2020 2020 2020 2020 206c  //             l
-00001d70: 6162 656c 3a20 2723 206f 6620 5472 6961  abel: '# of Tria
-00001d80: 6c73 272c 0d0a 2f2f 2020 2020 2020 2020  ls',..//        
-00001d90: 2020 2020 2064 6174 613a 205b 7b6f 7574       data: [{out
-00001da0: 636f 6d65 3a20 2263 6f72 7265 6374 227d  come: "correct"}
-00001db0: 2c20 7b6f 7574 636f 6d65 3a20 2269 6e63  , {outcome: "inc
-00001dc0: 6f72 7265 6374 227d 5d2c 0d0a 2f2f 2020  orrect"}],..//  
-00001dd0: 2020 2020 2020 2020 2020 202f 2f20 626f             // bo
-00001de0: 7264 6572 5769 6474 683a 2031 0d0a 2f2f  rderWidth: 1..//
-00001df0: 2020 2020 2020 2020 207d 5d0d 0a2f 2f20           }]..// 
-00001e00: 2020 2020 7d2c 0d0a 2f2f 2020 2020 206f      },..//     o
-00001e10: 7074 696f 6e73 3a20 7b0d 0a2f 2f20 2020  ptions: {..//   
-00001e20: 2020 2020 2020 7061 7273 696e 673a 207b        parsing: {
-00001e30: 0d0a 2f2f 2020 2020 2020 2020 2020 2020  ..//            
-00001e40: 206b 6579 3a20 276f 7574 636f 6d65 270d   key: 'outcome'.
-00001e50: 0a2f 2f20 2020 2020 2020 2020 7d0d 0a2f  .//         }../
-00001e60: 2f20 2020 2020 7d0d 0a2f 2f20 7d29 3b0d  /     }..// });.
-00001e70: 0a0d 0a0d 0a2f 2f2f 2044 796e 616d 6963  ...../// Dynamic
-00001e80: 2066 6f72 6d20 7570 6461 7465 7320 666f   form updates fo
-00001e90: 7220 7072 6f74 6f63 6f6c 2073 656c 6563  r protocol selec
-00001ea0: 7469 6f6e 0d0a 0d0a 2f2f 206c 6f61 6420  tion....// load 
-00001eb0: 7072 6f74 6f63 6f6c 206f 7074 696f 6e73  protocol options
-00001ec0: 206f 6e20 7365 6c65 6374 0d0a 7072 6f74   on select..prot
-00001ed0: 6f63 6f6c 5f73 656c 6563 746f 7220 3d20  ocol_selector = 
-00001ee0: 646f 6375 6d65 6e74 2e67 6574 456c 656d  document.getElem
-00001ef0: 656e 7442 7949 6428 2770 726f 746f 636f  entById('protoco
-00001f00: 6c27 293b 0d0a 0d0a 7072 6f74 6f63 6f6c  l');....protocol
-00001f10: 5f73 656c 6563 746f 722e 6f6e 6368 616e  _selector.onchan
-00001f20: 6765 203d 2066 756e 6374 696f 6e20 2829  ge = function ()
-00001f30: 207b 0d0a 2020 2020 242e 6765 7428 222f   {..    $.get("/
-00001f40: 6170 692f 7072 6f74 6f63 6f6c 2d66 6f72  api/protocol-for
-00001f50: 6d2f 2220 2b20 7072 6f74 6f63 6f6c 5f73  m/" + protocol_s
-00001f60: 656c 6563 746f 722e 7661 6c75 6529 2e64  elector.value).d
-00001f70: 6f6e 6528 6675 6e63 7469 6f6e 2028 6461  one(function (da
-00001f80: 7461 2920 7b0d 0a20 2020 2020 2020 2024  ta) {..        $
-00001f90: 2827 2370 726f 746f 636f 6c2d 6f70 7469  ('#protocol-opti
-00001fa0: 6f6e 7327 292e 6874 6d6c 2864 6174 6129  ons').html(data)
-00001fb0: 3b0d 0a20 2020 207d 290d 0a7d 0d0a 0d0a  ;..    })..}....
-00001fc0: 7072 6f74 6f63 6f6c 5f73 656c 6563 746f  protocol_selecto
-00001fd0: 722e 6f6e 6368 616e 6765 2829 3b0d 0a    r.onchange();..
+00001ba0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
+00001bb0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00001bc0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00001bd0: 0d0a 2020 2020 2020 2020 2020 2020 7d0d  ..            }.
+00001be0: 0a20 2020 2020 2020 207d 2c0d 0a20 2020  .        },..   
+00001bf0: 207d 293b 0d0a 2020 2020 7265 7475 726e   });..    return
+00001c00: 206e 6577 4368 6172 743b 0d0a 7d0d 0a0d   newChart;..}...
+00001c10: 0a2f 2f20 7265 7475 726e 7320 7472 7565  .// returns true
+00001c20: 2069 6620 616c 6c20 636f 6c6f 7220 6368   if all color ch
+00001c30: 616e 6e65 6c73 2069 6e20 6561 6368 2070  annels in each p
+00001c40: 6978 656c 2061 7265 2030 2028 6f72 2022  ixel are 0 (or "
+00001c50: 626c 616e 6b22 290d 0a66 756e 6374 696f  blank")..functio
+00001c60: 6e20 6973 4361 6e76 6173 426c 616e 6b28  n isCanvasBlank(
+00001c70: 6361 6e76 6173 2920 7b0d 0a20 2020 2072  canvas) {..    r
+00001c80: 6574 7572 6e20 2163 616e 7661 732e 6765  eturn !canvas.ge
+00001c90: 7443 6f6e 7465 7874 2827 3264 2729 0d0a  tContext('2d')..
+00001ca0: 2020 2020 2020 2020 2e67 6574 496d 6167          .getImag
+00001cb0: 6544 6174 6128 302c 2030 2c20 6361 6e76  eData(0, 0, canv
+00001cc0: 6173 2e77 6964 7468 2c20 6361 6e76 6173  as.width, canvas
+00001cd0: 2e68 6569 6768 7429 2e64 6174 610d 0a20  .height).data.. 
+00001ce0: 2020 2020 2020 202e 736f 6d65 2863 6861         .some(cha
+00001cf0: 6e6e 656c 203d 3e20 6368 616e 6e65 6c20  nnel => channel 
+00001d00: 213d 3d20 3029 3b0d 0a7d 0d0a 0d0a 2f2f  !== 0);..}....//
+00001d10: 206e 6577 2043 6861 7274 2863 7478 2c20   new Chart(ctx, 
+00001d20: 7b0d 0a2f 2f20 2020 2020 7479 7065 3a20  {..//     type: 
+00001d30: 2764 6f75 6768 6e75 7427 2c0d 0a2f 2f20  'doughnut',..// 
+00001d40: 2020 2020 6461 7461 3a20 7b0d 0a2f 2f20      data: {..// 
+00001d50: 2020 2020 2020 2020 6461 7461 7365 7473          datasets
+00001d60: 3a20 5b7b 0d0a 2f2f 2020 2020 2020 2020  : [{..//        
+00001d70: 2020 2020 206c 6162 656c 3a20 2723 206f       label: '# o
+00001d80: 6620 5472 6961 6c73 272c 0d0a 2f2f 2020  f Trials',..//  
+00001d90: 2020 2020 2020 2020 2020 2064 6174 613a             data:
+00001da0: 205b 7b6f 7574 636f 6d65 3a20 2263 6f72   [{outcome: "cor
+00001db0: 7265 6374 227d 2c20 7b6f 7574 636f 6d65  rect"}, {outcome
+00001dc0: 3a20 2269 6e63 6f72 7265 6374 227d 5d2c  : "incorrect"}],
+00001dd0: 0d0a 2f2f 2020 2020 2020 2020 2020 2020  ..//            
+00001de0: 202f 2f20 626f 7264 6572 5769 6474 683a   // borderWidth:
+00001df0: 2031 0d0a 2f2f 2020 2020 2020 2020 207d   1..//         }
+00001e00: 5d0d 0a2f 2f20 2020 2020 7d2c 0d0a 2f2f  ]..//     },..//
+00001e10: 2020 2020 206f 7074 696f 6e73 3a20 7b0d       options: {.
+00001e20: 0a2f 2f20 2020 2020 2020 2020 7061 7273  .//         pars
+00001e30: 696e 673a 207b 0d0a 2f2f 2020 2020 2020  ing: {..//      
+00001e40: 2020 2020 2020 206b 6579 3a20 276f 7574         key: 'out
+00001e50: 636f 6d65 270d 0a2f 2f20 2020 2020 2020  come'..//       
+00001e60: 2020 7d0d 0a2f 2f20 2020 2020 7d0d 0a2f    }..//     }../
+00001e70: 2f20 7d29 3b0d 0a0d 0a0d 0a2f 2f2f 2044  / });....../// D
+00001e80: 796e 616d 6963 2066 6f72 6d20 7570 6461  ynamic form upda
+00001e90: 7465 7320 666f 7220 7072 6f74 6f63 6f6c  tes for protocol
+00001ea0: 2073 656c 6563 7469 6f6e 0d0a 0d0a 2f2f   selection....//
+00001eb0: 206c 6f61 6420 7072 6f74 6f63 6f6c 206f   load protocol o
+00001ec0: 7074 696f 6e73 206f 6e20 7365 6c65 6374  ptions on select
+00001ed0: 0d0a 7072 6f74 6f63 6f6c 5f73 656c 6563  ..protocol_selec
+00001ee0: 746f 7220 3d20 646f 6375 6d65 6e74 2e67  tor = document.g
+00001ef0: 6574 456c 656d 656e 7442 7949 6428 2770  etElementById('p
+00001f00: 726f 746f 636f 6c27 293b 0d0a 0d0a 7072  rotocol');....pr
+00001f10: 6f74 6f63 6f6c 5f73 656c 6563 746f 722e  otocol_selector.
+00001f20: 6f6e 6368 616e 6765 203d 2066 756e 6374  onchange = funct
+00001f30: 696f 6e20 2829 207b 0d0a 2020 2020 242e  ion () {..    $.
+00001f40: 6765 7428 222f 6170 692f 7072 6f74 6f63  get("/api/protoc
+00001f50: 6f6c 2d66 6f72 6d2f 2220 2b20 7072 6f74  ol-form/" + prot
+00001f60: 6f63 6f6c 5f73 656c 6563 746f 722e 7661  ocol_selector.va
+00001f70: 6c75 6529 2e64 6f6e 6528 6675 6e63 7469  lue).done(functi
+00001f80: 6f6e 2028 6461 7461 2920 7b0d 0a20 2020  on (data) {..   
+00001f90: 2020 2020 2024 2827 2370 726f 746f 636f       $('#protoco
+00001fa0: 6c2d 6f70 7469 6f6e 7327 292e 6874 6d6c  l-options').html
+00001fb0: 2864 6174 6129 3b0d 0a20 2020 207d 290d  (data);..    }).
+00001fc0: 0a7d 0d0a 0d0a 7072 6f74 6f63 6f6c 5f73  .}....protocol_s
+00001fd0: 656c 6563 746f 722e 6f6e 6368 616e 6765  elector.onchange
+00001fe0: 2829 3b0d 0a                             ();..
```

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/base.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,117 +2,122 @@
   ~ This file is part of visiomode.
   ~ Copyright (c) 2020 Constantinos Eleftheriou <Constantinos.Eleftheriou@ed.ac.uk>
   ~ Distributed under the terms of the MIT Licence.
   -->
 
 <!DOCTYPE html>
 <html lang="en">
+
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
     <title>{% block title %}{% endblock %} - Visiomode</title>
     <link rel="stylesheet" href="static/bootstrap/css/bootstrap.min.css">
     <link rel="stylesheet"
-          href="https://fonts.googleapis.com/css?family=Nunito:200,200i,300,300i,400,400i,600,600i,700,700i,800,800i,900,900i">
+        href="https://fonts.googleapis.com/css?family=Nunito:200,200i,300,300i,400,400i,600,600i,700,700i,800,800i,900,900i">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Advent+Pro">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Rajdhani:300,400,500,600,700">
     <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Roboto+Condensed">
     <link rel="stylesheet" href="static/fonts/fontawesome-all.min.css">
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.5.2/animate.min.css">
     <link rel="stylesheet" href="static/css/styles.min.css">
     <link rel="shortcut icon" href="static/favicon.ico">
 </head>
 
 <body id="page-top">
-<div id="wrapper">
-    {% set navigation_bar = [
+    <div id="wrapper">
+        {% set navigation_bar = [
         ('/', 'index', 'Dashboard', 'fa-tachometer-alt'),
         ('/history', 'history', 'History', 'fa-history'),
         ('/settings', 'settings', 'Settings', 'fa-cog'),
-        ('/help', 'help', 'Help', 'fa-life-ring'),
+        ('https://visiomode.readthedocs.io/en/latest/', 'help', 'Help', 'fa-life-ring'),
         ('/about', 'about', 'About', 'fa-info-circle')
-    ] -%}
-    {% set active_page = active_page|default('index') -%}
-    <nav class="navbar navbar-dark align-items-start sidebar sidebar-dark accordion bg-gradient-primary p-0">
-        <div class="container-fluid d-flex flex-column p-0">
-            {# TODO - Align icon with menu elements, bring text closer to image #}
-            <a class="navbar-brand d-flex justify-content-center align-items-center sidebar-brand m-0" href="#">
-                <div class="sidebar-brand-icon"><img src="/static/img/visiomode_logo_icon.png"
-                                                     class="img-fluid" alt="VS"></div>
-                <div class="sidebar-brand-text mx-sm-2"><span
-                        style="font-family: 'Advent Pro', sans-serif;font-size: 22px;">Visiomode</span></div>
-            </a>
-            <hr class="sidebar-divider my-0">
-            <ul class="nav navbar-nav text-light" id="accordionSidebar">
-                <li class="nav-item" role="presentation">
-                    {% for href, id, caption, icon in navigation_bar %}
-                        <a class="nav-link text-left {% if id == active_page %}active{% endif %}"
-                           href="{{ href|e }}">
+        ] -%}
+        {% set active_page = active_page|default('index') -%}
+        <nav class="navbar navbar-dark align-items-start sidebar sidebar-dark accordion bg-gradient-primary p-0">
+            <div class="container-fluid d-flex flex-column p-0">
+                {# TODO - Align icon with menu elements, bring text closer to image #}
+                <a class="navbar-brand d-flex justify-content-center align-items-center sidebar-brand m-0" href="#">
+                    <div class="sidebar-brand-icon"><img src="/static/img/visiomode_logo_icon.png" class="img-fluid"
+                            alt="VS"></div>
+                    <div class="sidebar-brand-text mx-sm-2"><span
+                            style="font-family: 'Advent Pro', sans-serif;font-size: 22px;">Visiomode</span></div>
+                </a>
+                <hr class="sidebar-divider my-0">
+                <ul class="nav navbar-nav text-light" id="accordionSidebar">
+                    <li class="nav-item" role="presentation">
+                        {% for href, id, caption, icon in navigation_bar %}
+                        <a class="nav-link text-left {% if id == active_page %}active{% endif %}" href="{{ href|e }}">
                             <i class="fas {{ icon|e }} fa-fw" href="{{ href|e }}"></i>
                             <span class="d-none d-md-inline">{{ caption|e }}</span></a>
-                    {% endfor %}
-                </li>
-            </ul>
-            <div class="text-center d-none d-md-inline">
-                <button class="btn rounded-circle border-0" id="sidebarToggle" type="button"></button>
+                        {% endfor %}
+                    </li>
+                </ul>
+                <div class="text-center d-none d-md-inline">
+                    <button class="btn rounded-circle border-0" id="sidebarToggle" type="button"></button>
+                </div>
             </div>
-        </div>
-    </nav>
-    <div class="d-flex flex-column" id="content-wrapper">
-        <div id="content">
-            <nav class="navbar navbar-light navbar-expand bg-white shadow d-xl-flex align-items-xl-center mb-4 topbar static-top">
-                <div class="container-fluid">
-                    <button class="btn btn-link d-md-none rounded-circle mr-3" id="sidebarToggleTop" type="button"><i
-                            class="fas fa-bars"></i></button>
-                    <div class="row d-xl-flex justify-content-xl-center ml-auto">
-                        <div class="col d-xl-flex align-items-xl-center">
-                            <ul class="nav navbar-nav">
-                                <li class="nav-item" role="presentation"></li>
-                                <li id="hostname" class="nav-item" role="presentation"><a
-                                        class="nav-link active text-truncate text-muted d-flex"
-                                        style="max-height: 30px;"></a></li>
-                                <li class="nav-item" role="presentation"></li>
-                                <li class="nav-item" role="presentation"></li>
-                            </ul>
-                        </div>
-                        <div class="col d-xl-flex">
-                            <form class="form-inline d-none d-sm-inline-block mr-auto ml-md-3 my-2 my-md-0 mw-100 navbar-search"
-                                  style="padding-bottom: 0px;">
-                                <div class="input-group"><input class="bg-light form-control border-0 small" type="text"
-                                                                placeholder="Search documentation for ...">
-                                    <div class="input-group-append">
-                                        <button class="btn btn-primary py-0" type="button"><i class="fas fa-search"></i>
-                                        </button>
+        </nav>
+        <div class="d-flex flex-column" id="content-wrapper">
+            <div id="content">
+                <nav
+                    class="navbar navbar-light navbar-expand bg-white shadow d-xl-flex align-items-xl-center mb-4 topbar static-top">
+                    <div class="container-fluid">
+                        <button class="btn btn-link d-md-none rounded-circle mr-3" id="sidebarToggleTop"
+                            type="button"><i class="fas fa-bars"></i></button>
+                        <div class="row d-xl-flex justify-content-xl-center ml-auto">
+                            <div class="col d-xl-flex align-items-xl-center">
+                                <ul class="nav navbar-nav">
+                                    <li class="nav-item" role="presentation"></li>
+                                    <li id="hostname" class="nav-item" role="presentation"><a
+                                            class="nav-link active text-truncate text-muted d-flex"
+                                            style="max-height: 30px;"></a></li>
+                                    <li class="nav-item" role="presentation"></li>
+                                    <li class="nav-item" role="presentation"></li>
+                                </ul>
+                            </div>
+                            <div class="col d-xl-flex">
+                                <form
+                                    class="form-inline d-none d-sm-inline-block mr-auto ml-md-3 my-2 my-md-0 mw-100 navbar-search"
+                                    style="padding-bottom: 0px;">
+                                    <div class="input-group"><input class="bg-light form-control border-0 small"
+                                            type="text" placeholder="Search documentation for ...">
+                                        <div class="input-group-append">
+                                            <button class="btn btn-primary py-0" type="button"><i
+                                                    class="fas fa-search"></i>
+                                            </button>
+                                        </div>
                                     </div>
-                                </div>
-                            </form>
+                                </form>
+                            </div>
                         </div>
                     </div>
+                </nav>
+                <div class="container-fluid">
+                    {% block content %}{% endblock %}
                 </div>
-            </nav>
-            <div class="container-fluid">
-                {% block content %}{% endblock %}
             </div>
+            <footer class="bg-white sticky-footer">
+                <div class="container my-auto">
+                    <div class="text-center my-auto copyright"><span>Copyright © Constantinos Eleftheriou 2023</span>
+                    </div>
+                </div>
+            </footer>
         </div>
-        <footer class="bg-white sticky-footer">
-            <div class="container my-auto">
-                <div class="text-center my-auto copyright"><span>Copyright © Constantinos Eleftheriou 2023</span></div>
-            </div>
-        </footer>
+        <a class="border rounded d-inline scroll-to-top" href="#page-top"><i class="fas fa-angle-up"></i></a>
     </div>
-    <a class="border rounded d-inline scroll-to-top" href="#page-top"><i class="fas fa-angle-up"></i></a>
-</div>
-<script src="static/js/jquery.min.js"></script>
-<script src="static/bootstrap/js/bootstrap.min.js"></script>
-<script src="static/js/chart.min.js"></script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-easing/1.4.1/jquery.easing.js"></script>
-<script src="static/js/script.min.js"></script>
-<!-- <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/chart.js"></script> -->
-<script>
-    /// Get hostname
-    $.get("/api/hostname").done(function (data) {
-        $('#hostname').html(data);
-    })
-</script>
-{% block scripts %}{% endblock %}
+    <script src="static/js/jquery.min.js"></script>
+    <script src="static/bootstrap/js/bootstrap.min.js"></script>
+    <script src="static/js/chart.min.js"></script>
+    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery-easing/1.4.1/jquery.easing.js"></script>
+    <script src="static/js/script.min.js"></script>
+    <!-- <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/chart.js"></script> -->
+    <script>
+        /// Get hostname
+        $.get("/api/hostname").done(function (data) {
+            $('#hostname').html(data);
+        })
+    </script>
+    {% block scripts %}{% endblock %}
 </body>
+
 </html>
```

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/history.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/history.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/index.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/index.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/gonogo.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/gonogo.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/tafc.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/tafc.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/target_only.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/target_only.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/protocols/task.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/protocols/task.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/grating.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/grating.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/src/visiomode/webpanel/templates/stimuli/moving_grating.html` & `visiomode-0.5.2/src/visiomode/webpanel/templates/stimuli/moving_grating.html`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/tests/test_launch.py` & `visiomode-0.5.2/tests/test_launch.py`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/.gitignore` & `visiomode-0.5.2/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -135,7 +135,11 @@
 *.sublime-*
 .vscode/
 .nova/
 
 /devices/
 visiomode_data/
 /docs/_build/
+
+.hatch
+
+.visiomode.json
```

### Comparing `visiomode-0.5.1/LICENSE` & `visiomode-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/README.md` & `visiomode-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `visiomode-0.5.1/pyproject.toml` & `visiomode-0.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -5,62 +5,61 @@
 [tool.hatch]
 
 [project]
 name = "visiomode"
 description = "An open-source platform for touchscreen-based visuomotor tasks in rodents."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 authors = [
   { name = "Constantinos Eleftheriou", email = "Constantinos.Eleftheriou@ed.ac.uk" },
 ]
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
-    "Framework :: Flask",
-    "Topic :: Scientific/Engineering",
-    "Topic :: Scientific/Engineering :: Medical Science Apps.",
-    "Topic :: Software Development :: Libraries :: pygame",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: POSIX :: Linux",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
+  "Development Status :: 2 - Pre-Alpha",
+  "Framework :: Flask",
+  "Topic :: Scientific/Engineering",
+  "Topic :: Scientific/Engineering :: Medical Science Apps.",
+  "Topic :: Software Development :: Libraries :: pygame",
+  "Intended Audience :: Science/Research",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: POSIX :: Linux",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
 ]
 keywords = ["touchscreen", "rodent", "behaviour", "neuroscience"]
 dependencies = [
-    "Flask~=2.0.3",
-    "PyYAML~=6.0",
-    "pyserial~=3.5",
-    "numpy>=1.22",
-    "pygame==2.0.1",
-    "pynwb>=2.2.0"
+  "Flask~=2.0.3",
+  "PyYAML~=6.0",
+  "pyserial~=3.5",
+  "numpy>=1.22",
+  "pygame==2.0.1",
+  "pynwb>=2.2.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Website = "https://www.visiomode.org"
 Documentation = "https://visiomode.readthedocs.io/en/latest/"
 Issues = "https://github.com/DuguidLab/visiomode/issues"
 Source = "https://github.com/DuguidLab/visiomode"
 
 [project.scripts]
 visiomode = "visiomode:run"
 
 [tool.hatch.build]
-artifacts = [
-  "*.png",
-]
+artifacts = ["*.png"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/visiomode"]
 
 [tool.hatch.build.targets.sdist]
-exclude = [
-  "/.github",
-  "/docs",
-]
+exclude = ["/.github", "/docs"]
 
 [tool.hatch.version]
 path = "src/visiomode/__about__.py"
 
 [tool.hatch.envs.default]
 python = "3.9"
+
+[tool.hatch.envs.develop]
+python = "3.9"
+dependencies = ["black", "pylint"]
```

### Comparing `visiomode-0.5.1/PKG-INFO` & `visiomode-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visiomode
-Version: 0.5.1
+Version: 0.5.2
 Summary: An open-source platform for touchscreen-based visuomotor tasks in rodents.
 Project-URL: Website, https://www.visiomode.org
 Project-URL: Documentation, https://visiomode.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/DuguidLab/visiomode/issues
 Project-URL: Source, https://github.com/DuguidLab/visiomode
 Author-email: Constantinos Eleftheriou <Constantinos.Eleftheriou@ed.ac.uk>
 License: MIT License
```

