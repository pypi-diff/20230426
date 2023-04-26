# Comparing `tmp/govuk_frontend_django-0.2.0.tar.gz` & `tmp/govuk_frontend_django-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "govuk_frontend_django-0.2.0.tar", max compression
+gzip compressed data, was "govuk_frontend_django-0.3.0.tar", max compression
```

## Comparing `govuk_frontend_django-0.2.0.tar` & `govuk_frontend_django-0.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.2.0/LICENSE
--rw-r--r--   0        0        0     1017 2023-04-20 16:48:35.945315 govuk_frontend_django-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.2.0/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.2.0/govuk_frontend_django/components/__init__.py
--rw-r--r--   0        0        0     1252 2023-04-26 11:56:54.154039 govuk_frontend_django-0.2.0/govuk_frontend_django/components/accordion.py
--rw-r--r--   0        0        0      939 2023-04-21 17:53:53.640544 govuk_frontend_django-0.2.0/govuk_frontend_django/components/back_link.py
--rw-r--r--   0        0        0     4249 2023-04-26 11:55:41.152480 govuk_frontend_django-0.2.0/govuk_frontend_django/components/base.py
--rw-r--r--   0        0        0     1170 2023-04-21 17:53:53.647358 govuk_frontend_django-0.2.0/govuk_frontend_django/components/breadcrumbs.py
--rw-r--r--   0        0        0     1192 2023-04-26 11:56:54.154983 govuk_frontend_django-0.2.0/govuk_frontend_django/components/button.py
--rw-r--r--   0        0        0     1743 2023-04-26 11:56:54.154458 govuk_frontend_django-0.2.0/govuk_frontend_django/components/character_count.py
--rw-r--r--   0        0        0     1892 2023-04-26 11:22:44.437285 govuk_frontend_django-0.2.0/govuk_frontend_django/components/checkboxes.py
--rw-r--r--   0        0        0     1723 2023-04-21 17:53:53.661217 govuk_frontend_django-0.2.0/govuk_frontend_django/components/cookie_banner.py
--rw-r--r--   0        0        0     1598 2023-04-21 17:53:53.655825 govuk_frontend_django-0.2.0/govuk_frontend_django/components/date_input.py
--rw-r--r--   0        0        0     1053 2023-04-21 17:53:53.652778 govuk_frontend_django-0.2.0/govuk_frontend_django/components/details.py
--rw-r--r--   0        0        0     1023 2023-04-21 17:53:53.655383 govuk_frontend_django-0.2.0/govuk_frontend_django/components/error_message.py
--rw-r--r--   0        0        0     1349 2023-04-21 17:53:53.658748 govuk_frontend_django-0.2.0/govuk_frontend_django/components/error_summary.py
--rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.657118 govuk_frontend_django-0.2.0/govuk_frontend_django/components/fieldset.py
--rw-r--r--   0        0        0     1215 2023-04-26 11:56:54.154662 govuk_frontend_django-0.2.0/govuk_frontend_django/components/file_upload.py
--rw-r--r--   0        0        0     2007 2023-04-21 17:53:53.671128 govuk_frontend_django-0.2.0/govuk_frontend_django/components/footer.py
--rw-r--r--   0        0        0     1552 2023-04-21 17:53:53.664873 govuk_frontend_django-0.2.0/govuk_frontend_django/components/header.py
--rw-r--r--   0        0        0      927 2023-04-21 17:53:53.661696 govuk_frontend_django-0.2.0/govuk_frontend_django/components/hint.py
--rw-r--r--   0        0        0     1854 2023-04-26 11:56:54.154769 govuk_frontend_django-0.2.0/govuk_frontend_django/components/input.py
--rw-r--r--   0        0        0      960 2023-04-21 17:53:53.665398 govuk_frontend_django-0.2.0/govuk_frontend_django/components/inset_text.py
--rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.666367 govuk_frontend_django-0.2.0/govuk_frontend_django/components/label.py
--rw-r--r--   0        0        0     1241 2023-04-21 17:53:53.667052 govuk_frontend_django-0.2.0/govuk_frontend_django/components/notification_banner.py
--rw-r--r--   0        0        0     1729 2023-04-21 17:53:53.670872 govuk_frontend_django-0.2.0/govuk_frontend_django/components/pagination.py
--rw-r--r--   0        0        0     1015 2023-04-21 17:53:53.675594 govuk_frontend_django-0.2.0/govuk_frontend_django/components/panel.py
--rw-r--r--   0        0        0      980 2023-04-21 17:53:53.668688 govuk_frontend_django-0.2.0/govuk_frontend_django/components/phase_banner.py
--rw-r--r--   0        0        0     1753 2023-04-21 17:53:53.677427 govuk_frontend_django-0.2.0/govuk_frontend_django/components/radios.py
--rw-r--r--   0        0        0     1468 2023-04-26 11:56:54.154899 govuk_frontend_django-0.2.0/govuk_frontend_django/components/select.py
--rw-r--r--   0        0        0      956 2023-04-21 17:53:53.671708 govuk_frontend_django-0.2.0/govuk_frontend_django/components/skip_link.py
--rw-r--r--   0        0        0     1850 2023-04-21 17:53:53.679515 govuk_frontend_django-0.2.0/govuk_frontend_django/components/summary_list.py
--rw-r--r--   0        0        0     1653 2023-04-21 17:53:53.681216 govuk_frontend_django-0.2.0/govuk_frontend_django/components/table.py
--rw-r--r--   0        0        0     1171 2023-04-21 17:53:53.675164 govuk_frontend_django-0.2.0/govuk_frontend_django/components/tabs.py
--rw-r--r--   0        0        0      892 2023-04-21 17:53:53.675735 govuk_frontend_django-0.2.0/govuk_frontend_django/components/tag.py
--rw-r--r--   0        0        0     1308 2023-04-26 11:56:54.154218 govuk_frontend_django-0.2.0/govuk_frontend_django/components/textarea.py
--rw-r--r--   0        0        0      969 2023-04-26 11:56:54.155051 govuk_frontend_django-0.2.0/govuk_frontend_django/components/warning_text.py
--rw-r--r--   0        0        0     2583 2023-04-24 16:19:58.566629 govuk_frontend_django-0.2.0/govuk_frontend_django/templates/govuk_frontend_django/base.html
--rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/__init__.py
--rw-r--r--   0        0        0    13974 2023-04-26 11:55:41.159321 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
--rw-r--r--   0        0        0     1518 2023-04-26 11:55:41.160076 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
--rw-r--r--   0        0        0     1207 2023-04-26 11:55:41.160364 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
--rw-r--r--   0        0        0     3291 2023-04-26 11:55:41.160730 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
--rw-r--r--   0        0        0     2198 2023-04-26 11:55:41.161234 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
--rw-r--r--   0        0        0     1532 2023-04-26 11:55:41.162116 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
--rw-r--r--   0        0        0     5243 2023-04-26 11:55:41.162430 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
--rw-r--r--   0        0        0     1600 2023-04-26 11:55:41.162691 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
--rw-r--r--   0        0        0     2209 2023-04-26 11:55:41.162946 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
--rw-r--r--   0        0        0     1388 2023-04-26 11:55:41.163196 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
--rw-r--r--   0        0        0     7121 2023-04-26 11:55:41.163497 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
--rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
--rw-r--r--   0        0        0     1286 2023-04-26 11:55:41.164058 govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
--rw-r--r--   0        0        0     1367 2023-04-26 11:58:25.180503 govuk_frontend_django-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 govuk_frontend_django-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 16:00:56.529873 govuk_frontend_django-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1346 2023-04-26 12:03:56.841463 govuk_frontend_django-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.556313 govuk_frontend_django-0.3.0/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.561863 govuk_frontend_django-0.3.0/govuk_frontend_django/components/__init__.py
+-rw-r--r--   0        0        0     1296 2023-04-26 12:03:22.552736 govuk_frontend_django-0.3.0/govuk_frontend_django/components/accordion.py
+-rw-r--r--   0        0        0      939 2023-04-21 17:53:53.640544 govuk_frontend_django-0.3.0/govuk_frontend_django/components/back_link.py
+-rw-r--r--   0        0        0     4249 2023-04-26 11:55:41.152480 govuk_frontend_django-0.3.0/govuk_frontend_django/components/base.py
+-rw-r--r--   0        0        0     1170 2023-04-21 17:53:53.647358 govuk_frontend_django-0.3.0/govuk_frontend_django/components/breadcrumbs.py
+-rw-r--r--   0        0        0     1221 2023-04-26 12:03:22.554265 govuk_frontend_django-0.3.0/govuk_frontend_django/components/button.py
+-rw-r--r--   0        0        0     1838 2023-04-26 12:03:22.552820 govuk_frontend_django-0.3.0/govuk_frontend_django/components/character_count.py
+-rw-r--r--   0        0        0     1892 2023-04-26 11:22:44.437285 govuk_frontend_django-0.3.0/govuk_frontend_django/components/checkboxes.py
+-rw-r--r--   0        0        0     1723 2023-04-21 17:53:53.661217 govuk_frontend_django-0.3.0/govuk_frontend_django/components/cookie_banner.py
+-rw-r--r--   0        0        0     1598 2023-04-21 17:53:53.655825 govuk_frontend_django-0.3.0/govuk_frontend_django/components/date_input.py
+-rw-r--r--   0        0        0     1053 2023-04-21 17:53:53.652778 govuk_frontend_django-0.3.0/govuk_frontend_django/components/details.py
+-rw-r--r--   0        0        0     1023 2023-04-21 17:53:53.655383 govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_message.py
+-rw-r--r--   0        0        0     1349 2023-04-21 17:53:53.658748 govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_summary.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.657118 govuk_frontend_django-0.3.0/govuk_frontend_django/components/fieldset.py
+-rw-r--r--   0        0        0     1251 2023-04-26 12:03:22.554327 govuk_frontend_django-0.3.0/govuk_frontend_django/components/file_upload.py
+-rw-r--r--   0        0        0     2007 2023-04-21 17:53:53.671128 govuk_frontend_django-0.3.0/govuk_frontend_django/components/footer.py
+-rw-r--r--   0        0        0     1552 2023-04-21 17:53:53.664873 govuk_frontend_django-0.3.0/govuk_frontend_django/components/header.py
+-rw-r--r--   0        0        0      927 2023-04-21 17:53:53.661696 govuk_frontend_django-0.3.0/govuk_frontend_django/components/hint.py
+-rw-r--r--   0        0        0     1890 2023-04-26 12:03:22.554386 govuk_frontend_django-0.3.0/govuk_frontend_django/components/input.py
+-rw-r--r--   0        0        0      960 2023-04-21 17:53:53.665398 govuk_frontend_django-0.3.0/govuk_frontend_django/components/inset_text.py
+-rw-r--r--   0        0        0     1024 2023-04-21 17:53:53.666367 govuk_frontend_django-0.3.0/govuk_frontend_django/components/label.py
+-rw-r--r--   0        0        0     1241 2023-04-21 17:53:53.667052 govuk_frontend_django-0.3.0/govuk_frontend_django/components/notification_banner.py
+-rw-r--r--   0        0        0     1729 2023-04-21 17:53:53.670872 govuk_frontend_django-0.3.0/govuk_frontend_django/components/pagination.py
+-rw-r--r--   0        0        0     1015 2023-04-21 17:53:53.675594 govuk_frontend_django-0.3.0/govuk_frontend_django/components/panel.py
+-rw-r--r--   0        0        0      980 2023-04-21 17:53:53.668688 govuk_frontend_django-0.3.0/govuk_frontend_django/components/phase_banner.py
+-rw-r--r--   0        0        0     1753 2023-04-21 17:53:53.677427 govuk_frontend_django-0.3.0/govuk_frontend_django/components/radios.py
+-rw-r--r--   0        0        0     1504 2023-04-26 12:03:22.554441 govuk_frontend_django-0.3.0/govuk_frontend_django/components/select.py
+-rw-r--r--   0        0        0      956 2023-04-21 17:53:53.671708 govuk_frontend_django-0.3.0/govuk_frontend_django/components/skip_link.py
+-rw-r--r--   0        0        0     1850 2023-04-21 17:53:53.679515 govuk_frontend_django-0.3.0/govuk_frontend_django/components/summary_list.py
+-rw-r--r--   0        0        0     1653 2023-04-21 17:53:53.681216 govuk_frontend_django-0.3.0/govuk_frontend_django/components/table.py
+-rw-r--r--   0        0        0     1171 2023-04-21 17:53:53.675164 govuk_frontend_django-0.3.0/govuk_frontend_django/components/tabs.py
+-rw-r--r--   0        0        0      892 2023-04-21 17:53:53.675735 govuk_frontend_django-0.3.0/govuk_frontend_django/components/tag.py
+-rw-r--r--   0        0        0     1344 2023-04-26 12:03:22.554550 govuk_frontend_django-0.3.0/govuk_frontend_django/components/textarea.py
+-rw-r--r--   0        0        0      986 2023-04-26 12:03:22.554676 govuk_frontend_django-0.3.0/govuk_frontend_django/components/warning_text.py
+-rw-r--r--   0        0        0     2583 2023-04-24 16:19:58.566629 govuk_frontend_django-0.3.0/govuk_frontend_django/templates/govuk_frontend_django/base.html
+-rw-r--r--   0        0        0        0 2023-04-18 16:00:56.543579 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/__init__.py
+-rw-r--r--   0        0        0    13974 2023-04-26 11:55:41.159321 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py
+-rw-r--r--   0        0        0     1518 2023-04-26 11:55:41.160076 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py
+-rw-r--r--   0        0        0     1207 2023-04-26 11:55:41.160364 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py
+-rw-r--r--   0        0        0     3291 2023-04-26 11:55:41.160730 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py
+-rw-r--r--   0        0        0     2198 2023-04-26 11:55:41.161234 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py
+-rw-r--r--   0        0        0     1532 2023-04-26 11:55:41.162116 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py
+-rw-r--r--   0        0        0     5243 2023-04-26 11:55:41.162430 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py
+-rw-r--r--   0        0        0     1600 2023-04-26 11:55:41.162691 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py
+-rw-r--r--   0        0        0     2209 2023-04-26 11:55:41.162946 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py
+-rw-r--r--   0        0        0     1388 2023-04-26 11:55:41.163196 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py
+-rw-r--r--   0        0        0     7121 2023-04-26 11:55:41.163497 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py
+-rw-r--r--   0        0        0     1439 2023-04-26 11:55:41.163769 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py
+-rw-r--r--   0        0        0     1286 2023-04-26 11:55:41.164058 govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py
+-rw-r--r--   0        0        0     1367 2023-04-26 12:04:03.046183 govuk_frontend_django-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 govuk_frontend_django-0.3.0/PKG-INFO
```

### Comparing `govuk_frontend_django-0.2.0/LICENSE` & `govuk_frontend_django-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/README.md` & `govuk_frontend_django-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -23,7 +23,16 @@
 In your settings file, add the app to your `INSTALLED_APPS`:
 ```python
 INSTALLED_APPS = [
     ...
     "govuk_frontend_django",
 ]
 ```
