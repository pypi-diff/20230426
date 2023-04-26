# Comparing `tmp/Products.MeetingSeraing-4.2.0b4.tar.gz` & `tmp/Products.MeetingSeraing-4.2.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Products.MeetingSeraing-4.2.0b4.tar", last modified: Wed Apr 26 09:39:26 2023, max compression
+gzip compressed data, was "Products.MeetingSeraing-4.2.0b5.tar", last modified: Wed Apr 26 10:04:06 2023, max compression
```

## Comparing `Products.MeetingSeraing-4.2.0b4.tar` & `Products.MeetingSeraing-4.2.0b5.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/
--rw-rw-r--   0 adu       (1000) adu       (1000)     7387 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/CHANGES.rst
--rw-rw-r--   0 adu       (1000) adu       (1000)      679 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/MANIFEST.in
--rw-rw-r--   0 adu       (1000) adu       (1000)     8067 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)      153 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/README.rst
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/docs/
--rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/docs/LICENSE.GPL
--rw-rw-r--   0 adu       (1000) adu       (1000)      733 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/docs/LICENSE.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/setup.cfg
--rw-rw-r--   0 adu       (1000) adu       (1000)     1413 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/setup.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/Products/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/Extensions/
--rw-rw-r--   0 adu       (1000) adu       (1000)       26 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/Extensions/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      967 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/README.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1762 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)    56353 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/adapters.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/
--rw-rw-r--   0 adu       (1000) adu       (1000)       22 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      183 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)      391 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/messages.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1259 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/overrides.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2055 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/viewlets.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     2719 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/config.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3868 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/configure.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     4931 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/ecolsanit.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     4443 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/events.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1047 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/events.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)     5032 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/interfaces.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/
--rw-rw-r--   0 adu       (1000) adu       (1000)     7937 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/PloneMeeting.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)      728 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/datagridfield.pot
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 adu       (1000) adu       (1000)    11699 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/PloneMeeting.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     1051 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/datagridfield.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     5951 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.actionspanel.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     2397 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.history.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     8045 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/plone.po
--rw-rw-r--   0 adu       (1000) adu       (1000)     3904 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/imio.actionspanel.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     1721 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/imio.history.pot
--rw-rw-r--   0 adu       (1000) adu       (1000)     6814 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/plone.pot
--rwxrwxr-x   0 adu       (1000) adu       (1000)      309 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/sync_pos.sh
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     7239 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/migrate_to_4200.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      980 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/migrate_to_4_1.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/model/
--rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/model/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     5924 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/model/pm_updates.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      641 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/overrides.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/
--rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/MeetingSeraing_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      719 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/cssregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      773 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/jsregistry.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      245 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/metadata.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      576 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/rolemap.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      914 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/skins.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    86403 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/definition.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.647364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/
--rw-rw-r--   0 adu       (1000) adu       (1000)    13415 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/definition.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      734 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.651363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/MeetingSeraing_seraing_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.651363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/legalAdvice.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/nil.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/remarks.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/secretary_remarks.png
--rwxrwxr-x   0 adu       (1000) adu       (1000)     5696 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      623 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/import_steps.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.651363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)    24652 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/deliberation.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    17866 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/oj.odt
--rw-rw-r--   0 adu       (1000) adu       (1000)    18359 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/pv.odt
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/toolset.xml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.651363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/
--rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/MeetingSeraing_seraing_marker.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.651363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/
--rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/attach.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/budget.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/budgetAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/cahier.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/decisionAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/financialAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/itemAnnex.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/legalAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/negative.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/nil.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/overheadAnalysis.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/positive.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/remarks.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/secretary_remarks.png
--rwxrwxr-x   0 adu       (1000) adu       (1000)     4617 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/import_data.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)      579 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/import_steps.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)      173 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/metadata.xml
--rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/toolset.xml
--rw-rw-r--   0 adu       (1000) adu       (1000)     1512 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles.zcml
--rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/refresh.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)     5540 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/setuphandlers.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/
--rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_cautious_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_negative_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      465 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_given_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_required_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      740 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      697 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_with_remarks_finance.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      339 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/ask_advices_by_itemcreator.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAccepted.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAcceptedButModified.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      664 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemCreated.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemDelayed.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCommittee.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCouncil.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1041 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDG.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDGA.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToPresented.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDirector.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDivisionHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToOfficeManager.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToServiceHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1041 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToValidatedByDG.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_itemfrozen_from_returned_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_presented_from_returned_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_returned_to_proposing_group_from_returned_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_proposing_group.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      788 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/itemValidateByDG.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      821 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_committee.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      833 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_council.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1082 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.gif
--rw-rw-r--   0 adu       (1000) adu       (1000)      830 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.png
--rw-rw-r--   0 adu       (1000) adu       (1000)     1035 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/printed_in_dashboard.gif
--rw-rw-r--   0 adu       (1000) adu       (1000)      737 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToBudgetImpactReviewer.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      613 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDirector.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDivisionHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      608 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToOfficeManager.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      638 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToServiceHead.png
--rw-rw-r--   0 adu       (1000) adu       (1000)    48637 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/remove.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      213 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/removed.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      512 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      893 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_service.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      512 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/returned_to_advise.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      797 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/toPrint.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      695 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/validate.png
--rw-rw-r--   0 adu       (1000) adu       (1000)      718 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/validateByBudgetImpactReviewer.png
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/
--rw-rw-r--   0 adu       (1000) adu       (1000)    20208 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meeting_edit.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     9692 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_edit.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)    41032 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_view.pt
--rw-rw-r--   0 adu       (1000) adu       (1000)     1360 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/testing.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      603 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/testing.zcml
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.659364 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/
--rwxrwxr-x   0 adu       (1000) adu       (1000)     3984 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/MeetingSeraingTestCase.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1049 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/__init__.py
--rw-rw-r--   0 adu       (1000) adu       (1000)      873 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/dot.gif
--rw-rw-r--   0 adu       (1000) adu       (1000)     4431 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/helpers.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1363 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testAdvices.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1229 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testAnnexes.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1332 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testChangeItemOrderView.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1527 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testColumns.py
--rw-rw-r--   0 adu       (1000) adu       (1000)    14457 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testCustomMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     6296 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testCustomWorkflows.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1258 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testFaceted.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1284 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1309 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingCategory.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     8489 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingConfig.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)    17244 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingItem.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1271 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testPortlets.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     3450 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testSearches.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1262 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testSetup.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1316 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testToolPloneMeeting.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1381 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testUtils.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1274 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testValidators.py
--rw-rw-r--   0 adu       (1000) adu       (1000)     1220 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testViews.py
--rw-rw-r--   0 adu       (1000) adu       (1000)    16081 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testWFAdaptations.py
--rwxrwxr-x   0 adu       (1000) adu       (1000)    13042 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testWorkflows.py
--rw-rw-r--   0 adu       (1000) adu       (1000)       10 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/version.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products/__init__.py
-drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 09:39:26.643363 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/
--rw-rw-r--   0 adu       (1000) adu       (1000)     8067 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/PKG-INFO
--rw-rw-r--   0 adu       (1000) adu       (1000)    11325 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/SOURCES.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/dependency_links.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/namespace_packages.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/not-zip-safe
--rw-rw-r--   0 adu       (1000) adu       (1000)      284 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/requires.txt
--rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-04-26 09:39:26.000000 Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/top_level.txt
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.975629 Products.MeetingSeraing-4.2.0b5/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7535 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/CHANGES.rst
+-rw-rw-r--   0 adu       (1000) adu       (1000)      679 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/MANIFEST.in
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8215 2023-04-26 10:04:06.975629 Products.MeetingSeraing-4.2.0b5/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)      153 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/README.rst
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/docs/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18092 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/docs/LICENSE.GPL
+-rw-rw-r--   0 adu       (1000) adu       (1000)      733 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/docs/LICENSE.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)       38 2023-04-26 10:04:06.975629 Products.MeetingSeraing-4.2.0b5/setup.cfg
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1413 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/setup.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.955629 Products.MeetingSeraing-4.2.0b5/src/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/Extensions/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       26 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/Extensions/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      967 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/README.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1762 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    59066 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/adapters.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       22 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      183 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      391 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/messages.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1259 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/overrides.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2055 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/viewlets.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2719 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/config.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3868 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/configure.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4931 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/ecolsanit.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4443 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/events.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1047 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/events.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5032 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/interfaces.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7937 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/PloneMeeting.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)      728 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/datagridfield.pot
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.955629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    11699 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/PloneMeeting.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1051 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/datagridfield.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5951 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.actionspanel.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     2397 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.history.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8045 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/plone.po
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3904 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/imio.actionspanel.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1721 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/imio.history.pot
+-rw-rw-r--   0 adu       (1000) adu       (1000)     6814 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/plone.pot
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      309 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/sync_pos.sh
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     7239 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/migrate_to_4200.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      980 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/migrate_to_4_1.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/model/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/model/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5924 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/model/pm_updates.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      641 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/overrides.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/
+-rw-rw-r--   0 adu       (1000) adu       (1000)       23 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/MeetingSeraing_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      719 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/cssregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      773 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      423 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/jsregistry.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      245 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/metadata.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      576 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/rolemap.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      914 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/skins.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      167 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/toolset.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.955629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    86403 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/definition.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    13415 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/definition.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      734 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/MeetingSeraing_seraing_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.963629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      761 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/legalAdvice.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      885 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/nil.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/remarks.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/secretary_remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     5696 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      623 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/import_steps.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.967629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    24652 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/deliberation.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    17866 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/oj.odt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    18359 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/pv.odt
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/toolset.xml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.967629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      177 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/MeetingSeraing_seraing_marker.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.967629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3352 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/attach.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/budget.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      492 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/budgetAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      731 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/cahier.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/decisionAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      742 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/financialAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      216 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/itemAnnex.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      332 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/legalAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      411 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/negative.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      305 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/nil.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      880 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/overheadAnalysis.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1147 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/positive.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      355 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/remarks.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      730 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/secretary_remarks.png
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     4617 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/import_data.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      579 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/import_steps.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)      173 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/metadata.xml
+-rwxrwxr-x   0 adu       (1000) adu       (1000)      167 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/toolset.xml
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1512 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles.zcml
+-rw-rw-r--   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/refresh.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5540 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/setuphandlers.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.955629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.971629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/
+-rw-rw-r--   0 adu       (1000) adu       (1000)      680 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_cautious_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      630 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_negative_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      465 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_given_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      708 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_required_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      740 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      697 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_with_remarks_finance.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      339 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/ask_advices_by_itemcreator.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAccepted.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAcceptedButModified.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      664 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemCreated.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     5585 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemDelayed.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCommittee.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCouncil.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1041 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDG.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDGA.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToPresented.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDirector.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDivisionHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToOfficeManager.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToServiceHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1041 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToValidatedByDG.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_itemfrozen_from_returned_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_presented_from_returned_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_returned_to_proposing_group_from_returned_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      649 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_proposing_group.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      788 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/itemValidateByDG.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      821 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_committee.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      833 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_council.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1082 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      830 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1035 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/printed_in_dashboard.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)      737 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToBudgetImpactReviewer.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      613 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDirector.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      626 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDivisionHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      608 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToOfficeManager.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      638 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToServiceHead.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)    48637 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/remove.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      213 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/removed.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      512 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      893 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_service.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      512 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/returned_to_advise.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      797 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/toPrint.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      695 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/validate.png
+-rw-rw-r--   0 adu       (1000) adu       (1000)      718 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/validateByBudgetImpactReviewer.png
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.971629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/
+-rw-rw-r--   0 adu       (1000) adu       (1000)    20208 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meeting_edit.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     9692 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_edit.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)    41032 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_view.pt
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1360 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/testing.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      603 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/testing.zcml
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.975629 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/
+-rwxrwxr-x   0 adu       (1000) adu       (1000)     3984 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/MeetingSeraingTestCase.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1049 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/__init__.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)      873 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/dot.gif
+-rw-rw-r--   0 adu       (1000) adu       (1000)     4431 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/helpers.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1363 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testAdvices.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1229 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testAnnexes.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1332 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testChangeItemOrderView.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1527 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testColumns.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    14457 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testCustomMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     6296 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testCustomWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1258 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testFaceted.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1284 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1309 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingCategory.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8489 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingConfig.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    17244 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingItem.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1271 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testPortlets.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     3450 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testSearches.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1262 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testSetup.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1316 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testToolPloneMeeting.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1381 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testUtils.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1274 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testValidators.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)     1220 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testViews.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)    16081 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testWFAdaptations.py
+-rwxrwxr-x   0 adu       (1000) adu       (1000)    13042 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testWorkflows.py
+-rw-rw-r--   0 adu       (1000) adu       (1000)       10 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/version.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)       56 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products/__init__.py
+drwxrwxr-x   0 adu       (1000) adu       (1000)        0 2023-04-26 10:04:06.959629 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/
+-rw-rw-r--   0 adu       (1000) adu       (1000)     8215 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/PKG-INFO
+-rw-rw-r--   0 adu       (1000) adu       (1000)    11325 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/SOURCES.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/dependency_links.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        1 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/not-zip-safe
+-rw-rw-r--   0 adu       (1000) adu       (1000)      284 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/requires.txt
+-rw-rw-r--   0 adu       (1000) adu       (1000)        9 2023-04-26 10:04:06.000000 Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/top_level.txt
```

### Comparing `Products.MeetingSeraing-4.2.0b4/CHANGES.rst` & `Products.MeetingSeraing-4.2.0b5/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Products.MeetingSeraing Changelog
 =================================
 
