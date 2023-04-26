# Comparing `tmp/django-form-surveys-1.8.1.tar.gz` & `tmp/django-form-surveys-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-surveys-1.8.1.tar", last modified: Mon Apr 17 04:17:11 2023, max compression
+gzip compressed data, was "django-form-surveys-1.8.2.tar", last modified: Wed Apr 26 01:47:36 2023, max compression
```

## Comparing `django-form-surveys-1.8.1.tar` & `django-form-surveys-1.8.2.tar`

### file list

```diff
@@ -1,96 +1,111 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.538561 django-form-surveys-1.8.1/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.466562 django-form-surveys-1.8.1/django_form_surveys.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3478 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-17 04:17:11.000000 django-form-surveys-1.8.1/django_form_surveys.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.482561 django-form-surveys-1.8.1/djf_surveys/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-17 04:12:08.000000 django-form-surveys-1.8.1/djf_surveys/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admin.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.486561 django-form-surveys-1.8.1/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/admins/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8146 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/admins/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/app_settings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/apps.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/context_processors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/forms.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.498561 django-form-surveys-1.8.1/djf_surveys/migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0001_initial.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0002_auto_20220330_1033.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0003_auto_20220330_1036.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0004_auto_20220330_1112.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0005_auto_20220404_1518.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0006_survey_private_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0007_auto_20220525_1126.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0008_auto_20220721_0935.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0009_auto_20220803_0927.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0010_model_translation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-1.8.1/djf_surveys/migrations/0011_alter_question_key.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-1.8.1/djf_surveys/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/static/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.498561 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/css/rating.css
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.502561 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-border.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-fill.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7170 2022-12-26 04:13:44.000000 django-form-surveys-1.8.1/djf_surveys/summary.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.462562 django-form-surveys-1.8.1/djf_surveys/templates/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.502561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.510561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6956 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form_preview.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      998 2022-12-02 18:12:38.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/question_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1793 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/summary.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/survey_list.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4238 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/answer_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.514561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/add_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/delete_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/edit_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/buttons/share_button.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.526561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2022-12-02 01:19:44.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/empty_state.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/header_nav.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2386 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      774 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/pagination.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      938 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/search_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      542 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/section_welcome.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_border.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_fill.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      890 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/detail_result.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2015 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      786 2022-12-02 18:12:32.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1173 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/survey_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      291 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/datepicker.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-17 04:17:11.534561 django-form-surveys-1.8.1/djf_surveys/templatetags/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/templatetags/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/templatetags/djf_survey_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/tests.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-1.8.1/djf_surveys/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-03-15 09:08:50.000000 django-form-surveys-1.8.1/djf_surveys/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      550 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/djf_surveys/validators.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-1.8.1/djf_surveys/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-10-24 00:52:04.000000 django-form-surveys-1.8.1/djf_surveys/widgets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-17 04:17:11.538561 django-form-surveys-1.8.1/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-1.8.1/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.936463 django-form-surveys-1.8.2/django_form_surveys.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/top_level.txt
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.944463 django-form-surveys-1.8.2/djf_surveys/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-26 01:44:42.000000 django-form-surveys-1.8.2/djf_surveys/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admin.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.944463 django-form-surveys-1.8.2/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admins/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8146 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/admins/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/app_settings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/apps.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/context_processors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/forms.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.948463 django-form-surveys-1.8.2/djf_surveys/migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0001_initial.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0002_auto_20220330_1033.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0003_auto_20220330_1036.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0004_auto_20220330_1112.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0005_auto_20220404_1518.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0006_survey_private_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0007_auto_20220525_1126.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0008_auto_20220721_0935.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0009_auto_20220803_0927.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0010_model_translation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0011_alter_question_key.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-1.8.2/djf_surveys/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.948463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/rating.css
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   356448 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   455935 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.952463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-border.png
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-fill.png
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.952463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   198463 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      121 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.968463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   270873 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   783041 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12217 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50339 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   425275 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1151819 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   539120 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1929935 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7170 2022-12-26 04:13:44.000000 django-form-surveys-1.8.2/djf_surveys/summary.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/templates/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.976462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.976462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6956 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form_preview.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/question_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/summary.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/survey_list.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4237 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/answer_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.980462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/add_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/delete_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/edit_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/share_button.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/empty_state.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/header_nav.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3074 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/pagination.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      938 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/search_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      542 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/section_welcome.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_border.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_fill.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      889 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/detail_result.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2014 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      792 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/survey_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/datepicker.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templatetags/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templatetags/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/templatetags/djf_survey_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/tests.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      550 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/validators.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-1.8.2/djf_surveys/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/widgets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/setup.py
```

### Comparing `django-form-surveys-1.8.1/LICENSE` & `django-form-surveys-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/PKG-INFO` & `django-form-surveys-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-1.8.1/README.md` & `django-form-surveys-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/django_form_surveys.egg-info/PKG-INFO` & `django-form-surveys-1.8.2/django_form_surveys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.1
+Version: 1.8.2
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-1.8.1/django_form_surveys.egg-info/SOURCES.txt` & `django-form-surveys-1.8.2/django_form_surveys.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -35,16 +35,28 @@
 djf_surveys/migrations/0007_auto_20220525_1126.py
 djf_surveys/migrations/0008_auto_20220721_0935.py
 djf_surveys/migrations/0009_auto_20220803_0927.py
 djf_surveys/migrations/0010_model_translation.py
 djf_surveys/migrations/0011_alter_question_key.py
 djf_surveys/migrations/__init__.py
 djf_surveys/static/djf_surveys/css/rating.css
+djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
+djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
 djf_surveys/static/djf_surveys/images/star-border.png
 djf_surveys/static/djf_surveys/images/star-fill.png
+djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
+djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
+djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
+djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
+djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
+djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
+djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
+djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
+djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
+djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
 djf_surveys/templates/djf_surveys/answer_list.html
 djf_surveys/templates/djf_surveys/detail_result.html
 djf_surveys/templates/djf_surveys/form.html
 djf_surveys/templates/djf_surveys/master.html
 djf_surveys/templates/djf_surveys/survey_list.html
 djf_surveys/templates/djf_surveys/admins/form.html
 djf_surveys/templates/djf_surveys/admins/form_preview.html
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/admin.py` & `django-form-surveys-1.8.2/djf_surveys/admin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/admins/urls.py` & `django-form-surveys-1.8.2/djf_surveys/admins/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/admins/views.py` & `django-form-surveys-1.8.2/djf_surveys/admins/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/app_settings.py` & `django-form-surveys-1.8.2/djf_surveys/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/forms.py` & `django-form-surveys-1.8.2/djf_surveys/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0001_initial.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0002_auto_20220330_1033.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0002_auto_20220330_1033.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0003_auto_20220330_1036.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0003_auto_20220330_1036.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0004_auto_20220330_1112.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0004_auto_20220330_1112.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0007_auto_20220525_1126.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0007_auto_20220525_1126.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0008_auto_20220721_0935.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0008_auto_20220721_0935.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0009_auto_20220803_0927.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0009_auto_20220803_0927.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0010_model_translation.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0010_model_translation.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/migrations/0011_alter_question_key.py` & `django-form-surveys-1.8.2/djf_surveys/migrations/0011_alter_question_key.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/mixin.py` & `django-form-surveys-1.8.2/djf_surveys/mixin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/models.py` & `django-form-surveys-1.8.2/djf_surveys/models.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-border.png` & `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-border.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/static/djf_surveys/images/star-fill.png` & `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-fill.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/summary.py` & `django-form-surveys-1.8.2/djf_surveys/summary.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/form_preview.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form_preview.html`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
                     {% include "djf_surveys/buttons/edit_button.html" %}
                 </a>
                 <a href="#" class="button-share z-20 block p-4 text-amber-700 transition-all bg-amber-100 border-2 border-white rounded-full active:bg-amber-50 hover:scale-110 focus:outline-none focus:ring"
                     type="button" data-share-link="{% url 'djf_surveys:share_link' object.slug %}">
                     {% include "djf_surveys/buttons/share_button.html" %}
                 </a>
                 <a class="button-delete z-30 block p-4 text-red-700 transition-all bg-red-100 border-2 border-white rounded-full hover:scale-110 focus:outline-none focus:ring active:bg-red-50"
-                   data-bs-toggle="modal"
-                   data-bs-target="#modalDelete"
+                   data-te-toggle="modal"
+                   data-te-target="#modalDelete"
                    data-mdb-object_name="{{ object.name }}"
                    data-mdb-object_delete_url="{% url 'djf_surveys:admin_delete_survey' object.slug %}">
                     {% include "djf_surveys/buttons/delete_button.html" %}
                 </a>
             </div>
             <h1 class="text-2xl font-bold text-center text-blue-500 sm:text-3xl">{{ title_page }}</h1>
 
@@ -49,16 +49,16 @@
                             <a href="{% url 'djf_surveys:admin_edit_question' field|get_id_field %}"
                                class="z-20 block p-4 text-blue-700 transition-all bg-blue-100 border-2 border-white rounded-full active:bg-blue-50 hover:scale-110 focus:outline-none focus:ring"
                                type="button">
                                 {% include "djf_surveys/buttons/edit_button.html" %}
                             </a>
 
                             <a class="button-delete z-30 block p-4 text-red-700 transition-all bg-red-100 border-2 border-white rounded-full hover:scale-110 focus:outline-none focus:ring active:bg-red-50"
-                               data-bs-toggle="modal"
-                               data-bs-target="#modalDelete"
+                               data-te-toggle="modal"
+                               data-te-target="#modalDelete"
                                data-mdb-object_name="{{ field.label }}"
                                data-mdb-object_delete_url="{% url 'djf_surveys:admin_delete_question' field|get_id_field %}">
                                 {% include "djf_surveys/buttons/delete_button.html" %}
                             </a>
 
                         </div>
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/master.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/master.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 <!doctype html>
+{% load i18n static %}
 <html>
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Survey - {{ title }}</title>
-    <script src="https://cdn.tailwindcss.com"></script>
-    <script src="https://cdn.tailwindcss.com?plugins=forms,typography,aspect-ratio,line-clamp"></script>
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css" />
+    <title>{% trans "Survey" %} - {{ title }}</title>
+    <script src="{% static 'djf_surveys/css/tailwindcss-3.3.1.js' %}"></script>
+    <script src="{% static 'djf_surveys/css/tailwindcss-plugin-3.3.1.js' %}"></script>
     {% block extra_css %}{% endblock %}
 </head>
 <body>
     {% if messages %}
         {% for message in messages %}
             {% include 'djf_surveys/components/alert.html' %}
         {% endfor %}
     {% endif %}
-    {% include 'djf_surveys/components/header_nav.html' %}
     <div class="container mx-auto">
         {% block content %} {% endblock %}
     </div>
-    <script src="https://cdn.jsdelivr.net/npm/tw-elements/dist/js/index.min.js"></script>
+
     {% include 'djf_surveys/components/alert_js.html' %}
     {% block extra_js %}{% endblock %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-
+ {% load i18n static %}
 
  {% block extra_css %}{% endblock %}
 {% if messages %} {% for message in messages %} {% include 'djf_surveys/
-components/alert.html' %} {% endfor %} {% endif %} {% include 'djf_surveys/
-components/header_nav.html' %}
+components/alert.html' %} {% endfor %} {% endif %}
 {% block content %} {% endblock %}
- {% include 'djf_surveys/components/alert_js.html' %} {% block extra_js %}{%
+{% include 'djf_surveys/components/alert_js.html' %} {% block extra_js %}{%
 endblock %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/question_form.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/question_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/summary.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/summary.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% extends 'djf_surveys/admins/master.html' %}
 {% load static i18n %}
 
 {% block extra_css %}
     {{ chart_js_src|safe }}
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css"/>
+    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
     <link rel="stylesheet" href="{% static 'djf_surveys/css/rating.css' %}"/>
 {% endblock %}
 
 {% block content %}
     <div class="container px-5 py-5 ">
 
         <section>
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/admins/survey_list.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/answer_list.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/answer_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends get_master_template %}
 {% load i18n static %}
 
 {% block extra_css %}
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css"/>
+    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
     <link rel="stylesheet" href="{% static 'djf_surveys/css/rating.css' %}"/>
 {% endblock %}
 
 {% block content %}
     <div class="container px-5 py-5">
         <section>
             <div class="py-16 lg:items-end lg:justify-between lg:flex sm:px-6 lg:px-8">
@@ -64,11 +64,11 @@
     </div>
 
     {% include 'djf_surveys/components/modal_delete.html' %}
 
 {% endblock %}
 
 {% block extra_js %}
-    <script src="https://cdn.jsdelivr.net/npm/tw-elements/dist/js/index.min.js"></script>
+    <script src="{% static 'djf_surveys/te-starter/js/tw-elements.umd.min.js' %}"></script>
     {% include 'djf_surveys/components/modal_delete_js.html' %}
     {% include 'djf_surveys/components/share_link_button_js.html' %}
 {% endblock %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/alert.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
                                 <path stroke-linecap="round" stroke-linejoin="round" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z" />
                                 <path stroke-linecap="round" stroke-linejoin="round" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z" />
                               </svg>
                     </a>
                 {% endif %}
                 {% if object.survey.deletable %}
                     <a class="button-delete z-30 block p-4 text-red-700 transition-all bg-red-100 border-2 border-white rounded-full hover:scale-110 focus:outline-none focus:ring active:bg-red-50"
-                        data-bs-toggle="modal"
-                        data-bs-target="#modalDelete"
+                        data-te-toggle="modal"
+                        data-te-target="#modalDelete"
                         data-mdb-object_name="your answer"
                         data-mdb-object_delete_url="{% url 'djf_surveys:delete' object.id %}">
                         {% include "djf_surveys/buttons/delete_button.html" %}
                     </a>
                 {% endif %}
             </div>
         {% endif %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
                 <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                     <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 3.055A9.001 9.001 0 1020.945 13H11V3.055z" />
                     <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.488 9H15V3.512A9.025 9.025 0 0120.488 9z" />
                 </svg>
             </a>
 
             <button class="button-delete z-30 block p-4 text-red-700 transition-all bg-red-100 border-2 border-white rounded-full hover:scale-110 focus:outline-none focus:ring active:bg-red-50"
-                    data-bs-toggle="modal"
-                    data-bs-target="#modalDelete"
+                    data-te-toggle="modal"
+                    data-te-target="#modalDelete"
                     data-mdb-object_name="{{ survey.name }}"
                     data-mdb-object_delete_url="{% url 'djf_surveys:admin_delete_survey' survey.slug %}">
                 {% include "djf_surveys/buttons/delete_button.html" %}
             </button>
         {% endif %}
     </div>
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/header_nav.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/header_nav.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,70 @@
 {% load i18n %}
-<div class="modal fade fixed top-0 left-0 hidden w-full h-full outline-none overflow-x-hidden overflow-y-auto"
-     id="modalDelete" tabindex="-1" aria-labelledby="exampleModalCenterTitle" aria-modal="true" role="dialog">
-    <div class="modal-dialog modal-dialog-centered relative w-auto pointer-events-none">
-        <div class="modal-content border-none shadow-lg relative flex flex-col w-full pointer-events-auto bg-white bg-clip-padding rounded-md outline-none text-current">
-            <div class="modal-header flex flex-shrink-0 items-center justify-between p-4 border-b border-gray-200 rounded-t-md">
-                <h5 class="text-xl font-medium leading-normal text-gray-800" id="exampleModalScrollableLabel">
-                    {% trans "Confirmation" %}
-                </h5>
-                <button type="button"
-                        class="btn-close box-content w-4 h-4 p-1 text-black border-none rounded-none opacity-50 focus:shadow-none focus:outline-none focus:opacity-100 hover:text-black hover:opacity-75 hover:no-underline"
-                        data-bs-dismiss="modal" aria-label="{% trans "Close" %}"></button>
-            </div>
-            <div class="modal-body relative p-4">
-                <p>{% blocktrans with html='<span id="object_name" class="font-medium"/>' %}Are you sure to delete {{ html }}?{% endblocktrans %}</p>
-            </div>
-            <div
-                    class="modal-footer flex flex-shrink-0 flex-wrap items-center justify-end p-4 border-t border-gray-200 rounded-b-md">
-                <button type="button"
-                        class="inline-block px-6 py-2.5 bg-red-400 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-red-700 hover:shadow-lg focus:outline-none focus:ring-0 transition duration-150 ease-in-out"
-                        data-bs-dismiss="modal">
-                    {% trans "Cancel" %}
-                </button>
-                <a id="confirmDeleteButton"
-                        class="inline-block px-6 py-2.5 bg-blue-500 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-blue-800 transition duration-150 ease-in-out ml-1">
-                    {% trans "Yes" %}
-                </a>
-            </div>
-        </div>
+
+<div
+  data-te-modal-init
+  class="fixed left-0 top-0 z-[1055] hidden h-full w-full overflow-y-auto overflow-x-hidden outline-none"
+  id="modalDelete"
+  tabindex="-1"
+  aria-labelledby="modalDeleteLabel"
+  aria-hidden="true">
+  <div
+    data-te-modal-dialog-ref
+    class="pointer-events-none relative w-auto translate-y-[-50px] opacity-0 transition-all duration-300 ease-in-out min-[576px]:mx-auto min-[576px]:mt-7 min-[576px]:max-w-[500px]">
+    <div
+      class="min-[576px]:shadow-[0_0.5rem_1rem_rgba(#000, 0.15)] pointer-events-auto relative flex w-full flex-col rounded-md border-none bg-white bg-clip-padding text-current shadow-lg outline-none dark:bg-neutral-600">
+      <div
+        class="flex flex-shrink-0 items-center justify-between rounded-t-md border-b-2 border-neutral-100 border-opacity-100 p-4 dark:border-opacity-50">
+        <!--Modal title-->
+        <h5
+          class="text-xl font-medium leading-normal text-neutral-800 dark:text-neutral-200"
+          id="modalDeleteLabel">
+          {% trans "Confirmation" %}
+        </h5>
+        <!--Close button-->
+        <button
+          type="button"
+          class="box-content rounded-none border-none hover:no-underline hover:opacity-75 focus:opacity-100 focus:shadow-none focus:outline-none"
+          data-te-modal-dismiss
+          aria-label="Close">
+          <svg
+            xmlns="http://www.w3.org/2000/svg"
+            fill="none"
+            viewBox="0 0 24 24"
+            stroke-width="1.5"
+            stroke="currentColor"
+            class="h-6 w-6">
+            <path
+              stroke-linecap="round"
+              stroke-linejoin="round"
+              d="M6 18L18 6M6 6l12 12" />
+          </svg>
+        </button>
+      </div>
+
+      <!--Modal body-->
+      <div class="relative flex-auto p-4" data-te-modal-body-ref>
+        <p>{% blocktrans with html='<span id="object_name" class="font-medium"/>' %}Are you sure to delete {{ html }}?{% endblocktrans %}</p>
+      </div>
+
+      <!--Modal footer-->
+      <div
+        class="flex flex-shrink-0 flex-wrap items-center justify-end rounded-b-md border-t-2 border-neutral-100 border-opacity-100 p-4 dark:border-opacity-50">
+        <button
+          type="button"
+          class="inline-block px-6 py-2.5 bg-red-400 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-red-700 hover:shadow-lg focus:outline-none focus:ring-0 transition duration-150 ease-in-out"
+          data-te-modal-dismiss
+          data-te-ripple-init
+          data-te-ripple-color="light">
+          {% trans "Cancel" %}
+        </button>
+        <a
+          id="confirmDeleteButton"
+          class="inline-block px-6 py-2.5 bg-blue-500 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-blue-800 transition duration-150 ease-in-out ml-1"
+          data-te-ripple-init
+          data-te-ripple-color="light">
+          {% trans "Yes" %}
+        </a>
+      </div>
     </div>
-</div>
+  </div>
+</div>
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <script type="text/javascript">
     const buttonModals = document.getElementsByClassName('button-delete');
     const exampleModal = document.getElementById('modalDelete');
 
     for (var i = 0; i < buttonModals.length; i++) {
         buttonModals[i].addEventListener("click", (e) => {
-           const button = e.currentTarget;
-           const objectName = button.getAttribute('data-mdb-object_name');
-           const objectDeleteUrl = button.getAttribute('data-mdb-object_delete_url');
+            const button = e.currentTarget;
+            const objectName = button.getAttribute('data-mdb-object_name');
+            const objectDeleteUrl = button.getAttribute('data-mdb-object_delete_url');
 
             const modalTitle = exampleModal.querySelector('#object_name');
             const buttonDelete = exampleModal.querySelector('#confirmDeleteButton');
             buttonDelete.href = objectDeleteUrl;
             modalTitle.textContent = objectName;
         });
     }
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/pagination.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/pagination.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/search_form.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/search_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/section_welcome.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/section_welcome.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/components/star_border.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_border.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/detail_result.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/detail_result.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends get_master_template %}
 {% load djf_survey_tags static %}
 
 {% block extra_css %}
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css"/>
+    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
     <link rel="stylesheet" href="{% static 'djf_surveys/css/rating.css' %}"/>
 {% endblock %}
 
 {% block content %}
     <div class="max-w-screen-xl px-4 py-16 mx-auto sm:px-6 lg:px-8">
         <div class="max-w-lg mx-auto">
             <h1 class="text-2xl font-bold text-center text-blue-500 sm:text-3xl">{{ title_page }}</h1>
@@ -18,9 +18,9 @@
             {% include 'djf_surveys/components/card_list_answer.html' %}
         </div>
     </div>
 
 {% endblock %}
 
 {% block extra_js %}
-    <script src="https://cdn.jsdelivr.net/npm/tw-elements/dist/js/index.min.js"></script>
+    <script src="{% static 'djf_surveys/te-starter/js/tw-elements.umd.min.js' %}"></script>
 {% endblock %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/form.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/form.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% extends get_master_template %}
 {% load djf_survey_tags i18n static %}
 
 {% block extra_css %}
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css"/>
+    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
     <link rel="stylesheet" href="{% static 'djf_surveys/css/rating.css' %}"/>
 {% endblock %}
 
 {% block content %}
     <div class="max-w-screen-xl px-4 py-16 mx-auto sm:px-6 lg:px-8">
         <div class="max-w-lg mx-auto">
             <h1 class="text-2xl font-bold text-center text-blue-500 sm:text-3xl">{{ title_page }}</h1>
@@ -40,9 +40,9 @@
             </form>
         </div>
     </div>
 
 {% endblock %}
 
 {% block extra_js %}
-    <script src="https://cdn.jsdelivr.net/npm/tw-elements/dist/js/index.min.js"></script>
+    <script src="{% static 'djf_surveys/te-starter/js/tw-elements.umd.min.js' %}"></script>
 {% endblock %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/survey_list.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/survey_list.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends get_master_template %}
+{% load static %}
 
 {% block extra_css %}
-    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tw-elements/dist/css/index.min.css" />
+    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
 {% endblock %}
 
 {% block content %}
     <div class="container px-5 py-5">
         {% include 'djf_surveys/components/section_welcome.html' %}
 
         {% include 'djf_surveys/components/search_form.html' %}
@@ -24,10 +25,10 @@
     </div>
 
     {% include 'djf_surveys/components/modal_delete.html' %}
 
 {% endblock %}
 
 {% block extra_js %}
-    <script src="https://cdn.jsdelivr.net/npm/tw-elements/dist/js/index.min.js"></script>
+    <script src="{% static 'djf_surveys/te-starter/js/tw-elements.umd.min.js' %}"></script>
     {% include 'djf_surveys/components/modal_delete_js.html' %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-{% extends get_master_template %} {% block extra_css %}
+{% extends get_master_template %} {% load static %} {% block extra_css %}
  {% endblock %} {% block content %}
 {% include 'djf_surveys/components/section_welcome.html' %} {% include
 'djf_surveys/components/search_form.html' %} {% if object_list %}
 {% for survey in page_obj %} {% include 'djf_surveys/components/
 card_list_survey.html' %} {% endfor %}
 {% include 'djf_surveys/components/pagination.html' %}
 {% else %} {% include 'djf_surveys/components/empty_state.html' %} {% endif %}
```

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html` & `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/urls.py` & `django-form-surveys-1.8.2/djf_surveys/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/utils.py` & `django-form-surveys-1.8.2/djf_surveys/utils.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/validators.py` & `django-form-surveys-1.8.2/djf_surveys/validators.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/djf_surveys/views.py` & `django-form-surveys-1.8.2/djf_surveys/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.1/setup.py` & `django-form-surveys-1.8.2/setup.py`

 * *Files identical despite different names*

