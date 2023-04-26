# Comparing `tmp/pulp-deb-2.9.2.tar.gz` & `tmp/pulp-deb-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulp-deb-2.9.2.tar", last modified: Tue May 25 14:44:30 2021, max compression
+gzip compressed data, was "pulp-deb-2.9.3.tar", last modified: Tue Nov 16 09:44:47 2021, max compression
```

## Comparing `pulp-deb-2.9.2.tar` & `pulp-deb-2.9.3.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     9995 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (121)    18046 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      243 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)    12403 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0002_auto_20190905_1000.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0003_rename_package_field.py
--rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0004_auto_20191014_1722.py
--rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0005_rename_release_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0006_debrepository.py
--rw-r--r--   0 runner    (1001) docker     (121)     3508 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0007_create_metadata_models.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0008_debremote_gpgkey.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0009_apt_release_signing_service.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0010_debpublication_signing_service.py
--rw-r--r--   0 runner    (1001) docker     (121)     3078 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0011_rename_models_to_apt.py
--rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0012_auto_20200803_1337.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/0013_aptremote_ignore_missing_package_indices.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/models/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)      774 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     6049 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/models/signing_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      669 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17703 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/content_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/publication_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/remote_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/serializers/repository_serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12180 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/tasks/publishing.py
--rw-r--r--   0 runner    (1001) docker     (121)    27964 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/tasks/synchronizing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/
--rw-r--r--   0 runner    (1001) docker     (121)      527 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10445 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     4691 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/publication.py
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/app/viewsets/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11235 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (121)     8277 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5252 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_download_policies.py
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     7192 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_complex_dists.py
--rw-r--r--   0 runner    (1001) docker     (121)     4166 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_empty_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)     9591 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_flat_repo_format.py
--rw-r--r--   0 runner    (1001) docker     (121)     7077 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     6912 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_sync_missing_architecture.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/constants.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      666 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/setup_signing_service.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      973 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/sign_deb_release.sh
--rw-r--r--   0 runner    (1001) docker     (121)     9461 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/tests/performance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/performance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pulp_deb/tests/unit/test_serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/pulp_deb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       42 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-25 14:44:30.000000 pulp-deb-2.9.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1229 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-05-25 14:40:02.000000 pulp-deb-2.9.2/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    10067 2021-11-16 09:44:46.000000 pulp-deb-2.9.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2095 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (121)    18046 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.679676 pulp-deb-2.9.3/pulp_deb/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.679676 pulp-deb-2.9.3/pulp_deb/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.683676 pulp-deb-2.9.3/pulp_deb/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)    12403 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0002_auto_20190905_1000.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0003_rename_package_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1151 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0004_auto_20191014_1722.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1184 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0005_rename_release_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0006_debrepository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3508 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0007_create_metadata_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0008_debremote_gpgkey.py
+-rw-r--r--   0 runner    (1001) docker     (121)      752 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0009_apt_release_signing_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0010_debpublication_signing_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3078 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0011_rename_models_to_apt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5077 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0012_auto_20200803_1337.py
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/0013_aptremote_ignore_missing_package_indices.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.683676 pulp-deb-2.9.3/pulp_deb/app/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9764 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6049 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/models/signing_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.683676 pulp-deb-2.9.3/pulp_deb/app/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)      669 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17703 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/serializers/content_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1870 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/serializers/publication_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/serializers/remote_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/serializers/repository_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.683676 pulp-deb-2.9.3/pulp_deb/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12180 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27964 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/tasks/synchronizing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/app/viewsets/
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10445 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/viewsets/content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4691 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/viewsets/publication.py
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/viewsets/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2662 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/app/viewsets/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11235 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8277 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5252 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9949 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_download_policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6907 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7192 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_complex_dists.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4166 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_empty_repository.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9591 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_flat_repo_format.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7077 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6912 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_sync_missing_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      666 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/setup_signing_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      973 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/sign_deb_release.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     9461 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/tests/performance/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/performance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/pulp_deb/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3186 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1946 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pulp_deb/tests/unit/test_serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 09:44:47.679676 pulp-deb-2.9.3/pulp_deb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2261 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2842 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/pulp_deb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-16 09:44:47.687676 pulp-deb-2.9.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1229 2021-11-16 09:44:47.000000 pulp-deb-2.9.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-16 09:44:33.000000 pulp-deb-2.9.3/unittest_requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pulp-deb-2.9.2/CHANGES.rst` & `pulp-deb-2.9.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,23 @@
    You *may* edit previous change logs to correct typos or similar.
    To learn how to add new entries see the 'Changelog Update' heading in the CONTRIBUTING.rst file.
 
    WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+2.9.3 (2021-11-16)