+4.2.0b5 (2023-04-26)
+--------------------
+
+- Restore mayBackToMeeting and adapt it to use CUSTOM_RETURN_TO_PROPOSING_GROUP_MAPPINGS.
+  [aduchene]
+
+
 4.2.0b4 (2023-04-26)
 --------------------
 
 - Remove mayBackToMeeting as it is now useless.
   [aduchene]
 
 4.2.0b3 (2023-03-30)
```

### Comparing `Products.MeetingSeraing-4.2.0b4/MANIFEST.in` & `Products.MeetingSeraing-4.2.0b5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/PKG-INFO` & `Products.MeetingSeraing-4.2.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingSeraing
-Version: 4.2.0b4
+Version: 4.2.0b5
 Summary: PloneMeeting profile for city of Seraing
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -20,14 +20,21 @@
 ========================
 
 'Products.MeetingSeraing' is a custom profile for 'Products.MeetingCommunes'.
 
 Products.MeetingSeraing Changelog
 =================================
 
+4.2.0b5 (2023-04-26)
+--------------------
+
+- Restore mayBackToMeeting and adapt it to use CUSTOM_RETURN_TO_PROPOSING_GROUP_MAPPINGS.
+  [aduchene]
+
+
 4.2.0b4 (2023-04-26)
 --------------------
 
 - Remove mayBackToMeeting as it is now useless.
   [aduchene]
 
 4.2.0b3 (2023-03-30)
