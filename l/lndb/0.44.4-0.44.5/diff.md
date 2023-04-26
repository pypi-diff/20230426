# Comparing `tmp/lndb-0.44.4.tar.gz` & `tmp/lndb-0.44.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb-0.44.4.tar", last modified: Mon Apr 24 18:20:24 2023, max compression
+gzip compressed data, was "lndb-0.44.5.tar", last modified: Wed Apr 26 03:54:37 2023, max compression
```

## Comparing `lndb-0.44.4.tar` & `lndb-0.44.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0     3832 2023-04-10 13:46:35.171473 lndb-0.44.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-01-15 12:18:16.566196 lndb-0.44.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-01-15 12:18:16.566256 lndb-0.44.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-01-15 12:18:16.566326 lndb-0.44.4/.gitignore
--rw-r--r--   0        0        0     1777 2023-04-23 22:02:46.131957 lndb-0.44.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-01-15 12:18:16.566501 lndb-0.44.4/LICENSE
--rw-r--r--   0        0        0      173 2023-03-27 04:37:15.707800 lndb-0.44.4/README.md
--rw-r--r--   0        0        0       52 2023-03-06 11:50:26.265030 lndb-0.44.4/docs/api.md
--rw-r--r--   0        0        0    47603 2023-04-24 18:20:03.159537 lndb-0.44.4/docs/changelog.md
--rw-r--r--   0        0        0     4832 2023-03-22 14:41:54.962234 lndb-0.44.4/docs/faq/check-synchronization.ipynb
--rw-r--r--   0        0        0     3334 2023-03-09 09:28:04.965028 lndb-0.44.4/docs/faq/clone.ipynb
--rw-r--r--   0        0        0     8397 2023-03-22 05:59:33.863010 lndb-0.44.4/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      166 2023-03-22 14:56:35.817208 lndb-0.44.4/docs/faq/index.md
--rw-r--r--   0        0        0     1182 2023-04-21 17:31:22.885162 lndb-0.44.4/docs/faq/manage-migrations.ipynb
--rw-r--r--   0        0        0     3248 2023-03-09 09:28:04.965998 lndb-0.44.4/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     2798 2023-04-05 05:10:26.112662 lndb-0.44.4/docs/faq/test-migrations-e2e.ipynb
--rw-r--r--   0        0        0     2073 2023-04-05 05:10:26.112933 lndb-0.44.4/docs/faq/test-migrations-unit.ipynb
--rw-r--r--   0        0        0     5163 2023-04-10 13:41:10.762652 lndb-0.44.4/docs/guide/01-setup-user.ipynb
--rw-r--r--   0        0        0    11110 2023-04-21 00:21:08.924113 lndb-0.44.4/docs/guide/02-init-instance.ipynb
--rw-r--r--   0        0        0     5355 2023-04-21 00:21:08.924266 lndb-0.44.4/docs/guide/03-load-instance.ipynb
--rw-r--r--   0        0        0     6390 2023-04-23 22:02:46.132862 lndb-0.44.4/docs/guide/04-set-storage.ipynb
--rw-r--r--   0        0        0     3746 2023-04-24 11:37:18.295952 lndb-0.44.4/docs/guide/05-schema-modules.ipynb
--rw-r--r--   0        0        0     1496 2023-03-22 05:59:33.864524 lndb-0.44.4/docs/guide/06-info.ipynb
--rw-r--r--   0        0        0     2689 2023-04-20 14:48:13.955039 lndb-0.44.4/docs/guide/07-delete.ipynb
--rw-r--r--   0        0        0      129 2023-02-16 15:52:14.590660 lndb-0.44.4/docs/guide/index.md
--rw-r--r--   0        0        0     3158 2023-04-21 17:24:54.958979 lndb-0.44.4/docs/guide/migrate.md
--rw-r--r--   0        0        0      126 2023-02-16 21:53:37.660107 lndb-0.44.4/docs/index.md
--rw-r--r--   0        0        0      118 2023-02-17 10:58:37.191812 lndb-0.44.4/lamin-project.yaml
--rw-r--r--   0        0        0     1993 2023-04-24 18:19:55.932032 lndb-0.44.4/lndb/__init__.py
--rw-r--r--   0        0        0     4507 2023-04-21 00:21:08.924595 lndb-0.44.4/lndb/__main__.py
--rw-r--r--   0        0        0      100 2023-02-12 04:51:38.272115 lndb-0.44.4/lndb/_assets/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-10 10:56:05.782722 lndb-0.44.4/lndb/_check_instance_setup.py
--rw-r--r--   0        0        0      221 2023-04-22 05:22:50.971625 lndb-0.44.4/lndb/_check_versions.py
--rw-r--r--   0        0        0      567 2023-04-08 10:27:51.832949 lndb-0.44.4/lndb/_close.py
--rw-r--r--   0        0        0     2146 2023-04-05 13:47:39.618861 lndb-0.44.4/lndb/_delete.py
--rw-r--r--   0        0        0      329 2023-04-24 17:57:29.952669 lndb-0.44.4/lndb/_info.py
--rw-r--r--   0        0        0     6051 2023-04-21 12:45:57.904490 lndb-0.44.4/lndb/_init_instance.py
--rw-r--r--   0        0        0     4003 2023-04-19 13:17:39.106450 lndb-0.44.4/lndb/_load_instance.py
--rw-r--r--   0        0        0      135 2023-04-05 05:10:26.113647 lndb-0.44.4/lndb/_migrate/__init__.py
--rw-r--r--   0        0        0      723 2023-04-05 05:10:26.113978 lndb-0.44.4/lndb/_migrate/alembic.ini
--rw-r--r--   0        0        0     3704 2023-04-24 17:08:25.124000 lndb-0.44.4/lndb/_migrate/core.py
--rw-r--r--   0        0        0     7644 2023-04-22 12:00:39.395914 lndb-0.44.4/lndb/_migrate/deploy.py
--rw-r--r--   0        0        0     3179 2023-02-16 21:53:37.661733 lndb-0.44.4/lndb/_migrate/env.py
--rw-r--r--   0        0        0      334 2023-04-24 17:25:24.780147 lndb-0.44.4/lndb/_migrate/script.py.mako
--rw-r--r--   0        0        0     4840 2023-04-05 05:10:26.114776 lndb-0.44.4/lndb/_migrate/utils.py
--rw-r--r--   0        0        0      700 2023-04-21 00:21:08.924850 lndb-0.44.4/lndb/_register_instance.py
--rw-r--r--   0        0        0     1020 2023-02-12 04:51:38.274334 lndb-0.44.4/lndb/_schema.py
--rw-r--r--   0        0        0     1830 2023-04-23 22:02:46.133073 lndb-0.44.4/lndb/_set.py
--rw-r--r--   0        0        0     2189 2023-04-18 20:05:50.820265 lndb-0.44.4/lndb/_settings.py
--rw-r--r--   0        0        0       87 2023-02-16 21:53:37.662311 lndb-0.44.4/lndb/_settings_load.py
--rw-r--r--   0        0        0       72 2023-02-16 21:53:37.662460 lndb-0.44.4/lndb/_settings_store.py
--rw-r--r--   0        0        0     3902 2023-04-21 00:21:08.925324 lndb-0.44.4/lndb/_setup_user.py
--rw-r--r--   0        0        0      533 2023-04-08 10:27:51.834128 lndb-0.44.4/lndb/dev/__init__.py
--rw-r--r--   0        0        0     4030 2023-03-27 17:35:42.591834 lndb-0.44.4/lndb/dev/_clone.py
--rw-r--r--   0        0        0     6226 2023-04-07 09:41:26.325330 lndb-0.44.4/lndb/dev/_db.py
--rw-r--r--   0        0        0     2491 2023-02-16 21:53:37.663214 lndb-0.44.4/lndb/dev/_deprecated.py
--rw-r--r--   0        0        0      240 2023-02-16 21:53:37.663286 lndb-0.44.4/lndb/dev/_docs.py
--rw-r--r--   0        0        0     5317 2023-04-08 10:27:51.834481 lndb-0.44.4/lndb/dev/_exclusion.py
--rw-r--r--   0        0        0     8764 2023-04-21 12:45:57.904794 lndb-0.44.4/lndb/dev/_settings_instance.py
--rw-r--r--   0        0        0     2629 2023-03-22 05:59:33.865686 lndb-0.44.4/lndb/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-02-16 21:53:37.663723 lndb-0.44.4/lndb/dev/_settings_save.py
--rw-r--r--   0        0        0     2314 2023-04-20 14:59:21.978668 lndb-0.44.4/lndb/dev/_settings_store.py
--rw-r--r--   0        0        0      976 2023-02-16 21:53:37.663901 lndb-0.44.4/lndb/dev/_settings_user.py
--rw-r--r--   0        0        0     2446 2023-03-21 06:52:10.981980 lndb-0.44.4/lndb/dev/_setup_knowledge.py
--rw-r--r--   0        0        0     7204 2023-04-22 19:12:00.877065 lndb-0.44.4/lndb/dev/_setup_schema.py
--rw-r--r--   0        0        0     5288 2023-04-23 22:02:46.133274 lndb-0.44.4/lndb/dev/_storage.py
--rw-r--r--   0        0        0      140 2023-02-24 20:31:36.945684 lndb-0.44.4/lndb/dev/_testdb.py
--rw-r--r--   0        0        0     2536 2023-04-08 10:27:51.835422 lndb-0.44.4/lndb/dev/upath.py
--rw-r--r--   0        0        0      356 2023-04-05 05:10:26.115134 lndb-0.44.4/lndb/test/__init__.py
--rw-r--r--   0        0        0       50 2023-02-24 20:31:36.946187 lndb-0.44.4/lndb/test/_env.py
--rw-r--r--   0        0        0     3870 2023-04-19 13:17:39.107152 lndb-0.44.4/lndb/test/_migrations_e2e.py
--rw-r--r--   0        0        0     6646 2023-04-05 05:10:26.115464 lndb-0.44.4/lndb/test/_migrations_unit.py
--rw-r--r--   0        0        0      310 2023-02-24 20:31:36.946490 lndb-0.44.4/lndb/test/_nox.py
--rw-r--r--   0        0        0      188 2023-02-22 22:13:54.788863 lndb-0.44.4/lndb/test/nox.py
--rw-r--r--   0        0        0     1003 2023-04-10 13:46:02.409554 lndb-0.44.4/noxfile.py
--rw-r--r--   0        0        0     1396 2023-04-24 02:04:37.808599 lndb-0.44.4/pyproject.toml
--rw-r--r--   0        0        0      513 2023-04-10 13:57:46.942655 lndb-0.44.4/tests/test_bionty.py
--rw-r--r--   0        0        0      680 2023-03-09 09:28:04.969725 lndb-0.44.4/tests/test_init_instance.py
--rw-r--r--   0        0        0      384 2023-04-18 16:23:45.828153 lndb-0.44.4/tests/test_notebooks.py
--rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.4/PKG-INFO
+-rw-r--r--   0        0        0     3832 2023-04-21 13:18:34.631639 lndb-0.44.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-04-21 13:18:34.631707 lndb-0.44.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-04-21 13:18:34.631769 lndb-0.44.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-04-21 13:18:34.631841 lndb-0.44.5/.gitignore
+-rw-r--r--   0        0        0     1777 2023-04-24 06:41:18.770060 lndb-0.44.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-04-21 13:18:34.632006 lndb-0.44.5/LICENSE
+-rw-r--r--   0        0        0      173 2023-04-21 13:18:34.632071 lndb-0.44.5/README.md
+-rw-r--r--   0        0        0       52 2023-04-21 13:18:34.632182 lndb-0.44.5/docs/api.md
+-rw-r--r--   0        0        0    47755 2023-04-25 20:36:08.721067 lndb-0.44.5/docs/changelog.md
+-rw-r--r--   0        0        0     4832 2023-04-21 13:18:34.632486 lndb-0.44.5/docs/faq/check-synchronization.ipynb
+-rw-r--r--   0        0        0     3334 2023-04-21 13:18:34.632563 lndb-0.44.5/docs/faq/clone.ipynb
+-rw-r--r--   0        0        0     8397 2023-04-21 13:18:34.632642 lndb-0.44.5/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      166 2023-04-21 13:18:34.632695 lndb-0.44.5/docs/faq/index.md
+-rw-r--r--   0        0        0     1182 2023-04-24 06:41:18.770918 lndb-0.44.5/docs/faq/manage-migrations.ipynb
+-rw-r--r--   0        0        0     3248 2023-04-21 13:18:34.632807 lndb-0.44.5/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     2798 2023-04-21 13:18:34.632917 lndb-0.44.5/docs/faq/test-migrations-e2e.ipynb
+-rw-r--r--   0        0        0     2073 2023-04-21 13:18:34.633000 lndb-0.44.5/docs/faq/test-migrations-unit.ipynb
+-rw-r--r--   0        0        0     5163 2023-04-21 13:18:34.633102 lndb-0.44.5/docs/guide/01-setup-user.ipynb
+-rw-r--r--   0        0        0    11110 2023-04-21 13:18:34.633175 lndb-0.44.5/docs/guide/02-init-instance.ipynb
+-rw-r--r--   0        0        0     5355 2023-04-21 13:18:34.633258 lndb-0.44.5/docs/guide/03-load-instance.ipynb
+-rw-r--r--   0        0        0     6390 2023-04-24 06:41:18.771249 lndb-0.44.5/docs/guide/04-set-storage.ipynb
+-rw-r--r--   0        0        0     3746 2023-04-24 12:01:41.554380 lndb-0.44.5/docs/guide/05-schema-modules.ipynb
+-rw-r--r--   0        0        0     1496 2023-04-21 13:18:34.633441 lndb-0.44.5/docs/guide/06-info.ipynb
+-rw-r--r--   0        0        0     2689 2023-04-21 13:18:34.633502 lndb-0.44.5/docs/guide/07-delete.ipynb
+-rw-r--r--   0        0        0      129 2023-04-21 13:18:34.633563 lndb-0.44.5/docs/guide/index.md
+-rw-r--r--   0        0        0     3158 2023-04-24 06:41:18.771572 lndb-0.44.5/docs/guide/migrate.md
+-rw-r--r--   0        0        0      126 2023-04-21 13:18:34.633686 lndb-0.44.5/docs/index.md
+-rw-r--r--   0        0        0      118 2023-04-21 13:18:34.633747 lndb-0.44.5/lamin-project.yaml
+-rw-r--r--   0        0        0     1993 2023-04-25 20:36:22.476938 lndb-0.44.5/lndb/__init__.py
+-rw-r--r--   0        0        0     4507 2023-04-21 13:18:34.633901 lndb-0.44.5/lndb/__main__.py
+-rw-r--r--   0        0        0      100 2023-04-21 13:18:34.633976 lndb-0.44.5/lndb/_assets/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-21 13:18:34.634041 lndb-0.44.5/lndb/_check_instance_setup.py
+-rw-r--r--   0        0        0      221 2023-04-25 20:35:43.603247 lndb-0.44.5/lndb/_check_versions.py
+-rw-r--r--   0        0        0      567 2023-04-21 13:18:34.634153 lndb-0.44.5/lndb/_close.py
+-rw-r--r--   0        0        0     2146 2023-04-21 13:18:34.634210 lndb-0.44.5/lndb/_delete.py
+-rw-r--r--   0        0        0      329 2023-04-25 12:02:07.055852 lndb-0.44.5/lndb/_info.py
+-rw-r--r--   0        0        0     6051 2023-04-21 13:18:34.634337 lndb-0.44.5/lndb/_init_instance.py
+-rw-r--r--   0        0        0     4003 2023-04-21 13:18:34.634409 lndb-0.44.5/lndb/_load_instance.py
+-rw-r--r--   0        0        0      135 2023-04-21 13:18:34.634486 lndb-0.44.5/lndb/_migrate/__init__.py
+-rw-r--r--   0        0        0      723 2023-04-21 13:18:34.634548 lndb-0.44.5/lndb/_migrate/alembic.ini
+-rw-r--r--   0        0        0     3704 2023-04-25 12:02:07.056289 lndb-0.44.5/lndb/_migrate/core.py
+-rw-r--r--   0        0        0     7644 2023-04-24 06:41:18.772725 lndb-0.44.5/lndb/_migrate/deploy.py
+-rw-r--r--   0        0        0     3179 2023-04-21 13:18:34.634765 lndb-0.44.5/lndb/_migrate/env.py
+-rw-r--r--   0        0        0      334 2023-04-25 12:02:07.056619 lndb-0.44.5/lndb/_migrate/script.py.mako
+-rw-r--r--   0        0        0     4840 2023-04-21 13:18:34.634902 lndb-0.44.5/lndb/_migrate/utils.py
+-rw-r--r--   0        0        0      700 2023-04-21 13:18:34.634957 lndb-0.44.5/lndb/_register_instance.py
+-rw-r--r--   0        0        0     1020 2023-04-21 13:18:34.635011 lndb-0.44.5/lndb/_schema.py
+-rw-r--r--   0        0        0     1830 2023-04-24 06:41:18.772972 lndb-0.44.5/lndb/_set.py
+-rw-r--r--   0        0        0     2189 2023-04-21 13:18:34.635125 lndb-0.44.5/lndb/_settings.py
+-rw-r--r--   0        0        0       87 2023-04-21 13:18:34.635180 lndb-0.44.5/lndb/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-04-21 13:18:34.635232 lndb-0.44.5/lndb/_settings_store.py
+-rw-r--r--   0        0        0     3902 2023-04-21 13:18:34.635297 lndb-0.44.5/lndb/_setup_user.py
+-rw-r--r--   0        0        0      533 2023-04-21 13:18:34.635390 lndb-0.44.5/lndb/dev/__init__.py
+-rw-r--r--   0        0        0     4030 2023-04-21 13:18:34.635455 lndb-0.44.5/lndb/dev/_clone.py
+-rw-r--r--   0        0        0     6226 2023-04-21 13:18:34.635521 lndb-0.44.5/lndb/dev/_db.py
+-rw-r--r--   0        0        0     2491 2023-04-21 13:18:34.635580 lndb-0.44.5/lndb/dev/_deprecated.py
+-rw-r--r--   0        0        0      240 2023-04-21 13:18:34.635632 lndb-0.44.5/lndb/dev/_docs.py
+-rw-r--r--   0        0        0     5317 2023-04-21 13:18:34.635702 lndb-0.44.5/lndb/dev/_exclusion.py
+-rw-r--r--   0        0        0     8764 2023-04-21 13:18:34.635786 lndb-0.44.5/lndb/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2629 2023-04-21 13:18:34.635856 lndb-0.44.5/lndb/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-04-21 13:18:34.636120 lndb-0.44.5/lndb/dev/_settings_save.py
+-rw-r--r--   0        0        0     2314 2023-04-21 13:18:34.636185 lndb-0.44.5/lndb/dev/_settings_store.py
+-rw-r--r--   0        0        0      976 2023-04-21 13:18:34.636245 lndb-0.44.5/lndb/dev/_settings_user.py
+-rw-r--r--   0        0        0     2446 2023-04-21 13:18:34.636316 lndb-0.44.5/lndb/dev/_setup_knowledge.py
+-rw-r--r--   0        0        0     7204 2023-04-24 06:41:18.773287 lndb-0.44.5/lndb/dev/_setup_schema.py
+-rw-r--r--   0        0        0     5288 2023-04-24 06:41:18.773542 lndb-0.44.5/lndb/dev/_storage.py
+-rw-r--r--   0        0        0      140 2023-04-21 13:18:34.636532 lndb-0.44.5/lndb/dev/_testdb.py
+-rw-r--r--   0        0        0     2536 2023-04-21 13:18:34.636604 lndb-0.44.5/lndb/dev/upath.py
+-rw-r--r--   0        0        0      356 2023-04-21 13:18:34.636702 lndb-0.44.5/lndb/test/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-21 13:18:34.636748 lndb-0.44.5/lndb/test/_env.py
+-rw-r--r--   0        0        0     3870 2023-04-21 13:18:34.636808 lndb-0.44.5/lndb/test/_migrations_e2e.py
+-rw-r--r--   0        0        0     6646 2023-04-21 13:18:34.636877 lndb-0.44.5/lndb/test/_migrations_unit.py
+-rw-r--r--   0        0        0      310 2023-04-21 13:18:34.636938 lndb-0.44.5/lndb/test/_nox.py
+-rw-r--r--   0        0        0      188 2023-04-21 13:18:34.636995 lndb-0.44.5/lndb/test/nox.py
+-rw-r--r--   0        0        0     1003 2023-04-21 13:18:34.637059 lndb-0.44.5/noxfile.py
+-rw-r--r--   0        0        0     1396 2023-04-25 12:07:23.777541 lndb-0.44.5/pyproject.toml
+-rw-r--r--   0        0        0      513 2023-04-21 13:18:34.637215 lndb-0.44.5/tests/test_bionty.py
+-rw-r--r--   0        0        0      680 2023-04-21 13:18:34.637282 lndb-0.44.5/tests/test_init_instance.py
+-rw-r--r--   0        0        0      384 2023-04-21 13:18:34.637338 lndb-0.44.5/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1198 1970-01-01 00:00:00.000000 lndb-0.44.5/PKG-INFO
```

### Comparing `lndb-0.44.4/.github/workflows/build.yml` & `lndb-0.44.5/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/.github/workflows/latest-changes.yml` & `lndb-0.44.5/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/.gitignore` & `lndb-0.44.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/.pre-commit-config.yaml` & `lndb-0.44.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/LICENSE` & `lndb-0.44.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/changelog.md` & `lndb-0.44.5/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+⬆️ Upgrade lnhub-rest | [369](https://github.com/laminlabs/lndb/pull/369) | [fredericenard](https://github.com/fredericenard) | 2023-04-25 | 0.44.5
 ✨ Allow to set additional fsspec kwargs for cloud instances | [366](https://github.com/laminlabs/lndb/pull/366) | [Koncopd](https://github.com/Koncopd) | 2023-04-23 | 0.44.4
 ⬆️ Upgrade lnhub-rest to 0.8.2 | [365](https://github.com/laminlabs/lndb/pull/365) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.44.2
 🚸 New migration deployment logic that also factors in migration ids | [364](https://github.com/laminlabs/lndb/pull/364) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Mute warning about DB not reachable in init | [363](https://github.com/laminlabs/lndb/pull/363) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 |
 🚸 Allow registering local postgres instances on the hub | [361](https://github.com/laminlabs/lndb/pull/361) | [falexwolf](https://github.com/falexwolf) | 2023-04-21 | 0.43.0
 🚸 Add a `is_db_setup()` check after init and make it more robust | [362](https://github.com/laminlabs/lndb/pull/362) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
 👷 Remove lnhub-rest CI calls | [360](https://github.com/laminlabs/lndb/pull/360) | [falexwolf](https://github.com/falexwolf) | 2023-04-20 |
```

### Comparing `lndb-0.44.4/docs/faq/check-synchronization.ipynb` & `lndb-0.44.5/docs/faq/check-synchronization.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/clone.ipynb` & `lndb-0.44.5/docs/faq/clone.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/edge-cases-login-init.ipynb` & `lndb-0.44.5/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/manage-migrations.ipynb` & `lndb-0.44.5/docs/faq/manage-migrations.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/switch-environment.ipynb` & `lndb-0.44.5/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/test-migrations-e2e.ipynb` & `lndb-0.44.5/docs/faq/test-migrations-e2e.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/faq/test-migrations-unit.ipynb` & `lndb-0.44.5/docs/faq/test-migrations-unit.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/01-setup-user.ipynb` & `lndb-0.44.5/docs/guide/01-setup-user.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/02-init-instance.ipynb` & `lndb-0.44.5/docs/guide/02-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/03-load-instance.ipynb` & `lndb-0.44.5/docs/guide/03-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/04-set-storage.ipynb` & `lndb-0.44.5/docs/guide/04-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/05-schema-modules.ipynb` & `lndb-0.44.5/docs/guide/05-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/06-info.ipynb` & `lndb-0.44.5/docs/guide/06-info.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/07-delete.ipynb` & `lndb-0.44.5/docs/guide/07-delete.ipynb`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/docs/guide/migrate.md` & `lndb-0.44.5/docs/guide/migrate.md`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/__init__.py` & `lndb-0.44.5/lndb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 .. autosummary::
    :toctree:
 
    dev
 """
 
-__version__ = "0.44.4"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.44.5"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import sys
 from os import name as _os_name
 
 from . import _check_versions  # noqa
 from . import dev, test
 from ._close import close  # noqa
```

### Comparing `lndb-0.44.4/lndb/__main__.py` & `lndb-0.44.5/lndb/__main__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_check_instance_setup.py` & `lndb-0.44.5/lndb/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_close.py` & `lndb-0.44.5/lndb/_close.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_delete.py` & `lndb-0.44.5/lndb/_delete.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_init_instance.py` & `lndb-0.44.5/lndb/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_load_instance.py` & `lndb-0.44.5/lndb/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_migrate/alembic.ini` & `lndb-0.44.5/lndb/_migrate/alembic.ini`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_migrate/core.py` & `lndb-0.44.5/lndb/_migrate/core.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_migrate/deploy.py` & `lndb-0.44.5/lndb/_migrate/deploy.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_migrate/env.py` & `lndb-0.44.5/lndb/_migrate/env.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_migrate/utils.py` & `lndb-0.44.5/lndb/_migrate/utils.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_register_instance.py` & `lndb-0.44.5/lndb/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_schema.py` & `lndb-0.44.5/lndb/_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_set.py` & `lndb-0.44.5/lndb/_set.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_settings.py` & `lndb-0.44.5/lndb/_settings.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/_setup_user.py` & `lndb-0.44.5/lndb/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/__init__.py` & `lndb-0.44.5/lndb/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_clone.py` & `lndb-0.44.5/lndb/dev/_clone.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_db.py` & `lndb-0.44.5/lndb/dev/_db.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_deprecated.py` & `lndb-0.44.5/lndb/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_exclusion.py` & `lndb-0.44.5/lndb/dev/_exclusion.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_settings_instance.py` & `lndb-0.44.5/lndb/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_settings_load.py` & `lndb-0.44.5/lndb/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_settings_save.py` & `lndb-0.44.5/lndb/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_settings_store.py` & `lndb-0.44.5/lndb/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_settings_user.py` & `lndb-0.44.5/lndb/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_setup_knowledge.py` & `lndb-0.44.5/lndb/dev/_setup_knowledge.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_setup_schema.py` & `lndb-0.44.5/lndb/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/_storage.py` & `lndb-0.44.5/lndb/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/dev/upath.py` & `lndb-0.44.5/lndb/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/test/_migrations_e2e.py` & `lndb-0.44.5/lndb/test/_migrations_e2e.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/lndb/test/_migrations_unit.py` & `lndb-0.44.5/lndb/test/_migrations_unit.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/noxfile.py` & `lndb-0.44.5/noxfile.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/pyproject.toml` & `lndb-0.44.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
     # PINNED internal LAMIN dependency
     # !!! lnhub_rest cannot be pinned in LaminDB !!!
     # !!! LaminDB should not directly depend on lnhub_rest !!!
-    "lnhub_rest==0.8.2",
+    "lnhub_rest==0.9.2",
     # NO other Lamin packages should be pinned or even be a dependency
     "laminci>=0.3.0",  # disentangle over time
     "lnschema_core>=0.28.0",
     "lamin_logger>=0.2.3",
     # External dependencies
     "pytest_alembic==0.9.1",  # let's pin this as we use internals
     "cloudpathlib",  # we can remove this once lnschema-core is released (2023-04-07)
```

### Comparing `lndb-0.44.4/tests/test_bionty.py` & `lndb-0.44.5/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/tests/test_init_instance.py` & `lndb-0.44.5/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lndb-0.44.4/PKG-INFO` & `lndb-0.44.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: lndb
-Version: 0.44.4
+Version: 0.44.5
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
-Requires-Dist: lnhub_rest==0.8.2
+Requires-Dist: lnhub_rest==0.9.2
 Requires-Dist: laminci>=0.3.0
 Requires-Dist: lnschema_core>=0.28.0
 Requires-Dist: lamin_logger>=0.2.3
 Requires-Dist: pytest_alembic==0.9.1
 Requires-Dist: cloudpathlib
 Requires-Dist: sqlmodel>=0.0.8
 Requires-Dist: psycopg2-binary
```