+
+## Compatibility table
+
+Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
+
+| Package Version | GOV.UK Frontend Version |
+| --------------- | ----------------------- |
+| 0.2.0           | v4.5.0                  |
+| 0.3.0           | v4.6.0                  |
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/accordion.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/accordion.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     """GOV.UK Accordion
 
     See: https://design-system.service.gov.uk/components/accordion/
     """
 
     id: str
     headingLevel: Optional[int] = None
+    rememberExpanded: Optional[bool] = None
     hideAllSectionsText: Optional[str] = None
     hideSectionText: Optional[str] = None
     hideSectionAriaLabelText: Optional[str] = None
     showAllSectionsText: Optional[str] = None
     showSectionText: Optional[str] = None
     showSectionAriaLabelText: Optional[str] = None
     items: List[govuk_frontend_base.AccordionItem]
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/back_link.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/back_link.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/base.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/base.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/breadcrumbs.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/button.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,14 @@
     name: Optional[str] = None
     type: Optional[str] = None
     value: Optional[str] = None
     disabled: Optional[bool] = None
     href: Optional[str] = None
     preventDoubleClick: Optional[bool] = None
     isStartButton: Optional[bool] = None
+    id: Optional[str] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/button/macro.html"
     _macro_name = "govukButton"
 
 
 COMPONENT = GovUKButton
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/character_count.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/character_count.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,15 +35,17 @@
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
     spellcheck: Optional[bool] = None
     countMessage: Optional[CharacterCountCountmessage] = None
     textareaDescriptionText: Optional[str] = None
     charactersUnderLimitText: Optional[Any] = None
     charactersAtLimitText: Optional[str] = None
