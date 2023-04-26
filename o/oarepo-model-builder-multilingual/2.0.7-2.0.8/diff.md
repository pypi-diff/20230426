# Comparing `tmp/oarepo-model-builder-multilingual-2.0.7.tar.gz` & `tmp/oarepo-model-builder-multilingual-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-multilingual-2.0.7.tar", last modified: Mon Apr 24 11:38:32 2023, max compression
+gzip compressed data, was "oarepo-model-builder-multilingual-2.0.8.tar", last modified: Wed Apr 26 11:16:58 2023, max compression
```

## Comparing `oarepo-model-builder-multilingual-2.0.7.tar` & `oarepo-model-builder-multilingual-2.0.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.122138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/builtin_models/i18n.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/faker.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/i18n.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/multilingual_jsonschema.json5
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/multilingual_settings.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/ui_jsonschema.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.126138 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-24 11:38:32.000000 oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-24 11:38:32.134138 oarepo-model-builder-multilingual-2.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 11:38:32.130138 oarepo-model-builder-multilingual-2.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/mock_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/model.json5
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/multilingual_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_build_from_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_i18nStr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_marshmallow_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_multi_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-24 11:36:32.000000 oarepo-model-builder-multilingual-2.0.7/tests/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.971758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builders/mult_setup_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/builtin_models/i18n.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7320 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/multilings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/i18n.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_dumper_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_multilingual.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/multilingual_jsonschema.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/multilingual_settings.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/ui_jsonschema.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/supported_langs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.975758 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-26 11:16:58.000000 oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-04-26 11:16:58.983758 oarepo-model-builder-multilingual-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 11:16:58.979758 oarepo-model-builder-multilingual-2.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/mock_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/model.json5
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/multilingual_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_build_from_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_i18nStr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_marshmallow_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_multi_facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-26 11:15:05.000000 oarepo-model-builder-multilingual-2.0.8/tests/test_ui.py
```

### Comparing `oarepo-model-builder-multilingual-2.0.7/LICENSE` & `oarepo-model-builder-multilingual-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/PKG-INFO` & `oarepo-model-builder-multilingual-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.7
+Version: 2.0.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.7/README.md` & `oarepo-model-builder-multilingual-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/datatypes/multilings.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/datatypes/multilings.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/faker.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/faker.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_multilingual_poetry.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_record_dumper_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/invenio_search_multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/invenio/templates/invenio_record_search_multilingual.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/model_preprocessors/multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/i18nStr.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/property_preprocessors/multilingual.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/utils/supported_langs.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/utils/supported_langs.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual/validation/__init__.py` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/PKG-INFO` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-multilingual
-Version: 2.0.7
+Version: 2.0.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 License-File: LICENSE
 
 # OARepo Model Builder Multilingual
 
 plugin for the [oarepo-model-builder module](https://github.com/oarepo/oarepo-model-builder) that adds support for
```

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/SOURCES.txt` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/oarepo_model_builder_multilingual.egg-info/entry_points.txt` & `oarepo-model-builder-multilingual-2.0.8/oarepo_model_builder_multilingual.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/setup.cfg` & `oarepo-model-builder-multilingual-2.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-multilingual
-version = 2.0.7
+version = 2.0.8
 description = 
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/mock_filesystem.py` & `oarepo-model-builder-multilingual-2.0.8/tests/mock_filesystem.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/multilingual_schema.py` & `oarepo-model-builder-multilingual-2.0.8/tests/multilingual_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_build_from_entrypoints.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_build_from_entrypoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
     filesystem = MockFilesystem()
     builder = create_builder_from_entrypoints(filesystem=filesystem)
 
     builder.build(schema, "")
 
     data = builder.filesystem.open(os.path.join("test", "records", "api.py")).read()
-    assert "dumper_extensions = [MultilingualDumper()]" in data
+    assert "dumper_extensions = [MultilingualSearchDumper()]" in data
 def test_dumper_file():
     schema = load_model(
         "test.yaml",
         "test",
         model_content={
             "settings": {
                 "supported-langs": {"cs": {}, "en": {}},
```

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_cfg.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_helper.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_i18nStr.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_i18nStr.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_marshmallow_ui.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_marshmallow_ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_multi_facets.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_multi_facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_runtime.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_schema.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-multilingual-2.0.7/tests/test_ui.py` & `oarepo-model-builder-multilingual-2.0.8/tests/test_ui.py`

 * *Files identical despite different names*