+==================
+
+No significant changes.
+
+
+----
+
+
 2.9.2 (2021-05-25)
 ==================
 
 Compatible with: ``pulpcore>=3.7,<3.11``
 
 Bugfixes
 --------
```

### Comparing `pulp-deb-2.9.2/COMMITMENT` & `pulp-deb-2.9.3/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/COPYRIGHT` & `pulp-deb-2.9.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/LICENSE` & `pulp-deb-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/PKG-INFO` & `pulp-deb-2.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 Metadata-Version: 2.1
 Name: pulp-deb
-Version: 2.9.2
+Version: 2.9.3
 Summary: pulp-deb plugin for the Pulp Project
 Home-page: https://pulpproject.org
 Author: Matthias Dellweg
 Author-email: dellweg@atix.de
 License: GPLv2+
+Description: # pulp_deb
+        
+        ![main branch status](https://github.com/pulp/pulp_deb/workflows/Pulp%20CI/badge.svg)
+        ![release status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Release%20CI/CD/badge.svg)
+        ![nightly status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Nightly%20CI/CD/badge.svg)
+        ![python versions](https://img.shields.io/pypi/pyversions/pulp_deb.svg)
+        
+        A Pulp plugin to host APT repositories.
+        
+        Visit the [Pulp project homepage][1] or see the [plugin documentation][2] for more information.
+        If you want to report a bug, see the [issue tracker][3].
+        
+        The most important places:
+        
+        * The [Pulp project homepage][1].
+        * The [plugin documentation][2].
+        * The [plugin issue tracker][3].
+        * The [plugin source repository][4].
+        * The [plugin GitHub actions page][8].
+        * Released [python packages on pypi.org][5].
+        * The [pulp-deb-client Python package][6] (contains API bindings for Python).
+        * The [pulp-deb-client Ruby Gem][7] (contains API bindings for Ruby).
+        
+        [1]: https://pulpproject.org
+        [2]: https://pulp-deb.readthedocs.io/en/latest/
+        [3]: https://pulp.plan.io/projects/pulp_deb/issues/
+        [4]: https://github.com/pulp/pulp_deb
+        [5]: https://pypi.org/project/pulp-deb/
+        [6]: https://pypi.org/project/pulp-deb-client/
+        [7]: https://rubygems.org/gems/pulp_deb_client
+        [8]: https://github.com/pulp/pulp_deb/actions
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pulp_deb
-
-![main branch status](https://github.com/pulp/pulp_deb/workflows/Pulp%20CI/badge.svg)
-![release status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Release%20CI/CD/badge.svg)
-![nightly status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Nightly%20CI/CD/badge.svg)
-![python versions](https://img.shields.io/pypi/pyversions/pulp_deb.svg)
-
-A Pulp plugin to host APT repositories.
-
-Visit the [Pulp project homepage][1] or see the [plugin documentation][2] for more information.
-If you want to report a bug, see the [issue tracker][3].
-
-The most important places:
-
-* The [Pulp project homepage][1].
-* The [plugin documentation][2].
-* The [plugin issue tracker][3].
-* The [plugin source repository][4].
-* The [plugin GitHub actions page][8].
-* Released [python packages on pypi.org][5].
-* The [pulp-deb-client Python package][6] (contains API bindings for Python).
-* The [pulp-deb-client Ruby Gem][7] (contains API bindings for Ruby).
-
-[1]: https://pulpproject.org
-[2]: https://pulp-deb.readthedocs.io/en/latest/
-[3]: https://pulp.plan.io/projects/pulp_deb/issues/
-[4]: https://github.com/pulp/pulp_deb
-[5]: https://pypi.org/project/pulp-deb/
-[6]: https://pypi.org/project/pulp-deb-client/
-[7]: https://rubygems.org/gems/pulp_deb_client
-[8]: https://github.com/pulp/pulp_deb/actions
-
-
```

### Comparing `pulp-deb-2.9.2/README.md` & `pulp-deb-2.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0001_initial.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0003_rename_package_field.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0003_rename_package_field.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0004_auto_20191014_1722.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0004_auto_20191014_1722.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0005_rename_release_file.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0005_rename_release_file.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0006_debrepository.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0006_debrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0007_create_metadata_models.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0007_create_metadata_models.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0009_apt_release_signing_service.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0009_apt_release_signing_service.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0010_debpublication_signing_service.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0010_debpublication_signing_service.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0011_rename_models_to_apt.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0011_rename_models_to_apt.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/migrations/0012_auto_20200803_1337.py` & `pulp-deb-2.9.3/pulp_deb/app/migrations/0012_auto_20200803_1337.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/models/content.py` & `pulp-deb-2.9.3/pulp_deb/app/models/content.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/models/publication.py` & `pulp-deb-2.9.3/pulp_deb/app/models/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/models/remote.py` & `pulp-deb-2.9.3/pulp_deb/app/models/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/models/repository.py` & `pulp-deb-2.9.3/pulp_deb/app/models/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/models/signing_service.py` & `pulp-deb-2.9.3/pulp_deb/app/models/signing_service.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/serializers/__init__.py` & `pulp-deb-2.9.3/pulp_deb/app/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/serializers/content_serializers.py` & `pulp-deb-2.9.3/pulp_deb/app/serializers/content_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/serializers/publication_serializers.py` & `pulp-deb-2.9.3/pulp_deb/app/serializers/publication_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/serializers/remote_serializers.py` & `pulp-deb-2.9.3/pulp_deb/app/serializers/remote_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/tasks/publishing.py` & `pulp-deb-2.9.3/pulp_deb/app/tasks/publishing.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/tasks/synchronizing.py` & `pulp-deb-2.9.3/pulp_deb/app/tasks/synchronizing.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/viewsets/__init__.py` & `pulp-deb-2.9.3/pulp_deb/app/viewsets/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/viewsets/content.py` & `pulp-deb-2.9.3/pulp_deb/app/viewsets/content.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/viewsets/publication.py` & `pulp-deb-2.9.3/pulp_deb/app/viewsets/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/viewsets/remote.py` & `pulp-deb-2.9.3/pulp_deb/app/viewsets/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/app/viewsets/repository.py` & `pulp-deb-2.9.3/pulp_deb/app/viewsets/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_crud_content_unit.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_crud_content_unit.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_crud_remotes.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_download_content.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_download_policies.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_download_policies.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_complex_dists.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_complex_dists.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_empty_repository.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_empty_repository.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_publish_flat_repo_format.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_publish_flat_repo_format.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_sync.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/api/test_sync_missing_architecture.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/api/test_sync_missing_architecture.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/constants.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/constants.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/setup_signing_service.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/setup_signing_service.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/sign_deb_release.sh` & `pulp-deb-2.9.3/pulp_deb/tests/functional/sign_deb_release.sh`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/functional/utils.py` & `pulp-deb-2.9.3/pulp_deb/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/unit/test_models.py` & `pulp-deb-2.9.3/pulp_deb/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb/tests/unit/test_serializers.py` & `pulp-deb-2.9.3/pulp_deb/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pulp_deb.egg-info/PKG-INFO` & `pulp-deb-2.9.3/pulp_deb.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 Metadata-Version: 2.1
 Name: pulp-deb
-Version: 2.9.2
+Version: 2.9.3
 Summary: pulp-deb plugin for the Pulp Project
 Home-page: https://pulpproject.org
 Author: Matthias Dellweg
 Author-email: dellweg@atix.de
 License: GPLv2+
+Description: # pulp_deb
+        
+        ![main branch status](https://github.com/pulp/pulp_deb/workflows/Pulp%20CI/badge.svg)
+        ![release status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Release%20CI/CD/badge.svg)
+        ![nightly status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Nightly%20CI/CD/badge.svg)
+        ![python versions](https://img.shields.io/pypi/pyversions/pulp_deb.svg)
+        
+        A Pulp plugin to host APT repositories.
+        
+        Visit the [Pulp project homepage][1] or see the [plugin documentation][2] for more information.
+        If you want to report a bug, see the [issue tracker][3].
+        
+        The most important places:
+        
+        * The [Pulp project homepage][1].
+        * The [plugin documentation][2].
+        * The [plugin issue tracker][3].
+        * The [plugin source repository][4].
+        * The [plugin GitHub actions page][8].
+        * Released [python packages on pypi.org][5].
+        * The [pulp-deb-client Python package][6] (contains API bindings for Python).
+        * The [pulp-deb-client Ruby Gem][7] (contains API bindings for Ruby).
+        
+        [1]: https://pulpproject.org
+        [2]: https://pulp-deb.readthedocs.io/en/latest/
+        [3]: https://pulp.plan.io/projects/pulp_deb/issues/
+        [4]: https://github.com/pulp/pulp_deb
+        [5]: https://pypi.org/project/pulp-deb/
+        [6]: https://pypi.org/project/pulp-deb-client/
+        [7]: https://rubygems.org/gems/pulp_deb_client
+        [8]: https://github.com/pulp/pulp_deb/actions
+        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# pulp_deb
-
-![main branch status](https://github.com/pulp/pulp_deb/workflows/Pulp%20CI/badge.svg)
-![release status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Release%20CI/CD/badge.svg)
-![nightly status](https://github.com/pulp/pulp_deb/workflows/Pulp%20Nightly%20CI/CD/badge.svg)
-![python versions](https://img.shields.io/pypi/pyversions/pulp_deb.svg)
-
-A Pulp plugin to host APT repositories.
-
-Visit the [Pulp project homepage][1] or see the [plugin documentation][2] for more information.
-If you want to report a bug, see the [issue tracker][3].
-
-The most important places:
-
-* The [Pulp project homepage][1].
-* The [plugin documentation][2].
-* The [plugin issue tracker][3].
-* The [plugin source repository][4].
-* The [plugin GitHub actions page][8].
-* Released [python packages on pypi.org][5].
-* The [pulp-deb-client Python package][6] (contains API bindings for Python).
-* The [pulp-deb-client Ruby Gem][7] (contains API bindings for Ruby).
-
-[1]: https://pulpproject.org
-[2]: https://pulp-deb.readthedocs.io/en/latest/
-[3]: https://pulp.plan.io/projects/pulp_deb/issues/
-[4]: https://github.com/pulp/pulp_deb
-[5]: https://pypi.org/project/pulp-deb/
-[6]: https://pypi.org/project/pulp-deb-client/
-[7]: https://rubygems.org/gems/pulp_deb_client
-[8]: https://github.com/pulp/pulp_deb/actions
-
-
```

### Comparing `pulp-deb-2.9.2/pulp_deb.egg-info/SOURCES.txt` & `pulp-deb-2.9.3/pulp_deb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/pyproject.toml` & `pulp-deb-2.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-deb-2.9.2/setup.py` & `pulp-deb-2.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.md") as description:
     long_description = description.read()
 
 setup(
     name="pulp-deb",
-    version="2.9.2",
+    version="2.9.3",
     description="pulp-deb plugin for the Pulp Project",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPLv2+",
     author="Matthias Dellweg",
     author_email="dellweg@atix.de",
     url="https://pulpproject.org",
```