```

### Comparing `Products.MeetingSeraing-4.2.0b4/docs/LICENSE.GPL` & `Products.MeetingSeraing-4.2.0b5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/docs/LICENSE.txt` & `Products.MeetingSeraing-4.2.0b5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/setup.py` & `Products.MeetingSeraing-4.2.0b5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '4.2.0b4'
+version = '4.2.0b5'
 
 setup(
     name='Products.MeetingSeraing',
     version=version,
     description="PloneMeeting profile for city of Seraing",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/README.txt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/README.txt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/__init__.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/adapters.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/adapters.py`

 * *Files 3% similar despite different names*

```diff
@@ -998,14 +998,56 @@
 
     def mayProposeToDivisionHead(self):
         """
         Check that the user has the 'Review portal content'
         """
         return _checkPermission(ReviewPortalContent, self.context)
 
+    security.declarePublic("mayBackToMeeting")
+
+    def mayBackToMeeting(self, transitionName):
+        """Specific guard for the 'return_to_proposing_group' wfAdaptation.
+           As we have only one guard_expr for potentially several transitions departing
+           from the 'returned_to_proposing_group' state, we receive the p_transitionName."""
+        if not _checkPermission(ReviewPortalContent, self.context) and not \
+           self.tool.isManager(self.cfg):
+            return
+        # when using validation states, may return when in last validation state
+        if 'return_to_proposing_group' not in self.cfg.getWorkflowAdaptations():
+            current_validation_state = 'itemcreated' \
+                if self.review_state == 'returned_to_proposing_group' \
+                else self.review_state.replace('returned_to_proposing_group_', '')
+            last_val_state = self._getLastValidationState()
+            # we are in last validation state, or we are in state 'returned_to_proposing_group'
+            # and there is no last validation state, aka it is "itemcreated"
+            if current_validation_state != last_val_state:
+                return
+        # get the linked meeting
+        meeting = self.context.getMeeting()
+        meetingState = meeting.query_state()
+        # use RETURN_TO_PROPOSING_GROUP_MAPPINGS to know in wich meetingStates
+        # the given p_transitionName can be triggered
+        authorizedMeetingStates = CUSTOM_RETURN_TO_PROPOSING_GROUP_MAPPINGS[transitionName]
+        if meetingState in authorizedMeetingStates:
+            return True
+        # if we did not return True, then return a No(...) message specifying that
+        # it can no more be returned to the meeting because the meeting is in some
+        # specific states (like 'closed' for example)
+        if meetingState in CUSTOM_RETURN_TO_PROPOSING_GROUP_MAPPINGS['NO_MORE_RETURNABLE_STATES']:
+            # avoid to display No(...) message for each transition having the 'mayBackToMeeting'
+            # guard expr, just return the No(...) msg for the first transitionName checking this...
+            if 'may_not_back_to_meeting_warned_by' not in self.context.REQUEST:
+                self.context.REQUEST.set('may_not_back_to_meeting_warned_by', transitionName)
+            if self.context.REQUEST.get('may_not_back_to_meeting_warned_by') == transitionName:
+                return No(_('can_not_return_to_meeting_because_of_meeting_state',
+                            mapping={'meetingState': translate(
+                                meetingState,
+                                domain='plone',
+                                context=self.context.REQUEST)}))
+        return False
     security.declarePublic("mayClose")
 
     def mayClose(self):
         """
         Check that the user has the 'Review portal content' and meeting is closed (for automatic transitions)
         """
         res = False
```

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/overrides.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/overrides.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/browser/viewlets.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/config.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/config.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/configure.zcml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/configure.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/ecolsanit.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/ecolsanit.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/events.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/events.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/events.zcml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/events.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/interfaces.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/interfaces.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/PloneMeeting.pot` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/PloneMeeting.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/datagridfield.pot` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/datagridfield.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/PloneMeeting.po` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/PloneMeeting.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/datagridfield.po` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/datagridfield.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.actionspanel.po` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.actionspanel.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.history.po` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/imio.history.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/plone.po` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/imio.actionspanel.pot` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/imio.actionspanel.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/imio.history.pot` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/imio.history.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/locales/plone.pot` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/migrate_to_4200.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/migrate_to_4200.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/migrations/migrate_to_4_1.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/migrations/migrate_to_4_1.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/model/pm_updates.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/model/pm_updates.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/overrides.zcml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/overrides.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/cssregistry.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/cssregistry.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/import_steps.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/rolemap.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/rolemap.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/skins.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/skins.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/definition.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingitemseraing_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/definition.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows/meetingseraing_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/default/workflows.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/default/workflows.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/attach.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/budget.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/cahier.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/financialAnalysis.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/legalAdvice.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/legalAdvice.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/negative.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/negative.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/overheadAnalysis.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/positive.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/images/secretary_remarks.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/import_data.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/import_steps.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/deliberation.odt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/deliberation.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/oj.odt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/oj.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/seraing/templates/pv.odt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/seraing/templates/pv.odt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/attach.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/attach.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/budget.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/budget.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/cahier.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/cahier.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/financialAnalysis.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/financialAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/overheadAnalysis.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/overheadAnalysis.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/positive.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/positive.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/images/secretary_remarks.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/images/secretary_remarks.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/import_data.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/import_data.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles/testing/import_steps.xml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles/testing/import_steps.xml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/profiles.zcml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/profiles.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/setuphandlers.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_cautious_finance.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_cautious_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_negative_finance.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_negative_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_required_finance.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_not_required_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_finance.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_with_remarks_finance.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/advice_standard_positive_with_remarks_finance.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAccepted.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAccepted.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAcceptedButModified.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemAcceptedButModified.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemCreated.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemCreated.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemDelayed.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemDelayed.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCommittee.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCommittee.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCouncil.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemInCouncil.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDG.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDG.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDGA.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToItemValidatedByDGA.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToPresented.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToPresented.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDirector.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDivisionHead.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToOfficeManager.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToServiceHead.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToProposedToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backToValidatedByDG.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backToValidatedByDG.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_itemfrozen_from_returned_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_itemfrozen_from_returned_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_presented_from_returned_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_presented_from_returned_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_returned_to_proposing_group_from_returned_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_returned_to_proposing_group_from_returned_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_proposing_group.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/backTo_validated_by_dg_from_returned_to_proposing_group.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/itemValidateByDG.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/itemValidateByDG.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_committee.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_committee.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_council.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/item_in_council.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.gif` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/not_printed_in_dashboard.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/printed_in_dashboard.gif` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/printed_in_dashboard.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToBudgetImpactReviewer.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDirector.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDirector.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDivisionHead.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToDivisionHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToOfficeManager.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToOfficeManager.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToServiceHead.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/proposeToServiceHead.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/remove.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/remove.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_service.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/return_to_service.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/returned_to_advise.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/returned_to_advise.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/toPrint.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/toPrint.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/validate.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/validate.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_images/validateByBudgetImpactReviewer.png` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_images/validateByBudgetImpactReviewer.png`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meeting_edit.pt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meeting_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_edit.pt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_edit.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_view.pt` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/skins/meetingseraing_templates/meetingitem_view.pt`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/testing.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/testing.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/testing.zcml` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/testing.zcml`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/MeetingSeraingTestCase.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/MeetingSeraingTestCase.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/__init__.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/dot.gif` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/dot.gif`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/helpers.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testAdvices.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testAdvices.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testAnnexes.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testAnnexes.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testChangeItemOrderView.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testChangeItemOrderView.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testColumns.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testColumns.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testCustomMeetingItem.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testCustomMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testCustomWorkflows.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testCustomWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testFaceted.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testFaceted.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeeting.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingCategory.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingCategory.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingConfig.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingConfig.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testMeetingItem.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testMeetingItem.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testPortlets.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testPortlets.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testSearches.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testSearches.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testSetup.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testSetup.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testToolPloneMeeting.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testToolPloneMeeting.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testUtils.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testValidators.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testValidators.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testViews.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testViews.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testWFAdaptations.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testWFAdaptations.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products/MeetingSeraing/tests/testWorkflows.py` & `Products.MeetingSeraing-4.2.0b5/src/Products/MeetingSeraing/tests/testWorkflows.py`

 * *Files identical despite different names*

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/PKG-INFO` & `Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Products.MeetingSeraing
-Version: 4.2.0b4
+Version: 4.2.0b5
 Summary: PloneMeeting profile for city of Seraing
 Home-page: http://www.imio.be/produits/gestion-des-deliberations
 Author: Andre Nuyens
 Author-email: andre.nuyens@imio.be
 License: GPL
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -20,14 +20,21 @@
 ========================
 
 'Products.MeetingSeraing' is a custom profile for 'Products.MeetingCommunes'.
 
 Products.MeetingSeraing Changelog
 =================================
 
+4.2.0b5 (2023-04-26)
+--------------------
+
+- Restore mayBackToMeeting and adapt it to use CUSTOM_RETURN_TO_PROPOSING_GROUP_MAPPINGS.
+  [aduchene]
+
+
 4.2.0b4 (2023-04-26)
 --------------------
 
 - Remove mayBackToMeeting as it is now useless.
   [aduchene]
 
 4.2.0b3 (2023-03-30)
```

### Comparing `Products.MeetingSeraing-4.2.0b4/src/Products.MeetingSeraing.egg-info/SOURCES.txt` & `Products.MeetingSeraing-4.2.0b5/src/Products.MeetingSeraing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

