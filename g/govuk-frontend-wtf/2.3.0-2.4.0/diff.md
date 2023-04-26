# Comparing `tmp/govuk-frontend-wtf-2.3.0.tar.gz` & `tmp/govuk-frontend-wtf-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk-frontend-wtf-2.3.0.tar", last modified: Wed Feb 15 15:47:00 2023, max compression
+gzip compressed data, was "govuk-frontend-wtf-2.4.0.tar", last modified: Tue Apr 25 18:57:58 2023, max compression
```

## Comparing `govuk-frontend-wtf-2.3.0.tar` & `govuk-frontend-wtf-2.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:47:00.052159 govuk-frontend-wtf-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-02-15 15:47:00.052159 govuk-frontend-wtf-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:47:00.048159 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/gov_form_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:47:00.052159 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/button.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/charactercount.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/checkboxes.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/date.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/file-upload.html
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/input.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/radios.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/templates/textarea.html
--rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/wtforms_widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:47:00.048159 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-02-15 15:47:00.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-15 15:47:00.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 15:47:00.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-15 15:47:00.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-15 15:47:00.000000 govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-02-15 15:47:00.052159 govuk-frontend-wtf-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 15:47:00.052159 govuk-frontend-wtf-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-02-15 15:46:46.000000 govuk-frontend-wtf-2.3.0/tests/test_wtf_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10736 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.580022 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/gov_form_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/charactercount.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/checkboxes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/file-upload.html
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/radios.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/templates/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/wtforms_widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.584022 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-25 18:57:58.000000 govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:57:58.588023 govuk-frontend-wtf-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-25 18:57:45.000000 govuk-frontend-wtf-2.4.0/tests/test_wtf_widgets.py
```

### Comparing `govuk-frontend-wtf-2.3.0/LICENSE` & `govuk-frontend-wtf-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.3.0/PKG-INFO` & `govuk-frontend-wtf-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 2.3.0
+Version: 2.4.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.5.0](https://img.shields.io/badge/govuk--frontend%20version-4.5.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
@@ -197,18 +197,16 @@
 
 We welcome contribution from the community. If you want to contribute to this project, please review the [code of conduct](CODE_OF_CONDUCT.md) and [contribution guidelines](CONTRIBUTING.md).
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
-- [Hugo Baldwin](https://github.com/byzantime)
-- [Dale Potter](https://github.com/dalepotter)
-- [Gabriel Ionescu](https://github.com/ionescuig)
-- [Matt Pease](https://github.com/Skablam)
+
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-wtf/graphs/contributors)
 
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
```

### Comparing `govuk-frontend-wtf-2.3.0/README.md` & `govuk-frontend-wtf-2.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.5.0](https://img.shields.io/badge/govuk--frontend%20version-4.5.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
@@ -173,18 +173,16 @@
 
 We welcome contribution from the community. If you want to contribute to this project, please review the [code of conduct](CODE_OF_CONDUCT.md) and [contribution guidelines](CONTRIBUTING.md).
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
-- [Hugo Baldwin](https://github.com/byzantime)
-- [Dale Potter](https://github.com/dalepotter)
-- [Gabriel Ionescu](https://github.com/ionescuig)
-- [Matt Pease](https://github.com/Skablam)
+
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-wtf/graphs/contributors)
 
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
```

### Comparing `govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/gov_form_base.py` & `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/gov_form_base.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/main.py` & `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/main.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.3.0/govuk_frontend_wtf/wtforms_widgets.py` & `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf/wtforms_widgets.py`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/PKG-INFO` & `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-wtf
-Version: 2.3.0
+Version: 2.4.0
 Summary: GOV.UK Frontend WTForms Widgets
 Home-page: https://github.com/LandRegistry/govuk-frontend-wtf
 Author: Matt Shaw
 Author-email: matthew.shaw@landregistry.gov.uk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GOV.UK Frontend WTForms Widgets
 
 [![PyPI version](https://badge.fury.io/py/govuk-frontend-wtf.svg)](https://pypi.org/project/govuk-frontend-wtf/)
-![govuk-frontend 4.5.0](https://img.shields.io/badge/govuk--frontend%20version-4.5.0-005EA5?logo=gov.uk&style=flat)
+![govuk-frontend 4.6.0](https://img.shields.io/badge/govuk--frontend%20version-4.6.0-005EA5?logo=gov.uk&style=flat)
 [![Python package](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml/badge.svg)](https://github.com/LandRegistry/govuk-frontend-wtf/actions/workflows/python-package.yml)
 
 **GOV.UK Frontend WTForms is a [community tool](https://design-system.service.gov.uk/community/resources-and-tools/) of the [GOV.UK Design System](https://design-system.service.gov.uk/). The Design System team is not responsible for it and cannot support you with using it. Contact the [maintainers](#contributors) directly if you need [help](#support) or you want to request a feature.**
 
 This repository contains a set of [WTForms widgets](https://wtforms.readthedocs.io/en/2.3.x/widgets/) used to render [WTForm fields](https://wtforms.readthedocs.io/en/2.3.x/fields/) using [GOV.UK Frontend](https://design-system.service.gov.uk/) component styling. This is done using Jinja macros from the [GOV.UK Frontend Jinja](https://github.com/LandRegistry/govuk-frontend-jinja) port of the original GOV.UK Frontend Nunjucks macros. These are kept up-to-date with GOV.UK Frontend releases, are thoroughly tested and produce 100% equivalent markup.
 
 This approach also renders the associated error messages in the appropriate place, shows the error summary component at the top of the page and sets all related accessibility ARIA attributes. Adding the appropriate [widget](#widgets) to your existing form Python class, along with far simpler templates, makes it quick and easy to produce fully GOV.UK compliant forms.
@@ -197,18 +197,16 @@
 
 We welcome contribution from the community. If you want to contribute to this project, please review the [code of conduct](CODE_OF_CONDUCT.md) and [contribution guidelines](CONTRIBUTING.md).
 
 ## Contributors
 
 - [Matt Shaw](https://github.com/matthew-shaw) (Primary maintainer)
 - [Andy Mantell](https://github.com/andymantell) (Original author)
-- [Hugo Baldwin](https://github.com/byzantime)
-- [Dale Potter](https://github.com/dalepotter)
-- [Gabriel Ionescu](https://github.com/ionescuig)
-- [Matt Pease](https://github.com/Skablam)
+
+See the full list of [contributors on GitHub](https://github.com/LandRegistry/govuk-frontend-wtf/graphs/contributors)
 
 ## Support
 
 This software is provided _"as-is"_ without warranty. Support is provided on a _"best endeavours"_ basis by the maintainers and open source community.
 
 If you are a civil servant you can sign up to the [UK Government Digital Slack](https://ukgovernmentdigital.slack.com/signup) workspace to contact the maintainers listed [above](#contributors) and the community of people using this project in the [#govuk-design-system](https://ukgovernmentdigital.slack.com/archives/C6DMEH5R6) channel.
```

### Comparing `govuk-frontend-wtf-2.3.0/govuk_frontend_wtf.egg-info/SOURCES.txt` & `govuk-frontend-wtf-2.4.0/govuk_frontend_wtf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `govuk-frontend-wtf-2.3.0/setup.py` & `govuk-frontend-wtf-2.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 templates = []
 directories = glob.glob("govuk_frontend_wtf/templates/*.html")
 for directory in directories:
     templates.append(os.path.relpath(os.path.dirname(directory), "govuk_frontend_wtf") + "/*.html")
 
 setuptools.setup(
     name="govuk-frontend-wtf",
-    version="2.3.0",
+    version="2.4.0",
     author="Matt Shaw",
     author_email="matthew.shaw@landregistry.gov.uk",
     description="GOV.UK Frontend WTForms Widgets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LandRegistry/govuk-frontend-wtf",
     packages=setuptools.find_packages(exclude=["tests"]),
```

### Comparing `govuk-frontend-wtf-2.3.0/tests/test_wtf_widgets.py` & `govuk-frontend-wtf-2.4.0/tests/test_wtf_widgets.py`

 * *Files identical despite different names*

