# Comparing `tmp/docassemble.ALToolbox-0.7.1.tar.gz` & `tmp/docassemble.ALToolbox-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble.ALToolbox-0.7.1.tar", last modified: Tue Feb 14 21:48:58 2023, max compression
+gzip compressed data, was "docassemble.ALToolbox-0.8.0.tar", last modified: Tue Apr 25 15:59:37 2023, max compression
```

## Comparing `docassemble.ALToolbox-0.7.1.tar` & `docassemble.ALToolbox-0.8.0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.542558 docassemble.ALToolbox-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-02-14 21:48:58.546558 docassemble.ALToolbox-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.534557 docassemble.ALToolbox-0.7.1/docassemble/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.538558 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/
--rw-r--r--   0 runner    (1001) docker     (122)      714 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/Addup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/PhoneNumberDataType.py
--rw-r--r--   0 runner    (1001) docker     (122)     9042 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/ThreePartsDate.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/addenda.py
--rw-r--r--   0 runner    (1001) docker     (122)    50493 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/al_income.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/business_days.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/copy_button.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.534557 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.542558 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/
--rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Addup.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Bells and whistles.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Profiling.yml
--rw-r--r--   0 runner    (1001) docker     (122)      923 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Shorten a url.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/TextCounter.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1580 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/ThreePartsDate.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml
--rw-r--r--   0 runner    (1001) docker     (122)    26884 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/al_income.yml
--rw-r--r--   0 runner    (1001) docker     (122)    15092 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/al_income_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/altoolbox_overview.yml
--rw-r--r--   0 runner    (1001) docker     (122)     6056 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/business_days_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/collapse_template.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/collapse_template_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/copy_button.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/copy_button_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      146 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/display_template.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/display_template_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/escape_button.yml
--rw-r--r--   0 runner    (1001) docker     (122)      874 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/escape_button_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/multiselect.yml
--rw-r--r--   0 runner    (1001) docker     (122)      525 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/phone-number-validation.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/review_demo.yml
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/review_widget.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/save_input_data_demo.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.542558 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/sources/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/sources/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.542558 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/TextCounter.js
--rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.css
--rw-r--r--   0 runner    (1001) docker     (122)    81271 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.js
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/collapse_template.css
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/copy_button.css
--rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/copy_button.js
--rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/custom_504.html
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/display_template.css
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/escape_button.js
--rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/phone-number-validation.js
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/phone-number-validator.css
--rw-r--r--   0 runner    (1001) docker     (122)      122 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/review_widget.css
--rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/review_widget.js
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.542558 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (122)   184585 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/debts.pdf
--rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/output-checkbox.docx
--rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/table-addendum.docx
--rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx
--rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx
--rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/display_template.py
--rw-r--r--   0 runner    (1001) docker     (122)    10955 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/save_input_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6812 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/test_al_income.py
--rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/test_altoolbox.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/docassemble/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-14 21:48:58.534557 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3008 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3862 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-02-14 21:48:58.000000 docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      394 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-14 21:48:58.546558 docassemble.ALToolbox-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5252 2023-02-14 21:48:46.000000 docassemble.ALToolbox-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2754 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/
+-rw-r--r--   0 runner    (1001) docker     (122)      714 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/Addup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/PhoneNumberDataType.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37755 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/ThreePartsDate.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5634 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/addenda.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50493 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/al_income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/business_days.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2387 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/copy_button.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.566706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.574706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1406 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Addup.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Bells and whistles.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Profiling.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Shorten a url.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/TextCounter.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/ThreePartsDate.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2122 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2397 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3155 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    26884 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    15092 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3844 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/altoolbox_overview.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     6056 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/business_days_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      146 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4843 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      458 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      874 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      863 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1216 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone-number-validation.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1709 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_widget.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3717 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/save_input_data_demo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4588 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/three_parts_date_demo.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.574706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/sources/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1424 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/TextCounter.js
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/al_three_parts_date.css
+-rw-r--r--   0 runner    (1001) docker     (122)     6024 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.css
+-rw-r--r--   0 runner    (1001) docker     (122)    81271 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.js
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/collapse_template.css
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1606 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3428 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/custom_504.html
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/display_template.css
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/escape_button.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2955 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validation.js
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validator.css
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1472 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.js
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)   184585 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/debts.pdf
+-rw-r--r--   0 runner    (1001) docker     (122)     5234 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/output-checkbox.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     5624 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/table-addendum.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     5196 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     4948 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx
+-rw-r--r--   0 runner    (1001) docker     (122)     2235 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/display_template.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12200 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/misc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/save_input_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6812 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_al_income.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1312 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_altoolbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/docassemble/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 15:59:37.570706 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-04-25 15:59:37.000000 docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      394 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-25 15:59:37.578706 docassemble.ALToolbox-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-04-25 15:59:27.000000 docassemble.ALToolbox-0.8.0/setup.py
```

### Comparing `docassemble.ALToolbox-0.7.1/LICENSE` & `docassemble.ALToolbox-0.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 AssemblyLine
+Copyright (c) 2023 AssemblyLine
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `docassemble.ALToolbox-0.7.1/PKG-INFO` & `docassemble.ALToolbox-0.8.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: docassemble.ALToolbox
-Version: 0.7.1
+Version: 0.8.0
 Summary: Collection of small utility functions, classes, and web components for Docassemble interviews
 Home-page: https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox
 Author: AssemblyLine
 Author-email: 52798256+plocket@users.noreply.github.com
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALToolbox
 
+[![PyPI version](https://badge.fury.io/py/docassemble-ALToolbox.svg)](https://badge.fury.io/py/docassemble-ALToolbox)
+
 This repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were
 built as part of the Suffolk University Law School LIT Lab's [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 They are placed here
 rather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used
 by anyone, regardless of whether they use any other code from the Document Assembly Line project.
 
 If you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.
@@ -45,15 +47,15 @@
 
 # Related repositories
 
 * https://github.com/SuffolkLitLab/docassemble-AssemblyLine
 * https://github.com/SuffolkLitLab/docassemble-ALWeaver
 * https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
 * https://github.com/SuffolkLitLab/docassemble-MassAccess
-* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction
+* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate
 * https://github.com/SuffolkLitLab/EfileProxyServer
 
-## Contributors:  
+## Contributors:
 * @plocket  
 * @nonprofittechy
 * @purplesky2016
 * @brycestevenwilley
```

