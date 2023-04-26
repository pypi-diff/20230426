# Comparing `tmp/xiaomi_flashable_firmware_creator_gui-2.3.8.tar.gz` & `tmp/xiaomi_flashable_firmware_creator_gui-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaomi_flashable_firmware_creator_gui-2.3.8.tar", max compression
+gzip compressed data, was "xiaomi_flashable_firmware_creator_gui-2.3.9.tar", max compression
```

## Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8.tar` & `xiaomi_flashable_firmware_creator_gui-2.3.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    35149 2019-06-11 17:00:19.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/LICENSE
--rw-r--r--   0        0        0     2524 2021-03-26 11:07:52.312670 xiaomi_flashable_firmware_creator_gui-2.3.8/README.md
--rw-r--r--   0        0        0     1262 2021-08-02 12:50:25.781621 xiaomi_flashable_firmware_creator_gui-2.3.8/pyproject.toml
--rw-r--r--   0        0        0      124 2021-03-26 11:07:52.296003 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/__init__.py
--rw-r--r--   0        0        0      156 2020-10-17 09:32:58.923602 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/__main__.py
--rw-r--r--   0        0        0        0 2020-10-19 13:38:03.781664 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/__init__.py
--rw-r--r--   0        0        0    22984 2020-10-28 07:53:36.022397 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/about.py
--rw-r--r--   0        0        0     1331 2020-10-19 17:57:08.713446 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/drop_space.py
--rw-r--r--   0        0        0      628 2020-10-19 16:40:44.773034 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/input_dialog.py
--rw-r--r--   0        0        0     1613 2020-10-19 16:40:44.786368 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/message_box.py
--rw-r--r--   0        0        0       21 2020-10-20 11:42:02.081106 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/data/settings.json
--rw-r--r--   0        0        0        0 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/__init__.py
--rw-r--r--   0        0        0      585 2020-10-20 11:41:37.320980 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/layout.py
--rw-r--r--   0        0        0      517 2020-10-19 16:37:16.183860 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/misc.py
--rw-r--r--   0        0        0      808 2020-10-14 10:44:33.897605 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/settings.py
--rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/af.qm
--rw-r--r--   0        0        0    27763 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ar.qm
--rw-r--r--   0        0        0    27655 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/bn-IN.qm
--rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/bn.qm
--rw-r--r--   0        0        0    27796 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ca.qm
--rw-r--r--   0        0        0    28194 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/cs.qm
--rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/da.qm
--rw-r--r--   0        0        0    17637 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/de-DE.qm
--rw-r--r--   0        0        0    28276 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/de.qm
--rw-r--r--   0        0        0    25996 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/el.qm
--rw-r--r--   0        0        0    27919 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/en.qm
--rw-r--r--   0        0        0    17275 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/en_US.qm
--rw-r--r--   0        0        0    28581 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/es-ES.qm
--rw-r--r--   0        0        0    30457 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fa.qm
--rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fi.qm
--rw-r--r--   0        0        0    28028 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fr.qm
--rw-r--r--   0        0        0    27652 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ga-IE.qm
--rw-r--r--   0        0        0    26910 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/he.qm
--rw-r--r--   0        0        0    27778 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hi.qm
--rw-r--r--   0        0        0    27861 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hr.qm
--rw-r--r--   0        0        0    28127 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hu.qm
--rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hy-AM.qm
--rw-r--r--   0        0        0    28619 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/id.qm
--rw-r--r--   0        0        0    28546 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/it.qm
--rw-r--r--   0        0        0    27639 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ja.qm
--rw-r--r--   0        0        0    27639 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ko.qm
--rw-r--r--   0        0        0    28473 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ms.qm
--rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ne-NP.qm
--rw-r--r--   0        0        0    27940 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/nl.qm
--rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/no.qm
--rw-r--r--   0        0        0    28378 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pl.qm
--rw-r--r--   0        0        0    28513 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pt-BR.qm
--rw-r--r--   0        0        0    27765 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pt-PT.qm
--rw-r--r--   0        0        0    27917 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ro.qm
--rw-r--r--   0        0        0    28475 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ru.qm
--rw-r--r--   0        0        0    27650 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sk.qm
--rw-r--r--   0        0        0    28083 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sl.qm
--rw-r--r--   0        0        0    28312 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sq.qm
--rw-r--r--   0        0        0    27657 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sr.qm
--rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sv-SE.qm
--rw-r--r--   0        0        0    17440 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/tr-TR.qm
--rw-r--r--   0        0        0    28073 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/tr.qm
--rw-r--r--   0        0        0    28181 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/uk.qm
--rw-r--r--   0        0        0    27755 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ur-PK.qm
--rw-r--r--   0        0        0    28205 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/vi.qm
--rw-r--r--   0        0        0    23384 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/zh-CN.qm
--rw-r--r--   0        0        0    27642 2021-01-13 19:35:58.586039 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/zh-TW.qm
--rw-r--r--   0        0        0     2002 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/icon.png
--rw-r--r--   0        0        0    29322 2021-01-13 18:55:39.656530 xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/main.py
--rw-r--r--   0        0        0     3782 2021-08-02 12:51:50.255939 xiaomi_flashable_firmware_creator_gui-2.3.8/setup.py
--rw-r--r--   0        0        0     3476 2021-08-02 12:51:50.256356 xiaomi_flashable_firmware_creator_gui-2.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2019-06-11 17:00:19.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/LICENSE
+-rw-r--r--   0        0        0     2524 2021-03-26 11:07:52.312670 xiaomi_flashable_firmware_creator_gui-2.3.9/README.md
+-rw-r--r--   0        0        0     1262 2022-03-23 14:03:27.708660 xiaomi_flashable_firmware_creator_gui-2.3.9/pyproject.toml
+-rw-r--r--   0        0        0      124 2021-03-26 11:07:52.296003 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/__init__.py
+-rw-r--r--   0        0        0      156 2020-10-17 09:32:58.923602 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/__main__.py
+-rw-r--r--   0        0        0        0 2020-10-19 13:38:03.781664 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/__init__.py
+-rw-r--r--   0        0        0    22984 2020-10-28 07:53:36.022397 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/about.py
+-rw-r--r--   0        0        0     1331 2020-10-19 17:57:08.713446 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/drop_space.py
+-rw-r--r--   0        0        0      628 2020-10-19 16:40:44.773034 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/input_dialog.py
+-rw-r--r--   0        0        0     1613 2020-10-19 16:40:44.786368 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/message_box.py
+-rw-r--r--   0        0        0       21 2020-10-20 11:42:02.081106 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/data/settings.json
+-rw-r--r--   0        0        0        0 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/__init__.py
+-rw-r--r--   0        0        0      585 2020-10-20 11:41:37.320980 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/layout.py
+-rw-r--r--   0        0        0      517 2020-10-19 16:37:16.183860 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/misc.py
+-rw-r--r--   0        0        0      808 2020-10-14 10:44:33.897605 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/settings.py
+-rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/af.qm
+-rw-r--r--   0        0        0    27763 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ar.qm
+-rw-r--r--   0        0        0    27655 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/bn-IN.qm
+-rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.549372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/bn.qm
+-rw-r--r--   0        0        0    27796 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ca.qm
+-rw-r--r--   0        0        0    28194 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/cs.qm
+-rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.552705 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/da.qm
+-rw-r--r--   0        0        0    17637 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/de-DE.qm
+-rw-r--r--   0        0        0    28276 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/de.qm
+-rw-r--r--   0        0        0    25996 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/el.qm
+-rw-r--r--   0        0        0    27919 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/en.qm
+-rw-r--r--   0        0        0    17275 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/en_US.qm
+-rw-r--r--   0        0        0    28581 2021-01-13 19:35:58.556039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/es-ES.qm
+-rw-r--r--   0        0        0    30457 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fa.qm
+-rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fi.qm
+-rw-r--r--   0        0        0    28028 2021-01-13 19:35:58.559372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fr.qm
+-rw-r--r--   0        0        0    27652 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ga-IE.qm
+-rw-r--r--   0        0        0    26910 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/he.qm
+-rw-r--r--   0        0        0    27778 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hi.qm
+-rw-r--r--   0        0        0    27861 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hr.qm
+-rw-r--r--   0        0        0    28127 2021-01-13 19:35:58.562706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hu.qm
+-rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hy-AM.qm
+-rw-r--r--   0        0        0    28619 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/id.qm
+-rw-r--r--   0        0        0    28546 2021-01-13 19:35:58.566039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/it.qm
+-rw-r--r--   0        0        0    27639 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ja.qm
+-rw-r--r--   0        0        0    27639 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ko.qm
+-rw-r--r--   0        0        0    28473 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ms.qm
+-rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ne-NP.qm
+-rw-r--r--   0        0        0    27940 2021-01-13 19:35:58.569372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/nl.qm
+-rw-r--r--   0        0        0    27646 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/no.qm
+-rw-r--r--   0        0        0    28378 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pl.qm
+-rw-r--r--   0        0        0    28513 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pt-BR.qm
+-rw-r--r--   0        0        0    27765 2021-01-13 19:35:58.572706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pt-PT.qm
+-rw-r--r--   0        0        0    27917 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ro.qm
+-rw-r--r--   0        0        0    28475 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ru.qm
+-rw-r--r--   0        0        0    27650 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sk.qm
+-rw-r--r--   0        0        0    28083 2021-01-13 19:35:58.576039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sl.qm
+-rw-r--r--   0        0        0    28312 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sq.qm
+-rw-r--r--   0        0        0    27657 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sr.qm
+-rw-r--r--   0        0        0    27649 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sv-SE.qm
+-rw-r--r--   0        0        0    17440 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/tr-TR.qm
+-rw-r--r--   0        0        0    28073 2021-01-13 19:35:58.579372 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/tr.qm
+-rw-r--r--   0        0        0    28181 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/uk.qm
+-rw-r--r--   0        0        0    27755 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ur-PK.qm
+-rw-r--r--   0        0        0    28205 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/vi.qm
+-rw-r--r--   0        0        0    23384 2021-01-13 19:35:58.582706 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/zh-CN.qm
+-rw-r--r--   0        0        0    27642 2021-01-13 19:35:58.586039 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/zh-TW.qm
+-rw-r--r--   0        0        0     2002 2019-08-22 12:05:59.000000 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/icon.png
+-rw-r--r--   0        0        0    29322 2021-01-13 18:55:39.656530 xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/main.py
+-rw-r--r--   0        0        0     3782 2022-03-23 14:04:18.053699 xiaomi_flashable_firmware_creator_gui-2.3.9/setup.py
+-rw-r--r--   0        0        0     3527 2022-03-23 14:04:18.053960 xiaomi_flashable_firmware_creator_gui-2.3.9/PKG-INFO
```

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/LICENSE` & `xiaomi_flashable_firmware_creator_gui-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/README.md` & `xiaomi_flashable_firmware_creator_gui-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/pyproject.toml` & `xiaomi_flashable_firmware_creator_gui-2.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xiaomi_flashable_firmware_creator_gui"
-version = "2.3.8"
+version = "2.3.9"
 description = "Create flashable firmware zip from MIUI Recovery ROMs!"
 authors = ["yshalsager <ysh-alsager@hotmail.com>"]
 license = "GPL-3.0-only"
 repository = "https://github.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator-gui/"
 homepage = "https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/"
 keywords = ["xiaomi", "firmware", "android"]
 packages = [
@@ -19,15 +19,15 @@
 
 [tool.poetry.scripts]
 xiaomi_flashable_firmware_creator_g = "xiaomi_flashable_firmware_creator_gui.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 PyQt5 = "^5.13.0"
-xiaomi_flashable_firmware_creator = "^2.2.3"
+xiaomi_flashable_firmware_creator = "^2.2.5"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/about.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/about.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/drop_space.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/drop_space.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/input_dialog.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/input_dialog.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/components/message_box.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/components/message_box.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/layout.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/layout.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/misc.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/helpers/settings.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/af.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/af.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ar.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ar.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/bn-IN.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/bn-IN.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/bn.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/bn.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ca.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ca.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/cs.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/cs.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/da.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/da.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/de-DE.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/de-DE.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/de.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/de.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/el.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/el.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/en.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/en.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/en_US.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/en_US.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/es-ES.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/es-ES.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fa.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fa.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fi.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fi.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/fr.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/fr.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ga-IE.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ga-IE.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/he.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/he.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hi.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hi.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hr.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hr.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hu.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hu.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/hy-AM.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/hy-AM.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/id.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/id.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/it.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/it.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ja.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ja.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ko.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ko.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ms.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ms.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ne-NP.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ne-NP.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/nl.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/nl.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/no.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/no.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pl.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pl.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pt-BR.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pt-BR.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/pt-PT.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/pt-PT.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ro.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ro.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ru.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ru.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sk.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sk.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sl.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sl.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sq.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sq.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sr.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sr.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/sv-SE.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/sv-SE.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/tr-TR.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/tr-TR.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/tr.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/tr.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/uk.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/uk.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/ur-PK.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/ur-PK.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/vi.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/vi.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/zh-CN.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/zh-CN.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/i18n/zh-TW.qm` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/i18n/zh-TW.qm`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/icon.png` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/icon.png`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/xiaomi_flashable_firmware_creator_gui/main.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/xiaomi_flashable_firmware_creator_gui/main.py`

 * *Files identical despite different names*

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/setup.py` & `xiaomi_flashable_firmware_creator_gui-2.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,23 +7,23 @@
  'xiaomi_flashable_firmware_creator_gui.helpers']
 
 package_data = \
 {'': ['*'],
  'xiaomi_flashable_firmware_creator_gui': ['data/settings.json', 'i18n/*']}
 
 install_requires = \
-['PyQt5>=5.13.0,<6.0.0', 'xiaomi_flashable_firmware_creator>=2.2.3,<3.0.0']
+['PyQt5>=5.13.0,<6.0.0', 'xiaomi_flashable_firmware_creator>=2.2.5,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['xiaomi_flashable_firmware_creator_g = '
                      'xiaomi_flashable_firmware_creator_gui.main:main']}
 
 setup_kwargs = {
     'name': 'xiaomi-flashable-firmware-creator-gui',
-    'version': '2.3.8',
+    'version': '2.3.9',
     'description': 'Create flashable firmware zip from MIUI Recovery ROMs!',
     'long_description': '## Xiaomi Flashable Firmware Creator GUI\n\nCreate flashable firmware zip from MIUI Recovery ROMs!\n\n[![Crowdin](https://badges.crowdin.net/mi-flashable-firmware-creator/localized.svg)](https://crowdin.com/project/mi-flashable-firmware-creator)\n\n[![PyPI version](https://badge.fury.io/py/xiaomi-flashable-firmware-creator-gui.svg)](https://pypi.org/project/xiaomi-flashable-firmware-creator-gui/)\n[![made-with-python](https://img.shields.io/badge/Made%20with-Python%203-3776AB?style=flat\\&labelColor=3776AB\\&logo=python\\&logoColor=white\\&link=https://www.python.org/)](https://www.python.org/)\n[![Open Source Love](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](#) <br />\n[![PayPal](https://img.shields.io/badge/PayPal-Donate-00457C?style=flat\\&labelColor=00457C\\&logo=PayPal\\&logoColor=white\\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)\n[![Patreon](https://img.shields.io/badge/Patreon-Support-F96854?style=flat\\&labelColor=F96854\\&logo=Patreon\\&logoColor=white\\&link=https://www.paypal.me/yshalsager)](https://www.paypal.me/yshalsager)\n[![Liberapay](https://img.shields.io/badge/Liberapay-Support-F6C915?style=flat\\&labelColor=F6C915\\&logo=Liberapay\\&logoColor=white\\&link=https://liberapay.com/yshalsager)](https://liberapay.com/yshalsager)\n\nXiaomi Flashable Firmware Creator is a tool that generates flashable firmware-update packages from official MIUI ROMS.\n\nIt supports creating untouched firmware, non-arb firmware, firmware + vendor flashable zip, and firmware-less ROMs.\n[![screenshot](https://raw.githubusercontent.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator-gui/master/screenshots/1.png)](https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/)\n\n### Features:\n\n*   Easy-to-use interface\n*   Multilanguage support (more than 25 languages!). Thanks to our community members!\n\n#### Screenshots:\n\n[Here](https://github.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator-gui/tree/master/screenshots)\n\n### Installation\n\n**Using pip**\nYou can simply install this tool using Python pip.\n\n```shell script\npip install xiaomi_flashable_firmware_creator_gui\n```\n\n**Manual Installation**\n\n*   Clone this repo using `git clone`\n*   Make sure that you have Python3 installed with pip version higher than 19 on your device.\n*   Install the required packages by running the following command in cloned repo folder.\n\n```shell script\npip3 install .\n```\n\n### GUI Usage:\n\n*   Run the tool.\n\n```shell script\nxiaomi_flashable_firmware_creator_g\n```\n',
     'author': 'yshalsager',
     'author_email': 'ysh-alsager@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/',
```

### Comparing `xiaomi_flashable_firmware_creator_gui-2.3.8/PKG-INFO` & `xiaomi_flashable_firmware_creator_gui-2.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: xiaomi-flashable-firmware-creator-gui
-Version: 2.3.8
+Version: 2.3.9
 Summary: Create flashable firmware zip from MIUI Recovery ROMs!
 Home-page: https://xiaomifirmwareupdater.com/projects/xiaomi-flashable-firmware-creator/
 License: GPL-3.0-only
 Keywords: xiaomi,firmware,android
 Author: yshalsager
 Author-email: ysh-alsager@hotmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyQt5 (>=5.13.0,<6.0.0)
-Requires-Dist: xiaomi_flashable_firmware_creator (>=2.2.3,<3.0.0)
+Requires-Dist: xiaomi_flashable_firmware_creator (>=2.2.5,<3.0.0)
 Project-URL: Repository, https://github.com/XiaomiFirmwareUpdater/xiaomi-flashable-firmware-creator-gui/
 Description-Content-Type: text/markdown
 
 ## Xiaomi Flashable Firmware Creator GUI
 
 Create flashable firmware zip from MIUI Recovery ROMs!
```