+    charactersOverLimitText: Optional[Any] = None
     wordsUnderLimitText: Optional[Any] = None
     wordsAtLimitText: Optional[str] = None
+    wordsOverLimitText: Optional[Any] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/character-count/macro.html"
     _macro_name = "govukCharacterCount"
 
 
 COMPONENT = GovUKCharacterCount
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/checkboxes.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/cookie_banner.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/date_input.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/date_input.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/details.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/details.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/error_message.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_message.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/error_summary.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/fieldset.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/fieldset.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/file_upload.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/inset_text.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,22 @@
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class GovUKFileUpload(govuk_frontend_base.GovUKComponent):
-    """GOV.UK File Upload
+class GovUKInsetText(govuk_frontend_base.GovUKComponent):
+    """GOV.UK Inset Text
 
-    See: https://design-system.service.gov.uk/components/file-upload/
+    See: https://design-system.service.gov.uk/components/inset-text/
     """
 
-    name: str
-    id: str
-    value: Optional[str] = None
-    describedBy: Optional[str] = None
-    label: govuk_frontend_label.GovUKLabel
-    hint: Optional[govuk_frontend_hint.GovUKHint] = None
-    errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
-    formGroup: Optional[govuk_frontend_base.FormGroup] = None
+    text: Optional[str] = None
+    html: Optional[str] = None
+    id: Optional[str] = None
 
-    _jinja2_template = "govuk_frontend_jinja/components/file-upload/macro.html"
-    _macro_name = "govukFileUpload"
+    _jinja2_template = "govuk_frontend_jinja/components/inset-text/macro.html"
+    _macro_name = "govukInsetText"
 
 
-COMPONENT = GovUKFileUpload
+COMPONENT = GovUKInsetText
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/footer.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/header.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/hint.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/hint.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/input.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/input.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     """
 
     id: str
     name: str
     type: Optional[str] = None
     inputmode: Optional[str] = None
     value: Optional[str] = None
