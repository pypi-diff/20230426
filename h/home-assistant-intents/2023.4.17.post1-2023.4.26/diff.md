# Comparing `tmp/home-assistant-intents-2023.4.17.post1.tar.gz` & `tmp/home-assistant-intents-2023.4.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.4.17.post1.tar", last modified: Mon Apr 17 16:27:24 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.4.26.tar", last modified: Wed Apr 26 14:50:58 2023, max compression
```

## Comparing `home-assistant-intents-2023.4.17.post1.tar` & `home-assistant-intents-2023.4.26.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.738942 home-assistant-intents-2023.4.17.post1/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.17.post1/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.17.post1/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      909 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.17.post1/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:08:03.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12939 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21003 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    25271 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    68839 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.734942 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-17 16:27:19.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-17 16:27:20.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-17 16:27:21.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-17 16:27:24.730942 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      909 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-17 16:27:24.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      992 2023-04-17 16:27:17.000000 home-assistant-intents-2023.4.17.post1/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-17 16:27:24.738942 home-assistant-intents-2023.4.17.post1/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.26/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.26/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.26/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.4.26/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.769475 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    29471 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-04-26 14:50:44.000000 home-assistant-intents-2023.4.26/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/setup.cfg
```

### Comparing `home-assistant-intents-2023.4.17.post1/LICENSE.md` & `home-assistant-intents-2023.4.26/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/PKG-INFO` & `home-assistant-intents-2023.4.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.4.17.post1
+Version: 2023.4.26
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.4.26/home_assistant_intents/__init__.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ar.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9733340347923681%*

 * *Differences: {"'expansion_rules'": "{'what_is': '(ما هو|ما هي|ماذا يكون|ماذا تكون|كم هي|كم هو)', 'scene': "*

 * *                      "'[ال](مشهد|مشاهد|اعدادات)', 'is_it': '(هل [هي]|هل [هو]|هل هناك)', "*

 * *                      "'how_many': 'كم عدد', 'to': '(على|الى)', 'any': '(أي)', 'lock': "*

 * *                      "'[ال](اقفال|قفل)'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {0: {'response': 'fans_area'}, 1: {'response': 'fan_all'}, "*

 * *              "insert: [(8, OrderedDict([('sentences', ['<open> <name> [<in> <area>]']), "*

 * *  […]*

```diff
@@ -1,40 +1,93 @@
 {
     "expansion_rules": {
         "all": "(\u0643\u0644|\u062c\u0645\u064a\u0639)",
+        "any": "(\u0623\u064a)",
         "area": "[\u0627\u0644]{area}",
         "awning": "[\u0627\u0644](\u0645\u0638\u0644\u0629|\u0645\u0638\u0644\u0627\u062a)",
         "brightness": "{brightness}[% | \u0628\u0627\u0644\u0645\u0627\u0626\u0629]",
         "close": "(\u0627\u063a\u0644\u0642|\u0627\u0642\u0641\u0644|\u0627\u062e\u0641\u0636|\u0627\u0646\u0632\u0644|\u0646\u0632\u0644)",
         "color": "[\u0627\u0644](\u0644\u0648\u0646|\u0627\u0644\u0648\u0627\u0646)",
         "colors": "[\u0627\u0644]{color}",
         "curtain": "[\u0627\u0644](\u0633\u062a\u0627\u0626\u0631|\u0633\u062a\u0627\u0631\u0629|\u0633\u062a\u0627\u0631\u0627\u062a)",
         "door": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628)",
         "fan": "[\u0627\u0644](\u0645\u0631\u0648\u062d\u0629|\u0645\u0631\u0627\u0648\u062d|\u0645\u0631\u0648\u062d\u0627\u062a)",
         "garage": "[\u0627\u0644](\u0628\u0627\u0628|\u0627\u0628\u0648\u0627\u0628|\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a) [\u0627\u0644]\u062c\u0631\u0627\u062c",
         "gate": "[\u0627\u0644](\u0628\u0648\u0627\u0628\u0629|\u0628\u0648\u0627\u0628\u0627\u062a)",
+        "how_many": "\u0643\u0645 \u0639\u062f\u062f",
         "in": "(\u0641\u064a|\u062f\u0627\u062e\u0644)",
         "intensity": "[\u0627\u0644](\u062f\u0631\u062c\u0629 [\u0627\u0644]\u0633\u0637\u0648\u0639|[\u0634\u062f\u0629] [\u0627\u0644]\u0633\u0637\u0648\u0639|\u0642\u0648\u0629|\u0634\u062f\u0629)",
+        "is_it": "(\u0647\u0644 [\u0647\u064a]|\u0647\u0644 [\u0647\u0648]|\u0647\u0644 \u0647\u0646\u0627\u0643)",
         "light": "[\u0627\u0644](\u0627\u0636\u0648\u0627\u0621|\u0627\u0636\u0627\u0621\u0629|\u0636\u0648\u0621|\u0645\u0635\u0627\u0628\u064a\u062d|\u0645\u0635\u0628\u0627\u062d|\u0627\u0646\u0648\u0627\u0631|\u0646\u0648\u0631|\u0644\u0645\u0628\u0629|\u0644\u0645\u0628\u0627\u062a|\u0627\u0646\u0648\u0627\u0631)",
+        "lock": "[\u0627\u0644](\u0627\u0642\u0641\u0627\u0644|\u0642\u0641\u0644)",
         "name": "[\u0627\u0644]{name}",
         "open": "(\u0627\u0641\u062a\u062d|\u0627\u0631\u0641\u0639)",
+        "scene": "[\u0627\u0644](\u0645\u0634\u0647\u062f|\u0645\u0634\u0627\u0647\u062f|\u0627\u0639\u062f\u0627\u062f\u0627\u062a)",
         "script": "[\u0627\u0644](\u0628\u0631\u0646\u0627\u0645\u062c|\u0628\u0631\u0627\u0645\u062c|\u0645\u0633\u0627\u0631|\u0645\u0633\u0627\u0631\u0627\u062a|\u0633\u064a\u0646\u0627\u0631\u064a\u0648)",
         "switch": "[\u0627\u0644](\u0645\u0641\u062a\u0627\u062d|\u0645\u0641\u0627\u062a\u064a\u062d)",
         "temp": "(\u0628\u0627\u0631\u062f\u0629|\u062f\u0627\u0641\u0626\u0629|\u0644\u0637\u064a\u0641\u0629|\u062d\u0627\u0631\u0629|\u062f\u0631\u062c\u0629 [\u0627\u0644]\u062d\u0631\u0627\u0631\u0629)",
         "temperature": "{temperature}[\u00b0| \u062f\u0631\u062c\u0629] [{temperature_unit}]",
+        "to": "(\u0639\u0644\u0649|\u0627\u0644\u0649)",
         "turn": "(\u063a\u064a\u0631|\u0627\u0636\u0628\u0637|\u0636\u0628\u0637)",
         "turn_off": "(\u0627\u063a\u0644\u0642|\u0627\u0637\u0641\u0626|\u0637\u0641\u064a)",
         "turn_on": "(\u0627\u0641\u062a\u062d|\u0634\u063a\u0644|\u0627\u0634\u0639\u0644|\u0627\u0634\u063a\u0644|\u0627\u0628\u062f\u0623|\u0634\u0639\u0644|\u0641\u0639\u0644|\u062a\u0641\u0639\u064a\u0644|\u062a\u0634\u063a\u064a\u0644|\u0641\u0639\u0644)",
-        "what_is": "(\u0645\u0627 \u0647\u0648|\u0645\u0627 \u0647\u064a|\u0645\u0627\u0630\u0627 \u064a\u0643\u0648\u0646|\u0645\u0627\u0630\u0627 \u062a\u0643\u0648\u0646|\u0643\u0645 \u0647\u064a|\u0643\u0645 \u0647\u0648|\u0647\u0644 \u0647\u064a|\u0647\u0644 \u0647\u0648)",
+        "what_is": "(\u0645\u0627 \u0647\u0648|\u0645\u0627 \u0647\u064a|\u0645\u0627\u0630\u0627 \u064a\u0643\u0648\u0646|\u0645\u0627\u0630\u0627 \u062a\u0643\u0648\u0646|\u0643\u0645 \u0647\u064a|\u0643\u0645 \u0647\u0648)",
         "window": "[\u0627\u0644](\u0646\u0627\u0641\u0630\u0629|\u0646\u0648\u0627\u0641\u0630|\u0646\u0627\u0641\u0630\u0627\u062a|\u0634\u0628\u0627\u0643|\u0634\u0628\u0627\u0628\u064a\u0643)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "one",
+                    "sentences": [
+                        "<what_is> [\u062d\u0627\u0644\u0629] <name> [<in> <area>]"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover"
+                        ]
+                    },
+                    "response": "one_yesno",
+                    "sentences": [
+                        "<is_it> <name> [<in> <area>] {on_off_states:state}"
+                    ]
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "<is_it> <any> {on_off_domains:domain} {on_off_states:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "all",
+                    "sentences": [
+                        "<is_it> <all> {on_off_domains:domain} {on_off_states:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "which",
+                    "sentences": [
+                        "<what_is> {on_off_domains:domain} [\u0627\u0644\u062a\u064a] {on_off_states:state} [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "<how_many> {on_off_domains:domain} [\u0627\u0644\u062a\u064a] {on_off_states:state} [<in> <area>]"
+                    ]
+                },
+                {
                     "requires_context": {
                         "domain": "cover"
                     },
                     "response": "one_yesno",
                     "sentences": [
                         "\u0647\u0644 <name> {cover_states:state} [<in> <area>]"
                     ],
@@ -79,23 +132,25 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fans_area",
                     "sentences": [
                         "<turn_off> [<all>] <fan> [<in>] <area>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
+                    "response": "fan_all",
                     "sentences": [
                         "<turn_off> [<all>] <fan>"
                     ],
                     "slots": {
                         "area": "all",
                         "domain": "fan",
                         "name": "all"
@@ -161,20 +216,51 @@
                     "response": "cover_device_class",
                     "sentences": [
                         "<close> {cover_classes:device_class} [<in>] <area>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "unlock",
+                    "sentences": [
+                        "<open> <name> [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "unlock",
+                    "sentences": [
+                        "<open> [<all>] <lock> [<in>] <area>"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
+                    "sentences": [
+                        "[<turn_on>] [<scene>] <name>"
+                    ],
+                    "slots": {
+                        "domain": "scene"
+                    }
+                },
+                {
                     "response": "lights_area",
                     "sentences": [
                         "<turn_on> [<all>] <light> [<in>] <area>"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
@@ -205,24 +291,44 @@
                         "<open> {cover_classes:device_class} <in> <area>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
+                    "response": "fans_area",
                     "sentences": [
                         "<turn_on> [<all>] <fan> [<in>] <area>"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock",
+                    "sentences": [
+                        "<close> <name> [<in> <area>]"
+                    ]
+                },
+                {
+                    "response": "lock",
+                    "sentences": [
+                        "<close> [<all>] <lock> [<in>] <area>"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
                         "domain": "script"
                     },
                     "response": "script",
                     "sentences": [
                         "[<turn_on>] [<script>] <name>",
                         "[<script>] <name> <turn_on>"
                     ],
@@ -373,19 +479,19 @@
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "\u0634\u063a\u0644",
+                    "in": "(\u0634\u063a\u0627\u0644|[\u062a|\u064a]\u0639\u0645\u0644|[\u064a|\u062a]\u0648\u062c\u062f|[\u064a|\u062a]\u0634\u062d\u0646)",
                     "out": "on"
                 },
                 {
-                    "in": "\u0627\u0637\u0641\u064a",
+                    "in": "(\u0645\u0637\u0641\u064a|\u0644\u0627 [\u062a|\u064a]\u0639\u0645\u0644|\u0644\u0627 [\u064a|\u062a]\u0648\u062c\u062f|\u0644\u0627 [\u064a|\u062a]\u0634\u062d\u0646)",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
@@ -393,15 +499,15 @@
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 "\u0645\u0626\u0648\u064a\u0629",
                 {
-                    "in": "c",
+                    "in": "\u00b0c",
                     "out": "celsius"
                 },
                 "\u0641\u0647\u0631\u0646\u0647\u0627\u064a\u062a",
                 {
                     "in": "f",
                     "out": "fahrenheit"
                 }
@@ -418,27 +524,27 @@
             "no_intent": "\u0639\u0641\u0648\u0627, \u0644\u0645 \u0627\u0641\u0647\u0645 \u0647\u0630\u0627"
         },
         "intents": {
             "HassGetState": {
                 "all": "{% if not query.unmatched: %}\n  \u0627\u062c\u0644\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u0644\u0627, {{ no_match[:3] | join(\", \") }} \u0648 {{ (no_match | length - 3) }} \u0627\u064a\u0636\u0627\n  {%- else -%}\n    \u0644\u0627,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor %} \u0644\u064a\u0633\u062a\n  {% endif %}\n{% endif %}\n",
                 "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    \u0627\u062c\u0644, {{ match[:3] | join(\", \") }} \u0648 {{ (match | length - 3) }} \u0627\u064a\u0636\u0627\n  {%- else -%}\n    \u0627\u062c\u0644,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u0644\u0627\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "{{ slots.name | capitalize }} \u0647\u0648 {{ state.state_with_unit }}\n",
+                "one": "\u062d\u0627\u0644\u0629 {{ slots.name }} \u0647\u064a {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched %}\n  \u0627\u062c\u0644\n{% else %}\n  \u0644\u0627, {{ state.state_with_unit }}\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  \u0644\u0627 \u064a\u0648\u062c\u062f\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} \u0648 {{ (match | length - 3) }} \u0627\u064a\u0636\u0627\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} \u0648 {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
                 "cover": "\u062a\u0645 \u0627\u0644\u0627\u063a\u0644\u0627\u0642",
                 "cover_device_class": "\u062a\u0645 \u0627\u063a\u0644\u0627\u0642 {{ slots.device_class }}",
                 "default": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 {{state.domain}}",
                 "fan_all": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u062c\u0645\u064a\u0639 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
                 "fans_area": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
                 "light_all": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u062c\u0645\u064a\u0639 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
                 "lights_area": "\u062a\u0645 \u0627\u0637\u0641\u0627\u0621 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
-                "lock": "\u062a\u0645 \u0627\u0644\u0641\u062a\u062d"
+                "unlock": "\u062a\u0645 \u0627\u0644\u0641\u062a\u062d"
             },
             "HassTurnOn": {
                 "cover": "\u062a\u0645 \u0627\u0644\u0641\u062a\u062d",
                 "cover_device_class": "\u062a\u0645 \u0641\u062a\u062d {{ slots.device_class }}",
                 "default": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 {{state.domain}}",
                 "fans_area": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 \u0627\u0644\u0645\u0631\u0627\u0648\u062d",
                 "lights_area": "\u062a\u0645 \u062a\u0634\u063a\u064a\u0644 \u0627\u0644\u0627\u0636\u0648\u0627\u0621",
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/cs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996913580246914%*

 * *Differences: {"'intents'": "{'HassTurnOff': {'data': {7: {'requires_context': {'device_class': {insert: [(0, "*

 * *              "'awning'), (3, 'shade')]}}}, 8: {'sentences': ['(<zavrit>|<zatahnout>) "*

 * *              "(rolet(u|y)|žaluzi(i|e)|závěs[y]|markýz[u|y]|stínítk[o|a]) <area>'], 'slots': "*

 * *              "{'device_class': {insert: [(0, 'awning'), (3, 'shade')]}}}}}, 'HassTurnOn': "*

 * *              "{'data': {4: {'requires_context': {'device_class': {insert: [(0, 'awning'), (3, "*

 * *              "'shade')]}}}, 5: {'sentenc […]*

```diff
@@ -154,34 +154,38 @@
                     "sentences": [
                         "<zavrit> {name} [<area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "device_class": [
+                            "awning",
                             "blind",
                             "curtain",
+                            "shade",
                             "shutter"
                         ],
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
                         "<zatahnout> {name} [<area>]"
                     ]
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "(<zavrit>|<zatahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]) <area>"
+                        "(<zavrit>|<zatahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]|mark\u00fdz[u|y]|st\u00edn\u00edtk[o|a]) <area>"
                     ],
                     "slots": {
                         "device_class": [
+                            "awning",
                             "blind",
                             "curtain",
+                            "shade",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 }
             ]
         },
