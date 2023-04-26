# Comparing `tmp/djangocms-frontend-1.1.1.tar.gz` & `tmp/djangocms-frontend-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.1.1.tar", last modified: Tue Apr 18 21:10:50 2023, max compression
+gzip compressed data, was "djangocms-frontend-1.1.2.tar", last modified: Tue Apr 25 21:55:50 2023, max compression
```

## Comparing `djangocms-frontend-1.1.1.tar` & `djangocms-frontend-1.1.2.tar`

### file list

```diff
@@ -1,686 +1,686 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.705317 djangocms-frontend-1.1.1/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.705317 djangocms-frontend-1.1.1/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.705317 djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.705317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.685317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.685317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.685317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.685317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.709317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.689317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.713317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.717317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.721317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.721317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.721317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.721317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.721317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.737318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.741318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    41317 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    26139 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.745318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.745318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    20843 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.745318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.693317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.749318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.753318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.757318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.697317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.761318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.765318 djangocms-frontend-1.1.1/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.701317 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)    93442 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/div_select.css
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.705317 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 21:10:50.000000 djangocms-frontend-1.1.1/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-18 21:10:50.781318 djangocms-frontend-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.769318 djangocms-frontend-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.773318 djangocms-frontend-1.1.1/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/link/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:50.777318 djangocms-frontend-1.1.1/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-18 21:10:42.000000 djangocms-frontend-1.1.1/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.699537 djangocms-frontend-1.1.2/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.703537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.707537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.711537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.711537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.715537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.679537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.719537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.723538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.727537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.731537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.735538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.735538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.683537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.755538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.763538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.771538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.775538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.687537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.779538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.783538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.787538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.787538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.791538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.795538 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.691537 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.799538 djangocms-frontend-1.1.2/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.695537 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    93523 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.803538 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.807539 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.699537 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 21:55:50.000000 djangocms-frontend-1.1.2/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.811539 djangocms-frontend-1.1.2/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/link/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.815539 djangocms-frontend-1.1.2/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:50.819539 djangocms-frontend-1.1.2/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-25 21:55:37.000000 djangocms-frontend-1.1.2/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.1.1/LICENSE` & `djangocms-frontend-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/PKG-INFO` & `djangocms-frontend-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.1
+Version: 1.1.2
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -40,14 +40,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: djangocms-icon
 Provides-Extra: static-ace
+Provides-Extra: cms-4
+Provides-Extra: cms-3
 License-File: LICENSE
 
 #####################
  django CMS Frontend
 #####################
 
 |pypi| |docs| |coverage| |python| |django| |djangocms| |djangocms4|
@@ -208,15 +210,15 @@
 
 .. |coverage| image:: https://codecov.io/gh/fsbraun/djangocms-frontend/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/django-cms/djangocms-frontend
 
 .. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://pypi.org/project/djangocms-frontend/
 
-.. |django| image:: https://img.shields.io/badge/django-3.2--4.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2--4.2-blue.svg
    :target: https://www.djangoproject.com/
 
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.8%2B-blue.svg
    :target: https://www.django-cms.org/
 
 .. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
    :target: https://www.django-cms.org/en/preview-django-cms-40/
```

### Comparing `djangocms-frontend-1.1.1/README.rst` & `djangocms-frontend-1.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 .. |coverage| image:: https://codecov.io/gh/fsbraun/djangocms-frontend/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/django-cms/djangocms-frontend
 
 .. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://pypi.org/project/djangocms-frontend/
 