### Comparing `docassemble.ALToolbox-0.7.1/README.md` & `docassemble.ALToolbox-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # ALToolbox
 
+[![PyPI version](https://badge.fury.io/py/docassemble-ALToolbox.svg)](https://badge.fury.io/py/docassemble-ALToolbox)
+
 This repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were
 built as part of the Suffolk University Law School LIT Lab's [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 They are placed here
 rather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used
 by anyone, regardless of whether they use any other code from the Document Assembly Line project.
 
-If you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.
+If you want to add a small function to this project, consider adding it to the existing misc.py to avoid creating too many module files.
 
 ## Documentation
 
 Read the [documentation for the functions and components](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox) to learn
 how to use these components in your own [Docassemble](https://github.com/jhpyle/docassemble) projects.
 
 ## Suffolk LIT Lab Document Assembly Line
 
-<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>
+<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing of people working together on a website UI" width="300" style="align: center;"/>
 
 The Assembly Line Project is a collection of volunteers, students, and institutions who joined together
 during the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,
 easy to use **guided** online forms that help empower litigants to access the court remotely.
 
 Our signature project is [CourtFormsOnline.org](https://courtformsonline.org).
 
@@ -28,21 +30,21 @@
 
 This package contains **runtime code** and **pre-written questions** to support authoring robust, 
 consistent, and attractive Docassemble interviews that help complete court forms.
 
 Read more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 
 
-# Related repositories
+## Related repositories
 
 * https://github.com/SuffolkLitLab/docassemble-AssemblyLine
 * https://github.com/SuffolkLitLab/docassemble-ALWeaver
 * https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
 * https://github.com/SuffolkLitLab/docassemble-MassAccess
-* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction
+* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate
 * https://github.com/SuffolkLitLab/EfileProxyServer
 
-## Contributors:  
+## Contributors:
 * @plocket  
 * @nonprofittechy
 * @purplesky2016
 * @brycestevenwilley
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/Addup.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/Addup.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/PhoneNumberDataType.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/PhoneNumberDataType.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/addenda.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/addenda.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/al_income.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/al_income.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/business_days.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/business_days.py`

 * *Files 21% similar despite different names*

```diff
@@ -153,18 +153,23 @@
     date: Union[str, DADateTime],
     country="US",
     subdiv="MA",
     add_holidays: Optional[Mapping] = None,
     remove_holidays: Optional[Iterable[str]] = None,
 ) -> bool:
     """
-    Returns true iff the specified date is a business day (i.e., not a holiday)
+    Returns true if and only if the specified date is a business day (i.e., not a holiday)
     in the specified jurisdiction. Business days are considered to be:
     1. weekdays other than Saturday and Sunday and
     1. days that are not a federal or state-observed holiday
+
+    Example:
+    ```
+    assert(is_business_day("2023-03-26") == False)
+    ```
     """
     if not isinstance(date, DADateTime):
         date = as_datetime(date)
     if date.dow in [
         6,
         7,
     ]:  # Docassemble codes Saturday and Sunday as 6 and 7 respectively
@@ -192,15 +197,27 @@
     Returns the first day AFTER the specified start date that is
     not a federal or state holiday, Saturday or Sunday. Optionally,
     specify the parameter `wait_n_days` to get the first business day after
     at least, e.g., 10 days.
 
     Relies on the Python holidays package, which has fairly good support for
     holidays around the world and in various states and provinces, but local
-    court rules may differ.
+    court rules may differ. You can see what holidays are used at
+    https://github.com/dr-prodigy/python-holidays/tree/master/holidays/countries
+
+    Args:
+      start_date: the date to start with. Can be a date-formatted string (i.e. "2023-03-37", or
+          "3-27-2023") or a DADateTime object
+      wait_n_days: the number of days to find the find the date after. If 0, it returns the given
+          date if it's a business day.
+      country: the county to use business days from
+      subdiv: the subdivision (e.g. state or province) to use business days from
+      add_holidays: a dictionary from the date string ("12/25") to the name of the holiday,
+          will add those holidays to be considered
+      remove_holidays: the list of date strings ("12/25") of dates that are no longer holidays
     """
     if not isinstance(start_date, DADateTime):
         start_date = as_datetime(start_date)
     date_to_check = start_date.plus(days=wait_n_days)
 
     while not is_business_day(
         date_to_check,
@@ -219,14 +236,25 @@
     country="US",
     subdiv="MA",
     add_holidays: Optional[Mapping] = None,
     remove_holidays: Optional[Iterable[str]] = None,
 ) -> DADateTime:
     """
     Returns a time period which contains a minimum of `n` business days.
+
+    Args:
+      start_date: the date to start with. Can be a date-formatted string (i.e. "2023-03-37", or
+          "3-27-2023") or a DADateTime object
+      wait_n_days: the number of businesses days to wait for. For example, `start_date` is a
+          Friday, and `wait_n_days` is 2, then the date returned will be the next Tuesday.
+      country: the county to use business days from
+      subdiv: the subdivision (e.g. state or province) to use business days from
+      add_holidays: a dictionary from the date string ("12/25") to the name of the holiday,
+          will add those holidays to be considered
+      remove_holidays: the list of date strings ("12/25") of dates that are no longer holidays
     """
     if not isinstance(start_date, DADateTime):
         start_date = as_datetime(start_date)
     date_to_check = start_date
 
     for _ in range(wait_n_days):
         date_to_check = date_to_check.plus(days=1)
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/copy_button.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/copy_button.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,25 @@
     tooltip_inert_text: str = "Copy to clipboard",
     tooltip_copied_text: str = "Copied!",
     copy_template_block: bool = False,
     scroll_class: str = "",
     style_class: str = "",
     adjust_height: str = "",
 ) -> str:
-    """Return the html for a button that will let a user copy the given text"""
+    """Return the html for a button that will let a user copy the given text
+
+    To use, include `docassemble.ALToolbox:copy_button.yml` in your DA interview.
+
+    Args:
+      text_to_copy: text you want the user to be able to copy.
+      text_before: the prompt that will appear to the left of the HTML input
+      label: the label of the Button
+      tooltip_inert_text: text shown when the button is hovered over, before it's clicked
+      tooltip_copied_text: text shown when the button is hovered over, after the text is placed on the clipboard
+    """
 
     button_str = '<div class="al_copy">\n'
     if text_before != "":
         button_str += (
             f'<span class="al_copy_description">{word( text_before )}</span>\n'
         )
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Addup.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Addup.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Bells and whistles.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Bells and whistles.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Profiling.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Profiling.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/Shorten a url.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/Shorten a url.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/TextCounter.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/TextCounter.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_docx_text_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_pdf_text_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/addenda_for_table_ records_overflow.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/al_income.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/al_income_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/al_income_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/altoolbox_overview.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/altoolbox_overview.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/business_days_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/business_days_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/collapse_template_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/collapse_template_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/copy_button_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/copy_button_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/display_template_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/display_template_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/escape_button_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/escape_button_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/multiselect.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/multiselect.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 ---
 features:
   css: bootstrap-multiselect.css
   javascript: bootstrap-multiselect.js
 ---
+imports:
+  - base64
+---
 comment: |
   This feature requires JavaScript on the multiselect that you want to 
   transform into a filterable dropdown. 
   
   Apply the .multiselect() function to the input, with any desired parameters.
   Note you will need to use the base64-encoded version of the input's name because
   of the way Docassemble transforms input names.
   
   Example:  
   
   script: |
     <script type="text/javascript">
         $(document).ready(function() {
-            $('#bXNlbGVjdA').multiselect({enableCaseInsensitiveFiltering: true, inheritClass: true});
+            $("#${ base64.b64encode("input_name") }").multiselect({enableCaseInsensitiveFiltering: true, inheritClass: true});
         });
     </script>
     
     
   Additional documentation: 
   
   https://davidstutz.github.io/bootstrap-multiselect/
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/nice_county_name_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/output_checkbox_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/phone-number-validation.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone-number-validation.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/review_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/review_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/questions/save_input_data_demo.yml` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/questions/save_input_data_demo.yml`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/TextCounter.js` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/TextCounter.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.css` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/bootstrap-multiselect.js` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/bootstrap-multiselect.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/copy_button.css` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.css`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/copy_button.js` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/copy_button.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/custom_504.html` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/custom_504.html`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/phone-number-validation.js` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/phone-number-validation.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/static/review_widget.js` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/static/review_widget.js`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/debts.pdf` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/debts.pdf`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/output-checkbox.docx` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/output-checkbox.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/table-addendum.docx` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/table-addendum.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-docx.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/data/templates/text-addendum-to-pdf.docx`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/display_template.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/display_template.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/misc.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # The following three functions are from Quinten
 def thousands(num: Union[float, str, Decimal], show_decimals=False) -> str:
     """
     Return a whole number formatted with thousands separator.
     Optionally, format with 2 decimal points (for a PDF form with the
     currency symbol already present in the form)
 
-    If `trucate`, will call `int(num)`, truncating the decimals instead of
+    If `show_decimals`, will call `int(num)`, truncating the decimals instead of
     rounding to the closest int.
     """
     try:
         if show_decimals:
             return f"{num:,.2f}"
         else:
             return f"{int(num):,}"
@@ -59,47 +59,66 @@
 
 def tel(phone_number) -> str:
     """Format a phone number so you can click on it to open in your phone dialer"""
     return '<a href="tel:' + str(phone_number) + '">' + str(phone_number) + "</a>"
 
 
 def fa_icon(
-    icon: str, color="primary", color_css=None, size="sm", fa_class="fa-solid"
+    icon: str,
+    color: Optional[str] = "primary",
+    color_css: Optional[str] = None,
+    size: Optional[str] = "sm",
+    fa_class: str = "fa-solid",
 ) -> str:
-    """
-    Return HTML for a font-awesome icon of the specified size and color. You can reference
-    a CSS variable (such as Bootstrap theme color) or a true CSS color reference, such as 'blue' or
-    '#DDDDDD'. Defaults to Bootstrap theme color "primary".
+    """Display a fontawesome icon inline.
+
+    Docassemble allows you to display an icon from [fontawesome](https://fontawesome.com),
+    but it does not provide control over the size or color of the icon. This function gives
+    you more control over the icon that is inserted.
+
+    Args:
+      icon: a string representing a fontawesome icon. The icon needs to be in the
+        [free library](https://fontawesome.com/search?o=r&m=free).
+      color: can be any [Bootstrap color variable](https://getbootstrapc.mo/docs/4.0/utilities/colors).
+        For example: `primary`, `secondary`, `warning`
+      color_css: allows you to use a CSS code to represent the color, e.g., `blue`, or `#fff` for black
+      size: used to control the [fontawesome size](https://fontawesome.com/v6.0/docs/web/style/size)
+        (without the `fa-` prefix). Valid values include `2xs`, `xs`, the default of `sm`,
+        `md`, `lg`, `xl`, `2x1`, and the python `None`, which defaults to `md`.
+      fa_class: let's you specify the fontawesome class, needed for any icon that isn't
+        the default class of `fa-solid`, like `fa-brands`, or `fa-regular` and `fa-light`.
 
-    Sizes can be '2xs', 'xs', 'sm', 'md' (or None), 'lg', 'xl', '2xl'.
+    Returns:
+      HTML for a font-awesome icon of the specified size and color.
     """
     if not size or size == "md":
         size_str = ""
     else:
         size_str = " fa-" + size
     if not size and not color and not color_css:
         return ":" + icon + ":"  # Default to letting Docassemble handle it
-    elif color_css:
+    if color_css:
         return (
             f'<i class="{fa_class} fa-'
             + icon
             + size_str
             + '" style="color:'
             + color_css
             + ';"></i>'
         )
-    else:
+    if color:
         return (
             f'<i class="{fa_class} fa-'
             + icon
             + size_str
             + '" style="color:var(--'
             + color
             + ');"></i>'
         )
+    return f'<i class="{fa_class} fa-{icon}{size_str}"></i>'
 
 
 def space(var_name: str, prefix=" ", suffix="") -> str:
     """If the value as a string is defined, return it prefixed/suffixed. Defaults to prefix
     of a space. Helps build a sentence with less cruft. Equivalent to SPACE function in
     HotDocs."""
     if (
@@ -147,16 +166,16 @@
     open_icon="caret-down",
 ):
     """
     Insert HTML for a Bootstrap "collapse" div.
 
     Optionally, you can specify a custom icon to override the defaults:
 
-    The default icons are "🞂" which displays when the text is collapsed (`closed_icon`) and
-    "▼" which displays when the text is open (`open_icon`).
+    The default icons are "right caret" which displays when the text is collapsed (`closed_icon`) and
+    "down caret" which displays when the text is open (`open_icon`).
     """
     if not template.subject_as_html(trim=True) and not template.content_as_html():
         return ""
     if classname is None:
         classname = " bg-light"
     else:
         classname = " " + classname.strip()
@@ -200,37 +219,39 @@
 
 def review_widget(
     *,
     up_action: str,
     down_action: str,
     review_action: Optional[str] = None,
     thumbs_display: str = "Did we help you?",
-    review_display: str = "Thanks! Let us know what we could do better",
+    review_display: str = "Thank you for your feedback. Let us know what we could do better",
     submit_review_button: str = "Add your review",
     post_review_display: str = "Thank you for your review!",
 ) -> str:
     """
     A widget that allows people to give a quick review (thumbs up and down, with an optional text
     component) in the middle of an interview without triggering a page reload.
 
     If `review_action` is provided, once you press either of the thumbs, a text input screen with
     a submit button appears, and once the text review is submitted (or after the thumbs, if no
-    `review_action` was provided), a final "thank you" messsage is displayed.
+    `review_action` was provided), a final "thank you" message is displayed.
 
-    @param up_action {string} - the variable name of an event to be executed on the server if the
-        thumbs up is pressed
-    @param down_action {string} - the variable name of an event to be executed on the server i
-        the thumbs down is pressed
-    @param (optional) review_action {string} - the variable name of an event to be execute on the
-        server when someone submits their text review
-    @param (optional) thumbs_display {string} - text displayed to user describing the thumbs
-    @param (optional) review_display {string} - text displayed to user describing the text input
-    @param (optional) submit_review_button {string} - text on the button to submit their text review
-    @param (optional) post_review_display {string} - text displayed to user after review is
-        submitted
+    Args:
+        up_action: the variable name of an event to be executed on the server if the
+            thumbs up is pressed
+        down_action: the variable name of an event to be executed on the server if the
+            thumbs down is pressed
+        review_action: the variable name of an event to be execute on the
+            server when someone submits their text review
+        thumbs_display: text displayed to user describing the thumbs
+        review_display: text displayed to user describing the text input
+        submit_review_button: text on the button to submit their text review
+        post_review_display: text displayed to user after review is submitted
+    Returns:
+        the HTML string of the widget
     """
     js_thumbs_up = f"javascript:altoolbox_thumbs_up_send('{up_action}', {'true' if review_action else 'false'})"
     js_thumbs_down = f"javascript:altoolbox_thumbs_down_send('{down_action}', {'true' if review_action else 'false'})"
     widget = f"""
 <div class="card" style="width: 20rem;">
   <div class="card-body">
     <p class="al-thumbs-widget">{word(thumbs_display)}</p>
@@ -278,15 +299,22 @@
         index += 1
     return obj
 
 
 def output_checkbox(
     value_to_check: bool, checked_value: str = "[X]", unchecked_value: str = "[  ]"
 ):
-    """Generate a conditional checkbox for docx templates"""
+    """Generate a conditional checkbox for docx templates
+
+    Args:
+      checked_value: defaults to `[X]` but can be set to any string or even a `DAFile` or `DAStaticFile`
+          with the image of a checkbox
+      unchecked_value: opposite meaning of `checked_value` and defaults to `[  ]`
+
+    """
     if value_to_check:
         return checked_value
     else:
         return unchecked_value
 
 
 def nice_county_name(address: Address) -> str:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/save_input_data.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/save_input_data.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/test_al_income.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_al_income.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble/ALToolbox/test_altoolbox.py` & `docassemble.ALToolbox-0.8.0/docassemble/ALToolbox/test_altoolbox.py`

 * *Files identical despite different names*

### Comparing `docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/PKG-INFO` & `docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: docassemble.ALToolbox
-Version: 0.7.1
+Version: 0.8.0
 Summary: Collection of small utility functions, classes, and web components for Docassemble interviews
 Home-page: https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox
 Author: AssemblyLine
 Author-email: 52798256+plocket@users.noreply.github.com
 License: The MIT License (MIT)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ALToolbox
 
+[![PyPI version](https://badge.fury.io/py/docassemble-ALToolbox.svg)](https://badge.fury.io/py/docassemble-ALToolbox)
+
 This repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were
 built as part of the Suffolk University Law School LIT Lab's [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).
 They are placed here
 rather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used
 by anyone, regardless of whether they use any other code from the Document Assembly Line project.
 
 If you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.
@@ -45,15 +47,15 @@
 
 # Related repositories
 
 * https://github.com/SuffolkLitLab/docassemble-AssemblyLine
 * https://github.com/SuffolkLitLab/docassemble-ALWeaver
 * https://github.com/SuffolkLitLab/docassemble-ALMassachusetts
 * https://github.com/SuffolkLitLab/docassemble-MassAccess
-* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction
+* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate
 * https://github.com/SuffolkLitLab/EfileProxyServer
 
-## Contributors:  
+## Contributors:
 * @plocket  
 * @nonprofittechy
 * @purplesky2016
 * @brycestevenwilley
```

### Comparing `docassemble.ALToolbox-0.7.1/docassemble.ALToolbox.egg-info/SOURCES.txt` & `docassemble.ALToolbox-0.8.0/docassemble.ALToolbox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -45,24 +45,27 @@
 docassemble/ALToolbox/data/questions/copy_button.yml
 docassemble/ALToolbox/data/questions/copy_button_demo.yml
 docassemble/ALToolbox/data/questions/display_template.yml
 docassemble/ALToolbox/data/questions/display_template_demo.yml
 docassemble/ALToolbox/data/questions/escape_button.yml
 docassemble/ALToolbox/data/questions/escape_button_demo.yml
 docassemble/ALToolbox/data/questions/multiselect.yml
+docassemble/ALToolbox/data/questions/multiselect_demo.yml
 docassemble/ALToolbox/data/questions/nice_county_name_demo.yml
 docassemble/ALToolbox/data/questions/output_checkbox_demo.yml
 docassemble/ALToolbox/data/questions/phone-number-validation.yml
 docassemble/ALToolbox/data/questions/phone_number_validation_demo.yml
 docassemble/ALToolbox/data/questions/review_demo.yml
 docassemble/ALToolbox/data/questions/review_widget.yml
 docassemble/ALToolbox/data/questions/save_input_data_demo.yml
+docassemble/ALToolbox/data/questions/three_parts_date_demo.yml
 docassemble/ALToolbox/data/sources/README.md
 docassemble/ALToolbox/data/static/README.md
 docassemble/ALToolbox/data/static/TextCounter.js
+docassemble/ALToolbox/data/static/al_three_parts_date.css
 docassemble/ALToolbox/data/static/bootstrap-multiselect.css
 docassemble/ALToolbox/data/static/bootstrap-multiselect.js
 docassemble/ALToolbox/data/static/collapse_template.css
 docassemble/ALToolbox/data/static/copy_button.css
 docassemble/ALToolbox/data/static/copy_button.js
 docassemble/ALToolbox/data/static/custom_504.html
 docassemble/ALToolbox/data/static/display_template.css
```

### Comparing `docassemble.ALToolbox-0.7.1/setup.py` & `docassemble.ALToolbox-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,17 +40,17 @@
                         break
                 if bad_name:
                     continue
                 out.setdefault(package, []).append(prefix+name)
     return out
 
 setup(name='docassemble.ALToolbox',
-      version='0.7.1',
+      version='0.8.0',
       description=('Collection of small utility functions, classes, and web components for Docassemble interviews'),
-      long_description='# ALToolbox\r\n\r\nThis repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were\r\nbuilt as part of the Suffolk University Law School LIT Lab\'s [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\nThey are placed here\r\nrather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used\r\nby anyone, regardless of whether they use any other code from the Document Assembly Line project.\r\n\r\nIf you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.\r\n\r\n## Documentation\r\n\r\nRead the [documentation for the functions and components](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox) to learn\r\nhow to use these components in your own [Docassemble](https://github.com/jhpyle/docassemble) projects.\r\n\r\n## Suffolk LIT Lab Document Assembly Line\r\n\r\n<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>\r\n\r\nThe Assembly Line Project is a collection of volunteers, students, and institutions who joined together\r\nduring the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,\r\neasy to use **guided** online forms that help empower litigants to access the court remotely.\r\n\r\nOur signature project is [CourtFormsOnline.org](https://courtformsonline.org).\r\n\r\nWe designed a step-by-step, assembly line style process for automating court forms on top of Docassemble\r\nand built several tools along the way that **you** can use in your home jurisdiction.\r\n\r\nThis package contains **runtime code** and **pre-written questions** to support authoring robust, \r\nconsistent, and attractive Docassemble interviews that help complete court forms.\r\n\r\nRead more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\n\r\n\r\n# Related repositories\r\n\r\n* https://github.com/SuffolkLitLab/docassemble-AssemblyLine\r\n* https://github.com/SuffolkLitLab/docassemble-ALWeaver\r\n* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts\r\n* https://github.com/SuffolkLitLab/docassemble-MassAccess\r\n* https://github.com/SuffolkLitLab/docassemble-ALGenericJurisdiction\r\n* https://github.com/SuffolkLitLab/EfileProxyServer\r\n\r\n## Contributors:  \r\n* @plocket  \r\n* @nonprofittechy\r\n* @purplesky2016\r\n* @brycestevenwilley\r\n',
+      long_description='# ALToolbox\r\n\r\n[![PyPI version](https://badge.fury.io/py/docassemble-ALToolbox.svg)](https://badge.fury.io/py/docassemble-ALToolbox)\r\n\r\nThis repository is used to host small Python modules, widgets, and JavaScript web components js files that enhance Docassemble interviews. These modules were\r\nbuilt as part of the Suffolk University Law School LIT Lab\'s [Document Assembly Line project](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\nThey are placed here\r\nrather than in https://github.com/SuffolkLitLab/docassemble-AssemblyLine because we believe these small components can easily be used\r\nby anyone, regardless of whether they use any other code from the Document Assembly Line project.\r\n\r\nIf you want to add a small fuction to this project, consider adding it to the existing misc.py to avoid creating too many module files.\r\n\r\n## Documentation\r\n\r\nRead the [documentation for the functions and components](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox) to learn\r\nhow to use these components in your own [Docassemble](https://github.com/jhpyle/docassemble) projects.\r\n\r\n## Suffolk LIT Lab Document Assembly Line\r\n\r\n<img src="https://user-images.githubusercontent.com/7645641/142245862-c2eb02ab-3090-4e97-9653-bb700bf4c54d.png" alt="drawing" width="300" alt="work together" style="align: center;"/>\r\n\r\nThe Assembly Line Project is a collection of volunteers, students, and institutions who joined together\r\nduring the COVID-19 pandemic to help increase access to the court system. Our vision is mobile-friendly,\r\neasy to use **guided** online forms that help empower litigants to access the court remotely.\r\n\r\nOur signature project is [CourtFormsOnline.org](https://courtformsonline.org).\r\n\r\nWe designed a step-by-step, assembly line style process for automating court forms on top of Docassemble\r\nand built several tools along the way that **you** can use in your home jurisdiction.\r\n\r\nThis package contains **runtime code** and **pre-written questions** to support authoring robust, \r\nconsistent, and attractive Docassemble interviews that help complete court forms.\r\n\r\nRead more on our [documentation page](https://suffolklitlab.org/docassemble-AssemblyLine-documentation/).\r\n\r\n\r\n# Related repositories\r\n\r\n* https://github.com/SuffolkLitLab/docassemble-AssemblyLine\r\n* https://github.com/SuffolkLitLab/docassemble-ALWeaver\r\n* https://github.com/SuffolkLitLab/docassemble-ALMassachusetts\r\n* https://github.com/SuffolkLitLab/docassemble-MassAccess\r\n* https://github.com/SuffolkLitLab/docassemble-ALThemeTemplate\r\n* https://github.com/SuffolkLitLab/EfileProxyServer\r\n\r\n## Contributors:\r\n* @plocket  \r\n* @nonprofittechy\r\n* @purplesky2016\r\n* @brycestevenwilley\r\n',
       long_description_content_type='text/markdown',
       author='AssemblyLine',
       author_email='52798256+plocket@users.noreply.github.com',
       license='The MIT License (MIT)',
       url='https://suffolklitlab.org/docassemble-AssemblyLine-documentation/docs/framework/altoolbox',
       packages=find_packages(),
       namespace_packages=['docassemble'],
```

