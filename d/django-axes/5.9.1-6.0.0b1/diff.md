# Comparing `tmp/django-axes-5.9.1.tar.gz` & `tmp/django-axes-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-axes-5.9.1.tar", last modified: Wed Dec  2 16:01:47 2020, max compression
+gzip compressed data, was "django-axes-6.0.0b1.tar", last modified: Tue Apr 25 16:45:39 2023, max compression
```

## Comparing `django-axes-5.9.1.tar` & `django-axes-6.0.0b1.tar`

### file list

```diff
@@ -1,121 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/
--rw-r--r--   0 runner    (1001) docker     (116)       34 2020-12-02 16:01:29.000000 django-axes-5.9.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1340 2020-12-02 16:01:29.000000 django-axes-5.9.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1128 2020-12-02 16:01:29.000000 django-axes-5.9.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (116)      177 2020-12-02 16:01:29.000000 django-axes-5.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)       86 2020-12-02 16:01:29.000000 django-axes-5.9.1/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    24332 2020-12-02 16:01:29.000000 django-axes-5.9.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1184 2020-12-02 16:01:29.000000 django-axes-5.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      136 2020-12-02 16:01:29.000000 django-axes-5.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    39046 2020-12-02 16:01:47.139804 django-axes-5.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3115 2020-12-02 16:01:29.000000 django-axes-5.9.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/
--rw-r--r--   0 runner    (1001) docker     (116)      142 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2008 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (116)     1531 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)     3041 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (116)     2807 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (116)     4551 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (116)     4901 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      611 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)      380 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6752 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4529 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)    10177 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (116)      677 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (116)     4382 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (116)    16042 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)     2122 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.131804 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1950 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)     2494 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.127803 django-axes-5.9.1/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)     1450 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (116)     2072 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/management/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      404 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (116)      409 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (116)      552 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (116)      643 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (116)      579 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_user.py
--rw-r--r--   0 runner    (1001) docker     (116)      579 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (116)     2218 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     2831 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)     1723 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (116)     1948 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (116)     2197 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (116)      219 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (116)      274 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1404 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.135804 django-axes-5.9.1/axes/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5717 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2002 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      940 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (116)     5851 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (116)      752 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (116)     3600 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (116)     1944 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)    15136 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3329 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     4376 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (116)    27443 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (116)     3765 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (116)     4672 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (116)     1149 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (116)      494 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (116)    22266 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      112 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)       23 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/tests/urls_empty.py
--rw-r--r--   0 runner    (1001) docker     (116)     1656 2020-12-02 16:01:29.000000 django-axes-5.9.1/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      212 2020-12-02 16:01:29.000000 django-axes-5.9.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    39046 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2493 2020-12-02 16:01:47.000000 django-axes-5.9.1/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2020-12-02 16:01:46.000000 django-axes-5.9.1/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (116)       43 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)      648 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5518 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4307 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)    12450 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5199 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9545 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (116)     3596 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (116)      406 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1400 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/9_development.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7425 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     4011 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-02 16:01:47.139804 django-axes-5.9.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (116)   133029 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (116)      355 2020-12-02 16:01:29.000000 django-axes-5.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      254 2020-12-02 16:01:29.000000 django-axes-5.9.1/manage.py
--rw-r--r--   0 runner    (1001) docker     (116)      105 2020-12-02 16:01:29.000000 django-axes-5.9.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (116)       76 2020-12-02 16:01:29.000000 django-axes-5.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      245 2020-12-02 16:01:29.000000 django-axes-5.9.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)       44 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (116)       96 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (116)       89 2020-12-02 16:01:29.000000 django-axes-5.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-12-02 16:01:47.139804 django-axes-5.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2332 2020-12-02 16:01:29.000000 django-axes-5.9.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)      655 2020-12-02 16:01:29.000000 django-axes-5.9.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    30870 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.249824 django-axes-6.0.0b1/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19557 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.245824 django-axes-6.0.0b1/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.253824 django-axes-6.0.0b1/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36037 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 16:45:39.000000 django-axes-6.0.0b1/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    63212 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/9_development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.257824 django-axes-6.0.0b1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:39.261824 django-axes-6.0.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31476 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 16:45:25.000000 django-axes-6.0.0b1/tests/urls_empty.py
```

### Comparing `django-axes-5.9.1/.github/workflows/release.yml` & `django-axes-6.0.0b1/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,32 @@
 name: Release
 
 on:
   push:
     tags:
     - '*'
 
+permissions:
+  contents: read
+
 jobs:
   build:
     if: github.repository == 'jazzband/django-axes'
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: 3.8
 
-      - name: Get pip cache dir
-        id: pip-cache
-        run: |
-          echo "::set-output name=dir::$(pip cache dir)"
-
-      - name: Cache
-        uses: actions/cache@v2
-        with:
-          path: ${{ steps.pip-cache.outputs.dir }}
-          key: release-${{ hashFiles('**/setup.py') }}
-          restore-keys: |
-            release-
-
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U setuptools twine wheel
 
       - name: Build package
         run: |
```

### Comparing `django-axes-5.9.1/CHANGES.rst` & `django-axes-6.0.0b1/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,349 @@
 
 Changes
 =======
 
 
+6.0.0b1 (2023-04-25)
+--------------------
+
+- Set 429 as the default lockout response code. [hirotasoshu]
+
+
+5.41.1 (2023-04-16)
+-------------------
+
+- Fix sensitive parameter logging for database handler. [stereodamage]
+
+5.41.0 (2023-04-02)
+-------------------
+
+- Fix tests. [hirotasoshu]
+- Add ``AXES_CLIENT_CALLABLE`` setting. [hirotasoshu]
+- Update Python, Django, and package versions. [hramezani]
+
+
+5.40.1 (2022-11-24)
+-------------------
+
+- Fix bug in user agent request blocking. [PetrDlouhy]
+
+
+5.40.0 (2022-11-19)
+-------------------
+
+- Update packages and linters for new version support.
+  [hramezani]
+- Update documentation links.
+  [Arhell]
+- Use importlib instead of setuptools for Python 3.8+.
+  [jedie]
+- Python 3.11 support.
+  [joshuadavidthomas]
+- Documentation improvements.
+  [nsht]
+- Documentation improvements.
+  [timgates42]
+
+
+5.39.0 (2022-08-18)
+-------------------
+
+- Utilize new backend class in tests to fix false negative system check warnings.
+  [simonkern]
+
+
+5.38.0 (2022-08-16)
+-------------------
+
+- Adjust changelog so release notes are correctly visible on PyPy and released package.
+  [aleksihakli]
+
+
+5.37.0 (2022-08-16)
+-------------------
+
+- Add Django 4.1 support. PyPy 3.8 has a known issue with Django 4.1 and is exempted.
+  [hramezani]
+
+
+5.36.0 (2022-07-17)
+-------------------
+
+- Add ``AxesStandaloneBackend`` without ``ModelBackend`` dependencies.
+  [jcgiuffrida]
+
+
+5.35.0 (2022-06-01)
+-------------------
+
+- Add Arabic translations.
+  [YDA93]
+
+
+5.34.0 (2022-05-28)
+-------------------
+
+- Improve German translations.
+  [GitRon]
+
+
+5.33.0 (2022-05-16)
+-------------------
+
+- Migrate MD5 cache key digests to SHA256.
+  [aleksihakli]
+- Improve and streamline startup logging.
+  [ShaheedHaque]
+- Improve module typing.
+  [hramezani]
+- Add support for float or partial hours for ``AXES_COOLOFF_TIME``.
+  [hramezani]
+
+
+5.32.0 (2022-04-08)
+-------------------
+
+- Add support for persistent failure logging
+  where failed login attempts are persisted in the database
+  until a specific threshold is reached.
+  [p1-gdd]
+- Add support for not resetting login times when users
+  try to login during the lockout cooloff period.
+  [antoine-42]
+
+
+5.31.0 (2022-01-08)
+-------------------
+
+- Adjust version specifiers for newer Python and other package versions.
+  Set package minimum Python version to 3.7.
+  Relax ``django-ipware`` version requirements to allow newer versions.
+  [aleksihakli]
+
+
+5.30.0 (2022-01-08)
+-------------------
+
+- Fix package build error in 5.29.0 to allow publishing.
+  [aleksihakli]
+
+
+5.29.0 (2022-01-08)
+-------------------
+
+- Drop Python 3.6 support.
+  [aleksihakli]
+
+
+5.28.0 (2021-12-14)
+-------------------
+
+- Drop Django < 3.2 support.
+  [hramezani]
+- Add Django 4.0 to test matrix.
+  [hramezani]
+
+
+5.27.0 (2021-11-04)
+-------------------
+
+- Fix ``pkg_resources`` missing for package version resolution on runtime
+  due to ``setuptools`` not being a runtime dependency.
+  [asherf]
+- Add Python 3.10 and Django 3.2 support.
+  [hramezani]
+
+
+5.26.0 (2021-10-11)
+-------------------
+
+- Fix ``AXES_USERNAME_CALLABLE`` not receiving ``credentials`` attribute
+  in Axes middleware lockout response when user is locked out.
+  [rootart]
+
+
+5.25.0 (2021-09-19)
+-------------------
+
+- Fix duplicated AccessAttempts
+  with updated database model ``unique_together`` constraints
+  and data and schema migration.
+  [PetrDlouhy]
+
+
+5.24.0 (2021-09-09)
+-------------------
+
+- Use atomic transaction for updating AccessAttempts in database handler.
+  [okapies]
+
+
+5.23.0 (2021-09-02)
+-------------------
+
+- Pass ``request`` as argument to ``AXES_CLIENT_STR_CALLABLE``.
+  [sarahboyce]
+
+
+5.22.0 (2021-08-31)
+-------------------
+
+- Improve ``failures_since_start`` handling by moving the counter incrementation
+  from non-atomic Python code call to atomic database function.
+  [okapies]
+- Add publicly available ``request.axes_failures_since_start`` attribute.
+  [okapies]
+
+
+5.21.0 (2021-08-19)
+-------------------
+
+- Add configurable lockout HTTP status code responses
+  with the new ``AXES_HTTP_RESPONSE_CODE`` setting.
+  [phil-bell]
+
+
+5.20.0 (2021-06-29)
+-------------------
+
+- Improve race condition handling in e.g. multi-process environments by using
+  ``get_or_create`` for access attempt fetching and updates.
+  [uli-klank]
+
+
+5.19.0 (2021-06-16)
+-------------------
+
+- Add Polish locale.
+  [Quadric]
+
+
+5.18.0 (2021-06-09)
+-------------------
+
+- Fix ``default_auto_field`` warning.
+  [zkanda]
+
+
+5.17.0 (2021-06-05)
+-------------------
+
+- Fix ``default_app_config`` deprecation.
+  Django 3.2 automatically detects ``AppConfig`` and therefore this setting is no longer required.
+  [nikolaik]
+
+
+5.16.0 (2021-05-19)
+-------------------
+
+- Add ``AXES_CLIENT_STR_CALLABLE`` setting.
+  [smtydn]
+
+
+5.15.0 (2021-05-03)
+-------------------
+
+- Add option to cleanse sensitive GET and POST params in database handler
+  with the ``AXES_SENSITIVE_PARAMETERS`` setting.
+  [mcoconnor]
+
+
+5.14.0 (2021-04-06)
+-------------------
+
+- Improve message formatting for lockout message and translations.
+  [ashokdelphia]
+- Remove support for Django 3.0.
+  [hramezani]
+- Add support for Django 3.2.
+  [hramezani]
+
+
+5.13.1 (2021-02-22)
+-------------------
+
+- Default ``AXES_VERBOSE`` to ``AXES_ENABLED`` configuration setting,
+  disabling verbose startup logging when Axes itself is disabled.
+  [christianbundy]
+- Update documentation.
+  [KStenK]
+
+
+5.13.0 (2021-02-15)
+-------------------
+
+- Add support for resetting attempts with cache backend.
+  [nattyg93]
+
+
+5.12.0 (2021-01-07)
+-------------------
+
+- Clean up test structure and migrate tests outside
+  the main package for a smaller wheel distributions.
+  [aleksihakli]
+- Move configuration to pyproject.toml for cleaner layout.
+  [aleksihakli]
+- Clean up test settings override configuration.
+  [hramezani]
+
+
+5.11.1 (2021-01-06)
+-------------------
+
+- Fix cache entry creations for None username.
+  [cabarnes]
+
+
+5.11.0 (2021-01-05)
+-------------------
+
+- Add lockout view CORS support with ``AXES_ALLOWED_CORS_ORIGINS`` configuration flag.
+  [vladox]
+- Add missing ``@wraps`` decorator to ``axes.decorators.axes_dispatch``.
+  [aleksihakli]
+
+
+5.10.1 (2021-01-04)
+-------------------
+
+- Add ``DEFAULT_AUTO_FIELD`` to test settings.
+  [hramezani]
+- Fix documentation language.
+  [danielquinn]
+- Fix Python package version specifiers and remove redundant imports.
+  [aleksihakli]
+
+
+5.10.0 (2020-12-18)
+-------------------
+
+- Deprecate stock DRF support from 5.8.0,
+  require users to set it up per project.
+  Check the documentation for more information.
+  [aleksihakli]
+
+
 5.9.1 (2020-12-02)
 ------------------
 
 - Move tests to GitHub Actions
   [jezdez]
 - Fix running Axes code in middleware when ``AXES_ENABLED`` is ``False``.
   [ashokdelphia]
 
 
 5.9.0 (2020-11-05)
 ------------------
 
 - Add Python 3.9 support.
   [hramezani]
-- Prevent ``AccessAttempt`` creation with database handler 
-  when username is not set
-  and ``AXES_ONLY_USER_FAILURES`` setting is not set.
+- Prevent ``AccessAttempt`` creation with database handler when
+  username is not set and ``AXES_ONLY_USER_FAILURES`` setting is not set.
   [hramezani]
 
 
 5.8.0 (2020-10-16)
 ------------------
 
 - Improve Django REST Framework (DRF) integration.
```

### Comparing `django-axes-5.9.1/LICENSE` & `django-axes-6.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/README.rst` & `django-axes-6.0.0b1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,22 @@
    :target: https://github.com/jazzband/django-axes
    :alt: GitHub
 
 .. image:: https://img.shields.io/pypi/v/django-axes.svg
    :target: https://pypi.org/project/django-axes/
    :alt: PyPI release
 
+.. image:: https://img.shields.io/pypi/pyversions/django-axes.svg
+   :target: https://pypi.org/project/django-axes/
+   :alt: Supported Python versions
+
+.. image:: https://img.shields.io/pypi/djversions/django-axes.svg
+   :target: https://pypi.org/project/django-axes/
+   :alt: Supported Django versions
+
 .. image:: https://img.shields.io/readthedocs/django-axes.svg
    :target: https://django-axes.readthedocs.io/
    :alt: Documentation
 
 .. image:: https://github.com/jazzband/django-axes/workflows/Test/badge.svg
    :target: https://github.com/jazzband/django-axes/actions
    :alt: GitHub Actions
```

### Comparing `django-axes-5.9.1/axes/admin.py` & `django-axes-6.0.0b1/axes/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib import admin
+from django.http import HttpRequest
 from django.utils.translation import gettext_lazy as _
 
 from axes.conf import settings
-from axes.models import AccessAttempt, AccessLog
+from axes.models import AccessAttempt, AccessLog, AccessFailureLog
 
 
 class AccessAttemptAdmin(admin.ModelAdmin):
     list_display = (
         "attempt_time",
         "ip_address",
         "user_agent",
@@ -35,15 +36,15 @@
         "path_info",
         "attempt_time",
         "get_data",
         "post_data",
         "failures_since_start",
     ]
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request: HttpRequest) -> bool:
         return False
 
 
 class AccessLogAdmin(admin.ModelAdmin):
     list_display = (
         "attempt_time",
         "logout_time",
@@ -70,14 +71,50 @@
         "username",
         "http_accept",
         "path_info",
         "attempt_time",
         "logout_time",
     ]
 
-    def has_add_permission(self, request):
+    def has_add_permission(self, request: HttpRequest) -> bool:
+        return False
+
+
+class AccessFailureLogAdmin(admin.ModelAdmin):
+    list_display = (
+        "attempt_time",
+        "ip_address",
+        "username",
+        "user_agent",
+        "path_info",
+        "locked_out",
+    )
+
+    list_filter = ["attempt_time", "locked_out", "path_info"]
+
+    search_fields = ["ip_address", "user_agent", "username", "path_info"]
+
+    date_hierarchy = "attempt_time"
+
+    fieldsets = (
+        (None, {"fields": ("path_info",)}),
+        (_("Meta Data"), {"fields": ("user_agent", "ip_address", "http_accept")}),
+    )
+
+    readonly_fields = [
+        "user_agent",
+        "ip_address",
+        "username",
+        "http_accept",
+        "path_info",
+        "attempt_time",
+        "locked_out",
+    ]
+
+    def has_add_permission(self, request: HttpRequest) -> bool:
         return False
 
 
 if settings.AXES_ENABLE_ADMIN:
     admin.site.register(AccessAttempt, AccessAttemptAdmin)
     admin.site.register(AccessLog, AccessLogAdmin)
+    admin.site.register(AccessFailureLog, AccessFailureLogAdmin)
```

### Comparing `django-axes-5.9.1/axes/attempts.py` & `django-axes-6.0.0b1/axes/attempts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import List
 from logging import getLogger
+from typing import List, Optional
 
 from django.db.models import QuerySet
+from django.http import HttpRequest
 from django.utils.timezone import datetime, now
 
 from axes.conf import settings
-from axes.models import AccessAttempt
 from axes.helpers import get_client_username, get_client_parameters, get_cool_off
+from axes.models import AccessAttempt
 
 log = getLogger(__name__)
 
 
-def get_cool_off_threshold(attempt_time: datetime = None) -> datetime:
+def get_cool_off_threshold(attempt_time: Optional[datetime] = None) -> datetime:
     """
     Get threshold for fetching access attempts from the database.
     """
 
     cool_off = get_cool_off()
     if cool_off is None:
         raise TypeError(
@@ -23,15 +24,17 @@
         )
 
     if attempt_time is None:
         return now() - cool_off
     return attempt_time - cool_off
 
 