@@ -227,34 +231,38 @@
                     "sentences": [
                         "<otevrit> {name} [<area>]"
                     ]
                 },
                 {
                     "requires_context": {
                         "device_class": [
+                            "awning",
                             "blind",
                             "curtain",
+                            "shade",
                             "shutter"
                         ],
                         "domain": "cover"
                     },
                     "response": "cover",
                     "sentences": [
                         "<roztahnout> {name} [<area>]"
                     ]
                 },
                 {
                     "response": "cover_area",
                     "sentences": [
-                        "(<otevrit>|<roztahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]) <area>"
+                        "(<otevrit>|<roztahnout>) (rolet(u|y)|\u017ealuzi(i|e)|z\u00e1v\u011bs[y]|mark\u00fdz[u|y]|st\u00edn\u00edtk[o|a]) <area>"
                     ],
                     "slots": {
                         "device_class": [
+                            "awning",
                             "blind",
                             "curtain",
+                            "shade",
                             "shutter"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area",
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9617898441427853%*

 * *Differences: {"'expansion_rules'": "{'batterie': '[die|der|des] (Batterie[n]|Akku[s])', 'irgend': "*

 * *                      "'(irgend(ein[e][s]|welche)|einige)', 'ladestand': '[der] [Lade][zu]Stand'}",*

 * * "'intents'": "{'HassGetState': {'data': {insert: [(0, OrderedDict([('sentences', ['ist <name> "*

 * *              "[<batterie>] [<area>] {bs_battery_states:state}', 'ist [<ladestand>] <batterie> "*

 * *              "<von_dem> <name> [<area>] {bs_battery_states:state}']), ('response', "*

 * *              "'einzeln_janein'), ('requires_ […]*

```diff
@@ -9,18 +9,21 @@
         "alle_luefter": "alle (Ventilatoren|L\u00fcfter)",
         "alle_tore": "alle (Tore|Garagentore)",
         "an": "(an|ein|auf)",
         "area": "((in|an|auf) (der|dem)|im|am) {area}",
         "auf": "(auf|hoch|rauf|nach oben)",
         "aus": "(aus|ab|zu)",
         "ausfuehren": "(start[e|en]|ausf\u00fchren)",
+        "batterie": "[die|der|des] (Batterie[n]|Akku[s])",
         "brightness": "{brightness} [Prozent|%]",
         "deaktivieren": "de<aktivieren>",
         "entsperren": "((ent|auf)<sperren>|\u00f6ffne|entrieg(el|le))[n]",
         "garage": "(die Garage|die Garagen|das Garagentor|die Garagentore)",
+        "irgend": "(irgend(ein[e][s]|welche)|einige)",
+        "ladestand": "[der] [Lade][zu]Stand",
         "licht": "([das] Licht|[die] Lampe|[die] Beleuchtung)",
         "lichter": "[die|der|von den] (Lichter|Lichtern|Lampen|Leuchten|Beleuchtungen)",
         "luefter": "(den Ventilator|die Ventilatoren|(den|die) L\u00fcfter)",
         "machen": "(mach[e|en])",
         "name": "[(der|den|dem|die|das)] {name}",
         "schliessen": "(schlie(\u00df|ss)|schlie(\u00df|ss)e|zumachen|zu machen)",
         "schloss": "[das|die] (Schloss|Schl\u00f6sser)",
@@ -34,14 +37,126 @@
         "von_dem": "(von [dem]|vom)",
         "zu": "(zu|[he]runter|nach unten)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
+                    "requires_context": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    },
+                    "response": "einzeln_janein",
+                    "sentences": [
+                        "ist <name> [<batterie>] [<area>] {bs_battery_states:state}",
+                        "ist [<ladestand>] <batterie> <von_dem> <name> [<area>] {bs_battery_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "(ist|sind) <irgend> <batterie> [<area>] {bs_battery_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "alle",
+                    "sentences": [
+                        "sind alle <batterie> [<area>] {bs_battery_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "welches",
+                    "sentences": [
+                        "(welche[r]) <batterie> [<area>] (ist|sind) {bs_battery_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "wie_viele",
+                    "sentences": [
+                        "wie viele <batterie> [<area>] (ist|sind) {bs_battery_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    },
+                    "response": "einzeln_janein",
+                    "sentences": [
+                        "wird <name> [<batterie>] [<area>] {bs_battery_charging_states:state}",
+                        "{bs_battery_charging_states:state} <name> [<batterie>] [<area>] [auf]"
+                    ],
+                    "slots": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "(wird|werden) <irgend> <batterie> [<area>] {bs_battery_charging_states:state}",
+                        "{bs_battery_charging_states:state} <irgend> <batterie> [<area>] [auf]"
+                    ],
+                    "slots": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "alle",
+                    "sentences": [
+                        "werden alle <batterie> [<area>] {bs_battery_charging_states:state}",
+                        "{bs_battery_charging_states:state} alle <batterie> [<area>] [auf]"
+                    ],
+                    "slots": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "welches",
+                    "sentences": [
+                        "(welche[r]) <batterie> [<area>] [wird|werden] {bs_battery_charging_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "wie_viele",
+                    "sentences": [
+                        "wie viele <batterie> [<area>] [wird|werden] {bs_battery_charging_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "battery_charging",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "einzeln",
@@ -491,14 +606,38 @@
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
+        "bs_battery_charging_states": {
+            "values": [
+                {
+                    "in": "(l\u00e4dt|[auf][ge]laden) [auf]",
+                    "out": "on"
+                },
+                {
+                    "in": "(l\u00e4dt nicht|nicht [auf][ge]laden|laden nicht) [auf]",
+                    "out": "off"
+                }
+            ]
+        },
+        "bs_battery_states": {
+            "values": [
+                {
+                    "in": "(niedrig|gering|schwach)",
+                    "out": "on"
+                },
+                {
+                    "in": "normal",
+                    "out": "off"
+                }
+            ]
+        },
         "color": {
             "values": [
                 {
                     "in": "wei(\u00df|ss)",
                     "out": "white"
                 },
                 {
@@ -706,14 +845,17 @@
     "skip_words": [
         "bitte",
         "danke",
         "gef\u00e4lligst",
         "jetzt",
         "sofort",
         "gleich",
+        "gerade",
+        "momentan",
+        "im Moment",
         "mal",
         "eben",
         "kannst du",
         "k\u00f6nntest du",
         "w\u00fcrdest du",
         "du sollst",
         "\u00e4hm",
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/el.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nl.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9957574802006303%*

 * *Differences: {"'expansion_rules'": "{'open': '(open|omhoog|naar boven|opwaarts)', 'dicht': '(dicht|omlaag|naar "*

 * *                      "beneden|neerwaarts)'}",*

 * * "'intents'": "{'HassTurnOff': {'data': {0: {'sentences': ['[<doe>] [<alle>] <ventilator> [<naar>] "*

 * *              "uit <in> <area>', '<zou> [<alle>] <ventilator> [<naar>] (uit willen |uit kunnen "*

 * *              "|uit[ ])<doe> <in> <area>', '[<doe>] [<alle>] <ventilator> <in> <area> [<naar>] "*

 * *              "uit', '<zou> [<alle>] <ventilator> <in> <area> [<naar>] […]*

```diff
@@ -4,29 +4,29 @@
         "alle": "(alle[maal]|elk[e]|ieder[e]|overal)",
         "area": "[de|het] {area}",
         "awning": "(luifel[s]|[zonne]scherm[en])",
         "blind": "(jaloezie[\u00ebn]|luxaflex)",
         "brightness": "{brightness}[%|procent]",
         "curtain": "(gordijn[en]|vitrage[s])",
         "detecteer": "(detecteert|registreert|detecteren|registreren|gedetecteerd|geregistreerd|waar[ ]genomen)",
-        "dicht": "(dicht|omlaag|naar beneden|sluiten|neerwaarts)",
+        "dicht": "(dicht|omlaag|naar beneden|neerwaarts)",
         "doe": "(zet[ten]|mag|mogen|doe[n]|verander[en]|maak|maken|schakel[en])",
         "door": "deur[en]",
         "garage": "garage[ ]deur[en]",
         "gate": "(hek[ken]|poort[en])",
         "helderheid": "[de] (helderheid|felheid|intensiteit|lichtsterkte)",
         "in": "[in|op|van|bij]",
         "is": "(zijn|is|staa(n|t)|zit[ten]|word[t|en]|lig(t|gen))",
         "lamp": "[de|het|een] (lamp[en]|licht[en]|verlichting)",
         "met": "(door|met|bij)",
         "naar": "(naar|op)",
         "name": "[de|het] {name}",
         "name_area": "(\n  [[door|met|bij] [de|het] {area}][ ]{name}\n  |[<in> [de|het] {area}] [door|met|bij] <name>\n  |[<met>] [de|het] {name} [[in|op|van|bij] <area>]\n)\n",
         "op_slot": "<naar> (slot|vergrendeld)",
-        "open": "(open[en]|omhoog|naar boven|opwaarts)",
+        "open": "(open|omhoog|naar boven|opwaarts)",
         "schakelaar": "[de|een] (schakelaar[s]|switch[es]|plug[gen])",
         "sensor": "[een|de] (apparaat|apparaten|sensor[s|en]|iets)",
         "sensor_area": "(\n  [[de|een] {area}][ ](apparaat|apparaten|sensor[s|en])\n  |[<in> [de|het] {area}] <sensor>\n  |[een|de] (apparaat|apparaten|sensor[s|en]|iets) [[in|op|van|bij] <area>]\n)\n",
         "shade": "(screen[s]|rolgordijn[en])",
         "shutter": "(rolluik[en]|shutter[s])",
         "slot": "[de|het|een] ([deur]slot[en]|vergrendeling[en])",
         "slot_name_area": "[<in> <area>] (<slot> [van] [{area}[ ]]<name>|[de|het] {name}[ ]([deur]slot[en]|vergrendeling[en])) [[in|op|van|bij] [de|het] {area}]",
@@ -1017,28 +1017,35 @@
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
                     "response": "fans_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] uit [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
+                        "[<doe>] [<alle>] <ventilator> [<naar>] uit <in> <area>",
+                        "<zou> [<alle>] <ventilator> [<naar>] (uit willen |uit kunnen |uit[ ])<doe> <in> <area>",
+                        "[<doe>] [<alle>] <ventilator> <in> <area> [<naar>] uit",
+                        "<zou> [<alle>] <ventilator> <in> <area> [<naar>] (uit willen |uit kunnen |uit[ ])<doe>",
+                        "[<doe>] [(<alle>|<in>)] <area>[ ]<ventilator> [<naar>] uit",
+                        "<zou> [(<alle>|<in>)] <area>[ ]<ventilator> [<naar>] (uit willen |uit kunnen |uit[ ])<doe>",
+                        "<zou> [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen)",
+                        "[(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] (uit[ ](zetten|doen)|uitschakelen)"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "response": "fan_all",
                     "sentences": [
-                        "[<doe>|<zou>] ((overal|<alle>) <ventilator>|<ventilator> overal) uit [[willen|kunnen] <doe>]"
+                        "[<doe>] ((overal|<alle>) <ventilator>|<ventilator> overal) uit",
+                        "<zou> ((overal|<alle>) <ventilator>|<ventilator> overal) (uit willen |uit kunnen |uit[ ])<doe>",
+                        "<zou> ((overal|<alle>) <ventilator>|<ventilator> overal) [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen)",
+                        "((overal|<alle>) <ventilator>|<ventilator> overal) (uit[ ](zetten|doen)|uitschakelen)"
                     ],
                     "slots": {
                         "area": "all",
                         "domain": "fan",
                         "name": "all"
                     }
                 },
@@ -1046,69 +1053,87 @@
                     "excludes_context": {
                         "domain": [
                             "cover",
                             "script"
                         ]
                     },
                     "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
+                        "[<doe>] <name>[ ][<type>] [<naar>] uit",
+                        "<zou> <name>[ ][<type>] [<naar>] (uit willen |uit kunnen |uit [ ])<doe>",
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen|doen)"
                     ]
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] <lamp> [<naar>] uit [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <lamp> <in> <area> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area>[ ]<lamp> [<naar>] uit [[willen|kunnen] <doe>]",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] [willen|kunnen] (uit[ ]zetten|uitschakelen)"
+                        "[<doe>] [<alle>] <lamp> [<naar>] uit <in> <area>",
+                        "<zou> [<alle>] <lamp> [<naar>] (uit willen |uit kunnen |uit[ ])<doe> <in> <area>",
+                        "[<doe>] [<alle>] <lamp> <in> <area> [<naar>] uit",
+                        "<zou> [<alle>] <lamp> <in> <area> [<naar>] (uit willen |uit kunnen |uit[ ])<doe>",
+                        "[<doe>] [(<alle>|<in>)] <area>[ ]<lamp> [<naar>] uit",
+                        "<zou> [(<alle>|<in>)] <area>[ ]<lamp> [<naar>] (uit willen |uit kunnen |uit[ ])<doe>",
+                        "<zou> [(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen)",
+                        "[(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] (uit[ ](zetten|doen)|uitschakelen)"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
                     "response": "light_all",
                     "sentences": [
-                        "[<doe>|<zou>] ((overal|<alle>) <lamp>|<lamp> overal) uit [[willen|kunnen] <doe>]"
+                        "[<doe>] ((overal|<alle>) <lamp>|<lamp> overal) uit",
+                        "<zou> ((overal|<alle>) <lamp>|<lamp> overal) (uit willen |uit kunnen |uit[ ])<doe>",
+                        "<zou> ((overal|<alle>) <lamp>|<lamp> overal) [willen|kunnen] (uit[ ](zetten|doen)|uitschakelen)",
+                        "((overal|<alle>) <lamp>|<lamp> overal) (uit[ ](zetten|doen)|uitschakelen)"
                     ],
                     "slots": {
                         "area": "all",
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "sluit <name>",
-                        "[<doe>|<zou>] <name> <dicht> [[willen|kunnen] <doe>]"
+                        "<name> sluiten",
+                        "[<doe>] <name> <dicht>",
+                        "<zou> <name> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten)",
+                        "<zou> <name> (willen|kunnen) [<dicht>[ ]<doe>|sluiten]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
                         "sluit [de] garage[ ][deur]",
-                        "[<doe>|<zou>] [de] garage[ ][deur] dicht [[willen|kunnen] <doe>]"
+                        "[de] garage[ ][deur] sluiten",
+                        "[<doe>] [de] garage[ ][deur] <dicht>",
+                        "<zou> [de] garage[ ][deur] ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten)",
+                        "<zou> [de] garage[ ][deur] (kunnen|willen) [<dicht>[ ]<doe>|sluiten]"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "sluit <name> <in> <area>",
-                        "[<doe>|<zou>] <name> (<dicht> <in> <area>|<in> <area> <dicht>) [[willen|kunnen] <doe>]",
-                        "<zou> <name> <in> <area> (willen|kunnen) [<dicht>]"
+                        "<name> <in> <area> sluiten",
+                        "[<doe>] <name> (<dicht> <in> <area>|<in> <area> <dicht>)",
+                        "<zou> <name> <in> <area> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten)",
+                        "<zou> <name> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten) <in> <area>",
+                        "<zou> <name> <in> <area> (willen|kunnen) [<dicht>[ ]<doe>|sluiten]",
+                        "<zou> <name> (willen|kunnen) [<dicht>[ ]<doe>|sluiten] <in> <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter",
                             "shade"
@@ -1116,28 +1141,35 @@
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "sluit [de|het] <curtain> <in> <area>",
-                        "[<doe>|<zou>] [de|het] <curtain> (<dicht> <in> <area>|<in> <area> <dicht>) [[willen|kunnen] <doe>]",
-                        "<zou> [de|het] <curtain> <in> <area> [willen|kunnen] <dicht>"
+                        "[de|het] <curtain> <in> <area> sluiten",
+                        "[<doe>] [de|het] <curtain> (<dicht> <in> <area>|<in> <area> <dicht>)",
+                        "<zou> [de|het] <curtain> <in> <area> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten)",
+                        "<zou> [de|het] <curtain> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten) <in> <area>",
+                        "<zou> [de|het] <curtain> <in> <area> (willen|kunnen) [<dicht>[ ]<doe>|sluiten]",
+                        "<zou> [de|het] <curtain> (willen|kunnen) [<dicht>[ ]<doe>|sluiten] <in> <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "sluit [de|het] (<blind>|<shutter>|<shade>) <in> <area>",
-                        "[<doe>|<zou>] [de|het] (<blind>|<shutter>|<shade>) (<dicht> <in> <area>|<in> <area> <dicht>) [[willen|kunnen] <doe>]",
-                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> [willen|kunnen] <dicht>"
+                        "[<doe>] [de|het] (<blind>|<shutter>|<shade>) (<dicht> <in> <area>|<in> <area> <dicht>)",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten)",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) ((<dicht> willen | <dicht> kunnen | <dicht>[ ])<doe>|sluiten) <in> <area>",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> (willen|kunnen) [<dicht>[ ]<doe>|sluiten]",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) (willen|kunnen) [<dicht>[ ]<doe>|sluiten] <in> <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "shutter",
                             "shade"
                         ],
