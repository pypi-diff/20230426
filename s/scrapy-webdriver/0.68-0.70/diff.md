# Comparing `tmp/scrapy_webdriver-0.68.tar.gz` & `tmp/scrapy_webdriver-0.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapy_webdriver-0.68.tar", last modified: Mon Apr 24 18:59:29 2023, max compression
+gzip compressed data, was "dist/scrapy_webdriver-0.70.tar", last modified: Tue Apr 25 20:38:51 2023, max compression
```

## Comparing `scrapy_webdriver-0.68.tar` & `scrapy_webdriver-0.70.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      332 2021-06-12 13:54:15.000000 scrapy_webdriver-0.68/.gitignore
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1075 2021-06-11 16:03:00.000000 scrapy_webdriver-0.68/LICENSE
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      222 2021-06-14 09:30:07.000000 scrapy_webdriver-0.68/MANIFEST.in
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      872 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/PKG-INFO
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      361 2021-06-13 19:06:57.000000 scrapy_webdriver-0.68/README.md
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5503 2021-06-12 07:48:08.000000 scrapy_webdriver-0.68/proxies.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       84 2022-11-03 14:06:08.000000 scrapy_webdriver-0.68/requirements.txt
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       72 2021-07-09 13:43:05.000000 scrapy_webdriver-0.68/scrapy_webdriver/__init__.py
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-14 08:32:14.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/__init__.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   620448 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     8574 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.manifest
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     3110 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.sig
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     8895 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/manifest.mf
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4357 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.rsa
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      144 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.sf
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    15425 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/messages.json
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    21705 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/messages.json
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    24489 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/content_scripts.css
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      842 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/cssreset-min.css
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1912 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/default.css
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    16316 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/128.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      429 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16-image.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      400 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16-input.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      758 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/32.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     3819 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/48.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      790 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-16.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2147 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-32.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      815 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/anti.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1303 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/coss-input.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16-image.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      358 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16-input.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      696 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1979 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-32.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1116 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-coss-input.png
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      231 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/cross-red.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2147 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-active.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1979 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-disabled.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      370 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/flag_blue.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1732 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/icon-lock.png
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      605 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30.svg
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      596 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30_active.svg
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2093 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/manifest.json
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    18562 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/options.html
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/recaptcha_precache_debug.html
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    97016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/chord.wav
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    80856 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/ding.wav
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    36482 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/newemail.wav
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   119384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/notify.wav
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4168 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/start.wav
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   171100 2021-06-14 08:19:21.000000 scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/tada.wav
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/extension/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 20:46:22.000000 scrapy_webdriver-0.68/scrapy_webdriver/extension/__init__.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      527 2021-07-09 13:42:34.000000 scrapy_webdriver-0.68/scrapy_webdriver/extension/background.js
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      409 2021-08-08 13:49:45.000000 scrapy_webdriver-0.68/scrapy_webdriver/extension/manifest.json
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1967 2021-06-14 09:12:08.000000 scrapy_webdriver-0.68/scrapy_webdriver/extension_creator.py
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/extensions/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 20:26:22.000000 scrapy_webdriver-0.68/scrapy_webdriver/extensions/__init__.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)  5630432 2021-06-11 21:46:33.000000 scrapy_webdriver-0.68/scrapy_webdriver/extensions/adblocker_ultimate-3.7.10-an+fx.xpi
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   619703 2021-06-14 09:17:31.000000 scrapy_webdriver-0.68/scrapy_webdriver/extensions/anticaptcha-plugin.xpi
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1162 2021-07-09 13:42:34.000000 scrapy_webdriver-0.68/scrapy_webdriver/extensions/extension.xpi
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 09:19:48.000000 scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/__init__.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5050 2021-06-19 19:43:38.000000 scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/drivers.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1478 2022-05-05 21:38:17.000000 scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/http.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2223 2021-06-19 20:28:14.000000 scrapy_webdriver-0.68/scrapy_webdriver/middlewares.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5336 2022-11-03 14:07:40.000000 scrapy_webdriver-0.68/scrapy_webdriver/scrapy_webdriver.py
-drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      872 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/PKG-INFO
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5075 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/SOURCES.txt
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        1 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/dependency_links.txt
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       66 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/requires.txt
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       17 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/scrapy_webdriver.egg-info/top_level.txt
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       38 2023-04-24 18:59:29.000000 scrapy_webdriver-0.68/setup.cfg
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      832 2023-04-24 18:51:56.000000 scrapy_webdriver-0.68/setup.py
--rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4592 2021-06-12 07:29:26.000000 scrapy_webdriver-0.68/webshare.txt
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      332 2021-06-12 13:54:15.000000 scrapy_webdriver-0.70/.gitignore
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1075 2021-06-11 16:03:00.000000 scrapy_webdriver-0.70/LICENSE
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      222 2021-06-14 09:30:07.000000 scrapy_webdriver-0.70/MANIFEST.in
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      872 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/PKG-INFO
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      361 2021-06-13 19:06:57.000000 scrapy_webdriver-0.70/README.md
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5503 2021-06-12 07:48:08.000000 scrapy_webdriver-0.70/proxies.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       65 2023-04-25 19:49:53.000000 scrapy_webdriver-0.70/requirements.txt
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       72 2021-07-09 13:43:05.000000 scrapy_webdriver-0.70/scrapy_webdriver/__init__.py
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-14 08:32:14.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/__init__.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   620448 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     8574 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.manifest
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     3110 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.sig
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     8895 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/manifest.mf
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4357 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.rsa
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      144 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.sf
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    15425 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/messages.json
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    21705 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/messages.json
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    24489 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/content_scripts.css
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      842 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/cssreset-min.css
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1912 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/default.css
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    16316 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/128.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      429 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16-image.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      400 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16-input.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      758 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/32.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     3819 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/48.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      790 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-16.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2147 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-32.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      815 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/anti.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1303 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/coss-input.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16-image.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      358 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16-input.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      696 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1979 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-32.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1116 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-coss-input.png
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      231 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/cross-red.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2147 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-active.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1979 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-disabled.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      370 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/flag_blue.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1732 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/icon-lock.png
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      605 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30.svg
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      596 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30_active.svg
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2093 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/manifest.json
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    18562 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/options.html
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/recaptcha_precache_debug.html
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    97016 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/chord.wav
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    80856 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/ding.wav
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)    36482 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/newemail.wav
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   119384 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/notify.wav
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4168 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/start.wav
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   171100 2021-06-14 08:19:21.000000 scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/tada.wav
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/extension/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 20:46:22.000000 scrapy_webdriver-0.70/scrapy_webdriver/extension/__init__.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      527 2021-07-09 13:42:34.000000 scrapy_webdriver-0.70/scrapy_webdriver/extension/background.js
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      409 2021-08-08 13:49:45.000000 scrapy_webdriver-0.70/scrapy_webdriver/extension/manifest.json
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1967 2021-06-14 09:12:08.000000 scrapy_webdriver-0.70/scrapy_webdriver/extension_creator.py
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/extensions/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 20:26:22.000000 scrapy_webdriver-0.70/scrapy_webdriver/extensions/__init__.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)  5630432 2021-06-11 21:46:33.000000 scrapy_webdriver-0.70/scrapy_webdriver/extensions/adblocker_ultimate-3.7.10-an+fx.xpi
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)   619703 2021-06-14 09:17:31.000000 scrapy_webdriver-0.70/scrapy_webdriver/extensions/anticaptcha-plugin.xpi
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1162 2021-07-09 13:42:34.000000 scrapy_webdriver-0.70/scrapy_webdriver/extensions/extension.xpi
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        0 2021-06-13 09:19:48.000000 scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/__init__.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5506 2023-04-25 20:37:24.000000 scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/drivers.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     1478 2022-05-05 21:38:17.000000 scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/http.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     2223 2021-06-19 20:28:14.000000 scrapy_webdriver-0.70/scrapy_webdriver/middlewares.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5384 2023-04-25 20:37:24.000000 scrapy_webdriver-0.70/scrapy_webdriver/scrapy_webdriver.py
+drwxrwxr-x   0 aleksey   (1000) aleksey   (1000)        0 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      872 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/PKG-INFO
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     5075 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)        1 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       66 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/requires.txt
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       17 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/scrapy_webdriver.egg-info/top_level.txt
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)       38 2023-04-25 20:38:51.000000 scrapy_webdriver-0.70/setup.cfg
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)      832 2023-04-25 20:37:32.000000 scrapy_webdriver-0.70/setup.py
+-rw-rw-r--   0 aleksey   (1000) aleksey   (1000)     4592 2021-06-12 07:29:26.000000 scrapy_webdriver-0.70/webshare.txt
```

### Comparing `scrapy_webdriver-0.68/LICENSE` & `scrapy_webdriver-0.70/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/PKG-INFO` & `scrapy_webdriver-0.70/scrapy_webdriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapy_webdriver
-Version: 0.68
+Name: scrapy-webdriver
+Version: 0.70
 Summary: Class based on selenium webdriver.Firefox with methods  for scraping.
 Home-page: https://github.com/KvyatkovskyAleksey/ScrapeWebdriver
 Author: Aleksey Kvyatkovsky
 Author-email: kvyatkovsky@mail.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scrapy_webdriver-0.68/proxies.py` & `scrapy_webdriver-0.70/proxies.py`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.manifest` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.manifest`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.sig` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/cose.sig`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/manifest.mf` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/manifest.mf`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.rsa` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/META-INF/mozilla.rsa`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/messages.json` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/en/messages.json`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/messages.json` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/_locales/ru/messages.json`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/content_scripts.css` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/content_scripts.css`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/cssreset-min.css` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/cssreset-min.css`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/default.css` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/css/default.css`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/128.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/128.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/16.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/32.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/32.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/48.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/48.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-16.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-16.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-32.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/active-32.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/anti.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/anti.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/coss-input.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/coss-input.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-16.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-32.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-32.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-coss-input.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/anticaptcha-logo/disabled-coss-input.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-active.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-active.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-disabled.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32-disabled.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/coss/icon-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/icon-lock.png` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/icon-lock.png`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30.svg` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30.svg`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30_active.svg` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/img/reload_30_active.svg`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/manifest.json` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/manifest.json`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/options.html` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/options.html`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/recaptcha_precache_debug.html` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/recaptcha_precache_debug.html`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/chord.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/chord.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/ding.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/ding.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/newemail.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/newemail.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/notify.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/notify.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/start.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/start.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/tada.wav` & `scrapy_webdriver-0.70/scrapy_webdriver/anticaptcha_plugin/anticaptcha-plugin_v0.56.xpi_FILES/sounds/tada.wav`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/extension/background.js` & `scrapy_webdriver-0.70/scrapy_webdriver/extension/background.js`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/extension_creator.py` & `scrapy_webdriver-0.70/scrapy_webdriver/extension_creator.py`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/extensions/adblocker_ultimate-3.7.10-an+fx.xpi` & `scrapy_webdriver-0.70/scrapy_webdriver/extensions/adblocker_ultimate-3.7.10-an+fx.xpi`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/extensions/anticaptcha-plugin.xpi` & `scrapy_webdriver-0.70/scrapy_webdriver/extensions/anticaptcha-plugin.xpi`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/extensions/extension.xpi` & `scrapy_webdriver-0.70/scrapy_webdriver/extensions/extension.xpi`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/drivers.py` & `scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/drivers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from webdriver_manager.firefox import GeckoDriverManager
+
 from ..scrapy_webdriver import ScrapyWebdriver
 
 from scrapy.utils.python import to_bytes
 from scrapy.http import HtmlResponse
 
 from twisted.internet.threads import deferToThreadPool
 from twisted.internet import reactor
@@ -17,19 +19,23 @@
 
 class Driver:
     def __init__(self,
                  pool: 'DriverPool' = None,
                  change_proxy_on_each_request: bool = True,
                  proxies: tuple = (),
                  install_adblock: bool = True,
-                 anticaptcha_api_key: str = None):
+                 anticaptcha_api_key: str = None,
+                 executable_path: str = None
+                 ):
         self.web_driver = ScrapyWebdriver(change_proxies_on_each_request=change_proxy_on_each_request,
                                           proxies=proxies,
                                           install_adblock=install_adblock,
-                                          anticaptcha_api_key=anticaptcha_api_key)
+                                          anticaptcha_api_key=anticaptcha_api_key,
+                                          executable_path=executable_path
+                                          )
         self._blocked = False
         self.pool = pool
 
     @property
     def blocked(self):
         return self._blocked
 
@@ -50,21 +56,24 @@
         self.size = size
         self.drivers = []
         self._waiting = []
         self.chang_proxy_on_each_request = change_proxy_on_each_request
         self.proxies = proxies
         self.install_adblock = install_adblock
         self.anticaptcha_api_key = anticaptcha_api_key
+        self.executable_path = GeckoDriverManager().install()
 
     def append_driver(self):
         driver = Driver(pool=self,
                         change_proxy_on_each_request=self.chang_proxy_on_each_request,
                         proxies=self.proxies,
                         install_adblock=self.install_adblock,
-                        anticaptcha_api_key=self.anticaptcha_api_key)
+                        anticaptcha_api_key=self.anticaptcha_api_key,
+                        executable_path=self.executable_path
+                        )
         self.drivers.append(driver)
         return driver
 
     def close(self):
         for driver in self.drivers:
             driver.web_driver.quit()
 
@@ -93,31 +102,31 @@
             logger.info("Free driver not found. Waiting for ....")
             self._waiting.append(free_driver)
             logger.info('Append deferred tor waiting, len = %s', len(self._waiting))
         return free_driver
 
     @staticmethod
     def _get_url(driver: Driver, request: SeleniumRequest) -> HtmlResponse:
-        response = None
         try:
             web_driver = driver.web_driver
             if request.driver is None:
                 web_driver.get(request.url)
             if request.driver_func is not None:
                 func_res = request.driver_func(web_driver,
                                                *request.driver_func_args,
                                                **request.driver_func_kwargs)
                 if func_res:
                     request.meta['driver_func_res'] = func_res
             body = to_bytes(web_driver.page_source)  # body must be of type bytes
             response = HtmlResponse(web_driver.current_url, body=body, encoding='utf-8', request=request)
             response.meta['driver'] = driver
         except Exception as e:
-            logger.error(f'Error was happened in webdriver: {e}')
-            driver.unblock()
+            logger.exception(e)
+            response = HtmlResponse(request.url, body=str(e), encoding='utf-8', request=request, status=500)
+            response.meta['driver'] = driver
         return response
 
     @staticmethod
     def _response(driver: Driver, request: SeleniumRequest) -> Deferred:
         driver.block()
         deferred = deferToThreadPool(reactor, reactor.getThreadPool(), DriverPool._get_url, driver, request)
         return deferred
```

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/middleware_utils/http.py` & `scrapy_webdriver-0.70/scrapy_webdriver/middleware_utils/http.py`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/middlewares.py` & `scrapy_webdriver-0.70/scrapy_webdriver/middlewares.py`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver/scrapy_webdriver.py` & `scrapy_webdriver-0.70/scrapy_webdriver/scrapy_webdriver.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,16 @@
                  anticaptcha_api_key=None,
                  *args, **kwargs):
         self.path = os.path.dirname(os.path.realpath(__file__))
         self.change_proxies_on_each_request = change_proxies_on_each_request
         self.proxies = proxies
         if self.proxies:
             self.proxies = cycle(self.proxies)
