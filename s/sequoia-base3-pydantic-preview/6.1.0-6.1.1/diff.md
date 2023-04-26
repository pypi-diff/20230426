# Comparing `tmp/sequoia_base3_pydantic_preview-6.1.0.tar.gz` & `tmp/sequoia_base3_pydantic_preview-6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequoia_base3_pydantic_preview-6.1.0.tar", max compression
+gzip compressed data, was "sequoia_base3_pydantic_preview-6.1.1.tar", max compression
```

## Comparing `sequoia_base3_pydantic_preview-6.1.0.tar` & `sequoia_base3_pydantic_preview-6.1.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0      598 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/README.rst
--rw-r--r--   0        0        0     1732 2023-04-26 14:57:57.545468 sequoia_base3_pydantic_preview-6.1.0/pyproject.toml
--rw-r--r--   0        0        0      294 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/__init__.py
--rw-r--r--   0        0        0     3550 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/__main__.py
--rw-r--r--   0        0        0      133 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/__init__.py
--rw-r--r--   0        0        0     6010 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/base.py
--rw-r--r--   0        0        0     5739 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/dry_run.py
--rw-r--r--   0        0        0      179 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/index.py
--rw-r--r--   0        0        0     2104 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/monitoring.py
--rw-r--r--   0        0        0     4486 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/config.py
--rw-r--r--   0        0        0     1428 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/context.py
--rw-r--r--   0        0        0     5721 2023-04-26 09:46:22.917737 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/errors.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/__init__.py
--rw-r--r--   0        0        0     1319 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/bitmask.py
--rw-r--r--   0        0        0    24808 2023-04-24 12:22:32.444140 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/colander.py
--rw-r--r--   0        0        0    11666 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/cornice.py
--rw-r--r--   0        0        0     3061 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/i18n.py
--rw-r--r--   0        0        0      726 2023-04-26 14:52:20.121612 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/__init__.py
--rw-r--r--   0        0        0     5576 2023-04-26 14:52:20.124945 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/decorators.py
--rw-r--r--   0        0        0      635 2023-04-26 14:45:48.380078 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/pagination.py
--rw-r--r--   0        0        0     3361 2023-04-26 13:57:22.812111 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/renderer.py
--rw-r--r--   0        0        0     3105 2023-04-26 14:52:15.711562 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/request_validator.py
--rw-r--r--   0        0        0     1439 2023-04-26 14:56:59.364801 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/response_schema.py
--rw-r--r--   0        0        0     7952 2023-04-24 12:21:54.006923 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/translations.py
--rw-r--r--   0        0        0     1176 2023-04-24 12:22:54.191119 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/types.py
--rw-r--r--   0        0        0      758 2023-04-24 12:21:54.006923 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/typing.py
--rw-r--r--   0        0        0     8435 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pyramid.py
--rw-r--r--   0        0        0      236 2023-04-24 12:24:11.235556 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/__init__.py
--rw-r--r--   0        0        0    12052 2023-04-25 09:42:34.624381 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/colander.py
--rw-r--r--   0        0        0     1320 2023-04-26 14:49:05.026063 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/encoder.py
--rw-r--r--   0        0        0      290 2023-04-25 09:41:56.397279 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/predicate.py
--rw-r--r--   0        0        0     1328 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/settings.py
--rw-r--r--   0        0        0    22130 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/sqla.py
--rw-r--r--   0        0        0     2784 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4169 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     2762 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4198 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0      677 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     3303 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     2963 2023-04-21 09:15:11.755275 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4406 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     3183 2023-04-21 09:15:11.755275 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4628 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     2985 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/sequoia.base3.pot
--rw-r--r--   0        0        0     2728 2023-04-21 09:15:11.761942 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4165 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     2729 2023-04-21 09:15:11.761942 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.mo
--rw-r--r--   0        0        0     4168 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.po
--rw-r--r--   0        0        0     4081 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/sentry.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/__init__.py
--rw-r--r--   0        0        0     3522 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/case.py
--rw-r--r--   0        0        0       95 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/fixtures/__init__.py
--rw-r--r--   0        0        0     4867 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/fixtures/base.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/__init__.py
--rw-r--r--   0        0        0      222 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/authenticated_users.json
--rw-r--r--   0        0        0    12929 2023-04-21 12:30:00.416871 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/dummy.py
--rw-r--r--   0        0        0    10358 2023-04-26 14:30:01.793476 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/dummy_pydantic.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/locales/.empty
--rw-r--r--   0        0        0     2234 2023-04-26 09:35:28.946859 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_accept.py
--rw-r--r--   0        0        0     7985 2023-04-26 09:35:29.026860 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_base.py
--rw-r--r--   0        0        0    17170 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_bound_schema.py
--rw-r--r--   0        0        0     8424 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_dry_run.py
--rw-r--r--   0        0        0      595 2023-04-26 10:37:47.113224 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_empty_body.py
--rw-r--r--   0        0        0     7970 2023-04-26 14:17:06.287881 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_errors.py
--rw-r--r--   0        0        0      205 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_index.py
--rw-r--r--   0        0        0     1869 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_monitoring.py
--rw-r--r--   0        0        0     1125 2023-04-26 09:35:28.943525 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_types.py
--rw-r--r--   0        0        0     2074 2023-04-26 08:58:21.386455 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/__init__.py
--rw-r--r--   0        0        0      637 2023-04-26 09:34:02.302038 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/conftest.py
--rw-r--r--   0        0        0      155 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/json/dummy.json
--rw-r--r--   0        0        0     1712 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/sqlalchemy.py
--rw-r--r--   0        0        0    29908 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_colander.py
--rw-r--r--   0        0        0     6205 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_cornice.py
--rw-r--r--   0        0        0     1500 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_fixtures.py
--rw-r--r--   0        0        0     3352 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_i18n.py
--rw-r--r--   0        0        0     1264 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_missing_country.py
--rw-r--r--   0        0        0    12831 2023-04-26 14:46:25.457256 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_pydantic_request.py
--rw-r--r--   0        0        0    14381 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_pyramid.py
--rw-r--r--   0        0        0    11687 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_renderer.py
--rw-r--r--   0        0        0     5718 2023-04-26 10:01:47.949018 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_renderer_pydantic.py
--rw-r--r--   0        0        0     1112 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_settings.py
--rw-r--r--   0        0        0     6529 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_sqla.py
--rw-r--r--   0        0        0       58 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/yaml/mini_dummy.yaml
--rw-r--r--   0        0        0      922 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/test_config.py
--rw-r--r--   0        0        0     1898 2023-04-24 14:00:56.847386 sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/wsgi.py
--rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 sequoia_base3_pydantic_preview-6.1.0/PKG-INFO
+-rw-r--r--   0        0        0      598 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/README.rst
+-rw-r--r--   0        0        0     1732 2023-04-26 16:27:26.761406 sequoia_base3_pydantic_preview-6.1.1/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/__init__.py
+-rw-r--r--   0        0        0     3550 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/__main__.py
+-rw-r--r--   0        0        0      133 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/__init__.py
+-rw-r--r--   0        0        0     6010 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/base.py
+-rw-r--r--   0        0        0     5739 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/dry_run.py
+-rw-r--r--   0        0        0      179 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/index.py
+-rw-r--r--   0        0        0     2104 2023-03-20 09:57:41.385404 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/monitoring.py
+-rw-r--r--   0        0        0     4486 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/config.py
+-rw-r--r--   0        0        0     1428 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/context.py
+-rw-r--r--   0        0        0     5721 2023-04-26 09:46:22.917737 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/errors.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/__init__.py
+-rw-r--r--   0        0        0     1319 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/bitmask.py
+-rw-r--r--   0        0        0    24808 2023-04-24 12:22:32.444140 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/colander.py
+-rw-r--r--   0        0        0    11666 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/cornice.py
+-rw-r--r--   0        0        0     3061 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/i18n.py
+-rw-r--r--   0        0        0      923 2023-04-26 15:19:09.426900 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/__init__.py
+-rw-r--r--   0        0        0     5709 2023-04-26 16:26:24.073939 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/decorators.py
+-rw-r--r--   0        0        0      635 2023-04-26 14:45:48.380078 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/pagination.py
+-rw-r--r--   0        0        0     3388 2023-04-26 16:07:37.476390 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/renderer.py
+-rw-r--r--   0        0        0     3105 2023-04-26 14:52:15.711562 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/request_validator.py
+-rw-r--r--   0        0        0     1439 2023-04-26 14:56:59.364801 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/response_schema.py
+-rw-r--r--   0        0        0     7952 2023-04-24 12:21:54.006923 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/translations.py
+-rw-r--r--   0        0        0     1176 2023-04-24 12:22:54.191119 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/types.py
+-rw-r--r--   0        0        0      758 2023-04-24 12:21:54.006923 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/typing.py
+-rw-r--r--   0        0        0     8435 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pyramid.py
+-rw-r--r--   0        0        0      236 2023-04-24 12:24:11.235556 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/__init__.py
+-rw-r--r--   0        0        0    12052 2023-04-25 09:42:34.624381 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/colander.py
+-rw-r--r--   0        0        0     1320 2023-04-26 14:49:05.026063 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/encoder.py
+-rw-r--r--   0        0        0      290 2023-04-25 09:41:56.397279 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/predicate.py
+-rw-r--r--   0        0        0     1328 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/settings.py
+-rw-r--r--   0        0        0    22130 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/sqla.py
+-rw-r--r--   0        0        0     2784 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4169 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     2762 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4198 2023-02-21 10:58:14.998948 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0      677 2023-04-21 09:15:11.751942 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     3303 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     2963 2023-04-21 09:15:11.755275 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4406 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     3183 2023-04-21 09:15:11.755275 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4628 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     2985 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/sequoia.base3.pot
+-rw-r--r--   0        0        0     2728 2023-04-21 09:15:11.761942 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4165 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     2729 2023-04-21 09:15:11.761942 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.mo
+-rw-r--r--   0        0        0     4168 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.po
+-rw-r--r--   0        0        0     4081 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/sentry.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/__init__.py
+-rw-r--r--   0        0        0     3522 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/case.py
+-rw-r--r--   0        0        0       95 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0     4867 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/fixtures/base.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/__init__.py
+-rw-r--r--   0        0        0      222 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/authenticated_users.json
+-rw-r--r--   0        0        0    12929 2023-04-21 12:30:00.416871 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/dummy.py
+-rw-r--r--   0        0        0    10358 2023-04-26 14:30:01.793476 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/dummy_pydantic.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.237045 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/locales/.empty
+-rw-r--r--   0        0        0     2234 2023-04-26 09:35:28.946859 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_accept.py
+-rw-r--r--   0        0        0     7985 2023-04-26 09:35:29.026860 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_base.py
+-rw-r--r--   0        0        0    17170 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_bound_schema.py
+-rw-r--r--   0        0        0     8424 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_dry_run.py
+-rw-r--r--   0        0        0      595 2023-04-26 10:37:47.113224 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_empty_body.py
+-rw-r--r--   0        0        0     7970 2023-04-26 14:17:06.287881 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_errors.py
+-rw-r--r--   0        0        0      205 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_index.py
+-rw-r--r--   0        0        0     1869 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_monitoring.py
+-rw-r--r--   0        0        0     1125 2023-04-26 09:35:28.943525 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_types.py
+-rw-r--r--   0        0        0     2074 2023-04-26 08:58:21.386455 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      637 2023-04-26 09:34:02.302038 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/conftest.py
+-rw-r--r--   0        0        0      155 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/json/dummy.json
+-rw-r--r--   0        0        0     1712 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/sqlalchemy.py
+-rw-r--r--   0        0        0    29908 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_colander.py
+-rw-r--r--   0        0        0     6205 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_cornice.py
+-rw-r--r--   0        0        0     1500 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_fixtures.py
+-rw-r--r--   0        0        0     3352 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_i18n.py
+-rw-r--r--   0        0        0     1264 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_missing_country.py
+-rw-r--r--   0        0        0    12831 2023-04-26 14:46:25.457256 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_pydantic_request.py
+-rw-r--r--   0        0        0    14381 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_pyramid.py
+-rw-r--r--   0        0        0    11687 2023-04-24 12:24:11.232223 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_renderer.py
+-rw-r--r--   0        0        0     5718 2023-04-26 10:01:47.949018 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_renderer_pydantic.py
+-rw-r--r--   0        0        0     1112 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_settings.py
+-rw-r--r--   0        0        0     6529 2023-03-20 09:57:41.388738 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_sqla.py
+-rw-r--r--   0        0        0       58 2023-01-03 09:42:33.240378 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/yaml/mini_dummy.yaml
+-rw-r--r--   0        0        0      922 2023-02-21 10:58:15.002282 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/test_config.py
+-rw-r--r--   0        0        0     1898 2023-04-24 14:00:56.847386 sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/wsgi.py
+-rw-r--r--   0        0        0     2001 1970-01-01 00:00:00.000000 sequoia_base3_pydantic_preview-6.1.1/PKG-INFO
```

### Comparing `sequoia_base3_pydantic_preview-6.1.0/README.rst` & `sequoia_base3_pydantic_preview-6.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/pyproject.toml` & `sequoia_base3_pydantic_preview-6.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequoia-base3-pydantic-preview"
-version = "6.1.0"
+version = "6.1.1"
 description = "Base of Sequoias API services at Gandi.net"
 repository = "https://gitlab.corp.gandi.net/api-v5/sequoia.base3"
 authors = ["Chapitre-API <tech-team@lists.gandi.net>"]
 readme = "README.rst"
 classifiers=[
     "Programming Language :: Python",
     "Framework :: Pyramid",
```

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/__main__.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/__main__.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/base.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/base.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/dry_run.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/dry_run.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/api/monitoring.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/config.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/config.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/context.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/context.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/errors.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/errors.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/bitmask.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/bitmask.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/colander.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/colander.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/cornice.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/cornice.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/i18n.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/i18n.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/decorators.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from cornice.resource import add_view
 from cornice.resource import resource as cornice_resource
 from cornice.resource import view as cornice_view
 from pydantic import ValidationError
 from pyramid.httpexceptions import HTTPInternalServerError
 from pyramid.response import Response
+from pyramid.security import NO_PERMISSION_REQUIRED
 
 from sequoia.base3.context import DefaultContext
 from sequoia.base3.errors import colander_error_handler as error_handler
 from sequoia.base3.helpers.pydantic.pagination import PaginationSchema
 from sequoia.base3.helpers.pydantic.renderer import JsonRenderer
 from sequoia.base3.helpers.pydantic.request_validator import (
     build_pydantic_resource,
@@ -27,27 +28,27 @@
 
 def resource(**kwargs):
     kwargs["factory"] = DefaultContext
     kwargs["error_handler"] = error_handler
     return cornice_resource(**kwargs)
 
 
-def view(**kwargs):
+def view(permission: str = NO_PERMISSION_REQUIRED, **kwargs):
     renderer = JsonRenderer(None)
 
     def wrapper(func):
         sig = signature(func)
         params = sig.parameters.values()
         annotations = [p.annotation for p in params if p.annotation != p.empty]
         try:
             schema = annotations[0]
         except IndexError:
             raise ValueError(f"{func} is not a valid api handler")
         return_schema = sig.return_annotation
-        if not isinstance(return_schema, ResponseSchema):
+        if not issubclass(return_schema, ResponseSchema):
             return_schema = ResponseSchema[return_schema]
         kwargs["return_schema"] = return_schema
 
         def my_view(api):
             resource = build_pydantic_resource(api.request, schema)
             try:
                 ret = func(api, resource)
@@ -57,33 +58,33 @@
                     api.request.method,
                     api.request.matched_route.path,
                 )
 
                 raise HTTPInternalServerError
 
             response = api.request.response
-            response.text = renderer(ret, {"request": api.request})
+            response.text = renderer(
+                ret, {"request": api.request, "schema": return_schema}
+            )
             return api.request.response
 
         return add_view(my_view, **kwargs)
 
     return wrapper
 
 
-def paginated_view(**kw):
+def paginated_view(permission: str = NO_PERMISSION_REQUIRED, **kw):
     def wrapper(func):
         original = func
 
         @wraps(func)
-        def wrapped(self, page_info: PaginationSchema, *args, **kwargs):
-            ret = func(self, *args, **kwargs)
-            if isinstance(ret, (Response, str)):
-                return ret
+        def wrapped(self, page_info: PaginationSchema, **kwargs):
+            ret = func(self, page_info, **kwargs)
 
-            elif isinstance(ret, CollectionResponseSchema):
+            if isinstance(ret, CollectionResponseSchema):
                 xtra = self.build_list_headers(
                     page_info.page,
                     page_info.per_page,
                     page_info.sort_by,
                     ret.headers.get("X-Total-Count"),
                     ret.headers.get("X-Filtered-Count"),
                 )
@@ -99,15 +100,15 @@
                 ret.setdefault("headers", {}).update(xtra)
             else:
                 raise RuntimeError("Invalid return")
             return ret
 
         wrapped.unwrapped = original  # type: ignore
 
-        return view(**kw)(wrapped)
+        return view(permission=permission, **kw)(wrapped)
 
     return wrapper
 
 
 def legacy_view(**kwargs):
     if "renderer" not in kwargs:
         kwargs["renderer"] = "pydantic"
```

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/pagination.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/pagination.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/renderer.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     response: Response,
 ) -> str:
     if not schema:
         raise RuntimeError("Missing return_schema predicate")
     if not issubclass(schema, ResponseSchema):
         raise TypeError(f"{schema.__module__}.{schema.__name__}: not a ResponseSchema")
 