@@ -1146,34 +1178,42 @@
                 },
                 {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "lock",
                     "sentences": [
-                        "[<doe>|<zou>|haal] <name_area> <van_slot> [[willen|kunnen] (<doe>|halen)] [<in> <area>]",
+                        "[<doe>|haal] <name_area> <van_slot> [<in> <area>]",
+                        "<zou> <name_area> <van_slot> [willen|kunnen] (<doe>|halen) [<in> <area>]",
                         "ontgrendel <name_area>",
                         "<zou> <name_area> [willen|kunnen] ontgrendelen [<in> <area>]",
-                        "[<doe>|<zou>] <slot_name_area> open [[willen|kunnen] <doe>] [<in> <area>]",
+                        "[<doe>] <slot_name_area> open [<in> <area>]",
+                        "<zou> <slot_name_area> (open willen |open kunnen |open[ ])<doe> [<in> <area>]",
                         "open <slot_name_area>",
                         "<zou> <slot_name_area> [willen|kunnen] openen [<in> <area>]"
                     ]
                 },
                 {
                     "response": "lock_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <van_slot> [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <van_slot> [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <in> <area> <van_slot> [[willen|kunnen] <doe>]",
+                        "[<doe>] [<alle>] (<slot>|deur[en]) <van_slot> <in> <area>",
+                        "[<doe>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <van_slot>",
+                        "[<doe>] [<alle>] (<slot>|deur[en]) <in> <area> <van_slot>",
+                        "<zou> [<alle>] (<slot>|deur[en]) <van_slot> [willen|kunnen] <doe> <in> <area>",
+                        "<zou> [<alle>] <area>[ |<alle>](<slot>|deur[en]) <van_slot> [willen|kunnen] <doe>",
+                        "<zou> [<alle>] (<slot>|deur[en]) <in> <area> <van_slot> [willen|kunnen] <doe>",
                         "ontgrendel [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>)",
                         "<zou> [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>) [willen|kunnen] ontgrendelen",
                         "<zou> [<alle>] (<slot>|deur[en]) [willen|kunnen] ontgrendelen <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <in> <area>[ |<alle>]<slot> open [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> <in> <area> open [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> open [[willen|kunnen] <doe>] <in> <area>",
+                        "[<doe>] [<alle>] <in> <area>[ |<alle>]<slot> open",
+                        "[<doe>] [<alle>] <slot> <in> <area> open",
+                        "[<doe>] [<alle>] <slot> open <in> <area>",
+                        "<zou> [<alle>] <in> <area>[ |<alle>]<slot> (open willen |open kunnen |open[ ])<doe>",
+                        "<zou> [<alle>] <slot> <in> <area> (open willen |open kunnen |open[ ])<doe>",
+                        "<zou> [<alle>] <slot> (open willen |open kunnen |open[ ]<doe>) <in> <area>",
                         "open [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>)",
                         "<zou> [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>) [willen|kunnen] openen",
                         "<zou> [<alle>] <slot> [willen|kunnen] openen <in> <area>"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
@@ -1186,64 +1226,78 @@
                 {
                     "requires_context": {
                         "domain": "scene"
                     },
                     "response": "scene",
                     "sentences": [
                         "(activeer|start|schakel) [scene|sc\u00e8ne] <name>[ ][scene|sc\u00e8ne] [<naar>] [in]",
-                        "[<doe>|<zou>] [scene|sc\u00e8ne] <name>[ ][scene|sc\u00e8ne] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
-                        "[<zou>] <name>[ ][scene|sc\u00e8ne] [willen|kunnen] (aan[ ]zetten|inschakelen|starten|activeren)"
+                        "[<doe>] [scene|sc\u00e8ne] <name>[ ][scene|sc\u00e8ne] [<naar>] (aan|in)",
+                        "<zou> [scene|sc\u00e8ne] <name>[ ][scene|sc\u00e8ne] [<naar>] (aan willen |aan kunnen |aan [ ])<doe>",
+                        "[<zou>] <name>[ ][scene|sc\u00e8ne] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|starten|activeren)"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
                     "response": "lights_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] <lamp> [<naar>] aan [[willen|kunnen] <doe>] (in|op) <area>",
-                        "Schakel [<alle>] <lamp> [<naar>] in (in|op) <area>",
-                        "[<doe>|<zou>] [<alle>] <lamp> <in> <area> [<naar>] aan [[willen|kunnen] <doe>]",
-                        "Schakel [<alle>] <lamp> <in> <area> in",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area>[ ]<lamp> aan [[willen|kunnen] <doe>]",
-                        "Schakel [(<alle>|<in>)] <area>[ ]<lamp> in",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
+                        "[<doe>] [<alle>] <lamp> [<naar>] aan <in> <area>",
+                        "<zou> [<alle>] <lamp> [<naar>] (aan willen |aan kunnen |aan[ ])<doe> <in> <area>",
+                        "Schakel [<alle>] <lamp> [<naar>] in <in> <area>",
+                        "[<doe>] [<alle>] <lamp> <in> <area> [<naar>] aan",
+                        "<zou> [<alle>] <lamp> <in> <area> [<naar>] (aan willen |aan kunnen |aan[ ])<doe>",
+                        "Schakel [<alle>] <lamp> <in> <area> [<naar>] in",
+                        "[<doe>] [(<alle>|<in>)] <area> <lamp> [<naar>] aan",
+                        "<zou> [(<alle>|<in>)] <area> <lamp> [<naar>] (aan willen |aan kunnen |aan[ ])<doe>",
+                        "Schakel [(<alle>|<in>)] <area>[ ]<lamp> [<naar>] in",
+                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<lamp> [<in> <area>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen)"
                     ],
                     "slots": {
                         "domain": "light",
                         "name": "all"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "open <name>",
-                        "[<doe>|<zou>] <name> <open> [[willen|kunnen] <doe>]"
+                        "<name> openen",
+                        "[<doe>] <name> <open>",
+                        "<zou> <name> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen)",
+                        "<zou> <name> (willen|kunnen) [<open>[ ]<doe>|openen]"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover_device_class",
                     "sentences": [
                         "open [de] garage[ ][deur]",
-                        "[<doe>|<zou>] [de] garage[ ][deur] [<open>] [[willen|kunnen] <doe>]"
+                        "[de] garage[ ][deur] openen",
+                        "[<doe>] [de] garage[ ][deur] <open>",
+                        "<zou> [de] garage[ ][deur] ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen)",
+                        "<zou> [de] garage[ ][deur] (kunnen|willen) [<open>[ ]<doe>|openen]"
                     ],
                     "slots": {
                         "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "open <name> <in> <area>",
-                        "[<doe> |<zou> ]<name> (<open> <in> <area>|<in> <area> <open>) [[willen|kunnen] <doe>]",
-                        "<zou> <name> <in> <area> (willen|kunnen) <open>"
+                        "<name> <in> <area> openen",
+                        "[<doe>] <name> (<open> <in> <area>|<in> <area> <open>)",
+                        "<zou> <name> <in> <area> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen)",
+                        "<zou> <name> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen) <in> <area>",
+                        "<zou> <name> <in> <area> (willen|kunnen) [<open>[ ]<doe>|openen]",
+                        "<zou> <name> (willen|kunnen) [<open>[ ]<doe>|openen] <in> <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "curtain",
                             "shutter",
                             "shade"
@@ -1251,80 +1305,98 @@
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "open [de|het] <curtain> <in> <area>",
-                        "[<doe>|<zou>] [de|het] <curtain> (<open> <in> <area>|<in> <area> <open>) [[willen|kunnen] <doe>]",
-                        "<zou> [de|het] <curtain> <in> <area> [willen|kunnen] <open>"
+                        "[de|het] <curtain> <in> <area> openen",
+                        "[<doe>] [de|het] <curtain> (<open> <in> <area>|<in> <area> <open>)",
+                        "<zou> [de|het] <curtain> <in> <area> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen)",
+                        "<zou> [de|het] <curtain> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen) <in> <area>",
+                        "<zou> [de|het] <curtain> <in> <area> (willen|kunnen) [<open>[ ]<doe>|openen]",
+                        "<zou> [de|het] <curtain> (willen|kunnen) [<open>[ ]<doe>|openen] <in> <area>"
                     ],
                     "slots": {
                         "device_class": "curtain",
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "cover",
                     "sentences": [
                         "open [de|het] (<blind>|<shutter>|<shade>) <in> <area>",
-                        "[<doe>|<zou>] [de|het] (<blind>|<shutter>|<shade>) (<open> <in> <area>|<in> <area> <open>) [[willen|kunnen] <doe>]",
-                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> [willen|kunnen] <open>"
+                        "[<doe>] [de|het] (<blind>|<shutter>|<shade>) (<open> <in> <area>|<in> <area> <open>)",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen)",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) ((<open> willen | <open> kunnen | <open>[ ])<doe>|openen) <in> <area>",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) <in> <area> (willen|kunnen) [<open>[ ]<doe>|openen]",
+                        "<zou> [de|het] (<blind>|<shutter>|<shade>) (willen|kunnen) [<open>[ ]<doe>|openen] <in> <area>"
                     ],
                     "slots": {
                         "device_class": [
                             "blind",
                             "shutter",
                             "shade"
                         ],
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "fans_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] <ventilator> [<naar>] aan [[willen|kunnen] <doe>] <in> <area>",
+                        "[<doe>] [<alle>] <ventilator> [<naar>] aan <in> <area>",
+                        "<zou> [<alle>] <ventilator> [<naar>] [[aan willen |aan kunnen |aan[ ]]<doe>] <in> <area>",
                         "Schakel [<alle>] <ventilator> [<naar>] in <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <ventilator> <in> <area> [<naar>] aan [[willen|kunnen] <doe>]",
+                        "[<doe>] [<alle>] <ventilator> <in> <area> [<naar>] aan",
+                        "<zou> [<alle>] <ventilator> <in> <area> [<naar>] [[aan willen |aan kunnen |aan[ ]]<doe>]",
                         "Schakel [<alle>] <ventilator> <in> <area> [<naar>] in",
-                        "[<doe>|<zou>] [(<alle>|<in>)] <area> <ventilator> [<naar>] aan [[willen|kunnen] <doe>]",
+                        "[<doe>] [(<alle>|<in>)] <area> <ventilator> [<naar>] aan",
+                        "<zou> [(<alle>|<in>)] <area> <ventilator> [<naar>] [[aan willen |aan kunnen |aan[ ]]<doe>]",
                         "Schakel [(<alle>|<in>)] <area>[ ]<ventilator> [<naar>] in",
-                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
+                        "[<zou>] [(<alle>|<in>)] [<area>[ ]]<ventilator> [<in> <area>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen)"
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "lock",
                     "sentences": [
-                        "[<doe>|<zou>] <name_area> <op_slot> [[willen|kunnen] <doe>] [<in> <area>]",
+                        "[<doe>] <name_area> <op_slot>",
+                        "<zou> <name_area> <op_slot> [willen|kunnen] <doe> [<in> <area>]",
                         "vergrendel <name_area>",
                         "<zou> <name_area> [willen|kunnen] vergrendelen [<in> <area>]",
-                        "[<doe>|<zou>] <slot_name_area> dicht [[willen|kunnen] <doe>] [<in> <area>]",
+                        "[<doe>] <slot_name_area> dicht [<in> <area>]",
+                        "<zou> <slot_name_area> (dicht willen |dicht kunnen |dicht[ ])<doe> [<in> <area>]",
                         "sluit <slot_name_area>",
                         "<zou> <slot_name_area> [willen|kunnen] sluiten [<in> <area>]"
                     ]
                 },
                 {
                     "response": "lock_area",
                     "sentences": [
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>] <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <op_slot> [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] (<slot>|deur[en]) <in> <area> <op_slot> [[willen|kunnen] <doe>]",
+                        "[<doe>] [<alle>] (<slot>|deur[en]) <op_slot> <in> <area>",
+                        "[<doe>] [<alle>] <area>[ |<alle>](<slot>|deur[en]) <op_slot>",
+                        "[<doe>] [<alle>] (<slot>|deur[en]) <in> <area> <op_slot>",
+                        "<zou> [<alle>] (<slot>|deur[en]) <op_slot> [willen|kunnen] <doe> <in> <area>",
+                        "<zou> [<alle>] <area>[ |<alle>](<slot>|deur[en]) <op_slot> [willen|kunnen] <doe>",
+                        "<zou> [<alle>] (<slot>|deur[en]) <in> <area> <op_slot> [willen|kunnen] <doe>",
                         "vergrendel [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>)",
                         "<zou> [<alle>] (<in> <area>[ |<alle>](<slot>|deur[en])|(<slot>|deur[en]) <in> <area>) [willen|kunnen] vergrendelen",
                         "<zou> [<alle>] (<slot>|deur[en]) [willen|kunnen] vergrendelen <in> <area>",
-                        "[<doe>|<zou>] [<alle>] <in> <area>[ |<alle>]<slot> dicht [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> <in> <area> dicht [[willen|kunnen] <doe>]",
-                        "[<doe>|<zou>] [<alle>] <slot> dicht [[willen|kunnen] <doe>] <in> <area>",
+                        "[<doe>] [<alle>] <in> <area>[ |<alle>]<slot> dicht",
+                        "[<doe>] [<alle>] <slot> <in> <area> dicht",
+                        "[<doe>] [<alle>] <slot> dicht <in> <area>",
+                        "<zou> [<alle>] <in> <area>[ |<alle>]<slot> (dicht willen |dicht kunnen |dicht[ ])<doe>",
+                        "<zou> [<alle>] <slot> <in> <area> (dicht willen |dicht kunnen |dicht[ ])<doe>",
+                        "<zou> [<alle>] <slot> (dicht willen |dicht kunnen |dicht[ ])<doe> <in> <area>",
                         "sluit [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>)",
                         "<zou> [<alle>] (<in> <area>[ |<alle>]<slot>|<slot> <in> <area>) [willen|kunnen] sluiten",
                         "<zou> [<alle>] <slot> [willen|kunnen] sluiten <in> <area>"
                     ],
                     "slots": {
                         "domain": "lock",
                         "name": "all"
@@ -1332,34 +1404,36 @@
                 },
                 {
                     "requires_context": {
                         "domain": "script"
                     },
                     "response": "script",
                     "sentences": [
-                        "(activeer|start|schakel) [script] <name>[ ][script] [<naar>] [in]",
-                        "[<doe>|<zou>] [script] <name>[ ][script] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
-                        "[<zou>] <name>[ ][script] [willen|kunnen] (aan[ ]zetten|inschakelen|starten|activeren)"
+                        "(activeer|start|schakel) ([script] <name>|<name>[ ][script]) [<naar>] [in]",
+                        "[<doe>] ([script] <name>|<name>[ ][script]) [<naar>] (aan|in)",
+                        "<zou> ([script] <name>|<name>[ ][script]) [<naar>] ((aan|in) willen |(aan|in) kunnen |(aan|in) [ ])<doe>",
+                        "<zou> ([script] <name>|<name>[ ][script]) [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|starten|activeren)"
                     ],
                     "slots": {
                         "domain": "script"
                     }
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover",
                             "scene",
                             "script"
                         ]
                     },
                     "sentences": [
-                        "[<doe>|<zou>] <name>[ ][<type>] [<naar>] (aan|in) [[willen|kunnen] <doe>]",
+                        "[<doe>] <name>[ ][<type>] [<naar>] aan",
+                        "<zou> <name>[ ][<type>] [<naar>] ((aan|in) willen |(aan|in) kunnen |(aan|in) [ ])<doe>",
                         "schakel <name>[ ][<type>] [<naar>] in",
-                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ]zetten|inschakelen)"
+                        "[<zou>] <name>[ ][<type>] [willen|kunnen] (aan[ ](zetten|doen)|inschakelen|doen)"
                     ]
                 }
             ]
         }
     },
     "language": "nl",
     "lists": {
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/el.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/el.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/data/light/zh-tw.json` & `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-tw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents/domains.py` & `home-assistant-intents-2023.4.26/home_assistant_intents/domains.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/PKG-INFO` & `home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: home-assistant-intents
-Version: 2023.4.17.post1
+Version: 2023.4.26
 Summary: Intents for Home Assistant
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/home-assistant/intents
 Keywords: home,assistant,intent,recognition
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `home-assistant-intents-2023.4.17.post1/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.17.post1/pyproject.toml` & `home-assistant-intents-2023.4.26/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.4.17-1"
+version     = "2023.4.26"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