-        kwargs['executable_path'] = GeckoDriverManager().install()
+        if 'executable_path' not in kwargs:
+            kwargs['executable_path'] = GeckoDriverManager().install()
         super().__init__(*args, **kwargs)
         self.execute(Command.GET, {'url': "about:config"})
         # need for install extensions
         self.set_preference('xpinstall.signatures.required', 'false')
         if install_adblock:
             self.install_addon(f'{self.path}/extensions/adblocker_ultimate-3.7.10-an+fx.xpi')
         if anticaptcha_api_key:
```

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver.egg-info/PKG-INFO` & `scrapy_webdriver-0.70/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: scrapy-webdriver
-Version: 0.68
+Name: scrapy_webdriver
+Version: 0.70
 Summary: Class based on selenium webdriver.Firefox with methods  for scraping.
 Home-page: https://github.com/KvyatkovskyAleksey/ScrapeWebdriver
 Author: Aleksey Kvyatkovsky
 Author-email: kvyatkovsky@mail.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scrapy_webdriver-0.68/scrapy_webdriver.egg-info/SOURCES.txt` & `scrapy_webdriver-0.70/scrapy_webdriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrapy_webdriver-0.68/setup.py` & `scrapy_webdriver-0.70/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="scrapy_webdriver",
-	version="0.68",
+	version="0.70",
 	author="Aleksey Kvyatkovsky",
 	author_email="kvyatkovsky@mail.ru",
 	description="Class based on selenium webdriver.Firefox with methods  for scraping.",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/KvyatkovskyAleksey/ScrapeWebdriver",
 	packages=setuptools.find_packages(),
```

### Comparing `scrapy_webdriver-0.68/webshare.txt` & `scrapy_webdriver-0.70/webshare.txt`

 * *Files identical despite different names*

