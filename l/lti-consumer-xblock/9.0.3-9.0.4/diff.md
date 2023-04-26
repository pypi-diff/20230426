# Comparing `tmp/lti-consumer-xblock-9.0.3.tar.gz` & `tmp/lti-consumer-xblock-9.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lti-consumer-xblock-9.0.3.tar", last modified: Tue Apr 18 20:35:46 2023, max compression
+gzip compressed data, was "lti-consumer-xblock-9.0.4.tar", last modified: Tue Apr 25 18:30:45 2023, max compression
```

## Comparing `lti-consumer-xblock-9.0.3.tar` & `lti-consumer-xblock-9.0.4.tar`

### file list

```diff
@@ -1,213 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.647995 lti-consumer-xblock-9.0.3/lti_consumer/
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/data.py
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/filters.py
--rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/django.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_oauth.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/ags.py
--rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    32648 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.651996 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
--rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/nprs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.655995 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_key_handlers.py
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    69931 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/lti_xblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.659995 lti-consumer-xblock-9.0.3/lti_consumer/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0002_ltiagslineitem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0003_ltiagsscore.py
--rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0007_ltidlcontentitem.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0008_fix_uuid_backfill.py
--rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0013_auto_20210712_1352.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0014_adds_external_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/outcomes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/plugin/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/signals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/signals/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/css/student.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10596 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_lti_consumer.js
--rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_studio_view.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.663996 lti-consumer-xblock-9.0.3/lti_consumer/static/sass/
--rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/static/sass/student.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/dl_response_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/dl_response_saved.html
--rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_dl_content.html
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_html.html
--rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_image.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
--rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_permission_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_studio.html
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_iframe.html
--rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch.html
--rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_proctoring_start_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/html/student.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/outcome_service_response.xml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/get_dl_lti_launch_url.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/templatetags/lti_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.667996 lti-consumer-xblock-9.0.3/lti_consumer/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_proctoring.py
--rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
--rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
--rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
--rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_lti_xblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_outcomes.py
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/track.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.639995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.671995 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9197 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1404 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10080 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      461 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.675995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1349 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      601 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.643995 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/lti_consumer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      171 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-18 20:35:46.000000 lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 20:35:46.679996 lti-consumer-xblock-9.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-18 20:35:46.683996 lti-consumer-xblock-9.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-18 20:35:41.000000 lti-consumer-xblock-9.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13412 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1317 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5845 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14958 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5551 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/django.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6923 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5976 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13817 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3674 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_oauth.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2773 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32648 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3499 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1759 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14353 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10557 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/nprs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.476392 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4234 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9039 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39510 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10270 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_key_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    71037 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/lti_xblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0002_ltiagslineitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1677 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0003_ltiagsscore.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0004_keyset_mgmt_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0005_migrate_keyset_to_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2361 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0007_ltidlcontentitem.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0008_fix_uuid_backfill.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1403 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0009_backfill-empty-string-config-id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2510 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0012_rename_courseeditltifieldsenabledflag_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0013_auto_20210712_1352.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0014_adds_external_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3641 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0015_add_additional_1p3_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      521 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32021 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/outcomes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11681 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/plugin/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    22730 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3602 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    23422 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    21751 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    20445 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.480393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    17362 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)     3879 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)     4601 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    13621 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)     3772 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3800 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)     4091 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/css/student.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    11301 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_lti_consumer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6043 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_studio_view.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/static/sass/
+-rw-r--r--   0 runner    (1001) docker     (122)     4751 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/static/sass/student.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/dl_response_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/dl_response_saved.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_dl_content.html
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_html.html
+-rw-r--r--   0 runner    (1001) docker     (122)      890 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_image.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      355 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_lti_resource_link.html
+-rw-r--r--   0 runner    (1001) docker     (122)      893 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_permission_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_studio.html
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_iframe.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch.html
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_proctoring_start_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3849 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/html/student.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/outcome_service_response.xml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/get_dl_lti_launch_url.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/templatetags/lti_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.484393 lti-consumer-xblock-9.0.4/lti_consumer/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2807 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11288 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_proctoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25574 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38579 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_ags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10559 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26379 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2866 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    82946 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_lti_xblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24054 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16718 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_outcomes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4743 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/track.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16396 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20799 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26467 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18761 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25340 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.488393 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9166 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9608 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    21499 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16407 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9838 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    10907 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.468392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16477 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16884 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10221 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18852 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16547 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1987 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.472392 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      432 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16458 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10931 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/lti_consumer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14196 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     7590 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      199 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-04-25 18:30:45.000000 lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-25 18:30:45.492393 lti-consumer-xblock-9.0.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-25 18:30:45.496393 lti-consumer-xblock-9.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5875 2023-04-25 18:30:41.000000 lti-consumer-xblock-9.0.4/setup.py
```

### Comparing `lti-consumer-xblock-9.0.3/LICENSE` & `lti-consumer-xblock-9.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/NOTICE` & `lti-consumer-xblock-9.0.4/NOTICE`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/PKG-INFO` & `lti-consumer-xblock-9.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.3
+Version: 9.0.4
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.3/README.rst` & `lti-consumer-xblock-9.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/admin.py` & `lti-consumer-xblock-9.0.4/lti_consumer/admin.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/api.py` & `lti-consumer-xblock-9.0.4/lti_consumer/api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/apps.py` & `lti-consumer-xblock-9.0.4/lti_consumer/apps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/data.py` & `lti-consumer-xblock-9.0.4/lti_consumer/data.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/filters.py` & `lti-consumer-xblock-9.0.4/lti_consumer/filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/forms.py` & `lti-consumer-xblock-9.0.4/lti_consumer/forms.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/consumer.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/django.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/contrib/tests/test_django.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/contrib/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/oauth.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_consumer.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p1/tests/test_oauth.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p1/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/ags.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/constants.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/constants.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/consumer.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/deep_linking.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/exceptions.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/exceptions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/parsers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/renderers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/serializers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/extensions/rest_framework/utils.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/extensions/rest_framework/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/key_handlers.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/nprs.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/nprs.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/extensions/rest_framework/test_permissions.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_ags.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_consumer.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_deep_linking.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_key_handlers.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_key_handlers.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_1p3/tests/test_nrps.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_1p3/tests/test_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/lti_xblock.py` & `lti-consumer-xblock-9.0.4/lti_consumer/lti_xblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,18 +51,19 @@
 """
 
 import logging
 import re
 import urllib.parse
 from collections import namedtuple
 from importlib import import_module
+import pkg_resources
 
 import bleach
 from django.conf import settings
-from django.utils import timezone
+from django.utils import timezone, translation
 from web_fragments.fragment import Fragment
 
 from webob import Response
 from xblock.core import List, Scope, String, XBlock
 from xblock.fields import Boolean, Float, Integer
 from xblock.validation import ValidationMessage
 from xblockutils.resources import ResourceLoader
@@ -641,14 +642,30 @@
                         launch_target="iframe"
                         launch_url="https://lti.tools/saltire/tp" />
                 </sequence_demo>
              '''),
         ]
         return scenarios
 
+    @staticmethod
+    def _get_statici18n_js_url(loader):  # pragma: no cover
+        """
+        Returns the Javascript translation file for the currently selected language, if any found by
+        `pkg_resources`
+        """
+        lang_code = translation.get_language()
+        if not lang_code:
+            return None
+        text_js = 'public/js/translations/{lang_code}/text.js'
+        country_code = lang_code.split('-')[0]
+        for code in (translation.to_locale(lang_code), lang_code, country_code):
+            if pkg_resources.resource_exists(loader.module_name, text_js.format(lang_code=code)):
+                return text_js.format(lang_code=code)
+        return None
+
     def validate_field_data(self, validation, data):
         if not isinstance(data.custom_parameters, list):
             _ = self.runtime.service(self, "i18n").ugettext
             validation.add(ValidationMessage(ValidationMessage.ERROR, str(
                 _("Custom Parameters must be a list")
             )))
 
@@ -1121,14 +1138,17 @@
                 '/templates/html/lti_1p3_studio.html',
                 context,
                 i18n_service=self.runtime.service(self, 'i18n')
             ),
         )
         fragment.add_css(loader.load_unicode('static/css/student.css'))
         fragment.add_javascript(loader.load_unicode('static/js/xblock_lti_consumer.js'))
+        statici18n_js_url = self._get_statici18n_js_url(loader)
+        if statici18n_js_url:
+            fragment.add_javascript_url(self.runtime.local_resource_url(self, statici18n_js_url))
         fragment.initialize_js('LtiConsumerXBlock')
         return fragment
 
     @XBlock.supports("multi_device")
     def student_view(self, context):
         """
         XBlock student view of this component.
@@ -1145,14 +1165,17 @@
         """
         fragment = Fragment()
         loader = ResourceLoader(__name__)
         context.update(self._get_context_for_template())
         fragment.add_content(loader.render_mako_template('/templates/html/student.html', context))
         fragment.add_css(loader.load_unicode('static/css/student.css'))
         fragment.add_javascript(loader.load_unicode('static/js/xblock_lti_consumer.js'))
+        statici18n_js_url = self._get_statici18n_js_url(loader)
+        if statici18n_js_url:
+            fragment.add_javascript_url(self.runtime.local_resource_url(self, statici18n_js_url))
         fragment.initialize_js('LtiConsumerXBlock')
         return fragment
 
     @XBlock.handler
     def lti_launch_handler(self, request, suffix=''):  # pylint: disable=unused-argument
         """
         XBlock handler for launching LTI 1.1 tools.
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0001_initial.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0002_ltiagslineitem.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0002_ltiagslineitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0003_ltiagsscore.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0003_ltiagsscore.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0004_keyset_mgmt_to_model.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0004_keyset_mgmt_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0005_migrate_keyset_to_model.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0005_migrate_keyset_to_model.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0006_add_on_model_config_for_lti_1p1.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0007_ltidlcontentitem.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0007_ltidlcontentitem.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0008_fix_uuid_backfill.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0008_fix_uuid_backfill.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0009_backfill-empty-string-config-id.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0009_backfill-empty-string-config-id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0010_backfill-empty-string-lti-config.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0011_courseeditltifieldsenabledflag.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0013_auto_20210712_1352.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0013_auto_20210712_1352.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0014_adds_external_id.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0014_adds_external_id.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0015_add_additional_1p3_fields.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0015_add_additional_1p3_fields.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py` & `lti-consumer-xblock-9.0.4/lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/models.py` & `lti-consumer-xblock-9.0.4/lti_consumer/models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/outcomes.py` & `lti-consumer-xblock-9.0.4/lti_consumer/outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/plugin/compat.py` & `lti-consumer-xblock-9.0.4/lti_consumer/plugin/compat.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/plugin/urls.py` & `lti-consumer-xblock-9.0.4/lti_consumer/plugin/urls.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/plugin/views.py` & `lti-consumer-xblock-9.0.4/lti_consumer/plugin/views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/signals/signals.py` & `lti-consumer-xblock-9.0.4/lti_consumer/signals/signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/static/css/student.css` & `lti-consumer-xblock-9.0.4/lti_consumer/static/css/student.css`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_lti_consumer.js` & `lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_lti_consumer.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,25 @@
 function LtiConsumerXBlock(runtime, element) {
+    var gettext;
+    if ('XBlockLtiConsumerI18N' in window) {
+        // Use local translations
+        gettext = function(string) {
+            var translated = window.XBlockLtiConsumerI18N.gettext(string);
+            // if lti-consumer translation is the same as the input, check if global has a different value
+            // This is useful for overriding the XBlock's string by themes (only for English)
+            if (string === translated && 'gettext' in window) {
+                translated = window.gettext(string);
+            }
+            return translated;
+        };
+    } else if ('gettext' in window) {
+        // Use edxapp's global translations
+        gettext = window.gettext;
+    }
+
     $(function($) {
         // Adapted from leanModal v1.1 by Ray Stone - http://finelysliced.com.au
         // Dual licensed under the MIT and GPL
         // Renamed leanModal to iframeModal to avoid clash with platform-provided leanModal
         // which removes the href attribute from iframe elements upon modal closing
         $.fn.extend({
             iframeModal: function(options) {
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/static/js/xblock_studio_view.js` & `lti-consumer-xblock-9.0.4/lti_consumer/static/js/xblock_studio_view.js`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/static/sass/student.scss` & `lti-consumer-xblock-9.0.4/lti_consumer/static/sass/student.scss`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_dl_content.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_dl_content.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_image.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_image.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti-dl/render_link.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti-dl/render_link.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_launch.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_1p3_studio.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_1p3_studio.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/lti_launch.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/lti_launch.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/html/student.html` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/html/student.html`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templates/xml/outcome_service_response.xml` & `lti-consumer-xblock-9.0.4/lti_consumer/templates/xml/outcome_service_response.xml`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templatetags/get_dl_lti_launch_url.py` & `lti-consumer-xblock-9.0.4/lti_consumer/templatetags/get_dl_lti_launch_url.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/templatetags/lti_sanitize.py` & `lti-consumer-xblock-9.0.4/lti_consumer/templatetags/lti_sanitize.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/test_utils.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_proctoring.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_proctoring.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_ags.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_ags.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/plugin/test_views_lti_nrps.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_api.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_filters.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_filters.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_lti_xblock.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_lti_xblock.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_models.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_outcomes.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_signals.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_signals.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/tests/unit/test_utils.py` & `lti-consumer-xblock-9.0.4/lti_consumer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
-"PO-Revision-Date: 2017-09-23 22:34+0000\n"
-"Last-Translator: shefaa abu jabel <shefaa.aj@gmail.com>\n"
-"Language-Team: Arabic (http://www.transifex.com/open-edx/xblocks/language/"
+"Report-Msgid-Bugs-To: \n"
+"PO-Revision-Date: 2016-06-08 14:38+0000\n"
+"Last-Translator: shefaa abu jabel <shefaa.aj@gmail.com>, 2016\n"
+"Language-Team: Arabic (http://app.transifex.com/open-edx/xblocks/language/"
 "ar/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
-"X-Generator: Poedit 1.8.7\n"
-"X-Poedit-Basepath: ../../..\n"
-"X-Poedit-SearchPath-0: lti_consumer.py\n"
 
 msgid "Accept grades past deadline"
 msgstr "قبول العلامات بعد انقضاء الموعد المحدد"
 
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your e-"
 "book should open to or the background color for this component. Ex. "
@@ -34,27 +32,14 @@
 
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "الملاحظات التي تم إرجاعها من مانح العلامة، مواصفات LTI2.0"
 
 msgid "Could not get user id for current request"
 msgstr "تعذر الحصول على هوية مستخدم للطلب الحالي"
 
-msgid ""
-"Could not parse LTI passport: {lti_passport}. Should be \"id:key:secret\" "
-"string."
-msgstr ""
-"تعذر تحليل جواز مرورLTI : {lti_passport}. يجب أن يكون سلسلة \"id:key:"
-"secret\"."
-
-msgid ""
-"Could not parse custom parameter: {custom_parameter}. Should be \"x=y\" "
-"string."
-msgstr ""
-"تعذر تحليل العامل المخصص: {custom_parameter}. يجب أن يكون سلسلة \"x=y\"."
-
 msgid "Custom Parameters"
 msgstr "العوامل المخصصة"
 
 msgid "Display Name"
 msgstr "عرض الاسم"
 
 msgid ""
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ar/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/en/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files 23% similar despite different names*

```diff
@@ -1,575 +1,637 @@
-00000000: de12 0495 0000 0000 2800 0000 1c00 0000  ........(.......
-00000010: 5c01 0000 3500 0000 9c02 0000 0000 0000  \...5...........
-00000020: 7003 0000 1b00 0000 7103 0000 0c01 0000  p.......q.......
-00000030: 8d03 0000 0b00 0000 9a04 0000 2c00 0000  ............,...
-00000040: a604 0000 2900 0000 d304 0000 4f00 0000  ....).......O...
-00000050: fd04 0000 4d00 0000 4d05 0000 1100 0000  ....M...M.......
-00000060: 9b05 0000 0c00 0000 ad05 0000 ca00 0000  ................
-00000070: ba05 0000 0401 0000 8506 0000 e800 0000  ................
-00000080: 8a07 0000 b700 0000 7308 0000 cb00 0000  ........s.......
-00000090: 2b09 0000 ca00 0000 f709 0000 8000 0000  +...............
-000000a0: c20a 0000 8900 0000 430b 0000 bf00 0000  ........C.......
-000000b0: cd0b 0000 1200 0000 8d0c 0000 0d00 0000  ................
-000000c0: a00c 0000 1b00 0000 ae0c 0000 0c00 0000  ................
-000000d0: ca0c 0000 0600 0000 d70c 0000 1100 0000  ................
-000000e0: de0c 0000 0700 0000 f00c 0000 0c00 0000  ................
-000000f0: f80c 0000 0b00 0000 050d 0000 2600 0000  ............&...
-00000100: 110d 0000 1400 0000 380d 0000 1700 0000  ........8.......
-00000110: 4d0d 0000 0600 0000 650d 0000 3d01 0000  M.......e...=...
-00000120: 6c0d 0000 5a00 0000 aa0e 0000 da00 0000  l...Z...........
-00000130: 050f 0000 4a00 0000 e00f 0000 3000 0000  ....J.......0...
-00000140: 2b10 0000 2b00 0000 5c10 0000 5100 0000  +...+...\...Q...
-00000150: 8810 0000 2e00 0000 da10 0000 db01 0000  ................
-00000160: 0911 0000 2a00 0000 e512 0000 4b01 0000  ....*.......K...
-00000170: 1013 0000 1400 0000 5c14 0000 4200 0000  ........\...B...
-00000180: 7114 0000 3700 0000 b414 0000 6200 0000  q...7.......b...
-00000190: ec14 0000 5f00 0000 4f15 0000 1a00 0000  ...._...O.......
-000001a0: af15 0000 1000 0000 ca15 0000 f900 0000  ................
-000001b0: db15 0000 3501 0000 d516 0000 2601 0000  ....5.......&...
-000001c0: 0b18 0000 da00 0000 3219 0000 fa00 0000  ........2.......
-000001d0: 0d1a 0000 ff00 0000 081b 0000 ae00 0000  ................
-000001e0: 081c 0000 b300 0000 b71c 0000 e200 0000  ................
-000001f0: 6b1d 0000 1e00 0000 4e1e 0000 0d00 0000  k.......N.......
-00000200: 6d1e 0000 2500 0000 7b1e 0000 0e00 0000  m...%...{.......
-00000210: a11e 0000 0900 0000 b01e 0000 1200 0000  ................
-00000220: ba1e 0000 0a00 0000 cd1e 0000 1000 0000  ................
-00000230: d81e 0000 0f00 0000 e91e 0000 3f00 0000  ............?...
-00000240: f91e 0000 2d00 0000 391f 0000 2700 0000  ....-...9...'...
-00000250: 671f 0000 0800 0000 8f1f 0000 7e01 0000  g...........~...
-00000260: 981f 0000 6400 0000 1721 0000 e300 0000  ....d....!......
-00000270: 7c21 0000 6d00 0000 6022 0000 4200 0000  |!..m...`"..B...
-00000280: ce22 0000 3400 0000 1123 0000 6400 0000  ."..4....#..d...
-00000290: 4623 0000 4100 0000 ab23 0000 0100 0000  F#..A....#......
-000002a0: 1f00 0000 1900 0000 1700 0000 0700 0000  ................
-000002b0: 0f00 0000 0600 0000 1000 0000 1400 0000  ................
-000002c0: 1300 0000 1e00 0000 1a00 0000 0000 0000  ................
-000002d0: 0000 0000 0c00 0000 1100 0000 0000 0000  ................
-000002e0: 2000 0000 1800 0000 0e00 0000 2300 0000   ...........#...
-000002f0: 0000 0000 0400 0000 1b00 0000 0000 0000  ................
-00000300: 0500 0000 1200 0000 2600 0000 0800 0000  ........&.......
-00000310: 1d00 0000 0000 0000 0000 0000 0000 0000  ................
-00000320: 2100 0000 0900 0000 1600 0000 2400 0000  !...........$...
-00000330: 0000 0000 0000 0000 2800 0000 1c00 0000  ........(.......
-00000340: 0a00 0000 2200 0000 0d00 0000 0000 0000  ...."...........
-00000350: 0300 0000 2500 0000 0000 0000 1500 0000  ....%...........
-00000360: 0200 0000 0b00 0000 0000 0000 2700 0000  ............'...
-00000370: 0041 6363 6570 7420 6772 6164 6573 2070  .Accept grades p
-00000380: 6173 7420 6465 6164 6c69 6e65 0041 6464  ast deadline.Add
-00000390: 2074 6865 206b 6579 2f76 616c 7565 2070   the key/value p
-000003a0: 6169 7220 666f 7220 616e 7920 6375 7374  air for any cust
-000003b0: 6f6d 2070 6172 616d 6574 6572 732c 2073  om parameters, s
-000003c0: 7563 6820 6173 2074 6865 2070 6167 6520  uch as the page 
-000003d0: 796f 7572 2065 2d62 6f6f 6b20 7368 6f75  your e-book shou
-000003e0: 6c64 206f 7065 6e20 746f 206f 7220 7468  ld open to or th
-000003f0: 6520 6261 636b 6772 6f75 6e64 2063 6f6c  e background col
-00000400: 6f72 2066 6f72 2074 6869 7320 636f 6d70  or for this comp
-00000410: 6f6e 656e 742e 2045 782e 205b 2270 6167  onent. Ex. ["pag
-00000420: 653d 3122 2c20 2263 6f6c 6f72 3d77 6869  e=1", "color=whi
-00000430: 7465 225d 3c62 7220 2f3e 5365 6520 7468  te"]<br />See th
-00000440: 6520 7b64 6f63 735f 616e 6368 6f72 5f6f  e {docs_anchor_o
-00000450: 7065 6e7d 6564 5820 4c54 4920 646f 6375  pen}edX LTI docu
-00000460: 6d65 6e74 6174 696f 6e7b 616e 6368 6f72  mentation{anchor
-00000470: 5f63 6c6f 7365 7d20 666f 7220 6d6f 7265  _close} for more
-00000480: 2064 6574 6169 6c73 206f 6e20 7468 6973   details on this
-00000490: 2073 6574 7469 6e67 2e00 4275 7474 6f6e   setting..Button
-000004a0: 2054 6578 7400 436f 6d6d 656e 7420 6173   Text.Comment as
-000004b0: 2072 6574 7572 6e65 6420 6672 6f6d 2067   returned from g
-000004c0: 7261 6465 722c 204c 5449 322e 3020 7370  rader, LTI2.0 sp
-000004d0: 6563 0043 6f75 6c64 206e 6f74 2067 6574  ec.Could not get
-000004e0: 2075 7365 7220 6964 2066 6f72 2063 7572   user id for cur
-000004f0: 7265 6e74 2072 6571 7565 7374 0043 6f75  rent request.Cou
-00000500: 6c64 206e 6f74 2070 6172 7365 204c 5449  ld not parse LTI
-00000510: 2070 6173 7370 6f72 743a 207b 6c74 695f   passport: {lti_
-00000520: 7061 7373 706f 7274 7d2e 2053 686f 756c  passport}. Shoul
-00000530: 6420 6265 2022 6964 3a6b 6579 3a73 6563  d be "id:key:sec
-00000540: 7265 7422 2073 7472 696e 672e 0043 6f75  ret" string..Cou
-00000550: 6c64 206e 6f74 2070 6172 7365 2063 7573  ld not parse cus
-00000560: 746f 6d20 7061 7261 6d65 7465 723a 207b  tom parameter: {
-00000570: 6375 7374 6f6d 5f70 6172 616d 6574 6572  custom_parameter
-00000580: 7d2e 2053 686f 756c 6420 6265 2022 783d  }. Should be "x=
-00000590: 7922 2073 7472 696e 672e 0043 7573 746f  y" string..Custo
-000005a0: 6d20 5061 7261 6d65 7465 7273 0044 6973  m Parameters.Dis
-000005b0: 706c 6179 204e 616d 6500 456e 7465 7220  play Name.Enter 
-000005c0: 6120 6465 7363 7269 7074 696f 6e20 6f66  a description of
-000005d0: 2074 6865 2074 6869 7264 2070 6172 7479   the third party
-000005e0: 2061 7070 6c69 6361 7469 6f6e 2e20 4966   application. If
-000005f0: 2072 6571 7565 7374 696e 6720 7573 6572   requesting user
-00000600: 6e61 6d65 2061 6e64 2f6f 7220 656d 6169  name and/or emai
-00000610: 6c2c 2075 7365 2074 6869 7320 7465 7874  l, use this text
-00000620: 2062 6f78 2074 6f20 696e 666f 726d 2075   box to inform u
-00000630: 7365 7273 2077 6879 2074 6865 6972 2075  sers why their u
-00000640: 7365 726e 616d 6520 616e 642f 6f72 2065  sername and/or e
-00000650: 6d61 696c 2077 696c 6c20 6265 2066 6f72  mail will be for
-00000660: 7761 7264 6564 2074 6f20 6120 7468 6972  warded to a thir
-00000670: 6420 7061 7274 7920 6170 706c 6963 6174  d party applicat
-00000680: 696f 6e2e 0045 6e74 6572 2074 6865 204c  ion..Enter the L
-00000690: 5449 2049 4420 666f 7220 7468 6520 6578  TI ID for the ex
-000006a0: 7465 726e 616c 204c 5449 2070 726f 7669  ternal LTI provi
-000006b0: 6465 722e 2054 6869 7320 7661 6c75 6520  der. This value 
-000006c0: 6d75 7374 2062 6520 7468 6520 7361 6d65  must be the same
-000006d0: 204c 5449 2049 4420 7468 6174 2079 6f75   LTI ID that you
-000006e0: 2065 6e74 6572 6564 2069 6e20 7468 6520   entered in the 
-000006f0: 4c54 4920 5061 7373 706f 7274 7320 7365  LTI Passports se
-00000700: 7474 696e 6720 6f6e 2074 6865 2041 6476  tting on the Adv
-00000710: 616e 6365 6420 5365 7474 696e 6773 2070  anced Settings p
-00000720: 6167 652e 3c62 7220 2f3e 5365 6520 7468  age.<br />See th
-00000730: 6520 7b64 6f63 735f 616e 6368 6f72 5f6f  e {docs_anchor_o
-00000740: 7065 6e7d 6564 5820 4c54 4920 646f 6375  pen}edX LTI docu
-00000750: 6d65 6e74 6174 696f 6e7b 616e 6368 6f72  mentation{anchor
-00000760: 5f63 6c6f 7365 7d20 666f 7220 6d6f 7265  _close} for more
-00000770: 2064 6574 6169 6c73 206f 6e20 7468 6973   details on this
-00000780: 2073 6574 7469 6e67 2e00 456e 7465 7220   setting..Enter 
-00000790: 7468 6520 5552 4c20 6f66 2074 6865 2065  the URL of the e
-000007a0: 7874 6572 6e61 6c20 746f 6f6c 2074 6861  xternal tool tha
-000007b0: 7420 7468 6973 2063 6f6d 706f 6e65 6e74  t this component
-000007c0: 206c 6175 6e63 6865 732e 2054 6869 7320   launches. This 
-000007d0: 7365 7474 696e 6720 6973 206f 6e6c 7920  setting is only 
-000007e0: 7573 6564 2077 6865 6e20 4869 6465 2045  used when Hide E
-000007f0: 7874 6572 6e61 6c20 546f 6f6c 2069 7320  xternal Tool is 
-00000800: 7365 7420 746f 2046 616c 7365 2e3c 6272  set to False.<br
-00000810: 202f 3e53 6565 2074 6865 207b 646f 6373   />See the {docs
-00000820: 5f61 6e63 686f 725f 6f70 656e 7d65 6458  _anchor_open}edX
-00000830: 204c 5449 2064 6f63 756d 656e 7461 7469   LTI documentati
-00000840: 6f6e 7b61 6e63 686f 725f 636c 6f73 657d  on{anchor_close}
-00000850: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
-00000860: 7320 6f6e 2074 6869 7320 7365 7474 696e  s on this settin
-00000870: 672e 0045 6e74 6572 2074 6865 2064 6573  g..Enter the des
-00000880: 6972 6564 2070 6978 656c 2068 6569 6768  ired pixel heigh
-00000890: 7420 6f66 2074 6865 2069 6672 616d 6520  t of the iframe 
-000008a0: 7768 6963 6820 7769 6c6c 2063 6f6e 7461  which will conta
-000008b0: 696e 2074 6865 204c 5449 2074 6f6f 6c2e  in the LTI tool.
-000008c0: 2054 6869 7320 7365 7474 696e 6720 6973   This setting is
-000008d0: 206f 6e6c 7920 7573 6564 2077 6865 6e20   only used when 
-000008e0: 4869 6465 2045 7874 6572 6e61 6c20 546f  Hide External To
-000008f0: 6f6c 2069 7320 7365 7420 746f 2046 616c  ol is set to Fal
-00000900: 7365 2061 6e64 204c 5449 204c 6175 6e63  se and LTI Launc
-00000910: 6820 5461 7267 6574 2069 7320 7365 7420  h Target is set 
-00000920: 746f 2049 6e6c 696e 652e 0045 6e74 6572  to Inline..Enter
-00000930: 2074 6865 2064 6573 6972 6564 2076 6965   the desired vie
-00000940: 7770 6f72 7420 7065 7263 656e 7461 6765  wport percentage
-00000950: 2068 6569 6768 7420 6f66 2074 6865 206d   height of the m
-00000960: 6f64 616c 206f 7665 726c 6179 2077 6869  odal overlay whi
-00000970: 6368 2077 696c 6c20 636f 6e74 6169 6e20  ch will contain 
-00000980: 7468 6520 4c54 4920 746f 6f6c 2e20 5468  the LTI tool. Th
-00000990: 6973 2073 6574 7469 6e67 2069 7320 6f6e  is setting is on
-000009a0: 6c79 2075 7365 6420 7768 656e 2048 6964  ly used when Hid
-000009b0: 6520 4578 7465 726e 616c 2054 6f6f 6c20  e External Tool 
-000009c0: 6973 2073 6574 2074 6f20 4661 6c73 6520  is set to False 
-000009d0: 616e 6420 4c54 4920 4c61 756e 6368 2054  and LTI Launch T
-000009e0: 6172 6765 7420 6973 2073 6574 2074 6f20  arget is set to 
-000009f0: 4d6f 6461 6c2e 0045 6e74 6572 2074 6865  Modal..Enter the
-00000a00: 2064 6573 6972 6564 2076 6965 7770 6f72   desired viewpor
-00000a10: 7420 7065 7263 656e 7461 6765 2077 6964  t percentage wid
-00000a20: 7468 206f 6620 7468 6520 6d6f 6461 6c20  th of the modal 
-00000a30: 6f76 6572 6c61 7920 7768 6963 6820 7769  overlay which wi
-00000a40: 6c6c 2063 6f6e 7461 696e 2074 6865 204c  ll contain the L
-00000a50: 5449 2074 6f6f 6c2e 2054 6869 7320 7365  TI tool. This se
-00000a60: 7474 696e 6720 6973 206f 6e6c 7920 7573  tting is only us
-00000a70: 6564 2077 6865 6e20 4869 6465 2045 7874  ed when Hide Ext
-00000a80: 6572 6e61 6c20 546f 6f6c 2069 7320 7365  ernal Tool is se
-00000a90: 7420 746f 2046 616c 7365 2061 6e64 204c  t to False and L
-00000aa0: 5449 204c 6175 6e63 6820 5461 7267 6574  TI Launch Target
-00000ab0: 2069 7320 7365 7420 746f 204d 6f64 616c   is set to Modal
-00000ac0: 2e00 456e 7465 7220 7468 6520 6e61 6d65  ..Enter the name
-00000ad0: 2074 6861 7420 7374 7564 656e 7473 2073   that students s
-00000ae0: 6565 2066 6f72 2074 6869 7320 636f 6d70  ee for this comp
-00000af0: 6f6e 656e 742e 2041 6e61 6c79 7469 6373  onent. Analytics
-00000b00: 2072 6570 6f72 7473 206d 6179 2061 6c73   reports may als
-00000b10: 6f20 7573 6520 7468 6520 6469 7370 6c61  o use the displa
-00000b20: 7920 6e61 6d65 2074 6f20 6964 656e 7469  y name to identi
-00000b30: 6679 2074 6869 7320 636f 6d70 6f6e 656e  fy this componen
-00000b40: 742e 0045 6e74 6572 2074 6865 206e 756d  t..Enter the num
-00000b50: 6265 7220 6f66 2070 6f69 6e74 7320 706f  ber of points po
-00000b60: 7373 6962 6c65 2066 6f72 2074 6869 7320  ssible for this 
-00000b70: 636f 6d70 6f6e 656e 742e 2020 5468 6520  component.  The 
-00000b80: 6465 6661 756c 7420 7661 6c75 6520 6973  default value is
-00000b90: 2031 2e30 2e20 2054 6869 7320 7365 7474   1.0.  This sett
-00000ba0: 696e 6720 6973 206f 6e6c 7920 7573 6564  ing is only used
-00000bb0: 2077 6865 6e20 5363 6f72 6564 2069 7320   when Scored is 
-00000bc0: 7365 7420 746f 2054 7275 652e 0045 6e74  set to True..Ent
-00000bd0: 6572 2074 6865 2074 6578 7420 6f6e 2074  er the text on t
-00000be0: 6865 2062 7574 746f 6e20 7573 6564 2074  he button used t
-00000bf0: 6f20 6c61 756e 6368 2074 6865 2074 6869  o launch the thi
-00000c00: 7264 2070 6172 7479 2061 7070 6c69 6361  rd party applica
-00000c10: 7469 6f6e 2e20 5468 6973 2073 6574 7469  tion. This setti
-00000c20: 6e67 2069 7320 6f6e 6c79 2075 7365 6420  ng is only used 
-00000c30: 7768 656e 2048 6964 6520 4578 7465 726e  when Hide Extern
-00000c40: 616c 2054 6f6f 6c20 6973 2073 6574 2074  al Tool is set t
-00000c50: 6f20 4661 6c73 6520 616e 6420 4c54 4920  o False and LTI 
-00000c60: 4c61 756e 6368 2054 6172 6765 7420 6973  Launch Target is
-00000c70: 2073 6574 2074 6f20 4d6f 6461 6c20 6f72   set to Modal or
-00000c80: 204e 6577 2057 696e 646f 772e 0048 6964   New Window..Hid
-00000c90: 6520 4578 7465 726e 616c 2054 6f6f 6c00  e External Tool.
-00000ca0: 496e 6c69 6e65 2048 6569 6768 7400 4c54  Inline Height.LT
-00000cb0: 4920 4170 706c 6963 6174 696f 6e20 496e  I Application In
-00000cc0: 666f 726d 6174 696f 6e00 4c54 4920 436f  formation.LTI Co
-00000cd0: 6e73 756d 6572 004c 5449 2049 4400 4c54  nsumer.LTI ID.LT
-00000ce0: 4920 4c61 756e 6368 2054 6172 6765 7400  I Launch Target.
-00000cf0: 4c54 4920 5552 4c00 4d6f 6461 6c20 4865  LTI URL.Modal He
-00000d00: 6967 6874 004d 6f64 616c 2057 6964 7468  ight.Modal Width
-00000d10: 004e 6f20 7661 6c69 6420 7573 6572 2069  .No valid user i
-00000d20: 6420 666f 756e 6420 696e 2065 6e64 706f  d found in endpo
-00000d30: 696e 7420 5552 4c00 5265 7175 6573 7420  int URL.Request 
-00000d40: 7573 6572 2773 2065 6d61 696c 0052 6571  user's email.Req
-00000d50: 7565 7374 2075 7365 7227 7320 7573 6572  uest user's user
-00000d60: 6e61 6d65 0053 636f 7265 6400 5365 6c65  name.Scored.Sele
-00000d70: 6374 2049 6e6c 696e 6520 6966 2079 6f75  ct Inline if you
-00000d80: 2077 616e 7420 7468 6520 4c54 4920 636f   want the LTI co
-00000d90: 6e74 656e 7420 746f 206f 7065 6e20 696e  ntent to open in
-00000da0: 2061 6e20 4946 7261 6d65 2069 6e20 7468   an IFrame in th
-00000db0: 6520 6375 7272 656e 7420 7061 6765 2e20  e current page. 
-00000dc0: 5365 6c65 6374 204d 6f64 616c 2069 6620  Select Modal if 
-00000dd0: 796f 7520 7761 6e74 2074 6865 204c 5449  you want the LTI
-00000de0: 2063 6f6e 7465 6e74 2074 6f20 6f70 656e   content to open
-00000df0: 2069 6e20 6120 6d6f 6461 6c20 7769 6e64   in a modal wind
-00000e00: 6f77 2069 6e20 7468 6520 6375 7272 656e  ow in the curren
-00000e10: 7420 7061 6765 2e20 5365 6c65 6374 204e  t page. Select N
-00000e20: 6577 2057 696e 646f 7720 6966 2079 6f75  ew Window if you
-00000e30: 2077 616e 7420 7468 6520 4c54 4920 636f   want the LTI co
-00000e40: 6e74 656e 7420 746f 206f 7065 6e20 696e  ntent to open in
-00000e50: 2061 206e 6577 2062 726f 7773 6572 2077   a new browser w
-00000e60: 696e 646f 772e 2054 6869 7320 7365 7474  indow. This sett
-00000e70: 696e 6720 6973 206f 6e6c 7920 7573 6564  ing is only used
-00000e80: 2077 6865 6e20 4869 6465 2045 7874 6572   when Hide Exter
-00000e90: 6e61 6c20 546f 6f6c 2069 7320 7365 7420  nal Tool is set 
-00000ea0: 746f 2046 616c 7365 2e00 5365 6c65 6374  to False..Select
-00000eb0: 2054 7275 6520 6966 2074 6869 7320 636f   True if this co
-00000ec0: 6d70 6f6e 656e 7420 7769 6c6c 2072 6563  mponent will rec
-00000ed0: 6569 7665 2061 206e 756d 6572 6963 616c  eive a numerical
-00000ee0: 2073 636f 7265 2066 726f 6d20 7468 6520   score from the 
-00000ef0: 6578 7465 726e 616c 204c 5449 2073 7973  external LTI sys
-00000f00: 7465 6d2e 0053 656c 6563 7420 5472 7565  tem..Select True
-00000f10: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
-00000f20: 7573 6520 7468 6973 2063 6f6d 706f 6e65  use this compone
-00000f30: 6e74 2061 7320 6120 706c 6163 6568 6f6c  nt as a placehol
-00000f40: 6465 7220 666f 7220 7379 6e63 696e 6720  der for syncing 
-00000f50: 7769 7468 2061 6e20 6578 7465 726e 616c  with an external
-00000f60: 2067 7261 6469 6e67 2020 7379 7374 656d   grading  system
-00000f70: 2072 6174 6865 7220 7468 616e 206c 6175   rather than lau
-00000f80: 6e63 6820 616e 2065 7874 6572 6e61 6c20  nch an external 
-00000f90: 746f 6f6c 2e20 2054 6869 7320 7365 7474  tool.  This sett
-00000fa0: 696e 6720 6869 6465 7320 7468 6520 4c61  ing hides the La
-00000fb0: 756e 6368 2062 7574 746f 6e20 616e 6420  unch button and 
-00000fc0: 616e 7920 4946 7261 6d65 7320 666f 7220  any IFrames for 
-00000fd0: 7468 6973 2063 6f6d 706f 6e65 6e74 2e00  this component..
-00000fe0: 5365 6c65 6374 2054 7275 6520 746f 2061  Select True to a
-00000ff0: 6c6c 6f77 2074 6869 7264 2070 6172 7479  llow third party
-00001000: 2073 7973 7465 6d73 2074 6f20 706f 7374   systems to post
-00001010: 2067 7261 6465 7320 7061 7374 2074 6865   grades past the
-00001020: 2064 6561 646c 696e 652e 0053 656c 6563   deadline..Selec
-00001030: 7420 5472 7565 2074 6f20 7265 7175 6573  t True to reques
-00001040: 7420 7468 6520 7573 6572 2773 2065 6d61  t the user's ema
-00001050: 696c 2061 6464 7265 7373 2e00 5365 6c65  il address..Sele
-00001060: 6374 2054 7275 6520 746f 2072 6571 7565  ct True to reque
-00001070: 7374 2074 6865 2075 7365 7227 7320 7573  st the user's us
-00001080: 6572 6e61 6d65 2e00 5468 6520 7363 6f72  ername..The scor
-00001090: 6520 6b65 7074 2069 6e20 7468 6520 7862  e kept in the xb
-000010a0: 6c6f 636b 204b 5653 202d 2d20 6475 706c  lock KVS -- dupl
-000010b0: 6963 6174 6520 6f66 2074 6865 2070 7562  icate of the pub
-000010c0: 6c69 7368 6564 2073 636f 7265 2069 6e20  lished score in 
-000010d0: 646a 616e 676f 2044 4200 5b4c 5449 5d3a  django DB.[LTI]:
-000010e0: 2052 6561 6c20 7573 6572 206e 6f74 2066   Real user not f
-000010f0: 6f75 6e64 2061 6761 696e 7374 2061 6e6f  ound against ano
-00001100: 6e5f 6964 3a20 7b7d 0050 726f 6a65 6374  n_id: {}.Project
-00001110: 2d49 642d 5665 7273 696f 6e3a 2058 426c  -Id-Version: XBl
-00001120: 6f63 6b73 0a50 4f2d 5265 7669 7369 6f6e  ocks.PO-Revision
-00001130: 2d44 6174 653a 2032 3031 382d 3032 2d31  -Date: 2018-02-1
-00001140: 3620 3231 3a34 332b 3030 3030 0a4c 6173  6 21:43+0000.Las
-00001150: 742d 5472 616e 736c 6174 6f72 3a20 416c  t-Translator: Al
-00001160: 6265 6972 6f20 476f 6e7a 616c 657a 203c  beiro Gonzalez <
-00001170: 616c 6265 6972 6f2e 676f 6e7a 616c 657a  albeiro.gonzalez
-00001180: 4065 6475 6e65 7874 2e63 6f3e 0a4c 616e  @edunext.co>.Lan
-00001190: 6775 6167 652d 5465 616d 3a20 5370 616e  guage-Team: Span
-000011a0: 6973 6820 284c 6174 696e 2041 6d65 7269  ish (Latin Ameri
-000011b0: 6361 2920 2868 7474 703a 2f2f 7777 772e  ca) (http://www.
-000011c0: 7472 616e 7369 6665 782e 636f 6d2f 6f70  transifex.com/op
-000011d0: 656e 2d65 6478 2f78 626c 6f63 6b73 2f6c  en-edx/xblocks/l
-000011e0: 616e 6775 6167 652f 6573 5f34 3139 2f29  anguage/es_419/)
-000011f0: 0a4d 494d 452d 5665 7273 696f 6e3a 2031  .MIME-Version: 1
-00001200: 2e30 0a43 6f6e 7465 6e74 2d54 7970 653a  .0.Content-Type:
-00001210: 2074 6578 742f 706c 6169 6e3b 2063 6861   text/plain; cha
-00001220: 7273 6574 3d55 5446 2d38 0a43 6f6e 7465  rset=UTF-8.Conte
-00001230: 6e74 2d54 7261 6e73 6665 722d 456e 636f  nt-Transfer-Enco
-00001240: 6469 6e67 3a20 3862 6974 0a4c 616e 6775  ding: 8bit.Langu
-00001250: 6167 653a 2065 735f 3431 390a 506c 7572  age: es_419.Plur
-00001260: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
-00001270: 6c73 3d32 3b20 706c 7572 616c 3d28 6e20  ls=2; plural=(n 
-00001280: 213d 2031 293b 0a58 2d47 656e 6572 6174  != 1);.X-Generat
-00001290: 6f72 3a20 506f 6564 6974 2031 2e38 2e37  or: Poedit 1.8.7
-000012a0: 0a58 2d50 6f65 6469 742d 4261 7365 7061  .X-Poedit-Basepa
-000012b0: 7468 3a20 2e2e 2f2e 2e2f 2e2e 0a58 2d50  th: ../../...X-P
-000012c0: 6f65 6469 742d 5365 6172 6368 5061 7468  oedit-SearchPath
-000012d0: 2d30 3a20 6c74 695f 636f 6e73 756d 6572  -0: lti_consumer
-000012e0: 2e70 790a 0041 6365 7074 6172 206e 6f74  .py..Aceptar not
-000012f0: 6173 2064 6573 7075 c3a9 7320 6465 206c  as despu..s de l
-00001300: 6120 6665 6368 6120 6cc3 ad6d 6974 6500  a fecha l..mite.
-00001310: 4167 7265 6775 6520 656c 2070 6172 2063  Agregue el par c
-00001320: 6c61 7665 202f 2076 616c 6f72 2070 6172  lave / valor par
-00001330: 6120 6375 616c 7175 6965 7220 7061 72c3  a cualquier par.
-00001340: a16d 6574 726f 2070 6572 736f 6e61 6c69  .metro personali
-00001350: 7a61 646f 2c20 636f 6d6f 206c 6120 70c3  zado, como la p.
-00001360: a167 696e 6120 6120 6c61 2071 7565 2073  .gina a la que s
-00001370: 7520 6c69 6272 6f20 656c 6563 7472 c3b3  u libro electr..
-00001380: 6e69 636f 2064 6562 6520 6162 7269 7273  nico debe abrirs
-00001390: 6520 6f20 656c 2063 6f6c 6f72 2064 6520  e o el color de 
-000013a0: 666f 6e64 6f20 7061 7261 2065 7374 6520  fondo para este 
-000013b0: 636f 6d70 6f6e 656e 7465 2e20 456a 2e20  componente. Ej. 
-000013c0: 5b22 7061 6765 3d31 222c 2022 636f 6c6f  ["page=1", "colo
-000013d0: 723d 7768 6974 6522 5d3c 6272 202f 3e43  r=white"]<br />C
-000013e0: 6f6e 7375 6c74 6520 6c61 207b 646f 6373  onsulte la {docs
-000013f0: 5f61 6e63 686f 725f 6f70 656e 7d20 646f  _anchor_open} do
-00001400: 6375 6d65 6e74 6163 69c3 b36e 2064 6520  cumentaci..n de 
-00001410: 6564 5820 4c54 4920 7b61 6e63 686f 725f  edX LTI {anchor_
-00001420: 636c 6f73 657d 2070 6172 6120 6f62 7465  close} para obte
-00001430: 6e65 7220 6dc3 a173 2064 6574 616c 6c65  ner m..s detalle
-00001440: 7320 736f 6272 6520 6573 7461 2063 6f6e  s sobre esta con
-00001450: 6669 6775 7261 6369 c3b3 6e00 5465 7874  figuraci..n.Text
-00001460: 6f20 7061 7261 2065 6c20 626f 74c3 b36e  o para el bot..n
-00001470: 0045 6c20 636f 6d65 6e74 6172 696f 2074  .El comentario t
-00001480: 616c 2079 2063 6f6d 6f20 6675 6520 656e  al y como fue en
-00001490: 7669 6164 6f20 706f 7220 656c 2065 7661  viado por el eva
-000014a0: 6c75 6164 6f72 2c20 4c54 4932 2e30 2073  luador, LTI2.0 s
-000014b0: 7065 6300 4e6f 2073 6520 7075 646f 206f  pec.No se pudo o
-000014c0: 6274 656e 6572 2065 6c20 6964 2064 6520  btener el id de 
-000014d0: 7573 7561 7269 6f20 7061 7261 2065 7374  usuario para est
-000014e0: 6120 7065 7469 6369 c3b3 6e00 4e6f 2068  a petici..n.No h
-000014f0: 6120 7369 646f 2070 6f73 6962 6c65 206c  a sido posible l
-00001500: 6565 7220 656c 2070 6173 6170 6f72 7465  eer el pasaporte
-00001510: 204c 5449 3a20 7b6c 7469 5f70 6173 7370   LTI: {lti_passp
-00001520: 6f72 747d 2e20 4465 6265 72c3 ad61 2073  ort}. Deber..a s
-00001530: 6572 2075 6e61 2063 6164 656e 6120 2269  er una cadena "i
-00001540: 643a 6b65 793a 7365 6372 6574 222e 004e  d:key:secret"..N
-00001550: 6f20 7365 2070 7564 6f20 6c65 6572 2065  o se pudo leer e
-00001560: 6c20 7061 72c3 a16d 6574 726f 2070 6572  l par..metro per
-00001570: 736f 6e61 6c69 7a61 646f 3a20 7b63 7573  sonalizado: {cus
-00001580: 746f 6d5f 7061 7261 6d65 7465 727d 2e20  tom_parameter}. 
-00001590: 4465 6265 72c3 ad61 2073 6572 2075 6e61  Deber..a ser una
-000015a0: 2063 6164 656e 6120 2278 3d79 222e 0050   cadena "x=y"..P
-000015b0: 6172 c3a1 6d65 7472 6f73 2070 6572 736f  ar..metros perso
-000015c0: 6e61 6c69 7a61 646f 7300 4e6f 6d62 7265  nalizados.Nombre
-000015d0: 2061 206d 6f73 7472 6172 0050 726f 7665   a mostrar.Prove
-000015e0: 6120 756e 6120 6465 7363 7269 7063 69c3  a una descripci.
-000015f0: b36e 2064 6520 6c61 2061 706c 6963 6163  .n de la aplicac
-00001600: 69c3 b36e 2064 6520 756e 2074 6572 6365  i..n de un terce
-00001610: 726f 2e20 5369 2073 6520 736f 6c69 6369  ro. Si se solici
-00001620: 7461 2065 6c20 6e6f 6d62 7265 2064 656c  ta el nombre del
-00001630: 2075 7375 6172 696f 206f 2073 7520 636f   usuario o su co
-00001640: 7272 656f 2c20 7573 6520 6573 7465 2063  rreo, use este c
-00001650: 7561 6472 6f20 6465 2074 6578 746f 2070  uadro de texto p
-00001660: 6172 6120 696e 666f 726d 6172 2061 6c20  ara informar al 
-00001670: 7573 7561 7269 6f20 7175 6520 7375 206e  usuario que su n
-00001680: 6f6d 6272 6520 6465 2075 7375 6172 696f  ombre de usuario
-00001690: 2079 2073 7520 636f 7272 656f 2073 6572   y su correo ser
-000016a0: c3a1 6e20 7265 6469 7265 6363 696f 6e61  ..n redirecciona
-000016b0: 646f 7320 6120 756e 6120 6170 6c69 6361  dos a una aplica
-000016c0: 6369 c3b3 6e20 6465 2075 6e20 7465 7263  ci..n de un terc
-000016d0: 6572 6f2e 0049 6e74 726f 6475 7a63 6120  ero..Introduzca 
-000016e0: 656c 2049 4420 4c54 4920 7061 7261 2065  el ID LTI para e
-000016f0: 6c20 7072 6f76 6565 646f 7220 4c54 4920  l proveedor LTI 
-00001700: 6578 7465 726e 6f2e 2045 7374 6520 7661  externo. Este va
-00001710: 6c6f 7220 6465 6265 2073 6572 2065 6c20  lor debe ser el 
-00001720: 6d69 736d 6f20 4944 204c 5449 2071 7565  mismo ID LTI que
-00001730: 2069 6e67 7265 73c3 b320 656e 206c 6120   ingres.. en la 
-00001740: 636f 6e66 6967 7572 6163 69c3 b36e 2064  configuraci..n d
-00001750: 6520 5061 7361 706f 7274 6573 204c 5449  e Pasaportes LTI
-00001760: 2065 6e20 6c61 2070 c3a1 6769 6e61 2043   en la p..gina C
-00001770: 6f6e 6669 6775 7261 6369 c3b3 6e20 6176  onfiguraci..n av
-00001780: 616e 7a61 6461 2e3c 6272 202f 3e43 6f6e  anzada.<br />Con
-00001790: 7375 6c74 6520 6c61 207b 646f 6373 5f61  sulte la {docs_a
-000017a0: 6e63 686f 725f 6f70 656e 7d20 646f 6375  nchor_open} docu
-000017b0: 6d65 6e74 6163 69c3 b36e 2064 6520 6564  mentaci..n de ed
-000017c0: 5820 4c54 4920 7b61 6e63 686f 725f 636c  X LTI {anchor_cl
-000017d0: 6f73 657d 2070 6172 6120 6f62 7465 6e65  ose} para obtene
-000017e0: 7220 6dc3 a173 2064 6574 616c 6c65 7320  r m..s detalles 
-000017f0: 736f 6272 6520 6573 7461 2063 6f6e 6669  sobre esta confi
-00001800: 6775 7261 6369 c3b3 6e2e 0049 6e67 7265  guraci..n..Ingre
-00001810: 7365 206c 6120 5552 4c20 6465 206c 6120  se la URL de la 
-00001820: 6865 7272 616d 6965 6e74 6120 6578 7465  herramienta exte
-00001830: 726e 6120 7175 6520 6573 7465 2063 6f6d  rna que este com
-00001840: 706f 6e65 6e74 6520 696e 6963 6961 2e20  ponente inicia. 
-00001850: 4573 7461 2063 6f6e 6669 6775 7261 6369  Esta configuraci
-00001860: c3b3 6e20 73c3 b36c 6f20 7365 2075 7469  ..n s..lo se uti
-00001870: 6c69 7a61 2063 7561 6e64 6f20 4f63 756c  liza cuando Ocul
-00001880: 7461 7220 6865 7272 616d 6965 6e74 6120  tar herramienta 
-00001890: 6578 7465 726e 6120 7365 2065 7374 6162  externa se estab
-000018a0: 6c65 6365 2065 6e20 4661 6c73 6f2e 3c62  lece en Falso.<b
-000018b0: 7220 2f3e 436f 6e73 756c 7465 206c 6120  r />Consulte la 
-000018c0: 7b64 6f63 735f 616e 6368 6f72 5f6f 7065  {docs_anchor_ope
-000018d0: 6e7d 2064 6f63 756d 656e 7461 6369 c3b3  n} documentaci..
-000018e0: 6e20 6465 2065 6458 204c 5449 207b 616e  n de edX LTI {an
-000018f0: 6368 6f72 5f63 6c6f 7365 7d20 7061 7261  chor_close} para
-00001900: 206f 6274 656e 6572 206d c3a1 7320 6465   obtener m..s de
-00001910: 7461 6c6c 6573 2073 6f62 7265 2065 7374  talles sobre est
-00001920: 6120 636f 6e66 6967 7572 6163 69c3 b36e  a configuraci..n
-00001930: 2e00 496e 7472 6f64 757a 6361 206c 6120  ..Introduzca la 
-00001940: 616c 7475 7261 2065 6e20 70c3 ad78 656c  altura en p..xel
-00001950: 6573 2064 6573 6561 6461 2064 656c 2069  es deseada del i
-00001960: 6672 616d 6520 7175 6520 636f 6e74 656e  frame que conten
-00001970: 6472 c3a1 206c 6120 6865 7272 616d 6965  dr.. la herramie
-00001980: 6e74 6120 4c54 492e 2045 7374 6120 6f70  nta LTI. Esta op
-00001990: 6369 c3b3 6e20 73c3 b36c 6f20 7365 2075  ci..n s..lo se u
-000019a0: 7469 6c69 7a61 2063 7561 6e64 6f20 4f63  tiliza cuando Oc
-000019b0: 756c 7461 7220 6865 7272 616d 6965 6e74  ultar herramient
-000019c0: 6120 6578 7465 726e 6120 7365 2065 7374  a externa se est
-000019d0: 6162 6c65 6365 2065 6e20 4661 6c73 6520  ablece en False 
-000019e0: 7920 5461 7267 6574 2070 6172 6120 656c  y Target para el
-000019f0: 204c 5449 2073 6520 6573 7461 626c 6563   LTI se establec
-00001a00: 6520 656e 2049 6e6c 696e 652e 0049 6e67  e en Inline..Ing
-00001a10: 7265 7365 206c 6120 616c 7475 7261 2064  rese la altura d
-00001a20: 6520 706f 7263 656e 7461 6a65 2064 6520  e porcentaje de 
-00001a30: 7669 7375 616c 697a 6163 69c3 b36e 2064  visualizaci..n d
-00001a40: 6573 6561 6461 2064 6520 6c61 2073 7570  eseada de la sup
-00001a50: 6572 706f 7369 6369 c3b3 6e20 6d6f 6461  erposici..n moda
-00001a60: 6c20 7175 6520 636f 6e74 656e 6472 c3a1  l que contendr..
-00001a70: 206c 6120 6865 7272 616d 6965 6e74 6120   la herramienta 
-00001a80: 4c54 492e 2045 7374 6120 6f70 6369 c3b3  LTI. Esta opci..
-00001a90: 6e20 73c3 b36c 6f20 7365 2075 7469 6c69  n s..lo se utili
-00001aa0: 7a61 2063 7561 6e64 6f20 4f63 756c 7461  za cuando Oculta
-00001ab0: 7220 6865 7272 616d 6965 6e74 6120 6578  r herramienta ex
-00001ac0: 7465 726e 6120 7365 2065 7374 6162 6c65  terna se estable
-00001ad0: 6365 2065 6e20 4661 6c73 6520 7920 5461  ce en False y Ta
-00001ae0: 7267 6574 2070 6172 6120 656c 204c 5449  rget para el LTI
-00001af0: 2073 6520 6573 7461 626c 6563 6520 656e   se establece en
-00001b00: 204d 6f64 616c 2e00 496e 6772 6573 6520   Modal..Ingrese 
-00001b10: 656c 2061 6e63 686f 2064 6520 706f 7263  el ancho de porc
-00001b20: 656e 7461 6a65 2064 6520 6c61 2076 656e  entaje de la ven
-00001b30: 7461 6e61 2064 6520 7669 7375 616c 697a  tana de visualiz
-00001b40: 6163 69c3 b36e 2064 6520 6c61 2073 7570  aci..n de la sup
-00001b50: 6572 706f 7369 6369 c3b3 6e20 6d6f 6461  erposici..n moda
-00001b60: 6c20 7175 6520 636f 6e74 656e 6472 c3a1  l que contendr..
-00001b70: 206c 6120 6865 7272 616d 6965 6e74 6120   la herramienta 
-00001b80: 4c54 492e 2045 7374 6120 6f70 6369 c3b3  LTI. Esta opci..
-00001b90: 6e20 73c3 b36c 6f20 7365 2075 7469 6c69  n s..lo se utili
-00001ba0: 7a61 2063 7561 6e64 6f20 4f63 756c 7461  za cuando Oculta
-00001bb0: 7220 6865 7272 616d 6965 6e74 6120 6578  r herramienta ex
-00001bc0: 7465 726e 6120 7365 2065 7374 6162 6c65  terna se estable
-00001bd0: 6365 2065 6e20 4661 6c73 6520 7920 5461  ce en False y Ta
-00001be0: 7267 6574 2070 6172 6120 656c 204c 5449  rget para el LTI
-00001bf0: 2073 6520 6573 7461 626c 6563 6520 656e   se establece en
-00001c00: 204d 6f64 616c 2e00 496e 6772 6573 6520   Modal..Ingrese 
-00001c10: 656c 206e 6f6d 6272 6520 7175 6520 6c6f  el nombre que lo
-00001c20: 7320 6573 7475 6469 616e 7465 7320 7665  s estudiantes ve
-00001c30: 72c3 a16e 2070 6172 6120 6573 7465 2063  r..n para este c
-00001c40: 6f6d 706f 6e65 6e74 652e 204c 6f73 2072  omponente. Los r
-00001c50: 6570 6f72 7465 7320 6465 2041 6e61 6c79  eportes de Analy
-00001c60: 7469 6373 2074 616d 6269 c3a9 6e20 7075  tics tambi..n pu
-00001c70: 6564 656e 2075 7469 6c69 7a61 7220 656c  eden utilizar el
-00001c80: 206e 6f6d 6272 6520 7061 7261 206d 6f73   nombre para mos
-00001c90: 7472 6172 2070 6172 6120 6964 656e 7469  trar para identi
-00001ca0: 6669 6361 7220 6573 7465 2063 6f6d 706f  ficar este compo
-00001cb0: 6e65 6e74 652e 0049 6e67 7265 7365 2065  nente..Ingrese e
-00001cc0: 6c20 6ec3 ba6d 6572 6f20 6465 2070 756e  l n..mero de pun
-00001cd0: 746f 7320 706f 7369 626c 6573 2070 6172  tos posibles par
-00001ce0: 6120 6573 7465 2063 6f6d 706f 6e65 6e74  a este component
-00001cf0: 652e 2045 6c20 7661 6c6f 7220 706f 7220  e. El valor por 
-00001d00: 6465 6665 6374 6f20 6573 2031 2e30 2e20  defecto es 1.0. 
-00001d10: 4573 7465 2076 616c 6f72 2073 6f6c 6f20  Este valor solo 
-00001d20: 7365 2075 7469 6c69 7a61 2063 7561 6e64  se utiliza cuand
-00001d30: 6f20 656c 2070 6172 c3a1 6d65 7472 6f20  o el par..metro 
-00001d40: 6465 2063 616c 6966 6963 6163 69c3 b36e  de calificaci..n
-00001d50: 2065 7374 c3a1 2064 6566 696e 6964 6f20   est.. definido 
-00001d60: 636f 6d6f 2054 7275 652e 0049 6e67 7265  como True..Ingre
-00001d70: 7365 2065 6c20 7465 7874 6f20 656e 2065  se el texto en e
-00001d80: 6c20 626f 74c3 b36e 2075 7361 646f 2070  l bot..n usado p
-00001d90: 6172 6120 696e 6963 6961 7220 6c61 2061  ara iniciar la a
-00001da0: 706c 6963 6163 69c3 b36e 2064 6520 7465  plicaci..n de te
-00001db0: 7263 6572 6f73 2e20 4573 7461 206f 7063  rceros. Esta opc
-00001dc0: 69c3 b36e 2073 c3b3 6c6f 2073 6520 7574  i..n s..lo se ut
-00001dd0: 696c 697a 6120 6375 616e 646f 204f 6375  iliza cuando Ocu
-00001de0: 6c74 6172 2068 6572 7261 6d69 656e 7461  ltar herramienta
-00001df0: 2065 7874 6572 6e61 2073 6520 6573 7461   externa se esta
-00001e00: 626c 6563 6520 656e 2046 616c 736f 2079  blece en Falso y
-00001e10: 2065 6c20 5461 7267 6574 2070 6172 6120   el Target para 
-00001e20: 656c 204c 5449 2073 6520 6573 7461 626c  el LTI se establ
-00001e30: 6563 6520 656e 204d 6f64 616c 206f 204e  ece en Modal o N
-00001e40: 7565 7661 2056 656e 7461 6e61 2e00 4f63  ueva Ventana..Oc
-00001e50: 756c 7461 7220 6c61 2068 6572 7261 6d69  ultar la herrami
-00001e60: 656e 7461 2065 7874 6572 6e61 0041 6c74  enta externa.Alt
-00001e70: 7572 6120 496e 6c69 6e65 0049 6e66 6f72  ura Inline.Infor
-00001e80: 6d61 6369 c3b3 6e20 736f 6272 6520 6c61  maci..n sobre la
-00001e90: 2061 706c 6963 6163 69c3 b36e 204c 5449   aplicaci..n LTI
-00001ea0: 0043 6f6e 7375 6d69 646f 7220 4c54 4900  .Consumidor LTI.
-00001eb0: 4944 2064 6520 4c54 4900 5461 7267 6574  ID de LTI.Target
-00001ec0: 2070 6172 6120 656c 204c 5449 0055 524c   para el LTI.URL
-00001ed0: 2064 6520 4c54 4900 416c 7475 7261 2064   de LTI.Altura d
-00001ee0: 656c 206d 6f64 616c 0041 6e63 686f 2064  el modal.Ancho d
-00001ef0: 656c 206d 6f64 616c 004e 6f20 7365 2065  el modal.No se e
-00001f00: 6e63 6f6e 7472 c3b3 2075 6e20 6964 2064  ncontr.. un id d
-00001f10: 6520 7573 7561 7269 6f20 76c3 a16c 6964  e usuario v..lid
-00001f20: 6f20 656e 2065 6c20 5552 4c20 6465 6c20  o en el URL del 
-00001f30: 656e 6470 6f69 6e74 0053 6f6c 6963 6974  endpoint.Solicit
-00001f40: 6172 206c 6120 6469 7265 6363 69c3 b36e  ar la direcci..n
-00001f50: 2064 6520 636f 7272 656f 2064 656c 2075   de correo del u
-00001f60: 7375 6172 696f 0053 6f6c 6963 6974 6520  suario.Solicite 
-00001f70: 656c 206e 6f6d 6272 6520 70c3 ba62 6c69  el nombre p..bli
-00001f80: 636f 2064 656c 2075 7375 6172 696f 0050  co del usuario.P
-00001f90: 756e 7475 6164 6f00 5365 6c65 6363 696f  untuado.Seleccio
-00001fa0: 6e65 2049 6e6c 696e 6520 7369 2064 6573  ne Inline si des
-00001fb0: 6561 2071 7565 2065 6c20 636f 6e74 656e  ea que el conten
-00001fc0: 6964 6f20 4c54 4920 7365 2061 6272 6120  ido LTI se abra 
-00001fd0: 656e 2075 6e20 4946 7261 6d65 2065 6e20  en un IFrame en 
-00001fe0: 6c61 2070 c3a1 6769 6e61 2061 6374 7561  la p..gina actua
-00001ff0: 6c2e 2053 656c 6563 6369 6f6e 6520 4d6f  l. Seleccione Mo
-00002000: 6461 6c20 7369 2064 6573 6561 2071 7565  dal si desea que
-00002010: 2065 6c20 636f 6e74 656e 6964 6f20 4c54   el contenido LT
-00002020: 4920 7365 2061 6272 6120 656e 2075 6e61  I se abra en una
-00002030: 2076 656e 7461 6e61 206d 6f64 616c 2065   ventana modal e
-00002040: 6e20 6c61 2070 c3a1 6769 6e61 2061 6374  n la p..gina act
-00002050: 7561 6c2e 2053 656c 6563 6369 6f6e 6520  ual. Seleccione 
-00002060: 4e75 6576 6120 7665 6e74 616e 6120 7369  Nueva ventana si
-00002070: 2064 6573 6561 2071 7565 2065 6c20 636f   desea que el co
-00002080: 6e74 656e 6964 6f20 4c54 4920 7365 2061  ntenido LTI se a
-00002090: 6272 6120 656e 2075 6e61 206e 7565 7661  bra en una nueva
-000020a0: 2076 656e 7461 6e61 2064 656c 206e 6176   ventana del nav
-000020b0: 6567 6164 6f72 2e20 4573 7461 2063 6f6e  egador. Esta con
-000020c0: 6669 6775 7261 6369 c3b3 6e20 73c3 b36c  figuraci..n s..l
-000020d0: 6f20 7365 2075 7469 6c69 7a61 2063 7561  o se utiliza cua
-000020e0: 6e64 6f20 4f63 756c 7461 7220 6865 7272  ndo Ocultar herr
-000020f0: 616d 6965 6e74 6120 6578 7465 726e 6120  amienta externa 
-00002100: 7365 2065 7374 6162 6c65 6365 2065 6e20  se establece en 
-00002110: 4661 6c73 6f2e 0053 656c 6563 6369 6f6e  Falso..Seleccion
-00002120: 6520 5472 7565 2073 6920 6573 7465 2063  e True si este c
-00002130: 6f6d 706f 6e65 6e74 6520 7265 6369 6269  omponente recibi
-00002140: 72c3 a120 756e 6120 7075 6e74 7561 6369  r.. una puntuaci
-00002150: c3b3 6e20 6e75 6dc3 a972 6963 6120 6465  ..n num..rica de
-00002160: 7364 6520 756e 2073 6973 7465 6d61 204c  sde un sistema L
-00002170: 5449 2065 7874 6572 6e6f 2e00 5365 6c65  TI externo..Sele
-00002180: 6363 696f 6e65 2054 7275 6520 7369 2064  ccione True si d
-00002190: 6573 6561 2075 7361 7220 6573 7465 2063  esea usar este c
-000021a0: 6f6d 706f 6e65 6e74 6520 636f 6d6f 206d  omponente como m
-000021b0: 6172 6361 646f 7220 7061 7261 2073 696e  arcador para sin
-000021c0: 6372 6f6e 697a 6172 7365 2063 6f6e 2075  cronizarse con u
-000021d0: 6e20 7365 7276 6963 696f 2065 7874 6572  n servicio exter
-000021e0: 6e6f 2065 6e20 6c75 6761 7220 6465 206c  no en lugar de l
-000021f0: 616e 7a61 7220 756e 6120 6865 7272 616d  anzar una herram
-00002200: 6965 6e74 6120 6578 7465 726e 612e 2045  ienta externa. E
-00002210: 7374 6120 6f70 6369 c3b3 6e20 6f63 756c  sta opci..n ocul
-00002220: 7461 2065 6c20 626f 74c3 b36e 2064 6520  ta el bot..n de 
-00002230: 4c61 6e7a 6172 2079 2063 7561 6c71 7569  Lanzar y cualqui
-00002240: 6572 2069 6672 616d 6520 7061 7261 2065  er iframe para e
-00002250: 7374 6520 636f 6d70 6f6e 656e 7465 2e00  ste componente..
-00002260: 5365 6c65 6363 696f 6e65 2054 7275 6520  Seleccione True 
-00002270: 7061 7261 2070 6572 6d69 7469 7220 7175  para permitir qu
-00002280: 6520 7369 7374 656d 6173 2064 6520 7465  e sistemas de te
-00002290: 7263 6572 6f73 2070 7562 6c69 7175 656e  rceros publiquen
-000022a0: 2063 616c 6966 6963 6163 696f 6e65 7320   calificaciones 
-000022b0: 6465 7370 75c3 a973 2064 6520 6c61 2066  despu..s de la f
-000022c0: 6563 6861 206c c3ad 6d69 7465 2e00 5365  echa l..mite..Se
-000022d0: 6c65 6363 696f 6e65 2054 7275 6520 7061  leccione True pa
-000022e0: 7261 2073 6f6c 6963 6974 6172 2065 6c20  ra solicitar el 
-000022f0: 636f 7272 656f 2065 6c65 6374 72c3 b36e  correo electr..n
-00002300: 6963 6f20 6465 6c20 7573 7561 7269 6f2e  ico del usuario.
-00002310: 0053 656c 6563 6369 6f6e 6520 5472 7565  .Seleccione True
-00002320: 2070 6172 6120 736f 6c69 6369 7461 7220   para solicitar 
-00002330: 656c 206e 6f6d 6272 6520 6465 2075 7375  el nombre de usu
-00002340: 6172 696f 2e00 4c61 2063 616c 6966 6963  ario..La calific
-00002350: 6163 69c3 b36e 2061 6c6d 6163 656e 6164  aci..n almacenad
-00002360: 6120 656e 2078 626c 6f63 6b20 4b56 5320  a en xblock KVS 
-00002370: 2d2d 2075 6e20 6475 706c 6963 6164 6f20  -- un duplicado 
-00002380: 6465 206c 6120 6361 6c69 6669 6361 6369  de la calificaci
-00002390: c3b3 6e20 7075 626c 6963 6164 6120 656e  ..n publicada en
-000023a0: 2064 6a61 6e67 6f20 4442 005b 4c54 495d   django DB.[LTI]
-000023b0: 3a20 4e6f 2073 6520 656e 636f 6e74 72c3  : No se encontr.
-000023c0: b320 756e 2075 7375 6172 696f 2071 7565  . un usuario que
-000023d0: 2063 6f69 6e63 6964 6965 7261 2063 6f6e   coincidiera con
-000023e0: 2061 6e6f 6e5f 6964 3a20 7b7d 00          anon_id: {}.
+00000000: 2320 0a23 2054 7261 6e73 6c61 746f 7273  # .# Translators
+00000010: 3a0a 2320 5069 6572 7265 204d 6169 6c68  :.# Pierre Mailh
+00000020: 6f74 203c 7069 6572 7265 2e6d 6169 6c68  ot <pierre.mailh
+00000030: 6f74 4067 6d61 696c 2e63 6f6d 3e2c 2032  ot@gmail.com>, 2
+00000040: 3031 390a 6d73 6769 6420 2222 0a6d 7367  019.msgid "".msg
+00000050: 7374 7220 2222 0a22 5072 6f6a 6563 742d  str ""."Project-
+00000060: 4964 2d56 6572 7369 6f6e 3a20 5842 6c6f  Id-Version: XBlo
+00000070: 636b 735c 6e22 0a22 504f 542d 4372 6561  cks\n"."POT-Crea
+00000080: 7469 6f6e 2d44 6174 653a 2032 3031 362d  tion-Date: 2016-
+00000090: 3033 2d31 3820 3135 3a30 392b 3035 3030  03-18 15:09+0500
+000000a0: 5c6e 220a 2250 4f2d 5265 7669 7369 6f6e  \n"."PO-Revision
+000000b0: 2d44 6174 653a 2032 3031 392d 3038 2d32  -Date: 2019-08-2
+000000c0: 3620 3232 3a30 312b 3030 3030 5c6e 220a  6 22:01+0000\n".
+000000d0: 224c 6173 742d 5472 616e 736c 6174 6f72  "Last-Translator
+000000e0: 3a20 5069 6572 7265 204d 6169 6c68 6f74  : Pierre Mailhot
+000000f0: 203c 7069 6572 7265 2e6d 6169 6c68 6f74   <pierre.mailhot
+00000100: 4067 6d61 696c 2e63 6f6d 3e5c 6e22 0a22  @gmail.com>\n"."
+00000110: 4c61 6e67 7561 6765 2d54 6561 6d3a 2046  Language-Team: F
+00000120: 7265 6e63 6820 2843 616e 6164 6129 2028  rench (Canada) (
+00000130: 6874 7470 3a2f 2f77 7777 2e74 7261 6e73  http://www.trans
+00000140: 6966 6578 2e63 6f6d 2f6f 7065 6e2d 6564  ifex.com/open-ed
+00000150: 782f 7862 6c6f 636b 732f 6c61 6e67 7561  x/xblocks/langua
+00000160: 6765 2f66 725f 4341 2f29 5c6e 220a 224d  ge/fr_CA/)\n"."M
+00000170: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
+00000180: 5c6e 220a 2243 6f6e 7465 6e74 2d54 7970  \n"."Content-Typ
+00000190: 653a 2074 6578 742f 706c 6169 6e3b 2063  e: text/plain; c
+000001a0: 6861 7273 6574 3d55 5446 2d38 5c6e 220a  harset=UTF-8\n".
+000001b0: 2243 6f6e 7465 6e74 2d54 7261 6e73 6665  "Content-Transfe
+000001c0: 722d 456e 636f 6469 6e67 3a20 3862 6974  r-Encoding: 8bit
+000001d0: 5c6e 220a 224c 616e 6775 6167 653a 2066  \n"."Language: f
+000001e0: 725f 4341 5c6e 220a 2250 6c75 7261 6c2d  r_CA\n"."Plural-
+000001f0: 466f 726d 733a 206e 706c 7572 616c 733d  Forms: nplurals=
+00000200: 323b 2070 6c75 7261 6c3d 286e 203e 2031  2; plural=(n > 1
+00000210: 293b 5c6e 220a 2258 2d47 656e 6572 6174  );\n"."X-Generat
+00000220: 6f72 3a20 506f 6564 6974 2031 2e38 2e37  or: Poedit 1.8.7
+00000230: 5c6e 220a 2258 2d50 6f65 6469 742d 4261  \n"."X-Poedit-Ba
+00000240: 7365 7061 7468 3a20 2e2e 2f2e 2e2f 2e2e  sepath: ../../..
+00000250: 5c6e 220a 2258 2d50 6f65 6469 742d 5365  \n"."X-Poedit-Se
+00000260: 6172 6368 5061 7468 2d30 3a20 6c74 695f  archPath-0: lti_
+00000270: 636f 6e73 756d 6572 2e70 795c 6e22 0a0a  consumer.py\n"..
+00000280: 233a 206c 7469 5f63 6f6e 7375 6d65 722e  #: lti_consumer.
+00000290: 7079 0a6d 7367 6964 2022 4e6f 2076 616c  py.msgid "No val
+000002a0: 6964 2075 7365 7220 6964 2066 6f75 6e64  id user id found
+000002b0: 2069 6e20 656e 6470 6f69 6e74 2055 524c   in endpoint URL
+000002c0: 220a 6d73 6773 7472 2022 4175 6375 6e20  ".msgstr "Aucun 
+000002d0: 4944 2075 7469 6c69 7361 7465 7572 2076  ID utilisateur v
+000002e0: 616c 6964 6520 7472 6f75 76c3 a920 6461  alide trouv.. da
+000002f0: 6e73 206c 2755 524c 2063 6962 6c65 220a  ns l'URL cible".
+00000300: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00000310: 2e70 790a 6d73 6769 6420 2244 6973 706c  .py.msgid "Displ
+00000320: 6179 204e 616d 6522 0a6d 7367 7374 7220  ay Name".msgstr 
+00000330: 224e 6f6d 2064 2761 6666 6963 6861 6765  "Nom d'affichage
+00000340: 220a 0a23 3a20 6c74 695f 636f 6e73 756d  "..#: lti_consum
+00000350: 6572 2e70 790a 6d73 6769 6420 2222 0a22  er.py.msgid ""."
+00000360: 456e 7465 7220 7468 6520 6e61 6d65 2074  Enter the name t
+00000370: 6861 7420 7374 7564 656e 7473 2073 6565  hat students see
+00000380: 2066 6f72 2074 6869 7320 636f 6d70 6f6e   for this compon
+00000390: 656e 742e 2041 6e61 6c79 7469 6373 2072  ent. Analytics r
+000003a0: 6570 6f72 7473 206d 6179 2022 0a22 616c  eports may "."al
+000003b0: 736f 2075 7365 2074 6865 2064 6973 706c  so use the displ
+000003c0: 6179 206e 616d 6520 746f 2069 6465 6e74  ay name to ident
+000003d0: 6966 7920 7468 6973 2063 6f6d 706f 6e65  ify this compone
+000003e0: 6e74 2e22 0a6d 7367 7374 7220 2245 6e74  nt.".msgstr "Ent
+000003f0: 7265 7a20 6c65 206e 6f6d 2071 7565 206c  rez le nom que l
+00000400: 6573 20c3 a974 7564 6961 6e74 7320 766f  es ..tudiants vo
+00000410: 6965 6e74 2070 6f75 7220 6365 2063 6f6d  ient pour ce com
+00000420: 706f 7361 6e74 2e20 4c65 7320 7261 7070  posant. Les rapp
+00000430: 6f72 7473 2064 2761 6e61 6c79 7365 2070  orts d'analyse p
+00000440: 6575 7665 6e74 20c3 a967 616c 656d 656e  euvent ..galemen
+00000450: 7420 7574 696c 6973 6572 206c 6520 6e6f  t utiliser le no
+00000460: 6d20 6427 6166 6669 6368 6167 6520 706f  m d'affichage po
+00000470: 7572 2069 6465 6e74 6966 6965 7220 6365  ur identifier ce
+00000480: 2063 6f6d 706f 7361 6e74 2e22 0a0a 233a   composant."..#:
+00000490: 206c 7469 5f63 6f6e 7375 6d65 722e 7079   lti_consumer.py
+000004a0: 0a6d 7367 6964 2022 4c54 4920 436f 6e73  .msgid "LTI Cons
+000004b0: 756d 6572 220a 6d73 6773 7472 2022 436f  umer".msgstr "Co
+000004c0: 6e73 6f6d 6d61 7465 7572 204c 5449 220a  nsommateur LTI".
+000004d0: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+000004e0: 2e70 793a 3235 360a 6d73 6769 6420 224c  .py:256.msgid "L
+000004f0: 5449 2041 7070 6c69 6361 7469 6f6e 2049  TI Application I
+00000500: 6e66 6f72 6d61 7469 6f6e 220a 6d73 6773  nformation".msgs
+00000510: 7472 2022 496e 666f 726d 6174 696f 6e20  tr "Information 
+00000520: c3a0 2070 726f 706f 7320 6465 206c 2761  .. propos de l'a
+00000530: 7070 6c69 6361 7469 6f6e 204c 5449 220a  pplication LTI".
+00000540: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00000550: 2e70 790a 6d73 6769 6420 2222 0a22 456e  .py.msgid ""."En
+00000560: 7465 7220 6120 6465 7363 7269 7074 696f  ter a descriptio
+00000570: 6e20 6f66 2074 6865 2074 6869 7264 2070  n of the third p
+00000580: 6172 7479 2061 7070 6c69 6361 7469 6f6e  arty application
+00000590: 2e20 4966 2072 6571 7565 7374 696e 6720  . If requesting 
+000005a0: 7573 6572 6e61 6d65 2022 0a22 616e 642f  username "."and/
+000005b0: 6f72 2065 6d61 696c 2c20 7573 6520 7468  or email, use th
+000005c0: 6973 2074 6578 7420 626f 7820 746f 2069  is text box to i
+000005d0: 6e66 6f72 6d20 7573 6572 7320 7768 7920  nform users why 
+000005e0: 7468 6569 7220 7573 6572 6e61 6d65 2061  their username a
+000005f0: 6e64 2f6f 7220 220a 2265 6d61 696c 2077  nd/or "."email w
+00000600: 696c 6c20 6265 2066 6f72 7761 7264 6564  ill be forwarded
+00000610: 2074 6f20 6120 7468 6972 6420 7061 7274   to a third part
+00000620: 7920 6170 706c 6963 6174 696f 6e2e 220a  y application.".
+00000630: 6d73 6773 7472 2022 456e 7472 6572 2075  msgstr "Entrer u
+00000640: 6e65 2064 6573 6372 6970 7469 6f6e 2064  ne description d
+00000650: 6520 6c27 6170 706c 6963 6174 696f 6e20  e l'application 
+00000660: 7469 6572 6365 2e20 5369 2076 6f75 7320  tierce. Si vous 
+00000670: 6465 6d61 6e64 657a 206c 6520 6e6f 6d20  demandez le nom 
+00000680: 6427 7574 696c 6973 6174 6575 7220 6574  d'utilisateur et
+00000690: 2f6f 7520 636f 7572 7269 656c 2c20 7574  /ou courriel, ut
+000006a0: 696c 6973 657a 2063 6574 7465 2062 6fc3  ilisez cette bo.
+000006b0: ae74 6520 6465 2064 6961 6c6f 6775 6520  .te de dialogue 
+000006c0: 706f 7572 2069 6e66 6f72 6d65 7220 6c65  pour informer le
+000006d0: 7320 7574 696c 6973 6174 6575 7273 2070  s utilisateurs p
+000006e0: 6f75 7271 756f 6920 6c65 7572 206e 6f6d  ourquoi leur nom
+000006f0: 2064 2775 7469 6c69 7361 7465 7572 2065   d'utilisateur e
+00000700: 742f 6f75 2063 6f75 7272 6965 6c20 7365  t/ou courriel se
+00000710: 726f 6e74 2074 7261 6e73 6d69 7320 c3a0  ront transmis ..
+00000720: 2075 6e65 2061 7070 6c69 6361 7469 6f6e   une application
+00000730: 2074 6965 7263 652e 220a 0a23 3a20 6c74   tierce."..#: lt
+00000740: 695f 636f 6e73 756d 6572 2e70 790a 6d73  i_consumer.py.ms
+00000750: 6769 6420 224c 5449 2049 4422 0a6d 7367  gid "LTI ID".msg
+00000760: 7374 7220 2249 6465 6e74 6966 6961 6e74  str "Identifiant
+00000770: 204c 5449 220a 0a23 3a20 6c74 695f 636f   LTI"..#: lti_co
+00000780: 6e73 756d 6572 2e70 790a 232c 2070 7974  nsumer.py.#, pyt
+00000790: 686f 6e2d 6272 6163 652d 666f 726d 6174  hon-brace-format
+000007a0: 0a6d 7367 6964 2022 220a 2245 6e74 6572  .msgid ""."Enter
+000007b0: 2074 6865 204c 5449 2049 4420 666f 7220   the LTI ID for 
+000007c0: 7468 6520 6578 7465 726e 616c 204c 5449  the external LTI
+000007d0: 2070 726f 7669 6465 722e 2054 6869 7320   provider. This 
+000007e0: 7661 6c75 6520 6d75 7374 2062 6520 7468  value must be th
+000007f0: 6520 7361 6d65 2022 0a22 4c54 4920 4944  e same "."LTI ID
+00000800: 2074 6861 7420 796f 7520 656e 7465 7265   that you entere
+00000810: 6420 696e 2074 6865 204c 5449 2050 6173  d in the LTI Pas
+00000820: 7370 6f72 7473 2073 6574 7469 6e67 206f  sports setting o
+00000830: 6e20 7468 6520 4164 7661 6e63 6564 2022  n the Advanced "
+00000840: 0a22 5365 7474 696e 6773 2070 6167 652e  ."Settings page.
+00000850: 3c62 7220 2f3e 5365 6520 7468 6520 7b64  <br />See the {d
+00000860: 6f63 735f 616e 6368 6f72 5f6f 7065 6e7d  ocs_anchor_open}
+00000870: 6564 5820 4c54 4920 220a 2264 6f63 756d  edX LTI "."docum
+00000880: 656e 7461 7469 6f6e 7b61 6e63 686f 725f  entation{anchor_
+00000890: 636c 6f73 657d 2066 6f72 206d 6f72 6520  close} for more 
+000008a0: 6465 7461 696c 7320 6f6e 2074 6869 7320  details on this 
+000008b0: 7365 7474 696e 672e 220a 6d73 6773 7472  setting.".msgstr
+000008c0: 2022 456e 7472 657a 206c 2749 4420 4c54   "Entrez l'ID LT
+000008d0: 4920 6475 2066 6f75 726e 6973 7365 7572  I du fournisseur
+000008e0: 204c 5449 2065 7874 6572 6e65 2e20 4365   LTI externe. Ce
+000008f0: 7474 6520 7661 6c65 7572 2064 6f69 7420  tte valeur doit 
+00000900: c3aa 7472 6520 6964 656e 7469 7175 6520  ..tre identique 
+00000910: c3a0 206c 2749 4420 4c54 4920 7175 6520  .. l'ID LTI que 
+00000920: 766f 7573 2061 7665 7a20 656e 7472 c3a9  vous avez entr..
+00000930: 2064 616e 7320 6c65 2070 6172 616d c3a8   dans le param..
+00000940: 7472 6520 4c54 4920 5061 7373 706f 7274  tre LTI Passport
+00000950: 7320 6465 206c 6120 7061 6765 2064 6573  s de la page des
+00000960: 2070 6172 616d c3a8 7472 6573 2061 7661   param..tres ava
+00000970: 6e63 c3a9 732e 3c62 7220 2f3e 566f 6972  nc..s.<br />Voir
+00000980: 207b 646f 6373 5f61 6e63 686f 725f 6f70   {docs_anchor_op
+00000990: 656e 7d65 6458 204c 5449 2064 6f63 756d  en}edX LTI docum
+000009a0: 656e 7461 7469 6f6e 7b61 6e63 686f 725f  entation{anchor_
+000009b0: 636c 6f73 657d 2070 6f75 7220 706c 7573  close} pour plus
+000009c0: 2064 6520 64c3 a974 6169 6c73 2073 7572   de d..tails sur
+000009d0: 2063 6520 7061 7261 6dc3 a874 7265 2e22   ce param..tre."
+000009e0: 0a0a 233a 206c 7469 5f63 6f6e 7375 6d65  ..#: lti_consume
+000009f0: 722e 7079 0a6d 7367 6964 2022 4c54 4920  r.py.msgid "LTI 
+00000a00: 5552 4c22 0a6d 7367 7374 7220 2255 524c  URL".msgstr "URL
+00000a10: 204c 5449 220a 0a23 3a20 6c74 695f 636f   LTI"..#: lti_co
+00000a20: 6e73 756d 6572 2e70 790a 232c 2070 7974  nsumer.py.#, pyt
+00000a30: 686f 6e2d 6272 6163 652d 666f 726d 6174  hon-brace-format
+00000a40: 0a6d 7367 6964 2022 220a 2245 6e74 6572  .msgid ""."Enter
+00000a50: 2074 6865 2055 524c 206f 6620 7468 6520   the URL of the 
+00000a60: 6578 7465 726e 616c 2074 6f6f 6c20 7468  external tool th
+00000a70: 6174 2074 6869 7320 636f 6d70 6f6e 656e  at this componen
+00000a80: 7420 6c61 756e 6368 6573 2e20 5468 6973  t launches. This
+00000a90: 2022 0a22 7365 7474 696e 6720 6973 206f   "."setting is o
+00000aa0: 6e6c 7920 7573 6564 2077 6865 6e20 4869  nly used when Hi
+00000ab0: 6465 2045 7874 6572 6e61 6c20 546f 6f6c  de External Tool
+00000ac0: 2069 7320 7365 7420 746f 2046 616c 7365   is set to False
+00000ad0: 2e3c 6272 202f 3e53 6565 2074 6865 2022  .<br />See the "
+00000ae0: 0a22 7b64 6f63 735f 616e 6368 6f72 5f6f  ."{docs_anchor_o
+00000af0: 7065 6e7d 6564 5820 4c54 4920 646f 6375  pen}edX LTI docu
+00000b00: 6d65 6e74 6174 696f 6e7b 616e 6368 6f72  mentation{anchor
+00000b10: 5f63 6c6f 7365 7d20 666f 7220 6d6f 7265  _close} for more
+00000b20: 2064 6574 6169 6c73 206f 6e20 220a 2274   details on "."t
+00000b30: 6869 7320 7365 7474 696e 672e 220a 6d73  his setting.".ms
+00000b40: 6773 7472 2022 456e 7472 657a 206c 2755  gstr "Entrez l'U
+00000b50: 524c 2064 6520 6c27 6f75 7469 6c20 6578  RL de l'outil ex
+00000b60: 7465 726e 6520 7175 6520 6365 2063 6f6d  terne que ce com
+00000b70: 706f 7361 6e74 206c 616e 6365 2e20 4365  posant lance. Ce
+00000b80: 2070 6172 616d c3a8 7472 6520 6573 7420   param..tre est 
+00000b90: 756e 6971 7565 6d65 6e74 2075 7469 6c69  uniquement utili
+00000ba0: 73c3 a920 6c6f 7273 7175 6520 6c27 6f70  s.. lorsque l'op
+00000bb0: 7469 6f6e 204d 6173 7175 6572 206c 276f  tion Masquer l'o
+00000bc0: 7574 696c 2065 7874 6572 6e65 2065 7374  util externe est
+00000bd0: 2064 c3a9 6669 6e69 6520 7375 7220 4661   d..finie sur Fa
+00000be0: 6c73 652e 3c62 7220 2f3e 566f 6972 207b  lse.<br />Voir {
+00000bf0: 646f 6373 5f61 6e63 686f 725f 6f70 656e  docs_anchor_open
+00000c00: 7d65 6458 204c 5449 2064 6f63 756d 656e  }edX LTI documen
+00000c10: 7461 7469 6f6e 7b61 6e63 686f 725f 636c  tation{anchor_cl
+00000c20: 6f73 657d 2070 6f75 7220 706c 7573 2064  ose} pour plus d
+00000c30: 6520 64c3 a974 6169 6c73 2073 7572 2063  e d..tails sur c
+00000c40: 6520 7061 7261 6dc3 a874 7265 2e22 0a0a  e param..tre."..
+00000c50: 233a 206c 7469 5f63 6f6e 7375 6d65 722e  #: lti_consumer.
+00000c60: 7079 0a6d 7367 6964 2022 4375 7374 6f6d  py.msgid "Custom
+00000c70: 2050 6172 616d 6574 6572 7322 0a6d 7367   Parameters".msg
+00000c80: 7374 7220 2250 6172 616d c3a8 7472 6573  str "Param..tres
+00000c90: 2070 6572 736f 6e6e 616c 6973 c3a9 7322   personnalis..s"
+00000ca0: 0a0a 233a 206c 7469 5f63 6f6e 7375 6d65  ..#: lti_consume
+00000cb0: 722e 7079 0a23 2c20 7079 7468 6f6e 2d62  r.py.#, python-b
+00000cc0: 7261 6365 2d66 6f72 6d61 740a 6d73 6769  race-format.msgi
+00000cd0: 6420 2222 0a22 4164 6420 7468 6520 6b65  d ""."Add the ke
+00000ce0: 792f 7661 6c75 6520 7061 6972 2066 6f72  y/value pair for
+00000cf0: 2061 6e79 2063 7573 746f 6d20 7061 7261   any custom para
+00000d00: 6d65 7465 7273 2c20 7375 6368 2061 7320  meters, such as 
+00000d10: 7468 6520 7061 6765 2079 6f75 7220 220a  the page your ".
+00000d20: 2265 2d62 6f6f 6b20 7368 6f75 6c64 206f  "e-book should o
+00000d30: 7065 6e20 746f 206f 7220 7468 6520 6261  pen to or the ba
+00000d40: 636b 6772 6f75 6e64 2063 6f6c 6f72 2066  ckground color f
+00000d50: 6f72 2074 6869 7320 636f 6d70 6f6e 656e  or this componen
+00000d60: 742e 2045 782e 2022 0a22 5b5c 2270 6167  t. Ex. "."[\"pag
+00000d70: 653d 315c 222c 205c 2263 6f6c 6f72 3d77  e=1\", \"color=w
+00000d80: 6869 7465 5c22 5d3c 6272 202f 3e53 6565  hite\"]<br />See
+00000d90: 2074 6865 207b 646f 6373 5f61 6e63 686f   the {docs_ancho
+00000da0: 725f 6f70 656e 7d65 6458 204c 5449 2022  r_open}edX LTI "
+00000db0: 0a22 646f 6375 6d65 6e74 6174 696f 6e7b  ."documentation{
+00000dc0: 616e 6368 6f72 5f63 6c6f 7365 7d20 666f  anchor_close} fo
+00000dd0: 7220 6d6f 7265 2064 6574 6169 6c73 206f  r more details o
+00000de0: 6e20 7468 6973 2073 6574 7469 6e67 2e22  n this setting."
+00000df0: 0a6d 7367 7374 7220 2241 6a6f 7574 657a  .msgstr "Ajoutez
+00000e00: 206c 6120 7061 6972 6520 636c c3a9 202f   la paire cl.. /
+00000e10: 2076 616c 6575 7220 706f 7572 2074 6f75   valeur pour tou
+00000e20: 7320 6c65 7320 7061 7261 6dc3 a874 7265  s les param..tre
+00000e30: 7320 7065 7273 6f6e 6e61 6c69 73c3 a973  s personnalis..s
+00000e40: 2c20 7465 6c73 2071 7565 206c 6120 7061  , tels que la pa
+00000e50: 6765 2071 7565 2076 6f74 7265 206c 6976  ge que votre liv
+00000e60: 7265 20c3 a96c 6563 7472 6f6e 6971 7565  re ..lectronique
+00000e70: 2064 6f69 7420 6f75 7672 6972 206f 7520   doit ouvrir ou 
+00000e80: 6c61 2063 6f75 6c65 7572 2064 2761 7272  la couleur d'arr
+00000e90: 69c3 a872 652d 706c 616e 2064 6520 6365  i..re-plan de ce
+00000ea0: 2063 6f6d 706f 7361 6e74 2e20 4578 2e20   composant. Ex. 
+00000eb0: 5b5c 2270 6167 653d 315c 222c 205c 2263  [\"page=1\", \"c
+00000ec0: 6f6c 6f72 3d77 6869 7465 5c22 5d3c 6272  olor=white\"]<br
+00000ed0: 202f 3e56 6f69 7220 7b64 6f63 735f 616e   />Voir {docs_an
+00000ee0: 6368 6f72 5f6f 7065 6e7d 6564 5820 4c54  chor_open}edX LT
+00000ef0: 4920 646f 6375 6d65 6e74 6174 696f 6e7b  I documentation{
+00000f00: 616e 6368 6f72 5f63 6c6f 7365 7d20 706f  anchor_close} po
+00000f10: 7572 2070 6c75 7320 6465 2064 c3a9 7461  ur plus de d..ta
+00000f20: 696c 7320 7375 7220 6365 2070 6172 616d  ils sur ce param
+00000f30: c3a8 7472 652e 220a 0a23 3a20 6c74 695f  ..tre."..#: lti_
+00000f40: 636f 6e73 756d 6572 2e70 790a 6d73 6769  consumer.py.msgi
+00000f50: 6420 224c 5449 204c 6175 6e63 6820 5461  d "LTI Launch Ta
+00000f60: 7267 6574 220a 6d73 6773 7472 2022 4369  rget".msgstr "Ci
+00000f70: 626c 6520 6465 206c 616e 6365 6d65 6e74  ble de lancement
+00000f80: 204c 5449 220a 0a23 3a20 6c74 695f 636f   LTI"..#: lti_co
+00000f90: 6e73 756d 6572 2e70 790a 6d73 6769 6420  nsumer.py.msgid 
+00000fa0: 2222 0a22 5365 6c65 6374 2049 6e6c 696e  ""."Select Inlin
+00000fb0: 6520 6966 2079 6f75 2077 616e 7420 7468  e if you want th
+00000fc0: 6520 4c54 4920 636f 6e74 656e 7420 746f  e LTI content to
+00000fd0: 206f 7065 6e20 696e 2061 6e20 4946 7261   open in an IFra
+00000fe0: 6d65 2069 6e20 7468 6520 220a 2263 7572  me in the "."cur
+00000ff0: 7265 6e74 2070 6167 652e 2053 656c 6563  rent page. Selec
+00001000: 7420 4d6f 6461 6c20 6966 2079 6f75 2077  t Modal if you w
+00001010: 616e 7420 7468 6520 4c54 4920 636f 6e74  ant the LTI cont
+00001020: 656e 7420 746f 206f 7065 6e20 696e 2061  ent to open in a
+00001030: 206d 6f64 616c 2022 0a22 7769 6e64 6f77   modal "."window
+00001040: 2069 6e20 7468 6520 6375 7272 656e 7420   in the current 
+00001050: 7061 6765 2e20 5365 6c65 6374 204e 6577  page. Select New
+00001060: 2057 696e 646f 7720 6966 2079 6f75 2077   Window if you w
+00001070: 616e 7420 7468 6520 4c54 4920 636f 6e74  ant the LTI cont
+00001080: 656e 7420 746f 220a 2220 6f70 656e 2069  ent to"." open i
+00001090: 6e20 6120 6e65 7720 6272 6f77 7365 7220  n a new browser 
+000010a0: 7769 6e64 6f77 2e20 5468 6973 2073 6574  window. This set
+000010b0: 7469 6e67 2069 7320 6f6e 6c79 2075 7365  ting is only use
+000010c0: 6420 7768 656e 2048 6964 6520 4578 7465  d when Hide Exte
+000010d0: 726e 616c 2022 0a22 546f 6f6c 2069 7320  rnal "."Tool is 
+000010e0: 7365 7420 746f 2046 616c 7365 2e22 0a6d  set to False.".m
+000010f0: 7367 7374 7220 2253 c3a9 6c65 6374 696f  sgstr "S..lectio
+00001100: 6e6e 657a 2049 6e6c 696e 6520 7369 2076  nnez Inline si v
+00001110: 6f75 7320 736f 7568 6169 7465 7a20 7175  ous souhaitez qu
+00001120: 6520 6c65 2063 6f6e 7465 6e75 204c 5449  e le contenu LTI
+00001130: 2073 276f 7576 7265 2064 616e 7320 756e   s'ouvre dans un
+00001140: 2049 4672 616d 6520 6465 206c 6120 7061   IFrame de la pa
+00001150: 6765 2065 6e20 636f 7572 732e 2053 c3a9  ge en cours. S..
+00001160: 6c65 6374 696f 6e6e 657a 204d 6f64 616c  lectionnez Modal
+00001170: 2073 6920 766f 7573 2073 6f75 6861 6974   si vous souhait
+00001180: 657a 2071 7565 206c 6520 636f 6e74 656e  ez que le conten
+00001190: 7520 4c54 4920 7327 6f75 7672 6520 6461  u LTI s'ouvre da
+000011a0: 6e73 2075 6e65 2066 656e c3aa 7472 6520  ns une fen..tre 
+000011b0: 6d6f 6461 6c65 2064 6520 6c61 2070 6167  modale de la pag
+000011c0: 6520 656e 2063 6f75 7273 2e20 53c3 a96c  e en cours. S..l
+000011d0: 6563 7469 6f6e 6e65 7a20 4e6f 7576 656c  ectionnez Nouvel
+000011e0: 6c65 2046 656e c3aa 7472 6520 7369 2076  le Fen..tre si v
+000011f0: 6f75 7320 736f 7568 6169 7465 7a20 7175  ous souhaitez qu
+00001200: 6520 6c65 2063 6f6e 7465 6e75 204c 5449  e le contenu LTI
+00001210: 2073 276f 7576 7265 2064 616e 7320 756e   s'ouvre dans un
+00001220: 6520 6e6f 7576 656c 6c65 2066 656e c3aa  e nouvelle fen..
+00001230: 7472 6520 6475 206e 6176 6967 6174 6575  tre du navigateu
+00001240: 722e 2043 6520 7061 7261 6dc3 a874 7265  r. Ce param..tre
+00001250: 2065 7374 2075 6e69 7175 656d 656e 7420   est uniquement 
+00001260: 7574 696c 6973 c3a9 206c 6f72 7371 7565  utilis.. lorsque
+00001270: 206c 276f 7074 696f 6e20 6d61 7371 7565   l'option masque
+00001280: 7220 6c27 6f75 7469 6c20 6578 7465 726e  r l'outil extern
+00001290: 6520 6573 7420 64c3 a966 696e 6965 2073  e est d..finie s
+000012a0: 7572 2046 616c 7365 2e22 0a0a 233a 206c  ur False."..#: l
+000012b0: 7469 5f63 6f6e 7375 6d65 722e 7079 0a6d  ti_consumer.py.m
+000012c0: 7367 6964 2022 4275 7474 6f6e 2054 6578  sgid "Button Tex
+000012d0: 7422 0a6d 7367 7374 7220 2254 6578 7465  t".msgstr "Texte
+000012e0: 2064 7520 626f 7574 6f6e 220a 0a23 3a20   du bouton"..#: 
+000012f0: 6c74 695f 636f 6e73 756d 6572 2e70 790a  lti_consumer.py.
+00001300: 6d73 6769 6420 2222 0a22 456e 7465 7220  msgid ""."Enter 
+00001310: 7468 6520 7465 7874 206f 6e20 7468 6520  the text on the 
+00001320: 6275 7474 6f6e 2075 7365 6420 746f 206c  button used to l
+00001330: 6175 6e63 6820 7468 6520 7468 6972 6420  aunch the third 
+00001340: 7061 7274 7920 6170 706c 6963 6174 696f  party applicatio
+00001350: 6e2e 2022 0a22 5468 6973 2073 6574 7469  n. "."This setti
+00001360: 6e67 2069 7320 6f6e 6c79 2075 7365 6420  ng is only used 
+00001370: 7768 656e 2048 6964 6520 4578 7465 726e  when Hide Extern
+00001380: 616c 2054 6f6f 6c20 6973 2073 6574 2074  al Tool is set t
+00001390: 6f20 4661 6c73 6520 616e 6420 4c54 4920  o False and LTI 
+000013a0: 220a 224c 6175 6e63 6820 5461 7267 6574  "."Launch Target
+000013b0: 2069 7320 7365 7420 746f 204d 6f64 616c   is set to Modal
+000013c0: 206f 7220 4e65 7720 5769 6e64 6f77 2e22   or New Window."
+000013d0: 0a6d 7367 7374 7220 2245 6e74 7265 7a20  .msgstr "Entrez 
+000013e0: 6c65 2074 6578 7465 2064 7520 626f 7574  le texte du bout
+000013f0: 6f6e 2071 7569 2073 6572 6120 7574 696c  on qui sera util
+00001400: 6973 c3a9 2070 6f75 7220 6c61 6e63 6572  is.. pour lancer
+00001410: 206c 2761 7070 6c69 6361 7469 6f6e 2074   l'application t
+00001420: 6965 7263 652e 2043 6520 7061 7261 6dc3  ierce. Ce param.
+00001430: a874 7265 2065 7374 2075 7469 6c69 73c3  .tre est utilis.
+00001440: a920 756e 6971 7565 6d65 6e74 206c 6f72  . uniquement lor
+00001450: 7371 7565 206d 6173 7175 6572 206c 276f  sque masquer l'o
+00001460: 7574 696c 2065 7874 6572 6e65 2065 7374  util externe est
+00001470: 2064 c3a9 6669 6e69 2073 7572 2046 616c   d..fini sur Fal
+00001480: 7365 2065 7420 7175 6520 4c54 4920 4c61  se et que LTI La
+00001490: 756e 6368 2054 6172 6765 7420 6573 7420  unch Target est 
+000014a0: 64c3 a966 696e 6920 7375 7220 4d6f 6461  d..fini sur Moda
+000014b0: 6c20 6f75 204e 6f75 7665 6c6c 6520 6665  l ou Nouvelle fe
+000014c0: 6ec3 aa74 7265 2e22 0a0a 233a 206c 7469  n..tre."..#: lti
+000014d0: 5f63 6f6e 7375 6d65 722e 7079 0a6d 7367  _consumer.py.msg
+000014e0: 6964 2022 496e 6c69 6e65 2048 6569 6768  id "Inline Heigh
+000014f0: 7422 0a6d 7367 7374 7220 2248 6175 7465  t".msgstr "Haute
+00001500: 7572 2069 6e74 c3a9 6772 c3a9 220a 0a23  ur int..gr.."..#
+00001510: 3a20 6c74 695f 636f 6e73 756d 6572 2e70  : lti_consumer.p
+00001520: 790a 6d73 6769 6420 2222 0a22 456e 7465  y.msgid ""."Ente
+00001530: 7220 7468 6520 6465 7369 7265 6420 7069  r the desired pi
+00001540: 7865 6c20 6865 6967 6874 206f 6620 7468  xel height of th
+00001550: 6520 6966 7261 6d65 2077 6869 6368 2077  e iframe which w
+00001560: 696c 6c20 636f 6e74 6169 6e20 7468 6520  ill contain the 
+00001570: 4c54 4920 220a 2274 6f6f 6c2e 2054 6869  LTI "."tool. Thi
+00001580: 7320 7365 7474 696e 6720 6973 206f 6e6c  s setting is onl
+00001590: 7920 7573 6564 2077 6865 6e20 4869 6465  y used when Hide
+000015a0: 2045 7874 6572 6e61 6c20 546f 6f6c 2069   External Tool i
+000015b0: 7320 7365 7420 746f 2046 616c 7365 2061  s set to False a
+000015c0: 6e64 2022 0a22 4c54 4920 4c61 756e 6368  nd "."LTI Launch
+000015d0: 2054 6172 6765 7420 6973 2073 6574 2074   Target is set t
+000015e0: 6f20 496e 6c69 6e65 2e22 0a6d 7367 7374  o Inline.".msgst
+000015f0: 7220 2245 6e74 7265 7a20 6c61 2068 6175  r "Entrez la hau
+00001600: 7465 7572 2064 6520 7069 7865 6c20 736f  teur de pixel so
+00001610: 7568 6169 74c3 a965 2064 6520 6c27 6966  uhait..e de l'if
+00001620: 7261 6d65 2071 7569 2063 6f6e 7469 656e  rame qui contien
+00001630: 6472 6120 6c27 6f75 7469 6c20 4c54 492e  dra l'outil LTI.
+00001640: 2043 6520 7061 7261 6dc3 a874 7265 2065   Ce param..tre e
+00001650: 7374 2075 6e69 7175 656d 656e 7420 7574  st uniquement ut
+00001660: 696c 6973 c3a9 206c 6f72 7371 7565 206d  ilis.. lorsque m
+00001670: 6173 7175 6572 206c 276f 7574 696c 2065  asquer l'outil e
+00001680: 7874 6572 6e65 2065 7374 2064 c3a9 6669  xterne est d..fi
+00001690: 6e69 2073 7572 2046 616c 7365 2065 7420  ni sur False et 
+000016a0: 7175 6520 4c54 4920 4c61 756e 6368 2054  que LTI Launch T
+000016b0: 6172 6765 7420 6573 7420 64c3 a966 696e  arget est d..fin
+000016c0: 6920 7375 7220 496e 6c69 6e65 2e22 0a0a  i sur Inline."..
+000016d0: 233a 206c 7469 5f63 6f6e 7375 6d65 722e  #: lti_consumer.
+000016e0: 7079 0a6d 7367 6964 2022 4d6f 6461 6c20  py.msgid "Modal 
+000016f0: 4865 6967 6874 220a 6d73 6773 7472 2022  Height".msgstr "
+00001700: 4861 7574 6575 7220 6d6f 6461 6c65 220a  Hauteur modale".
+00001710: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00001720: 2e70 790a 6d73 6769 6420 2222 0a22 456e  .py.msgid ""."En
+00001730: 7465 7220 7468 6520 6465 7369 7265 6420  ter the desired 
+00001740: 7669 6577 706f 7274 2070 6572 6365 6e74  viewport percent
+00001750: 6167 6520 6865 6967 6874 206f 6620 7468  age height of th
+00001760: 6520 6d6f 6461 6c20 6f76 6572 6c61 7920  e modal overlay 
+00001770: 7768 6963 6820 7769 6c6c 220a 2220 636f  which will"." co
+00001780: 6e74 6169 6e20 7468 6520 4c54 4920 746f  ntain the LTI to
+00001790: 6f6c 2e20 5468 6973 2073 6574 7469 6e67  ol. This setting
+000017a0: 2069 7320 6f6e 6c79 2075 7365 6420 7768   is only used wh
+000017b0: 656e 2048 6964 6520 4578 7465 726e 616c  en Hide External
+000017c0: 2054 6f6f 6c20 6973 2022 0a22 7365 7420   Tool is "."set 
+000017d0: 746f 2046 616c 7365 2061 6e64 204c 5449  to False and LTI
+000017e0: 204c 6175 6e63 6820 5461 7267 6574 2069   Launch Target i
+000017f0: 7320 7365 7420 746f 204d 6f64 616c 2e22  s set to Modal."
+00001800: 0a6d 7367 7374 7220 2245 6e74 7265 7a20  .msgstr "Entrez 
+00001810: 6c65 2070 6f75 7263 656e 7461 6765 2064  le pourcentage d
+00001820: 6520 6861 7574 6575 7220 6465 206c 6120  e hauteur de la 
+00001830: 6665 6ec3 aa74 7265 2064 6520 7669 7375  fen..tre de visu
+00001840: 616c 6973 6174 696f 6e20 6465 206c 6120  alisation de la 
+00001850: 7375 7065 7270 6f73 6974 696f 6e20 6d6f  superposition mo
+00001860: 6461 6c65 2071 7569 2063 6f6e 7469 656e  dale qui contien
+00001870: 6472 6120 6ce2 8099 6f75 7469 6c20 4c54  dra l...outil LT
+00001880: 492e 2043 6520 7061 7261 6dc3 a874 7265  I. Ce param..tre
+00001890: 2065 7374 2075 6e69 7175 656d 656e 7420   est uniquement 
+000018a0: 7574 696c 6973 c3a9 206c 6f72 7371 7565  utilis.. lorsque
+000018b0: 206d 6173 7175 6572 206c 276f 7574 696c   masquer l'outil
+000018c0: 2065 7874 6572 6e65 2065 7374 2064 c3a9   externe est d..
+000018d0: 6669 6e69 2073 7572 2046 616c 7365 2065  fini sur False e
+000018e0: 7420 7175 6520 4c54 4920 4c61 756e 6368  t que LTI Launch
+000018f0: 2054 6172 6765 7420 6573 7420 64c3 a966   Target est d..f
+00001900: 696e 6920 7375 7220 4d6f 6461 6c2e 220a  ini sur Modal.".
+00001910: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00001920: 2e70 790a 6d73 6769 6420 224d 6f64 616c  .py.msgid "Modal
+00001930: 2057 6964 7468 220a 6d73 6773 7472 2022   Width".msgstr "
+00001940: 4c61 7267 6575 7220 6d6f 6461 6c65 220a  Largeur modale".
+00001950: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00001960: 2e70 790a 6d73 6769 6420 2222 0a22 456e  .py.msgid ""."En
+00001970: 7465 7220 7468 6520 6465 7369 7265 6420  ter the desired 
+00001980: 7669 6577 706f 7274 2070 6572 6365 6e74  viewport percent
+00001990: 6167 6520 7769 6474 6820 6f66 2074 6865  age width of the
+000019a0: 206d 6f64 616c 206f 7665 726c 6179 2077   modal overlay w
+000019b0: 6869 6368 2077 696c 6c20 220a 2263 6f6e  hich will "."con
+000019c0: 7461 696e 2074 6865 204c 5449 2074 6f6f  tain the LTI too
+000019d0: 6c2e 2054 6869 7320 7365 7474 696e 6720  l. This setting 
+000019e0: 6973 206f 6e6c 7920 7573 6564 2077 6865  is only used whe
+000019f0: 6e20 4869 6465 2045 7874 6572 6e61 6c20  n Hide External 
+00001a00: 546f 6f6c 2069 7320 220a 2273 6574 2074  Tool is "."set t
+00001a10: 6f20 4661 6c73 6520 616e 6420 4c54 4920  o False and LTI 
+00001a20: 4c61 756e 6368 2054 6172 6765 7420 6973  Launch Target is
+00001a30: 2073 6574 2074 6f20 4d6f 6461 6c2e 220a   set to Modal.".
+00001a40: 6d73 6773 7472 2022 456e 7472 657a 206c  msgstr "Entrez l
+00001a50: 6520 706f 7572 6365 6e74 6167 6520 6465  e pourcentage de
+00001a60: 206c 6172 6765 7572 2064 6520 6c61 2066   largeur de la f
+00001a70: 656e c3aa 7472 6520 6465 2073 7570 6572  en..tre de super
+00001a80: 706f 7369 7469 6f6e 206d 6f64 616c 6520  position modale 
+00001a90: 7175 6920 636f 6e74 6965 6e64 7261 206c  qui contiendra l
+00001aa0: e280 996f 7574 696c 204c 5449 2e20 4365  ...outil LTI. Ce
+00001ab0: 2070 6172 616d c3a8 7472 6520 6573 7420   param..tre est 
+00001ac0: 756e 6971 7565 6d65 6e74 2075 7469 6c69  uniquement utili
+00001ad0: 73c3 a920 6c6f 7273 7175 6520 6d61 7371  s.. lorsque masq
+00001ae0: 7565 7220 6c27 6f75 7469 6c20 6578 7465  uer l'outil exte
+00001af0: 726e 6520 6573 7420 64c3 a966 696e 6920  rne est d..fini 
+00001b00: 7375 7220 4661 6c73 6520 6574 2071 7565  sur False et que
+00001b10: 204c 5449 204c 6175 6e63 6820 5461 7267   LTI Launch Targ
+00001b20: 6574 2065 7374 2064 c3a9 6669 6e69 2073  et est d..fini s
+00001b30: 7572 204d 6f64 616c 2e22 0a0a 233a 206c  ur Modal."..#: l
+00001b40: 7469 5f63 6f6e 7375 6d65 722e 7079 0a6d  ti_consumer.py.m
+00001b50: 7367 6964 2022 5363 6f72 6564 220a 6d73  sgid "Scored".ms
+00001b60: 6773 7472 2022 4e6f 74c3 a922 0a0a 233a  gstr "Not.."..#:
+00001b70: 206c 7469 5f63 6f6e 7375 6d65 722e 7079   lti_consumer.py
+00001b80: 0a6d 7367 6964 2022 220a 2253 656c 6563  .msgid ""."Selec
+00001b90: 7420 5472 7565 2069 6620 7468 6973 2063  t True if this c
+00001ba0: 6f6d 706f 6e65 6e74 2077 696c 6c20 7265  omponent will re
+00001bb0: 6365 6976 6520 6120 6e75 6d65 7269 6361  ceive a numerica
+00001bc0: 6c20 7363 6f72 6520 6672 6f6d 2074 6865  l score from the
+00001bd0: 2022 0a22 6578 7465 726e 616c 204c 5449   "."external LTI
+00001be0: 2073 7973 7465 6d2e 220a 6d73 6773 7472   system.".msgstr
+00001bf0: 2022 53c3 a96c 6563 7469 6f6e 6e65 7220   "S..lectionner 
+00001c00: 7672 6169 2028 7472 7565 2920 7369 2063  vrai (true) si c
+00001c10: 6520 636f 6d70 6f73 616e 7420 7661 2072  e composant va r
+00001c20: 6563 6576 6f69 7220 756e 6520 6e6f 7465  ecevoir une note
+00001c30: 206e 756d c3a9 7269 7175 6520 6465 206c   num..rique de l
+00001c40: 6120 7061 7274 2064 7520 7379 7374 c3a8  a part du syst..
+00001c50: 6d65 2065 7874 6572 6e65 204c 5449 2e22  me externe LTI."
+00001c60: 0a0a 233a 206c 7469 5f63 6f6e 7375 6d65  ..#: lti_consume
+00001c70: 722e 7079 0a6d 7367 6964 2022 220a 2245  r.py.msgid ""."E
+00001c80: 6e74 6572 2074 6865 206e 756d 6265 7220  nter the number 
+00001c90: 6f66 2070 6f69 6e74 7320 706f 7373 6962  of points possib
+00001ca0: 6c65 2066 6f72 2074 6869 7320 636f 6d70  le for this comp
+00001cb0: 6f6e 656e 742e 2020 5468 6520 6465 6661  onent.  The defa
+00001cc0: 756c 7420 7661 6c75 6520 220a 2269 7320  ult value "."is 
+00001cd0: 312e 302e 2020 5468 6973 2073 6574 7469  1.0.  This setti
+00001ce0: 6e67 2069 7320 6f6e 6c79 2075 7365 6420  ng is only used 
+00001cf0: 7768 656e 2053 636f 7265 6420 6973 2073  when Scored is s
+00001d00: 6574 2074 6f20 5472 7565 2e22 0a6d 7367  et to True.".msg
+00001d10: 7374 7220 2245 6e74 7265 7220 6c65 206e  str "Entrer le n
+00001d20: 6f6d 6272 6520 6465 2070 6f69 6e74 7320  ombre de points 
+00001d30: 706f 7373 6962 6c65 2070 6f75 7220 6365  possible pour ce
+00001d40: 2063 6f6d 706f 7361 6e74 2e20 4c61 2076   composant. La v
+00001d50: 616c 6575 7220 6465 2064 c3a9 6661 7574  aleur de d..faut
+00001d60: 2065 7374 2031 2e30 2e20 4365 2070 6172   est 1.0. Ce par
+00001d70: 616d c3a8 7472 6520 6573 7420 756e 6971  am..tre est uniq
+00001d80: 7565 6d65 6e74 2075 7469 6c69 73c3 a920  uement utilis.. 
+00001d90: 7175 616e 6420 4e6f 74c3 a920 6573 7420  quand Not.. est 
+00001da0: 696e 6974 6961 6c69 73c3 a920 c3a0 2056  initialis.. .. V
+00001db0: 7261 6920 2854 7275 6529 2e22 0a0a 233a  rai (True)."..#:
+00001dc0: 206c 7469 5f63 6f6e 7375 6d65 722e 7079   lti_consumer.py
+00001dd0: 0a6d 7367 6964 2022 220a 2254 6865 2073  .msgid ""."The s
+00001de0: 636f 7265 206b 6570 7420 696e 2074 6865  core kept in the
+00001df0: 2078 626c 6f63 6b20 4b56 5320 2d2d 2064   xblock KVS -- d
+00001e00: 7570 6c69 6361 7465 206f 6620 7468 6520  uplicate of the 
+00001e10: 7075 626c 6973 6865 6420 7363 6f72 6520  published score 
+00001e20: 696e 2022 0a22 646a 616e 676f 2044 4222  in "."django DB"
+00001e30: 0a6d 7367 7374 7220 224c 6120 6e6f 7465  .msgstr "La note
+00001e40: 2063 6f6e 7365 7276 c3a9 6520 6461 6e73   conserv..e dans
+00001e50: 206c 6520 7862 6c6f 636b 204b 5653 202d   le xblock KVS -
+00001e60: 2d20 6475 706c 6963 6174 2064 6520 6c61  - duplicat de la
+00001e70: 206e 6f74 6520 7075 626c 69c3 a965 2064   note publi..e d
+00001e80: 616e 7320 646a 616e 676f 2044 4222 0a0a  ans django DB"..
+00001e90: 233a 206c 7469 5f63 6f6e 7375 6d65 722e  #: lti_consumer.
+00001ea0: 7079 0a6d 7367 6964 2022 436f 6d6d 656e  py.msgid "Commen
+00001eb0: 7420 6173 2072 6574 7572 6e65 6420 6672  t as returned fr
+00001ec0: 6f6d 2067 7261 6465 722c 204c 5449 322e  om grader, LTI2.
+00001ed0: 3020 7370 6563 220a 6d73 6773 7472 2022  0 spec".msgstr "
+00001ee0: 436f 6d6d 656e 7461 6972 6520 636f 6d6d  Commentaire comm
+00001ef0: 6520 7265 746f 7572 6ec3 a920 7061 7220  e retourn.. par 
+00001f00: 6c27 c3a9 7661 6c75 6174 6575 722c 2073  l'..valuateur, s
+00001f10: 70c3 a963 6966 6963 6174 696f 6e20 4c54  p..cification LT
+00001f20: 4932 2e30 220a 0a23 3a20 6c74 695f 636f  I2.0"..#: lti_co
+00001f30: 6e73 756d 6572 2e70 790a 6d73 6769 6420  nsumer.py.msgid 
+00001f40: 2248 6964 6520 4578 7465 726e 616c 2054  "Hide External T
+00001f50: 6f6f 6c22 0a6d 7367 7374 7220 2243 6163  ool".msgstr "Cac
+00001f60: 6865 7220 6c65 7320 6f75 7469 6c73 2065  her les outils e
+00001f70: 7874 6572 6e65 7322 0a0a 233a 206c 7469  xternes"..#: lti
+00001f80: 5f63 6f6e 7375 6d65 722e 7079 0a6d 7367  _consumer.py.msg
+00001f90: 6964 2022 220a 2253 656c 6563 7420 5472  id ""."Select Tr
+00001fa0: 7565 2069 6620 796f 7520 7761 6e74 2074  ue if you want t
+00001fb0: 6f20 7573 6520 7468 6973 2063 6f6d 706f  o use this compo
+00001fc0: 6e65 6e74 2061 7320 6120 706c 6163 6568  nent as a placeh
+00001fd0: 6f6c 6465 7220 666f 7220 7379 6e63 696e  older for syncin
+00001fe0: 6720 220a 2277 6974 6820 616e 2065 7874  g "."with an ext
+00001ff0: 6572 6e61 6c20 6772 6164 696e 6720 2073  ernal grading  s
+00002000: 7973 7465 6d20 7261 7468 6572 2074 6861  ystem rather tha
+00002010: 6e20 6c61 756e 6368 2061 6e20 6578 7465  n launch an exte
+00002020: 726e 616c 2074 6f6f 6c2e 2020 5468 6973  rnal tool.  This
+00002030: 2022 0a22 7365 7474 696e 6720 6869 6465   "."setting hide
+00002040: 7320 7468 6520 4c61 756e 6368 2062 7574  s the Launch but
+00002050: 746f 6e20 616e 6420 616e 7920 4946 7261  ton and any IFra
+00002060: 6d65 7320 666f 7220 7468 6973 2063 6f6d  mes for this com
+00002070: 706f 6e65 6e74 2e22 0a6d 7367 7374 7220  ponent.".msgstr 
+00002080: 2253 c3a9 6c65 6374 696f 6e6e 6572 2076  "S..lectionner v
+00002090: 7261 6920 2874 7275 6529 2073 6920 766f  rai (true) si vo
+000020a0: 7573 2076 6f75 6c65 7a20 7574 696c 6973  us voulez utilis
+000020b0: 6572 2063 6520 636f 6d70 6f73 616e 7420  er ce composant 
+000020c0: 636f 6d6d 6520 756e 2065 7370 6163 6520  comme un espace 
+000020d0: 72c3 a973 6572 76c3 a920 706f 7572 2073  r..serv.. pour s
+000020e0: 796e 6368 726f 6e69 7365 7220 6176 6563  ynchroniser avec
+000020f0: 2075 6e20 7379 7374 c3a8 6d65 2064 27c3   un syst..me d'.
+00002100: a976 616c 7561 7469 6f6e 2065 7874 6572  .valuation exter
+00002110: 6e65 2061 7520 6c69 6575 2064 6520 64c3  ne au lieu de d.
+00002120: a96d 6172 7265 7220 756e 206f 7574 696c  .marrer un outil
+00002130: 2065 7874 6572 6e65 2e20 2043 6520 7061   externe.  Ce pa
+00002140: 7261 6dc3 a874 7265 2063 6163 6865 206c  ram..tre cache l
+00002150: 6520 626f 7574 6f6e 2044 c3a9 6d61 7272  e bouton D..marr
+00002160: 6167 6520 6574 2074 6f75 7420 4946 7261  age et tout IFra
+00002170: 6d65 7320 706f 7572 2063 6520 636f 6d70  mes pour ce comp
+00002180: 6f73 616e 742e 220a 0a23 3a20 6c74 695f  osant."..#: lti_
+00002190: 636f 6e73 756d 6572 2e70 790a 6d73 6769  consumer.py.msgi
+000021a0: 6420 2241 6363 6570 7420 6772 6164 6573  d "Accept grades
+000021b0: 2070 6173 7420 6465 6164 6c69 6e65 220a   past deadline".
+000021c0: 6d73 6773 7472 2022 4163 6365 7074 6572  msgstr "Accepter
+000021d0: 206c 6573 206e 6f74 6573 2061 7072 c3a8   les notes apr..
+000021e0: 7320 6c61 2064 6174 6520 6c69 6d69 7465  s la date limite
+000021f0: 220a 0a23 3a20 6c74 695f 636f 6e73 756d  "..#: lti_consum
+00002200: 6572 2e70 790a 6d73 6769 6420 2222 0a22  er.py.msgid ""."
+00002210: 5365 6c65 6374 2054 7275 6520 746f 2061  Select True to a
+00002220: 6c6c 6f77 2074 6869 7264 2070 6172 7479  llow third party
+00002230: 2073 7973 7465 6d73 2074 6f20 706f 7374   systems to post
+00002240: 2067 7261 6465 7320 7061 7374 2074 6865   grades past the
+00002250: 2064 6561 646c 696e 652e 220a 6d73 6773   deadline.".msgs
+00002260: 7472 2022 53c3 a96c 6563 7469 6f6e 6e65  tr "S..lectionne
+00002270: 7220 7672 6169 2028 7472 7565 2920 706f  r vrai (true) po
+00002280: 7572 2070 6572 6d65 7474 7265 2061 7578  ur permettre aux
+00002290: 2073 7973 74c3 a86d 6573 2074 6965 7263   syst..mes tierc
+000022a0: 6573 2064 6520 706f 7374 6572 2064 6573  es de poster des
+000022b0: 206e 6f74 6573 2061 7072 c3a8 7320 6c61   notes apr..s la
+000022c0: 2064 6174 6520 6c69 6d69 7465 2e22 0a0a   date limite."..
+000022d0: 233a 206c 7469 5f63 6f6e 7375 6d65 722e  #: lti_consumer.
+000022e0: 7079 0a6d 7367 6964 2022 5265 7175 6573  py.msgid "Reques
+000022f0: 7420 7573 6572 2773 2075 7365 726e 616d  t user's usernam
+00002300: 6522 0a6d 7367 7374 7220 2244 656d 616e  e".msgstr "Deman
+00002310: 6465 7220 6c65 206e 6f6d 2064 2775 7469  der le nom d'uti
+00002320: 6c69 7361 7465 7572 220a 0a23 3a20 6c74  lisateur"..#: lt
+00002330: 695f 636f 6e73 756d 6572 2e70 790a 6d73  i_consumer.py.ms
+00002340: 6769 6420 2253 656c 6563 7420 5472 7565  gid "Select True
+00002350: 2074 6f20 7265 7175 6573 7420 7468 6520   to request the 
+00002360: 7573 6572 2773 2075 7365 726e 616d 652e  user's username.
+00002370: 220a 6d73 6773 7472 2022 4368 6f69 7369  ".msgstr "Choisi
+00002380: 7220 7672 6169 2028 7472 7565 2920 6166  r vrai (true) af
+00002390: 696e 2064 6520 6465 6d61 6e64 6572 206c  in de demander l
+000023a0: 6520 6e6f 6d20 6427 7574 696c 6973 6174  e nom d'utilisat
+000023b0: 6575 722e 220a 0a23 3a20 6c74 695f 636f  eur."..#: lti_co
+000023c0: 6e73 756d 6572 2e70 790a 6d73 6769 6420  nsumer.py.msgid 
+000023d0: 2252 6571 7565 7374 2075 7365 7227 7320  "Request user's 
+000023e0: 656d 6169 6c22 0a6d 7367 7374 7220 2244  email".msgstr "D
+000023f0: 656d 616e 6465 7220 6c27 6164 7265 7373  emander l'adress
+00002400: 6520 636f 7572 7269 656c 2064 6520 6c27  e courriel de l'
+00002410: 7574 696c 6973 6174 6575 7222 0a0a 233a  utilisateur"..#:
+00002420: 206c 7469 5f63 6f6e 7375 6d65 722e 7079   lti_consumer.py
+00002430: 0a6d 7367 6964 2022 5365 6c65 6374 2054  .msgid "Select T
+00002440: 7275 6520 746f 2072 6571 7565 7374 2074  rue to request t
+00002450: 6865 2075 7365 7227 7320 656d 6169 6c20  he user's email 
+00002460: 6164 6472 6573 732e 220a 6d73 6773 7472  address.".msgstr
+00002470: 2022 4368 6f69 7369 7220 7672 6169 2028   "Choisir vrai (
+00002480: 7472 7565 2920 6166 696e 2064 6520 6465  true) afin de de
+00002490: 6d61 6e64 6572 206c 2761 6472 6573 7365  mander l'adresse
+000024a0: 2063 6f75 7272 6965 6c20 6465 206c 2775   courriel de l'u
+000024b0: 7469 6c69 7361 7465 7572 2e22 0a0a 233a  tilisateur."..#:
+000024c0: 206c 7469 5f63 6f6e 7375 6d65 722e 7079   lti_consumer.py
+000024d0: 0a23 2c20 7079 7468 6f6e 2d62 7261 6365  .#, python-brace
+000024e0: 2d66 6f72 6d61 740a 6d73 6769 6420 2222  -format.msgid ""
+000024f0: 0a22 436f 756c 6420 6e6f 7420 7061 7273  ."Could not pars
+00002500: 6520 4c54 4920 7061 7373 706f 7274 3a20  e LTI passport: 
+00002510: 7b6c 7469 5f70 6173 7370 6f72 747d 2e20  {lti_passport}. 
+00002520: 5368 6f75 6c64 2062 6520 5c22 6964 3a6b  Should be \"id:k
+00002530: 6579 3a73 6563 7265 745c 2220 220a 2273  ey:secret\" "."s
+00002540: 7472 696e 672e 220a 6d73 6773 7472 2022  tring.".msgstr "
+00002550: 496d 706f 7373 6962 6c65 2064 2761 6e61  Impossible d'ana
+00002560: 6c79 7365 7220 6c65 2070 6173 7365 706f  lyser le passepo
+00002570: 7274 204c 5449 3a20 7b6c 7469 5f70 6173  rt LTI: {lti_pas
+00002580: 7370 6f72 747d 2e20 4465 7672 6169 7420  sport}. Devrait 
+00002590: c3aa 7472 6520 756e 6520 6368 61c3 ae6e  ..tre une cha..n
+000025a0: 6520 5c22 6964 3a6b 6579 3a73 6563 7265  e \"id:key:secre
+000025b0: 745c 222e 220a 0a23 3a20 6c74 695f 636f  t\"."..#: lti_co
+000025c0: 6e73 756d 6572 2e70 790a 6d73 6769 6420  nsumer.py.msgid 
+000025d0: 2243 6f75 6c64 206e 6f74 2067 6574 2075  "Could not get u
+000025e0: 7365 7220 6964 2066 6f72 2063 7572 7265  ser id for curre
+000025f0: 6e74 2072 6571 7565 7374 220a 6d73 6773  nt request".msgs
+00002600: 7472 2022 496d 706f 7373 6962 6c65 2064  tr "Impossible d
+00002610: 276f 6274 656e 6972 206c 2749 4420 7574  'obtenir l'ID ut
+00002620: 696c 6973 6174 6575 7220 706f 7572 206c  ilisateur pour l
+00002630: 6120 6465 6d61 6e64 6520 656e 2063 6f75  a demande en cou
+00002640: 7273 220a 0a23 3a20 6c74 695f 636f 6e73  rs"..#: lti_cons
+00002650: 756d 6572 2e70 790a 232c 2070 7974 686f  umer.py.#, pytho
+00002660: 6e2d 6272 6163 652d 666f 726d 6174 0a6d  n-brace-format.m
+00002670: 7367 6964 2022 220a 2243 6f75 6c64 206e  sgid ""."Could n
+00002680: 6f74 2070 6172 7365 2063 7573 746f 6d20  ot parse custom 
+00002690: 7061 7261 6d65 7465 723a 207b 6375 7374  parameter: {cust
+000026a0: 6f6d 5f70 6172 616d 6574 6572 7d2e 2053  om_parameter}. S
+000026b0: 686f 756c 6420 6265 205c 2278 3d79 5c22  hould be \"x=y\"
+000026c0: 2022 0a22 7374 7269 6e67 2e22 0a6d 7367   "."string.".msg
+000026d0: 7374 7220 2249 6d70 6f73 7369 626c 6520  str "Impossible 
+000026e0: 6427 616e 616c 7973 6572 206c 6520 7061  d'analyser le pa
+000026f0: 7261 6dc3 a874 7265 2070 6572 736f 6e6e  ram..tre personn
+00002700: 616c 6973 c3a9 3a20 7b63 7573 746f 6d5f  alis..: {custom_
+00002710: 7061 7261 6d65 7465 727d 2e20 4465 7672  parameter}. Devr
+00002720: 6169 7420 c3aa 7472 6520 756e 6520 6368  ait ..tre une ch
+00002730: 61c3 ae6e 6520 5c22 783d 795c 222e 220a  a..ne \"x=y\".".
+00002740: 0a23 3a20 6c74 695f 636f 6e73 756d 6572  .#: lti_consumer
+00002750: 2e70 790a 6d73 6769 6420 225b 4c54 495d  .py.msgid "[LTI]
+00002760: 3a20 5265 616c 2075 7365 7220 6e6f 7420  : Real user not 
+00002770: 666f 756e 6420 6167 6169 6e73 7420 616e  found against an
+00002780: 6f6e 5f69 643a 207b 7d22 0a6d 7367 7374  on_id: {}".msgst
+00002790: 7220 225b 4c54 495d 3a20 5574 696c 6973  r "[LTI]: Utilis
+000027a0: 6174 6575 7220 72c3 a965 6c20 6e6f 6e20  ateur r..el non 
+000027b0: 7472 6f75 76c3 a920 706f 7572 2061 6e6f  trouv.. pour ano
+000027c0: 6e5f 6964 3a20 7b7d 220a                 n_id: {}".
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/es_419/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
-"PO-Revision-Date: 2017-09-23 22:34+0000\n"
-"Last-Translator: qualityalltext <quality@alltext.co.il>\n"
-"Language-Team: Hebrew (http://www.transifex.com/open-edx/xblocks/language/"
+"Report-Msgid-Bugs-To: \n"
+"PO-Revision-Date: 2016-06-08 14:38+0000\n"
+"Last-Translator: qualityalltext <quality@alltext.co.il>, 2016\n"
+"Language-Team: Hebrew (http://app.transifex.com/open-edx/xblocks/language/"
 "he/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: he\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n == 2 && n % "
 "1 == 0) ? 1: (n % 10 == 0 && n % 1 == 0 && n > 10) ? 2 : 3;\n"
-"X-Generator: Poedit 1.8.7\n"
-"X-Poedit-Basepath: ../../..\n"
-"X-Poedit-SearchPath-0: lti_consumer.py\n"
 
 msgid "Accept grades past deadline"
 msgstr "קבל ציונים לאחר המועד הסופי"
 
 msgid ""
 "Add the key/value pair for any custom parameters, such as the page your e-"
 "book should open to or the background color for this component. Ex. "
@@ -34,27 +32,14 @@
 
 msgid "Comment as returned from grader, LTI2.0 spec"
 msgstr "הערה חוזרת ממעניק הציון, LTI2.0 spec"
 
 msgid "Could not get user id for current request"
 msgstr "לא ניתן להשיג מזהה משתמש לבקשה הנוכחית"
 
-msgid ""
-"Could not parse LTI passport: {lti_passport}. Should be \"id:key:secret\" "
-"string."
-msgstr ""
-"ניתוח LTI passport נכשל: {lti_passport}. צריך להיות במחרוזת \"id:key:"
-"secret\"."
-
-msgid ""
-"Could not parse custom parameter: {custom_parameter}. Should be \"x=y\" "
-"string."
-msgstr ""
-"ניתוח פרמטר מותאם אישית נכשל: {custom_parameter}. צריך להיות במחרוזת \"x=y\"."
-
 msgid "Custom Parameters"
 msgstr "פרמטרים מותאמים אישית"
 
 msgid "Display Name"
 msgstr "הצג שם"
 
 msgid ""
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/he/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/hi/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ja_JP/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ko_KR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,22 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: XBlocks\n"
-"PO-Revision-Date: 2018-10-02 18:41+0000\n"
-"Last-Translator: Fabio Oliveira Silva <fabio.oliv.silva@gmail.com>\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/open-edx/"
+"Report-Msgid-Bugs-To: \n"
+"PO-Revision-Date: 2016-06-08 14:38+0000\n"
+"Last-Translator: Simone Baldissera, 2021\n"
+"Language-Team: Portuguese (Brazil) (http://app.transifex.com/open-edx/"
 "xblocks/language/pt_BR/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Language: pt_BR\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
-"X-Generator: Poedit 1.8.7\n"
-"X-Poedit-Basepath: ../../..\n"
-"X-Poedit-SearchPath-0: lti_consumer.py\n"
+"Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
+"1000000 == 0 ? 1 : 2;\n"
 
 msgid "Display Name"
 msgstr "Nome de exibição"
 
 msgid ""
 "Enter the name that students see for this component. Analytics reports may "
 "also use the display name to identify this component."
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.mo` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: XBlocks*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0300 0000 2c00 0000 0000 0000  $.......,.......
-00000020: 3800 0000 1f02 0000 3900 0000 0100 0000  8.......9.......
+00000020: 3800 0000 f201 0000 3900 0000 0100 0000  8.......9.......
 00000030: 0000 0000 0000 0000 0050 726f 6a65 6374  .........Project
 00000040: 2d49 642d 5665 7273 696f 6e3a 2058 426c  -Id-Version: XBl
-00000050: 6f63 6b73 0a50 4f2d 5265 7669 7369 6f6e  ocks.PO-Revision
-00000060: 2d44 6174 653a 2032 3031 362d 3036 2d30  -Date: 2016-06-0
-00000070: 3820 3134 3a33 382b 3030 3030 0a4c 6173  8 14:38+0000.Las
-00000080: 742d 5472 616e 736c 6174 6f72 3a20 0a4c  t-Translator: .L
-00000090: 616e 6775 6167 652d 5465 616d 3a20 5275  anguage-Team: Ru
-000000a0: 7373 6961 6e20 2868 7474 703a 2f2f 7777  ssian (http://ww
-000000b0: 772e 7472 616e 7369 6665 782e 636f 6d2f  w.transifex.com/
-000000c0: 6f70 656e 2d65 6478 2f78 626c 6f63 6b73  open-edx/xblocks
-000000d0: 2f6c 616e 6775 6167 652f 7275 2f29 0a4d  /language/ru/).M
-000000e0: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
-000000f0: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
-00000100: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
-00000110: 6574 3d55 5446 2d38 0a43 6f6e 7465 6e74  et=UTF-8.Content
-00000120: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
-00000130: 6e67 3a20 3862 6974 0a4c 616e 6775 6167  ng: 8bit.Languag
-00000140: 653a 2072 750a 506c 7572 616c 2d46 6f72  e: ru.Plural-For
-00000150: 6d73 3a20 6e70 6c75 7261 6c73 3d34 3b20  ms: nplurals=4; 
-00000160: 706c 7572 616c 3d28 6e25 3130 3d3d 3120  plural=(n%10==1 
-00000170: 2626 206e 2531 3030 213d 3131 203f 2030  && n%100!=11 ? 0
-00000180: 203a 206e 2531 303e 3d32 2026 2620 6e25   : n%10>=2 && n%
-00000190: 3130 3c3d 3420 2626 2028 6e25 3130 303c  10<=4 && (n%100<
-000001a0: 3132 207c 7c20 6e25 3130 303e 3134 2920  12 || n%100>14) 
-000001b0: 3f20 3120 3a20 6e25 3130 3d3d 3020 7c7c  ? 1 : n%10==0 ||
-000001c0: 2028 6e25 3130 3e3d 3520 2626 206e 2531   (n%10>=5 && n%1
-000001d0: 303c 3d39 2920 7c7c 2028 6e25 3130 303e  0<=9) || (n%100>
-000001e0: 3d31 3120 2626 206e 2531 3030 3c3d 3134  =11 && n%100<=14
-000001f0: 293f 2032 203a 2033 293b 0a58 2d47 656e  )? 2 : 3);.X-Gen
-00000200: 6572 6174 6f72 3a20 506f 6564 6974 2031  erator: Poedit 1
-00000210: 2e38 2e37 0a58 2d50 6f65 6469 742d 4261  .8.7.X-Poedit-Ba
-00000220: 7365 7061 7468 3a20 2e2e 2f2e 2e2f 2e2e  sepath: ../../..
-00000230: 0a58 2d50 6f65 6469 742d 5365 6172 6368  .X-Poedit-Search
-00000240: 5061 7468 2d30 3a20 6c74 695f 636f 6e73  Path-0: lti_cons
-00000250: 756d 6572 2e70 790a 00                   umer.py..
+00000050: 6f63 6b73 0a52 6570 6f72 742d 4d73 6769  ocks.Report-Msgi
+00000060: 642d 4275 6773 2d54 6f3a 200a 504f 2d52  d-Bugs-To: .PO-R
+00000070: 6576 6973 696f 6e2d 4461 7465 3a20 3230  evision-Date: 20
+00000080: 3136 2d30 362d 3038 2031 343a 3338 2b30  16-06-08 14:38+0
+00000090: 3030 300a 4c61 7374 2d54 7261 6e73 6c61  000.Last-Transla
+000000a0: 746f 723a 2046 554c 4c20 4e41 4d45 203c  tor: FULL NAME <
+000000b0: 454d 4149 4c40 4144 4452 4553 533e 0a4c  EMAIL@ADDRESS>.L
+000000c0: 616e 6775 6167 652d 5465 616d 3a20 5275  anguage-Team: Ru
+000000d0: 7373 6961 6e20 2868 7474 703a 2f2f 6170  ssian (http://ap
+000000e0: 702e 7472 616e 7369 6665 782e 636f 6d2f  p.transifex.com/
+000000f0: 6f70 656e 2d65 6478 2f78 626c 6f63 6b73  open-edx/xblocks
+00000100: 2f6c 616e 6775 6167 652f 7275 2f29 0a4d  /language/ru/).M
+00000110: 494d 452d 5665 7273 696f 6e3a 2031 2e30  IME-Version: 1.0
+00000120: 0a43 6f6e 7465 6e74 2d54 7970 653a 2074  .Content-Type: t
+00000130: 6578 742f 706c 6169 6e3b 2063 6861 7273  ext/plain; chars
+00000140: 6574 3d55 5446 2d38 0a43 6f6e 7465 6e74  et=UTF-8.Content
+00000150: 2d54 7261 6e73 6665 722d 456e 636f 6469  -Transfer-Encodi
+00000160: 6e67 3a20 3862 6974 0a4c 616e 6775 6167  ng: 8bit.Languag
+00000170: 653a 2072 750a 506c 7572 616c 2d46 6f72  e: ru.Plural-For
+00000180: 6d73 3a20 6e70 6c75 7261 6c73 3d34 3b20  ms: nplurals=4; 
+00000190: 706c 7572 616c 3d28 6e25 3130 3d3d 3120  plural=(n%10==1 
+000001a0: 2626 206e 2531 3030 213d 3131 203f 2030  && n%100!=11 ? 0
+000001b0: 203a 206e 2531 303e 3d32 2026 2620 6e25   : n%10>=2 && n%
+000001c0: 3130 3c3d 3420 2626 2028 6e25 3130 303c  10<=4 && (n%100<
+000001d0: 3132 207c 7c20 6e25 3130 303e 3134 2920  12 || n%100>14) 
+000001e0: 3f20 3120 3a20 6e25 3130 3d3d 3020 7c7c  ? 1 : n%10==0 ||
+000001f0: 2028 6e25 3130 3e3d 3520 2626 206e 2531   (n%10>=5 && n%1
+00000200: 303c 3d39 2920 7c7c 2028 6e25 3130 303e  0<=9) || (n%100>
+00000210: 3d31 3120 2626 206e 2531 3030 3c3d 3134  =11 && n%100<=14
+00000220: 293f 2032 203a 2033 293b 0a00            )? 2 : 3);..
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/ru/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po` & `lti-consumer-xblock-9.0.4/lti_consumer/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer/utils.py` & `lti-consumer-xblock-9.0.4/lti_consumer/utils.py`

 * *Files identical despite different names*

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/PKG-INFO` & `lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lti-consumer-xblock
-Version: 9.0.3
+Version: 9.0.4
 Summary: This XBlock implements the consumer side of the LTI specification.
 Home-page: https://github.com/openedx/xblock-lti-consumer
 Author: Open edX project
 Author-email: oscm@edx.org
 Keywords: lti consumer xblock
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
```

### Comparing `lti-consumer-xblock-9.0.3/lti_consumer_xblock.egg-info/SOURCES.txt` & `lti-consumer-xblock-9.0.4/lti_consumer_xblock.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,27 @@
 lti_consumer/migrations/0016_lticonfiguration_lti_1p3_proctoring_enabled.py
 lti_consumer/migrations/0017_lticonfiguration_lti_1p3_redirect_uris.py
 lti_consumer/migrations/__init__.py
 lti_consumer/plugin/__init__.py
 lti_consumer/plugin/compat.py
 lti_consumer/plugin/urls.py
 lti_consumer/plugin/views.py
+lti_consumer/public/js/translations/ar/text.js
+lti_consumer/public/js/translations/en/text.js
+lti_consumer/public/js/translations/es_419/text.js
+lti_consumer/public/js/translations/fr/text.js
+lti_consumer/public/js/translations/he/text.js
+lti_consumer/public/js/translations/hi/text.js
+lti_consumer/public/js/translations/it/text.js
+lti_consumer/public/js/translations/ja/text.js
+lti_consumer/public/js/translations/ko/text.js
+lti_consumer/public/js/translations/pt_BR/text.js
+lti_consumer/public/js/translations/pt_PT/text.js
+lti_consumer/public/js/translations/ru/text.js
+lti_consumer/public/js/translations/zh_CN/text.js
 lti_consumer/signals/__init__.py
 lti_consumer/signals/signals.py
 lti_consumer/static/css/student.css
 lti_consumer/static/js/xblock_lti_consumer.js
 lti_consumer/static/js/xblock_studio_view.js
 lti_consumer/static/sass/student.scss
 lti_consumer/templates/html/lti_1p3_launch.html
@@ -116,16 +129,19 @@
 lti_consumer/tests/unit/plugin/__init__.py
 lti_consumer/tests/unit/plugin/test_proctoring.py
 lti_consumer/tests/unit/plugin/test_views.py
 lti_consumer/tests/unit/plugin/test_views_lti_ags.py
 lti_consumer/tests/unit/plugin/test_views_lti_deep_linking.py
 lti_consumer/tests/unit/plugin/test_views_lti_nrps.py
 lti_consumer/translations/config.yaml
+lti_consumer/translations/settings.py
 lti_consumer/translations/ar/LC_MESSAGES/text.mo
 lti_consumer/translations/ar/LC_MESSAGES/text.po
+lti_consumer/translations/en/LC_MESSAGES/django.mo
+lti_consumer/translations/en/LC_MESSAGES/django.po
 lti_consumer/translations/en/LC_MESSAGES/text.mo
 lti_consumer/translations/en/LC_MESSAGES/text.po
 lti_consumer/translations/es_419/LC_MESSAGES/text.mo
 lti_consumer/translations/es_419/LC_MESSAGES/text.po
 lti_consumer/translations/fr/LC_MESSAGES/text.mo
 lti_consumer/translations/fr/LC_MESSAGES/text.po
 lti_consumer/translations/fr_CA/LC_MESSAGES/text.mo
```

### Comparing `lti-consumer-xblock-9.0.3/setup.py` & `lti-consumer-xblock-9.0.4/setup.py`

 * *Files identical despite different names*