-.. |django| image:: https://img.shields.io/badge/django-3.2--4.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2--4.2-blue.svg
    :target: https://www.djangoproject.com/
 
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.8%2B-blue.svg
    :target: https://www.django-cms.org/
 
 .. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
    :target: https://www.django-cms.org/en/preview-django-cms-40/
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/__init__.py` & `djangocms-frontend-1.1.2/djangocms_frontend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/attributes.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/background.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/spacing.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/common/title.py` & `djangocms-frontend-1.1.2/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/constants.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/constants.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/constants.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/conf.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 
+VENDOR_PATH = "djangocms_frontend/icon/vendor/assets"
+
 ICON_CDN = {
-    "bootstrap-icons": "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.3/font/bootstrap-icons.css",
+    "bootstrap-icons": "https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css",
     "font-awesome": "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css",
     "material-icons-filled": "https://fonts.googleapis.com/css2?family=Material+Icons",
     "material-icons-outlined": "https://fonts.googleapis.com/css2?family=Material+Icons+Outlined",
     "material-icons-round": "https://fonts.googleapis.com/css2?family=Material+Icons+Round",
     "material-icons-sharp": "https://fonts.googleapis.com/css2?family=Material+Icons+Sharp",
     "material-icons-two-tone": "https://fonts.googleapis.com/css2?family=Material+Icons+Two+Tone",
     "fomantic-ui": "fomantic-ui-icons.css",
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,10 +13,10 @@
                 instance.add_classes(size)
         if instance.config.get("icon_foreground", None):
             instance.add_classes(f"text-{instance.icon_foreground}")
         if instance.config.get("icon_rounded", False):
             instance.add_classes("text-center", "rounded", "rounded-circle")
             instance.add_attribute(
                 "style",
-                "display:inline-block;line-height:1.42em;height:1.42em;width:1.42em;",
+                "display:inline-block;line-height:1.49em;height:1.42em;width:1.42em;",
             )
         return super().render(context, instance, placeholder)
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7285714285714285%*

 * *Differences: {"'icons'": "{insert: [(0, '0-circle'), (1, '0-circle-fill'), (2, '0-square'), (3, "*

 * *            "'0-square-fill'), (4, '1-circle'), (5, '1-circle-fill'), (6, '1-square'), (7, "*

 * *            "'1-square-fill'), (9, '2-circle'), (10, '2-circle-fill'), (11, '2-square'), (12, "*

 * *            "'2-square-fill'), (13, '3-circle'), (14, '3-circle-fill'), (15, '3-square'), (16, "*

 * *            "'3-square-fill'), (17, '4-circle'), (18, '4-circle-fill'), (19, '4-square'), (20, "*

 * *            "'4-square-fill'), (21, '5-circl […]*

```diff
@@ -1,381 +1,518 @@
 {
     "icon-style": "bi",
     "icons": [
+        "0-circle",
+        "0-circle-fill",
+        "0-square",
+        "0-square-fill",
+        "1-circle",
+        "1-circle-fill",
+        "1-square",
+        "1-square-fill",
         "123",
-        "alarm-fill",
+        "2-circle",
+        "2-circle-fill",
+        "2-square",
+        "2-square-fill",
+        "3-circle",
+        "3-circle-fill",
+        "3-square",
+        "3-square-fill",
+        "4-circle",
+        "4-circle-fill",
+        "4-square",
+        "4-square-fill",
+        "5-circle",
+        "5-circle-fill",
+        "5-square",
+        "5-square-fill",
+        "6-circle",
+        "6-circle-fill",
+        "6-square",
+        "6-square-fill",
+        "7-circle",
+        "7-circle-fill",
+        "7-square",
+        "7-square-fill",
+        "8-circle",
+        "8-circle-fill",
+        "8-square",
+        "8-square-fill",
+        "9-circle",
+        "9-circle-fill",
+        "9-square",
+        "9-square-fill",
+        "activity",
+        "airplane",
+        "airplane-engines",
+        "airplane-engines-fill",
+        "airplane-fill",
         "alarm",
+        "alarm-fill",
+        "alexa",
         "align-bottom",
         "align-center",
         "align-end",
         "align-middle",
         "align-start",
         "align-top",
+        "alipay",
         "alt",
-        "app-indicator",
+        "amd",
+        "android",
+        "android2",
         "app",
-        "archive-fill",
+        "app-indicator",
+        "apple",
         "archive",
+        "archive-fill",
         "arrow-90deg-down",
         "arrow-90deg-left",
         "arrow-90deg-right",
         "arrow-90deg-up",
         "arrow-bar-down",
         "arrow-bar-left",
         "arrow-bar-right",
         "arrow-bar-up",
         "arrow-clockwise",
         "arrow-counterclockwise",
-        "arrow-down-circle-fill",
+        "arrow-down",
         "arrow-down-circle",
-        "arrow-down-left-circle-fill",
+        "arrow-down-circle-fill",
         "arrow-down-left-circle",
-        "arrow-down-left-square-fill",
+        "arrow-down-left-circle-fill",
         "arrow-down-left-square",
-        "arrow-down-left",
-        "arrow-down-right-circle-fill",
+        "arrow-down-left-square-fill",
         "arrow-down-right-circle",
-        "arrow-down-right-square-fill",
+        "arrow-down-right-circle-fill",
         "arrow-down-right-square",
+        "arrow-down-right-square-fill",
+        "arrow-down-square",
+        "arrow-down-square-fill",
+        "arrow-down-left",
         "arrow-down-right",
         "arrow-down-short",
-        "arrow-down-square-fill",
-        "arrow-down-square",
         "arrow-down-up",
-        "arrow-down",
-        "arrow-left-circle-fill",
+        "arrow-left",
         "arrow-left-circle",
+        "arrow-left-circle-fill",
+        "arrow-left-square",
+        "arrow-left-square-fill",
         "arrow-left-right",
         "arrow-left-short",
-        "arrow-left-square-fill",
-        "arrow-left-square",
-        "arrow-left",
         "arrow-repeat",
         "arrow-return-left",
         "arrow-return-right",
-        "arrow-right-circle-fill",
+        "arrow-right",
         "arrow-right-circle",
-        "arrow-right-short",
-        "arrow-right-square-fill",
+        "arrow-right-circle-fill",
         "arrow-right-square",
-        "arrow-right",
-        "arrow-up-circle-fill",
+        "arrow-right-square-fill",
+        "arrow-right-short",
+        "arrow-through-heart",
+        "arrow-through-heart-fill",
+        "arrow-up",
         "arrow-up-circle",
-        "arrow-up-left-circle-fill",
+        "arrow-up-circle-fill",
         "arrow-up-left-circle",
-        "arrow-up-left-square-fill",
+        "arrow-up-left-circle-fill",
         "arrow-up-left-square",
-        "arrow-up-left",
-        "arrow-up-right-circle-fill",
+        "arrow-up-left-square-fill",
         "arrow-up-right-circle",
-        "arrow-up-right-square-fill",
+        "arrow-up-right-circle-fill",
         "arrow-up-right-square",
+        "arrow-up-right-square-fill",
+        "arrow-up-square",
+        "arrow-up-square-fill",
+        "arrow-up-left",
         "arrow-up-right",
         "arrow-up-short",
-        "arrow-up-square-fill",
-        "arrow-up-square",
-        "arrow-up",
         "arrows-angle-contract",
         "arrows-angle-expand",
         "arrows-collapse",
         "arrows-expand",
         "arrows-fullscreen",
         "arrows-move",
-        "aspect-ratio-fill",
         "aspect-ratio",
+        "aspect-ratio-fill",
         "asterisk",
         "at",
-        "award-fill",
         "award",
+        "award-fill",
         "back",
+        "backspace",
         "backspace-fill",
-        "backspace-reverse-fill",
         "backspace-reverse",
-        "backspace",
-        "badge-3d-fill",
+        "backspace-reverse-fill",
         "badge-3d",
-        "badge-4k-fill",
+        "badge-3d-fill",
         "badge-4k",
-        "badge-8k-fill",
+        "badge-4k-fill",
         "badge-8k",
-        "badge-ad-fill",
+        "badge-8k-fill",
         "badge-ad",
-        "badge-ar-fill",
+        "badge-ad-fill",
         "badge-ar",
-        "badge-cc-fill",
+        "badge-ar-fill",
         "badge-cc",
-        "badge-hd-fill",
+        "badge-cc-fill",
         "badge-hd",
-        "badge-tm-fill",
+        "badge-hd-fill",
+        "badge-sd",
+        "badge-sd-fill",
         "badge-tm",
-        "badge-vo-fill",
+        "badge-tm-fill",
         "badge-vo",
-        "badge-vr-fill",
+        "badge-vo-fill",
         "badge-vr",
-        "badge-wc-fill",
+        "badge-vr-fill",
         "badge-wc",
-        "bag-check-fill",
+        "badge-wc-fill",
+        "bag",
         "bag-check",
-        "bag-dash-fill",
+        "bag-check-fill",
         "bag-dash",
+        "bag-dash-fill",
         "bag-fill",
-        "bag-plus-fill",
+        "bag-heart",
+        "bag-heart-fill",
         "bag-plus",
-        "bag-x-fill",
+        "bag-plus-fill",
         "bag-x",
-        "bag",
+        "bag-x-fill",
+        "balloon",
+        "balloon-fill",
+        "balloon-heart",
+        "balloon-heart-fill",
+        "bandaid",
+        "bandaid-fill",
+        "bank",
+        "bank2",
+        "bar-chart",
         "bar-chart-fill",
-        "bar-chart-line-fill",
         "bar-chart-line",
+        "bar-chart-line-fill",
         "bar-chart-steps",
-        "bar-chart",
-        "basket-fill",
         "basket",
-        "basket2-fill",
+        "basket-fill",
         "basket2",
-        "basket3-fill",
+        "basket2-fill",
         "basket3",
+        "basket3-fill",
+        "battery",
         "battery-charging",
         "battery-full",
         "battery-half",
-        "battery",
-        "bell-fill",
+        "behance",
         "bell",
+        "bell-fill",
+        "bell-slash",
+        "bell-slash-fill",
         "bezier",
         "bezier2",
         "bicycle",
-        "binoculars-fill",
         "binoculars",
+        "binoculars-fill",
         "blockquote-left",
         "blockquote-right",
+        "bluetooth",
+        "body-text",
+        "book",
         "book-fill",
         "book-half",
-        "book",
-        "bookmark-check-fill",
+        "bookmark",
         "bookmark-check",
-        "bookmark-dash-fill",
+        "bookmark-check-fill",
         "bookmark-dash",
+        "bookmark-dash-fill",
         "bookmark-fill",
-        "bookmark-heart-fill",
         "bookmark-heart",
-        "bookmark-plus-fill",
+        "bookmark-heart-fill",
         "bookmark-plus",
-        "bookmark-star-fill",
+        "bookmark-plus-fill",
         "bookmark-star",
-        "bookmark-x-fill",
+        "bookmark-star-fill",
         "bookmark-x",
-        "bookmark",
-        "bookmarks-fill",
+        "bookmark-x-fill",
         "bookmarks",
+        "bookmarks-fill",
         "bookshelf",
+        "boombox",
+        "boombox-fill",
+        "bootstrap",
         "bootstrap-fill",
         "bootstrap-reboot",
-        "bootstrap",
+        "border",
         "border-all",
         "border-bottom",
         "border-center",
         "border-inner",
         "border-left",
         "border-middle",
         "border-outer",
         "border-right",
         "border-style",
         "border-top",
         "border-width",
-        "border",
-        "bounding-box-circles",
         "bounding-box",
+        "bounding-box-circles",
+        "box",
         "box-arrow-down-left",
         "box-arrow-down-right",
         "box-arrow-down",
+        "box-arrow-in-down",
         "box-arrow-in-down-left",
         "box-arrow-in-down-right",
-        "box-arrow-in-down",
         "box-arrow-in-left",
         "box-arrow-in-right",
+        "box-arrow-in-up",
         "box-arrow-in-up-left",
         "box-arrow-in-up-right",
-        "box-arrow-in-up",
         "box-arrow-left",
         "box-arrow-right",
+        "box-arrow-up",
         "box-arrow-up-left",
         "box-arrow-up-right",
-        "box-arrow-up",
+        "box-fill",
         "box-seam",
-        "box",
+        "box-seam-fill",
+        "box2",
+        "box2-fill",
+        "box2-heart",
+        "box2-heart-fill",
+        "boxes",
         "braces",
+        "braces-asterisk",
         "bricks",
-        "briefcase-fill",
         "briefcase",
-        "brightness-alt-high-fill",
+        "briefcase-fill",
         "brightness-alt-high",
-        "brightness-alt-low-fill",
+        "brightness-alt-high-fill",
         "brightness-alt-low",
-        "brightness-high-fill",
+        "brightness-alt-low-fill",
         "brightness-high",
-        "brightness-low-fill",
+        "brightness-high-fill",
         "brightness-low",
-        "broadcast-pin",
+        "brightness-low-fill",
         "broadcast",
-        "brush-fill",
+        "broadcast-pin",
+        "browser-chrome",
+        "browser-edge",
+        "browser-firefox",
+        "browser-safari",
         "brush",
-        "bucket-fill",
+        "brush-fill",
         "bucket",
-        "bug-fill",
+        "bucket-fill",
         "bug",
+        "bug-fill",
         "building",
+        "building-add",
+        "building-check",
+        "building-dash",
+        "building-down",
+        "building-exclamation",
+        "building-fill",
+        "building-fill-add",
+        "building-fill-check",
+        "building-fill-dash",
+        "building-fill-down",
+        "building-fill-exclamation",
+        "building-fill-gear",
+        "building-fill-lock",
+        "building-fill-slash",
+        "building-fill-up",
+        "building-fill-x",
+        "building-gear",
+        "building-lock",
+        "building-slash",
+        "building-up",
+        "building-x",
+        "buildings",
+        "buildings-fill",
         "bullseye",
-        "calculator-fill",
+        "bus-front",
+        "bus-front-fill",
+        "c-circle",
+        "c-circle-fill",
+        "c-square",
+        "c-square-fill",
         "calculator",
-        "calendar-check-fill",
+        "calculator-fill",
+        "calendar",
         "calendar-check",
-        "calendar-date-fill",
+        "calendar-check-fill",
         "calendar-date",
-        "calendar-day-fill",
+        "calendar-date-fill",
         "calendar-day",
-        "calendar-event-fill",
+        "calendar-day-fill",
         "calendar-event",
+        "calendar-event-fill",
         "calendar-fill",
-        "calendar-minus-fill",
+        "calendar-heart",
+        "calendar-heart-fill",
         "calendar-minus",
-        "calendar-month-fill",
+        "calendar-minus-fill",
         "calendar-month",
-        "calendar-plus-fill",
+        "calendar-month-fill",
         "calendar-plus",
-        "calendar-range-fill",
+        "calendar-plus-fill",
         "calendar-range",
-        "calendar-week-fill",
+        "calendar-range-fill",
         "calendar-week",
-        "calendar-x-fill",
+        "calendar-week-fill",
         "calendar-x",
-        "calendar",
-        "calendar2-check-fill",
+        "calendar-x-fill",
+        "calendar2",
         "calendar2-check",
-        "calendar2-date-fill",
+        "calendar2-check-fill",
         "calendar2-date",
-        "calendar2-day-fill",
+        "calendar2-date-fill",
         "calendar2-day",
-        "calendar2-event-fill",
+        "calendar2-day-fill",
         "calendar2-event",
+        "calendar2-event-fill",
         "calendar2-fill",
-        "calendar2-minus-fill",
+        "calendar2-heart",
+        "calendar2-heart-fill",
         "calendar2-minus",
-        "calendar2-month-fill",
+        "calendar2-minus-fill",
         "calendar2-month",
-        "calendar2-plus-fill",
+        "calendar2-month-fill",
         "calendar2-plus",
-        "calendar2-range-fill",
+        "calendar2-plus-fill",
         "calendar2-range",
-        "calendar2-week-fill",
+        "calendar2-range-fill",
         "calendar2-week",
-        "calendar2-x-fill",
+        "calendar2-week-fill",
         "calendar2-x",
-        "calendar2",
-        "calendar3-event-fill",
+        "calendar2-x-fill",
+        "calendar3",
         "calendar3-event",
+        "calendar3-event-fill",
         "calendar3-fill",
-        "calendar3-range-fill",
         "calendar3-range",
-        "calendar3-week-fill",
+        "calendar3-range-fill",
         "calendar3-week",
-        "calendar3",
+        "calendar3-week-fill",
+        "calendar4",
         "calendar4-event",
         "calendar4-range",
         "calendar4-week",
-        "calendar4",
+        "camera",
+        "camera2",
         "camera-fill",
-        "camera-reels-fill",
         "camera-reels",
+        "camera-reels-fill",
+        "camera-video",
         "camera-video-fill",
-        "camera-video-off-fill",
         "camera-video-off",
-        "camera-video",
-        "camera",
-        "camera2",
-        "capslock-fill",
+        "camera-video-off-fill",
         "capslock",
+        "capslock-fill",
+        "capsule",
+        "capsule-pill",
+        "car-front",
+        "car-front-fill",
         "card-checklist",
         "card-heading",
         "card-image",
         "card-list",
         "card-text",
+        "caret-down",
         "caret-down-fill",
-        "caret-down-square-fill",
         "caret-down-square",
-        "caret-down",
+        "caret-down-square-fill",
+        "caret-left",
         "caret-left-fill",
-        "caret-left-square-fill",
         "caret-left-square",
-        "caret-left",
+        "caret-left-square-fill",
+        "caret-right",
         "caret-right-fill",
-        "caret-right-square-fill",
         "caret-right-square",
-        "caret-right",
+        "caret-right-square-fill",
+        "caret-up",
         "caret-up-fill",
-        "caret-up-square-fill",
         "caret-up-square",
-        "caret-up",
-        "cart-check-fill",
+        "caret-up-square-fill",
+        "cart",
         "cart-check",
-        "cart-dash-fill",
+        "cart-check-fill",
         "cart-dash",
+        "cart-dash-fill",
         "cart-fill",
-        "cart-plus-fill",
         "cart-plus",
-        "cart-x-fill",
+        "cart-plus-fill",
         "cart-x",
-        "cart",
+        "cart-x-fill",
         "cart2",
         "cart3",
         "cart4",
-        "cash-stack",
         "cash",
+        "cash-coin",
+        "cash-stack",
+        "cassette",
+        "cassette-fill",
         "cast",
-        "chat-dots-fill",
+        "cc-circle",
+        "cc-circle-fill",
+        "cc-square",
+        "cc-square-fill",
+        "chat",
         "chat-dots",
+        "chat-dots-fill",
         "chat-fill",
-        "chat-left-dots-fill",
+        "chat-heart",
+        "chat-heart-fill",
+        "chat-left",
         "chat-left-dots",
+        "chat-left-dots-fill",
         "chat-left-fill",
-        "chat-left-quote-fill",
+        "chat-left-heart",
+        "chat-left-heart-fill",
         "chat-left-quote",
-        "chat-left-text-fill",
+        "chat-left-quote-fill",
         "chat-left-text",
-        "chat-left",
-        "chat-quote-fill",
+        "chat-left-text-fill",
         "chat-quote",
-        "chat-right-dots-fill",
+        "chat-quote-fill",
+        "chat-right",
         "chat-right-dots",
+        "chat-right-dots-fill",
         "chat-right-fill",
-        "chat-right-quote-fill",
+        "chat-right-heart",
+        "chat-right-heart-fill",
         "chat-right-quote",
-        "chat-right-text-fill",
+        "chat-right-quote-fill",
         "chat-right-text",
-        "chat-right",
-        "chat-square-dots-fill",
+        "chat-right-text-fill",
+        "chat-square",
         "chat-square-dots",
+        "chat-square-dots-fill",
         "chat-square-fill",
-        "chat-square-quote-fill",
+        "chat-square-heart",
+        "chat-square-heart-fill",
         "chat-square-quote",
-        "chat-square-text-fill",
+        "chat-square-quote-fill",
         "chat-square-text",
-        "chat-square",
-        "chat-text-fill",
+        "chat-square-text-fill",
         "chat-text",
-        "chat",
+        "chat-text-fill",
+        "check",
         "check-all",
-        "check-circle-fill",
         "check-circle",
-        "check-square-fill",
+        "check-circle-fill",
+        "check-lg",
         "check-square",
-        "check",
+        "check-square-fill",
+        "check2",
         "check2-all",
         "check2-circle",
         "check2-square",
-        "check2",
         "chevron-bar-contract",
         "chevron-bar-down",
         "chevron-bar-expand",
         "chevron-bar-left",
         "chevron-bar-right",
         "chevron-bar-up",
         "chevron-compact-down",
@@ -388,1303 +525,1437 @@
         "chevron-double-right",
         "chevron-double-up",
         "chevron-down",
         "chevron-expand",
         "chevron-left",
         "chevron-right",
         "chevron-up",
+        "circle",
         "circle-fill",
         "circle-half",
+        "slash-circle",
         "circle-square",
-        "circle",
+        "clipboard",
         "clipboard-check",
+        "clipboard-check-fill",
         "clipboard-data",
+        "clipboard-data-fill",
+        "clipboard-fill",
+        "clipboard-heart",
+        "clipboard-heart-fill",
         "clipboard-minus",
+        "clipboard-minus-fill",
         "clipboard-plus",
+        "clipboard-plus-fill",
+        "clipboard-pulse",
         "clipboard-x",
-        "clipboard",
+        "clipboard-x-fill",
+        "clipboard2",
+        "clipboard2-check",
+        "clipboard2-check-fill",
+        "clipboard2-data",
+        "clipboard2-data-fill",
+        "clipboard2-fill",
+        "clipboard2-heart",
+        "clipboard2-heart-fill",
+        "clipboard2-minus",
+        "clipboard2-minus-fill",
+        "clipboard2-plus",
+        "clipboard2-plus-fill",
+        "clipboard2-pulse",
+        "clipboard2-pulse-fill",
+        "clipboard2-x",
+        "clipboard2-x-fill",
+        "clock",
         "clock-fill",
         "clock-history",
-        "clock",
-        "cloud-arrow-down-fill",
+        "cloud",
         "cloud-arrow-down",
-        "cloud-arrow-up-fill",
+        "cloud-arrow-down-fill",
         "cloud-arrow-up",
-        "cloud-check-fill",
+        "cloud-arrow-up-fill",
         "cloud-check",
-        "cloud-download-fill",
+        "cloud-check-fill",
         "cloud-download",
-        "cloud-drizzle-fill",
+        "cloud-download-fill",
         "cloud-drizzle",
+        "cloud-drizzle-fill",
         "cloud-fill",
-        "cloud-fog-fill",
         "cloud-fog",
-        "cloud-fog2-fill",
+        "cloud-fog-fill",
         "cloud-fog2",
-        "cloud-hail-fill",
+        "cloud-fog2-fill",
         "cloud-hail",
-        "cloud-haze-1",
-        "cloud-haze-fill",
+        "cloud-hail-fill",
         "cloud-haze",
+        "cloud-haze-fill",
+        "cloud-haze2",
         "cloud-haze2-fill",
+        "cloud-lightning",
         "cloud-lightning-fill",
-        "cloud-lightning-rain-fill",
         "cloud-lightning-rain",
-        "cloud-lightning",
-        "cloud-minus-fill",
+        "cloud-lightning-rain-fill",
         "cloud-minus",
-        "cloud-moon-fill",
+        "cloud-minus-fill",
         "cloud-moon",
-        "cloud-plus-fill",
+        "cloud-moon-fill",
         "cloud-plus",
+        "cloud-plus-fill",
+        "cloud-rain",
         "cloud-rain-fill",
-        "cloud-rain-heavy-fill",
         "cloud-rain-heavy",
-        "cloud-rain",
-        "cloud-slash-fill",
+        "cloud-rain-heavy-fill",
         "cloud-slash",
-        "cloud-sleet-fill",
+        "cloud-slash-fill",
         "cloud-sleet",
-        "cloud-snow-fill",
+        "cloud-sleet-fill",
         "cloud-snow",
-        "cloud-sun-fill",
+        "cloud-snow-fill",
         "cloud-sun",
-        "cloud-upload-fill",
+        "cloud-sun-fill",
         "cloud-upload",
-        "cloud",
-        "clouds-fill",
+        "cloud-upload-fill",
         "clouds",
-        "cloudy-fill",
+        "clouds-fill",
         "cloudy",
+        "cloudy-fill",
+        "code",
         "code-slash",
         "code-square",
-        "code",
+        "coin",
+        "collection",
         "collection-fill",
-        "collection-play-fill",
         "collection-play",
-        "collection",
-        "columns-gap",
+        "collection-play-fill",
         "columns",
+        "columns-gap",
         "command",
-        "compass-fill",
         "compass",
-        "cone-striped",
+        "compass-fill",
         "cone",
+        "cone-striped",
         "controller",
-        "cpu-fill",
         "cpu",
-        "credit-card-2-back-fill",
+        "cpu-fill",
+        "credit-card",
         "credit-card-2-back",
-        "credit-card-2-front-fill",
+        "credit-card-2-back-fill",
         "credit-card-2-front",
+        "credit-card-2-front-fill",
         "credit-card-fill",
-        "credit-card",
         "crop",
+        "cup",
         "cup-fill",
+        "cup-hot",
+        "cup-hot-fill",
         "cup-straw",
-        "cup",
+        "currency-bitcoin",
+        "currency-dollar",
+        "currency-euro",
+        "currency-exchange",
+        "currency-pound",
+        "currency-rupee",
+        "currency-yen",
+        "cursor",
         "cursor-fill",
         "cursor-text",
-        "cursor",
+        "dash",
+        "dash-circle",
         "dash-circle-dotted",
         "dash-circle-fill",
-        "dash-circle",
+        "dash-lg",
+        "dash-square",
         "dash-square-dotted",
         "dash-square-fill",
-        "dash-square",
-        "dash",
-        "diagram-2-fill",
+        "database",
+        "database-add",
+        "database-check",
+        "database-dash",
+        "database-down",
+        "database-exclamation",
+        "database-fill",
+        "database-fill-add",
+        "database-fill-check",
+        "database-fill-dash",
+        "database-fill-down",
+        "database-fill-exclamation",
+        "database-fill-gear",
+        "database-fill-lock",
+        "database-fill-slash",
+        "database-fill-up",
+        "database-fill-x",
+        "database-gear",
+        "database-lock",
+        "database-slash",
+        "database-up",
+        "database-x",
+        "device-hdd",
+        "device-hdd-fill",
+        "device-ssd",
+        "device-ssd-fill",
         "diagram-2",
-        "diagram-3-fill",
+        "diagram-2-fill",
         "diagram-3",
+        "diagram-3-fill",
+        "diamond",
         "diamond-fill",
         "diamond-half",
-        "diamond",
-        "dice-1-fill",
         "dice-1",
-        "dice-2-fill",
+        "dice-1-fill",
         "dice-2",
-        "dice-3-fill",
+        "dice-2-fill",
         "dice-3",
-        "dice-4-fill",
+        "dice-3-fill",
         "dice-4",
-        "dice-5-fill",
+        "dice-4-fill",
         "dice-5",
-        "dice-6-fill",
+        "dice-5-fill",
         "dice-6",
-        "disc-fill",
+        "dice-6-fill",
         "disc",
+        "disc-fill",
         "discord",
-        "display-fill",
         "display",
+        "display-fill",
+        "displayport",
+        "displayport-fill",
         "distribute-horizontal",
         "distribute-vertical",
-        "door-closed-fill",
         "door-closed",
-        "door-open-fill",
+        "door-closed-fill",
         "door-open",
+        "door-open-fill",
         "dot",
         "download",
+        "dpad",
+        "dpad-fill",
+        "dribbble",
+        "dropbox",
+        "droplet",
         "droplet-fill",
         "droplet-half",
-        "droplet",
+        "ear",
+        "ear-fill",
         "earbuds",
-        "easel-fill",
         "easel",
+        "easel-fill",
+        "easel2",
+        "easel2-fill",
+        "easel3",
+        "easel3-fill",
+        "egg",
         "egg-fill",
         "egg-fried",
-        "egg",
-        "eject-fill",
         "eject",
-        "emoji-angry-fill",
+        "eject-fill",
         "emoji-angry",
-        "emoji-dizzy-fill",
+        "emoji-angry-fill",
         "emoji-dizzy",
-        "emoji-expressionless-fill",
+        "emoji-dizzy-fill",
         "emoji-expressionless",
-        "emoji-frown-fill",
+        "emoji-expressionless-fill",
         "emoji-frown",
-        "emoji-heart-eyes-fill",
+        "emoji-frown-fill",
         "emoji-heart-eyes",
-        "emoji-laughing-fill",
+        "emoji-heart-eyes-fill",
+        "emoji-kiss",
+        "emoji-kiss-fill",
         "emoji-laughing",
-        "emoji-neutral-fill",
+        "emoji-laughing-fill",
         "emoji-neutral",
+        "emoji-neutral-fill",
+        "emoji-smile",
         "emoji-smile-fill",
-        "emoji-smile-upside-down-fill",
         "emoji-smile-upside-down",
-        "emoji-smile",
-        "emoji-sunglasses-fill",
+        "emoji-smile-upside-down-fill",
         "emoji-sunglasses",
-        "emoji-wink-fill",
+        "emoji-sunglasses-fill",
         "emoji-wink",
+        "emoji-wink-fill",
+        "envelope",
+        "envelope-at",
+        "envelope-at-fill",
+        "envelope-check",
+        "envelope-check-fill",
+        "envelope-dash",
+        "envelope-dash-fill",
+        "envelope-exclamation",
+        "envelope-exclamation-fill",
         "envelope-fill",
-        "envelope-open-fill",
+        "envelope-heart",
+        "envelope-heart-fill",
         "envelope-open",
-        "envelope",
-        "eraser-fill",
+        "envelope-open-fill",
+        "envelope-open-heart",
+        "envelope-open-heart-fill",
+        "envelope-paper",
+        "envelope-paper-fill",
+        "envelope-paper-heart",
+        "envelope-paper-heart-fill",
+        "envelope-plus",
+        "envelope-plus-fill",
+        "envelope-slash",
+        "envelope-slash-fill",
+        "envelope-x",
+        "envelope-x-fill",
         "eraser",
-        "exclamation-circle-fill",
+        "eraser-fill",
+        "escape",
+        "ethernet",
+        "ev-front",
+        "ev-front-fill",
+        "ev-station",
+        "ev-station-fill",
+        "exclamation",
         "exclamation-circle",
-        "exclamation-diamond-fill",
+        "exclamation-circle-fill",
         "exclamation-diamond",
-        "exclamation-octagon-fill",
+        "exclamation-diamond-fill",
+        "exclamation-lg",
         "exclamation-octagon",
-        "exclamation-square-fill",
+        "exclamation-octagon-fill",
         "exclamation-square",
-        "exclamation-triangle-fill",
+        "exclamation-square-fill",
         "exclamation-triangle",
-        "exclamation",
+        "exclamation-triangle-fill",
         "exclude",
+        "explicit",
+        "explicit-fill",
+        "eye",
         "eye-fill",
-        "eye-slash-fill",
         "eye-slash",
-        "eye",
+        "eye-slash-fill",
         "eyedropper",
         "eyeglasses",
         "facebook",
-        "file-arrow-down-fill",
+        "fan",
+        "fast-forward",
+        "fast-forward-btn",
+        "fast-forward-btn-fill",
+        "fast-forward-circle",
+        "fast-forward-circle-fill",
+        "fast-forward-fill",
+        "file",
         "file-arrow-down",
-        "file-arrow-up-fill",
+        "file-arrow-down-fill",
         "file-arrow-up",
-        "file-bar-graph-fill",
+        "file-arrow-up-fill",
         "file-bar-graph",
-        "file-binary-fill",
+        "file-bar-graph-fill",
         "file-binary",
-        "file-break-fill",
+        "file-binary-fill",
         "file-break",
-        "file-check-fill",
+        "file-break-fill",
         "file-check",
-        "file-code-fill",
+        "file-check-fill",
         "file-code",
-        "file-diff-fill",
+        "file-code-fill",
         "file-diff",
-        "file-earmark-arrow-down-fill",
+        "file-diff-fill",
+        "file-earmark",
         "file-earmark-arrow-down",
-        "file-earmark-arrow-up-fill",
+        "file-earmark-arrow-down-fill",
         "file-earmark-arrow-up",
-        "file-earmark-bar-graph-fill",
+        "file-earmark-arrow-up-fill",
         "file-earmark-bar-graph",
-        "file-earmark-binary-fill",
+        "file-earmark-bar-graph-fill",
         "file-earmark-binary",
-        "file-earmark-break-fill",
+        "file-earmark-binary-fill",
         "file-earmark-break",
-        "file-earmark-check-fill",
+        "file-earmark-break-fill",
         "file-earmark-check",
-        "file-earmark-code-fill",
+        "file-earmark-check-fill",
         "file-earmark-code",
-        "file-earmark-diff-fill",
+        "file-earmark-code-fill",
         "file-earmark-diff",
-        "file-earmark-easel-fill",
+        "file-earmark-diff-fill",
         "file-earmark-easel",
-        "file-earmark-excel-fill",
+        "file-earmark-easel-fill",
         "file-earmark-excel",
+        "file-earmark-excel-fill",
         "file-earmark-fill",
-        "file-earmark-font-fill",
         "file-earmark-font",
-        "file-earmark-image-fill",
+        "file-earmark-font-fill",
         "file-earmark-image",
-        "file-earmark-lock-fill",
+        "file-earmark-image-fill",
         "file-earmark-lock",
-        "file-earmark-lock2-fill",
+        "file-earmark-lock-fill",
         "file-earmark-lock2",
-        "file-earmark-medical-fill",
+        "file-earmark-lock2-fill",
         "file-earmark-medical",
-        "file-earmark-minus-fill",
+        "file-earmark-medical-fill",
         "file-earmark-minus",
-        "file-earmark-music-fill",
+        "file-earmark-minus-fill",
         "file-earmark-music",
-        "file-earmark-person-fill",
+        "file-earmark-music-fill",
+        "file-earmark-pdf",
+        "file-earmark-pdf-fill",
         "file-earmark-person",
-        "file-earmark-play-fill",
+        "file-earmark-person-fill",
         "file-earmark-play",
-        "file-earmark-plus-fill",
+        "file-earmark-play-fill",
         "file-earmark-plus",
-        "file-earmark-post-fill",
+        "file-earmark-plus-fill",
         "file-earmark-post",
-        "file-earmark-ppt-fill",
+        "file-earmark-post-fill",
         "file-earmark-ppt",
-        "file-earmark-richtext-fill",
+        "file-earmark-ppt-fill",
         "file-earmark-richtext",
-        "file-earmark-ruled-fill",
+        "file-earmark-richtext-fill",
         "file-earmark-ruled",
-        "file-earmark-slides-fill",
+        "file-earmark-ruled-fill",
         "file-earmark-slides",
-        "file-earmark-spreadsheet-fill",
+        "file-earmark-slides-fill",
         "file-earmark-spreadsheet",
-        "file-earmark-text-fill",
+        "file-earmark-spreadsheet-fill",
         "file-earmark-text",
-        "file-earmark-word-fill",
+        "file-earmark-text-fill",
         "file-earmark-word",
-        "file-earmark-x-fill",
+        "file-earmark-word-fill",
         "file-earmark-x",
-        "file-earmark-zip-fill",
+        "file-earmark-x-fill",
         "file-earmark-zip",
-        "file-earmark",
-        "file-easel-fill",
+        "file-earmark-zip-fill",
         "file-easel",
-        "file-excel-fill",
+        "file-easel-fill",
         "file-excel",
+        "file-excel-fill",
         "file-fill",
-        "file-font-fill",
         "file-font",
-        "file-image-fill",
+        "file-font-fill",
         "file-image",
-        "file-lock-fill",
+        "file-image-fill",
         "file-lock",
-        "file-lock2-fill",
+        "file-lock-fill",
         "file-lock2",
-        "file-medical-fill",
+        "file-lock2-fill",
         "file-medical",
-        "file-minus-fill",
+        "file-medical-fill",
         "file-minus",
-        "file-music-fill",
+        "file-minus-fill",
         "file-music",
-        "file-person-fill",
+        "file-music-fill",
+        "file-pdf",
+        "file-pdf-fill",
         "file-person",
-        "file-play-fill",
+        "file-person-fill",
         "file-play",
-        "file-plus-fill",
+        "file-play-fill",
         "file-plus",
-        "file-post-fill",
+        "file-plus-fill",
         "file-post",
-        "file-ppt-fill",
+        "file-post-fill",
         "file-ppt",
-        "file-richtext-fill",
+        "file-ppt-fill",
         "file-richtext",
-        "file-ruled-fill",
+        "file-richtext-fill",
         "file-ruled",
-        "file-slides-fill",
+        "file-ruled-fill",
         "file-slides",
-        "file-spreadsheet-fill",
+        "file-slides-fill",
         "file-spreadsheet",
-        "file-text-fill",
+        "file-spreadsheet-fill",
         "file-text",
-        "file-word-fill",
+        "file-text-fill",
         "file-word",
-        "file-x-fill",
+        "file-word-fill",
         "file-x",
-        "file-zip-fill",
+        "file-x-fill",
         "file-zip",
-        "file",
-        "files-alt",
+        "file-zip-fill",
         "files",
+        "files-alt",
+        "filetype-aac",
+        "filetype-ai",
+        "filetype-bmp",
+        "filetype-cs",
+        "filetype-css",
+        "filetype-csv",
+        "filetype-doc",
+        "filetype-docx",
+        "filetype-exe",
+        "filetype-gif",
+        "filetype-heic",
+        "filetype-html",
+        "filetype-java",
+        "filetype-jpg",
+        "filetype-js",
+        "filetype-json",
+        "filetype-jsx",
+        "filetype-key",
+        "filetype-m4p",
+        "filetype-md",
+        "filetype-mdx",
+        "filetype-mov",
+        "filetype-mp3",
+        "filetype-mp4",
+        "filetype-otf",
+        "filetype-pdf",
+        "filetype-php",
+        "filetype-png",
+        "filetype-ppt",
+        "filetype-pptx",
+        "filetype-psd",
+        "filetype-py",
+        "filetype-raw",
+        "filetype-rb",
+        "filetype-sass",
+        "filetype-scss",
+        "filetype-sh",
+        "filetype-sql",
+        "filetype-svg",
+        "filetype-tiff",
+        "filetype-tsx",
+        "filetype-ttf",
+        "filetype-txt",
+        "filetype-wav",
+        "filetype-woff",
+        "filetype-xls",
+        "filetype-xlsx",
+        "filetype-xml",
+        "filetype-yml",
         "film",
-        "filter-circle-fill",
+        "filter",
         "filter-circle",
+        "filter-circle-fill",
         "filter-left",
         "filter-right",
-        "filter-square-fill",
         "filter-square",
-        "filter",
-        "flag-fill",
+        "filter-square-fill",
+        "fingerprint",
+        "fire",
         "flag",
+        "flag-fill",
         "flower1",
         "flower2",
         "flower3",
+        "folder",
         "folder-check",
         "folder-fill",
         "folder-minus",
         "folder-plus",
-        "folder-symlink-fill",
         "folder-symlink",
+        "folder-symlink-fill",
         "folder-x",
-        "folder",
-        "folder2-open",
         "folder2",
+        "folder2-open",
         "fonts",
-        "forward-fill",
         "forward",
+        "forward-fill",
         "front",
-        "fullscreen-exit",
+        "fuel-pump",
+        "fuel-pump-diesel",
+        "fuel-pump-diesel-fill",
+        "fuel-pump-fill",
         "fullscreen",
-        "funnel-fill",
+        "fullscreen-exit",
         "funnel",
+        "funnel-fill",
+        "gear",
         "gear-fill",
-        "gear-wide-connected",
         "gear-wide",
-        "gear",
+        "gear-wide-connected",
         "gem",
-        "geo-alt-fill",
+        "gender-ambiguous",
+        "gender-female",
+        "gender-male",
+        "gender-trans",
+        "geo",
         "geo-alt",
+        "geo-alt-fill",
         "geo-fill",
-        "geo",
-        "gift-fill",
         "gift",
+        "gift-fill",
+        "git",
         "github",
         "globe",
+        "globe-americas",
+        "globe-asia-australia",
+        "globe-central-south-asia",
+        "globe-europe-africa",
         "globe2",
         "google",
+        "google-play",
+        "gpu-card",
         "graph-down",
+        "graph-down-arrow",
         "graph-up",
-        "grid-1x2-fill",
+        "graph-up-arrow",
+        "grid",
         "grid-1x2",
-        "grid-3x2-gap-fill",
-        "grid-3x2-gap",
+        "grid-1x2-fill",
         "grid-3x2",
-        "grid-3x3-gap-fill",
-        "grid-3x3-gap",
+        "grid-3x2-gap",
+        "grid-3x2-gap-fill",
         "grid-3x3",
+        "grid-3x3-gap",
+        "grid-3x3-gap-fill",
         "grid-fill",
-        "grid",
         "grip-horizontal",
         "grip-vertical",
+        "h-circle",
+        "h-circle-fill",
+        "h-square",
+        "h-square-fill",
         "hammer",
+        "hand-index",
         "hand-index-fill",
-        "hand-index-thumb-fill",
         "hand-index-thumb",
-        "hand-index",
-        "hand-thumbs-down-fill",
+        "hand-index-thumb-fill",
         "hand-thumbs-down",
-        "hand-thumbs-up-fill",
+        "hand-thumbs-down-fill",
         "hand-thumbs-up",
-        "handbag-fill",
+        "hand-thumbs-up-fill",
         "handbag",
+        "handbag-fill",
         "hash",
+        "hdd",
         "hdd-fill",
-        "hdd-network-fill",
         "hdd-network",
-        "hdd-rack-fill",
+        "hdd-network-fill",
         "hdd-rack",
-        "hdd-stack-fill",
+        "hdd-rack-fill",
         "hdd-stack",
-        "hdd",
+        "hdd-stack-fill",
+        "hdmi",
+        "hdmi-fill",
         "headphones",
         "headset",
+        "headset-vr",
+        "heart",
+        "heart-arrow",
         "heart-fill",
         "heart-half",
-        "heart",
+        "heart-pulse",
+        "heart-pulse-fill",
+        "heartbreak",
+        "heartbreak-fill",
+        "hearts",
+        "heptagon",
         "heptagon-fill",
         "heptagon-half",
-        "heptagon",
+        "hexagon",
         "hexagon-fill",
         "hexagon-half",
-        "hexagon",
+        "hospital",
+        "hospital-fill",
+        "hourglass",
         "hourglass-bottom",
         "hourglass-split",
         "hourglass-top",
-        "hourglass",
-        "house-door-fill",
+        "house",
+        "house-add",
+        "house-add-fill",
+        "house-check",
+        "house-check-fill",
+        "house-dash",
+        "house-dash-fill",
         "house-door",
+        "house-door-fill",
+        "house-down",
+        "house-down-fill",
+        "house-exclamation",
+        "house-exclamation-fill",
         "house-fill",
-        "house",
+        "house-gear",
+        "house-gear-fill",
+        "house-heart",
+        "house-heart-fill",
+        "house-lock",
+        "house-lock-fill",
+        "house-slash",
+        "house-slash-fill",
+        "house-up",
+        "house-up-fill",
+        "house-x",
+        "house-x-fill",
+        "houses",
+        "houses-fill",
         "hr",
         "hurricane",
+        "hypnotize",
+        "image",
         "image-alt",
         "image-fill",
-        "image",
         "images",
-        "inbox-fill",
         "inbox",
+        "inbox-fill",
         "inboxes-fill",
         "inboxes",
-        "info-circle-fill",
+        "incognito",
+        "indent",
+        "infinity",
+        "info",
         "info-circle",
-        "info-square-fill",
+        "info-circle-fill",
+        "info-lg",
         "info-square",
-        "info",
-        "input-cursor-text",
+        "info-square-fill",
         "input-cursor",
+        "input-cursor-text",
         "instagram",
         "intersect",
+        "journal",
         "journal-album",
         "journal-arrow-down",
         "journal-arrow-up",
-        "journal-bookmark-fill",
         "journal-bookmark",
+        "journal-bookmark-fill",
         "journal-check",
         "journal-code",
         "journal-medical",
         "journal-minus",
         "journal-plus",
         "journal-richtext",
         "journal-text",
         "journal-x",
-        "journal",
         "journals",
         "joystick",
+        "justify",
         "justify-left",
         "justify-right",
-        "justify",
-        "kanban-fill",
         "kanban",
-        "key-fill",
+        "kanban-fill",
         "key",
-        "keyboard-fill",
+        "key-fill",
         "keyboard",
+        "keyboard-fill",
         "ladder",
-        "lamp-fill",
         "lamp",
-        "laptop-fill",
+        "lamp-fill",
         "laptop",
+        "laptop-fill",
         "layer-backward",
         "layer-forward",
+        "layers",
         "layers-fill",
         "layers-half",
-        "layers",
+        "layout-sidebar",
         "layout-sidebar-inset-reverse",
         "layout-sidebar-inset",
         "layout-sidebar-reverse",
-        "layout-sidebar",
         "layout-split",
-        "layout-text-sidebar-reverse",
         "layout-text-sidebar",
-        "layout-text-window-reverse",
+        "layout-text-sidebar-reverse",
         "layout-text-window",
+        "layout-text-window-reverse",
         "layout-three-columns",
         "layout-wtf",
         "life-preserver",
+        "lightbulb",
         "lightbulb-fill",
-        "lightbulb-off-fill",
         "lightbulb-off",
-        "lightbulb",
-        "lightning-charge-fill",
+        "lightbulb-off-fill",
+        "lightning",
         "lightning-charge",
+        "lightning-charge-fill",
         "lightning-fill",
-        "lightning",
-        "link-45deg",
+        "line",
         "link",
+        "link-45deg",
         "linkedin",
+        "list",
         "list-check",
+        "list-columns",
+        "list-columns-reverse",
         "list-nested",
         "list-ol",
         "list-stars",
         "list-task",
         "list-ul",
-        "list",
-        "lock-fill",
         "lock",
+        "lock-fill",
+        "lungs",
+        "lungs-fill",
+        "magic",
+        "magnet",
+        "magnet-fill",
         "mailbox",
         "mailbox2",
-        "map-fill",
         "map",
-        "markdown-fill",
+        "map-fill",
         "markdown",
+        "markdown-fill",
         "mask",
-        "megaphone-fill",
+        "mastodon",
+        "medium",
         "megaphone",
-        "menu-app-fill",
+        "megaphone-fill",
+        "memory",
         "menu-app",
+        "menu-app-fill",
+        "menu-button",
         "menu-button-fill",
-        "menu-button-wide-fill",
         "menu-button-wide",
-        "menu-button",
+        "menu-button-wide-fill",
         "menu-down",
         "menu-up",
+        "messenger",
+        "meta",
+        "mic",
         "mic-fill",
-        "mic-mute-fill",
         "mic-mute",
-        "mic",
-        "minecart-loaded",
+        "mic-mute-fill",
+        "microsoft",
+        "microsoft-teams",
         "minecart",
+        "minecart-loaded",
+        "modem",
+        "modem-fill",
         "moisture",
+        "moon",
         "moon-fill",
-        "moon-stars-fill",
         "moon-stars",
-        "moon",
-        "mouse-fill",
+        "moon-stars-fill",
+        "mortarboard",
+        "mortarboard-fill",
+        "motherboard",
+        "motherboard-fill",
         "mouse",
-        "mouse2-fill",
+        "mouse-fill",
         "mouse2",
-        "mouse3-fill",
+        "mouse2-fill",
         "mouse3",
+        "mouse3-fill",
+        "music-note",
         "music-note-beamed",
         "music-note-list",
-        "music-note",
-        "music-player-fill",
         "music-player",
+        "music-player-fill",
         "newspaper",
-        "node-minus-fill",
+        "nintendo-switch",
         "node-minus",
-        "node-plus-fill",
+        "node-minus-fill",
         "node-plus",
-        "nut-fill",
+        "node-plus-fill",
         "nut",
+        "nut-fill",
+        "nvidia",
+        "octagon",
         "octagon-fill",
         "octagon-half",
-        "octagon",
+        "optical-audio",
+        "optical-audio-fill",
         "option",
         "outlet",
+        "p-circle",
+        "p-circle-fill",
+        "p-square",
+        "p-square-fill",
         "paint-bucket",
-        "palette-fill",
         "palette",
+        "palette-fill",
         "palette2",
         "paperclip",
         "paragraph",
-        "patch-check-fill",
+        "pass",
+        "pass-fill",
         "patch-check",
-        "patch-exclamation-fill",
+        "patch-check-fill",
         "patch-exclamation",
-        "patch-minus-fill",
+        "patch-exclamation-fill",
         "patch-minus",
-        "patch-plus-fill",
+        "patch-minus-fill",
         "patch-plus",
-        "patch-question-fill",
+        "patch-plus-fill",
         "patch-question",
-        "pause-btn-fill",
+        "patch-question-fill",
+        "pause",
         "pause-btn",
-        "pause-circle-fill",
+        "pause-btn-fill",
         "pause-circle",
+        "pause-circle-fill",
         "pause-fill",
-        "pause",
-        "peace-fill",
+        "paypal",
+        "pc",
+        "pc-display",
+        "pc-display-horizontal",
+        "pc-horizontal",
+        "pci-card",
         "peace",
-        "pen-fill",
+        "peace-fill",
         "pen",
+        "pen-fill",
+        "pencil",
         "pencil-fill",
         "pencil-square",
-        "pencil",
+        "pentagon",
         "pentagon-fill",
         "pentagon-half",
-        "pentagon",
-        "people-fill",
         "people",
+        "person-circle",
+        "people-fill",
         "percent",
-        "person-badge-fill",
+        "person",
+        "person-add",
         "person-badge",
+        "person-badge-fill",
         "person-bounding-box",
-        "person-check-fill",
         "person-check",
-        "person-circle",
-        "person-dash-fill",
+        "person-check-fill",
         "person-dash",
+        "person-dash-fill",
+        "person-down",
+        "person-exclamation",
         "person-fill",
+        "person-fill-add",
+        "person-fill-check",
+        "person-fill-dash",
+        "person-fill-down",
+        "person-fill-exclamation",
+        "person-fill-gear",
+        "person-fill-lock",
+        "person-fill-slash",
+        "person-fill-up",
+        "person-fill-x",
+        "person-gear",
+        "person-heart",
+        "person-hearts",
         "person-lines-fill",
-        "person-plus-fill",
+        "person-lock",
         "person-plus",
+        "person-plus-fill",
+        "person-rolodex",
+        "person-slash",
         "person-square",
-        "person-x-fill",
+        "person-up",
+        "person-vcard",
+        "person-vcard-fill",
+        "person-video",
+        "person-video2",
+        "person-video3",
+        "person-workspace",
         "person-x",
-        "person",
+        "person-x-fill",
+        "phone",
         "phone-fill",
-        "phone-landscape-fill",
+        "phone-flip",
         "phone-landscape",
-        "phone-vibrate-fill",
+        "phone-landscape-fill",
         "phone-vibrate",
-        "phone",
-        "pie-chart-fill",
+        "phone-vibrate-fill",
         "pie-chart",
-        "pin-angle-fill",
+        "pie-chart-fill",
+        "piggy-bank",
+        "piggy-bank-fill",
+        "pin",
         "pin-angle",
+        "pin-angle-fill",
         "pin-fill",
-        "pin",
-        "pip-fill",
+        "pin-map",
+        "pin-map-fill",
+        "pinterest",
         "pip",
-        "play-btn-fill",
+        "pip-fill",
+        "play",
         "play-btn",
-        "play-circle-fill",
+        "play-btn-fill",
         "play-circle",
+        "play-circle-fill",
         "play-fill",
-        "play",
-        "plug-fill",
+        "playstation",
         "plug",
+        "plug-fill",
+        "plugin",
+        "plus",
+        "plus-circle",
         "plus-circle-dotted",
         "plus-circle-fill",
-        "plus-circle",
+        "plus-lg",
+        "plus-slash-minus",
+        "plus-square",
         "plus-square-dotted",
         "plus-square-fill",
-        "plus-square",
-        "plus",
+        "postage",
+        "postage-fill",
+        "postage-heart",
+        "postage-heart-fill",
+        "postcard",
+        "postcard-fill",
+        "postcard-heart",
+        "postcard-heart-fill",
         "power",
-        "printer-fill",
+        "prescription",
+        "prescription2",
         "printer",
-        "puzzle-fill",
+        "printer-fill",
+        "projector",
+        "projector-fill",
         "puzzle",
-        "question-circle-fill",
+        "puzzle-fill",
+        "qr-code",
+        "qr-code-scan",
+        "question",
         "question-circle",
-        "question-diamond-fill",
         "question-diamond",
-        "question-octagon-fill",
+        "question-diamond-fill",
+        "question-circle-fill",
+        "question-lg",
         "question-octagon",
-        "question-square-fill",
+        "question-octagon-fill",
         "question-square",
-        "question",
+        "question-square-fill",
+        "quora",
+        "quote",
+        "r-circle",
+        "r-circle-fill",
+        "r-square",
+        "r-square-fill",
+        "radioactive",
         "rainbow",
-        "receipt-cutoff",
         "receipt",
+        "receipt-cutoff",
         "reception-0",
         "reception-1",
         "reception-2",
         "reception-3",
         "reception-4",
-        "record-btn-fill",
+        "record",
         "record-btn",
-        "record-circle-fill",
+        "record-btn-fill",
         "record-circle",
+        "record-circle-fill",
         "record-fill",
-        "record",
-        "record2-fill",
         "record2",
-        "reply-all-fill",
+        "record2-fill",
+        "recycle",
+        "reddit",
+        "regex",
+        "repeat",
+        "repeat-1",
+        "reply",
         "reply-all",
+        "reply-all-fill",
         "reply-fill",
-        "reply",
-        "rss-fill",
+        "rewind",
+        "rewind-btn",
+        "rewind-btn-fill",
+        "rewind-circle",
+        "rewind-circle-fill",
+        "rewind-fill",
+        "robot",
+        "rocket",
+        "rocket-fill",
+        "rocket-takeoff",
+        "rocket-takeoff-fill",
+        "router",
+        "router-fill",
         "rss",
+        "rss-fill",
         "rulers",
-        "save-fill",
+        "safe",
+        "safe-fill",
+        "safe2",
+        "safe2-fill",
         "save",
-        "save2-fill",
+        "save-fill",
         "save2",
+        "save2-fill",
         "scissors",
+        "scooter",
         "screwdriver",
+        "sd-card",
+        "sd-card-fill",
         "search",
+        "search-heart",
+        "search-heart-fill",
         "segmented-nav",
+        "send",
+        "send-check",
+        "send-check-fill",
+        "send-dash",
+        "send-dash-fill",
+        "send-exclamation",
+        "send-exclamation-fill",
+        "send-fill",
+        "send-plus",
+        "send-plus-fill",
+        "send-slash",
+        "send-slash-fill",
+        "send-x",
+        "send-x-fill",
         "server",
-        "share-fill",
         "share",
+        "share-fill",
+        "shield",
         "shield-check",
         "shield-exclamation",
+        "shield-fill",
         "shield-fill-check",
         "shield-fill-exclamation",
         "shield-fill-minus",
         "shield-fill-plus",
         "shield-fill-x",
-        "shield-fill",
-        "shield-lock-fill",
         "shield-lock",
+        "shield-lock-fill",
         "shield-minus",
         "shield-plus",
         "shield-shaded",
-        "shield-slash-fill",
         "shield-slash",
+        "shield-slash-fill",
         "shield-x",
-        "shield",
-        "shift-fill",
         "shift",
-        "shop-window",
+        "shift-fill",
         "shop",
+        "shop-window",
         "shuffle",
-        "signpost-2-fill",
+        "sign-dead-end",
+        "sign-dead-end-fill",
+        "sign-do-not-enter",
+        "sign-do-not-enter-fill",
+        "sign-intersection",
+        "sign-intersection-fill",
+        "sign-intersection-side",
+        "sign-intersection-side-fill",
+        "sign-intersection-t",
+        "sign-intersection-t-fill",
+        "sign-intersection-y",
+        "sign-intersection-y-fill",
+        "sign-merge-left",
+        "sign-merge-left-fill",
+        "sign-merge-right",
+        "sign-merge-right-fill",
+        "sign-no-left-turn",
+        "sign-no-left-turn-fill",
+        "sign-no-parking",
+        "sign-no-parking-fill",
+        "sign-no-right-turn",
+        "sign-no-right-turn-fill",
+        "sign-railroad",
+        "sign-railroad-fill",
+        "sign-stop",
+        "sign-stop-fill",
+        "sign-stop-lights",
+        "sign-stop-lights-fill",
+        "sign-turn-left",
+        "sign-turn-left-fill",
+        "sign-turn-right",
+        "sign-turn-right-fill",
+        "sign-turn-slight-left",
+        "sign-turn-slight-left-fill",
+        "sign-turn-slight-right",
+        "sign-turn-slight-right-fill",
+        "sign-yield",
+        "sign-yield-fill",
+        "signal",
+        "signpost",
         "signpost-2",
+        "signpost-2-fill",
         "signpost-fill",
-        "signpost-split-fill",
         "signpost-split",
-        "signpost",
-        "sim-fill",
+        "signpost-split-fill",
         "sim",
-        "skip-backward-btn-fill",
+        "sim-fill",
+        "sina-weibo",
+        "skip-backward",
         "skip-backward-btn",
-        "skip-backward-circle-fill",
+        "skip-backward-btn-fill",
         "skip-backward-circle",
+        "skip-backward-circle-fill",
         "skip-backward-fill",
-        "skip-backward",
-        "skip-end-btn-fill",
+        "skip-end",
         "skip-end-btn",
-        "skip-end-circle-fill",
+        "skip-end-btn-fill",
         "skip-end-circle",
+        "skip-end-circle-fill",
         "skip-end-fill",
-        "skip-end",
-        "skip-forward-btn-fill",
+        "skip-forward",
         "skip-forward-btn",
-        "skip-forward-circle-fill",
+        "skip-forward-btn-fill",
         "skip-forward-circle",
+        "skip-forward-circle-fill",
         "skip-forward-fill",
-        "skip-forward",
-        "skip-start-btn-fill",
+        "skip-start",
         "skip-start-btn",
-        "skip-start-circle-fill",
+        "skip-start-btn-fill",
         "skip-start-circle",
+        "skip-start-circle-fill",
         "skip-start-fill",
-        "skip-start",
+        "skype",
         "slack",
+        "slash",
         "slash-circle-fill",
-        "slash-circle",
-        "slash-square-fill",
+        "slash-lg",
         "slash-square",
-        "slash",
+        "slash-square-fill",
         "sliders",
+        "sliders2",
+        "sliders2-vertical",
         "smartwatch",
+        "snapchat",
         "snow",
         "snow2",
         "snow3",
-        "sort-alpha-down-alt",
         "sort-alpha-down",
-        "sort-alpha-up-alt",
+        "sort-alpha-down-alt",
         "sort-alpha-up",
-        "sort-down-alt",
+        "sort-alpha-up-alt",
         "sort-down",
-        "sort-numeric-down-alt",
+        "sort-down-alt",
         "sort-numeric-down",
-        "sort-numeric-up-alt",
+        "sort-numeric-down-alt",
         "sort-numeric-up",
-        "sort-up-alt",
+        "sort-numeric-up-alt",
         "sort-up",
+        "sort-up-alt",
         "soundwave",
-        "speaker-fill",
         "speaker",
+        "speaker-fill",
         "speedometer",
         "speedometer2",
         "spellcheck",
+        "spotify",
+        "square",
         "square-fill",
         "square-half",
-        "square",
         "stack",
+        "stack-overflow",
+        "star",
         "star-fill",
         "star-half",
-        "star",
         "stars",
-        "stickies-fill",
+        "steam",
         "stickies",
-        "sticky-fill",
+        "stickies-fill",
         "sticky",
-        "stop-btn-fill",
+        "sticky-fill",
+        "stop",
         "stop-btn",
-        "stop-circle-fill",
+        "stop-btn-fill",
         "stop-circle",
+        "stop-circle-fill",
         "stop-fill",
-        "stop",
-        "stoplights-fill",
         "stoplights",
-        "stopwatch-fill",
+        "stoplights-fill",
         "stopwatch",
+        "stopwatch-fill",
+        "strava",
+        "stripe",
+        "subscript",
         "subtract",
-        "suit-club-fill",
         "suit-club",
-        "suit-diamond-fill",
+        "suit-club-fill",
         "suit-diamond",
-        "suit-heart-fill",
+        "suit-diamond-fill",
         "suit-heart",
-        "suit-spade-fill",
+        "suit-heart-fill",
         "suit-spade",
-        "sun-fill",
+        "suit-spade-fill",
         "sun",
+        "sun-fill",
         "sunglasses",
-        "sunrise-fill",
         "sunrise",
-        "sunset-fill",
+        "sunrise-fill",
         "sunset",
+        "sunset-fill",
+        "superscript",
         "symmetry-horizontal",
         "symmetry-vertical",
         "table",
+        "tablet",
         "tablet-fill",
-        "tablet-landscape-fill",
         "tablet-landscape",
-        "tablet",
-        "tag-fill",
+        "tablet-landscape-fill",
         "tag",
-        "tags-fill",
+        "tag-fill",
         "tags",
+        "tags-fill",
+        "taxi-front",
+        "taxi-front-fill",
         "telegram",
+        "telephone",
         "telephone-fill",
-        "telephone-forward-fill",
         "telephone-forward",
-        "telephone-inbound-fill",
+        "telephone-forward-fill",
         "telephone-inbound",
-        "telephone-minus-fill",
+        "telephone-inbound-fill",
         "telephone-minus",
-        "telephone-outbound-fill",
+        "telephone-minus-fill",
         "telephone-outbound",
-        "telephone-plus-fill",
+        "telephone-outbound-fill",
         "telephone-plus",
-        "telephone-x-fill",
+        "telephone-plus-fill",
         "telephone-x",
-        "telephone",
-        "terminal-fill",
+        "telephone-x-fill",
+        "tencent-qq",
         "terminal",
+        "terminal-dash",
+        "terminal-fill",
+        "terminal-plus",
+        "terminal-split",
+        "terminal-x",
         "text-center",
         "text-indent-left",
         "text-indent-right",
         "text-left",
         "text-paragraph",
         "text-right",
+        "text-wrap",
+        "textarea",
         "textarea-resize",
         "textarea-t",
-        "textarea",
+        "thermometer",
         "thermometer-half",
         "thermometer-high",
         "thermometer-low",
         "thermometer-snow",
         "thermometer-sun",
-        "thermometer",
-        "three-dots-vertical",
         "three-dots",
+        "three-dots-vertical",
+        "thunderbolt",
+        "thunderbolt-fill",
+        "ticket",
+        "ticket-detailed",
+        "ticket-detailed-fill",
+        "ticket-fill",
+        "ticket-perforated",
+        "ticket-perforated-fill",
+        "tiktok",
         "toggle-off",
         "toggle-on",
         "toggle2-off",
         "toggle2-on",
         "toggles",
         "toggles2",
         "tools",
         "tornado",
-        "trash-fill",
+        "train-freight-front",
+        "train-freight-front-fill",
+        "train-front",
+        "train-front-fill",
+        "train-lightrail-front",
+        "train-lightrail-front-fill",
+        "translate",
         "trash",
-        "trash2-fill",
+        "trash-fill",
         "trash2",
-        "tree-fill",
+        "trash2-fill",
+        "trash3",
+        "trash3-fill",
         "tree",
+        "tree-fill",
+        "trello",
+        "triangle",
         "triangle-fill",
         "triangle-half",
-        "triangle",
-        "trophy-fill",
         "trophy",
+        "trophy-fill",
         "tropical-storm",
-        "truck-flatbed",
         "truck",
+        "truck-flatbed",
+        "truck-front",
+        "truck-front-fill",
         "tsunami",
-        "tv-fill",
         "tv",
+        "tv-fill",
         "twitch",
         "twitter",
+        "type",
         "type-bold",
         "type-h1",
         "type-h2",
         "type-h3",
         "type-italic",
         "type-strikethrough",
         "type-underline",
-        "type",
-        "ui-checks-grid",
+        "ubuntu",
         "ui-checks",
-        "ui-radios-grid",
+        "ui-checks-grid",
         "ui-radios",
-        "umbrella-fill",
+        "ui-radios-grid",
         "umbrella",
+        "umbrella-fill",
+        "unindent",
         "union",
-        "unlock-fill",
+        "unity",
+        "universal-access",
+        "universal-access-circle",
         "unlock",
-        "upc-scan",
+        "unlock-fill",
         "upc",
+        "upc-scan",
         "upload",
+        "usb",
+        "usb-c",
+        "usb-c-fill",
+        "usb-drive",
+        "usb-drive-fill",
+        "usb-fill",
+        "usb-micro",
+        "usb-micro-fill",
+        "usb-mini",
+        "usb-mini-fill",
+        "usb-plug",
+        "usb-plug-fill",
+        "usb-symbol",
+        "valentine",
+        "valentine2",
         "vector-pen",
         "view-list",
         "view-stacked",
-        "vinyl-fill",
+        "vimeo",
         "vinyl",
+        "vinyl-fill",
+        "virus",
+        "virus2",
         "voicemail",
-        "volume-down-fill",
         "volume-down",
-        "volume-mute-fill",
+        "volume-down-fill",
         "volume-mute",
-        "volume-off-fill",
+        "volume-mute-fill",
         "volume-off",
-        "volume-up-fill",
+        "volume-off-fill",
         "volume-up",
+        "volume-up-fill",
         "vr",
-        "wallet-fill",
         "wallet",
+        "wallet-fill",
         "wallet2",
         "watch",
         "water",
+        "webcam",
+        "webcam-fill",
+        "wechat",
         "whatsapp",
+        "wifi",
         "wifi-1",
         "wifi-2",
         "wifi-off",
-        "wifi",
+        "wikipedia",
         "wind",
-        "window-dock",
-        "window-sidebar",
         "window",
-        "wrench",
-        "x-circle-fill",
-        "x-circle",
-        "x-diamond-fill",
-        "x-diamond",
-        "x-octagon-fill",
-        "x-octagon",
-        "x-square-fill",
-        "x-square",
-        "x",
-        "youtube",
-        "zoom-in",
-        "zoom-out",
-        "bank",
-        "bank2",
-        "bell-slash-fill",
-        "bell-slash",
-        "cash-coin",
-        "check-lg",
-        "coin",
-        "currency-bitcoin",
-        "currency-dollar",
-        "currency-euro",
-        "currency-exchange",
-        "currency-pound",
-        "currency-yen",
-        "dash-lg",
-        "exclamation-lg",
-        "file-earmark-pdf-fill",
-        "file-earmark-pdf",
-        "file-pdf-fill",
-        "file-pdf",
-        "gender-ambiguous",
-        "gender-female",
-        "gender-male",
-        "gender-trans",
-        "headset-vr",
-        "info-lg",
-        "mastodon",
-        "messenger",
-        "piggy-bank-fill",
-        "piggy-bank",
-        "pin-map-fill",
-        "pin-map",
-        "plus-lg",
-        "question-lg",
-        "recycle",
-        "reddit",
-        "safe-fill",
-        "safe2-fill",
-        "safe2",
-        "sd-card-fill",
-        "sd-card",
-        "skype",
-        "slash-lg",
-        "translate",
-        "x-lg",
-        "safe",
-        "apple",
-        "microsoft",
-        "windows",
-        "behance",
-        "dribbble",
-        "line",
-        "medium",
-        "paypal",
-        "pinterest",
-        "signal",
-        "snapchat",
-        "spotify",
-        "stack-overflow",
-        "strava",
-        "wordpress",
-        "vimeo",
-        "activity",
-        "easel2-fill",
-        "easel2",
-        "easel3-fill",
-        "easel3",
-        "fan",
-        "fingerprint",
-        "graph-down-arrow",
-        "graph-up-arrow",
-        "hypnotize",
-        "magic",
-        "person-rolodex",
-        "person-video",
-        "person-video2",
-        "person-video3",
-        "person-workspace",
-        "radioactive",
-        "webcam-fill",
-        "webcam",
-        "yin-yang",
-        "bandaid-fill",
-        "bandaid",
-        "bluetooth",
-        "body-text",
-        "boombox",
-        "boxes",
-        "dpad-fill",
-        "dpad",
-        "ear-fill",
-        "ear",
-        "envelope-check-1",
-        "envelope-check-fill",
-        "envelope-check",
-        "envelope-dash-1",
-        "envelope-dash-fill",
-        "envelope-dash",
-        "envelope-exclamation-1",
-        "envelope-exclamation-fill",
-        "envelope-exclamation",
-        "envelope-plus-fill",
-        "envelope-plus",
-        "envelope-slash-1",
-        "envelope-slash-fill",
-        "envelope-slash",
-        "envelope-x-1",
-        "envelope-x-fill",
-        "envelope-x",
-        "explicit-fill",
-        "explicit",
-        "git",
-        "infinity",
-        "list-columns-reverse",
-        "list-columns",
-        "meta",
-        "mortorboard-fill",
-        "mortorboard",
-        "nintendo-switch",
-        "pc-display-horizontal",
-        "pc-display",
-        "pc-horizontal",
-        "pc",
-        "playstation",
-        "plus-slash-minus",
-        "projector-fill",
-        "projector",
-        "qr-code-scan",
-        "qr-code",
-        "quora",
-        "quote",
-        "robot",
-        "send-check-fill",
-        "send-check",
-        "send-dash-fill",
-        "send-dash",
-        "send-exclamation-1",
-        "send-exclamation-fill",
-        "send-exclamation",
-        "send-fill",
-        "send-plus-fill",
-        "send-plus",
-        "send-slash-fill",
-        "send-slash",
-        "send-x-fill",
-        "send-x",
-        "send",
-        "steam",
-        "terminal-dash-1",
-        "terminal-dash",
-        "terminal-plus",
-        "terminal-split",
-        "ticket-detailed-fill",
-        "ticket-detailed",
-        "ticket-fill",
-        "ticket-perforated-fill",
-        "ticket-perforated",
-        "ticket",
-        "tiktok",
         "window-dash",
         "window-desktop",
+        "window-dock",
         "window-fullscreen",
         "window-plus",
+        "window-sidebar",
         "window-split",
         "window-stack",
         "window-x",
-        "xbox",
-        "ethernet",
-        "hdmi-fill",
-        "hdmi",
-        "usb-c-fill",
-        "usb-c",
-        "usb-fill",
-        "usb-plug-fill",
-        "usb-plug",
-        "usb-symbol",
-        "usb",
-        "boombox-fill",
-        "displayport-1",
-        "displayport",
-        "gpu-card",
-        "memory",
-        "modem-fill",
-        "modem",
-        "motherboard-fill",
-        "motherboard",
-        "optical-audio-fill",
-        "optical-audio",
-        "pci-card",
-        "router-fill",
-        "router",
-        "ssd-fill",
-        "ssd",
-        "thunderbolt-fill",
-        "thunderbolt",
-        "usb-drive-fill",
-        "usb-drive",
-        "usb-micro-fill",
-        "usb-micro",
-        "usb-mini-fill",
-        "usb-mini",
-        "cloud-haze2",
-        "device-hdd-fill",
-        "device-hdd",
-        "device-ssd-fill",
-        "device-ssd",
-        "displayport-fill",
-        "mortarboard-fill",
-        "mortarboard",
-        "terminal-x",
-        "arrow-through-heart-fill",
-        "arrow-through-heart",
-        "badge-sd-fill",
-        "badge-sd",
-        "bag-heart-fill",
-        "bag-heart",
-        "balloon-fill",
-        "balloon-heart-fill",
-        "balloon-heart",
-        "balloon",
-        "box2-fill",
-        "box2-heart-fill",
-        "box2-heart",
-        "box2",
-        "braces-asterisk",
-        "calendar-heart-fill",
-        "calendar-heart",
-        "calendar2-heart-fill",
-        "calendar2-heart",
-        "chat-heart-fill",
-        "chat-heart",
-        "chat-left-heart-fill",
-        "chat-left-heart",
-        "chat-right-heart-fill",
-        "chat-right-heart",
-        "chat-square-heart-fill",
-        "chat-square-heart",
-        "clipboard-check-fill",
-        "clipboard-data-fill",
-        "clipboard-fill",
-        "clipboard-heart-fill",
-        "clipboard-heart",
-        "clipboard-minus-fill",
-        "clipboard-plus-fill",
-        "clipboard-pulse",
-        "clipboard-x-fill",
-        "clipboard2-check-fill",
-        "clipboard2-check",
-        "clipboard2-data-fill",
-        "clipboard2-data",
-        "clipboard2-fill",
-        "clipboard2-heart-fill",
-        "clipboard2-heart",
-        "clipboard2-minus-fill",
-        "clipboard2-minus",
-        "clipboard2-plus-fill",
-        "clipboard2-plus",
-        "clipboard2-pulse-fill",
-        "clipboard2-pulse",
-        "clipboard2-x-fill",
-        "clipboard2-x",
-        "clipboard2",
-        "emoji-kiss-fill",
-        "emoji-kiss",
-        "envelope-heart-fill",
-        "envelope-heart",
-        "envelope-open-heart-fill",
-        "envelope-open-heart",
-        "envelope-paper-fill",
-        "envelope-paper-heart-fill",
-        "envelope-paper-heart",
-        "envelope-paper",
-        "filetype-aac",
-        "filetype-ai",
-        "filetype-bmp",
-        "filetype-cs",
-        "filetype-css",
-        "filetype-csv",
-        "filetype-doc",
-        "filetype-docx",
-        "filetype-exe",
-        "filetype-gif",
-        "filetype-heic",
-        "filetype-html",
-        "filetype-java",
-        "filetype-jpg",
-        "filetype-js",
-        "filetype-jsx",
-        "filetype-key",
-        "filetype-m4p",
-        "filetype-md",
-        "filetype-mdx",
-        "filetype-mov",
-        "filetype-mp3",
-        "filetype-mp4",
-        "filetype-otf",
-        "filetype-pdf",
-        "filetype-php",
-        "filetype-png",
-        "filetype-ppt-1",
-        "filetype-ppt",
-        "filetype-psd",
-        "filetype-py",
-        "filetype-raw",
-        "filetype-rb",
-        "filetype-sass",
-        "filetype-scss",
-        "filetype-sh",
-        "filetype-svg",
-        "filetype-tiff",
-        "filetype-tsx",
-        "filetype-ttf",
-        "filetype-txt",
-        "filetype-wav",
-        "filetype-woff",
-        "filetype-xls-1",
-        "filetype-xls",
-        "filetype-xml",
-        "filetype-yml",
-        "heart-arrow",
-        "heart-pulse-fill",
-        "heart-pulse",
-        "heartbreak-fill",
-        "heartbreak",
-        "hearts",
-        "hospital-fill",
-        "hospital",
-        "house-heart-fill",
-        "house-heart",
-        "incognito",
-        "magnet-fill",
-        "magnet",
-        "person-heart",
-        "person-hearts",
-        "phone-flip",
-        "plugin",
-        "postage-fill",
-        "postage-heart-fill",
-        "postage-heart",
-        "postage",
-        "postcard-fill",
-        "postcard-heart-fill",
-        "postcard-heart",
-        "postcard",
-        "search-heart-fill",
-        "search-heart",
-        "sliders2-vertical",
-        "sliders2",
-        "trash3-fill",
-        "trash3",
-        "valentine",
-        "valentine2",
-        "wrench-adjustable-circle-fill",
-        "wrench-adjustable-circle",
+        "windows",
+        "wordpress",
+        "wrench",
         "wrench-adjustable",
-        "filetype-json",
-        "filetype-pptx",
-        "filetype-xlsx"
+        "wrench-adjustable-circle",
+        "wrench-adjustable-circle-fill",
+        "x",
+        "x-circle",
+        "x-circle-fill",
+        "x-diamond",
+        "x-diamond-fill",
+        "x-lg",
+        "x-octagon",
+        "x-octagon-fill",
+        "x-square",
+        "x-square-fill",
+        "xbox",
+        "yelp",
+        "yin-yang",
+        "youtube",
+        "zoom-in",
+        "zoom-out"
     ],
     "list-icon": "bi bi-badge1",
-    "prefix": "bi bi-"
+    "prefix": "bi bi-",
+    "version": "1.10.3"
 }
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7285714285714285%*

 * *Differences: {"'icons'": "{insert: [(0, '0-circle'), (1, '0-circle-fill'), (2, '0-square'), (3, "*

 * *            "'0-square-fill'), (4, '1-circle'), (5, '1-circle-fill'), (6, '1-square'), (7, "*

 * *            "'1-square-fill'), (9, '2-circle'), (10, '2-circle-fill'), (11, '2-square'), (12, "*

 * *            "'2-square-fill'), (13, '3-circle'), (14, '3-circle-fill'), (15, '3-square'), (16, "*

 * *            "'3-square-fill'), (17, '4-circle'), (18, '4-circle-fill'), (19, '4-square'), (20, "*

 * *            "'4-square-fill'), (21, '5-circl […]*

```diff
@@ -1,381 +1,518 @@
 {
     "icon-style": "bi",
     "icons": [
+        "0-circle",
+        "0-circle-fill",
+        "0-square",
+        "0-square-fill",
+        "1-circle",
+        "1-circle-fill",
+        "1-square",
+        "1-square-fill",
         "123",
-        "alarm-fill",
+        "2-circle",
+        "2-circle-fill",
+        "2-square",
+        "2-square-fill",
+        "3-circle",
+        "3-circle-fill",
+        "3-square",
+        "3-square-fill",
+        "4-circle",
+        "4-circle-fill",
+        "4-square",
+        "4-square-fill",
+        "5-circle",
+        "5-circle-fill",
+        "5-square",
+        "5-square-fill",
+        "6-circle",
+        "6-circle-fill",
+        "6-square",
+        "6-square-fill",
+        "7-circle",
+        "7-circle-fill",
+        "7-square",
+        "7-square-fill",
+        "8-circle",
+        "8-circle-fill",
+        "8-square",
+        "8-square-fill",
+        "9-circle",
+        "9-circle-fill",
+        "9-square",
+        "9-square-fill",
+        "activity",
+        "airplane",
+        "airplane-engines",
+        "airplane-engines-fill",
+        "airplane-fill",
         "alarm",
+        "alarm-fill",
+        "alexa",
         "align-bottom",
         "align-center",
         "align-end",
         "align-middle",
         "align-start",
         "align-top",
+        "alipay",
         "alt",
-        "app-indicator",
+        "amd",
+        "android",
+        "android2",
         "app",
-        "archive-fill",
+        "app-indicator",
+        "apple",
         "archive",
+        "archive-fill",
         "arrow-90deg-down",
         "arrow-90deg-left",
         "arrow-90deg-right",
         "arrow-90deg-up",
         "arrow-bar-down",
         "arrow-bar-left",
         "arrow-bar-right",
         "arrow-bar-up",
         "arrow-clockwise",
         "arrow-counterclockwise",
-        "arrow-down-circle-fill",
+        "arrow-down",
         "arrow-down-circle",
-        "arrow-down-left-circle-fill",
+        "arrow-down-circle-fill",
         "arrow-down-left-circle",
-        "arrow-down-left-square-fill",
+        "arrow-down-left-circle-fill",
         "arrow-down-left-square",
-        "arrow-down-left",
-        "arrow-down-right-circle-fill",
+        "arrow-down-left-square-fill",
         "arrow-down-right-circle",
-        "arrow-down-right-square-fill",
+        "arrow-down-right-circle-fill",
         "arrow-down-right-square",
+        "arrow-down-right-square-fill",
+        "arrow-down-square",
+        "arrow-down-square-fill",
+        "arrow-down-left",
         "arrow-down-right",
         "arrow-down-short",
-        "arrow-down-square-fill",
-        "arrow-down-square",
         "arrow-down-up",
-        "arrow-down",
-        "arrow-left-circle-fill",
+        "arrow-left",
         "arrow-left-circle",
+        "arrow-left-circle-fill",
+        "arrow-left-square",
+        "arrow-left-square-fill",
         "arrow-left-right",
         "arrow-left-short",
-        "arrow-left-square-fill",
-        "arrow-left-square",
-        "arrow-left",
         "arrow-repeat",
         "arrow-return-left",
         "arrow-return-right",
-        "arrow-right-circle-fill",
+        "arrow-right",
         "arrow-right-circle",
-        "arrow-right-short",
-        "arrow-right-square-fill",
+        "arrow-right-circle-fill",
         "arrow-right-square",
-        "arrow-right",
-        "arrow-up-circle-fill",
+        "arrow-right-square-fill",
+        "arrow-right-short",
+        "arrow-through-heart",
+        "arrow-through-heart-fill",
+        "arrow-up",
         "arrow-up-circle",
-        "arrow-up-left-circle-fill",
+        "arrow-up-circle-fill",
         "arrow-up-left-circle",
-        "arrow-up-left-square-fill",
+        "arrow-up-left-circle-fill",
         "arrow-up-left-square",
-        "arrow-up-left",
-        "arrow-up-right-circle-fill",
+        "arrow-up-left-square-fill",
         "arrow-up-right-circle",
-        "arrow-up-right-square-fill",
+        "arrow-up-right-circle-fill",
         "arrow-up-right-square",
+        "arrow-up-right-square-fill",
+        "arrow-up-square",
+        "arrow-up-square-fill",
+        "arrow-up-left",
         "arrow-up-right",
         "arrow-up-short",
-        "arrow-up-square-fill",
-        "arrow-up-square",
-        "arrow-up",
         "arrows-angle-contract",
         "arrows-angle-expand",
         "arrows-collapse",
         "arrows-expand",
         "arrows-fullscreen",
         "arrows-move",
-        "aspect-ratio-fill",
         "aspect-ratio",
+        "aspect-ratio-fill",
         "asterisk",
         "at",
-        "award-fill",
         "award",
+        "award-fill",
         "back",
+        "backspace",
         "backspace-fill",
-        "backspace-reverse-fill",
         "backspace-reverse",
-        "backspace",
-        "badge-3d-fill",
+        "backspace-reverse-fill",
         "badge-3d",
-        "badge-4k-fill",
+        "badge-3d-fill",
         "badge-4k",
-        "badge-8k-fill",
+        "badge-4k-fill",
         "badge-8k",
-        "badge-ad-fill",
+        "badge-8k-fill",
         "badge-ad",
-        "badge-ar-fill",
+        "badge-ad-fill",
         "badge-ar",
-        "badge-cc-fill",
+        "badge-ar-fill",
         "badge-cc",
-        "badge-hd-fill",
+        "badge-cc-fill",
         "badge-hd",
-        "badge-tm-fill",
+        "badge-hd-fill",
+        "badge-sd",
+        "badge-sd-fill",
         "badge-tm",
-        "badge-vo-fill",
+        "badge-tm-fill",
         "badge-vo",
-        "badge-vr-fill",
+        "badge-vo-fill",
         "badge-vr",
-        "badge-wc-fill",
+        "badge-vr-fill",
         "badge-wc",
-        "bag-check-fill",
+        "badge-wc-fill",
+        "bag",
         "bag-check",
-        "bag-dash-fill",
+        "bag-check-fill",
         "bag-dash",
+        "bag-dash-fill",
         "bag-fill",
-        "bag-plus-fill",
+        "bag-heart",
+        "bag-heart-fill",
         "bag-plus",
-        "bag-x-fill",
+        "bag-plus-fill",
         "bag-x",
-        "bag",
+        "bag-x-fill",
+        "balloon",
+        "balloon-fill",
+        "balloon-heart",
+        "balloon-heart-fill",
+        "bandaid",
+        "bandaid-fill",
+        "bank",
+        "bank2",
+        "bar-chart",
         "bar-chart-fill",
-        "bar-chart-line-fill",
         "bar-chart-line",
+        "bar-chart-line-fill",
         "bar-chart-steps",
-        "bar-chart",
-        "basket-fill",
         "basket",
-        "basket2-fill",
+        "basket-fill",
         "basket2",
-        "basket3-fill",
+        "basket2-fill",
         "basket3",
+        "basket3-fill",
+        "battery",
         "battery-charging",
         "battery-full",
         "battery-half",
-        "battery",
-        "bell-fill",
+        "behance",
         "bell",
+        "bell-fill",
+        "bell-slash",
+        "bell-slash-fill",
         "bezier",
         "bezier2",
         "bicycle",
-        "binoculars-fill",
         "binoculars",
+        "binoculars-fill",
         "blockquote-left",
         "blockquote-right",
+        "bluetooth",
+        "body-text",
+        "book",
         "book-fill",
         "book-half",
-        "book",
-        "bookmark-check-fill",
+        "bookmark",
         "bookmark-check",
-        "bookmark-dash-fill",
+        "bookmark-check-fill",
         "bookmark-dash",
+        "bookmark-dash-fill",
         "bookmark-fill",
-        "bookmark-heart-fill",
         "bookmark-heart",
-        "bookmark-plus-fill",
+        "bookmark-heart-fill",
         "bookmark-plus",
-        "bookmark-star-fill",
+        "bookmark-plus-fill",
         "bookmark-star",
-        "bookmark-x-fill",
+        "bookmark-star-fill",
         "bookmark-x",
-        "bookmark",
-        "bookmarks-fill",
+        "bookmark-x-fill",
         "bookmarks",
+        "bookmarks-fill",
         "bookshelf",
+        "boombox",
+        "boombox-fill",
+        "bootstrap",
         "bootstrap-fill",
         "bootstrap-reboot",
-        "bootstrap",
+        "border",
         "border-all",
         "border-bottom",
         "border-center",
         "border-inner",
         "border-left",
         "border-middle",
         "border-outer",
         "border-right",
         "border-style",
         "border-top",
         "border-width",
-        "border",
-        "bounding-box-circles",
         "bounding-box",
+        "bounding-box-circles",
+        "box",
         "box-arrow-down-left",
         "box-arrow-down-right",
         "box-arrow-down",
+        "box-arrow-in-down",
         "box-arrow-in-down-left",
         "box-arrow-in-down-right",
-        "box-arrow-in-down",
         "box-arrow-in-left",
         "box-arrow-in-right",
+        "box-arrow-in-up",
         "box-arrow-in-up-left",
         "box-arrow-in-up-right",
-        "box-arrow-in-up",
         "box-arrow-left",
         "box-arrow-right",
+        "box-arrow-up",
         "box-arrow-up-left",
         "box-arrow-up-right",
-        "box-arrow-up",
+        "box-fill",
         "box-seam",
-        "box",
+        "box-seam-fill",
+        "box2",
+        "box2-fill",
+        "box2-heart",
+        "box2-heart-fill",
+        "boxes",
         "braces",
+        "braces-asterisk",
         "bricks",
-        "briefcase-fill",
         "briefcase",
-        "brightness-alt-high-fill",
+        "briefcase-fill",
         "brightness-alt-high",
-        "brightness-alt-low-fill",
+        "brightness-alt-high-fill",
         "brightness-alt-low",
-        "brightness-high-fill",
+        "brightness-alt-low-fill",
         "brightness-high",
-        "brightness-low-fill",
+        "brightness-high-fill",
         "brightness-low",
-        "broadcast-pin",
+        "brightness-low-fill",
         "broadcast",
-        "brush-fill",
+        "broadcast-pin",
+        "browser-chrome",
+        "browser-edge",
+        "browser-firefox",
+        "browser-safari",
         "brush",
-        "bucket-fill",
+        "brush-fill",
         "bucket",
-        "bug-fill",
+        "bucket-fill",
         "bug",
+        "bug-fill",
         "building",
+        "building-add",
+        "building-check",
+        "building-dash",
+        "building-down",
+        "building-exclamation",
+        "building-fill",
+        "building-fill-add",
+        "building-fill-check",
+        "building-fill-dash",
+        "building-fill-down",
+        "building-fill-exclamation",
+        "building-fill-gear",
+        "building-fill-lock",
+        "building-fill-slash",
+        "building-fill-up",
+        "building-fill-x",
+        "building-gear",
+        "building-lock",
+        "building-slash",
+        "building-up",
+        "building-x",
+        "buildings",
+        "buildings-fill",
         "bullseye",
-        "calculator-fill",
+        "bus-front",
+        "bus-front-fill",
+        "c-circle",
+        "c-circle-fill",
+        "c-square",
+        "c-square-fill",
         "calculator",
-        "calendar-check-fill",
+        "calculator-fill",
+        "calendar",
         "calendar-check",
-        "calendar-date-fill",
+        "calendar-check-fill",
         "calendar-date",
-        "calendar-day-fill",
+        "calendar-date-fill",
         "calendar-day",
-        "calendar-event-fill",
+        "calendar-day-fill",
         "calendar-event",
+        "calendar-event-fill",
         "calendar-fill",
-        "calendar-minus-fill",
+        "calendar-heart",
+        "calendar-heart-fill",
         "calendar-minus",
-        "calendar-month-fill",
+        "calendar-minus-fill",
         "calendar-month",
-        "calendar-plus-fill",
+        "calendar-month-fill",
         "calendar-plus",
-        "calendar-range-fill",
+        "calendar-plus-fill",
         "calendar-range",
-        "calendar-week-fill",
+        "calendar-range-fill",
         "calendar-week",
-        "calendar-x-fill",
+        "calendar-week-fill",
         "calendar-x",
-        "calendar",
-        "calendar2-check-fill",
+        "calendar-x-fill",
+        "calendar2",
         "calendar2-check",
-        "calendar2-date-fill",
+        "calendar2-check-fill",
         "calendar2-date",
-        "calendar2-day-fill",
+        "calendar2-date-fill",
         "calendar2-day",
-        "calendar2-event-fill",
+        "calendar2-day-fill",
         "calendar2-event",
+        "calendar2-event-fill",
         "calendar2-fill",
-        "calendar2-minus-fill",
+        "calendar2-heart",
+        "calendar2-heart-fill",
         "calendar2-minus",
-        "calendar2-month-fill",
+        "calendar2-minus-fill",
         "calendar2-month",
-        "calendar2-plus-fill",
+        "calendar2-month-fill",
         "calendar2-plus",
-        "calendar2-range-fill",
+        "calendar2-plus-fill",
         "calendar2-range",
-        "calendar2-week-fill",
+        "calendar2-range-fill",
         "calendar2-week",
-        "calendar2-x-fill",
+        "calendar2-week-fill",
         "calendar2-x",
-        "calendar2",
-        "calendar3-event-fill",
+        "calendar2-x-fill",
+        "calendar3",
         "calendar3-event",
+        "calendar3-event-fill",
         "calendar3-fill",
-        "calendar3-range-fill",
         "calendar3-range",
-        "calendar3-week-fill",
+        "calendar3-range-fill",
         "calendar3-week",
-        "calendar3",
+        "calendar3-week-fill",
+        "calendar4",
         "calendar4-event",
         "calendar4-range",
         "calendar4-week",
-        "calendar4",
+        "camera",
+        "camera2",
         "camera-fill",
-        "camera-reels-fill",
         "camera-reels",
+        "camera-reels-fill",
+        "camera-video",
         "camera-video-fill",
-        "camera-video-off-fill",
         "camera-video-off",
-        "camera-video",
-        "camera",
-        "camera2",
-        "capslock-fill",
+        "camera-video-off-fill",
         "capslock",
+        "capslock-fill",
+        "capsule",
+        "capsule-pill",
+        "car-front",
+        "car-front-fill",
         "card-checklist",
         "card-heading",
         "card-image",
         "card-list",
         "card-text",
+        "caret-down",
         "caret-down-fill",
-        "caret-down-square-fill",
         "caret-down-square",
-        "caret-down",
+        "caret-down-square-fill",
+        "caret-left",
         "caret-left-fill",
-        "caret-left-square-fill",
         "caret-left-square",
-        "caret-left",
+        "caret-left-square-fill",
+        "caret-right",
         "caret-right-fill",
-        "caret-right-square-fill",
         "caret-right-square",
-        "caret-right",
+        "caret-right-square-fill",
+        "caret-up",
         "caret-up-fill",
-        "caret-up-square-fill",
         "caret-up-square",
-        "caret-up",
-        "cart-check-fill",
+        "caret-up-square-fill",
+        "cart",
         "cart-check",
-        "cart-dash-fill",
+        "cart-check-fill",
         "cart-dash",
+        "cart-dash-fill",
         "cart-fill",
-        "cart-plus-fill",
         "cart-plus",
-        "cart-x-fill",
+        "cart-plus-fill",
         "cart-x",
-        "cart",
+        "cart-x-fill",
         "cart2",
         "cart3",
         "cart4",
-        "cash-stack",
         "cash",
+        "cash-coin",
+        "cash-stack",
+        "cassette",
+        "cassette-fill",
         "cast",
-        "chat-dots-fill",
+        "cc-circle",
+        "cc-circle-fill",
+        "cc-square",
+        "cc-square-fill",
+        "chat",
         "chat-dots",
+        "chat-dots-fill",
         "chat-fill",
-        "chat-left-dots-fill",
+        "chat-heart",
+        "chat-heart-fill",
+        "chat-left",
         "chat-left-dots",
+        "chat-left-dots-fill",
         "chat-left-fill",
-        "chat-left-quote-fill",
+        "chat-left-heart",
+        "chat-left-heart-fill",
         "chat-left-quote",
-        "chat-left-text-fill",
+        "chat-left-quote-fill",
         "chat-left-text",
-        "chat-left",
-        "chat-quote-fill",
+        "chat-left-text-fill",
         "chat-quote",
-        "chat-right-dots-fill",
+        "chat-quote-fill",
+        "chat-right",
         "chat-right-dots",
+        "chat-right-dots-fill",
         "chat-right-fill",
-        "chat-right-quote-fill",
+        "chat-right-heart",
+        "chat-right-heart-fill",
         "chat-right-quote",
-        "chat-right-text-fill",
+        "chat-right-quote-fill",
         "chat-right-text",
-        "chat-right",
-        "chat-square-dots-fill",
+        "chat-right-text-fill",
+        "chat-square",
         "chat-square-dots",
+        "chat-square-dots-fill",
         "chat-square-fill",
-        "chat-square-quote-fill",
+        "chat-square-heart",
+        "chat-square-heart-fill",
         "chat-square-quote",
-        "chat-square-text-fill",
+        "chat-square-quote-fill",
         "chat-square-text",
-        "chat-square",
-        "chat-text-fill",
+        "chat-square-text-fill",
         "chat-text",
-        "chat",
+        "chat-text-fill",
+        "check",
         "check-all",
-        "check-circle-fill",
         "check-circle",
-        "check-square-fill",
+        "check-circle-fill",
+        "check-lg",
         "check-square",
-        "check",
+        "check-square-fill",
+        "check2",
         "check2-all",
         "check2-circle",
         "check2-square",
-        "check2",
         "chevron-bar-contract",
         "chevron-bar-down",
         "chevron-bar-expand",
         "chevron-bar-left",
         "chevron-bar-right",
         "chevron-bar-up",
         "chevron-compact-down",
@@ -388,1303 +525,1437 @@
         "chevron-double-right",
         "chevron-double-up",
         "chevron-down",
         "chevron-expand",
         "chevron-left",
         "chevron-right",
         "chevron-up",
+        "circle",
         "circle-fill",
         "circle-half",
+        "slash-circle",
         "circle-square",
-        "circle",
+        "clipboard",
         "clipboard-check",
+        "clipboard-check-fill",
         "clipboard-data",
+        "clipboard-data-fill",
+        "clipboard-fill",
+        "clipboard-heart",
+        "clipboard-heart-fill",
         "clipboard-minus",
+        "clipboard-minus-fill",
         "clipboard-plus",
+        "clipboard-plus-fill",
+        "clipboard-pulse",
         "clipboard-x",
-        "clipboard",
+        "clipboard-x-fill",
+        "clipboard2",
+        "clipboard2-check",
+        "clipboard2-check-fill",
+        "clipboard2-data",
+        "clipboard2-data-fill",
+        "clipboard2-fill",
+        "clipboard2-heart",
+        "clipboard2-heart-fill",
+        "clipboard2-minus",
+        "clipboard2-minus-fill",
+        "clipboard2-plus",
+        "clipboard2-plus-fill",
+        "clipboard2-pulse",
+        "clipboard2-pulse-fill",
+        "clipboard2-x",
+        "clipboard2-x-fill",
+        "clock",
         "clock-fill",
         "clock-history",
-        "clock",
-        "cloud-arrow-down-fill",
+        "cloud",
         "cloud-arrow-down",
-        "cloud-arrow-up-fill",
+        "cloud-arrow-down-fill",
         "cloud-arrow-up",
-        "cloud-check-fill",
+        "cloud-arrow-up-fill",
         "cloud-check",
-        "cloud-download-fill",
+        "cloud-check-fill",
         "cloud-download",
-        "cloud-drizzle-fill",
+        "cloud-download-fill",
         "cloud-drizzle",
+        "cloud-drizzle-fill",
         "cloud-fill",
-        "cloud-fog-fill",
         "cloud-fog",
-        "cloud-fog2-fill",
+        "cloud-fog-fill",
         "cloud-fog2",
-        "cloud-hail-fill",
+        "cloud-fog2-fill",
         "cloud-hail",
-        "cloud-haze-1",
-        "cloud-haze-fill",
+        "cloud-hail-fill",
         "cloud-haze",
+        "cloud-haze-fill",
+        "cloud-haze2",
         "cloud-haze2-fill",
+        "cloud-lightning",
         "cloud-lightning-fill",
-        "cloud-lightning-rain-fill",
         "cloud-lightning-rain",
-        "cloud-lightning",
-        "cloud-minus-fill",
+        "cloud-lightning-rain-fill",
         "cloud-minus",
-        "cloud-moon-fill",
+        "cloud-minus-fill",
         "cloud-moon",
-        "cloud-plus-fill",
+        "cloud-moon-fill",
         "cloud-plus",
+        "cloud-plus-fill",
+        "cloud-rain",
         "cloud-rain-fill",
-        "cloud-rain-heavy-fill",
         "cloud-rain-heavy",
-        "cloud-rain",
-        "cloud-slash-fill",
+        "cloud-rain-heavy-fill",
         "cloud-slash",
-        "cloud-sleet-fill",
+        "cloud-slash-fill",
         "cloud-sleet",
-        "cloud-snow-fill",
+        "cloud-sleet-fill",
         "cloud-snow",
-        "cloud-sun-fill",
+        "cloud-snow-fill",
         "cloud-sun",
-        "cloud-upload-fill",
+        "cloud-sun-fill",
         "cloud-upload",
-        "cloud",
-        "clouds-fill",
+        "cloud-upload-fill",
         "clouds",
-        "cloudy-fill",
+        "clouds-fill",
         "cloudy",
+        "cloudy-fill",
+        "code",
         "code-slash",
         "code-square",
-        "code",
+        "coin",
+        "collection",
         "collection-fill",
-        "collection-play-fill",
         "collection-play",
-        "collection",
-        "columns-gap",
+        "collection-play-fill",
         "columns",
+        "columns-gap",
         "command",
-        "compass-fill",
         "compass",
-        "cone-striped",
+        "compass-fill",
         "cone",
+        "cone-striped",
         "controller",
-        "cpu-fill",
         "cpu",
-        "credit-card-2-back-fill",
+        "cpu-fill",
+        "credit-card",
         "credit-card-2-back",
-        "credit-card-2-front-fill",
+        "credit-card-2-back-fill",
         "credit-card-2-front",
+        "credit-card-2-front-fill",
         "credit-card-fill",
-        "credit-card",
         "crop",
+        "cup",
         "cup-fill",
+        "cup-hot",
+        "cup-hot-fill",
         "cup-straw",
-        "cup",
+        "currency-bitcoin",
+        "currency-dollar",
+        "currency-euro",
+        "currency-exchange",
+        "currency-pound",
+        "currency-rupee",
+        "currency-yen",
+        "cursor",
         "cursor-fill",
         "cursor-text",
-        "cursor",
+        "dash",
+        "dash-circle",
         "dash-circle-dotted",
         "dash-circle-fill",
-        "dash-circle",
+        "dash-lg",
+        "dash-square",
         "dash-square-dotted",
         "dash-square-fill",
-        "dash-square",
-        "dash",
-        "diagram-2-fill",
+        "database",
+        "database-add",
+        "database-check",
+        "database-dash",
+        "database-down",
+        "database-exclamation",
+        "database-fill",
+        "database-fill-add",
+        "database-fill-check",
+        "database-fill-dash",
+        "database-fill-down",
+        "database-fill-exclamation",
+        "database-fill-gear",
+        "database-fill-lock",
+        "database-fill-slash",
+        "database-fill-up",
+        "database-fill-x",
+        "database-gear",
+        "database-lock",
+        "database-slash",
+        "database-up",
+        "database-x",
+        "device-hdd",
+        "device-hdd-fill",
+        "device-ssd",
+        "device-ssd-fill",
         "diagram-2",
-        "diagram-3-fill",
+        "diagram-2-fill",
         "diagram-3",
+        "diagram-3-fill",
+        "diamond",
         "diamond-fill",
         "diamond-half",
-        "diamond",
-        "dice-1-fill",
         "dice-1",
-        "dice-2-fill",
+        "dice-1-fill",
         "dice-2",
-        "dice-3-fill",
+        "dice-2-fill",
         "dice-3",
-        "dice-4-fill",
+        "dice-3-fill",
         "dice-4",
-        "dice-5-fill",
+        "dice-4-fill",
         "dice-5",
-        "dice-6-fill",
+        "dice-5-fill",
         "dice-6",
-        "disc-fill",
+        "dice-6-fill",
         "disc",
+        "disc-fill",
         "discord",
-        "display-fill",
         "display",
+        "display-fill",
+        "displayport",
+        "displayport-fill",
         "distribute-horizontal",
         "distribute-vertical",
-        "door-closed-fill",
         "door-closed",
-        "door-open-fill",
+        "door-closed-fill",
         "door-open",
+        "door-open-fill",
         "dot",
         "download",
+        "dpad",
+        "dpad-fill",
+        "dribbble",
+        "dropbox",
+        "droplet",
         "droplet-fill",
         "droplet-half",
-        "droplet",
+        "ear",
+        "ear-fill",
         "earbuds",
-        "easel-fill",
         "easel",
+        "easel-fill",
+        "easel2",
+        "easel2-fill",
+        "easel3",
+        "easel3-fill",
+        "egg",
         "egg-fill",
         "egg-fried",
-        "egg",
-        "eject-fill",
         "eject",
-        "emoji-angry-fill",
+        "eject-fill",
         "emoji-angry",
-        "emoji-dizzy-fill",
+        "emoji-angry-fill",
         "emoji-dizzy",
-        "emoji-expressionless-fill",
+        "emoji-dizzy-fill",
         "emoji-expressionless",
-        "emoji-frown-fill",
+        "emoji-expressionless-fill",
         "emoji-frown",
-        "emoji-heart-eyes-fill",
+        "emoji-frown-fill",
         "emoji-heart-eyes",
-        "emoji-laughing-fill",
+        "emoji-heart-eyes-fill",
+        "emoji-kiss",
+        "emoji-kiss-fill",
         "emoji-laughing",
-        "emoji-neutral-fill",
+        "emoji-laughing-fill",
         "emoji-neutral",
+        "emoji-neutral-fill",
+        "emoji-smile",
         "emoji-smile-fill",
-        "emoji-smile-upside-down-fill",
         "emoji-smile-upside-down",
-        "emoji-smile",
-        "emoji-sunglasses-fill",
+        "emoji-smile-upside-down-fill",
         "emoji-sunglasses",
-        "emoji-wink-fill",
+        "emoji-sunglasses-fill",
         "emoji-wink",
+        "emoji-wink-fill",
+        "envelope",
+        "envelope-at",
+        "envelope-at-fill",
+        "envelope-check",
+        "envelope-check-fill",
+        "envelope-dash",
+        "envelope-dash-fill",
+        "envelope-exclamation",
+        "envelope-exclamation-fill",
         "envelope-fill",
-        "envelope-open-fill",
+        "envelope-heart",
+        "envelope-heart-fill",
         "envelope-open",
-        "envelope",
-        "eraser-fill",
+        "envelope-open-fill",
+        "envelope-open-heart",
+        "envelope-open-heart-fill",
+        "envelope-paper",
+        "envelope-paper-fill",
+        "envelope-paper-heart",
+        "envelope-paper-heart-fill",
+        "envelope-plus",
+        "envelope-plus-fill",
+        "envelope-slash",
+        "envelope-slash-fill",
+        "envelope-x",
+        "envelope-x-fill",
         "eraser",
-        "exclamation-circle-fill",
+        "eraser-fill",
+        "escape",
+        "ethernet",
+        "ev-front",
+        "ev-front-fill",
+        "ev-station",
+        "ev-station-fill",
+        "exclamation",
         "exclamation-circle",
-        "exclamation-diamond-fill",
+        "exclamation-circle-fill",
         "exclamation-diamond",
-        "exclamation-octagon-fill",
+        "exclamation-diamond-fill",
+        "exclamation-lg",
         "exclamation-octagon",
-        "exclamation-square-fill",
+        "exclamation-octagon-fill",
         "exclamation-square",
-        "exclamation-triangle-fill",
+        "exclamation-square-fill",
         "exclamation-triangle",
-        "exclamation",
+        "exclamation-triangle-fill",
         "exclude",
+        "explicit",
+        "explicit-fill",
+        "eye",
         "eye-fill",
-        "eye-slash-fill",
         "eye-slash",
-        "eye",
+        "eye-slash-fill",
         "eyedropper",
         "eyeglasses",
         "facebook",
-        "file-arrow-down-fill",
+        "fan",
+        "fast-forward",
+        "fast-forward-btn",
+        "fast-forward-btn-fill",
+        "fast-forward-circle",
+        "fast-forward-circle-fill",
+        "fast-forward-fill",
+        "file",
         "file-arrow-down",
-        "file-arrow-up-fill",
+        "file-arrow-down-fill",
         "file-arrow-up",
-        "file-bar-graph-fill",
+        "file-arrow-up-fill",
         "file-bar-graph",
-        "file-binary-fill",
+        "file-bar-graph-fill",
         "file-binary",
-        "file-break-fill",
+        "file-binary-fill",
         "file-break",
-        "file-check-fill",
+        "file-break-fill",
         "file-check",
-        "file-code-fill",
+        "file-check-fill",
         "file-code",
-        "file-diff-fill",
+        "file-code-fill",
         "file-diff",
-        "file-earmark-arrow-down-fill",
+        "file-diff-fill",
+        "file-earmark",
         "file-earmark-arrow-down",
-        "file-earmark-arrow-up-fill",
+        "file-earmark-arrow-down-fill",
         "file-earmark-arrow-up",
-        "file-earmark-bar-graph-fill",
+        "file-earmark-arrow-up-fill",
         "file-earmark-bar-graph",
-        "file-earmark-binary-fill",
+        "file-earmark-bar-graph-fill",
         "file-earmark-binary",
-        "file-earmark-break-fill",
+        "file-earmark-binary-fill",
         "file-earmark-break",
-        "file-earmark-check-fill",
+        "file-earmark-break-fill",
         "file-earmark-check",
-        "file-earmark-code-fill",
+        "file-earmark-check-fill",
         "file-earmark-code",
-        "file-earmark-diff-fill",
+        "file-earmark-code-fill",
         "file-earmark-diff",
-        "file-earmark-easel-fill",
+        "file-earmark-diff-fill",
         "file-earmark-easel",
-        "file-earmark-excel-fill",
+        "file-earmark-easel-fill",
         "file-earmark-excel",
+        "file-earmark-excel-fill",
         "file-earmark-fill",
-        "file-earmark-font-fill",
         "file-earmark-font",
-        "file-earmark-image-fill",
+        "file-earmark-font-fill",
         "file-earmark-image",
-        "file-earmark-lock-fill",
+        "file-earmark-image-fill",
         "file-earmark-lock",
-        "file-earmark-lock2-fill",
+        "file-earmark-lock-fill",
         "file-earmark-lock2",
-        "file-earmark-medical-fill",
+        "file-earmark-lock2-fill",
         "file-earmark-medical",
-        "file-earmark-minus-fill",
+        "file-earmark-medical-fill",
         "file-earmark-minus",
-        "file-earmark-music-fill",
+        "file-earmark-minus-fill",
         "file-earmark-music",
-        "file-earmark-person-fill",
+        "file-earmark-music-fill",
+        "file-earmark-pdf",
+        "file-earmark-pdf-fill",
         "file-earmark-person",
-        "file-earmark-play-fill",
+        "file-earmark-person-fill",
         "file-earmark-play",
-        "file-earmark-plus-fill",
+        "file-earmark-play-fill",
         "file-earmark-plus",
-        "file-earmark-post-fill",
+        "file-earmark-plus-fill",
         "file-earmark-post",
-        "file-earmark-ppt-fill",
+        "file-earmark-post-fill",
         "file-earmark-ppt",
-        "file-earmark-richtext-fill",
+        "file-earmark-ppt-fill",
         "file-earmark-richtext",
-        "file-earmark-ruled-fill",
+        "file-earmark-richtext-fill",
         "file-earmark-ruled",
-        "file-earmark-slides-fill",
+        "file-earmark-ruled-fill",
         "file-earmark-slides",
-        "file-earmark-spreadsheet-fill",
+        "file-earmark-slides-fill",
         "file-earmark-spreadsheet",
-        "file-earmark-text-fill",
+        "file-earmark-spreadsheet-fill",
         "file-earmark-text",
-        "file-earmark-word-fill",
+        "file-earmark-text-fill",
         "file-earmark-word",
-        "file-earmark-x-fill",
+        "file-earmark-word-fill",
         "file-earmark-x",
-        "file-earmark-zip-fill",
+        "file-earmark-x-fill",
         "file-earmark-zip",
-        "file-earmark",
-        "file-easel-fill",
+        "file-earmark-zip-fill",
         "file-easel",
-        "file-excel-fill",
+        "file-easel-fill",
         "file-excel",
+        "file-excel-fill",
         "file-fill",
-        "file-font-fill",
         "file-font",
-        "file-image-fill",
+        "file-font-fill",
         "file-image",
-        "file-lock-fill",
+        "file-image-fill",
         "file-lock",
-        "file-lock2-fill",
+        "file-lock-fill",
         "file-lock2",
-        "file-medical-fill",
+        "file-lock2-fill",
         "file-medical",
-        "file-minus-fill",
+        "file-medical-fill",
         "file-minus",
-        "file-music-fill",
+        "file-minus-fill",
         "file-music",
-        "file-person-fill",
+        "file-music-fill",
+        "file-pdf",
+        "file-pdf-fill",
         "file-person",
-        "file-play-fill",
+        "file-person-fill",
         "file-play",
-        "file-plus-fill",
+        "file-play-fill",
         "file-plus",
-        "file-post-fill",
+        "file-plus-fill",
         "file-post",
-        "file-ppt-fill",
+        "file-post-fill",
         "file-ppt",
-        "file-richtext-fill",
+        "file-ppt-fill",
         "file-richtext",
-        "file-ruled-fill",
+        "file-richtext-fill",
         "file-ruled",
-        "file-slides-fill",
+        "file-ruled-fill",
         "file-slides",
-        "file-spreadsheet-fill",
+        "file-slides-fill",
         "file-spreadsheet",
-        "file-text-fill",
+        "file-spreadsheet-fill",
         "file-text",
-        "file-word-fill",
+        "file-text-fill",
         "file-word",
-        "file-x-fill",
+        "file-word-fill",
         "file-x",
-        "file-zip-fill",
+        "file-x-fill",
         "file-zip",
-        "file",
-        "files-alt",
+        "file-zip-fill",
         "files",
+        "files-alt",
+        "filetype-aac",
+        "filetype-ai",
+        "filetype-bmp",
+        "filetype-cs",
+        "filetype-css",
+        "filetype-csv",
+        "filetype-doc",
+        "filetype-docx",
+        "filetype-exe",
+        "filetype-gif",
+        "filetype-heic",
+        "filetype-html",
+        "filetype-java",
+        "filetype-jpg",
+        "filetype-js",
+        "filetype-json",
+        "filetype-jsx",
+        "filetype-key",
+        "filetype-m4p",
+        "filetype-md",
+        "filetype-mdx",
+        "filetype-mov",
+        "filetype-mp3",
+        "filetype-mp4",
+        "filetype-otf",
+        "filetype-pdf",
+        "filetype-php",
+        "filetype-png",
+        "filetype-ppt",
+        "filetype-pptx",
+        "filetype-psd",
+        "filetype-py",
+        "filetype-raw",
+        "filetype-rb",
+        "filetype-sass",
+        "filetype-scss",
+        "filetype-sh",
+        "filetype-sql",
+        "filetype-svg",
+        "filetype-tiff",
+        "filetype-tsx",
+        "filetype-ttf",
+        "filetype-txt",
+        "filetype-wav",
+        "filetype-woff",
+        "filetype-xls",
+        "filetype-xlsx",
+        "filetype-xml",
+        "filetype-yml",
         "film",
-        "filter-circle-fill",
+        "filter",
         "filter-circle",
+        "filter-circle-fill",
         "filter-left",
         "filter-right",
-        "filter-square-fill",
         "filter-square",
-        "filter",
-        "flag-fill",
+        "filter-square-fill",
+        "fingerprint",
+        "fire",
         "flag",
+        "flag-fill",
         "flower1",
         "flower2",
         "flower3",
+        "folder",
         "folder-check",
         "folder-fill",
         "folder-minus",
         "folder-plus",
-        "folder-symlink-fill",
         "folder-symlink",
+        "folder-symlink-fill",
         "folder-x",
-        "folder",
-        "folder2-open",
         "folder2",
+        "folder2-open",
         "fonts",
-        "forward-fill",
         "forward",
+        "forward-fill",
         "front",
-        "fullscreen-exit",
+        "fuel-pump",
+        "fuel-pump-diesel",
+        "fuel-pump-diesel-fill",
+        "fuel-pump-fill",
         "fullscreen",
-        "funnel-fill",
+        "fullscreen-exit",
         "funnel",
+        "funnel-fill",
+        "gear",
         "gear-fill",
-        "gear-wide-connected",
         "gear-wide",
-        "gear",
+        "gear-wide-connected",
         "gem",
-        "geo-alt-fill",
+        "gender-ambiguous",
+        "gender-female",
+        "gender-male",
+        "gender-trans",
+        "geo",
         "geo-alt",
+        "geo-alt-fill",
         "geo-fill",
-        "geo",
-        "gift-fill",
         "gift",
+        "gift-fill",
+        "git",
         "github",
         "globe",
+        "globe-americas",
+        "globe-asia-australia",
+        "globe-central-south-asia",
+        "globe-europe-africa",
         "globe2",
         "google",
+        "google-play",
+        "gpu-card",
         "graph-down",
+        "graph-down-arrow",
         "graph-up",
-        "grid-1x2-fill",
+        "graph-up-arrow",
+        "grid",
         "grid-1x2",
-        "grid-3x2-gap-fill",
-        "grid-3x2-gap",
+        "grid-1x2-fill",
         "grid-3x2",
-        "grid-3x3-gap-fill",
-        "grid-3x3-gap",
+        "grid-3x2-gap",
+        "grid-3x2-gap-fill",
         "grid-3x3",
+        "grid-3x3-gap",
+        "grid-3x3-gap-fill",
         "grid-fill",
-        "grid",
         "grip-horizontal",
         "grip-vertical",
+        "h-circle",
+        "h-circle-fill",
+        "h-square",
+        "h-square-fill",
         "hammer",
+        "hand-index",
         "hand-index-fill",
-        "hand-index-thumb-fill",
         "hand-index-thumb",
-        "hand-index",
-        "hand-thumbs-down-fill",
+        "hand-index-thumb-fill",
         "hand-thumbs-down",
-        "hand-thumbs-up-fill",
+        "hand-thumbs-down-fill",
         "hand-thumbs-up",
-        "handbag-fill",
+        "hand-thumbs-up-fill",
         "handbag",
+        "handbag-fill",
         "hash",
+        "hdd",
         "hdd-fill",
-        "hdd-network-fill",
         "hdd-network",
-        "hdd-rack-fill",
+        "hdd-network-fill",
         "hdd-rack",
-        "hdd-stack-fill",
+        "hdd-rack-fill",
         "hdd-stack",
-        "hdd",
+        "hdd-stack-fill",
+        "hdmi",
+        "hdmi-fill",
         "headphones",
         "headset",
+        "headset-vr",
+        "heart",
+        "heart-arrow",
         "heart-fill",
         "heart-half",
-        "heart",
+        "heart-pulse",
+        "heart-pulse-fill",
+        "heartbreak",
+        "heartbreak-fill",
+        "hearts",
+        "heptagon",
         "heptagon-fill",
         "heptagon-half",
-        "heptagon",
+        "hexagon",
         "hexagon-fill",
         "hexagon-half",
-        "hexagon",
+        "hospital",
+        "hospital-fill",
+        "hourglass",
         "hourglass-bottom",
         "hourglass-split",
         "hourglass-top",
-        "hourglass",
-        "house-door-fill",
+        "house",
+        "house-add",
+        "house-add-fill",
+        "house-check",
+        "house-check-fill",
+        "house-dash",
+        "house-dash-fill",
         "house-door",
+        "house-door-fill",
+        "house-down",
+        "house-down-fill",
+        "house-exclamation",
+        "house-exclamation-fill",
         "house-fill",
-        "house",
+        "house-gear",
+        "house-gear-fill",
+        "house-heart",
+        "house-heart-fill",
+        "house-lock",
+        "house-lock-fill",
+        "house-slash",
+        "house-slash-fill",
+        "house-up",
+        "house-up-fill",
+        "house-x",
+        "house-x-fill",
+        "houses",
+        "houses-fill",
         "hr",
         "hurricane",
+        "hypnotize",
+        "image",
         "image-alt",
         "image-fill",
-        "image",
         "images",
-        "inbox-fill",
         "inbox",
+        "inbox-fill",
         "inboxes-fill",
         "inboxes",
-        "info-circle-fill",
+        "incognito",
+        "indent",
+        "infinity",
+        "info",
         "info-circle",
-        "info-square-fill",
+        "info-circle-fill",
+        "info-lg",
         "info-square",
-        "info",
-        "input-cursor-text",
+        "info-square-fill",
         "input-cursor",
+        "input-cursor-text",
         "instagram",
         "intersect",
+        "journal",
         "journal-album",
         "journal-arrow-down",
         "journal-arrow-up",
-        "journal-bookmark-fill",
         "journal-bookmark",
+        "journal-bookmark-fill",
         "journal-check",
         "journal-code",
         "journal-medical",
         "journal-minus",
         "journal-plus",
         "journal-richtext",
         "journal-text",
         "journal-x",
-        "journal",
         "journals",
         "joystick",
+        "justify",
         "justify-left",
         "justify-right",
-        "justify",
-        "kanban-fill",
         "kanban",
-        "key-fill",
+        "kanban-fill",
         "key",
-        "keyboard-fill",
+        "key-fill",
         "keyboard",
+        "keyboard-fill",
         "ladder",
-        "lamp-fill",
         "lamp",
-        "laptop-fill",
+        "lamp-fill",
         "laptop",
+        "laptop-fill",
         "layer-backward",
         "layer-forward",
+        "layers",
         "layers-fill",
         "layers-half",
-        "layers",
+        "layout-sidebar",
         "layout-sidebar-inset-reverse",
         "layout-sidebar-inset",
         "layout-sidebar-reverse",
-        "layout-sidebar",
         "layout-split",
-        "layout-text-sidebar-reverse",
         "layout-text-sidebar",
-        "layout-text-window-reverse",
+        "layout-text-sidebar-reverse",
         "layout-text-window",
+        "layout-text-window-reverse",
         "layout-three-columns",
         "layout-wtf",
         "life-preserver",
+        "lightbulb",
         "lightbulb-fill",
-        "lightbulb-off-fill",
         "lightbulb-off",
-        "lightbulb",
-        "lightning-charge-fill",
+        "lightbulb-off-fill",
+        "lightning",
         "lightning-charge",
+        "lightning-charge-fill",
         "lightning-fill",
-        "lightning",
-        "link-45deg",
+        "line",
         "link",
+        "link-45deg",
         "linkedin",
+        "list",
         "list-check",
+        "list-columns",
+        "list-columns-reverse",
         "list-nested",
         "list-ol",
         "list-stars",
         "list-task",
         "list-ul",
-        "list",
-        "lock-fill",
         "lock",
+        "lock-fill",
+        "lungs",
+        "lungs-fill",
+        "magic",
+        "magnet",
+        "magnet-fill",
         "mailbox",
         "mailbox2",
-        "map-fill",
         "map",
-        "markdown-fill",
+        "map-fill",
         "markdown",
+        "markdown-fill",
         "mask",
-        "megaphone-fill",
+        "mastodon",
+        "medium",
         "megaphone",
-        "menu-app-fill",
+        "megaphone-fill",
+        "memory",
         "menu-app",
+        "menu-app-fill",
+        "menu-button",
         "menu-button-fill",
-        "menu-button-wide-fill",
         "menu-button-wide",
-        "menu-button",
+        "menu-button-wide-fill",
         "menu-down",
         "menu-up",
+        "messenger",
+        "meta",
+        "mic",
         "mic-fill",
-        "mic-mute-fill",
         "mic-mute",
-        "mic",
-        "minecart-loaded",
+        "mic-mute-fill",
+        "microsoft",
+        "microsoft-teams",
         "minecart",
+        "minecart-loaded",
+        "modem",
+        "modem-fill",
         "moisture",
+        "moon",
         "moon-fill",
-        "moon-stars-fill",
         "moon-stars",
-        "moon",
-        "mouse-fill",
+        "moon-stars-fill",
+        "mortarboard",
+        "mortarboard-fill",
+        "motherboard",
+        "motherboard-fill",
         "mouse",
-        "mouse2-fill",
+        "mouse-fill",
         "mouse2",
-        "mouse3-fill",
+        "mouse2-fill",
         "mouse3",
+        "mouse3-fill",
+        "music-note",
         "music-note-beamed",
         "music-note-list",
-        "music-note",
-        "music-player-fill",
         "music-player",
+        "music-player-fill",
         "newspaper",
-        "node-minus-fill",
+        "nintendo-switch",
         "node-minus",
-        "node-plus-fill",
+        "node-minus-fill",
         "node-plus",
-        "nut-fill",
+        "node-plus-fill",
         "nut",
+        "nut-fill",
+        "nvidia",
+        "octagon",
         "octagon-fill",
         "octagon-half",
-        "octagon",
+        "optical-audio",
+        "optical-audio-fill",
         "option",
         "outlet",
+        "p-circle",
+        "p-circle-fill",
+        "p-square",
+        "p-square-fill",
         "paint-bucket",
-        "palette-fill",
         "palette",
+        "palette-fill",
         "palette2",
         "paperclip",
         "paragraph",
-        "patch-check-fill",
+        "pass",
+        "pass-fill",
         "patch-check",
-        "patch-exclamation-fill",
+        "patch-check-fill",
         "patch-exclamation",
-        "patch-minus-fill",
+        "patch-exclamation-fill",
         "patch-minus",
-        "patch-plus-fill",
+        "patch-minus-fill",
         "patch-plus",
-        "patch-question-fill",
+        "patch-plus-fill",
         "patch-question",
-        "pause-btn-fill",
+        "patch-question-fill",
+        "pause",
         "pause-btn",
-        "pause-circle-fill",
+        "pause-btn-fill",
         "pause-circle",
+        "pause-circle-fill",
         "pause-fill",
-        "pause",
-        "peace-fill",
+        "paypal",
+        "pc",
+        "pc-display",
+        "pc-display-horizontal",
+        "pc-horizontal",
+        "pci-card",
         "peace",
-        "pen-fill",
+        "peace-fill",
         "pen",
+        "pen-fill",
+        "pencil",
         "pencil-fill",
         "pencil-square",
-        "pencil",
+        "pentagon",
         "pentagon-fill",
         "pentagon-half",
-        "pentagon",
-        "people-fill",
         "people",
+        "person-circle",
+        "people-fill",
         "percent",
-        "person-badge-fill",
+        "person",
+        "person-add",
         "person-badge",
+        "person-badge-fill",
         "person-bounding-box",
-        "person-check-fill",
         "person-check",
-        "person-circle",
-        "person-dash-fill",
+        "person-check-fill",
         "person-dash",
+        "person-dash-fill",
+        "person-down",
+        "person-exclamation",
         "person-fill",
+        "person-fill-add",
+        "person-fill-check",
+        "person-fill-dash",
+        "person-fill-down",
+        "person-fill-exclamation",
+        "person-fill-gear",
+        "person-fill-lock",
+        "person-fill-slash",
+        "person-fill-up",
+        "person-fill-x",
+        "person-gear",
+        "person-heart",
+        "person-hearts",
         "person-lines-fill",
-        "person-plus-fill",
+        "person-lock",
         "person-plus",
+        "person-plus-fill",
+        "person-rolodex",
+        "person-slash",
         "person-square",
-        "person-x-fill",
+        "person-up",
+        "person-vcard",
+        "person-vcard-fill",
+        "person-video",
+        "person-video2",
+        "person-video3",
+        "person-workspace",
         "person-x",
-        "person",
+        "person-x-fill",
+        "phone",
         "phone-fill",
-        "phone-landscape-fill",
+        "phone-flip",
         "phone-landscape",
-        "phone-vibrate-fill",
+        "phone-landscape-fill",
         "phone-vibrate",
-        "phone",
-        "pie-chart-fill",
+        "phone-vibrate-fill",
         "pie-chart",
-        "pin-angle-fill",
+        "pie-chart-fill",
+        "piggy-bank",
+        "piggy-bank-fill",
+        "pin",
         "pin-angle",
+        "pin-angle-fill",
         "pin-fill",
-        "pin",
-        "pip-fill",
+        "pin-map",
+        "pin-map-fill",
+        "pinterest",
         "pip",
-        "play-btn-fill",
+        "pip-fill",
+        "play",
         "play-btn",
-        "play-circle-fill",
+        "play-btn-fill",
         "play-circle",
+        "play-circle-fill",
         "play-fill",
-        "play",
-        "plug-fill",
+        "playstation",
         "plug",
+        "plug-fill",
+        "plugin",
+        "plus",
+        "plus-circle",
         "plus-circle-dotted",
         "plus-circle-fill",
-        "plus-circle",
+        "plus-lg",
+        "plus-slash-minus",
+        "plus-square",
         "plus-square-dotted",
         "plus-square-fill",
-        "plus-square",
-        "plus",
+        "postage",
+        "postage-fill",
+        "postage-heart",
+        "postage-heart-fill",
+        "postcard",
+        "postcard-fill",
+        "postcard-heart",
+        "postcard-heart-fill",
         "power",
-        "printer-fill",
+        "prescription",
+        "prescription2",
         "printer",
-        "puzzle-fill",
+        "printer-fill",
+        "projector",
+        "projector-fill",
         "puzzle",
-        "question-circle-fill",
+        "puzzle-fill",
+        "qr-code",
+        "qr-code-scan",
+        "question",
         "question-circle",
-        "question-diamond-fill",
         "question-diamond",
-        "question-octagon-fill",
+        "question-diamond-fill",
+        "question-circle-fill",
+        "question-lg",
         "question-octagon",
-        "question-square-fill",
+        "question-octagon-fill",
         "question-square",
-        "question",
+        "question-square-fill",
+        "quora",
+        "quote",
+        "r-circle",
+        "r-circle-fill",
+        "r-square",
+        "r-square-fill",
+        "radioactive",
         "rainbow",
-        "receipt-cutoff",
         "receipt",
+        "receipt-cutoff",
         "reception-0",
         "reception-1",
         "reception-2",
         "reception-3",
         "reception-4",
-        "record-btn-fill",
+        "record",
         "record-btn",
-        "record-circle-fill",
+        "record-btn-fill",
         "record-circle",
+        "record-circle-fill",
         "record-fill",
-        "record",
-        "record2-fill",
         "record2",
-        "reply-all-fill",
+        "record2-fill",
+        "recycle",
+        "reddit",
+        "regex",
+        "repeat",
+        "repeat-1",
+        "reply",
         "reply-all",
+        "reply-all-fill",
         "reply-fill",
-        "reply",
-        "rss-fill",
+        "rewind",
+        "rewind-btn",
+        "rewind-btn-fill",
+        "rewind-circle",
+        "rewind-circle-fill",
+        "rewind-fill",
+        "robot",
+        "rocket",
+        "rocket-fill",
+        "rocket-takeoff",
+        "rocket-takeoff-fill",
+        "router",
+        "router-fill",
         "rss",
+        "rss-fill",
         "rulers",
-        "save-fill",
+        "safe",
+        "safe-fill",
+        "safe2",
+        "safe2-fill",
         "save",
-        "save2-fill",
+        "save-fill",
         "save2",
+        "save2-fill",
         "scissors",
+        "scooter",
         "screwdriver",
+        "sd-card",
+        "sd-card-fill",
         "search",
+        "search-heart",
+        "search-heart-fill",
         "segmented-nav",
+        "send",
+        "send-check",
+        "send-check-fill",
+        "send-dash",
+        "send-dash-fill",
+        "send-exclamation",
+        "send-exclamation-fill",
+        "send-fill",
+        "send-plus",
+        "send-plus-fill",
+        "send-slash",
+        "send-slash-fill",
+        "send-x",
+        "send-x-fill",
         "server",
-        "share-fill",
         "share",
+        "share-fill",
+        "shield",
         "shield-check",
         "shield-exclamation",
+        "shield-fill",
         "shield-fill-check",
         "shield-fill-exclamation",
         "shield-fill-minus",
         "shield-fill-plus",
         "shield-fill-x",
-        "shield-fill",
-        "shield-lock-fill",
         "shield-lock",
+        "shield-lock-fill",
         "shield-minus",
         "shield-plus",
         "shield-shaded",
-        "shield-slash-fill",
         "shield-slash",
+        "shield-slash-fill",
         "shield-x",
-        "shield",
-        "shift-fill",
         "shift",
-        "shop-window",
+        "shift-fill",
         "shop",
+        "shop-window",
         "shuffle",
-        "signpost-2-fill",
+        "sign-dead-end",
+        "sign-dead-end-fill",
+        "sign-do-not-enter",
+        "sign-do-not-enter-fill",
+        "sign-intersection",
+        "sign-intersection-fill",
+        "sign-intersection-side",
+        "sign-intersection-side-fill",
+        "sign-intersection-t",
+        "sign-intersection-t-fill",
+        "sign-intersection-y",
+        "sign-intersection-y-fill",
+        "sign-merge-left",
+        "sign-merge-left-fill",
+        "sign-merge-right",
+        "sign-merge-right-fill",
+        "sign-no-left-turn",
+        "sign-no-left-turn-fill",
+        "sign-no-parking",
+        "sign-no-parking-fill",
+        "sign-no-right-turn",
+        "sign-no-right-turn-fill",
+        "sign-railroad",
+        "sign-railroad-fill",
+        "sign-stop",
+        "sign-stop-fill",
+        "sign-stop-lights",
+        "sign-stop-lights-fill",
+        "sign-turn-left",
+        "sign-turn-left-fill",
+        "sign-turn-right",
+        "sign-turn-right-fill",
+        "sign-turn-slight-left",
+        "sign-turn-slight-left-fill",
+        "sign-turn-slight-right",
+        "sign-turn-slight-right-fill",
+        "sign-yield",
+        "sign-yield-fill",
+        "signal",
+        "signpost",
         "signpost-2",
+        "signpost-2-fill",
         "signpost-fill",
-        "signpost-split-fill",
         "signpost-split",
-        "signpost",
-        "sim-fill",
+        "signpost-split-fill",
         "sim",
-        "skip-backward-btn-fill",
+        "sim-fill",
+        "sina-weibo",
+        "skip-backward",
         "skip-backward-btn",
-        "skip-backward-circle-fill",
+        "skip-backward-btn-fill",
         "skip-backward-circle",
+        "skip-backward-circle-fill",
         "skip-backward-fill",
-        "skip-backward",
-        "skip-end-btn-fill",
+        "skip-end",
         "skip-end-btn",
-        "skip-end-circle-fill",
+        "skip-end-btn-fill",
         "skip-end-circle",
+        "skip-end-circle-fill",
         "skip-end-fill",
-        "skip-end",
-        "skip-forward-btn-fill",
+        "skip-forward",
         "skip-forward-btn",
-        "skip-forward-circle-fill",
+        "skip-forward-btn-fill",
         "skip-forward-circle",
+        "skip-forward-circle-fill",
         "skip-forward-fill",
-        "skip-forward",
-        "skip-start-btn-fill",
+        "skip-start",
         "skip-start-btn",
-        "skip-start-circle-fill",
+        "skip-start-btn-fill",
         "skip-start-circle",
+        "skip-start-circle-fill",
         "skip-start-fill",
-        "skip-start",
+        "skype",
         "slack",
+        "slash",
         "slash-circle-fill",
-        "slash-circle",
-        "slash-square-fill",
+        "slash-lg",
         "slash-square",
-        "slash",
+        "slash-square-fill",
         "sliders",
+        "sliders2",
+        "sliders2-vertical",
         "smartwatch",
+        "snapchat",
         "snow",
         "snow2",
         "snow3",
-        "sort-alpha-down-alt",
         "sort-alpha-down",
-        "sort-alpha-up-alt",
+        "sort-alpha-down-alt",
         "sort-alpha-up",
-        "sort-down-alt",
+        "sort-alpha-up-alt",
         "sort-down",
-        "sort-numeric-down-alt",
+        "sort-down-alt",
         "sort-numeric-down",
-        "sort-numeric-up-alt",
+        "sort-numeric-down-alt",
         "sort-numeric-up",
-        "sort-up-alt",
+        "sort-numeric-up-alt",
         "sort-up",
+        "sort-up-alt",
         "soundwave",
-        "speaker-fill",
         "speaker",
+        "speaker-fill",
         "speedometer",
         "speedometer2",
         "spellcheck",
+        "spotify",
+        "square",
         "square-fill",
         "square-half",
-        "square",
         "stack",
+        "stack-overflow",
+        "star",
         "star-fill",
         "star-half",
-        "star",
         "stars",
-        "stickies-fill",
+        "steam",
         "stickies",
-        "sticky-fill",
+        "stickies-fill",
         "sticky",
-        "stop-btn-fill",
+        "sticky-fill",
+        "stop",
         "stop-btn",
-        "stop-circle-fill",
+        "stop-btn-fill",
         "stop-circle",
+        "stop-circle-fill",
         "stop-fill",
-        "stop",
-        "stoplights-fill",
         "stoplights",
-        "stopwatch-fill",
+        "stoplights-fill",
         "stopwatch",
+        "stopwatch-fill",
+        "strava",
+        "stripe",
+        "subscript",
         "subtract",
-        "suit-club-fill",
         "suit-club",
-        "suit-diamond-fill",
+        "suit-club-fill",
         "suit-diamond",
-        "suit-heart-fill",
+        "suit-diamond-fill",
         "suit-heart",
-        "suit-spade-fill",
+        "suit-heart-fill",
         "suit-spade",
-        "sun-fill",
+        "suit-spade-fill",
         "sun",
+        "sun-fill",
         "sunglasses",
-        "sunrise-fill",
         "sunrise",
-        "sunset-fill",
+        "sunrise-fill",
         "sunset",
+        "sunset-fill",
+        "superscript",
         "symmetry-horizontal",
         "symmetry-vertical",
         "table",
+        "tablet",
         "tablet-fill",
-        "tablet-landscape-fill",
         "tablet-landscape",
-        "tablet",
-        "tag-fill",
+        "tablet-landscape-fill",
         "tag",
-        "tags-fill",
+        "tag-fill",
         "tags",
+        "tags-fill",
+        "taxi-front",
+        "taxi-front-fill",
         "telegram",
+        "telephone",
         "telephone-fill",
-        "telephone-forward-fill",
         "telephone-forward",
-        "telephone-inbound-fill",
+        "telephone-forward-fill",
         "telephone-inbound",
-        "telephone-minus-fill",
+        "telephone-inbound-fill",
         "telephone-minus",
-        "telephone-outbound-fill",
+        "telephone-minus-fill",
         "telephone-outbound",
-        "telephone-plus-fill",
+        "telephone-outbound-fill",
         "telephone-plus",
-        "telephone-x-fill",
+        "telephone-plus-fill",
         "telephone-x",
-        "telephone",
-        "terminal-fill",
+        "telephone-x-fill",
+        "tencent-qq",
         "terminal",
+        "terminal-dash",
+        "terminal-fill",
+        "terminal-plus",
+        "terminal-split",
+        "terminal-x",
         "text-center",
         "text-indent-left",
         "text-indent-right",
         "text-left",
         "text-paragraph",
         "text-right",
+        "text-wrap",
+        "textarea",
         "textarea-resize",
         "textarea-t",
-        "textarea",
+        "thermometer",
         "thermometer-half",
         "thermometer-high",
         "thermometer-low",
         "thermometer-snow",
         "thermometer-sun",
-        "thermometer",
-        "three-dots-vertical",
         "three-dots",
+        "three-dots-vertical",
+        "thunderbolt",
+        "thunderbolt-fill",
+        "ticket",
+        "ticket-detailed",
+        "ticket-detailed-fill",
+        "ticket-fill",
+        "ticket-perforated",
+        "ticket-perforated-fill",
+        "tiktok",
         "toggle-off",
         "toggle-on",
         "toggle2-off",
         "toggle2-on",
         "toggles",
         "toggles2",
         "tools",
         "tornado",
-        "trash-fill",
+        "train-freight-front",
+        "train-freight-front-fill",
+        "train-front",
+        "train-front-fill",
+        "train-lightrail-front",
+        "train-lightrail-front-fill",
+        "translate",
         "trash",
-        "trash2-fill",
+        "trash-fill",
         "trash2",
-        "tree-fill",
+        "trash2-fill",
+        "trash3",
+        "trash3-fill",
         "tree",
+        "tree-fill",
+        "trello",
+        "triangle",
         "triangle-fill",
         "triangle-half",
-        "triangle",
-        "trophy-fill",
         "trophy",
+        "trophy-fill",
         "tropical-storm",
-        "truck-flatbed",
         "truck",
+        "truck-flatbed",
+        "truck-front",
+        "truck-front-fill",
         "tsunami",
-        "tv-fill",
         "tv",
+        "tv-fill",
         "twitch",
         "twitter",
+        "type",
         "type-bold",
         "type-h1",
         "type-h2",
         "type-h3",
         "type-italic",
         "type-strikethrough",
         "type-underline",
-        "type",
-        "ui-checks-grid",
+        "ubuntu",
         "ui-checks",
-        "ui-radios-grid",
+        "ui-checks-grid",
         "ui-radios",
-        "umbrella-fill",
+        "ui-radios-grid",
         "umbrella",
+        "umbrella-fill",
+        "unindent",
         "union",
-        "unlock-fill",
+        "unity",
+        "universal-access",
+        "universal-access-circle",
         "unlock",
-        "upc-scan",
+        "unlock-fill",
         "upc",
+        "upc-scan",
         "upload",
+        "usb",
+        "usb-c",
+        "usb-c-fill",
+        "usb-drive",
+        "usb-drive-fill",
+        "usb-fill",
+        "usb-micro",
+        "usb-micro-fill",
+        "usb-mini",
+        "usb-mini-fill",
+        "usb-plug",
+        "usb-plug-fill",
+        "usb-symbol",
+        "valentine",
+        "valentine2",
         "vector-pen",
         "view-list",
         "view-stacked",
-        "vinyl-fill",
+        "vimeo",
         "vinyl",
+        "vinyl-fill",
+        "virus",
+        "virus2",
         "voicemail",
-        "volume-down-fill",
         "volume-down",
-        "volume-mute-fill",
+        "volume-down-fill",
         "volume-mute",
-        "volume-off-fill",
+        "volume-mute-fill",
         "volume-off",
-        "volume-up-fill",
+        "volume-off-fill",
         "volume-up",
+        "volume-up-fill",
         "vr",
-        "wallet-fill",
         "wallet",
+        "wallet-fill",
         "wallet2",
         "watch",
         "water",
+        "webcam",
+        "webcam-fill",
+        "wechat",
         "whatsapp",
+        "wifi",
         "wifi-1",
         "wifi-2",
         "wifi-off",
-        "wifi",
+        "wikipedia",
         "wind",
-        "window-dock",
-        "window-sidebar",
         "window",
-        "wrench",
-        "x-circle-fill",
-        "x-circle",
-        "x-diamond-fill",
-        "x-diamond",
-        "x-octagon-fill",
-        "x-octagon",
-        "x-square-fill",
-        "x-square",
-        "x",
-        "youtube",
-        "zoom-in",
-        "zoom-out",
-        "bank",
-        "bank2",
-        "bell-slash-fill",
-        "bell-slash",
-        "cash-coin",
-        "check-lg",
-        "coin",
-        "currency-bitcoin",
-        "currency-dollar",
-        "currency-euro",
-        "currency-exchange",
-        "currency-pound",
-        "currency-yen",
-        "dash-lg",
-        "exclamation-lg",
-        "file-earmark-pdf-fill",
-        "file-earmark-pdf",
-        "file-pdf-fill",
-        "file-pdf",
-        "gender-ambiguous",
-        "gender-female",
-        "gender-male",
-        "gender-trans",
-        "headset-vr",
-        "info-lg",
-        "mastodon",
-        "messenger",
-        "piggy-bank-fill",
-        "piggy-bank",
-        "pin-map-fill",
-        "pin-map",
-        "plus-lg",
-        "question-lg",
-        "recycle",
-        "reddit",
-        "safe-fill",
-        "safe2-fill",
-        "safe2",
-        "sd-card-fill",
-        "sd-card",
-        "skype",
-        "slash-lg",
-        "translate",
-        "x-lg",
-        "safe",
-        "apple",
-        "microsoft",
-        "windows",
-        "behance",
-        "dribbble",
-        "line",
-        "medium",
-        "paypal",
-        "pinterest",
-        "signal",
-        "snapchat",
-        "spotify",
-        "stack-overflow",
-        "strava",
-        "wordpress",
-        "vimeo",
-        "activity",
-        "easel2-fill",
-        "easel2",
-        "easel3-fill",
-        "easel3",
-        "fan",
-        "fingerprint",
-        "graph-down-arrow",
-        "graph-up-arrow",
-        "hypnotize",
-        "magic",
-        "person-rolodex",
-        "person-video",
-        "person-video2",
-        "person-video3",
-        "person-workspace",
-        "radioactive",
-        "webcam-fill",
-        "webcam",
-        "yin-yang",
-        "bandaid-fill",
-        "bandaid",
-        "bluetooth",
-        "body-text",
-        "boombox",
-        "boxes",
-        "dpad-fill",
-        "dpad",
-        "ear-fill",
-        "ear",
-        "envelope-check-1",
-        "envelope-check-fill",
-        "envelope-check",
-        "envelope-dash-1",
-        "envelope-dash-fill",
-        "envelope-dash",
-        "envelope-exclamation-1",
-        "envelope-exclamation-fill",
-        "envelope-exclamation",
-        "envelope-plus-fill",
-        "envelope-plus",
-        "envelope-slash-1",
-        "envelope-slash-fill",
-        "envelope-slash",
-        "envelope-x-1",
-        "envelope-x-fill",
-        "envelope-x",
-        "explicit-fill",
-        "explicit",
-        "git",
-        "infinity",
-        "list-columns-reverse",
-        "list-columns",
-        "meta",
-        "mortorboard-fill",
-        "mortorboard",
-        "nintendo-switch",
-        "pc-display-horizontal",
-        "pc-display",
-        "pc-horizontal",
-        "pc",
-        "playstation",
-        "plus-slash-minus",
-        "projector-fill",
-        "projector",
-        "qr-code-scan",
-        "qr-code",
-        "quora",
-        "quote",
-        "robot",
-        "send-check-fill",
-        "send-check",
-        "send-dash-fill",
-        "send-dash",
-        "send-exclamation-1",
-        "send-exclamation-fill",
-        "send-exclamation",
-        "send-fill",
-        "send-plus-fill",
-        "send-plus",
-        "send-slash-fill",
-        "send-slash",
-        "send-x-fill",
-        "send-x",
-        "send",
-        "steam",
-        "terminal-dash-1",
-        "terminal-dash",
-        "terminal-plus",
-        "terminal-split",
-        "ticket-detailed-fill",
-        "ticket-detailed",
-        "ticket-fill",
-        "ticket-perforated-fill",
-        "ticket-perforated",
-        "ticket",
-        "tiktok",
         "window-dash",
         "window-desktop",
+        "window-dock",
         "window-fullscreen",
         "window-plus",
+        "window-sidebar",
         "window-split",
         "window-stack",
         "window-x",
-        "xbox",
-        "ethernet",
-        "hdmi-fill",
-        "hdmi",
-        "usb-c-fill",
-        "usb-c",
-        "usb-fill",
-        "usb-plug-fill",
-        "usb-plug",
-        "usb-symbol",
-        "usb",
-        "boombox-fill",
-        "displayport-1",
-        "displayport",
-        "gpu-card",
-        "memory",
-        "modem-fill",
-        "modem",
-        "motherboard-fill",
-        "motherboard",
-        "optical-audio-fill",
-        "optical-audio",
-        "pci-card",
-        "router-fill",
-        "router",
-        "ssd-fill",
-        "ssd",
-        "thunderbolt-fill",
-        "thunderbolt",
-        "usb-drive-fill",
-        "usb-drive",
-        "usb-micro-fill",
-        "usb-micro",
-        "usb-mini-fill",
-        "usb-mini",
-        "cloud-haze2",
-        "device-hdd-fill",
-        "device-hdd",
-        "device-ssd-fill",
-        "device-ssd",
-        "displayport-fill",
-        "mortarboard-fill",
-        "mortarboard",
-        "terminal-x",
-        "arrow-through-heart-fill",
-        "arrow-through-heart",
-        "badge-sd-fill",
-        "badge-sd",
-        "bag-heart-fill",
-        "bag-heart",
-        "balloon-fill",
-        "balloon-heart-fill",
-        "balloon-heart",
-        "balloon",
-        "box2-fill",
-        "box2-heart-fill",
-        "box2-heart",
-        "box2",
-        "braces-asterisk",
-        "calendar-heart-fill",
-        "calendar-heart",
-        "calendar2-heart-fill",
-        "calendar2-heart",
-        "chat-heart-fill",
-        "chat-heart",
-        "chat-left-heart-fill",
-        "chat-left-heart",
-        "chat-right-heart-fill",
-        "chat-right-heart",
-        "chat-square-heart-fill",
-        "chat-square-heart",
-        "clipboard-check-fill",
-        "clipboard-data-fill",
-        "clipboard-fill",
-        "clipboard-heart-fill",
-        "clipboard-heart",
-        "clipboard-minus-fill",
-        "clipboard-plus-fill",
-        "clipboard-pulse",
-        "clipboard-x-fill",
-        "clipboard2-check-fill",
-        "clipboard2-check",
-        "clipboard2-data-fill",
-        "clipboard2-data",
-        "clipboard2-fill",
-        "clipboard2-heart-fill",
-        "clipboard2-heart",
-        "clipboard2-minus-fill",
-        "clipboard2-minus",
-        "clipboard2-plus-fill",
-        "clipboard2-plus",
-        "clipboard2-pulse-fill",
-        "clipboard2-pulse",
-        "clipboard2-x-fill",
-        "clipboard2-x",
-        "clipboard2",
-        "emoji-kiss-fill",
-        "emoji-kiss",
-        "envelope-heart-fill",
-        "envelope-heart",
-        "envelope-open-heart-fill",
-        "envelope-open-heart",
-        "envelope-paper-fill",
-        "envelope-paper-heart-fill",
-        "envelope-paper-heart",
-        "envelope-paper",
-        "filetype-aac",
-        "filetype-ai",
-        "filetype-bmp",
-        "filetype-cs",
-        "filetype-css",
-        "filetype-csv",
-        "filetype-doc",
-        "filetype-docx",
-        "filetype-exe",
-        "filetype-gif",
-        "filetype-heic",
-        "filetype-html",
-        "filetype-java",
-        "filetype-jpg",
-        "filetype-js",
-        "filetype-jsx",
-        "filetype-key",
-        "filetype-m4p",
-        "filetype-md",
-        "filetype-mdx",
-        "filetype-mov",
-        "filetype-mp3",
-        "filetype-mp4",
-        "filetype-otf",
-        "filetype-pdf",
-        "filetype-php",
-        "filetype-png",
-        "filetype-ppt-1",
-        "filetype-ppt",
-        "filetype-psd",
-        "filetype-py",
-        "filetype-raw",
-        "filetype-rb",
-        "filetype-sass",
-        "filetype-scss",
-        "filetype-sh",
-        "filetype-svg",
-        "filetype-tiff",
-        "filetype-tsx",
-        "filetype-ttf",
-        "filetype-txt",
-        "filetype-wav",
-        "filetype-woff",
-        "filetype-xls-1",
-        "filetype-xls",
-        "filetype-xml",
-        "filetype-yml",
-        "heart-arrow",
-        "heart-pulse-fill",
-        "heart-pulse",
-        "heartbreak-fill",
-        "heartbreak",
-        "hearts",
-        "hospital-fill",
-        "hospital",
-        "house-heart-fill",
-        "house-heart",
-        "incognito",
-        "magnet-fill",
-        "magnet",
-        "person-heart",
-        "person-hearts",
-        "phone-flip",
-        "plugin",
-        "postage-fill",
-        "postage-heart-fill",
-        "postage-heart",
-        "postage",
-        "postcard-fill",
-        "postcard-heart-fill",
-        "postcard-heart",
-        "postcard",
-        "search-heart-fill",
-        "search-heart",
-        "sliders2-vertical",
-        "sliders2",
-        "trash3-fill",
-        "trash3",
-        "valentine",
-        "valentine2",
-        "wrench-adjustable-circle-fill",
-        "wrench-adjustable-circle",
+        "windows",
+        "wordpress",
+        "wrench",
         "wrench-adjustable",
-        "filetype-json",
-        "filetype-pptx",
-        "filetype-xlsx"
+        "wrench-adjustable-circle",
+        "wrench-adjustable-circle-fill",
+        "x",
+        "x-circle",
+        "x-circle-fill",
+        "x-diamond",
+        "x-diamond-fill",
+        "x-lg",
+        "x-octagon",
+        "x-octagon-fill",
+        "x-square",
+        "x-square-fill",
+        "xbox",
+        "yelp",
+        "yin-yang",
+        "youtube",
+        "zoom-in",
+        "zoom-out"
     ],
     "list-icon": "bi bi-badge1",
-    "prefix": "bi bi-"
+    "prefix": "bi bi-",
+    "version": "1.10.3"
 }
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,7 +1,9 @@
+/* eslint-disable no-console */
+/*jshint esversion: 8 */
 var iconPickerUrl = document.currentScript.src.replace(/js\/([a-z\.-]+)$/gm, '');
 var loadedDependencies = [];
 
 (function(root, factory) {
     if (typeof define === 'function' && define.amd) {
         define([], factory('UniversalIconPicker'));
     } else if (typeof exports === 'object') {
@@ -12,15 +14,15 @@
 }(this, function() {
     'use strict';
 
     var createDomEle = function(string) {
         var ele = document.createElement('div');
         ele.innerHTML = string;
         return ele.firstChild;
-    }
+    };
 
     var debounce = function(func, wait, immediate) {
         var timeout;
         return function() {
             var context = this,
                 args = arguments;
             var later = function() {
@@ -36,15 +38,15 @@
 
     var escapeHtml = function(text) {
         var map = {
             '&': '&amp;',
             '<': '&lt;',
             '>': '&gt;',
             '"': '&quot;',
-            "'": '&#039;'
+            '\'': '&#039;',
         };
 
         return text.replace(/[&<>"']/g, function(m) {
             return map[m];
         });
     };
 
@@ -67,50 +69,50 @@
         }
 
         return extended;
     };
 
     var getLibraryName = function(string) {
         return string.replace(/([A-Z])/g, ' $1');
-    }
+    };
 
     /**
      * Plugin Object
      * @param selector The html selector to initialize
      * @param {Object} options User options
      * @constructor
      */
     function UniversalIconPicker(selector, options) {
         this.selector = selector;
 
-        let defaults = {
+        const defaults = {
             allowEmpty: true,
             iconLibraries: null,
             iconLibrariesCss: null,
             mode: 'autoload', // autoload | onrequest
             onBeforeOpen: null,
             onReset: null,
             onSelect: null,
             resetSelector: null,
-            loadCustomCss: false
+            loadCustomCss: false,
         };
         this.options = extend(defaults, options);
 
         this.activeLibraryId = '';
         this.filterIcon = '';
         this.iconEventsLoaded = false;
         this.iconLibraries = {};
         this.iconLibrariesLoaded = false;
         this.iconMarkup = '';
         this.iconWrap = '';
         this.idSuffix = '-' + this.selector.replace(/[#\s[\]="]/g, '');
         this.sideBarBtn = '';
         this.sideBarList = [];
 
-        this.universalWrap = '<div class="uip-modal uip-open" id="uip-modal' + this.idSuffix + '"><div class="uip-modal--content"><div class="uip-modal--header"><div class="uip-modal--header-logo-area"><span class="uip-modal--header-logo-title">Universal Icon Picker</span></div><div class="uip-modal--header-close-btn"><img src="' + iconPickerUrl + '/images/xmark-solid.svg" width="20" height="16" alt="Close" title="Close" /></div></div><div class="uip-modal--body"><div id="uip-modal--sidebar' + this.idSuffix + '" class="uip-modal--sidebar"><div class="uip-modal--sidebar-tabs"></div></div><div id="uip-modal--icon-preview-wrap' + this.idSuffix + '" class="uip-modal--icon-preview-wrap"><div class="uip-modal--icon-search"><input name="" value="" placeholder="Filter by name..."><img src="' + iconPickerUrl + '/images/magnifying-glass-solid.svg" width="20" height="16" alt="Search" title="Search" /></div><div class="uip-modal--icon-preview-inner"><div id="uip-modal--icon-preview' + this.idSuffix + '" class="uip-modal--icon-preview"></div></div></div></div><div class="uip-modal--footer"><button class="uip-insert-icon-button">Insert</button></div></div></div>';
+        this.universalWrap = '<div class="uip-modal uip-open" id="uip-modal' + this.idSuffix + '"><div class="uip-modal--content"><div class="uip-modal--header"><div class="uip-modal--header-logo-area"><span class="uip-modal--header-logo-title">Universal Icon Picker</span></div><div class="uip-modal--header-close-btn"><img src="' + (options.closeUrl || iconPickerUrl + '/images/xmark-solid.svg') + '" width="20" height="16" alt="Close" title="Close" /></div></div><div class="uip-modal--body"><div id="uip-modal--sidebar' + this.idSuffix + '" class="uip-modal--sidebar"><div class="uip-modal--sidebar-tabs"></div></div><div id="uip-modal--icon-preview-wrap' + this.idSuffix + '" class="uip-modal--icon-preview-wrap"><div class="uip-modal--icon-search"><input name="" value="" placeholder="Filter by name..."><img src="' + (options.searchUrl || iconPickerUrl + '/images/magnifying-glass-solid.svg') + '" width="20" height="16" alt="Search" title="Search" /></div><div class="uip-modal--icon-preview-inner"><div id="uip-modal--icon-preview' + this.idSuffix + '" class="uip-modal--icon-preview"></div></div></div></div><div class="uip-modal--footer"><button class="uip-insert-icon-button">Insert</button></div></div></div>';
 
         this.universalDomEle = createDomEle(this.universalWrap);
         this.sidebarTabs = this.universalDomEle.querySelector('.uip-modal--sidebar-tabs');
         this.previewWrap = this.universalDomEle.querySelector('#uip-modal--icon-preview' + this.idSuffix);
         this.searchInput = this.universalDomEle.querySelector('.uip-modal--icon-search input');
         if (this.options.mode === 'autoload') {
             this.init();
@@ -168,15 +170,15 @@
                             let iconHtml = selected.querySelector('i').outerHTML;
                             let jsonOutput = {
                                 'libraryId': selected.dataset.libraryId,
                                 'libraryName': selected.dataset.libraryName,
                                 'iconHtml': null,
                                 'iconMarkup': null,
                                 'iconClass': null,
-                                'iconText': null
+                                'iconText': null,
                             };
                             if (!selected.querySelector('i').classList.value.match('uip-icon-none')) {
                                 jsonOutput.iconHtml = iconHtml;
                                 jsonOutput.iconMarkup = escapeHtml(iconHtml);
                                 jsonOutput.iconClass = selected.querySelector('i').classList.value;
                                 jsonOutput.iconText = selected.querySelector('i').innerText;
                             }
@@ -229,33 +231,33 @@
         -------------------------------------------------- */
 
         _clickHandlerFunc: function(e) {
             if (!e.currentTarget.classList.contains('universal-active')) {
                 this.sideBarBtn.forEach(function(item) {
                     item.classList.remove('universal-active');
                 });
-                e.currentTarget.classList.add('universal-active')
+                e.currentTarget.classList.add('universal-active');
             }
             this._sidebarFilterFunc(e.currentTarget.dataset['libraryId']);
         },
 
         _iconItemMarkup: function(libraryName, libraryItem) {
-            var markup = '',
+            let markup = '',
                 library = libraryItem['icon-style'],
                 prefix = libraryItem['prefix'];
             if (this.options.allowEmpty) {
                 markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + prefix + ' uip-icon-none">&nbsp;</i><div class="uip-icon-item-name" title="None">None</div></div></div>';
             }
             if (prefix.match(/^material-icons/)) {
                 libraryItem['icons'].forEach(function(item) {
-                    markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="' + item + '" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + prefix + '">' + item + '</i><div class="uip-icon-item-name" title="' + item + '">' + item.replace("-", " ") + '</div></div></div>';
+                    markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="' + item + '" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + prefix + '">' + item + '</i><div class="uip-icon-item-name" title="' + item + '">' + item.replace('-', ' ') + '</div></div></div>';
                 });
             } else {
                 libraryItem['icons'].forEach(function(item) {
-                    markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="' + item + '" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + [prefix, item].join('') + '"></i><div class="uip-icon-item-name" title="' + item + '">' + item.replace("-", " ") + '</div></div></div>';
+                    markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="' + item + '" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + [prefix, item].join('') + '"></i><div class="uip-icon-item-name" title="' + item + '">' + item.replace('-', ' ') + '</div></div></div>';
                 });
             }
 
             return markup;
         },
 
         _iconItemPush: function(arrayList) {
@@ -263,28 +265,30 @@
             arrayList.forEach((item) => {
                 this.previewWrap.appendChild(item[1]);
             });
         },
 
         _loadCssFiles: function() {
             let link = document.createElement('link');
-            if (!loadedDependencies.includes('universal-icon-picker.min.css') & !this.options.loadCustomCss) {
+            if (!loadedDependencies.includes('universal-icon-picker.min.css') && !this.options.loadCustomCss) {
                 link.rel = 'stylesheet';
                 link.type = 'text/css';
                 link.href = iconPickerUrl + 'stylesheets/universal-icon-picker.min.css';
                 link.media = 'screen';
                 document.head.appendChild(link);
                 loadedDependencies.push('universal-icon-picker.min.css');
             }
             if (this.options.iconLibrariesCss) {
                 this.options.iconLibrariesCss.forEach(cssFile => {
                     if (!loadedDependencies.includes(cssFile)) {
-                        let cssFileLink = iconPickerUrl + 'stylesheets/' + cssFile;
-                        if (cssFile.match(/^http|^\/\//)) {
+                        let cssFileLink;
+                        if (cssFile.includes('/')) {
                             cssFileLink = cssFile;
+                        } else {
+                            cssFileLink = iconPickerUrl + 'stylesheets/' + cssFile;
                         }
                         link = document.createElement('link');
                         link.rel = 'stylesheet';
                         link.type = 'text/css';
                         link.href = cssFileLink;
                         link.media = 'screen';
                         document.head.appendChild(link);
@@ -300,24 +304,32 @@
                 return false;
             }
             if (this.iconLibrariesLoaded) {
                 return true;
             }
             if (i === 0 && this.options.iconLibraries.length > 1) {
                 this.sideBarList.push({
-                    "title": "all icons",
-                    "list-icon": "",
-                    "library-id": "all",
-                    "prefix": ""
+                    'title': 'all icons',
+                    'list-icon': '',
+                    'library-id': 'all',
+                    'prefix': '',
                 });
             }
 
-            let iconLib = this.options.iconLibraries[i];
+            let iconLibUrl = this.options.iconLibraries[i];
+            let iconLib;
+            if (iconLibUrl.includes('/')) {
+                iconLib = /[^/]*$/.exec(iconLibUrl)[0];
+                iconLib = /^[^.]*/.exec(iconLib)[0];
+            } else {
+                iconLibUrl = iconPickerUrl + 'icons-libraries/' + iconLibUrl;
+                iconLib = iconLibUrl;
+            }
 
-            await fetch(iconPickerUrl + 'icons-libraries/' + iconLib)
+            await fetch(iconLibUrl)
                 .then(response => response.json())
                 .then(data => {
                     // Success!
                     var camelCasedIconLibrary = iconLib.replace(/-([a-z])/g, function(g) {
                         return g[1].toUpperCase();
                     }).replace(/\.[a-z.]+$/, '');
                     let newLibrary = {};
@@ -381,37 +393,37 @@
             var searchText = e.target.value.toLowerCase();
             this._searchFilterFunc(searchText, 'filter');
 
         },
 
         _searchFilterFunc: function(filterText, dataName) {
             this.filterIcon = Object.entries(this.iconWrap).filter((item) => {
-                if (-1 == item[1].dataset[dataName].indexOf(filterText) || (this.activeLibraryId !== 'all' && item[1].dataset['libraryId'] !== this.activeLibraryId)) {
+                if (-1 === item[1].dataset[dataName].indexOf(filterText) || (this.activeLibraryId !== 'all' && item[1].dataset['libraryId'] !== this.activeLibraryId)) {
                     return false;
                 }
                 return true;
             });
 
             this._iconItemPush(this.filterIcon);
 
         },
 
         _setIconAndSidebarList: function() {
             for (const [libraryName, libraryContent] of Object.entries(this.iconLibraries)) {
-                this._setSideBarList(getLibraryName(libraryName), libraryContent);
+                this._setSideBarList(libraryContent.verboseName || getLibraryName(libraryName), libraryContent);
                 this._setIconMarkup(libraryName, libraryContent);
             }
         },
 
         _setIconMarkup: function(libraryName, libraryContent) {
             if (libraryContent.icons !== undefined) {
-                this.iconMarkup += this._iconItemMarkup(libraryName, libraryContent)
+                this.iconMarkup += this._iconItemMarkup(libraryName, libraryContent);
             } else {
                 Object.entries(libraryContent).forEach((item) => {
-                    this.iconMarkup += this._iconItemMarkup(libraryName, item[1])
+                    this.iconMarkup += this._iconItemMarkup(libraryName, item[1]);
                 });
             }
         },
 
         _sidebarFilterFunc: function(filterText) {
             this.activeLibraryId = filterText;
             this.filterIcon = Object.entries(this.iconWrap).filter(function(item) {
@@ -434,20 +446,20 @@
                     'list-icon': libraryContent['list-icon'] !== undefined ? libraryContent['list-icon'] : '',
                     'library-id': libraryContent['icon-style'] !== undefined ? libraryContent['icon-style'] : 'all',
                 };
                 this.sideBarList.push(listItem);
             } else {
                 Object.entries(libraryContent).forEach(item => {
                     listItem = {
-                        "title": libraryName + ' - ' + item[0],
-                        "prefix": item[1]['prefix'] !== undefined ? item[1]['prefix'] : '',
-                        "list-icon": item[1]['list-icon'] !== undefined ? item[1]['list-icon'] : "",
-                        "library-id": item[1]['icon-style'] !== undefined ? item[1]['icon-style'] : "all",
+                        'title': libraryName + ' - ' + item[0],
+                        'prefix': item[1]['prefix'] !== undefined ? item[1]['prefix'] : '',
+                        'list-icon': item[1]['list-icon'] !== undefined ? item[1]['list-icon'] : '',
+                        'library-id': item[1]['icon-style'] !== undefined ? item[1]['icon-style'] : 'all',
                     };
-                    this.sideBarList.push(listItem)
+                    this.sideBarList.push(listItem);
                 });
             }
         },
 
         _sideBarListMarkup: function(sideBarList) {
             var markup = '';
             sideBarList.forEach((item) => {
@@ -458,17 +470,17 @@
                 if ('all' !== item['library-id']) {
                     let iconTag = '<i class="' + item['list-icon'] + '"></i>';
                     if (item['prefix'].match(/^material-icons/)) {
                         iconTag = '<i class="' + item['prefix'] + '">' + item['list-icon'] + '</i>';
                     }
                     markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item['library-id'] + '">' + iconTag + item['title'] + '</div>';
                 } else {
-                    markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item['library-id'] + '"><img src="' + iconPickerUrl + '/images/star-of-life-solid.svg" width="13.125px" height="auto" alt="All" title="All" />' + item['title'] + '</div>';
+                    markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item['library-id'] + '"><img src="' + (this.options.starUrl || iconPickerUrl + '/images/star-of-life-solid.svg') + '" width="13.125px" height="auto" alt="All" title="All" />' + item['title'] + '</div>';
                 }
             });
 
             return markup;
-        }
+        },
     };
 
     return UniversalIconPicker;
 }));
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -58,15 +58,15 @@
     };
     var getLibraryName = function(string) {
         return string.replace(/([A-Z])/g, " $1")
     };
 
     function UniversalIconPicker(selector, options) {
         this.selector = selector;
-        let defaults = {
+        const defaults = {
             allowEmpty: true,
             iconLibraries: null,
             iconLibrariesCss: null,
             mode: "autoload",
             onBeforeOpen: null,
             onReset: null,
             onSelect: null,
@@ -80,15 +80,15 @@
         this.iconLibraries = {};
         this.iconLibrariesLoaded = false;
         this.iconMarkup = "";
         this.iconWrap = "";
         this.idSuffix = "-" + this.selector.replace(/[#\s[\]="]/g, "");
         this.sideBarBtn = "";
         this.sideBarList = [];
-        this.universalWrap = '<div class="uip-modal uip-open" id="uip-modal' + this.idSuffix + '"><div class="uip-modal--content"><div class="uip-modal--header"><div class="uip-modal--header-logo-area"><span class="uip-modal--header-logo-title">Universal Icon Picker</span></div><div class="uip-modal--header-close-btn"><img src="' + iconPickerUrl + '/images/xmark-solid.svg" width="20" height="16" alt="Close" title="Close" /></div></div><div class="uip-modal--body"><div id="uip-modal--sidebar' + this.idSuffix + '" class="uip-modal--sidebar"><div class="uip-modal--sidebar-tabs"></div></div><div id="uip-modal--icon-preview-wrap' + this.idSuffix + '" class="uip-modal--icon-preview-wrap"><div class="uip-modal--icon-search"><input name="" value="" placeholder="Filter by name..."><img src="' + iconPickerUrl + '/images/magnifying-glass-solid.svg" width="20" height="16" alt="Search" title="Search" /></div><div class="uip-modal--icon-preview-inner"><div id="uip-modal--icon-preview' + this.idSuffix + '" class="uip-modal--icon-preview"></div></div></div></div><div class="uip-modal--footer"><button class="uip-insert-icon-button">Insert</button></div></div></div>';
+        this.universalWrap = '<div class="uip-modal uip-open" id="uip-modal' + this.idSuffix + '"><div class="uip-modal--content"><div class="uip-modal--header"><div class="uip-modal--header-logo-area"><span class="uip-modal--header-logo-title">Universal Icon Picker</span></div><div class="uip-modal--header-close-btn"><img src="' + (options.closeUrl || iconPickerUrl + "/images/xmark-solid.svg") + '" width="20" height="16" alt="Close" title="Close" /></div></div><div class="uip-modal--body"><div id="uip-modal--sidebar' + this.idSuffix + '" class="uip-modal--sidebar"><div class="uip-modal--sidebar-tabs"></div></div><div id="uip-modal--icon-preview-wrap' + this.idSuffix + '" class="uip-modal--icon-preview-wrap"><div class="uip-modal--icon-search"><input name="" value="" placeholder="Filter by name..."><img src="' + (options.searchUrl || iconPickerUrl + "/images/magnifying-glass-solid.svg") + '" width="20" height="16" alt="Search" title="Search" /></div><div class="uip-modal--icon-preview-inner"><div id="uip-modal--icon-preview' + this.idSuffix + '" class="uip-modal--icon-preview"></div></div></div></div><div class="uip-modal--footer"><button class="uip-insert-icon-button">Insert</button></div></div></div>';
         this.universalDomEle = createDomEle(this.universalWrap);
         this.sidebarTabs = this.universalDomEle.querySelector(".uip-modal--sidebar-tabs");
         this.previewWrap = this.universalDomEle.querySelector("#uip-modal--icon-preview" + this.idSuffix);
         this.searchInput = this.universalDomEle.querySelector(".uip-modal--icon-search input");
         if (this.options.mode === "autoload") {
             this.init()
         } else {
@@ -184,15 +184,15 @@
                     item.classList.remove("universal-active")
                 });
                 e.currentTarget.classList.add("universal-active")
             }
             this._sidebarFilterFunc(e.currentTarget.dataset["libraryId"])
         },
         _iconItemMarkup: function(libraryName, libraryItem) {
-            var markup = "",
+            let markup = "",
                 library = libraryItem["icon-style"],
                 prefix = libraryItem["prefix"];
             if (this.options.allowEmpty) {
                 markup += '<div class="uip-icon-item" data-library-id="' + library + '" data-filter="" data-library-name="' + libraryName + '"><div class="uip-icon-item-inner"><i class="' + prefix + ' uip-icon-none">&nbsp;</i><div class="uip-icon-item-name" title="None">None</div></div></div>'
             }
             if (prefix.match(/^material-icons/)) {
                 libraryItem["icons"].forEach(function(item) {
@@ -209,28 +209,30 @@
             this.previewWrap.innerHTML = "";
             arrayList.forEach(item => {
                 this.previewWrap.appendChild(item[1])
             })
         },
         _loadCssFiles: function() {
             let link = document.createElement("link");
-            if (!loadedDependencies.includes("universal-icon-picker.min.css") & !this.options.loadCustomCss) {
+            if (!loadedDependencies.includes("universal-icon-picker.min.css") && !this.options.loadCustomCss) {
                 link.rel = "stylesheet";
                 link.type = "text/css";
                 link.href = iconPickerUrl + "stylesheets/universal-icon-picker.min.css";
                 link.media = "screen";
                 document.head.appendChild(link);
                 loadedDependencies.push("universal-icon-picker.min.css")
             }
             if (this.options.iconLibrariesCss) {
                 this.options.iconLibrariesCss.forEach(cssFile => {
                     if (!loadedDependencies.includes(cssFile)) {
-                        let cssFileLink = iconPickerUrl + "stylesheets/" + cssFile;
-                        if (cssFile.match(/^http|^\/\//)) {
+                        let cssFileLink;
+                        if (cssFile.includes("/")) {
                             cssFileLink = cssFile
+                        } else {
+                            cssFileLink = iconPickerUrl + "stylesheets/" + cssFile
                         }
                         link = document.createElement("link");
                         link.rel = "stylesheet";
                         link.type = "text/css";
                         link.href = cssFileLink;
                         link.media = "screen";
                         document.head.appendChild(link);
@@ -251,16 +253,24 @@
                 this.sideBarList.push({
                     title: "all icons",
                     "list-icon": "",
                     "library-id": "all",
                     prefix: ""
                 })
             }
-            let iconLib = this.options.iconLibraries[i];
-            await fetch(iconPickerUrl + "icons-libraries/" + iconLib).then(response => response.json()).then(data => {
+            let iconLibUrl = this.options.iconLibraries[i];
+            let iconLib;
+            if (iconLibUrl.includes("/")) {
+                iconLib = /[^/]*$/.exec(iconLibUrl)[0];
+                iconLib = /^[^.]*/.exec(iconLib)[0]
+            } else {
+                iconLibUrl = iconPickerUrl + "icons-libraries/" + iconLibUrl;
+                iconLib = iconLibUrl
+            }
+            await fetch(iconLibUrl).then(response => response.json()).then(data => {
                 var camelCasedIconLibrary = iconLib.replace(/-([a-z])/g, function(g) {
                     return g[1].toUpperCase()
                 }).replace(/\.[a-z.]+$/, "");
                 let newLibrary = {};
                 newLibrary[camelCasedIconLibrary] = data;
                 Object.assign(this.iconLibraries, newLibrary);
                 if (i + 1 === this.options.iconLibraries.length) {
@@ -299,24 +309,24 @@
         },
         _searchFunc: function(e) {
             var searchText = e.target.value.toLowerCase();
             this._searchFilterFunc(searchText, "filter")
         },
         _searchFilterFunc: function(filterText, dataName) {
             this.filterIcon = Object.entries(this.iconWrap).filter(item => {
-                if (-1 == item[1].dataset[dataName].indexOf(filterText) || this.activeLibraryId !== "all" && item[1].dataset["libraryId"] !== this.activeLibraryId) {
+                if (-1 === item[1].dataset[dataName].indexOf(filterText) || this.activeLibraryId !== "all" && item[1].dataset["libraryId"] !== this.activeLibraryId) {
                     return false
                 }
                 return true
             });
             this._iconItemPush(this.filterIcon)
         },
         _setIconAndSidebarList: function() {
             for (const [libraryName, libraryContent] of Object.entries(this.iconLibraries)) {
-                this._setSideBarList(getLibraryName(libraryName), libraryContent);
+                this._setSideBarList(libraryContent.verboseName || getLibraryName(libraryName), libraryContent);
                 this._setIconMarkup(libraryName, libraryContent)
             }
         },
         _setIconMarkup: function(libraryName, libraryContent) {
             if (libraryContent.icons !== undefined) {
                 this.iconMarkup += this._iconItemMarkup(libraryName, libraryContent)
             } else {
@@ -367,15 +377,15 @@
                 if ("all" !== item["library-id"]) {
                     let iconTag = '<i class="' + item["list-icon"] + '"></i>';
                     if (item["prefix"].match(/^material-icons/)) {
                         iconTag = '<i class="' + item["prefix"] + '">' + item["list-icon"] + "</i>"
                     }
                     markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item["library-id"] + '">' + iconTag + item["title"] + "</div>"
                 } else {
-                    markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item["library-id"] + '"><img src="' + iconPickerUrl + '/images/star-of-life-solid.svg" width="13.125px" height="auto" alt="All" title="All" />' + item["title"] + "</div>"
+                    markup += '<div class="uip-modal--sidebar-tab-item' + activeClazz + '" data-library-id="' + item["library-id"] + '"><img src="' + (this.options.starUrl || iconPickerUrl + "/images/star-of-life-solid.svg") + '" width="13.125px" height="auto" alt="All" title="All" />' + item["title"] + "</div>"
                 }
             });
             return markup
         }
     };
     return UniversalIconPicker
 });
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% load i18n %}<div{% if widget.attrs.id %} id="{{ widget.attrs.id|safe }}"{% endif %} class="frontend-icon-picker{% if widget.attrs.class %} {{ widget.attrs.class }}{% endif %}">
+{% load i18n static %}<div{% if widget.attrs.id %} id="{{ widget.attrs.id|safe }}"{% endif %} class="frontend-icon-picker{% if widget.attrs.class %} {{ widget.attrs.class }}{% endif %}">
     <div class="icon-container">
         <div id="{{ widget.attrs.id|safe }}-preview" class="icon-preview">
             <div class="icon-box">{{ widget.preview|safe }}</div>
             <div class="empty-box{% if widget.preview %} hidden{% endif %}">{% translate "Click to add icon" %}</div>
         </div>
         {% if not widget.required %}<div class="icon-close-indicator"></div>{% endif %}
     </div>
@@ -38,14 +38,17 @@
                 resetSelector: '#{{ widget.attrs.id|safe }} .icon-close-indicator',
             {% endif %}
             onSelect: setIcon,
             onReset: setIcon,
             iconLibraries: [selectElement.find(':selected').data('json')],
             iconLibrariesCss: [selectElement.find(':selected').data('css')],
             loadCustomCss: true,
+            searchUrl: '{% static "djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg" %}',
+            starUrl: '{% static "djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg" %}',
+            closeUrl: '{% static "djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg" %}',
             allowEmpty: false
         };
         var uip = new UniversalIconPicker(options.selector, options);
         selectElement.on('change', function () {
             uip.setOptions({
                iconLibraries: [this.options[this.selectedIndex].dataset.json],
                iconLibrariesCss: [this.options[this.selectedIndex].dataset.css]
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/apps.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/constants.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/helpers.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/link/views.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/listgroup/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/media/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/constants.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/forms.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms-frontend-1.1.2/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/fields.py` & `djangocms-frontend-1.1.2/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.2/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/helpers.py` & `djangocms-frontend-1.1.2/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.2/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/frontend.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/icon_migration.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/management/styled_link_migration.py` & `djangocms-frontend-1.1.2/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/migrations/0001_initial.py` & `djangocms-frontend-1.1.2/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/models.py` & `djangocms-frontend-1.1.2/djangocms_frontend/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/settings.py` & `djangocms-frontend-1.1.2/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/base.css` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css`

 * *Files 0% similar despite different names*

```diff
@@ -5623,219 +5623,224 @@
 00015f60: 6974 6961 6c7d 2e75 6970 2d6d 6f64 616c  itial}.uip-modal
 00015f70: 202e 7569 702d 6d6f 6461 6c2d 2d66 6f6f   .uip-modal--foo
 00015f80: 7465 7220 2e75 6e69 7665 7273 616c 2d62  ter .universal-b
 00015f90: 7574 746f 6e2d 7375 6363 6573 733a 686f  utton-success:ho
 00015fa0: 7665 727b 6261 636b 6772 6f75 6e64 2d63  ver{background-c
 00015fb0: 6f6c 6f72 3a23 3062 667d 406d 6564 6961  olor:#0bf}@media
 00015fc0: 2028 6d69 6e2d 7769 6474 683a 3134 3430   (min-width:1440
-00015fd0: 7078 297b 2e75 6970 2d6d 6f64 616c 202e  px){.uip-modal .
-00015fe0: 7569 702d 6d6f 6461 6c2d 2d63 6f6e 7465  uip-modal--conte
-00015ff0: 6e74 7b6d 6178 2d77 6964 7468 3a31 3230  nt{max-width:120
-00016000: 3070 787d 7d40 6d65 6469 6120 286d 6178  0px}}@media (max
-00016010: 2d77 6964 7468 3a31 3433 3970 7829 7b2e  -width:1439px){.
-00016020: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
-00016030: 6f64 616c 2d2d 636f 6e74 656e 747b 6d61  odal--content{ma
-00016040: 782d 7769 6474 683a 3939 3070 787d 2e75  x-width:990px}.u
-00016050: 6970 2d6d 6f64 616c 2d2d 6963 6f6e 2d70  ip-modal--icon-p
-00016060: 7265 7669 6577 2d77 7261 707b 7061 6464  review-wrap{padd
-00016070: 696e 673a 3330 7078 2035 3070 7820 307d  ing:30px 50px 0}
-00016080: 7d40 6d65 6469 6120 286d 6178 2d77 6964  }@media (max-wid
-00016090: 7468 3a31 3032 3370 7829 7b2e 7569 702d  th:1023px){.uip-
-000160a0: 6d6f 6461 6c20 2e75 6970 2d6d 6f64 616c  modal .uip-modal
-000160b0: 2d2d 636f 6e74 656e 747b 6d61 782d 7769  --content{max-wi
-000160c0: 6474 683a 3734 3070 787d 7d40 6d65 6469  dth:740px}}@medi
-000160d0: 6120 286d 6178 2d77 6964 7468 3a37 3637  a (max-width:767
-000160e0: 7078 297b 2e75 6970 2d6d 6f64 616c 2d2d  px){.uip-modal--
-000160f0: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
-00016100: 707b 7061 6464 696e 673a 3135 7078 2169  p{padding:15px!i
-00016110: 6d70 6f72 7461 6e74 7d2e 7569 702d 6d6f  mportant}.uip-mo
-00016120: 6461 6c2d 2d73 6964 6562 6172 7b64 6973  dal--sidebar{dis
-00016130: 706c 6179 3a6e 6f6e 657d 7d40 6d65 6469  play:none}}@medi
-00016140: 6120 286d 696e 2d77 6964 7468 3a31 3434  a (min-width:144
-00016150: 3070 7829 7b2e 7569 702d 6d6f 6461 6c2d  0px){.uip-modal-
-00016160: 2d69 636f 6e2d 7072 6576 6965 777b 2d6d  -icon-preview{-m
-00016170: 732d 6772 6964 2d63 6f6c 756d 6e73 3a28  s-grid-columns:(
-00016180: 3166 7229 5b37 5d3b 6772 6964 2d74 656d  1fr)[7];grid-tem
-00016190: 706c 6174 652d 636f 6c75 6d6e 733a 7265  plate-columns:re
-000161a0: 7065 6174 2837 2c31 6672 297d 7d40 6d65  peat(7,1fr)}}@me
-000161b0: 6469 6120 286d 6178 2d77 6964 7468 3a31  dia (max-width:1
-000161c0: 3433 3970 7829 7b2e 7569 702d 6d6f 6461  439px){.uip-moda
-000161d0: 6c2d 2d69 636f 6e2d 7072 6576 6965 777b  l--icon-preview{
-000161e0: 2d6d 732d 6772 6964 2d63 6f6c 756d 6e73  -ms-grid-columns
-000161f0: 3a28 3166 7229 5b36 5d3b 6772 6964 2d74  :(1fr)[6];grid-t
-00016200: 656d 706c 6174 652d 636f 6c75 6d6e 733a  emplate-columns:
-00016210: 7265 7065 6174 2836 2c31 6672 297d 7d40  repeat(6,1fr)}}@
-00016220: 6d65 6469 6120 286d 6178 2d77 6964 7468  media (max-width
-00016230: 3a31 3032 3470 7829 7b2e 7569 702d 6d6f  :1024px){.uip-mo
-00016240: 6461 6c2d 2d69 636f 6e2d 7072 6576 6965  dal--icon-previe
-00016250: 777b 2d6d 732d 6772 6964 2d63 6f6c 756d  w{-ms-grid-colum
-00016260: 6e73 3a28 3166 7229 5b35 5d3b 6772 6964  ns:(1fr)[5];grid
-00016270: 2d74 656d 706c 6174 652d 636f 6c75 6d6e  -template-column
-00016280: 733a 7265 7065 6174 2835 2c31 6672 297d  s:repeat(5,1fr)}
-00016290: 7d40 6d65 6469 6120 286d 6178 2d77 6964  }@media (max-wid
-000162a0: 7468 3a37 3637 7078 297b 2e75 6970 2d6d  th:767px){.uip-m
-000162b0: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
-000162c0: 6577 7b2d 6d73 2d67 7269 642d 636f 6c75  ew{-ms-grid-colu
-000162d0: 6d6e 733a 2831 6672 295b 345d 3b67 7269  mns:(1fr)[4];gri
-000162e0: 642d 7465 6d70 6c61 7465 2d63 6f6c 756d  d-template-colum
-000162f0: 6e73 3a72 6570 6561 7428 342c 3166 7229  ns:repeat(4,1fr)
-00016300: 7d7d 406d 6564 6961 2028 6d61 782d 7769  }}@media (max-wi
-00016310: 6474 683a 3437 3970 7829 7b2e 7569 702d  dth:479px){.uip-
-00016320: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
-00016330: 6965 777b 2d6d 732d 6772 6964 2d63 6f6c  iew{-ms-grid-col
-00016340: 756d 6e73 3a28 3166 7229 5b33 5d3b 6772  umns:(1fr)[3];gr
-00016350: 6964 2d74 656d 706c 6174 652d 636f 6c75  id-template-colu
-00016360: 6d6e 733a 7265 7065 6174 2833 2c31 6672  mns:repeat(3,1fr
-00016370: 297d 7d40 6d65 6469 6120 286d 6178 2d77  )}}@media (max-w
-00016380: 6964 7468 3a31 3433 3970 7829 7b2e 7569  idth:1439px){.ui
-00016390: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
-000163a0: 2d74 6162 2d69 7465 6d7b 7061 6464 696e  -tab-item{paddin
-000163b0: 673a 3135 7078 2031 3570 7820 3135 7078  g:15px 15px 15px
-000163c0: 2032 3570 783b 666f 6e74 2d73 697a 653a   25px;font-size:
-000163d0: 3131 7078 7d2e 7569 702d 6d6f 6461 6c2d  11px}.uip-modal-
-000163e0: 2d73 6964 6562 6172 2d74 6162 2d69 7465  -sidebar-tab-ite
-000163f0: 6d20 697b 666f 6e74 2d73 697a 653a 3135  m i{font-size:15
-00016400: 7078 7d7d 406d 6564 6961 2028 6d61 782d  px}}@media (max-
-00016410: 7769 6474 683a 3130 3234 7078 297b 2e75  width:1024px){.u
-00016420: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
-00016430: 722d 7461 622d 6974 656d 2069 2c2e 7569  r-tab-item i,.ui
-00016440: 702d 6d6f 6461 6c2d 2d73 6964 6562 6172  p-modal--sidebar
-00016450: 2d74 6162 2d69 7465 6d20 696d 677b 6469  -tab-item img{di
-00016460: 7370 6c61 793a 6e6f 6e65 7d7d 2e73 722d  splay:none}}.sr-
-00016470: 6f6e 6c79 7b70 6f73 6974 696f 6e3a 6162  only{position:ab
-00016480: 736f 6c75 7465 2169 6d70 6f72 7461 6e74  solute!important
-00016490: 3b77 6964 7468 3a31 7078 2169 6d70 6f72  ;width:1px!impor
-000164a0: 7461 6e74 3b68 6569 6768 743a 3170 7821  tant;height:1px!
-000164b0: 696d 706f 7274 616e 743b 7061 6464 696e  important;paddin
-000164c0: 673a 3021 696d 706f 7274 616e 743b 6d61  g:0!important;ma
-000164d0: 7267 696e 3a2d 3170 7821 696d 706f 7274  rgin:-1px!import
-000164e0: 616e 743b 6f76 6572 666c 6f77 3a68 6964  ant;overflow:hid
-000164f0: 6465 6e21 696d 706f 7274 616e 743b 636c  den!important;cl
-00016500: 6970 3a72 6563 7428 302c 302c 302c 3029  ip:rect(0,0,0,0)
-00016510: 2169 6d70 6f72 7461 6e74 3b77 6869 7465  !important;white
-00016520: 2d73 7061 6365 3a6e 6f77 7261 7021 696d  -space:nowrap!im
-00016530: 706f 7274 616e 743b 626f 7264 6572 3a30  portant;border:0
-00016540: 2169 6d70 6f72 7461 6e74 7d75 6c2e 6e61  !important}ul.na
-00016550: 767b 6d61 7267 696e 2d62 6f74 746f 6d3a  v{margin-bottom:
-00016560: 3165 6d7d 756c 2e6e 6176 3e6c 692e 6e61  1em}ul.nav>li.na
-00016570: 762d 6974 656d 7b6c 6973 742d 7374 796c  v-item{list-styl
-00016580: 652d 7479 7065 3a6e 6f6e 653b 7061 6464  e-type:none;padd
-00016590: 696e 673a 696e 6865 7269 747d 2e63 6f6c  ing:inherit}.col
-000165a0: 4d20 756c 3a6e 6f74 282e 6f62 6a65 6374  M ul:not(.object
-000165b0: 2d74 6f6f 6c73 292e 6e61 767b 6d61 7267  -tools).nav{marg
-000165c0: 696e 2d74 6f70 3a30 3b6d 6172 6769 6e2d  in-top:0;margin-
-000165d0: 626f 7474 6f6d 3a32 3070 787d 756c 2e6e  bottom:20px}ul.n
-000165e0: 6176 202e 6e61 762d 6974 656d 7b6d 6172  av .nav-item{mar
-000165f0: 6769 6e2d 7269 6768 743a 3172 656d 7d75  gin-right:1rem}u
-00016600: 6c2e 6e61 7620 2e6e 6176 2d6c 696e 6b7b  l.nav .nav-link{
-00016610: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
-00016620: 653b 7465 7874 2d64 6563 6f72 6174 696f  e;text-decoratio
-00016630: 6e3a 6e6f 6e65 7d75 6c2e 6e61 7620 2e6e  n:none}ul.nav .n
-00016640: 6176 2d6c 696e 6b20 7370 616e 2e69 6e64  av-link span.ind
-00016650: 6963 6174 6f72 7b64 6973 706c 6179 3a6e  icator{display:n
-00016660: 6f6e 653b 626f 7264 6572 2d72 6164 6975  one;border-radiu
-00016670: 733a 3530 253b 7061 6464 696e 673a 2e35  s:50%;padding:.5
-00016680: 7265 6d3b 626f 7264 6572 3a31 7078 2073  rem;border:1px s
-00016690: 6f6c 6964 2076 6172 282d 2d64 6361 2d77  olid var(--dca-w
-000166a0: 6869 7465 2c76 6172 282d 2d62 6f64 792d  hite,var(--body-
-000166b0: 6267 2c23 6666 6629 293b 7472 616e 7366  bg,#fff));transf
-000166c0: 6f72 6d3a 7472 616e 736c 6174 6528 2d35  orm:translate(-5
-000166d0: 3025 2c2d 3530 2529 3b74 6f70 3a30 3b6c  0%,-50%);top:0;l
-000166e0: 6566 743a 3130 3025 3b70 6f73 6974 696f  eft:100%;positio
-000166f0: 6e3a 6162 736f 6c75 7465 7d75 6c2e 6e61  n:absolute}ul.na
-00016700: 7620 2e6e 6176 2d6c 696e 6b20 7370 616e  v .nav-link span
-00016710: 2e69 6e64 6963 6174 6f72 2e65 7272 6f72  .indicator.error
-00016720: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
-00016730: 723a 7661 7228 2d2d 6273 2d64 616e 6765  r:var(--bs-dange
-00016740: 7229 7d75 6c2e 6e61 7620 2e6e 6176 2d6c  r)}ul.nav .nav-l
-00016750: 696e 6b20 7370 616e 2e69 6e64 6963 6174  ink span.indicat
-00016760: 6f72 2e61 7474 7269 6275 7465 737b 6261  or.attributes{ba
-00016770: 636b 6772 6f75 6e64 2d63 6f6c 6f72 3a76  ckground-color:v
-00016780: 6172 282d 2d62 732d 696e 666f 293b 6469  ar(--bs-info);di
-00016790: 7370 6c61 793a 626c 6f63 6b7d 756c 2e6e  splay:block}ul.n
-000167a0: 6176 202e 6e61 762d 6c69 6e6b 2e65 7272  av .nav-link.err
-000167b0: 6f72 3e73 7061 6e2e 696e 6469 6361 746f  or>span.indicato
-000167c0: 727b 6469 7370 6c61 793a 626c 6f63 6b7d  r{display:block}
-000167d0: 756c 2e6e 6176 2e6e 6176 2d70 696c 6c73  ul.nav.nav-pills
-000167e0: 202e 6e61 762d 6c69 6e6b 3a6e 6f74 282e   .nav-link:not(.
-000167f0: 6163 7469 7665 297b 626f 7264 6572 2d73  active){border-s
-00016800: 7479 6c65 3a73 6f6c 6964 3b62 6f72 6465  tyle:solid;borde
-00016810: 722d 7769 6474 683a 3170 787d 626f 6479  r-width:1px}body
-00016820: 3a6e 6f74 282e 646a 616e 676f 636d 732d  :not(.djangocms-
-00016830: 6164 6d69 6e2d 7374 796c 6529 2075 6c2e  admin-style) ul.
-00016840: 646a 616e 676f 636d 732d 6672 6f6e 7465  djangocms-fronte
-00016850: 6e64 2e6e 6176 2d74 6162 732b 6469 762e  nd.nav-tabs+div.
-00016860: 7461 622d 636f 6e74 656e 7420 2e74 6162  tab-content .tab
-00016870: 2d70 616e 657b 626f 7264 6572 2d6c 6566  -pane{border-lef
-00016880: 742d 7374 796c 653a 736f 6c69 643b 626f  t-style:solid;bo
-00016890: 7264 6572 2d62 6f74 746f 6d2d 7374 796c  rder-bottom-styl
-000168a0: 653a 736f 6c69 643b 626f 7264 6572 2d72  e:solid;border-r
-000168b0: 6967 6874 2d73 7479 6c65 3a73 6f6c 6964  ight-style:solid
-000168c0: 3b62 6f72 6465 722d 6c65 6674 2d63 6f6c  ;border-left-col
-000168d0: 6f72 3a76 6172 282d 2d68 6169 726c 696e  or:var(--hairlin
-000168e0: 652d 636f 6c6f 7229 3b62 6f72 6465 722d  e-color);border-
-000168f0: 626f 7474 6f6d 2d63 6f6c 6f72 3a76 6172  bottom-color:var
-00016900: 282d 2d68 6169 726c 696e 652d 636f 6c6f  (--hairline-colo
-00016910: 7229 3b62 6f72 6465 722d 7269 6768 742d  r);border-right-
-00016920: 636f 6c6f 723a 7661 7228 2d2d 6861 6972  color:var(--hair
-00016930: 6c69 6e65 2d63 6f6c 6f72 293b 626f 7264  line-color);bord
-00016940: 6572 2d77 6964 7468 3a31 7078 7d62 6f64  er-width:1px}bod
-00016950: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
-00016960: 2d61 646d 696e 2d73 7479 6c65 2920 756c  -admin-style) ul
-00016970: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
-00016980: 656e 642e 6e61 762d 7461 6273 2b64 6976  end.nav-tabs+div
-00016990: 2e74 6162 2d63 6f6e 7465 6e74 202e 7461  .tab-content .ta
-000169a0: 622d 7061 6e65 2066 6965 6c64 7365 743a  b-pane fieldset:
-000169b0: 6c61 7374 2d63 6869 6c64 7b6d 6172 6769  last-child{margi
-000169c0: 6e2d 626f 7474 6f6d 3a30 7d64 6976 2e74  n-bottom:0}div.t
-000169d0: 6162 2d70 6b7b 2d6d 732d 666c 6578 2d69  ab-pk{-ms-flex-i
-000169e0: 7465 6d2d 616c 6967 6e3a 6365 6e74 6572  tem-align:center
-000169f0: 3b2d 6d73 2d67 7269 642d 726f 772d 616c  ;-ms-grid-row-al
-00016a00: 6967 6e3a 6365 6e74 6572 3b61 6c69 676e  ign:center;align
-00016a10: 2d73 656c 663a 6365 6e74 6572 3b63 6f6c  -self:center;col
-00016a20: 6f72 3a76 6172 282d 2d64 6361 2d67 7261  or:var(--dca-gra
-00016a30: 792d 6461 726b 6572 2c76 6172 282d 2d62  y-darker,var(--b
-00016a40: 6f64 792d 6667 2c23 3333 3329 293b 666f  ody-fg,#333));fo
-00016a50: 6e74 2d73 697a 653a 3830 253b 6d61 7267  nt-size:80%;marg
-00016a60: 696e 2d6c 6566 743a 6175 746f 7d2e 646a  in-left:auto}.dj
-00016a70: 616e 676f 636d 732d 6164 6d69 6e2d 7374  angocms-admin-st
-00016a80: 796c 6520 2e64 6a61 6e67 6f63 6d73 2d66  yle .djangocms-f
-00016a90: 726f 6e74 656e 6420 6c69 2e6e 6176 2d69  rontend li.nav-i
-00016aa0: 7465 6d7b 626f 7264 6572 2d74 6f70 3a6e  tem{border-top:n
-00016ab0: 6f6e 657d 696e 7075 745b 7479 7065 3d6e  one}input[type=n
-00016ac0: 756d 6265 725d 2e61 7574 6f2d 6669 656c  umber].auto-fiel
-00016ad0: 642b 7370 616e 7b64 6973 706c 6179 3a6e  d+span{display:n
-00016ae0: 6f6e 653b 706f 7369 7469 6f6e 3a61 6273  one;position:abs
-00016af0: 6f6c 7574 653b 626f 7474 6f6d 3a30 3b72  olute;bottom:0;r
-00016b00: 6967 6874 3a30 3b74 6578 742d 616c 6967  ight:0;text-alig
-00016b10: 6e3a 7269 6768 743b 6d61 7267 696e 2d72  n:right;margin-r
-00016b20: 6967 6874 3a33 3170 783b 6d61 7267 696e  ight:31px;margin
-00016b30: 2d62 6f74 746f 6d3a 3233 7078 3b63 7572  -bottom:23px;cur
-00016b40: 736f 723a 706f 696e 7465 727d 626f 6479  sor:pointer}body
-00016b50: 3a6e 6f74 282e 646a 616e 676f 636d 732d  :not(.djangocms-
-00016b60: 6164 6d69 6e2d 7374 796c 6529 2069 6e70  admin-style) inp
-00016b70: 7574 5b74 7970 653d 6e75 6d62 6572 5d2e  ut[type=number].
-00016b80: 6175 746f 2d66 6965 6c64 2b73 7061 6e7b  auto-field+span{
-00016b90: 6d61 7267 696e 2d62 6f74 746f 6d3a 3233  margin-bottom:23
-00016ba0: 7078 7d40 6d65 6469 6120 286d 6178 2d77  px}@media (max-w
-00016bb0: 6964 7468 3a31 3032 3470 7829 7b62 6f64  idth:1024px){bod
-00016bc0: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
-00016bd0: 2d61 646d 696e 2d73 7479 6c65 2920 696e  -admin-style) in
-00016be0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
-00016bf0: 2e61 7574 6f2d 6669 656c 642b 7370 616e  .auto-field+span
-00016c00: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a32  {margin-bottom:2
-00016c10: 3470 787d 7d69 6e70 7574 5b74 7970 653d  4px}}input[type=
-00016c20: 6e75 6d62 6572 5d2e 6175 746f 2d66 6965  number].auto-fie
-00016c30: 6c64 2b73 7061 6e3a 6166 7465 727b 636f  ld+span:after{co
-00016c40: 6e74 656e 743a 2261 7574 6f22 7d69 6e70  ntent:"auto"}inp
-00016c50: 7574 5b74 7970 653d 6e75 6d62 6572 5d2e  ut[type=number].
-00016c60: 6175 746f 2d66 6965 6c64 2e61 7574 6f7b  auto-field.auto{
-00016c70: 636f 6c6f 723a 7661 7228 2d2d 6463 612d  color:var(--dca-
-00016c80: 7768 6974 652c 7661 7228 2d2d 626f 6479  white,var(--body
-00016c90: 2d62 672c 2366 6666 2929 3b63 6172 6574  -bg,#fff));caret
-00016ca0: 2d63 6f6c 6f72 3a76 6172 282d 2d64 6361  -color:var(--dca
-00016cb0: 2d62 6c61 636b 2c76 6172 282d 2d62 6f64  -black,var(--bod
-00016cc0: 792d 6667 2c23 3030 3029 297d 696e 7075  y-fg,#000))}inpu
-00016cd0: 745b 7479 7065 3d6e 756d 6265 725d 2e61  t[type=number].a
-00016ce0: 7574 6f2d 6669 656c 642e 6175 746f 2b73  uto-field.auto+s
-00016cf0: 7061 6e7b 6469 7370 6c61 793a 626c 6f63  pan{display:bloc
-00016d00: 6b7d                                     k}
+00015fd0: 7078 297b 626f 6479 3a6e 6f74 282e 636d  px){body:not(.cm
+00015fe0: 732d 6164 6d69 6e2d 6d6f 6461 6c29 202e  s-admin-modal) .
+00015ff0: 7569 702d 6d6f 6461 6c20 2e75 6970 2d6d  uip-modal .uip-m
+00016000: 6f64 616c 2d2d 636f 6e74 656e 747b 6d61  odal--content{ma
+00016010: 782d 7769 6474 683a 3132 3030 7078 7d7d  x-width:1200px}}
+00016020: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
+00016030: 683a 3134 3339 7078 297b 626f 6479 3a6e  h:1439px){body:n
+00016040: 6f74 282e 636d 732d 6164 6d69 6e2d 6d6f  ot(.cms-admin-mo
+00016050: 6461 6c29 202e 7569 702d 6d6f 6461 6c20  dal) .uip-modal 
+00016060: 2e75 6970 2d6d 6f64 616c 2d2d 636f 6e74  .uip-modal--cont
+00016070: 656e 747b 6d61 782d 7769 6474 683a 3939  ent{max-width:99
+00016080: 3070 787d 2e75 6970 2d6d 6f64 616c 2d2d  0px}.uip-modal--
+00016090: 6963 6f6e 2d70 7265 7669 6577 2d77 7261  icon-preview-wra
+000160a0: 707b 7061 6464 696e 673a 3330 7078 2035  p{padding:30px 5
+000160b0: 3070 7820 307d 7d40 6d65 6469 6120 286d  0px 0}}@media (m
+000160c0: 6178 2d77 6964 7468 3a31 3032 3370 7829  ax-width:1023px)
+000160d0: 7b62 6f64 793a 6e6f 7428 2e63 6d73 2d61  {body:not(.cms-a
+000160e0: 646d 696e 2d6d 6f64 616c 2920 2e75 6970  dmin-modal) .uip
+000160f0: 2d6d 6f64 616c 202e 7569 702d 6d6f 6461  -modal .uip-moda
+00016100: 6c2d 2d63 6f6e 7465 6e74 7b6d 6178 2d77  l--content{max-w
+00016110: 6964 7468 3a37 3430 7078 7d7d 406d 6564  idth:740px}}@med
+00016120: 6961 2028 6d61 782d 7769 6474 683a 3736  ia (max-width:76
+00016130: 3770 7829 7b2e 7569 702d 6d6f 6461 6c2d  7px){.uip-modal-
+00016140: 2d69 636f 6e2d 7072 6576 6965 772d 7772  -icon-preview-wr
+00016150: 6170 7b70 6164 6469 6e67 3a31 3570 7821  ap{padding:15px!
+00016160: 696d 706f 7274 616e 747d 2e75 6970 2d6d  important}.uip-m
+00016170: 6f64 616c 2d2d 7369 6465 6261 727b 6469  odal--sidebar{di
+00016180: 7370 6c61 793a 6e6f 6e65 7d7d 406d 6564  splay:none}}@med
+00016190: 6961 2028 6d69 6e2d 7769 6474 683a 3134  ia (min-width:14
+000161a0: 3430 7078 297b 2e75 6970 2d6d 6f64 616c  40px){.uip-modal
+000161b0: 2d2d 6963 6f6e 2d70 7265 7669 6577 7b2d  --icon-preview{-
+000161c0: 6d73 2d67 7269 642d 636f 6c75 6d6e 733a  ms-grid-columns:
+000161d0: 2831 6672 295b 375d 3b67 7269 642d 7465  (1fr)[7];grid-te
+000161e0: 6d70 6c61 7465 2d63 6f6c 756d 6e73 3a72  mplate-columns:r
+000161f0: 6570 6561 7428 372c 3166 7229 7d7d 406d  epeat(7,1fr)}}@m
+00016200: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
+00016210: 3134 3339 7078 297b 2e75 6970 2d6d 6f64  1439px){.uip-mod
+00016220: 616c 2d2d 6963 6f6e 2d70 7265 7669 6577  al--icon-preview
+00016230: 7b2d 6d73 2d67 7269 642d 636f 6c75 6d6e  {-ms-grid-column
+00016240: 733a 2831 6672 295b 365d 3b67 7269 642d  s:(1fr)[6];grid-
+00016250: 7465 6d70 6c61 7465 2d63 6f6c 756d 6e73  template-columns
+00016260: 3a72 6570 6561 7428 362c 3166 7229 7d7d  :repeat(6,1fr)}}
+00016270: 406d 6564 6961 2028 6d61 782d 7769 6474  @media (max-widt
+00016280: 683a 3130 3234 7078 297b 2e75 6970 2d6d  h:1024px){.uip-m
+00016290: 6f64 616c 2d2d 6963 6f6e 2d70 7265 7669  odal--icon-previ
+000162a0: 6577 7b2d 6d73 2d67 7269 642d 636f 6c75  ew{-ms-grid-colu
+000162b0: 6d6e 733a 2831 6672 295b 355d 3b67 7269  mns:(1fr)[5];gri
+000162c0: 642d 7465 6d70 6c61 7465 2d63 6f6c 756d  d-template-colum
+000162d0: 6e73 3a72 6570 6561 7428 352c 3166 7229  ns:repeat(5,1fr)
+000162e0: 7d7d 406d 6564 6961 2028 6d61 782d 7769  }}@media (max-wi
+000162f0: 6474 683a 3736 3770 7829 7b2e 7569 702d  dth:767px){.uip-
+00016300: 6d6f 6461 6c2d 2d69 636f 6e2d 7072 6576  modal--icon-prev
+00016310: 6965 777b 2d6d 732d 6772 6964 2d63 6f6c  iew{-ms-grid-col
+00016320: 756d 6e73 3a28 3166 7229 5b34 5d3b 6772  umns:(1fr)[4];gr
+00016330: 6964 2d74 656d 706c 6174 652d 636f 6c75  id-template-colu
+00016340: 6d6e 733a 7265 7065 6174 2834 2c31 6672  mns:repeat(4,1fr
+00016350: 297d 7d40 6d65 6469 6120 286d 6178 2d77  )}}@media (max-w
+00016360: 6964 7468 3a34 3739 7078 297b 2e75 6970  idth:479px){.uip
+00016370: 2d6d 6f64 616c 2d2d 6963 6f6e 2d70 7265  -modal--icon-pre
+00016380: 7669 6577 7b2d 6d73 2d67 7269 642d 636f  view{-ms-grid-co
+00016390: 6c75 6d6e 733a 2831 6672 295b 335d 3b67  lumns:(1fr)[3];g
+000163a0: 7269 642d 7465 6d70 6c61 7465 2d63 6f6c  rid-template-col
+000163b0: 756d 6e73 3a72 6570 6561 7428 332c 3166  umns:repeat(3,1f
+000163c0: 7229 7d7d 406d 6564 6961 2028 6d61 782d  r)}}@media (max-
+000163d0: 7769 6474 683a 3134 3339 7078 297b 2e75  width:1439px){.u
+000163e0: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+000163f0: 722d 7461 622d 6974 656d 7b70 6164 6469  r-tab-item{paddi
+00016400: 6e67 3a31 3570 7820 3135 7078 2031 3570  ng:15px 15px 15p
+00016410: 7820 3235 7078 3b66 6f6e 742d 7369 7a65  x 25px;font-size
+00016420: 3a31 3170 787d 2e75 6970 2d6d 6f64 616c  :11px}.uip-modal
+00016430: 2d2d 7369 6465 6261 722d 7461 622d 6974  --sidebar-tab-it
+00016440: 656d 2069 7b66 6f6e 742d 7369 7a65 3a31  em i{font-size:1
+00016450: 3570 787d 7d40 6d65 6469 6120 286d 6178  5px}}@media (max
+00016460: 2d77 6964 7468 3a31 3032 3470 7829 7b2e  -width:1024px){.
+00016470: 7569 702d 6d6f 6461 6c2d 2d73 6964 6562  uip-modal--sideb
+00016480: 6172 2d74 6162 2d69 7465 6d20 692c 2e75  ar-tab-item i,.u
+00016490: 6970 2d6d 6f64 616c 2d2d 7369 6465 6261  ip-modal--sideba
+000164a0: 722d 7461 622d 6974 656d 2069 6d67 7b64  r-tab-item img{d
+000164b0: 6973 706c 6179 3a6e 6f6e 657d 7d2e 7372  isplay:none}}.sr
+000164c0: 2d6f 6e6c 797b 706f 7369 7469 6f6e 3a61  -only{position:a
+000164d0: 6273 6f6c 7574 6521 696d 706f 7274 616e  bsolute!importan
+000164e0: 743b 7769 6474 683a 3170 7821 696d 706f  t;width:1px!impo
+000164f0: 7274 616e 743b 6865 6967 6874 3a31 7078  rtant;height:1px
+00016500: 2169 6d70 6f72 7461 6e74 3b70 6164 6469  !important;paddi
+00016510: 6e67 3a30 2169 6d70 6f72 7461 6e74 3b6d  ng:0!important;m
+00016520: 6172 6769 6e3a 2d31 7078 2169 6d70 6f72  argin:-1px!impor
+00016530: 7461 6e74 3b6f 7665 7266 6c6f 773a 6869  tant;overflow:hi
+00016540: 6464 656e 2169 6d70 6f72 7461 6e74 3b63  dden!important;c
+00016550: 6c69 703a 7265 6374 2830 2c30 2c30 2c30  lip:rect(0,0,0,0
+00016560: 2921 696d 706f 7274 616e 743b 7768 6974  )!important;whit
+00016570: 652d 7370 6163 653a 6e6f 7772 6170 2169  e-space:nowrap!i
+00016580: 6d70 6f72 7461 6e74 3b62 6f72 6465 723a  mportant;border:
+00016590: 3021 696d 706f 7274 616e 747d 756c 2e6e  0!important}ul.n
+000165a0: 6176 7b6d 6172 6769 6e2d 626f 7474 6f6d  av{margin-bottom
+000165b0: 3a31 656d 7d75 6c2e 6e61 763e 6c69 2e6e  :1em}ul.nav>li.n
+000165c0: 6176 2d69 7465 6d7b 6c69 7374 2d73 7479  av-item{list-sty
+000165d0: 6c65 2d74 7970 653a 6e6f 6e65 3b70 6164  le-type:none;pad
+000165e0: 6469 6e67 3a69 6e68 6572 6974 7d2e 636f  ding:inherit}.co
+000165f0: 6c4d 2075 6c3a 6e6f 7428 2e6f 626a 6563  lM ul:not(.objec
+00016600: 742d 746f 6f6c 7329 2e6e 6176 7b6d 6172  t-tools).nav{mar
+00016610: 6769 6e2d 746f 703a 303b 6d61 7267 696e  gin-top:0;margin
+00016620: 2d62 6f74 746f 6d3a 3230 7078 7d75 6c2e  -bottom:20px}ul.
+00016630: 6e61 7620 2e6e 6176 2d69 7465 6d7b 6d61  nav .nav-item{ma
+00016640: 7267 696e 2d72 6967 6874 3a31 7265 6d7d  rgin-right:1rem}
+00016650: 756c 2e6e 6176 202e 6e61 762d 6c69 6e6b  ul.nav .nav-link
+00016660: 7b70 6f73 6974 696f 6e3a 7265 6c61 7469  {position:relati
+00016670: 7665 3b74 6578 742d 6465 636f 7261 7469  ve;text-decorati
+00016680: 6f6e 3a6e 6f6e 657d 756c 2e6e 6176 202e  on:none}ul.nav .
+00016690: 6e61 762d 6c69 6e6b 2073 7061 6e2e 696e  nav-link span.in
+000166a0: 6469 6361 746f 727b 6469 7370 6c61 793a  dicator{display:
+000166b0: 6e6f 6e65 3b62 6f72 6465 722d 7261 6469  none;border-radi
+000166c0: 7573 3a35 3025 3b70 6164 6469 6e67 3a2e  us:50%;padding:.
+000166d0: 3572 656d 3b62 6f72 6465 723a 3170 7820  5rem;border:1px 
+000166e0: 736f 6c69 6420 7661 7228 2d2d 6463 612d  solid var(--dca-
+000166f0: 7768 6974 652c 7661 7228 2d2d 626f 6479  white,var(--body
+00016700: 2d62 672c 2366 6666 2929 3b74 7261 6e73  -bg,#fff));trans
+00016710: 666f 726d 3a74 7261 6e73 6c61 7465 282d  form:translate(-
+00016720: 3530 252c 2d35 3025 293b 746f 703a 303b  50%,-50%);top:0;
+00016730: 6c65 6674 3a31 3030 253b 706f 7369 7469  left:100%;positi
+00016740: 6f6e 3a61 6273 6f6c 7574 657d 756c 2e6e  on:absolute}ul.n
+00016750: 6176 202e 6e61 762d 6c69 6e6b 2073 7061  av .nav-link spa
+00016760: 6e2e 696e 6469 6361 746f 722e 6572 726f  n.indicator.erro
+00016770: 727b 6261 636b 6772 6f75 6e64 2d63 6f6c  r{background-col
+00016780: 6f72 3a76 6172 282d 2d62 732d 6461 6e67  or:var(--bs-dang
+00016790: 6572 297d 756c 2e6e 6176 202e 6e61 762d  er)}ul.nav .nav-
+000167a0: 6c69 6e6b 2073 7061 6e2e 696e 6469 6361  link span.indica
+000167b0: 746f 722e 6174 7472 6962 7574 6573 7b62  tor.attributes{b
+000167c0: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
+000167d0: 7661 7228 2d2d 6273 2d69 6e66 6f29 3b64  var(--bs-info);d
+000167e0: 6973 706c 6179 3a62 6c6f 636b 7d75 6c2e  isplay:block}ul.
+000167f0: 6e61 7620 2e6e 6176 2d6c 696e 6b2e 6572  nav .nav-link.er
+00016800: 726f 723e 7370 616e 2e69 6e64 6963 6174  ror>span.indicat
+00016810: 6f72 7b64 6973 706c 6179 3a62 6c6f 636b  or{display:block
+00016820: 7d75 6c2e 6e61 762e 6e61 762d 7069 6c6c  }ul.nav.nav-pill
+00016830: 7320 2e6e 6176 2d6c 696e 6b3a 6e6f 7428  s .nav-link:not(
+00016840: 2e61 6374 6976 6529 7b62 6f72 6465 722d  .active){border-
+00016850: 7374 796c 653a 736f 6c69 643b 626f 7264  style:solid;bord
+00016860: 6572 2d77 6964 7468 3a31 7078 7d62 6f64  er-width:1px}bod
+00016870: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
+00016880: 2d61 646d 696e 2d73 7479 6c65 2920 756c  -admin-style) ul
+00016890: 2e64 6a61 6e67 6f63 6d73 2d66 726f 6e74  .djangocms-front
+000168a0: 656e 642e 6e61 762d 7461 6273 2b64 6976  end.nav-tabs+div
+000168b0: 2e74 6162 2d63 6f6e 7465 6e74 202e 7461  .tab-content .ta
+000168c0: 622d 7061 6e65 7b62 6f72 6465 722d 6c65  b-pane{border-le
+000168d0: 6674 2d73 7479 6c65 3a73 6f6c 6964 3b62  ft-style:solid;b
+000168e0: 6f72 6465 722d 626f 7474 6f6d 2d73 7479  order-bottom-sty
+000168f0: 6c65 3a73 6f6c 6964 3b62 6f72 6465 722d  le:solid;border-
+00016900: 7269 6768 742d 7374 796c 653a 736f 6c69  right-style:soli
+00016910: 643b 626f 7264 6572 2d6c 6566 742d 636f  d;border-left-co
+00016920: 6c6f 723a 7661 7228 2d2d 6861 6972 6c69  lor:var(--hairli
+00016930: 6e65 2d63 6f6c 6f72 293b 626f 7264 6572  ne-color);border
+00016940: 2d62 6f74 746f 6d2d 636f 6c6f 723a 7661  -bottom-color:va
+00016950: 7228 2d2d 6861 6972 6c69 6e65 2d63 6f6c  r(--hairline-col
+00016960: 6f72 293b 626f 7264 6572 2d72 6967 6874  or);border-right
+00016970: 2d63 6f6c 6f72 3a76 6172 282d 2d68 6169  -color:var(--hai
+00016980: 726c 696e 652d 636f 6c6f 7229 3b62 6f72  rline-color);bor
+00016990: 6465 722d 7769 6474 683a 3170 787d 626f  der-width:1px}bo
+000169a0: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
+000169b0: 732d 6164 6d69 6e2d 7374 796c 6529 2075  s-admin-style) u
+000169c0: 6c2e 646a 616e 676f 636d 732d 6672 6f6e  l.djangocms-fron
+000169d0: 7465 6e64 2e6e 6176 2d74 6162 732b 6469  tend.nav-tabs+di
+000169e0: 762e 7461 622d 636f 6e74 656e 7420 2e74  v.tab-content .t
+000169f0: 6162 2d70 616e 6520 6669 656c 6473 6574  ab-pane fieldset
+00016a00: 3a6c 6173 742d 6368 696c 647b 6d61 7267  :last-child{marg
+00016a10: 696e 2d62 6f74 746f 6d3a 307d 6469 762e  in-bottom:0}div.
+00016a20: 7461 622d 706b 7b2d 6d73 2d66 6c65 782d  tab-pk{-ms-flex-
+00016a30: 6974 656d 2d61 6c69 676e 3a63 656e 7465  item-align:cente
+00016a40: 723b 2d6d 732d 6772 6964 2d72 6f77 2d61  r;-ms-grid-row-a
+00016a50: 6c69 676e 3a63 656e 7465 723b 616c 6967  lign:center;alig
+00016a60: 6e2d 7365 6c66 3a63 656e 7465 723b 636f  n-self:center;co
+00016a70: 6c6f 723a 7661 7228 2d2d 6463 612d 6772  lor:var(--dca-gr
+00016a80: 6179 2d64 6172 6b65 722c 7661 7228 2d2d  ay-darker,var(--
+00016a90: 626f 6479 2d66 672c 2333 3333 2929 3b66  body-fg,#333));f
+00016aa0: 6f6e 742d 7369 7a65 3a38 3025 3b6d 6172  ont-size:80%;mar
+00016ab0: 6769 6e2d 6c65 6674 3a61 7574 6f7d 2e64  gin-left:auto}.d
+00016ac0: 6a61 6e67 6f63 6d73 2d61 646d 696e 2d73  jangocms-admin-s
+00016ad0: 7479 6c65 202e 646a 616e 676f 636d 732d  tyle .djangocms-
+00016ae0: 6672 6f6e 7465 6e64 206c 692e 6e61 762d  frontend li.nav-
+00016af0: 6974 656d 7b62 6f72 6465 722d 746f 703a  item{border-top:
+00016b00: 6e6f 6e65 7d69 6e70 7574 5b74 7970 653d  none}input[type=
+00016b10: 6e75 6d62 6572 5d2e 6175 746f 2d66 6965  number].auto-fie
+00016b20: 6c64 2b73 7061 6e7b 6469 7370 6c61 793a  ld+span{display:
+00016b30: 6e6f 6e65 3b70 6f73 6974 696f 6e3a 6162  none;position:ab
+00016b40: 736f 6c75 7465 3b62 6f74 746f 6d3a 303b  solute;bottom:0;
+00016b50: 7269 6768 743a 303b 7465 7874 2d61 6c69  right:0;text-ali
+00016b60: 676e 3a72 6967 6874 3b6d 6172 6769 6e2d  gn:right;margin-
+00016b70: 7269 6768 743a 3331 7078 3b6d 6172 6769  right:31px;margi
+00016b80: 6e2d 626f 7474 6f6d 3a32 3370 783b 6375  n-bottom:23px;cu
+00016b90: 7273 6f72 3a70 6f69 6e74 6572 7d62 6f64  rsor:pointer}bod
+00016ba0: 793a 6e6f 7428 2e64 6a61 6e67 6f63 6d73  y:not(.djangocms
+00016bb0: 2d61 646d 696e 2d73 7479 6c65 2920 696e  -admin-style) in
+00016bc0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
+00016bd0: 2e61 7574 6f2d 6669 656c 642b 7370 616e  .auto-field+span
+00016be0: 7b6d 6172 6769 6e2d 626f 7474 6f6d 3a32  {margin-bottom:2
+00016bf0: 3370 787d 406d 6564 6961 2028 6d61 782d  3px}@media (max-
+00016c00: 7769 6474 683a 3130 3234 7078 297b 626f  width:1024px){bo
+00016c10: 6479 3a6e 6f74 282e 646a 616e 676f 636d  dy:not(.djangocm
+00016c20: 732d 6164 6d69 6e2d 7374 796c 6529 2069  s-admin-style) i
+00016c30: 6e70 7574 5b74 7970 653d 6e75 6d62 6572  nput[type=number
+00016c40: 5d2e 6175 746f 2d66 6965 6c64 2b73 7061  ].auto-field+spa
+00016c50: 6e7b 6d61 7267 696e 2d62 6f74 746f 6d3a  n{margin-bottom:
+00016c60: 3234 7078 7d7d 696e 7075 745b 7479 7065  24px}}input[type
+00016c70: 3d6e 756d 6265 725d 2e61 7574 6f2d 6669  =number].auto-fi
+00016c80: 656c 642b 7370 616e 3a61 6674 6572 7b63  eld+span:after{c
+00016c90: 6f6e 7465 6e74 3a22 6175 746f 227d 696e  ontent:"auto"}in
+00016ca0: 7075 745b 7479 7065 3d6e 756d 6265 725d  put[type=number]
+00016cb0: 2e61 7574 6f2d 6669 656c 642e 6175 746f  .auto-field.auto
+00016cc0: 7b63 6f6c 6f72 3a76 6172 282d 2d64 6361  {color:var(--dca
+00016cd0: 2d77 6869 7465 2c76 6172 282d 2d62 6f64  -white,var(--bod
+00016ce0: 792d 6267 2c23 6666 6629 293b 6361 7265  y-bg,#fff));care
+00016cf0: 742d 636f 6c6f 723a 7661 7228 2d2d 6463  t-color:var(--dc
+00016d00: 612d 626c 6163 6b2c 7661 7228 2d2d 626f  a-black,var(--bo
+00016d10: 6479 2d66 672c 2330 3030 2929 7d69 6e70  dy-fg,#000))}inp
+00016d20: 7574 5b74 7970 653d 6e75 6d62 6572 5d2e  ut[type=number].
+00016d30: 6175 746f 2d66 6965 6c64 2e61 7574 6f2b  auto-field.auto+
+00016d40: 7370 616e 7b64 6973 706c 6179 3a62 6c6f  span{display:blo
+00016d50: 636b 7d                                  ck}
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/css/select2.css` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/css/select2.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms-frontend-1.1.2/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms-frontend-1.1.2/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend/templatetags/frontend.py` & `djangocms-frontend-1.1.2/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend.egg-info/PKG-INFO` & `djangocms-frontend-1.1.2/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.1
+Version: 1.1.2
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -40,14 +40,16 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/x-rst
 Provides-Extra: djangocms-icon
 Provides-Extra: static-ace
+Provides-Extra: cms-4
+Provides-Extra: cms-3
 License-File: LICENSE
 
 #####################
  django CMS Frontend
 #####################
 
 |pypi| |docs| |coverage| |python| |django| |djangocms| |djangocms4|
@@ -208,15 +210,15 @@
 
 .. |coverage| image:: https://codecov.io/gh/fsbraun/djangocms-frontend/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/django-cms/djangocms-frontend
 
 .. |python| image:: https://img.shields.io/badge/python-3.7+-blue.svg
    :target: https://pypi.org/project/djangocms-frontend/
 
-.. |django| image:: https://img.shields.io/badge/django-3.2--4.1-blue.svg
+.. |django| image:: https://img.shields.io/badge/django-3.2--4.2-blue.svg
    :target: https://www.djangoproject.com/
 
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.8%2B-blue.svg
    :target: https://www.django-cms.org/
 
 .. |djangocms4| image:: https://img.shields.io/badge/django%20CMS-4-blue.svg
    :target: https://www.django-cms.org/en/preview-django-cms-40/
```

### Comparing `djangocms-frontend-1.1.1/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms-frontend-1.1.2/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/pyproject.toml` & `djangocms-frontend-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/setup.py` & `djangocms-frontend-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,22 @@
 EXTRA_REQUIREMENTS = {
     "djangocms-icon": [
         "djangocms-icon>=1.4.0",
     ],
     "static-ace": [
         "djangocms-static-ace",
     ],
+    "cms-4": [
+        "django-cms>=4.1.0rc2",
+        "django-parler",
+    ],
+    "cms-3": [
+        "django-cms<4",
+        "django-parler",
+    ],
 }
 
 CLASSIFIERS = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
```

### Comparing `djangocms-frontend-1.1.1/tests/accordion/test_models.py` & `djangocms-frontend-1.1.2/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/accordion/test_plugins.py` & `djangocms-frontend-1.1.2/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/alert/test_plugins.py` & `djangocms-frontend-1.1.2/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/badge/test_plugins.py` & `djangocms-frontend-1.1.2/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/card/test_models.py` & `djangocms-frontend-1.1.2/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/card/test_plugins.py` & `djangocms-frontend-1.1.2/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/carousel/test_models.py` & `djangocms-frontend-1.1.2/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/carousel/test_plugins.py` & `djangocms-frontend-1.1.2/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/collapse/test_models.py` & `djangocms-frontend-1.1.2/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/collapse/test_plugins.py` & `djangocms-frontend-1.1.2/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/content/test_models.py` & `djangocms-frontend-1.1.2/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/content/test_plugins.py` & `djangocms-frontend-1.1.2/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/fixtures.py` & `djangocms-frontend-1.1.2/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/grid/test_models.py` & `djangocms-frontend-1.1.2/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/grid/test_plugins.py` & `djangocms-frontend-1.1.2/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/helpers.py` & `djangocms-frontend-1.1.2/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/icon/test_models.py` & `djangocms-frontend-1.1.2/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/icon/test_plugins.py` & `djangocms-frontend-1.1.2/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/image/test_plugins.py` & `djangocms-frontend-1.1.2/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/jumbotron/test_plugins.py` & `djangocms-frontend-1.1.2/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/link/test_plugins.py` & `djangocms-frontend-1.1.2/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/listgroup/test_models.py` & `djangocms-frontend-1.1.2/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/listgroup/test_plugins.py` & `djangocms-frontend-1.1.2/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/media/test_models.py` & `djangocms-frontend-1.1.2/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/media/test_plugins.py` & `djangocms-frontend-1.1.2/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/navigation/test_models.py` & `djangocms-frontend-1.1.2/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/navigation/test_plugins.py` & `djangocms-frontend-1.1.2/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/tabs/test_models.py` & `djangocms-frontend-1.1.2/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/tabs/test_plugins.py` & `djangocms-frontend-1.1.2/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/test_constants.py` & `djangocms-frontend-1.1.2/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/test_fields.py` & `djangocms-frontend-1.1.2/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/test_helpers.py` & `djangocms-frontend-1.1.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/test_migrations.py` & `djangocms-frontend-1.1.2/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/test_settings.py` & `djangocms-frontend-1.1.2/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/utilities/test_models.py` & `djangocms-frontend-1.1.2/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.1/tests/utilities/test_plugins.py` & `djangocms-frontend-1.1.2/tests/utilities/test_plugins.py`

 * *Files identical despite different names*