-def filter_user_attempts(request, credentials: dict = None) -> List[QuerySet]:
+def filter_user_attempts(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> List[QuerySet]:
     """
     Return a list querysets of AccessAttempts that match the given request and credentials.
     """
 
     username = get_client_username(request, credentials)
 
     filter_kwargs_list = get_client_parameters(
@@ -40,15 +43,17 @@
     attempts_list = [
         AccessAttempt.objects.filter(**filter_kwargs)
         for filter_kwargs in filter_kwargs_list
     ]
     return attempts_list
 
 
-def get_user_attempts(request, credentials: dict = None) -> List[QuerySet]:
+def get_user_attempts(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> List[QuerySet]:
     """
     Get list of querysets with valid user attempts that match the given request and credentials.
     """
 
     attempts_list = filter_user_attempts(request, credentials)
 
     if settings.AXES_COOLOFF_TIME is None:
@@ -58,15 +63,15 @@
         return attempts_list
 
     threshold = get_cool_off_threshold(request.axes_attempt_time)
     log.debug("AXES: Getting access attempts that are newer than %s", threshold)
     return [attempts.filter(attempt_time__gte=threshold) for attempts in attempts_list]
 
 
-def clean_expired_user_attempts(attempt_time: datetime = None) -> int:
+def clean_expired_user_attempts(attempt_time: Optional[datetime] = None) -> int:
     """
     Clean expired user attempts from the database.
     """
 
     if settings.AXES_COOLOFF_TIME is None:
         log.debug(
             "AXES: Skipping clean for expired access attempts because no AXES_COOLOFF_TIME is configured"
@@ -79,15 +84,17 @@
         "AXES: Cleaned up %s expired access attempts from database that were older than %s",
         count,
         threshold,
     )
     return count
 
 
-def reset_user_attempts(request, credentials: dict = None) -> int:
+def reset_user_attempts(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> int:
     """
     Reset all user attempts that match the given request and credentials.
     """
 
     attempts_list = filter_user_attempts(request, credentials)
 
     count = 0
```

### Comparing `django-axes-5.9.1/axes/backends.py` & `django-axes-6.0.0b1/axes/backends.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,39 @@
-from django.contrib.auth.backends import ModelBackend
+from typing import Optional
+from django.conf import settings
+from django.contrib.auth.backends import BaseBackend, ModelBackend
+from django.http import HttpRequest
 
 from axes.exceptions import (
     AxesBackendPermissionDenied,
     AxesBackendRequestParameterRequired,
 )
 from axes.handlers.proxy import AxesProxyHandler
 from axes.helpers import get_credentials, get_lockout_message, toggleable
 
 
-class AxesBackend(ModelBackend):
+class AxesStandaloneBackend(BaseBackend):
     """
     Authentication backend class that forbids login attempts for locked out users.
 
     Use this class as the first item of ``AUTHENTICATION_BACKENDS`` to
     prevent locked out users from being logged in by the Django authentication flow.
 
     .. note:: This backend does not log your user in. It monitors login attempts.
+              It also does not run any permissions checks at all.
               Authentication is handled by the following backends that are configured in ``AUTHENTICATION_BACKENDS``.
     """
 
     @toggleable
     def authenticate(
-        self, request, username: str = None, password: str = None, **kwargs: dict
+        self,
+        request: HttpRequest,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        **kwargs: dict,
     ):
         """
         Checks user lockout status and raises an exception if user is not allowed to log in.
 
         This method interrupts the login flow and inserts  error message directly to the
         ``response_context`` attribute that is supplied as a keyword argument.
 
@@ -47,16 +55,33 @@
         # Locked out, don't try to authenticate, just update response_context and return.
         # Its a bit weird to pass a context and expect a response value but its nice to get a "why" back.
 
         error_msg = get_lockout_message()
         response_context = kwargs.get("response_context", {})
         response_context["error"] = error_msg
 
+        # This flag can be used later to check if it was Axes that denied the login attempt.
+        if not settings.AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT:
+            request.axes_locked_out = True
+
         # Raise an error that stops the authentication flows at django.contrib.auth.authenticate.
         # This error stops bubbling up at the authenticate call which catches backend PermissionDenied errors.
         # After this error is caught by authenticate it emits a signal indicating user login failed,
         # which is processed by axes.signals.log_user_login_failed which logs and flags the failed request.
         # The axes.middleware.AxesMiddleware further processes the flagged request into a readable response.
 
         raise AxesBackendPermissionDenied(
             "AxesBackend detected that the given user is locked out"
         )
+
+
+class AxesBackend(AxesStandaloneBackend, ModelBackend):
+    """
+    Axes authentication backend that also inherits from ModelBackend,
+    and thus also performs other functions of ModelBackend such as permissions checks.
+
+    Use this class as the first item of ``AUTHENTICATION_BACKENDS`` to
+    prevent locked out users from being logged in by the Django authentication flow.
+
+    .. note:: This backend does not log your user in. It monitors login attempts.
+              Authentication is handled by the following backends that are configured in ``AUTHENTICATION_BACKENDS``.
+    """
```

### Comparing `django-axes-5.9.1/axes/checks.py` & `django-axes-6.0.0b1/axes/checks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 from django.core.checks import (  # pylint: disable=redefined-builtin
     Tags,
     Warning,
     register,
 )
 from django.utils.module_loading import import_string
 
-from axes.backends import AxesBackend
+from axes.backends import AxesStandaloneBackend
 from axes.conf import settings
 
 
 class Messages:
     CACHE_INVALID = (
         "You are using the django-axes cache handler for login attempt tracking."
         " Your cache configuration is however invalid and will not work correctly with django-axes."
         " This can leave security holes in your login systems as attempts are not tracked correctly."
         " Reconfigure settings.AXES_CACHE and settings.CACHES per django-axes configuration documentation."
     )
     MIDDLEWARE_INVALID = (
         "You do not have 'axes.middleware.AxesMiddleware' in your settings.MIDDLEWARE."
     )
-    BACKEND_INVALID = "You do not have 'axes.backends.AxesBackend' or a subclass in your settings.AUTHENTICATION_BACKENDS."
+    BACKEND_INVALID = "You do not have 'axes.backends.AxesStandaloneBackend' or a subclass in your settings.AUTHENTICATION_BACKENDS."
     SETTING_DEPRECATED = "You have a deprecated setting {deprecated_setting} configured in your project settings"
 
 
 class Hints:
     CACHE_INVALID = None
     MIDDLEWARE_INVALID = None
-    BACKEND_INVALID = (
-        "AxesModelBackend was renamed to AxesBackend in django-axes version 5.0."
-    )
+    BACKEND_INVALID = "AxesModelBackend was renamed to AxesStandaloneBackend in django-axes version 5.0."
     SETTING_DEPRECATED = None
 
 
 class Codes:
     CACHE_INVALID = "axes.W001"
     MIDDLEWARE_INVALID = "axes.W002"
     BACKEND_INVALID = "axes.W003"
@@ -97,15 +95,15 @@
                 "Can not find module path defined in settings.AUTHENTICATION_BACKENDS"
             ) from e
         except ImportError as e:
             raise ImportError(
                 "Can not import backend class defined in settings.AUTHENTICATION_BACKENDS"
             ) from e
 
-        if issubclass(backend, AxesBackend):
+        if issubclass(backend, AxesStandaloneBackend):
             found = True
             break
 
     if not found:
         warnings.append(
             Warning(
                 msg=Messages.BACKEND_INVALID,
```

### Comparing `django-axes-5.9.1/axes/conf.py` & `django-axes-6.0.0b1/axes/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 
-
 # disable plugin when set to False
 settings.AXES_ENABLED = getattr(settings, "AXES_ENABLED", True)
 
 # see if the user has overridden the failure limit
 settings.AXES_FAILURE_LIMIT = getattr(settings, "AXES_FAILURE_LIMIT", 3)
 
 # see if the user has set axes to lock out logins after failure limit
@@ -48,30 +47,41 @@
 
 # determine if given user should be always allowed to attempt authentication
 settings.AXES_WHITELIST_CALLABLE = getattr(settings, "AXES_WHITELIST_CALLABLE", None)
 
 # return custom lockout response if configured
 settings.AXES_LOCKOUT_CALLABLE = getattr(settings, "AXES_LOCKOUT_CALLABLE", None)
 
+# use a provided callable to get client ip address
+settings.AXES_CLIENT_IP_CALLABLE = getattr(settings, "AXES_CLIENT_IP_CALLABLE", None)
+
 # reset the number of failed attempts after one successful attempt
 settings.AXES_RESET_ON_SUCCESS = getattr(settings, "AXES_RESET_ON_SUCCESS", False)
 
 settings.AXES_DISABLE_ACCESS_LOG = getattr(settings, "AXES_DISABLE_ACCESS_LOG", False)
 
+settings.AXES_ENABLE_ACCESS_FAILURE_LOG = getattr(
+    settings, "AXES_ENABLE_ACCESS_FAILURE_LOG", False
+)
+
+settings.AXES_ACCESS_FAILURE_LOG_PER_USER_LIMIT = getattr(
+    settings, "AXES_ACCESS_FAILURE_LOG_PER_USER_LIMIT", 1000
+)
+
 settings.AXES_HANDLER = getattr(
     settings, "AXES_HANDLER", "axes.handlers.database.AxesDatabaseHandler"
 )
 
 settings.AXES_LOCKOUT_TEMPLATE = getattr(settings, "AXES_LOCKOUT_TEMPLATE", None)
 
 settings.AXES_LOCKOUT_URL = getattr(settings, "AXES_LOCKOUT_URL", None)
 
 settings.AXES_COOLOFF_TIME = getattr(settings, "AXES_COOLOFF_TIME", None)
 
-settings.AXES_VERBOSE = getattr(settings, "AXES_VERBOSE", True)
+settings.AXES_VERBOSE = getattr(settings, "AXES_VERBOSE", settings.AXES_ENABLED)
 
 # whitelist and blacklist
 settings.AXES_NEVER_LOCKOUT_WHITELIST = getattr(
     settings, "AXES_NEVER_LOCKOUT_WHITELIST", False
 )
 
 settings.AXES_NEVER_LOCKOUT_GET = getattr(settings, "AXES_NEVER_LOCKOUT_GET", False)
@@ -82,15 +92,15 @@
 
 settings.AXES_IP_BLACKLIST = getattr(settings, "AXES_IP_BLACKLIST", None)
 
 # message to show when locked out and have cooloff enabled
 settings.AXES_COOLOFF_MESSAGE = getattr(
     settings,
     "AXES_COOLOFF_MESSAGE",
-    _("Account locked: too many login attempts. Please try again later"),
+    _("Account locked: too many login attempts. Please try again later."),
 )
 
 # message to show when locked out and have cooloff disabled
 settings.AXES_PERMALOCK_MESSAGE = getattr(
     settings,
     "AXES_PERMALOCK_MESSAGE",
     _(
@@ -112,11 +122,28 @@
 # ensure that the client can not spoof the headers by setting them and sending them through the proxy
 settings.AXES_META_PRECEDENCE_ORDER = getattr(
     settings,
     "AXES_META_PRECEDENCE_ORDER",
     getattr(settings, "IPWARE_META_PRECEDENCE_ORDER", ("REMOTE_ADDR",)),
 )
 
-# set to `True` if using with Django REST Framework
-settings.AXES_REST_FRAMEWORK_ACTIVE = getattr(
-    settings, "AXES_REST_FRAMEWORK_ACTIVE", False
+# set CORS allowed origins when calling authentication over ajax
+settings.AXES_ALLOWED_CORS_ORIGINS = getattr(settings, "AXES_ALLOWED_CORS_ORIGINS", "*")
+
+# set the list of sensitive parameters to cleanse from get/post data before logging
+settings.AXES_SENSITIVE_PARAMETERS = getattr(
+    settings,
+    "AXES_SENSITIVE_PARAMETERS",
+    [],
+)
+
+# set the callable for the readable string that can be used in
+# e.g. logging to distinguish client requests
+settings.AXES_CLIENT_STR_CALLABLE = getattr(settings, "AXES_CLIENT_STR_CALLABLE", None)
+
+# set the HTTP response code given by too many requests
+settings.AXES_HTTP_RESPONSE_CODE = getattr(settings, "AXES_HTTP_RESPONSE_CODE", 429)
+
+# If True, a failed login attempt during lockout will reset the cool off period
+settings.AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT = getattr(
+    settings, "AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT", True
 )
```

### Comparing `django-axes-5.9.1/axes/decorators.py` & `django-axes-6.0.0b1/axes/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import wraps
 
 from axes.handlers.proxy import AxesProxyHandler
 from axes.helpers import get_lockout_response
 
 
 def axes_dispatch(func):
+    @wraps(func)
     def inner(request, *args, **kwargs):
         if AxesProxyHandler.is_allowed(request):
             return func(request, *args, **kwargs)
 
         return get_lockout_response(request)
 
     return inner
```

### Comparing `django-axes-5.9.1/axes/handlers/base.py` & `django-axes-6.0.0b1/axes/handlers/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from abc import ABC, abstractmethod
 import re
+from abc import ABC, abstractmethod
+from typing import Optional
 
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 from axes.conf import settings
 from axes.helpers import (
     get_failure_limit,
@@ -37,15 +38,15 @@
     def user_logged_out(self, sender, request, user, **kwargs):
         """
         Handles the Django ``django.contrib.auth.signals.user_logged_out`` authentication signal.
         """
         raise NotImplementedError("user_logged_out should be implemented")
 
     @abstractmethod
-    def get_failures(self, request, credentials: dict = None) -> int:
+    def get_failures(self, request, credentials: Optional[dict] = None) -> int:
         """
         Checks the number of failures associated to the given request and credentials.
 
         This is a virtual method that needs an implementation in the handler subclass
         if the ``settings.AXES_LOCK_OUT_AT_FAILURE`` flag is set to ``True``.
         """
         raise NotImplementedError("get_failures should be implemented")
@@ -61,15 +62,15 @@
     Refer to `AxesHandler` for an example.
 
     The default implementation that is actually used by Axes is ``axes.handlers.database.AxesDatabaseHandler``.
 
     .. note:: This is a virtual class and **can not be used without specialization**.
     """
 
-    def is_allowed(self, request, credentials: dict = None) -> bool:
+    def is_allowed(self, request, credentials: Optional[dict] = None) -> bool:
         """
         Checks if the user is allowed to access or use given functionality such as a login view or authentication.
 
         This method is abstract and other backends can specialize it as needed, but the default implementation
         checks if the user has attempted to authenticate into the site too many times through the
         Django authentication backends and returns ``False`` if user exceeds the configured Axes thresholds.
 
@@ -90,25 +91,25 @@
             return True
 
         if self.is_locked(request, credentials):
             return False
 
         return True
 
-    def is_blacklisted(self, request, credentials: dict = None) -> bool:
+    def is_blacklisted(self, request, credentials: Optional[dict] = None) -> bool:
         """
         Checks if the request or given credentials are blacklisted from access.
         """
 
         if is_client_ip_address_blacklisted(request):
             return True
 
         return False
 
-    def is_whitelisted(self, request, credentials: dict = None) -> bool:
+    def is_whitelisted(self, request, credentials: Optional[dict] = None) -> bool:
         """
         Checks if the request or given credentials are whitelisted for access.
         """
 
         if is_user_attempt_whitelisted(request, credentials):
             return True
 
@@ -116,15 +117,15 @@
             return True
 
         if is_client_method_whitelisted(request):
             return True
 
         return False
 
-    def is_locked(self, request, credentials: dict = None) -> bool:
+    def is_locked(self, request, credentials: Optional[dict] = None) -> bool:
         """
         Checks if the request or given credentials are locked.
         """
 
         if settings.AXES_LOCK_OUT_AT_FAILURE:
             # get_failures will have to be implemented by each specialized handler
             return self.get_failures(  # type: ignore
@@ -138,46 +139,71 @@
         Checks if the request is for admin site.
         """
         if settings.AXES_ONLY_ADMIN_SITE and hasattr(request, "path"):
             try:
                 admin_url = reverse("admin:index")
             except NoReverseMatch:
                 return True
-            return not re.match("^%s" % admin_url, request.path)
+            return not re.match(f"^{admin_url}", request.path)
 
         return False
 
     def reset_attempts(
         self,
         *,
-        ip_address: str = None,
-        username: str = None,
+        ip_address: Optional[str] = None,
+        username: Optional[str] = None,
         ip_or_username: bool = False,
     ) -> int:
         """
         Resets access attempts that match the given IP address or username.
 
         This method makes more sense for the DB backend, but as it is used by the ProxyHandler
-        (via inherent), it needs to be defined here so we get compliant with all proxy methods.
+        (via inherent), it needs to be defined here, so we get compliant with all proxy methods.
 
         Please overwrite it on each specialized handler as needed.
         """
         return 0
 
-    def reset_logs(self, *, age_days: int = None) -> int:
+    def reset_logs(self, *, age_days: Optional[int] = None) -> int:
         """
         Resets access logs that are older than given number of days.
 
         This method makes more sense for the DB backend, but as it is used by the ProxyHandler
-        (via inherent), it needs to be defined here so we get compliant with all proxy methods.
+        (via inherent), it needs to be defined here, so we get compliant with all proxy methods.
+
+        Please overwrite it on each specialized handler as needed.
+        """
+        return 0
+
+    def reset_failure_logs(self, *, age_days: Optional[int] = None) -> int:
+        """
+        Resets access failure logs that are older than given number of days.
+
+        This method makes more sense for the DB backend, but as it is used by the ProxyHandler
+        (via inherent), it needs to be defined here, so we get compliant with all proxy methods.
 
         Please overwrite it on each specialized handler as needed.
         """
         return 0
 
+    def remove_out_of_limit_failure_logs(
+        self, *, username: str, limit: Optional[int] = None
+    ) -> int:
+        """Remove access failure logs that are over
+        AXES_ACCESS_FAILURE_LOG_PER_USER_LIMIT for user username.
+
+        This method makes more sense for the DB backend, but as it is used by the ProxyHandler
+        (via inherent), it needs to be defined here, so we get compliant with all proxy methods.
+
+        Please overwrite it on each specialized handler as needed.
+
+        """
+        return 0
+
 
 class AxesHandler(AbstractAxesHandler, AxesBaseHandler):
     """
     Signal bare handler implementation without any storage backend.
     """
 
     def user_login_failed(self, sender, credentials: dict, request=None, **kwargs):
@@ -185,9 +211,9 @@
 
     def user_logged_in(self, sender, request, user, **kwargs):
         pass
 
     def user_logged_out(self, sender, request, user, **kwargs):
         pass
 
-    def get_failures(self, request, credentials: dict = None) -> int:
+    def get_failures(self, request, credentials: Optional[dict] = None) -> int:
         return 0
```

### Comparing `django-axes-5.9.1/axes/handlers/cache.py` & `django-axes-6.0.0b1/axes/handlers/cache.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,121 @@
 from logging import getLogger
+from typing import Optional
 
 from axes.conf import settings
 from axes.handlers.base import AxesBaseHandler, AbstractAxesHandler
-from axes.signals import user_locked_out
 from axes.helpers import (
     get_cache,
     get_cache_timeout,
     get_client_cache_key,
     get_client_str,
     get_client_username,
     get_credentials,
     get_failure_limit,
 )
+from axes.models import AccessAttempt
+from axes.signals import user_locked_out
 
 log = getLogger(__name__)
 
 
 class AxesCacheHandler(AbstractAxesHandler, AxesBaseHandler):
     """
     Signal handler implementation that records user login attempts to cache and locks users out if necessary.
     """
 
     def __init__(self):
         self.cache = get_cache()
-        self.cache_timeout = get_cache_timeout()
 
-    def get_failures(self, request, credentials: dict = None) -> int:
+    def reset_attempts(
+        self,
+        *,
+        ip_address: Optional[str] = None,
+        username: Optional[str] = None,
+        ip_or_username: bool = False,
+    ) -> int:
+        cache_keys: list = []
+        count = 0
+
+        if ip_address is None and username is None:
+            raise NotImplementedError("Cannot clear all entries from cache")
+        if ip_or_username:
+            raise NotImplementedError(
+                "Due to the cache key ip_or_username=True is not supported"
+            )
+
+        cache_keys.extend(
+            get_client_cache_key(
+                AccessAttempt(username=username, ip_address=ip_address)
+            )
+        )
+
+        for cache_key in cache_keys:
+            deleted = self.cache.delete(cache_key)
+            count += int(deleted) if deleted is not None else 1
+
+        log.info("AXES: Reset %d access attempts from database.", count)
+
+        return count
+
+    def get_failures(self, request, credentials: Optional[dict] = None) -> int:
         cache_keys = get_client_cache_key(request, credentials)
         failure_count = max(
             self.cache.get(cache_key, default=0) for cache_key in cache_keys
         )
         return failure_count
 
-    def user_login_failed(
-        self, sender, credentials: dict, request=None, **kwargs
-    ):  # pylint: disable=too-many-locals
+    def user_login_failed(self, sender, credentials: dict, request=None, **kwargs):
         """
         When user login fails, save attempt record in cache and lock user out if necessary.
 
         :raises AxesSignalPermissionDenied: if user should be locked out.
         """
 
         if request is None:
             log.error(
                 "AXES: AxesCacheHandler.user_login_failed does not function without a request."
             )
             return
 
         username = get_client_username(request, credentials)
+        if settings.AXES_ONLY_USER_FAILURES and username is None:
+            log.warning(
+                "AXES: Username is None and AXES_ONLY_USER_FAILURES is enabled, new record will NOT be created."
+            )
+            return
+
+        # If axes denied access, don't record the failed attempt as that would reset the lockout time.
+        if (
+            not settings.AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT
+            and request.axes_locked_out
+        ):
+            request.axes_credentials = credentials
+            user_locked_out.send(
+                "axes",
+                request=request,
+                username=username,
+                ip_address=request.axes_ip_address,
+            )
+            return
+
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
         if self.is_whitelisted(request, credentials):
             log.info("AXES: Login failed from whitelisted client %s.", client_str)
             return
 
         failures_since_start = 1 + self.get_failures(request, credentials)
+        request.axes_failures_since_start = failures_since_start
 
         if failures_since_start > 1:
             log.warning(
                 "AXES: Repeated login failure by %s. Count = %d of %d. Updating existing record in the cache.",
                 client_str,
                 failures_since_start,
                 get_failure_limit(request, credentials),
@@ -73,46 +125,46 @@
                 "AXES: New login failure by %s. Creating new record in the cache.",
                 client_str,
             )
 
         cache_keys = get_client_cache_key(request, credentials)
         for cache_key in cache_keys:
             failures = self.cache.get(cache_key, default=0)
-            self.cache.set(cache_key, failures + 1, self.cache_timeout)
+            self.cache.set(cache_key, failures + 1, get_cache_timeout())
 
         if (
             settings.AXES_LOCK_OUT_AT_FAILURE
             and failures_since_start >= get_failure_limit(request, credentials)
         ):
             log.warning(
                 "AXES: Locking out %s after repeated login failures.", client_str
             )
 
             request.axes_locked_out = True
+            request.axes_credentials = credentials
             user_locked_out.send(
                 "axes",
                 request=request,
                 username=username,
                 ip_address=request.axes_ip_address,
             )
 
-    def user_logged_in(
-        self, sender, request, user, **kwargs
-    ):  # pylint: disable=unused-argument
+    def user_logged_in(self, sender, request, user, **kwargs):
         """
         When user logs in, update the AccessLog related to the user.
         """
 
         username = user.get_username()
         credentials = get_credentials(username)
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
         log.info("AXES: Successful login by %s.", client_str)
 
         if settings.AXES_RESET_ON_SUCCESS:
             cache_keys = get_client_cache_key(request, credentials)
             for cache_key in cache_keys:
@@ -127,10 +179,11 @@
     def user_logged_out(self, sender, request, user, **kwargs):
         username = user.get_username() if user else None
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
         log.info("AXES: Successful logout by %s.", client_str)
```

### Comparing `django-axes-5.9.1/axes/handlers/database.py` & `django-axes-6.0.0b1/axes/handlers/database.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from logging import getLogger
+from typing import Optional
 
-from django.db.models import Sum, Value, Q
+from django.db import transaction
+from django.db.models import F, Sum, Value, Q
 from django.db.models.functions import Concat
 from django.utils import timezone
 
 from axes.attempts import (
     clean_expired_user_attempts,
     get_user_attempts,
     reset_user_attempts,
 )
 from axes.conf import settings
 from axes.handlers.base import AxesBaseHandler, AbstractAxesHandler
-from axes.models import AccessLog, AccessAttempt
-from axes.signals import user_locked_out
 from axes.helpers import (
     get_client_str,
     get_client_username,
     get_credentials,
     get_failure_limit,
     get_query_str,
 )
-
+from axes.models import AccessLog, AccessAttempt, AccessFailureLog
+from axes.signals import user_locked_out
 
 log = getLogger(__name__)
 
 
 class AxesDatabaseHandler(AbstractAxesHandler, AxesBaseHandler):
     """
     Signal handler implementation that records user login attempts to database and locks users out if necessary.
@@ -32,16 +33,16 @@
     .. note:: The get_user_attempts function is called several time during the authentication and lockout
               process, caching its output can be dangerous.
     """
 
     def reset_attempts(
         self,
         *,
-        ip_address: str = None,
-        username: str = None,
+        ip_address: Optional[str] = None,
+        username: Optional[str] = None,
         ip_or_username: bool = False,
     ) -> int:
         attempts = AccessAttempt.objects.all()
 
         if ip_or_username:
             attempts = attempts.filter(Q(ip_address=ip_address) | Q(username=username))
         else:
@@ -51,51 +52,81 @@
                 attempts = attempts.filter(username=username)
 
         count, _ = attempts.delete()
         log.info("AXES: Reset %d access attempts from database.", count)
 
         return count
 
-    def reset_logs(self, *, age_days: int = None) -> int:
+    def reset_logs(self, *, age_days: Optional[int] = None) -> int:
         if age_days is None:
             count, _ = AccessLog.objects.all().delete()
             log.info("AXES: Reset all %d access logs from database.", count)
         else:
             limit = timezone.now() - timezone.timedelta(days=age_days)
             count, _ = AccessLog.objects.filter(attempt_time__lte=limit).delete()
             log.info(
                 "AXES: Reset %d access logs older than %d days from database.",
                 count,
                 age_days,
             )
 
         return count
 
-    def get_failures(self, request, credentials: dict = None) -> int:
+    def reset_failure_logs(self, *, age_days: Optional[int] = None) -> int:
+        if age_days is None:
+            count, _ = AccessFailureLog.objects.all().delete()
+            log.info("AXES: Reset all %d access failure logs from database.", count)
+        else:
+            limit = timezone.now() - timezone.timedelta(days=age_days)
+            count, _ = AccessFailureLog.objects.filter(attempt_time__lte=limit).delete()
+            log.info(
+                "AXES: Reset %d access failure logs older than %d days from database.",
+                count,
+                age_days,
+            )
+
+        return count
+
+    def remove_out_of_limit_failure_logs(
+        self,
+        *,
+        username: str,
+        limit: Optional[int] = settings.AXES_ACCESS_FAILURE_LOG_PER_USER_LIMIT,
+    ) -> int:
+        count = 0
+        failures = AccessFailureLog.objects.filter(username=username)
+        out_of_limit_failures_logs = failures.count() - limit
+        if out_of_limit_failures_logs > 0:
+            for failure in failures[:out_of_limit_failures_logs]:
+                failure.delete()
+                count += 1
+        return count
+
+    def get_failures(self, request, credentials: Optional[dict] = None) -> int:
         attempts_list = get_user_attempts(request, credentials)
         attempt_count = max(
             (
                 attempts.aggregate(Sum("failures_since_start"))[
                     "failures_since_start__sum"
                 ]
                 or 0
             )
             for attempts in attempts_list
         )
         return attempt_count
 
-    def user_login_failed(
-        self, sender, credentials: dict, request=None, **kwargs
-    ):  # pylint: disable=too-many-locals
-        """
-        When user login fails, save AccessAttempt record in database and lock user out if necessary.
+    def user_login_failed(self, sender, credentials: dict, request=None, **kwargs):
+        """When user login fails, save AccessFailureLog record in database,
+        save AccessAttempt record in database, mark request with
+        lockout attribute and emit lockout signal.
 
-        :raises AxesSignalPermissionDenied: if user should be locked out.
         """
 
+        log.info("AXES: User login failed, running database handler for failure.")
+
         if request is None:
             log.error(
                 "AXES: AxesDatabaseHandler.user_login_failed does not function without a request."
             )
             return
 
         # 1. database query: Clean up expired user attempts from the database before logging new attempts
@@ -103,113 +134,145 @@
 
         username = get_client_username(request, credentials)
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
-        # This replaces null byte chars that crash saving failures, meaning an attacker doesn't get locked out.
+        # If axes denied access, don't record the failed attempt as that would reset the lockout time.
+        if (
+            not settings.AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT
+            and request.axes_locked_out
+        ):
+            request.axes_credentials = credentials
+            user_locked_out.send(
+                "axes",
+                request=request,
+                username=username,
+                ip_address=request.axes_ip_address,
+            )
+            return
+
+        # This replaces null byte chars that crash saving failures.
         get_data = get_query_str(request.GET).replace("\0", "0x00")
         post_data = get_query_str(request.POST).replace("\0", "0x00")
 
         if self.is_whitelisted(request, credentials):
             log.info("AXES: Login failed from whitelisted client %s.", client_str)
             return
 
-        # 2. database query: Calculate the current maximum failure number from the existing attempts
-        failures_since_start = 1 + self.get_failures(request, credentials)
-
-        # 3. database query: Insert or update access records with the new failure data
-        try:
-            attempt = AccessAttempt.objects.get(
-                username=username,
-                ip_address=request.axes_ip_address,
-                user_agent=request.axes_user_agent,
-            )
-            # Update failed attempt information but do not touch the username, IP address, or user agent fields,
-            # because attackers can request the site with multiple different configurations
-            # in order to bypass the defense mechanisms that are used by the site.
-
+        # 2. database query: Get or create access record with the new failure data
+        if settings.AXES_ONLY_USER_FAILURES and username is None:
             log.warning(
-                "AXES: Repeated login failure by %s. Count = %d of %d. Updating existing record in the database.",
-                client_str,
-                attempt.failures_since_start,
-                get_failure_limit(request, credentials),
+                "AXES: Username is None and AXES_ONLY_USER_FAILURES is enabled, new record will NOT be created."
             )
-
-            separator = "\n---------\n"
-
-            attempt.get_data = Concat("get_data", Value(separator + get_data))
-            attempt.post_data = Concat("post_data", Value(separator + post_data))
-            attempt.http_accept = request.axes_http_accept
-            attempt.path_info = request.axes_path_info
-            attempt.failures_since_start += 1
-            attempt.attempt_time = request.axes_attempt_time
-            attempt.save()
-        except AccessAttempt.DoesNotExist:
-            # Record failed attempt with all the relevant information.
-            # Filtering based on username, IP address and user agent handled elsewhere,
-            # and this handler just records the available information for further use.
-
-            if not (settings.AXES_ONLY_USER_FAILURES and username is None):
-                log.warning(
-                    "AXES: New login failure by %s. Creating new record in the database.",
-                    client_str,
-                )
-                AccessAttempt.objects.create(
+        else:
+            with transaction.atomic():
+                (
+                    attempt,
+                    created,
+                ) = AccessAttempt.objects.select_for_update().get_or_create(
                     username=username,
                     ip_address=request.axes_ip_address,
                     user_agent=request.axes_user_agent,
-                    get_data=get_data,
-                    post_data=post_data,
-                    http_accept=request.axes_http_accept,
-                    path_info=request.axes_path_info,
-                    failures_since_start=1,
-                    attempt_time=request.axes_attempt_time,
-                )
-            else:
-                log.warning(
-                    "AXES: Username is None and AXES_ONLY_USER_FAILURES is enable, New record won't be created."
+                    defaults={
+                        "get_data": get_data,
+                        "post_data": post_data,
+                        "http_accept": request.axes_http_accept,
+                        "path_info": request.axes_path_info,
+                        "failures_since_start": 1,
+                        "attempt_time": request.axes_attempt_time,
+                    },
                 )
+
+                # Record failed attempt with all the relevant information.
+                # Filtering based on username, IP address and user agent handled elsewhere,
+                # and this handler just records the available information for further use.
+                if created:
+                    log.warning(
+                        "AXES: New login failure by %s. Created new record in the database.",
+                        client_str,
+                    )
+
+                # 3. database query if there were previous attempts in the database
+                # Update failed attempt information but do not touch the username, IP address, or user agent fields,
+                # because attackers can request the site with multiple different configurations
+                # in order to bypass the defense mechanisms that are used by the site.
+                else:
+                    separator = "\n---------\n"
+
+                    attempt.get_data = Concat("get_data", Value(separator + get_data))
+                    attempt.post_data = Concat(
+                        "post_data", Value(separator + post_data)
+                    )
+                    attempt.http_accept = request.axes_http_accept
+                    attempt.path_info = request.axes_path_info
+                    attempt.failures_since_start = F("failures_since_start") + 1
+                    attempt.attempt_time = request.axes_attempt_time
+                    attempt.save()
+
+                    log.warning(
+                        "AXES: Repeated login failure by %s. Updated existing record in the database.",
+                        client_str,
+                    )
+
+        # 3. or 4. database query: Calculate the current maximum failure number from the existing attempts
+        failures_since_start = self.get_failures(request, credentials)
+        request.axes_failures_since_start = failures_since_start
+
         if (
             settings.AXES_LOCK_OUT_AT_FAILURE
             and failures_since_start >= get_failure_limit(request, credentials)
         ):
             log.warning(
                 "AXES: Locking out %s after repeated login failures.", client_str
             )
 
             request.axes_locked_out = True
-
+            request.axes_credentials = credentials
             user_locked_out.send(
                 "axes",
                 request=request,
                 username=username,
                 ip_address=request.axes_ip_address,
             )
 
-    def user_logged_in(
-        self, sender, request, user, **kwargs
-    ):  # pylint: disable=unused-argument
+        # 5. database entry: Log for ever the attempt in the AccessFailureLog
+        if settings.AXES_ENABLE_ACCESS_FAILURE_LOG:
+            with transaction.atomic():
+                AccessFailureLog.objects.create(
+                    username=username,
+                    ip_address=request.axes_ip_address,
+                    user_agent=request.axes_user_agent,
+                    http_accept=request.axes_http_accept,
+                    path_info=request.axes_path_info,
+                    attempt_time=request.axes_attempt_time,
+                    locked_out=request.axes_locked_out,
+                )
+                self.remove_out_of_limit_failure_logs(username=username)
+
+    def user_logged_in(self, sender, request, user, **kwargs):
         """
         When user logs in, update the AccessLog related to the user.
         """
 
         # 1. database query: Clean up expired user attempts from the database
         clean_expired_user_attempts(request.axes_attempt_time)
 
         username = user.get_username()
         credentials = get_credentials(username)
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
         log.info("AXES: Successful login by %s.", client_str)
 
         if not settings.AXES_DISABLE_ACCESS_LOG:
             # 2. database query: Insert new access logs with login time
             AccessLog.objects.create(
@@ -226,30 +289,29 @@
             count = reset_user_attempts(request, credentials)
             log.info(
                 "AXES: Deleted %d failed login attempts by %s from database.",
                 count,
                 client_str,
             )
 
-    def user_logged_out(
-        self, sender, request, user, **kwargs
-    ):  # pylint: disable=unused-argument
+    def user_logged_out(self, sender, request, user, **kwargs):
         """
         When user logs out, update the AccessLog related to the user.
         """
 
         # 1. database query: Clean up expired user attempts from the database
         clean_expired_user_attempts(request.axes_attempt_time)
 
         username = user.get_username() if user else None
         client_str = get_client_str(
             username,
             request.axes_ip_address,
             request.axes_user_agent,
             request.axes_path_info,
+            request,
         )
 
         log.info("AXES: Successful logout by %s.", client_str)
 
         if username and not settings.AXES_DISABLE_ACCESS_LOG:
             # 2. database query: Update existing attempt logs with logout time
             AccessLog.objects.filter(
```

### Comparing `django-axes-5.9.1/axes/handlers/test.py` & `django-axes-6.0.0b1/axes/handlers/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from axes.handlers.base import AxesHandler
+from typing import Optional
 
 
-class AxesTestHandler(AxesHandler):  # pylint: disable=unused-argument
+class AxesTestHandler(AxesHandler):
     """
     Signal handler implementation that does nothing, ideal for a test suite.
     """
 
     def reset_attempts(
         self,
         *,
-        ip_address: str = None,
-        username: str = None,
+        ip_address: Optional[str] = None,
+        username: Optional[str] = None,
         ip_or_username: bool = False,
     ) -> int:
         return 0
 
-    def reset_logs(self, *, age_days: int = None) -> int:
+    def reset_logs(self, *, age_days: Optional[int] = None) -> int:
         return 0
 
-    def is_allowed(self, request, credentials: dict = None) -> bool:
+    def is_allowed(self, request, credentials: Optional[dict] = None) -> bool:
         return True
 
-    def get_failures(self, request, credentials: dict = None) -> int:
+    def get_failures(self, request, credentials: Optional[dict] = None) -> int:
         return 0
```

### Comparing `django-axes-5.9.1/axes/helpers.py` & `django-axes-6.0.0b1/axes/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from datetime import timedelta
-from hashlib import md5
+from hashlib import sha256
 from logging import getLogger
 from string import Template
 from typing import Callable, Optional, Type, Union
 from urllib.parse import urlencode
 
-from django.core.cache import caches, BaseCache
+import ipware.ip
+from django.core.cache import BaseCache, caches
 from django.http import HttpRequest, HttpResponse, JsonResponse, QueryDict
-from django.shortcuts import render, redirect
+from django.shortcuts import redirect, render
 from django.utils.module_loading import import_string
 
-import ipware.ip
-
 from axes.conf import settings
 from axes.models import AccessBase
 
 log = getLogger(__name__)
 
 
 def get_cache() -> BaseCache:
@@ -56,18 +55,20 @@
     :exception TypeError: if settings.AXES_COOLOFF_TIME is of wrong type.
     """
 
     cool_off = settings.AXES_COOLOFF_TIME
 
     if isinstance(cool_off, int):
         return timedelta(hours=cool_off)
+    if isinstance(cool_off, float):
+        return timedelta(minutes=cool_off * 60)
     if isinstance(cool_off, str):
         return import_string(cool_off)()
     if callable(cool_off):
-        return cool_off()
+        return cool_off()  # pylint: disable=not-callable
 
     return cool_off
 
 
 def get_cool_off_iso8601(delta: timedelta) -> str:
     """
     Return datetime.timedelta translated to ISO 8601 formatted duration for use in e.g. cool offs.
@@ -87,28 +88,30 @@
     )
 
     if time_str:
         return f"P{days_str}T{time_str}"
     return f"P{days_str}"
 
 
-def get_credentials(username: str = None, **kwargs) -> dict:
+def get_credentials(username: Optional[str] = None, **kwargs) -> dict:
     """
     Calculate credentials for Axes to use internally from given username and kwargs.
 
     Axes will set the username value into the key defined with ``settings.AXES_USERNAME_FORM_FIELD``
     and update the credentials dictionary with the kwargs given on top of that.
     """
 
     credentials = {settings.AXES_USERNAME_FORM_FIELD: username}
     credentials.update(kwargs)
     return credentials
 
 
-def get_client_username(request, credentials: dict = None) -> str:
+def get_client_username(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> str:
     """
     Resolve client username from the given request or credentials if supplied.
 
     The order of preference for fetching the username is as follows:
 
     1. If configured, use ``AXES_USERNAME_CALLABLE``, and supply ``request, credentials`` as arguments
     2. If given, use ``credentials`` and fetch username from ``AXES_USERNAME_FORM_FIELD`` (defaults to ``username``)
@@ -118,15 +121,17 @@
     :param credentials: incoming credentials ``dict`` or similar object from authentication backend or other source
     """
 
     if settings.AXES_USERNAME_CALLABLE:
         log.debug("Using settings.AXES_USERNAME_CALLABLE to get username")
 
         if callable(settings.AXES_USERNAME_CALLABLE):
-            return settings.AXES_USERNAME_CALLABLE(request, credentials)
+            return settings.AXES_USERNAME_CALLABLE(  # pylint: disable=not-callable
+                request, credentials
+            )
         if isinstance(settings.AXES_USERNAME_CALLABLE, str):
             return import_string(settings.AXES_USERNAME_CALLABLE)(request, credentials)
         raise TypeError(
             "settings.AXES_USERNAME_CALLABLE needs to be a string, callable, or None."
         )
 
     if credentials:
@@ -139,42 +144,59 @@
         "Using parameter request.POST to get username with key settings.AXES_USERNAME_FORM_FIELD"
     )
 
     request_data = getattr(request, "data", request.POST)
     return request_data.get(settings.AXES_USERNAME_FORM_FIELD, None)
 
 
-def get_client_ip_address(request) -> str:
+def get_client_ip_address(request: HttpRequest) -> str:
     """
     Get client IP address as configured by the user.
 
-    The django-ipware package is used for address resolution
-    and parameters can be configured in the Axes package.
+    The order of preference for address resolution is as follows:
+
+    1. If configured, use ``AXES_CLIENT_IP_CALLABLE``, and supply ``request`` as argument
+    2. Use django-ipware package (parameters can be configured in the Axes package)
+
+    :param request: incoming Django ``HttpRequest`` or similar object from authentication backend or other source
     """
 
+    if settings.AXES_CLIENT_IP_CALLABLE:
+        log.debug("Using settings.AXES_CLIENT_IP_CALLABLE to get username")
+
+        if callable(settings.AXES_CLIENT_IP_CALLABLE):
+            return settings.AXES_CLIENT_IP_CALLABLE(  # pylint: disable=not-callable
+                request
+            )
+        if isinstance(settings.AXES_CLIENT_IP_CALLABLE, str):
+            return import_string(settings.AXES_CLIENT_IP_CALLABLE)(request)
+        raise TypeError(
+            "settings.AXES_CLIENT_IP_CALLABLE needs to be a string, callable, or None."
+        )
+
     client_ip_address, _ = ipware.ip.get_client_ip(
         request,
         proxy_order=settings.AXES_PROXY_ORDER,
         proxy_count=settings.AXES_PROXY_COUNT,
         proxy_trusted_ips=settings.AXES_PROXY_TRUSTED_IPS,
         request_header_order=settings.AXES_META_PRECEDENCE_ORDER,
     )
 
     return client_ip_address
 
 
-def get_client_user_agent(request) -> str:
+def get_client_user_agent(request: HttpRequest) -> str:
     return request.META.get("HTTP_USER_AGENT", "<unknown>")[:255]
 
 
-def get_client_path_info(request) -> str:
+def get_client_path_info(request: HttpRequest) -> str:
     return request.META.get("PATH_INFO", "<unknown>")[:255]
 
 
-def get_client_http_accept(request) -> str:
+def get_client_http_accept(request: HttpRequest) -> str:
     return request.META.get("HTTP_ACCEPT", "<unknown>")[:1025]
 
 
 def get_client_parameters(username: str, ip_address: str, user_agent: str) -> list:
     """
     Get query parameters for filtering AccessAttempt queryset.
 
@@ -196,32 +218,33 @@
             filter_query = [{"username": username, "ip_address": ip_address}]
         else:
             # 3. Default case is to track the IP address only, which is the most secure option
             filter_query = [{"ip_address": ip_address}]
 
         if settings.AXES_USE_USER_AGENT:
             # 4. The HTTP User-Agent can be used to track e.g. one browser
-            filter_query.append({"user_agent": user_agent})
+            filter_query[0]["user_agent"] = user_agent
 
     return filter_query
 
 
 def make_cache_key_list(filter_kwargs_list):
     cache_keys = []
     for filter_kwargs in filter_kwargs_list:
         cache_key_components = "".join(
             value for value in filter_kwargs.values() if value
         )
-        cache_key_digest = md5(cache_key_components.encode()).hexdigest()
+        cache_key_digest = sha256(cache_key_components.encode()).hexdigest()
         cache_keys.append(f"axes-{cache_key_digest}")
     return cache_keys
 
 
 def get_client_cache_key(
-    request_or_attempt: Union[HttpRequest, AccessBase], credentials: dict = None
+    request_or_attempt: Union[HttpRequest, AccessBase],
+    credentials: Optional[dict] = None,
 ) -> str:
     """
     Build cache key name from request or AccessAttempt object.
 
     :param request_or_attempt: HttpRequest or AccessAttempt object
     :param credentials: credentials containing user information
     :return cache_key: Hash key that is usable for Django cache backends
@@ -238,97 +261,146 @@
 
     filter_kwargs_list = get_client_parameters(username, ip_address, user_agent)
 
     return make_cache_key_list(filter_kwargs_list)
 
 
 def get_client_str(
-    username: str, ip_address: str, user_agent: str, path_info: str
+    username: str,
+    ip_address: str,
+    user_agent: str,
+    path_info: str,
+    request: HttpRequest,
 ) -> str:
     """
     Get a readable string that can be used in e.g. logging to distinguish client requests.
 
     Example log format would be
     ``{username: "example", ip_address: "127.0.0.1", path_info: "/example/"}``
     """
 
-    client_dict = dict()
+    if settings.AXES_CLIENT_STR_CALLABLE:
+        log.debug("Using settings.AXES_CLIENT_STR_CALLABLE to get client string.")
+
+        if callable(settings.AXES_CLIENT_STR_CALLABLE):
+            return settings.AXES_CLIENT_STR_CALLABLE(  # pylint: disable=not-callable
+                username, ip_address, user_agent, path_info, request
+            )
+        if isinstance(settings.AXES_CLIENT_STR_CALLABLE, str):
+            return import_string(settings.AXES_CLIENT_STR_CALLABLE)(
+                username, ip_address, user_agent, path_info, request
+            )
+        raise TypeError(
+            "settings.AXES_CLIENT_STR_CALLABLE needs to be a string, callable or None."
+        )
+
+    client_dict = {}
 
     if settings.AXES_VERBOSE:
         # Verbose mode logs every attribute that is available
         client_dict["username"] = username
         client_dict["ip_address"] = ip_address
         client_dict["user_agent"] = user_agent
     else:
         # Other modes initialize the attributes that are used for the actual lockouts
         client_list = get_client_parameters(username, ip_address, user_agent)
         client_dict = {}
         for client in client_list:
             client_dict.update(client)
-
+    client_dict = cleanse_parameters(client_dict.copy())
     # Path info is always included as last component in the client string for traceability purposes
     if path_info and isinstance(path_info, (tuple, list)):
         path_info = path_info[0]
     client_dict["path_info"] = path_info
 
     # Template the internal dictionary representation into a readable and concatenated {key: "value"} format
     template = Template('$key: "$value"')
     items = [{"key": k, "value": v} for k, v in client_dict.items()]
     client_str = ", ".join(template.substitute(item) for item in items)
     client_str = "{" + client_str + "}"
     return client_str
 
 
+def cleanse_parameters(params: dict) -> dict:
+    """
+    Replace sensitive parameter values in a parameter dict with
+    a safe placeholder value.
+
+    Parameters name ``'password'`` will always be cleansed.  Additionally,
+    parameters named in ``settings.AXES_SENSITIVE_PARAMETERS`` and
+    ``settings.AXES_PASSWORD_FORM_FIELD will be cleansed.
+
+    This is used to prevent passwords and similar values from
+    being logged in cleartext.
+    """
+    sensitive_parameters = ["password"] + settings.AXES_SENSITIVE_PARAMETERS
+    if settings.AXES_PASSWORD_FORM_FIELD:
+        sensitive_parameters.append(settings.AXES_PASSWORD_FORM_FIELD)
+
+    if sensitive_parameters:
+        cleansed = params.copy()
+        for param in sensitive_parameters:
+            if param in cleansed:
+                cleansed[param] = "********************"
+        return cleansed
+    return params
+
+
 def get_query_str(query: Type[QueryDict], max_length: int = 1024) -> str:
     """
     Turns a query dictionary into an easy-to-read list of key-value pairs.
 
-    If a field is called either ``'password'`` or ``settings.AXES_PASSWORD_FORM_FIELD`` it will be excluded.
+    If a field is called either ``'password'`` or ``settings.AXES_PASSWORD_FORM_FIELD`` or if the fieldname is included
+    in ``settings.AXES_SENSITIVE_PARAMETERS`` its value will be masked.
 
     The length of the output is limited to max_length to avoid a DoS attack via excessively large payloads.
     """
 
-    query_dict = query.copy()
-    query_dict.pop("password", None)
-    query_dict.pop(settings.AXES_PASSWORD_FORM_FIELD, None)
+    query_dict = cleanse_parameters(query.copy())
 
     template = Template("$key=$value")
     items = [{"key": k, "value": v} for k, v in query_dict.items()]
     query_str = "\n".join(template.substitute(item) for item in items)
 
     return query_str[:max_length]
 
 
-def get_failure_limit(request, credentials) -> int:
+def get_failure_limit(request: HttpRequest, credentials) -> int:
     if callable(settings.AXES_FAILURE_LIMIT):
-        return settings.AXES_FAILURE_LIMIT(request, credentials)
+        return settings.AXES_FAILURE_LIMIT(  # pylint: disable=not-callable
+            request, credentials
+        )
     if isinstance(settings.AXES_FAILURE_LIMIT, str):
         return import_string(settings.AXES_FAILURE_LIMIT)(request, credentials)
     if isinstance(settings.AXES_FAILURE_LIMIT, int):
         return settings.AXES_FAILURE_LIMIT
     raise TypeError("settings.AXES_FAILURE_LIMIT needs to be a callable or an integer")
 
 
 def get_lockout_message() -> str:
     if settings.AXES_COOLOFF_TIME:
         return settings.AXES_COOLOFF_MESSAGE
     return settings.AXES_PERMALOCK_MESSAGE
 
 
-def get_lockout_response(request, credentials: dict = None) -> HttpResponse:
+def get_lockout_response(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> HttpResponse:
     if settings.AXES_LOCKOUT_CALLABLE:
         if callable(settings.AXES_LOCKOUT_CALLABLE):
-            return settings.AXES_LOCKOUT_CALLABLE(request, credentials)
+            return settings.AXES_LOCKOUT_CALLABLE(  # pylint: disable=not-callable
+                request, credentials
+            )
         if isinstance(settings.AXES_LOCKOUT_CALLABLE, str):
             return import_string(settings.AXES_LOCKOUT_CALLABLE)(request, credentials)
         raise TypeError(
             "settings.AXES_LOCKOUT_CALLABLE needs to be a string, callable, or None."
         )
 
-    status = 403
+    status = settings.AXES_HTTP_RESPONSE_CODE
     context = {
         "failure_limit": get_failure_limit(request, credentials),
         "username": get_client_username(request, credentials) or "",
     }
 
     cool_off = get_cool_off()
     if cool_off:
@@ -338,43 +410,55 @@
                     cool_off
                 ),  # differing old name is kept for backwards compatibility
                 "cooloff_timedelta": cool_off,
             }
         )
 
     if request.META.get("HTTP_X_REQUESTED_WITH") == "XMLHttpRequest":
-        return JsonResponse(context, status=status)
+        json_response = JsonResponse(context, status=status)
+        json_response[
+            "Access-Control-Allow-Origin"
+        ] = settings.AXES_ALLOWED_CORS_ORIGINS
+        json_response["Access-Control-Allow-Methods"] = "POST, OPTIONS"
+        json_response[
+            "Access-Control-Allow-Headers"
+        ] = "Origin, Content-Type, Accept, Authorization, x-requested-with"
+        return json_response
 
     if settings.AXES_LOCKOUT_TEMPLATE:
         return render(request, settings.AXES_LOCKOUT_TEMPLATE, context, status=status)
 
     if settings.AXES_LOCKOUT_URL:
         lockout_url = settings.AXES_LOCKOUT_URL
         query_string = urlencode({"username": context["username"]})
-        url = "{}?{}".format(lockout_url, query_string)
+        url = f"{lockout_url}?{query_string}"
         return redirect(url)
 
     return HttpResponse(get_lockout_message(), status=status)
 
 
 def is_ip_address_in_whitelist(ip_address: str) -> bool:
     if not settings.AXES_IP_WHITELIST:
         return False
 
-    return ip_address in settings.AXES_IP_WHITELIST
+    return (  # pylint: disable=unsupported-membership-test
+        ip_address in settings.AXES_IP_WHITELIST
+    )
 
 
 def is_ip_address_in_blacklist(ip_address: str) -> bool:
     if not settings.AXES_IP_BLACKLIST:
         return False
 
-    return ip_address in settings.AXES_IP_BLACKLIST
+    return (  # pylint: disable=unsupported-membership-test
+        ip_address in settings.AXES_IP_BLACKLIST
+    )
 
 
-def is_client_ip_address_whitelisted(request):
+def is_client_ip_address_whitelisted(request: HttpRequest):
     """
     Check if the given request refers to a whitelisted IP.
     """
 
     if settings.AXES_NEVER_LOCKOUT_WHITELIST and is_ip_address_in_whitelist(
         request.axes_ip_address
     ):
@@ -384,15 +468,15 @@
         request.axes_ip_address
     ):
         return True
 
     return False
 
 
-def is_client_ip_address_blacklisted(request) -> bool:
+def is_client_ip_address_blacklisted(request: HttpRequest) -> bool:
     """
     Check if the given request refers to a blacklisted IP.
     """
 
     if is_ip_address_in_blacklist(request.axes_ip_address):
         return True
 
@@ -400,26 +484,28 @@
         request.axes_ip_address
     ):
         return True
 
     return False
 
 
-def is_client_method_whitelisted(request) -> bool:
+def is_client_method_whitelisted(request: HttpRequest) -> bool:
     """
     Check if the given request uses a whitelisted method.
     """
 
     if settings.AXES_NEVER_LOCKOUT_GET and request.method == "GET":
         return True
 
     return False
 
 
-def is_user_attempt_whitelisted(request, credentials: dict = None) -> bool:
+def is_user_attempt_whitelisted(
+    request: HttpRequest, credentials: Optional[dict] = None
+) -> bool:
     """
     Check if the given request or credentials refer to a whitelisted username.
 
     This method invokes the ``settings.AXES_WHITELIST`` callable
     with ``request`` and ``credentials`` arguments.
 
     This function could use the following implementation for checking
@@ -440,15 +526,15 @@
        return user.nolockout
     """
 
     whitelist_callable = settings.AXES_WHITELIST_CALLABLE
     if whitelist_callable is None:
         return False
     if callable(whitelist_callable):
-        return whitelist_callable(request, credentials)
+        return whitelist_callable(request, credentials)  # pylint: disable=not-callable
     if isinstance(whitelist_callable, str):
         return import_string(whitelist_callable)(request, credentials)
 
     raise TypeError(
         "settings.AXES_WHITELIST_CALLABLE needs to be a string, callable, or None."
     )
```

### Comparing `django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.0b1/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files 27% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,29 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-07-17 15:56+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
+msgid "Access lock out"
+msgstr "Zugriff gesperrt"
+
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
 "account."
 msgstr ""
 "Zugang gesperrt: zu viele fehlgeschlagene Anmeldeversuche. Kontaktieren Sie "
 "einen Administrator, um Ihren Zugang zu entsperren."
 
-msgid "Account locked: too many login attempts. Please try again later"
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
 "Zugang gesperrt: zu viele fehlgeschlagene Anmeldeversuche. Bitte versuchen "
 "Sie es später erneut."
 
 msgid "Attempt Time"
 msgstr "Zugriffszeitpunkt"
 
@@ -32,14 +34,17 @@
 
 msgid "Form Data"
 msgstr "Form-Daten"
 
 msgid "GET Data"
 msgstr "GET-Daten"
 
+msgid "HTTP Accept"
+msgstr "HTTP-Accept"
+
 msgid "IP Address"
 msgstr "IP-Adresse"
 
 msgid "Logout Time"
 msgstr "Abmeldezeitpunkt"
 
 msgid "Meta Data"
@@ -59,12 +64,18 @@
 
 msgid "access attempt"
 msgstr "Zugriffsversuch"
 
 msgid "access attempts"
 msgstr "Zugriffsversuche"
 
+msgid "access failure"
+msgstr "Fehlgeschlagener Zugriff"
+
+msgid "access failures"
+msgstr "Fehlgeschlagene Zugriffe"
+
 msgid "access log"
 msgstr "Zugriffslog"
 
 msgid "access logs"
 msgstr "Zugriffslogs"
```

### Comparing `django-axes-5.9.1/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -16,82 +16,81 @@
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: axes/admin.py:38
 msgid "Form Data"
-msgstr "Form-Daten"
+msgstr "Form-Verisi"
 
 #: axes/admin.py:41 axes/admin.py:95
 msgid "Meta Data"
-msgstr "Meta-Daten"
+msgstr "Meta-Verisi"
 
 #: axes/conf.py:58
-msgid "Account locked: too many login attempts. Please try again later"
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
-"Zugang gesperrt: zu viele fehlgeschlagene Anmeldeversuche. Bitte versuchen "
-"Sie es später erneut."
+"Hesap kilitlendi: cok fazla erişim denemesi. Lütfen daha sonra tekrar deneyiniz."
 
 #: axes/conf.py:61
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
 "account."
 msgstr ""
-"Zugang gesperrt: zu viele fehlgeschlagene Anmeldeversuche. Kontaktieren Sie "
-"einen Administrator, um Ihren Zugang zu entsperren."
+"Hesap kilitlendi: cok fazla erişim denemesi. Hesabını açtırmak için yöneticiyle iletişime"
+"geçin."
 
 #: axes/models.py:9
 msgid "User Agent"
-msgstr "Browserkennung"
+msgstr ""
 
 #: axes/models.py:15
 msgid "IP Address"
-msgstr "IP-Adresse"
+msgstr "IP-Adresi"
 
 #: axes/models.py:21
 msgid "Username"
-msgstr "Benutzername"
+msgstr "Kullanıcı Adı"
 
 #: axes/models.py:35
 msgid "HTTP Accept"
 msgstr ""
 
 #: axes/models.py:40
 msgid "Path"
-msgstr "Pfad"
+msgstr "Yol"
 
 #: axes/models.py:45
 msgid "Attempt Time"
-msgstr "Zugriffszeitpunkt"
+msgstr "Girişim Zamanı"
 
 #: axes/models.py:57
 msgid "GET Data"
-msgstr "GET-Daten"
+msgstr "GET-Verisi"
 
 #: axes/models.py:61
 msgid "POST Data"
-msgstr "POST-Daten"
+msgstr "POST-Verisi"
 
 #: axes/models.py:65
 msgid "Failed Logins"
-msgstr "Fehlgeschlagene Anmeldeversuche"
+msgstr "Geçersiz Girişler"
 
 #: axes/models.py:76
 msgid "access attempt"
-msgstr "Zugriffsversuch"
+msgstr "erişim denemesi"
 
 #: axes/models.py:77
 msgid "access attempts"
-msgstr "Zugriffsversuche"
+msgstr "erişim denemeleri"
 
 #: axes/models.py:81
 msgid "Logout Time"
-msgstr "Abmeldezeitpunkt"
+msgstr "Çıkış Zamanı"
 
 #: axes/models.py:90
 msgid "access log"
-msgstr "Zugriffslog"
+msgstr "erişim kaydı"
 
 #: axes/models.py:91
 msgid "access logs"
-msgstr "Zugriffslogs"
+msgstr "erişim kayıtları"
```

### Comparing `django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-01-11 12:20+0300\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -15,15 +14,15 @@
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
 "account."
 msgstr ""
 "Учетная запись заблокирована: слишком много попыток входа. Обратитесь к "
 "администратору для разблокирования учетной записи."
 
-msgid "Account locked: too many login attempts. Please try again later"
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
 "Учетная запись заблокирована: слишком много попыток входа. Повторите попытку "
 "позже."
 
 msgid "Attempt Time"
 msgstr "Время входа"
```

### Comparing `django-axes-5.9.1/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.0b1/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 msgstr "Данные формы"
 
 #: axes/admin.py:41 axes/admin.py:95
 msgid "Meta Data"
 msgstr "Метаданные"
 
 #: axes/conf.py:58
-msgid "Account locked: too many login attempts. Please try again later"
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
 "Учетная запись заблокирована: слишком много попыток входа. "
 "Повторите попытку позже."
 
 #: axes/conf.py:61
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
```

### Comparing `django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.0b1/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,32 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-07-17 15:56+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
 "account."
 msgstr ""
 "Hesap kilitlendi: cok fazla erişim denemesi. Hesabını açtırmak için "
-"yöneticiyle iletişimegeçin"
+"yöneticiyle iletişimegeçin."
 
-msgid "Account locked: too many login attempts. Please try again later"
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
 "Hesap kilitlendi: cok fazla erişim denemesi. Lütfen daha sonra tekrar "
-"deneyiniz"
+"deneyiniz."
 
 msgid "Attempt Time"
 msgstr "Girişim Zamanı"
 
 msgid "Failed Logins"
 msgstr "Geçersiz Girişler"
```

### Comparing `django-axes-5.9.1/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.0b1/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,100 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
+"Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2018-07-17 15:56+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2021-06-11 23:36+0200\n"
+"PO-Revision-Date: 2021-06-16 10:51+0300\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n==1 ? 0 : (n%10>=2 && n%10<=4) && (n"
+"%100<12 || n%100>14) ? 1 : n!=1 && (n%10>=0 && n%10<=1) || (n%10>=5 && n"
+"%10<=9) || (n%100>=12 && n%100<=14) ? 2 : 3);\n"
+"Last-Translator: \n"
+"Language-Team: \n"
+"X-Generator: Poedit 3.0\n"
 
-#: axes/admin.py:38
+#: .\axes\admin.py:26
 msgid "Form Data"
-msgstr "Form-Verisi"
+msgstr "Dane formularza"
 
-#: axes/admin.py:41 axes/admin.py:95
+#: .\axes\admin.py:27 .\axes\admin.py:64
 msgid "Meta Data"
-msgstr "Meta-Verisi"
+msgstr "Metadane"
 
-#: axes/conf.py:58
-msgid "Account locked: too many login attempts. Please try again later"
+#: .\axes\conf.py:89
+msgid "Account locked: too many login attempts. Please try again later."
 msgstr ""
-"Hesap kilitlendi: cok fazla erişim denemesi. Lütfen daha sonra tekrar deneyiniz"
+"Konto zablokowane: zbyt wiele prób logowania. Spróbuj ponownie później."
 
-#: axes/conf.py:61
+#: .\axes\conf.py:97
 msgid ""
 "Account locked: too many login attempts. Contact an admin to unlock your "
 "account."
 msgstr ""
-"Hesap kilitlendi: cok fazla erişim denemesi. Hesabını açtırmak için yöneticiyle iletişime"
-"geçin"
+"Konto zablokowane: zbyt wiele prób logowania. Skontaktuj się z "
+"administratorem, aby odblokować swoje konto."
 
-#: axes/models.py:9
+#: .\axes\models.py:6
+#, fuzzy
 msgid "User Agent"
-msgstr ""
+msgstr "User Agent"
 
-#: axes/models.py:15
+#: .\axes\models.py:8
 msgid "IP Address"
-msgstr "IP-Adresi"
+msgstr "Adres IP"
 
-#: axes/models.py:21
+#: .\axes\models.py:10
 msgid "Username"
-msgstr "Kullanıcı Adı"
+msgstr "Nazwa Użytkownika"
 
-#: axes/models.py:35
+#: .\axes\models.py:12
+#, fuzzy
 msgid "HTTP Accept"
-msgstr ""
+msgstr "HTTP Accept"
 
-#: axes/models.py:40
+#: .\axes\models.py:14
 msgid "Path"
-msgstr "Yol"
+msgstr "Ścieżka"
 
-#: axes/models.py:45
+#: .\axes\models.py:16
 msgid "Attempt Time"
-msgstr "Girişim Zamanı"
+msgstr "Czas wystąpienia"
 
-#: axes/models.py:57
+#: .\axes\models.py:25
 msgid "GET Data"
-msgstr "GET-Verisi"
+msgstr "Dane GET"
 
-#: axes/models.py:61
+#: .\axes\models.py:27
 msgid "POST Data"
-msgstr "POST-Verisi"
+msgstr "Dane POST"
 
-#: axes/models.py:65
+#: .\axes\models.py:29
 msgid "Failed Logins"
-msgstr "Geçersiz Girişler"
+msgstr "Nieudane logowania"
 
-#: axes/models.py:76
+#: .\axes\models.py:35
 msgid "access attempt"
-msgstr "erişim denemesi"
+msgstr "próba dostępu"
 
-#: axes/models.py:77
+#: .\axes\models.py:36
 msgid "access attempts"
-msgstr "erişim denemeleri"
+msgstr "próby dostępu"
 
-#: axes/models.py:81
+#: .\axes\models.py:40
 msgid "Logout Time"
-msgstr "Çıkış Zamanı"
+msgstr "Czas wylogowania"
 
-#: axes/models.py:90
+#: .\axes\models.py:46
 msgid "access log"
-msgstr "erişim kaydı"
+msgstr "dziennik logowania"
 
-#: axes/models.py:91
+#: .\axes\models.py:47
 msgid "access logs"
-msgstr "erişim kayıtları"
+msgstr "dzienniki logowania"
```

### Comparing `django-axes-5.9.1/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.0b1/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.0b1/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/axes/management/commands/axes_reset_user.py` & `django-axes-6.0.0b1/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/axes/middleware.py` & `django-axes-6.0.0b1/axes/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from typing import Callable
 
 from django.conf import settings
+from django.http import HttpRequest, HttpResponse
 
-from axes.helpers import (
-    get_lockout_response,
-    get_failure_limit,
-    get_client_username,
-    get_credentials,
-)
-
-from axes.handlers.proxy import AxesProxyHandler
+from axes.helpers import get_lockout_response
 
 
 class AxesMiddleware:
     """
     Middleware that calculates necessary HTTP request attributes for attempt monitoring
     and maps lockout signals into readable HTTP 403 Forbidden responses.
 
@@ -32,32 +26,19 @@
 
     - ``AXES_LOCKOUT_TEMPLATE``,
     - ``AXES_LOCKOUT_URL``,
     - ``AXES_COOLOFF_MESSAGE``, and
     - ``AXES_PERMALOCK_MESSAGE``.
     """
 
-    def __init__(self, get_response: Callable):
+    def __init__(self, get_response: Callable) -> None:
         self.get_response = get_response
 
-    def __call__(self, request):
+    def __call__(self, request: HttpRequest) -> HttpResponse:
         response = self.get_response(request)
 
         if settings.AXES_ENABLED:
-            if "rest_framework" in settings.INSTALLED_APPS:
-                AxesProxyHandler.update_request(request)
-                username = get_client_username(request)
-                credentials = get_credentials(username)
-                failures_since_start = AxesProxyHandler.get_failures(
-                    request, credentials
-                )
-                if (
-                    settings.AXES_LOCK_OUT_AT_FAILURE
-                    and failures_since_start >= get_failure_limit(request, credentials)
-                ):
-
-                    request.axes_locked_out = True
-
             if getattr(request, "axes_locked_out", None):
-                response = get_lockout_response(request)  # type: ignore
+                credentials = getattr(request, "axes_credentials", None)
+                response = get_lockout_response(request, credentials)  # type: ignore
 
         return response
```

### Comparing `django-axes-5.9.1/axes/migrations/0001_initial.py` & `django-axes-6.0.0b1/axes/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="AccessAttempt",
             fields=[
                 (
```

### Comparing `django-axes-5.9.1/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.0b1/axes/migrations/0002_auto_20151217_2044.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("axes", "0001_initial")]
 
     operations = [
         migrations.AlterField(
             model_name="accessattempt",
             name="ip_address",
             field=models.GenericIPAddressField(
```

### Comparing `django-axes-5.9.1/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.0b1/axes/migrations/0003_auto_20160322_0929.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import models, migrations
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("axes", "0002_auto_20151217_2044")]
 
     operations = [
         migrations.AlterField(
             model_name="accessattempt",
             name="failures_since_start",
             field=models.PositiveIntegerField(verbose_name="Failed Logins"),
```

### Comparing `django-axes-5.9.1/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.0b1/axes/migrations/0004_auto_20181024_1538.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [("axes", "0003_auto_20160322_0929")]
 
     operations = [
         migrations.AlterModelOptions(
             name="accessattempt",
             options={
                 "verbose_name": "access attempt",
```

### Comparing `django-axes-5.9.1/axes/signals.py` & `django-axes-6.0.0b1/axes/signals.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from django.contrib.auth.signals import (
     user_logged_in,
     user_logged_out,
     user_login_failed,
 )
 from django.core.signals import setting_changed
 from django.db.models.signals import post_save, post_delete
-from django.dispatch import receiver
 from django.dispatch import Signal
+from django.dispatch import receiver
 
-from axes.models import AccessAttempt
 from axes.handlers.proxy import AxesProxyHandler
+from axes.models import AccessAttempt
 
 log = getLogger(__name__)
 
 
 # This signal provides the following arguments to any listeners:
 # request - The current Request object.
 # username - The username of the User who has been locked out.
```

### Comparing `django-axes-5.9.1/axes/tests/base.py` & `django-axes-6.0.0b1/tests/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from django.contrib.auth import get_user_model
 from django.http import HttpRequest
 from django.test import TestCase
 from django.urls import reverse
 from django.utils.timezone import now
 
-from axes.utils import reset
 from axes.conf import settings
 from axes.helpers import (
     get_cache,
     get_client_http_accept,
     get_client_ip_address,
     get_client_path_info,
     get_client_user_agent,
     get_cool_off,
     get_credentials,
     get_failure_limit,
 )
-from axes.models import AccessAttempt, AccessLog
+from axes.models import AccessAttempt, AccessLog, AccessFailureLog
+from axes.utils import reset
 
 
 def custom_failure_limit(request, credentials):
     return 3
 
 
 class AxesTestCase(TestCase):
@@ -44,15 +44,15 @@
 
     LOCKED_MESSAGE = "Account locked: too many login attempts."
     LOGOUT_MESSAGE = "Logged out"
     LOGIN_FORM_KEY = '<input type="submit" value="Log in" />'
 
     STATUS_SUCCESS = 200
     ALLOWED = 302
-    BLOCKED = 403
+    BLOCKED = 429
 
     def setUp(self):
         """
         Create a valid user for login.
         """
 
         self.username = self.VALID_USERNAME
@@ -74,14 +74,16 @@
         self.request.META["PATH_INFO"] = self.path_info
 
         self.request.axes_attempt_time = now()
         self.request.axes_ip_address = get_client_ip_address(self.request)
         self.request.axes_user_agent = get_client_user_agent(self.request)
         self.request.axes_path_info = get_client_path_info(self.request)
         self.request.axes_http_accept = get_client_http_accept(self.request)
+        self.request.axes_failures_since_start = None
+        self.request.axes_locked_out = False
 
         self.credentials = get_credentials(self.username)
 
     def tearDown(self):
         get_cache().clear()
 
     def get_kwargs_with_defaults(self, **kwargs):
@@ -98,18 +100,27 @@
         kwargs = self.get_kwargs_with_defaults(**kwargs)
         kwargs.setdefault("failures_since_start", 1)
         return AccessAttempt.objects.create(**kwargs)
 
     def create_log(self, **kwargs):
         return AccessLog.objects.create(**self.get_kwargs_with_defaults(**kwargs))
 
+    def create_failure_log(self, **kwargs):
+        return AccessFailureLog.objects.create(**self.get_kwargs_with_defaults(**kwargs))
+
     def reset(self, ip=None, username=None):
         return reset(ip, username)
 
-    def login(self, is_valid_username=False, is_valid_password=False, **kwargs):
+    def login(
+        self,
+        is_valid_username=False,
+        is_valid_password=False,
+        remote_addr=None,
+        **kwargs
+    ):
         """
         Login a user.
 
         A valid credential is used when is_valid_username is True,
         otherwise it will use a random string to make a failed login.
         """
 
@@ -124,15 +135,15 @@
             password = self.INVALID_PASSWORD
 
         post_data = {"username": username, "password": password, **kwargs}
 
         return self.client.post(
             reverse("admin:login"),
             post_data,
-            REMOTE_ADDR=self.ip_address,
+            REMOTE_ADDR=remote_addr or self.ip_address,
             HTTP_USER_AGENT=self.user_agent,
         )
 
     def logout(self):
         return self.client.post(
             reverse("admin:logout"),
             REMOTE_ADDR=self.ip_address,
```

### Comparing `django-axes-5.9.1/axes/tests/settings.py` & `django-axes-6.0.0b1/tests/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,21 +16,24 @@
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "axes.middleware.AxesMiddleware",
 ]
 
 AUTHENTICATION_BACKENDS = [
-    "axes.backends.AxesBackend",
+    "axes.backends.AxesStandaloneBackend",
     "django.contrib.auth.backends.ModelBackend",
 ]
 
+# Use MD5 for tests as it is considerably faster than other options
+# note that this should never be used in any online setting
+# where users actually log in to the system due to easy exploitability
 PASSWORD_HASHERS = ["django.contrib.auth.hashers.MD5PasswordHasher"]
 
-ROOT_URLCONF = "axes.tests.urls"
+ROOT_URLCONF = "tests.urls"
 
 INSTALLED_APPS = [
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.sites",
     "django.contrib.messages",
@@ -61,14 +64,14 @@
     "loggers": {"axes": {"handlers": ["console"], "level": "INFO", "propagate": False}},
 }
 
 SECRET_KEY = "too-secret-for-test"
 
 USE_I18N = False
 
-USE_L10N = False
-
 USE_TZ = False
 
 LOGIN_REDIRECT_URL = "/admin/"
 
 AXES_FAILURE_LIMIT = 10
+
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
```

### Comparing `django-axes-5.9.1/axes/tests/test_attempts.py` & `django-axes-6.0.0b1/tests/test_attempts.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from django.http import HttpRequest
 from django.test import override_settings
 from django.utils.timezone import now
 
 from axes.attempts import get_cool_off_threshold
 from axes.models import AccessAttempt
-from axes.tests.base import AxesTestCase
 from axes.utils import reset, reset_request
+from tests.base import AxesTestCase
 
 
 class GetCoolOffThresholdTestCase(AxesTestCase):
     @override_settings(AXES_COOLOFF_TIME=42)
     def test_get_cool_off_threshold(self):
         timestamp = now()
```

### Comparing `django-axes-5.9.1/axes/tests/test_backends.py` & `django-axes-6.0.0b1/tests/test_backends.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from unittest.mock import patch, MagicMock
 
 from axes.backends import AxesBackend
 from axes.exceptions import (
     AxesBackendRequestParameterRequired,
     AxesBackendPermissionDenied,
 )
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
 
 
 class BackendTestCase(AxesTestCase):
     def test_authenticate_raises_on_missing_request(self):
         request = None
 
         with self.assertRaises(AxesBackendRequestParameterRequired):
```

### Comparing `django-axes-5.9.1/axes/tests/test_checks.py` & `django-axes-6.0.0b1/tests/test_checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.core.checks import run_checks, Warning  # pylint: disable=redefined-builtin
 from django.test import override_settings, modify_settings
 
-from axes.backends import AxesBackend
+from axes.backends import AxesStandaloneBackend
 from axes.checks import Messages, Hints, Codes
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
 
 
 class CacheCheckTestCase(AxesTestCase):
     @override_settings(
         AXES_HANDLER="axes.handlers.cache.AxesCacheHandler",
         CACHES={
             "default": {
@@ -54,39 +54,41 @@
             hint=Hints.MIDDLEWARE_INVALID,
             id=Codes.MIDDLEWARE_INVALID,
         )
 
         self.assertEqual(warnings, [warning])
 
 
-class AxesSpecializedBackend(AxesBackend):
+class AxesSpecializedBackend(AxesStandaloneBackend):
     pass
 
 
 class BackendCheckTestCase(AxesTestCase):
-    @modify_settings(AUTHENTICATION_BACKENDS={"remove": ["axes.backends.AxesBackend"]})
+    @modify_settings(
+        AUTHENTICATION_BACKENDS={"remove": ["axes.backends.AxesStandaloneBackend"]}
+    )
     def test_backend_missing(self):
         warnings = run_checks()
         warning = Warning(
             msg=Messages.BACKEND_INVALID,
             hint=Hints.BACKEND_INVALID,
             id=Codes.BACKEND_INVALID,
         )
 
         self.assertEqual(warnings, [warning])
 
     @override_settings(
-        AUTHENTICATION_BACKENDS=["axes.tests.test_checks.AxesSpecializedBackend"]
+        AUTHENTICATION_BACKENDS=["tests.test_checks.AxesSpecializedBackend"]
     )
     def test_specialized_backend(self):
         warnings = run_checks()
         self.assertEqual(warnings, [])
 
     @override_settings(
-        AUTHENTICATION_BACKENDS=["axes.tests.test_checks.AxesNotDefinedBackend"]
+        AUTHENTICATION_BACKENDS=["tests.test_checks.AxesNotDefinedBackend"]
     )
     def test_import_error(self):
         with self.assertRaises(ImportError):
             run_checks()
 
     @override_settings(AUTHENTICATION_BACKENDS=["module.not_defined"])
     def test_module_not_found_error(self):
```

### Comparing `django-axes-5.9.1/axes/tests/test_decorators.py` & `django-axes-6.0.0b1/tests/test_decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest.mock import MagicMock, patch
 
 from django.http import HttpResponse
 
 from axes.decorators import axes_dispatch, axes_form_invalid
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
 
 
 class DecoratorTestCase(AxesTestCase):
     SUCCESS_RESPONSE = HttpResponse(status=200, content="Dispatched")
-    LOCKOUT_RESPONSE = HttpResponse(status=403, content="Locked out")
+    LOCKOUT_RESPONSE = HttpResponse(status=429, content="Locked out")
 
     def setUp(self):
         self.request = MagicMock()
         self.cls = MagicMock(return_value=self.request)
         self.func = MagicMock(return_value=self.SUCCESS_RESPONSE)
 
     @patch("axes.handlers.proxy.AxesProxyHandler.is_allowed", return_value=False)
```

### Comparing `django-axes-5.9.1/axes/tests/test_handlers.py` & `django-axes-6.0.0b1/tests/test_handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+from platform import python_implementation
 from unittest.mock import MagicMock, patch
 
+from pytest import mark
+
+from django.core.cache import cache
 from django.test import override_settings
 from django.urls import reverse
 from django.utils import timezone
 from django.utils.timezone import timedelta
 
 from axes.conf import settings
 from axes.handlers.proxy import AxesProxyHandler
 from axes.helpers import get_client_str
-from axes.models import AccessAttempt, AccessLog
-from axes.tests.base import AxesTestCase
+from axes.models import AccessAttempt, AccessLog, AccessFailureLog
+from tests.base import AxesTestCase
 
 
 @override_settings(AXES_HANDLER="axes.handlers.base.AxesHandler")
 class AxesHandlerTestCase(AxesTestCase):
     @override_settings(AXES_IP_BLACKLIST=["127.0.0.1"])
     def test_is_allowed_with_blacklisted_ip_address(self):
         self.assertFalse(AxesProxyHandler.is_allowed(self.request))
@@ -49,15 +53,15 @@
         )
 
         for setting_value, url, expected in tests:
             with override_settings(AXES_ONLY_ADMIN_SITE=setting_value):
                 request.path = url
                 self.assertEqual(AxesProxyHandler().is_admin_site(request), expected)
 
-    @override_settings(ROOT_URLCONF="axes.tests.urls_empty")
+    @override_settings(ROOT_URLCONF="tests.urls_empty")
     @override_settings(AXES_ONLY_ADMIN_SITE=True)
     def test_is_admin_site_no_admin_site(self):
         request = MagicMock()
         request.path = "/admin/"
         self.assertTrue(AxesProxyHandler().is_admin_site(self.request))
 
 
@@ -112,30 +116,34 @@
         with override_settings(
             AXES_NEVER_LOCKOUT_WHITELIST=True, AXES_IP_WHITELIST=[self.ip_address]
         ):
             AxesProxyHandler.user_login_failed(
                 sender=None, request=self.request, credentials=self.credentials
             )
             client_str = get_client_str(
-                self.username, self.ip_address, self.user_agent, self.path_info
+                self.username,
+                self.ip_address,
+                self.user_agent,
+                self.path_info,
+                self.request,
             )
             log.info.assert_called_with(
                 "AXES: Login failed from whitelisted client %s.", client_str
             )
 
     def check_empty_request(self, log, handler):
         AxesProxyHandler.user_login_failed(sender=None, credentials={}, request=None)
         log.error.assert_called_with(
             f"AXES: {handler}.user_login_failed does not function without a request."
         )
 
 
 @override_settings(AXES_HANDLER="axes.handlers.database.AxesDatabaseHandler")
 class ResetAttemptsTestCase(AxesHandlerBaseTestCase):
-    """ Resetting attempts is currently implemented only for database handler """
+    """Resetting attempts is currently implemented only for database handler"""
 
     USERNAME_1 = "foo_username"
     USERNAME_2 = "bar_username"
     IP_1 = "127.1.0.1"
     IP_2 = "127.1.0.2"
 
     def setUp(self):
@@ -200,14 +208,20 @@
         )
 
 
 @override_settings(
     AXES_HANDLER="axes.handlers.database.AxesDatabaseHandler",
     AXES_COOLOFF_TIME=timedelta(seconds=2),
     AXES_RESET_ON_SUCCESS=True,
+    AXES_ENABLE_ACCESS_FAILURE_LOG=True,
+)
+@mark.xfail(
+    python_implementation() == "PyPy",
+    reason="PyPy implementation is flaky for this test",
+    strict=False,
 )
 class AxesDatabaseHandlerTestCase(AxesHandlerBaseTestCase):
     def test_handler_reset_attempts(self):
         self.create_attempt()
         self.assertEqual(1, AxesProxyHandler.reset_attempts())
         self.assertFalse(AccessAttempt.objects.count())
 
@@ -223,27 +237,49 @@
         with patch("django.utils.timezone.now", return_value=then):
             self.create_log()
 
         self.assertEqual(AccessLog.objects.count(), 2)
         self.assertEqual(1, AxesProxyHandler.reset_logs(age_days=42))
         self.assertEqual(AccessLog.objects.count(), 1)
 
+    def test_handler_reset_failure_logs(self):
+        self.create_failure_log()
+        self.assertEqual(1, AxesProxyHandler.reset_failure_logs())
+        self.assertFalse(AccessFailureLog.objects.count())
+
+    def test_handler_reset_failure_logs_older_than_42_days(self):
+        self.create_failure_log()
+
+        then = timezone.now() - timezone.timedelta(days=90)
+        with patch("django.utils.timezone.now", return_value=then):
+            self.create_failure_log()
+
+        self.assertEqual(AccessFailureLog.objects.count(), 2)
+        self.assertEqual(1, AxesProxyHandler.reset_failure_logs(age_days=42))
+        self.assertEqual(AccessFailureLog.objects.count(), 1)
+
+    def test_handler_remove_out_of_limit_failure_logs(self):
+        _more = 10
+        for i in range(settings.AXES_ACCESS_FAILURE_LOG_PER_USER_LIMIT + _more):
+            self.create_failure_log()
+        self.assertEqual(_more, AxesProxyHandler.remove_out_of_limit_failure_logs(username=self.username))
+
     @override_settings(AXES_RESET_ON_SUCCESS=True)
     def test_handler(self):
         self.check_handler()
 
     @override_settings(AXES_RESET_ON_SUCCESS=False)
     def test_handler_without_reset(self):
         self.check_handler()
 
     @override_settings(AXES_FAILURE_LIMIT=lambda *args: 3)
     def test_handler_callable_failure_limit(self):
         self.check_handler()
 
-    @override_settings(AXES_FAILURE_LIMIT="axes.tests.base.custom_failure_limit")
+    @override_settings(AXES_FAILURE_LIMIT="tests.base.custom_failure_limit")
     def test_handler_str_failure_limit(self):
         self.check_handler()
 
     @override_settings(AXES_FAILURE_LIMIT=None)
     def test_handler_invalid_failure_limit(self):
         with self.assertRaises(TypeError):
             self.check_handler()
@@ -256,24 +292,24 @@
     def test_empty_request(self, log):
         self.check_empty_request(log, "AxesDatabaseHandler")
 
     @patch("axes.handlers.database.log")
     def test_whitelist(self, log):
         self.check_whitelist(log)
 
+    @override_settings(AXES_ONLY_USER_FAILURES=True)
     @patch("axes.handlers.database.log")
     def test_user_login_failed_only_user_failures_with_none_username(self, log):
-        with self.settings(**{"AXES_ONLY_USER_FAILURES": True}):
-            credentials = {"username": None, "password": "test"}
-            sender = MagicMock()
-            AxesProxyHandler.user_login_failed(sender, credentials, self.request)
-            attempt = AccessAttempt.objects.all()
-            self.assertEqual(0, AccessAttempt.objects.count())
+        credentials = {"username": None, "password": "test"}
+        sender = MagicMock()
+        AxesProxyHandler.user_login_failed(sender, credentials, self.request)
+        attempt = AccessAttempt.objects.all()
+        self.assertEqual(0, AccessAttempt.objects.count())
         log.warning.assert_called_with(
-            "AXES: Username is None and AXES_ONLY_USER_FAILURES is enable, New record won't be created."
+            "AXES: Username is None and AXES_ONLY_USER_FAILURES is enabled, new record will NOT be created."
         )
 
     def test_user_login_failed_with_none_username(self):
         credentials = {"username": None, "password": "test"}
         sender = MagicMock()
         AxesProxyHandler.user_login_failed(sender, credentials, self.request)
         attempt = AccessAttempt.objects.all()
@@ -325,14 +361,106 @@
                     self.assertEqual(
                         total_attempts_count, AccessAttempt.objects.count()
                     )
 
             AccessAttempt.objects.all().delete()
 
 
+@override_settings(AXES_HANDLER="axes.handlers.cache.AxesCacheHandler")
+class ResetAttemptsCacheHandlerTestCase(AxesHandlerBaseTestCase):
+    """Test reset attempts for the cache handler"""
+
+    USERNAME_1 = "foo_username"
+    USERNAME_2 = "bar_username"
+    IP_1 = "127.1.0.1"
+    IP_2 = "127.1.0.2"
+
+    def set_up_login_attempts(self):
+        """Set up the login attempts."""
+        self.login(username=self.USERNAME_1, remote_addr=self.IP_1)
+        self.login(username=self.USERNAME_1, remote_addr=self.IP_2)
+        self.login(username=self.USERNAME_2, remote_addr=self.IP_1)
+        self.login(username=self.USERNAME_2, remote_addr=self.IP_2)
+
+    def check_failures(self, failures, username=None, ip_address=None):
+        if ip_address is None and username is None:
+            raise NotImplementedError("Must supply ip_address or username")
+        try:
+            prev_ip = self.request.META["REMOTE_ADDR"]
+            credentials = {"username": username} if username else {}
+            if ip_address is not None:
+                self.request.META["REMOTE_ADDR"] = ip_address
+            self.assertEqual(
+                failures,
+                AxesProxyHandler.get_failures(self.request, credentials=credentials),
+            )
+        finally:
+            self.request.META["REMOTE_ADDR"] = prev_ip
+
+    def test_handler_reset_attempts(self):
+        with self.assertRaises(NotImplementedError):
+            AxesProxyHandler.reset_attempts()
+
+    @override_settings(AXES_ONLY_USER_FAILURES=True)
+    def test_handler_reset_attempts_username(self):
+        self.set_up_login_attempts()
+        self.assertEqual(
+            2,
+            AxesProxyHandler.get_failures(
+                self.request, credentials={"username": self.USERNAME_1}
+            ),
+        )
+        self.assertEqual(
+            2,
+            AxesProxyHandler.get_failures(
+                self.request, credentials={"username": self.USERNAME_2}
+            ),
+        )
+        self.assertEqual(1, AxesProxyHandler.reset_attempts(username=self.USERNAME_1))
+        self.assertEqual(
+            0,
+            AxesProxyHandler.get_failures(
+                self.request, credentials={"username": self.USERNAME_1}
+            ),
+        )
+        self.assertEqual(
+            2,
+            AxesProxyHandler.get_failures(
+                self.request, credentials={"username": self.USERNAME_2}
+            ),
+        )
+
+    def test_handler_reset_attempts_ip(self):
+        self.set_up_login_attempts()
+        self.check_failures(2, ip_address=self.IP_1)
+        self.assertEqual(1, AxesProxyHandler.reset_attempts(ip_address=self.IP_1))
+        self.check_failures(0, ip_address=self.IP_1)
+        self.check_failures(2, ip_address=self.IP_2)
+
+    @override_settings(AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=True)
+    def test_handler_reset_attempts_ip_and_username(self):
+        self.set_up_login_attempts()
+        self.check_failures(1, username=self.USERNAME_1, ip_address=self.IP_1)
+        self.check_failures(1, username=self.USERNAME_2, ip_address=self.IP_1)
+        self.check_failures(1, username=self.USERNAME_1, ip_address=self.IP_2)
+        self.assertEqual(
+            1,
+            AxesProxyHandler.reset_attempts(
+                ip_address=self.IP_1, username=self.USERNAME_1
+            ),
+        )
+        self.check_failures(0, username=self.USERNAME_1, ip_address=self.IP_1)
+        self.check_failures(1, username=self.USERNAME_2, ip_address=self.IP_1)
+        self.check_failures(1, username=self.USERNAME_1, ip_address=self.IP_2)
+
+    def test_handler_reset_attempts_ip_or_username(self):
+        with self.assertRaises(NotImplementedError):
+            AxesProxyHandler.reset_attempts()
+
+
 @override_settings(
     AXES_HANDLER="axes.handlers.cache.AxesCacheHandler",
     AXES_COOLOFF_TIME=timedelta(seconds=1),
 )
 class AxesCacheHandlerTestCase(AxesHandlerBaseTestCase):
     @override_settings(AXES_RESET_ON_SUCCESS=True)
     def test_handler(self):
@@ -350,14 +478,35 @@
     def test_empty_request(self, log):
         self.check_empty_request(log, "AxesCacheHandler")
 
     @patch("axes.handlers.cache.log")
     def test_whitelist(self, log):
         self.check_whitelist(log)
 
+    @override_settings(AXES_ONLY_USER_FAILURES=True)
+    @patch.object(cache, "set")
+    @patch("axes.handlers.cache.log")
+    def test_user_login_failed_only_user_failures_with_none_username(
+        self, log, cache_set
+    ):
+        credentials = {"username": None, "password": "test"}
+        sender = MagicMock()
+        AxesProxyHandler.user_login_failed(sender, credentials, self.request)
+        self.assertFalse(cache_set.called)
+        log.warning.assert_called_with(
+            "AXES: Username is None and AXES_ONLY_USER_FAILURES is enabled, new record will NOT be created."
+        )
+
+    @patch.object(cache, "set")
+    def test_user_login_failed_with_none_username(self, cache_set):
+        credentials = {"username": None, "password": "test"}
+        sender = MagicMock()
+        AxesProxyHandler.user_login_failed(sender, credentials, self.request)
+        self.assertTrue(cache_set.called)
+
 
 @override_settings(AXES_HANDLER="axes.handlers.dummy.AxesDummyHandler")
 class AxesDummyHandlerTestCase(AxesHandlerBaseTestCase):
     def test_handler(self):
         for _ in range(settings.AXES_FAILURE_LIMIT):
             self.login()
```

### Comparing `django-axes-5.9.1/axes/tests/test_logging.py` & `django-axes-6.0.0b1/tests/test_logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from unittest.mock import patch
 
 from django.test import override_settings
 from django.urls import reverse
+from pkg_resources import get_distribution
 
 from axes.apps import AppConfig
 from axes.models import AccessAttempt, AccessLog
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
+
+_BEGIN = "AXES: BEGIN version %s, %s"
+_VERSION = get_distribution("django-axes").version
 
 
 @patch("axes.apps.AppConfig.initialized", False)
 @patch("axes.apps.log")
 class AppsTestCase(AxesTestCase):
     def test_axes_config_log_re_entrant(self, log):
         """
@@ -29,46 +33,47 @@
     def test_axes_config_log_not_verbose(self, log):
         AppConfig.initialize()
         self.assertFalse(log.info.called)
 
     @override_settings(AXES_ONLY_USER_FAILURES=True)
     def test_axes_config_log_user_only(self, log):
         AppConfig.initialize()
-        log.info.assert_called_with("AXES: blocking by username only.")
+        log.info.assert_called_with(_BEGIN, _VERSION, "blocking by username only")
 
     @override_settings(AXES_ONLY_USER_FAILURES=False)
     def test_axes_config_log_ip_only(self, log):
         AppConfig.initialize()
-        log.info.assert_called_with("AXES: blocking by IP only.")
+        log.info.assert_called_with(_BEGIN, _VERSION, "blocking by IP only")
 
     @override_settings(AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=True)
     def test_axes_config_log_user_ip(self, log):
         AppConfig.initialize()
-        log.info.assert_called_with("AXES: blocking by combination of username and IP.")
+        log.info.assert_called_with(_BEGIN, _VERSION, "blocking by combination of username and IP")
 
     @override_settings(AXES_LOCK_OUT_BY_USER_OR_IP=True)
     def test_axes_config_log_user_or_ip(self, log):
         AppConfig.initialize()
-        log.info.assert_called_with("AXES: blocking by username or IP.")
+        log.info.assert_called_with(_BEGIN, _VERSION, "blocking by username or IP")
 
 
 class AccessLogTestCase(AxesTestCase):
     def test_access_log_on_logout(self):
         """
         Test a valid logout and make sure the logout_time is updated.
         """
 
         self.login(is_valid_username=True, is_valid_password=True)
         self.assertIsNone(AccessLog.objects.latest("id").logout_time)
 
-        response = self.client.get(reverse("admin:logout"))
+        response = self.client.post(reverse("admin:logout"))
         self.assertContains(response, "Logged out")
 
         self.assertIsNotNone(AccessLog.objects.latest("id").logout_time)
 
+    @override_settings(DATA_UPLOAD_MAX_NUMBER_FIELDS=1500)
     def test_log_data_truncated(self):
         """
         Test that get_query_str properly truncates data to the max_length (default 1024).
         """
 
         # An impossibly large post dict
         extra_data = {"a" * x: x for x in range(1024)}
@@ -76,15 +81,15 @@
         self.assertEqual(len(AccessAttempt.objects.latest("id").post_data), 1024)
 
     @override_settings(AXES_DISABLE_ACCESS_LOG=True)
     def test_valid_logout_without_success_log(self):
         AccessLog.objects.all().delete()
 
         response = self.login(is_valid_username=True, is_valid_password=True)
-        response = self.client.get(reverse("admin:logout"))
+        response = self.client.post(reverse("admin:logout"))
 
         self.assertEqual(AccessLog.objects.all().count(), 0)
         self.assertContains(response, "Logged out", html=True)
 
     @override_settings(AXES_DISABLE_ACCESS_LOG=True)
     def test_valid_login_without_success_log(self):
         """
@@ -99,15 +104,15 @@
         self.assertEqual(AccessLog.objects.all().count(), 0)
 
     @override_settings(AXES_DISABLE_ACCESS_LOG=True)
     def test_valid_logout_without_log(self):
         AccessLog.objects.all().delete()
 
         response = self.login(is_valid_username=True, is_valid_password=True)
-        response = self.client.get(reverse("admin:logout"))
+        response = self.client.post(reverse("admin:logout"))
 
         self.assertEqual(AccessLog.objects.count(), 0)
         self.assertContains(response, "Logged out", html=True)
 
     @override_settings(AXES_DISABLE_ACCESS_LOG=True)
     def test_non_valid_login_without_log(self):
         """
```

### Comparing `django-axes-5.9.1/axes/tests/test_login.py` & `django-axes-6.0.0b1/tests/test_login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Integration tests for the login handling.
 
 TODO: Clean up the tests in this module.
 """
-
+from datetime import timedelta
 from importlib import import_module
+from time import sleep
 
+from django.contrib.auth import get_user_model, login, logout
 from django.http import HttpRequest
 from django.test import override_settings, TestCase
 from django.urls import reverse
-from django.contrib.auth import get_user_model, login, logout
 
 from axes.conf import settings
+from axes.helpers import get_cache, make_cache_key_list, get_cool_off, get_failure_limit
 from axes.models import AccessAttempt
-from axes.helpers import get_cache, make_cache_key_list
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
 
 
 class DjangoLoginTestCase(TestCase):
     def setUp(self):
         engine = import_module(settings.SESSION_ENGINE)
 
         self.request = HttpRequest()
@@ -79,38 +80,38 @@
     VALID_IP_ADDRESS = IP_1
 
     WRONG_PASSWORD = "wrong-password"
     LOCKED_MESSAGE = "Account locked: too many login attempts."
     LOGIN_FORM_KEY = '<input type="submit" value="Log in" />'
     ATTEMPT_NOT_BLOCKED = 200
     ALLOWED = 302
-    BLOCKED = 403
+    BLOCKED = 429
 
-    def _login(self, username, password, ip_addr="127.0.0.1", **kwargs):
+    def _login(self, username, password, ip_addr="127.0.0.1", user_agent="test-browser", **kwargs):
         """
         Login a user and get the response.
 
         IP address can be configured to test IP blocking functionality.
         """
 
         post_data = {"username": username, "password": password}
 
         post_data.update(kwargs)
 
         return self.client.post(
             reverse("admin:login"),
             post_data,
             REMOTE_ADDR=ip_addr,
-            HTTP_USER_AGENT="test-browser",
+            HTTP_USER_AGENT=user_agent,
         )
 
-    def _lockout_user_from_ip(self, username, ip_addr):
+    def _lockout_user_from_ip(self, username, ip_addr, user_agent="test-browser"):
         for _ in range(settings.AXES_FAILURE_LIMIT):
             response = self._login(
-                username=username, password=self.WRONG_PASSWORD, ip_addr=ip_addr
+                username=username, password=self.WRONG_PASSWORD, ip_addr=ip_addr, user_agent=user_agent,
             )
         return response
 
     def _lockout_user1_from_ip1(self):
         return self._lockout_user_from_ip(username=self.USER_1, ip_addr=self.IP_1)
 
     def setUp(self):
@@ -192,15 +193,15 @@
             response = self.login(is_valid_username=True, is_valid_password=False)
             # Check if we are in the same login page
             self.assertContains(response, self.LOGIN_FORM_KEY, html=True)
 
         # So, we shouldn't have gotten a lock-out yet.
         # But we should get one now
         response = self.login(is_valid_username=True, is_valid_password=False)
-        self.assertContains(response, self.LOCKED_MESSAGE, status_code=403)
+        self.assertContains(response, self.LOCKED_MESSAGE, status_code=429)
 
     @override_settings(AXES_ONLY_USER_FAILURES=True)
     def test_lockout_by_only_user_failures(self):
         """
         Test login failure when AXES_ONLY_USER_FAILURES is True.
         """
 
@@ -363,14 +364,27 @@
         # User with empty username is locked out from IP 1.
         self._lockout_user_from_ip(username="", ip_addr=self.IP_1)
 
         # Still possible to access the login page
         response = self.client.get(reverse("admin:login"), REMOTE_ADDR=self.IP_1)
         self.assertContains(response, self.LOGIN_FORM_KEY, status_code=200, html=True)
 
+    @override_settings(AXES_USE_USER_AGENT=True)
+    def test_lockout_by_user_still_allows_login_with_differnet_user_agent(self):
+        # User with empty username is locked out with "test-browser" user agent.
+        self._lockout_user_from_ip(username="username", ip_addr=self.IP_1, user_agent="test-browser")
+
+        # Test he is locked:
+        response = self._login("username", self.VALID_PASSWORD, ip_addr=self.IP_1, user_agent="test-browser")
+        self.assertEqual(response.status_code, self.BLOCKED)
+
+        # Test with another user agent:
+        response = self._login("username", self.VALID_PASSWORD, ip_addr=self.IP_1, user_agent="test-browser-2")
+        self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
+
     # Test for true and false positives when blocking by IP *OR* user (default)
     # With cache enabled. Default criteria.
     def test_lockout_by_ip_blocks_when_same_user_same_ip_using_cache(self):
         # User 1 is locked out from IP 1.
         self._lockout_user1_from_ip1()
 
         # User 1 is still blocked from IP 1.
@@ -586,15 +600,15 @@
         response = self._login(self.USER_3, self.WRONG_PASSWORD, ip_addr=self.IP_1)
         self.assertContains(response, self.LOCKED_MESSAGE, status_code=self.BLOCKED)
 
     @override_settings(AXES_LOCK_OUT_BY_USER_OR_IP=True, AXES_FAILURE_LIMIT=3)
     def test_lockout_by_user_or_ip_allows_when_diff_user_same_ip_using_cache_multiple_failed_attempts(
         self,
     ):
-        """ Test, if the failed attempts make also impact on the attempt count """
+        """Test, if the failed attempts make also impact on the attempt count"""
         # User 1 is locked out from IP 1.
         response = self._login(self.USER_1, self.WRONG_PASSWORD, self.IP_1)
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
 
         # Second attempt from different IP
         response = self._login(self.USER_1, self.WRONG_PASSWORD, self.IP_2)
         self.assertEqual(response.status_code, self.ATTEMPT_NOT_BLOCKED)
@@ -627,14 +641,54 @@
         # User with empty username is locked out from IP 1.
         self._lockout_user_from_ip(username="", ip_addr=self.IP_1)
 
         # Still possible to access the login page
         response = self.client.get(reverse("admin:login"), REMOTE_ADDR=self.IP_1)
         self.assertContains(response, self.LOGIN_FORM_KEY, status_code=200, html=True)
 
+    @override_settings(
+        AXES_COOLOFF_TIME=timedelta(seconds=1),
+        AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT=False,
+        AXES_FAILURE_LIMIT=2,
+    )
+    def test_login_during_lockout_doesnt_reset_cool_off_time(self):
+        # Lockout
+        for _ in range(get_failure_limit(None, None)):
+            self.login(self.USER_1)
+
+        # Attempt during lockout
+        sleep_time = get_cool_off().total_seconds() / 2
+        sleep(sleep_time)
+        self.login(self.USER_1)
+        sleep(sleep_time)
+
+        # New attempt after initial lockout period: should work
+        response = self.login(is_valid_username=True, is_valid_password=True)
+        self.assertNotContains(response, self.LOCKED_MESSAGE, status_code=self.ALLOWED)
+
+    @override_settings(
+        AXES_COOLOFF_TIME=timedelta(seconds=1),
+        AXES_RESET_COOL_OFF_ON_FAILURE_DURING_LOCKOUT=True,
+        AXES_FAILURE_LIMIT=2,
+    )
+    def test_login_during_lockout_does_reset_cool_off_time(self):
+        # Lockout
+        for _ in range(get_failure_limit(None, None)):
+            self.login(self.USER_1)
+
+        # Attempt during lockout
+        sleep_time = get_cool_off().total_seconds() / 2
+        sleep(sleep_time)
+        self.login(self.USER_1)
+        sleep(sleep_time)
+
+        # New attempt after initial lockout period: should not work
+        response = self.login(is_valid_username=True, is_valid_password=True)
+        self.assertContains(response, self.LOCKED_MESSAGE, status_code=self.BLOCKED)
+
 
 # Test the same logic with cache handler
 @override_settings(AXES_HANDLER="axes.handlers.cache.AxesCacheHandler")
 class CacheLoginTestCase(DatabaseLoginTestCase):
     def attempt_count(self):
         cache = get_cache()
         keys = cache._cache
```

### Comparing `django-axes-5.9.1/axes/tests/test_management.py` & `django-axes-6.0.0b1/tests/test_management.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from io import StringIO
 from unittest.mock import patch, Mock
 
 from django.core.management import call_command
 from django.utils import timezone
 
 from axes.models import AccessAttempt, AccessLog
-from axes.tests.base import AxesTestCase
+from tests.base import AxesTestCase
 
 
 class ResetAccessLogsManagementCommandTestCase(AxesTestCase):
     def setUp(self):
         self.msg_not_found = "No logs found.\n"
         self.msg_num_found = "{} logs removed.\n"
```

### Comparing `django-axes-5.9.1/axes/tests/test_models.py` & `django-axes-6.0.0b1/tests/test_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from django.apps.registry import apps
 from django.db import connection
 from django.db.migrations.autodetector import MigrationAutodetector
 from django.db.migrations.executor import MigrationExecutor
 from django.db.migrations.state import ProjectState
 
-from axes.models import AccessAttempt, AccessLog
-from axes.tests.base import AxesTestCase
+from axes.models import AccessAttempt, AccessLog, AccessFailureLog
+from tests.base import AxesTestCase
 
 
 class ModelsTestCase(AxesTestCase):
     def setUp(self):
         self.failures_since_start = 42
 
         self.access_attempt = AccessAttempt(
             failures_since_start=self.failures_since_start
         )
         self.access_log = AccessLog()
+        self.access_failure_log = AccessFailureLog()
 
     def test_access_attempt_str(self):
         self.assertIn("Access", str(self.access_attempt))
 
     def test_access_log_str(self):
         self.assertIn("Access", str(self.access_log))
 
+    def test_access_failure_log_str(self):
+        self.assertIn("Failed", str(self.access_failure_log))
+
 
 class MigrationsTestCase(AxesTestCase):
     def test_missing_migrations(self):
         executor = MigrationExecutor(connection)
         autodetector = MigrationAutodetector(
             executor.loader.project_state(), ProjectState.from_apps(apps)
         )
```

### Comparing `django-axes-5.9.1/axes/tests/test_utils.py` & `django-axes-6.0.0b1/tests/test_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from datetime import timedelta
-from hashlib import md5
+from hashlib import sha256
 from unittest.mock import patch
 
-from django.http import JsonResponse, HttpResponseRedirect, HttpResponse, HttpRequest
-from django.test import override_settings, RequestFactory
+from django.contrib.auth import get_user_model
+from django.http import HttpRequest, HttpResponse, HttpResponseRedirect, JsonResponse
+from django.test import RequestFactory, override_settings
 
 from axes.apps import AppConfig
-from axes.models import AccessAttempt
-from axes.tests.base import AxesTestCase
 from axes.helpers import (
+    cleanse_parameters,
     get_cache_timeout,
-    get_client_str,
-    get_client_username,
     get_client_cache_key,
+    get_client_ip_address,
     get_client_parameters,
+    get_client_str,
+    get_client_username,
+    get_cool_off,
     get_cool_off_iso8601,
     get_lockout_response,
     is_client_ip_address_blacklisted,
     is_client_ip_address_whitelisted,
+    is_client_method_whitelisted,
     is_ip_address_in_blacklist,
     is_ip_address_in_whitelist,
-    is_client_method_whitelisted,
+    is_user_attempt_whitelisted,
     toggleable,
 )
+from axes.models import AccessAttempt
+from tests.base import AxesTestCase
 
 
 @override_settings(AXES_ENABLED=False)
 class AxesDisabledTestCase(AxesTestCase):
     def test_initialize(self):
         AppConfig.logging_initialized = False
         AppConfig.initialize()
@@ -87,144 +92,217 @@
     def test_verbose_ip_only_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info
+            username, ip_address, user_agent, path_info, self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_VERBOSE=True)
     def test_imbalanced_quotes(self):
         username = "butterfly.. },,,"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info
+            username, ip_address, user_agent, path_info, self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_VERBOSE=True)
     def test_verbose_ip_only_client_details_tuple(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = ("admin", "login")
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info[0]
+            username, ip_address, user_agent, path_info[0], self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_VERBOSE=False)
     def test_non_verbose_ip_only_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = '{ip_address: "127.0.0.1", path_info: "/admin/"}'
-        actual = get_client_str(username, ip_address, user_agent, path_info)
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
+        )
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_ONLY_USER_FAILURES=True)
     @override_settings(AXES_VERBOSE=True)
     def test_verbose_user_only_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info
+            username, ip_address, user_agent, path_info, self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_ONLY_USER_FAILURES=True)
     @override_settings(AXES_VERBOSE=False)
     def test_non_verbose_user_only_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = '{username: "test@example.com", path_info: "/admin/"}'
-        actual = get_client_str(username, ip_address, user_agent, path_info)
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
+        )
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=True)
     @override_settings(AXES_VERBOSE=True)
     def test_verbose_user_ip_combo_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info
+            username, ip_address, user_agent, path_info, self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=True)
     @override_settings(AXES_VERBOSE=False)
     def test_non_verbose_user_ip_combo_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = '{username: "test@example.com", ip_address: "127.0.0.1", path_info: "/admin/"}'
-        actual = get_client_str(username, ip_address, user_agent, path_info)
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
+        )
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_USE_USER_AGENT=True)
     @override_settings(AXES_VERBOSE=True)
     def test_verbose_user_agent_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = self.get_expected_client_str(
-            username, ip_address, user_agent, path_info
+            username, ip_address, user_agent, path_info, self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
         )
-        actual = get_client_str(username, ip_address, user_agent, path_info)
 
         self.assertEqual(expected, actual)
 
     @override_settings(AXES_USE_USER_AGENT=True)
     @override_settings(AXES_VERBOSE=False)
     def test_non_verbose_user_agent_client_details(self):
         username = "test@example.com"
         ip_address = "127.0.0.1"
         user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
         path_info = "/admin/"
 
         expected = '{ip_address: "127.0.0.1", user_agent: "Googlebot/2.1 (+http://www.googlebot.com/bot.html)", path_info: "/admin/"}'
-        actual = get_client_str(username, ip_address, user_agent, path_info)
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
+        )
 
         self.assertEqual(expected, actual)
 
+    @override_settings(
+        AXES_CLIENT_STR_CALLABLE="tests.test_helpers.get_dummy_client_str"
+    )
+    def test_get_client_str_callable_return_str(self):
+        self.assertEqual(
+            get_client_str(
+                "username", "ip_address", "user_agent", "path_info", self.request
+            ),
+            "client string",
+        )
+
+    @override_settings(
+        AXES_CLIENT_STR_CALLABLE="tests.test_helpers.get_dummy_client_str_using_request"
+    )
+    def test_get_client_str_callable_using_request(self):
+        self.request.user = self.user
+        self.assertEqual(
+            get_client_str(
+                "username", "ip_address", "user_agent", "path_info", self.request
+            ),
+            self.email,
+        )
+
+    @override_settings(AXES_SENSITIVE_PARAMETERS=["username"])
+    def test_get_client_str_with_sensitive_parameters(self):
+        username = "test@example.com"
+        ip_address = "127.0.0.1"
+        user_agent = "Googlebot/2.1 (+http://www.googlebot.com/bot.html)"
+        path_info = "/admin/"
+
+        expected = self.get_expected_client_str(
+            "********************",
+            ip_address,
+            user_agent,
+            path_info,
+            self.request
+        )
+        actual = get_client_str(
+            username, ip_address, user_agent, path_info, self.request
+        )
+
+        self.assertEqual(expected, actual)
+
+
+def get_dummy_client_str(username, ip_address, user_agent, path_info, request):
+    return "client string"
+
+
+def get_dummy_client_str_using_request(
+    username, ip_address, user_agent, path_info, request
+):
+    return f"{request.user.email}"
+
 
 class ClientParametersTestCase(AxesTestCase):
     @override_settings(AXES_ONLY_USER_FAILURES=True)
     def test_get_filter_kwargs_user(self):
         self.assertEqual(
             get_client_parameters(self.username, self.ip_address, self.user_agent),
             [{"username": self.username}],
@@ -268,39 +346,42 @@
         AXES_ONLY_USER_FAILURES=False,
         AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=False,
         AXES_USE_USER_AGENT=True,
     )
     def test_get_filter_kwargs_ip_and_agent(self):
         self.assertEqual(
             get_client_parameters(self.username, self.ip_address, self.user_agent),
-            [{"ip_address": self.ip_address}, {"user_agent": self.user_agent}],
+            [{"ip_address": self.ip_address, "user_agent": self.user_agent}],
         )
 
     @override_settings(
         AXES_ONLY_USER_FAILURES=False,
         AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP=True,
         AXES_USE_USER_AGENT=True,
     )
     def test_get_filter_kwargs_user_ip_agent(self):
         self.assertEqual(
             get_client_parameters(self.username, self.ip_address, self.user_agent),
             [
-                {"username": self.username, "ip_address": self.ip_address},
-                {"user_agent": self.user_agent},
+                {
+                    "username": self.username,
+                    "ip_address": self.ip_address,
+                    "user_agent": self.user_agent,
+                },
             ],
         )
 
 
 class ClientCacheKeyTestCase(AxesTestCase):
     def test_get_cache_key(self):
         """
         Test the cache key format.
         """
 
-        cache_hash_digest = md5(self.ip_address.encode()).hexdigest()
+        cache_hash_digest = sha256(self.ip_address.encode()).hexdigest()
         cache_hash_key = f"axes-{cache_hash_digest}"
 
         # Getting cache key from request
         request_factory = RequestFactory()
         request = request_factory.post(
             "/admin/login/", data={"username": self.username, "password": "test"}
         )
@@ -324,15 +405,15 @@
     def test_get_cache_key_empty_ip_address(self):
         """
         Simulate an empty IP address in the request.
         """
 
         empty_ip_address = ""
 
-        cache_hash_digest = md5(empty_ip_address.encode()).hexdigest()
+        cache_hash_digest = sha256(empty_ip_address.encode()).hexdigest()
         cache_hash_key = f"axes-{cache_hash_digest}"
 
         # Getting cache key from request
         request_factory = RequestFactory()
         request = request_factory.post(
             "/admin/login/",
             data={"username": self.username, "password": "test"},
@@ -357,15 +438,15 @@
 
     def test_get_cache_key_credentials(self):
         """
         Test the cache key format.
         """
 
         ip_address = self.ip_address
-        cache_hash_digest = md5(ip_address.encode()).hexdigest()
+        cache_hash_digest = sha256(ip_address.encode()).hexdigest()
         cache_hash_key = f"axes-{cache_hash_digest}"
 
         # Getting cache key from request
         request_factory = RequestFactory()
         request = request_factory.post(
             "/admin/login/", data={"username": self.username, "password": "test"}
         )
@@ -484,23 +565,60 @@
             get_client_username(HttpRequest(), {})
 
     @override_settings(AXES_USERNAME_CALLABLE=True)
     def test_get_client_username_not_callable(self):
         with self.assertRaises(TypeError):
             get_client_username(HttpRequest(), {})
 
-    @override_settings(AXES_USERNAME_CALLABLE="axes.tests.test_utils.get_username")
+    @override_settings(AXES_USERNAME_CALLABLE="tests.test_helpers.get_username")
     def test_get_client_username_str(self):
         self.assertEqual(get_client_username(HttpRequest(), {}), "username")
 
 
 def get_username(request, credentials: dict) -> str:
     return "username"
 
 
+def get_ip(request: HttpRequest) -> str:
+    return "127.0.0.1"
+
+
+class ClientIpAddressTestCase(AxesTestCase):
+    @override_settings(AXES_CLIENT_IP_CALLABLE=get_ip)
+    def test_get_client_ip_address(self):
+        self.assertEqual(get_client_ip_address(HttpRequest()), "127.0.0.1")
+
+    @override_settings(AXES_CLIENT_IP_CALLABLE="tests.test_helpers.get_ip")
+    def test_get_client_ip_address_str(self):
+        self.assertEqual(get_client_ip_address(HttpRequest()), "127.0.0.1")
+
+    @override_settings(
+        AXES_CLIENT_IP_CALLABLE=lambda request: "127.0.0.1"
+    )  # pragma: no cover
+    def test_get_client_ip_address_lambda(self):
+        self.assertEqual(get_client_ip_address(HttpRequest()), "127.0.0.1")
+
+    @override_settings(AXES_CLIENT_IP_CALLABLE=True)
+    def test_get_client_ip_address_not_callable(self):
+        with self.assertRaises(TypeError):
+            get_client_ip_address(HttpRequest())
+
+    @override_settings(AXES_CLIENT_IP_CALLABLE=lambda: None)  # pragma: no cover
+    def test_get_client_ip_address_invalid_callable_too_few_arguments(self):
+        with self.assertRaises(TypeError):
+            get_client_ip_address(HttpRequest())
+
+    @override_settings(
+        AXES_CLIENT_IP_CALLABLE=lambda request, extra: None
+    )  # pragma: no cover
+    def test_get_client_ip_address_invalid_callable_too_many_arguments(self):
+        with self.assertRaises(TypeError):
+            get_client_ip_address(HttpRequest())
+
+
 class IPWhitelistTestCase(AxesTestCase):
     def setUp(self):
         self.request = HttpRequest()
         self.request.method = "POST"
         self.request.META["REMOTE_ADDR"] = "127.0.0.1"
         self.request.axes_ip_address = "127.0.0.1"
 
@@ -594,7 +712,142 @@
         self.request.META["HTTP_X_REQUESTED_WITH"] = "XMLHttpRequest"
         response = get_lockout_response(request=self.request)
         self.assertEqual(type(response), JsonResponse)
 
     def test_get_lockout_response_lockout_response(self):
         response = get_lockout_response(request=self.request)
         self.assertEqual(type(response), HttpResponse)
+
+
+def mock_get_cool_off_str():
+    return timedelta(seconds=30)
+
+
+class AxesCoolOffTestCase(AxesTestCase):
+    @override_settings(AXES_COOLOFF_TIME=None)
+    def test_get_cool_off_none(self):
+        self.assertIsNone(get_cool_off())
+
+    @override_settings(AXES_COOLOFF_TIME=2)
+    def test_get_cool_off_int(self):
+        self.assertEqual(get_cool_off(), timedelta(hours=2))
+
+    @override_settings(AXES_COOLOFF_TIME=2.0)
+    def test_get_cool_off_int(self):
+        self.assertEqual(get_cool_off(), timedelta(minutes=120))
+
+    @override_settings(AXES_COOLOFF_TIME=0.25)
+    def test_get_cool_off_int(self):
+        self.assertEqual(get_cool_off(), timedelta(minutes=15))
+
+    @override_settings(AXES_COOLOFF_TIME=1.7)
+    def test_get_cool_off_int(self):
+        self.assertEqual(get_cool_off(), timedelta(seconds=6120))
+
+    @override_settings(AXES_COOLOFF_TIME=lambda: timedelta(seconds=30))
+    def test_get_cool_off_callable(self):
+        self.assertEqual(get_cool_off(), timedelta(seconds=30))
+
+    @override_settings(AXES_COOLOFF_TIME="tests.test_helpers.mock_get_cool_off_str")
+    def test_get_cool_off_path(self):
+        self.assertEqual(get_cool_off(), timedelta(seconds=30))
+
+
+def mock_is_whitelisted(request, credentials):
+    return True
+
+
+class AxesWhitelistTestCase(AxesTestCase):
+    def setUp(self):
+        self.user_model = get_user_model()
+        self.user = self.user_model.objects.create(username="jane.doe")
+        self.request = HttpRequest()
+        self.credentials = dict()
+
+    def test_is_whitelisted(self):
+        self.assertFalse(is_user_attempt_whitelisted(self.request, self.credentials))
+
+    @override_settings(AXES_WHITELIST_CALLABLE=mock_is_whitelisted)
+    def test_is_whitelisted_override_callable(self):
+        self.assertTrue(is_user_attempt_whitelisted(self.request, self.credentials))
+
+    @override_settings(AXES_WHITELIST_CALLABLE="tests.test_helpers.mock_is_whitelisted")
+    def test_is_whitelisted_override_path(self):
+        self.assertTrue(is_user_attempt_whitelisted(self.request, self.credentials))
+
+    @override_settings(AXES_WHITELIST_CALLABLE=42)
+    def test_is_whitelisted_override_invalid(self):
+        with self.assertRaises(TypeError):
+            is_user_attempt_whitelisted(self.request, self.credentials)
+
+
+def mock_get_lockout_response(request, credentials):
+    return HttpResponse(status=400)
+
+
+class AxesLockoutTestCase(AxesTestCase):
+    def setUp(self):
+        self.request = HttpRequest()
+        self.credentials = dict()
+
+    def test_get_lockout_response(self):
+        response = get_lockout_response(self.request, self.credentials)
+        self.assertEqual(429, response.status_code)
+
+    @override_settings(AXES_HTTP_RESPONSE_CODE=403)
+    def test_get_lockout_response_with_custom_http_response_code(self):
+        response = get_lockout_response(self.request, self.credentials)
+        self.assertEqual(403, response.status_code)
+
+    @override_settings(AXES_LOCKOUT_CALLABLE=mock_get_lockout_response)
+    def test_get_lockout_response_override_callable(self):
+        response = get_lockout_response(self.request, self.credentials)
+        self.assertEqual(400, response.status_code)
+
+    @override_settings(
+        AXES_LOCKOUT_CALLABLE="tests.test_helpers.mock_get_lockout_response"
+    )
+    def test_get_lockout_response_override_path(self):
+        response = get_lockout_response(self.request, self.credentials)
+        self.assertEqual(400, response.status_code)
+
+    @override_settings(AXES_LOCKOUT_CALLABLE=42)
+    def test_get_lockout_response_override_invalid(self):
+        with self.assertRaises(TypeError):
+            get_lockout_response(self.request, self.credentials)
+
+
+class AxesCleanseParamsTestCase(AxesTestCase):
+    def setUp(self):
+        self.parameters = {
+            "username": "test_user",
+            "password": "test_password",
+            "other_sensitive_data": "sensitive",
+        }
+
+    def test_cleanse_parameters(self):
+        cleansed = cleanse_parameters(self.parameters)
+        self.assertEqual("test_user", cleansed["username"])
+        self.assertEqual("********************", cleansed["password"])
+        self.assertEqual("sensitive", cleansed["other_sensitive_data"])
+
+    @override_settings(AXES_SENSITIVE_PARAMETERS=["other_sensitive_data"])
+    def test_cleanse_parameters_override_sensitive(self):
+        cleansed = cleanse_parameters(self.parameters)
+        self.assertEqual("test_user", cleansed["username"])
+        self.assertEqual("********************", cleansed["password"])
+        self.assertEqual("********************", cleansed["other_sensitive_data"])
+
+    @override_settings(AXES_SENSITIVE_PARAMETERS=["other_sensitive_data"])
+    @override_settings(AXES_PASSWORD_FORM_FIELD="username")
+    def test_cleanse_parameters_override_both(self):
+        cleansed = cleanse_parameters(self.parameters)
+        self.assertEqual("********************", cleansed["username"])
+        self.assertEqual("********************", cleansed["password"])
+        self.assertEqual("********************", cleansed["other_sensitive_data"])
+
+    @override_settings(AXES_PASSWORD_FORM_FIELD=None)
+    def test_cleanse_parameters_override_empty(self):
+        cleansed = cleanse_parameters(self.parameters)
+        self.assertEqual("test_user", cleansed["username"])
+        self.assertEqual("********************", cleansed["password"])
+        self.assertEqual("sensitive", cleansed["other_sensitive_data"])
```

### Comparing `django-axes-5.9.1/axes/utils.py` & `django-axes-6.0.0b1/axes/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from axes.conf import settings
 from axes.handlers.proxy import AxesProxyHandler
 from axes.helpers import get_client_ip_address
 
 log = getLogger(__name__)
 
 
-def reset(ip: str = None, username: str = None, ip_or_username=False) -> int:
+def reset(
+    ip: Optional[str] = None, username: Optional[str] = None, ip_or_username=False
+) -> int:
     """
     Reset records that match IP or username, and return the count of removed attempts.
 
     This utility method is meant to be used from the CLI or via Python API.
     """
 
     return AxesProxyHandler.reset_attempts(
```

### Comparing `django-axes-5.9.1/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.0b1/django_axes.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-.coveragerc
 .gitignore
+.pre-commit-config.yaml
 .prospector.yaml
 CHANGES.rst
+CODE_OF_CONDUCT.md
 LICENSE
-MANIFEST.in
 README.rst
 codecov.yml
 manage.py
 mypy.ini
 pyproject.toml
-pytest.ini
 requirements-qa.txt
 requirements-test.txt
 requirements.txt
 setup.py
-tox.ini
+.github/dependabot.yml
+.github/workflows/codeql.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 axes/__init__.py
 axes/admin.py
 axes/apps.py
 axes/attempts.py
 axes/backends.py
@@ -34,54 +34,41 @@
 axes/handlers/__init__.py
 axes/handlers/base.py
 axes/handlers/cache.py
 axes/handlers/database.py
 axes/handlers/dummy.py
 axes/handlers/proxy.py
 axes/handlers/test.py
+axes/locale/ar/LC_MESSAGES/django.mo
+axes/locale/ar/LC_MESSAGES/django.po
 axes/locale/de/LC_MESSAGES/django.mo
 axes/locale/de/LC_MESSAGES/django.po
+axes/locale/pl/LC_MESSAGES/django.mo
+axes/locale/pl/LC_MESSAGES/django.po
 axes/locale/ru/LC_MESSAGES/django.mo
 axes/locale/ru/LC_MESSAGES/django.po
 axes/locale/tr/LC_MESSAGES/django.mo
 axes/locale/tr/LC_MESSAGES/django.po
 axes/management/__init__.py
 axes/management/commands/__init__.py
 axes/management/commands/axes_list_attempts.py
 axes/management/commands/axes_reset.py
+axes/management/commands/axes_reset_failure_logs.py
 axes/management/commands/axes_reset_ip.py
 axes/management/commands/axes_reset_logs.py
-axes/management/commands/axes_reset_user.py
 axes/management/commands/axes_reset_username.py
 axes/migrations/0001_initial.py
 axes/migrations/0002_auto_20151217_2044.py
 axes/migrations/0003_auto_20160322_0929.py
 axes/migrations/0004_auto_20181024_1538.py
 axes/migrations/0005_remove_accessattempt_trusted.py
 axes/migrations/0006_remove_accesslog_trusted.py
+axes/migrations/0007_alter_accessattempt_unique_together.py
+axes/migrations/0008_accessfailurelog.py
 axes/migrations/__init__.py
-axes/tests/__init__.py
-axes/tests/base.py
-axes/tests/settings.py
-axes/tests/test_admin.py
-axes/tests/test_attempts.py
-axes/tests/test_backends.py
-axes/tests/test_checks.py
-axes/tests/test_decorators.py
-axes/tests/test_handlers.py
-axes/tests/test_helpers.py
-axes/tests/test_logging.py
-axes/tests/test_login.py
-axes/tests/test_management.py
-axes/tests/test_middleware.py
-axes/tests/test_models.py
-axes/tests/test_signals.py
-axes/tests/test_utils.py
-axes/tests/urls.py
-axes/tests/urls_empty.py
 django_axes.egg-info/PKG-INFO
 django_axes.egg-info/SOURCES.txt
 django_axes.egg-info/dependency_links.txt
 django_axes.egg-info/not-zip-safe
 django_axes.egg-info/requires.txt
 django_axes.egg-info/top_level.txt
 docs/10_changelog.rst
@@ -93,8 +80,27 @@
 docs/6_integration.rst
 docs/7_architecture.rst
 docs/8_reference.rst
 docs/9_development.rst
 docs/Makefile
 docs/conf.py
 docs/index.rst
-docs/images/flow.png
+docs/images/flow.png
+tests/__init__.py
+tests/base.py
+tests/settings.py
+tests/test_admin.py
+tests/test_attempts.py
+tests/test_backends.py
+tests/test_checks.py
+tests/test_decorators.py
+tests/test_failures.py
+tests/test_handlers.py
+tests/test_helpers.py
+tests/test_logging.py
+tests/test_login.py
+tests/test_management.py
+tests/test_middleware.py
+tests/test_models.py
+tests/test_signals.py
+tests/urls.py
+tests/urls_empty.py
```

### Comparing `django-axes-5.9.1/docs/1_requirements.rst` & `django-axes-6.0.0b1/docs/1_requirements.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .. _requirements:
 
 Requirements
 ============
 
-Axes requires a supported Django version and runs on Python versions 3.6 and above.
+Axes requires a supported Django version and runs on Python versions 3.7 and above.
 
 Refer to the project source code repository in
 `GitHub <https://github.com/jazzband/django-axes/>`_ and see the
-`Tox configuration <https://github.com/jazzband/django-axes/blob/master/tox.ini>`_ and
+`pyproject.toml file <https://github.com/jazzband/django-axes/blob/master/pyproject.toml>`_ and
 `Python package definition <https://github.com/jazzband/django-axes/blob/master/setup.py>`_
 to check if your Django and Python version are supported.
 
 The `GitHub Actions builds <https://github.com/jazzband/django-axes/actions>`_
 test Axes compatibility with the Django master branch for future compatibility as well.
```

### Comparing `django-axes-5.9.1/docs/2_installation.rst` & `django-axes-6.0.0b1/docs/2_installation.rst`

 * *Files 19% similar despite different names*

```diff
@@ -19,24 +19,29 @@
         'django.contrib.messages',
         'django.contrib.staticfiles',
 
         # Axes app can be in any position in the INSTALLED_APPS list.
         'axes',
     ]
 
-**2.** Add ``axes.backends.AxesBackend`` to the top of ``AUTHENTICATION_BACKENDS``::
+**2.** Add ``axes.backends.AxesStandaloneBackend`` to the top of ``AUTHENTICATION_BACKENDS``::
 
     AUTHENTICATION_BACKENDS = [
-        # AxesBackend should be the first backend in the AUTHENTICATION_BACKENDS list.
-        'axes.backends.AxesBackend',
+        # AxesStandaloneBackend should be the first backend in the AUTHENTICATION_BACKENDS list.
+        'axes.backends.AxesStandaloneBackend',
 
         # Django ModelBackend is the default authentication backend.
         'django.contrib.auth.backends.ModelBackend',
     ]
 
+    For backwards compatibility, ``AxesBackend`` can be used in place of ``AxesStandaloneBackend``. 
+    The only difference is that ``AxesBackend`` also provides the permissions-checking functionality
+    of Django's ``ModelBackend`` behind the scenes. We recommend using ``AxesStandaloneBackend``
+    if you have any custom logic to override Django's standard permissions checks. 
+
 **3.** Add ``axes.middleware.AxesMiddleware`` to your list of ``MIDDLEWARE``::
 
     MIDDLEWARE = [
         # The following is the list of default middleware in new Django projects.
         'django.middleware.security.SecurityMiddleware',
         'django.contrib.sessions.middleware.SessionMiddleware',
         'django.middleware.common.CommonMiddleware',
@@ -69,15 +74,15 @@
 and running the application with misconfigured settings can prevent security features from working.
 
 
 Disabling Axes system checks
 ----------------------------
 
 If you are implementing custom authentication, request middleware, or signal handlers
-the Axes checks system might false positives in the Django checks framework.
+the Axes checks system might generate false positives in the Django checks framework.
 
 You can silence the unnecessary warnings by using the following Django settings::
 
    SILENCED_SYSTEM_CHECKS = ['axes.W003']
 
 
 Axes has the following warnings codes built in:
```

### Comparing `django-axes-5.9.1/docs/3_usage.rst` & `django-axes-6.0.0b1/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/docs/5_customization.rst` & `django-axes-6.0.0b1/docs/5_customization.rst`

 * *Files 20% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 Customizing authentication views
 --------------------------------
 
 Here is a more detailed example of sending the necessary signals using
 and a custom auth backend at an endpoint that expects JSON
 requests. The custom authentication can be swapped out with ``authenticate``
 and ``login`` from ``django.contrib.auth``, but beware that those methods take
-care of sending the nessary signals for you, and there is no need to duplicate
+care of sending the necessary signals for you, and there is no need to duplicate
 them as per the example.
 
 ``example/forms.py``::
 
     from django import forms
 
     class LoginForm(forms.Form):
@@ -150,7 +150,41 @@
     AXES_USERNAME_CALLABLE = 'example.utils.get_username'
 
 .. note::
    You still have to make these modifications yourself before calling
    authenticate. If you want to re-use the same function for consistency, that's
    fine, but Axes does not inject these changes into the authentication flow
    for you.
+
+
+Customizing lockout responses
+-----------------------------
+
+Axes can be configured with ``AXES_LOCKOUT_CALLABLE`` to return a custom lockout response when using the plugin with e.g. DRF (Django REST Framework) or other third party libraries which require specialized formats such as JSON or XML response formats or customized response status codes.
+
+An example of usage could be e.g. a custom view for processing lockouts.
+
+``example/views.py``::
+
+    from django.http import JsonResponse
+
+    def lockout(request, credentials, *args, **kwargs):
+        return JsonResponse({"status": "Locked out due to too many login failures"}, status=403)
+
+``settings.py``::
+
+    AXES_LOCKOUT_CALLABLE = "example.views.lockout"
+
+
+Customizing client ip address lookups
+-----------------------------
+
+Axes can be configured with ``AXES_CLIENT_IP_CALLABLE`` to use custom client ip address lookup logic.
+
+``example/utils.py``::
+
+    def get_client_ip(request):
+        return request.META.get("REMOTE_ADDR")
+
+``settings.py``::
+
+    AXES_LOCKOUT_CALLABLE = "example.utils.get_client_ip"
```

### Comparing `django-axes-5.9.1/docs/6_integration.rst` & `django-axes-6.0.0b1/docs/6_integration.rst`

 * *Files 6% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 Axes is intended to be pluggable and usable with custom authentication solutions.
 This document describes the integration with some popular 3rd party packages
 such as Django Allauth, Django REST Framework, and other tools.
 
 In the following table
 **Compatible** means that a component should be fully compatible out-of-the-box,
-**Functional** means that a component should be functional after customization, and
+**Functional** means that a component should be functional after configuration, and
 **Incompatible** means that a component has been reported as non-functional with Axes.
 
 =======================   =============   ============   ============   ==============
 Project                   Version         Compatible     Functional     Incompatible
 =======================   =============   ============   ============   ==============
-Django REST Framework     |gte| 3.7.0     |check|
-Django REST Framework     |lt| 3.7.0                     |check|
+Django REST Framework                                    |check|
 Django Allauth                                           |check|
 Django Simple Captcha                                    |check|
 Django OAuth Toolkit                                     |check|
 Django Reversion                                         |check|
+Django Auth LDAP                          |check|               
 =======================   =============   ============   ============   ==============
 
 .. |check|  unicode:: U+2713
 .. |lt|     unicode:: U+003C
 .. |lte|    unicode:: U+2264
 .. |gte|    unicode:: U+2265
 .. |gt|     unicode:: U+003E
@@ -95,54 +95,55 @@
         path('accounts/', include('allauth.urls')),
     ]
 
 
 Integration with Django REST Framework
 --------------------------------------
 
-.. note::
-   Modern versions of Django REST Framework after 3.7.0 work normally with Axes
-   out-of-the-box and require no customization in DRF.
+.. warning::
+   The following guide only covers authentication schemes that rely on
+   Django's ``authenticate()`` function. Other schemes (e.g.
+   ``TokenAuthentication``) are currently not supported.
 
+Django Axes requires REST Framework to be connected
+via lockout signals for correct functionality.
 
-Django REST Framework versions prior to 3.7.0
-require the request object to be passed for authentication
-by a customized DRF authentication class::
+You can use the following snippet in your project signals such as ``example/signals.py``::
 
-    from rest_framework.authentication import BasicAuthentication
+    from django.dispatch import receiver
 
-    class AxesBasicAuthentication(BasicAuthentication):
-        """
-        Extended basic authentication backend class that supplies the
-        request object into the authentication call for Axes compatibility.
+    from axes.signals import user_locked_out
+    from rest_framework.exceptions import PermissionDenied
 
-        NOTE: This patch is only needed for DRF versions < 3.7.0.
-        """
 
-        def authenticate(self, request):
-            # NOTE: Request is added as an instance attribute in here
-            self._current_request = request
-            return super().authenticate(request)
-
-        def authenticate_credentials(self, userid, password, request=None):
-            credentials = {
-                get_user_model().USERNAME_FIELD: userid,
-                'password': password
-            }
-
-            # NOTE: Request is added as an argument to the authenticate call here
-            user = authenticate(request=request or self._current_request, **credentials)
+    @receiver(user_locked_out)
+    def raise_permission_denied(*args, **kwargs):
+        raise PermissionDenied("Too many failed login attempts")
+
+And then configure your application to load it in ``examples/apps.py``::
+
+    from django import apps
+
+
+    class AppConfig(apps.AppConfig):
+        name = "example"
+
+        def ready(self):
+            from example import signals  # noqa
+
+Please check the Django signals documentation for more information:
 
-            if user is None:
-                raise exceptions.AuthenticationFailed(_('Invalid username/password.'))
+https://docs.djangoproject.com/en/3.2/topics/signals/
 
-            if not user.is_active:
-                raise exceptions.AuthenticationFailed(_('User inactive or deleted.'))
+When a user login fails a signal is emitted and PermissionDenied
+raises a HTTP 403 reply which interrupts the login process.
 
-            return (user, None)
+This functionality was handled in the middleware for a time,
+but that resulted in extra database requests being made for
+each and every web request, and was migrated to signals.
 
 
 Integration with Django Simple Captcha
 --------------------------------------
 
 Axes supports Captcha with the Django Simple Captcha package in the following manner.
```

### Comparing `django-axes-5.9.1/docs/7_architecture.rst` & `django-axes-6.0.0b1/docs/7_architecture.rst`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 Axes implements authentication blocking with the custom
 ``AxesBackend`` authentication backend which checks every request
 coming through the Django authentication flow and verifies they
 are not blocked, and allows the requests to go through if the check passes.
 
 If the authentication attempt matches a lockout rule, e.g. it is from a
 blacklisted IP or exceeds the maximum configured authentication attempts,
-it is blocked by raising the ``PermissionDenied`` excepton in the backend.
+it is blocked by raising the ``PermissionDenied`` exception in the backend.
 
 Axes monitors logins with the ``user_login_failed`` signal receiver
 and records authentication failures from both the ``AxesBackend`` and
 other authentication backends and tracks the failed attempts
 by tracking the attempt IP address, username, user agent, or all of them.
 
 If the lockout rules match, then Axes marks the request
```

### Comparing `django-axes-5.9.1/docs/9_development.rst` & `django-axes-6.0.0b1/docs/9_development.rst`

 * *Files 2% similar despite different names*

```diff
@@ -37,10 +37,10 @@
 
     $ tox
 
 Tox runs the same test set that is run by GitHub Actions, and your code should be good to go if it passes.
 
 If you wish to limit the testing to specific environment(s), you can parametrize the tox run::
 
-    $ tox -e py37-django21
+    $ tox -e py39-django32
 
 After you have pushed your changes, open a pull request on GitHub for getting your code upstreamed.
```

### Comparing `django-axes-5.9.1/docs/Makefile` & `django-axes-6.0.0b1/docs/Makefile`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 SPHINXOPTS    =
 SPHINXBUILD   = sphinx-build
 PAPER         =
 BUILDDIR      = _build
 
 # User-friendly check for sphinx-build
 ifeq ($(shell which $(SPHINXBUILD) >/dev/null 2>&1; echo $$?), 1)
-$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from http://sphinx-doc.org/)
+$(error The '$(SPHINXBUILD)' command was not found. Make sure you have Sphinx installed, then set the SPHINXBUILD environment variable to point to the full path of the '$(SPHINXBUILD)' executable. Alternatively you can add the directory with the executable to your PATH. If you don't have Sphinx installed, grab it from https://sphinx-doc.org/)
 endif
 
 # Internal variables.
 PAPEROPT_a4     = -D latex_paper_size=a4
 PAPEROPT_letter = -D latex_paper_size=letter
 ALLSPHINXOPTS   = -d $(BUILDDIR)/doctrees $(PAPEROPT_$(PAPER)) $(SPHINXOPTS) .
 # the i18n builder cannot share the environment and doctrees with the others
```

### Comparing `django-axes-5.9.1/docs/conf.py` & `django-axes-6.0.0b1/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Sphinx documentation generator configuration.
 
 More information on the configuration options is available at:
 
-    http://www.sphinx-doc.org/en/master/usage/configuration.html
+    https://www.sphinx-doc.org/en/master/usage/configuration.html
 """
 
-from os import environ
+import sphinx_rtd_theme
 from pkg_resources import get_distribution
 
 import django
-import sphinx_rtd_theme
+from django.conf import settings
 
-environ.setdefault("DJANGO_SETTINGS_MODULE", "axes.tests.settings")
+settings.configure(INSTALLED_APPS=["django", "django.contrib.auth", "axes"], DEBUG=True)
 django.setup()
 
+
 # -- Extra custom configuration  ------------------------------------------
 
 title = "django-axes documentation"
 description = ("Keep track of failed login attempts in Django-powered sites.",)
 
 # -- General configuration ------------------------------------------------
```

### Comparing `django-axes-5.9.1/docs/images/flow.png` & `django-axes-6.0.0b1/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-5.9.1/setup.py` & `django-axes-6.0.0b1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,36 +31,37 @@
         "Source": "https://github.com/jazzband/django-axes",
         "Tracker": "https://github.com/jazzband/django-axes/issues",
     },
     license="MIT",
     package_dir={"axes": "axes"},
     use_scm_version=True,
     setup_requires=["setuptools_scm"],
-    python_requires="~=3.6",
-    install_requires=["django>=2.0", "django-ipware>=3,<4"],
+    python_requires=">=3.7",
+    install_requires=["django>=3.2", "django-ipware>=3", "setuptools"],
     include_package_data=True,
-    packages=find_packages(),
+    packages=find_packages(exclude=["tests"]),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Environment :: Plugins",
         "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
+        "Framework :: Django :: 3.2",
+        "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Internet :: Log Analysis",
         "Topic :: Security",
         "Topic :: System :: Logging",
     ],
     zip_safe=False,
```