+    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: govuk_frontend_label.GovUKLabel
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     prefix: Optional[InputPrefix] = None
     suffix: Optional[InputSuffix] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/inset_text.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/skip_link.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class GovUKInsetText(govuk_frontend_base.GovUKComponent):
-    """GOV.UK Inset Text
+class GovUKSkipLink(govuk_frontend_base.GovUKComponent):
+    """GOV.UK Skip Link
 
-    See: https://design-system.service.gov.uk/components/inset-text/
+    See: https://design-system.service.gov.uk/components/skip-link/
     """
 
     text: Optional[str] = None
     html: Optional[str] = None
-    id: Optional[str] = None
+    href: Optional[str] = None
 
-    _jinja2_template = "govuk_frontend_jinja/components/inset-text/macro.html"
-    _macro_name = "govukInsetText"
+    _jinja2_template = "govuk_frontend_jinja/components/skip-link/macro.html"
+    _macro_name = "govukSkipLink"
 
 
-COMPONENT = GovUKInsetText
+COMPONENT = GovUKSkipLink
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/label.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/label.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/notification_banner.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/notification_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/pagination.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/panel.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/panel.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/phase_banner.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/radios.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/radios.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/select.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     See: https://design-system.service.gov.uk/components/select/
     """
 
     id: str
     name: str
     items: List[SelectItems]
     value: Optional[str] = None