-    if isinstance(data, schema):
+    if isinstance(data, ResponseSchema):
         validated_data = data
     elif isinstance(data, schema.__fields__["body"].type_):
         validated_data = schema(body=data)
     elif isinstance(data, dict):
         validated_data = schema(**data)
     else:
         raise TypeError(f"{data}: unmanaged type")
@@ -85,18 +85,17 @@
     """
 
     def __init__(self, _renderer_helper):
         ...
 
     def __call__(self, data, context):
         request = context["request"]
+        schema = context.get("schema") or request.context.return_schema
         try:
-            resp = render_response(
-                request.context.return_schema, data, request.response
-            )
+            resp = render_response(schema, data, request.response)
         except ValidationError:
             log.exception(
                 "Unexpected exception raised while rendering response of %s %s",
                 request.method,
                 request.matched_route.path,
             )
             raise HTTPInternalServerError()
```

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/request_validator.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/request_validator.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/response_schema.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/response_schema.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/translations.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/translations.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/types.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/types.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pydantic/typing.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pydantic/typing.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/pyramid.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/pyramid.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/colander.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/colander.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/renderer/encoder.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/renderer/encoder.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/settings.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/settings.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/helpers/sqla.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/helpers/sqla.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/de/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/en/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/es/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/fr/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/ja/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/sequoia.base3.pot` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/sequoia.base3.pot`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_CN/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.mo` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.mo`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.po` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/locales/zh_TW/LC_MESSAGES/sequoia.base3.po`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/sentry.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/sentry.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/case.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/case.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/testing/fixtures/base.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/testing/fixtures/base.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/dummy.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/dummy.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/dummy_pydantic.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/dummy_pydantic.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_accept.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_accept.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_base.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_base.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_bound_schema.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_bound_schema.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_dry_run.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_dry_run.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_empty_body.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_empty_body.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_errors.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_errors.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_monitoring.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/api/test_types.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/api/test_types.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/conftest.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/conftest.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/conftest.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/sqlalchemy.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_colander.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_colander.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_cornice.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_cornice.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_fixtures.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_i18n.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_i18n.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_missing_country.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_missing_country.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_pydantic_request.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_pydantic_request.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_pyramid.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_renderer.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_renderer.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_renderer_pydantic.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_renderer_pydantic.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_settings.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_settings.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/helpers/test_sqla.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/helpers/test_sqla.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/tests/test_config.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/sequoia/base3/wsgi.py` & `sequoia_base3_pydantic_preview-6.1.1/sequoia/base3/wsgi.py`

 * *Files identical despite different names*

### Comparing `sequoia_base3_pydantic_preview-6.1.0/PKG-INFO` & `sequoia_base3_pydantic_preview-6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequoia-base3-pydantic-preview
-Version: 6.1.0
+Version: 6.1.1
 Summary: Base of Sequoias API services at Gandi.net
 Home-page: https://gitlab.corp.gandi.net/api-v5/sequoia.base3
 Author: Chapitre-API
 Author-email: tech-team@lists.gandi.net
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pyramid
 Classifier: Programming Language :: Python
```