+    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: Optional[govuk_frontend_label.GovUKLabel] = None
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/select/macro.html"
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/skip_link.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/textarea.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,31 @@
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class GovUKSkipLink(govuk_frontend_base.GovUKComponent):
-    """GOV.UK Skip Link
+class GovUKTextarea(govuk_frontend_base.GovUKComponent):
+    """GOV.UK Textarea
 
-    See: https://design-system.service.gov.uk/components/skip-link/
+    See: https://design-system.service.gov.uk/components/textarea/
     """
 
-    text: Optional[str] = None
-    html: Optional[str] = None
-    href: Optional[str] = None
+    id: str
+    name: str
+    spellcheck: Optional[bool] = None
+    rows: Optional[str] = None
+    value: Optional[str] = None
+    disabled: Optional[bool] = None
+    describedBy: Optional[str] = None
+    label: govuk_frontend_label.GovUKLabel
+    hint: Optional[govuk_frontend_hint.GovUKHint] = None
+    errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
+    formGroup: Optional[govuk_frontend_base.FormGroup] = None
+    autocomplete: Optional[str] = None
 
-    _jinja2_template = "govuk_frontend_jinja/components/skip-link/macro.html"
-    _macro_name = "govukSkipLink"
+    _jinja2_template = "govuk_frontend_jinja/components/textarea/macro.html"
+    _macro_name = "govukTextarea"
 
 
-COMPONENT = GovUKSkipLink
+COMPONENT = GovUKTextarea
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/summary_list.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/table.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/tabs.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/tag.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/tag.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/textarea.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/file_upload.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 from govuk_frontend_django.components import fieldset as govuk_frontend_fieldset
 from govuk_frontend_django.components import hint as govuk_frontend_hint
 from govuk_frontend_django.components import label as govuk_frontend_label
 from govuk_frontend_django.components import tag as govuk_frontend_tag
 
 
 @dataclass(kw_only=True)
-class GovUKTextarea(govuk_frontend_base.GovUKComponent):
-    """GOV.UK Textarea
+class GovUKFileUpload(govuk_frontend_base.GovUKComponent):
+    """GOV.UK File Upload
 
-    See: https://design-system.service.gov.uk/components/textarea/
+    See: https://design-system.service.gov.uk/components/file-upload/
     """
 
-    id: str
     name: str
-    spellcheck: Optional[bool] = None
-    rows: Optional[str] = None
+    id: str
     value: Optional[str] = None
+    disabled: Optional[bool] = None
     describedBy: Optional[str] = None
     label: govuk_frontend_label.GovUKLabel
     hint: Optional[govuk_frontend_hint.GovUKHint] = None
     errorMessage: Optional[govuk_frontend_error_message.GovUKErrorMessage] = None
     formGroup: Optional[govuk_frontend_base.FormGroup] = None
-    autocomplete: Optional[str] = None
 
-    _jinja2_template = "govuk_frontend_jinja/components/textarea/macro.html"
-    _macro_name = "govukTextarea"
+    _jinja2_template = "govuk_frontend_jinja/components/file-upload/macro.html"
+    _macro_name = "govukFileUpload"
 
 
-COMPONENT = GovUKTextarea
+COMPONENT = GovUKFileUpload
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/components/warning_text.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/components/warning_text.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,14 @@
     """GOV.UK Warning Text
 
     See: https://design-system.service.gov.uk/components/warning-text/
     """
 
     text: Optional[str] = None
     html: Optional[str] = None
-    iconFallbackText: str
+    iconFallbackText: Optional[str] = None
 
     _jinja2_template = "govuk_frontend_jinja/components/warning-text/macro.html"
     _macro_name = "govukWarningText"
 
 
 COMPONENT = GovUKWarningText
```

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templates/govuk_frontend_django/base.html` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templates/govuk_frontend_django/base.html`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/__init__.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/accordion.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/checkboxes.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/error_summary.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/footer.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/header.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/pagination.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/phase_banner.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/summary_list.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/table.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py` & `govuk_frontend_django-0.3.0/govuk_frontend_django/templatetags/govuk_frontend_django/tabs.py`

 * *Files identical despite different names*

### Comparing `govuk_frontend_django-0.2.0/pyproject.toml` & `govuk_frontend_django-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "govuk-frontend-django"
-version = "0.2.0"
+version = "0.3.0"
 description = "Django functionality to help when building a GOV.UK website."
 authors = [
     "DBT Live Service Team <live.services@digital.trade.gov.uk>",
     "Cam Lamb <cameron.lamb@digital.trade.gov.uk>",
     "Sam Dudley <samuel.dudley@digital.trade.gov.uk>",
 ]
 license = "MIT"
@@ -18,15 +18,15 @@
 documentation = "https://uktrade.github.io/govuk-frontend-django/"
 packages = [{include = "govuk_frontend_django"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Django = "^4.1.7"
 jinja2 = "^3.1.2"
-govuk-frontend-jinja = "2.5.0"
+govuk-frontend-jinja = "2.6.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pyyaml = "^6.0"
 isort = "^5.12.0"
 autoflake = "^2.0.2"
 mypy = "^1.2.0"
```

### Comparing `govuk_frontend_django-0.2.0/PKG-INFO` & `govuk_frontend_django-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: govuk-frontend-django
-Version: 0.2.0
+Version: 0.3.0
 Summary: Django functionality to help when building a GOV.UK website.
 Home-page: https://uktrade.github.io/govuk-frontend-django/
 License: MIT
 Author: DBT Live Service Team
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=4.1.7,<5.0.0)
-Requires-Dist: govuk-frontend-jinja (==2.5.0)
+Requires-Dist: govuk-frontend-jinja (==2.6.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Project-URL: Documentation, https://uktrade.github.io/govuk-frontend-django/
 Project-URL: Repository, https://github.com/uktrade/govuk-frontend-django/
 Description-Content-Type: text/markdown
 
 # GOV.UK Frontend Django
 
@@ -46,7 +46,16 @@
 ```python
 INSTALLED_APPS = [
     ...
     "govuk_frontend_django",
 ]
 ```
 
+## Compatibility table
+
+Below is a list of the versions of this package and the versions of the GOV.UK Frontend that they are compatible with.
+
+| Package Version | GOV.UK Frontend Version |
+| --------------- | ----------------------- |
+| 0.2.0           | v4.5.0                  |
+| 0.3.0           | v4.6.0                  |
+
```

