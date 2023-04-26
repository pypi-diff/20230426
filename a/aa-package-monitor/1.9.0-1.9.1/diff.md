# Comparing `tmp/aa_package_monitor-1.9.0.tar.gz` & `tmp/aa_package_monitor-1.9.1.tar.gz`

## Comparing `aa_package_monitor-1.9.0.tar` & `aa_package_monitor-1.9.1.tar`

### file list

```diff
@@ -1,58 +1,64 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/app_settings.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/apps.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/auth_hooks.py
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/core.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/managers.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/models.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tasks.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/urls.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/views.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/django.pot
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/management/commands/package_monitor_refresh.py
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0001_initial.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/0003_add_update_notifications.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/migrations/__init__.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/global.css
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/package_list.css
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/templates/package_monitor/base.html
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/templates/package_monitor/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_commands.py
--rw-r--r--   0        0        0    15922 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_core.py
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_integration.py
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_managers.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_models.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_tasks.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/test_views.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/__init__.py
--rw-r--r--   0        0        0     4116 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/factories.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/stubs.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/package_monitor/tests/factories/tests.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/LICENSE
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/README.md
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/pyproject.toml
--rw-r--r--   0        0        0    10220 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/app_settings.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/apps.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/auth_hooks.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/managers.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/models.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tasks.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/urls.py
+-rw-r--r--   0        0        0     5091 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/__init__.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/distribution_packages.py
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/metadata_helpers.py
+-rw-r--r--   0        0        0     5159 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/core/pypi.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/django.pot
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/management/commands/package_monitor_refresh.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/0003_add_update_notifications.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/migrations/__init__.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/global.css
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/package_list.css
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/base.html
+-rw-r--r--   0        0        0    10198 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_commands.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_integration.py
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_managers.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_models.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_tasks.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/__init__.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_distribution_packages.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_metadata_helpers.py
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/core/test_pypi.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/__init__.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/factories.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/stubs.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/package_monitor/tests/factories/tests.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/LICENSE
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/README.md
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10223 2020-02-02 00:00:00.000000 aa_package_monitor-1.9.1/PKG-INFO
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/app_settings.py` & `aa_package_monitor-1.9.1/package_monitor/app_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from app_utils.django import clean_setting
+from app_utils.app_settings import clean_setting
 
 PACKAGE_MONITOR_EXCLUDE_PACKAGES = clean_setting(
     "PACKAGE_MONITOR_EXCLUDE_PACKAGES", default_value=[]
 )
 """Names of distribution packages to be excluded."""
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/auth_hooks.py` & `aa_package_monitor-1.9.1/package_monitor/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/managers.py` & `aa_package_monitor-1.9.1/package_monitor/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from .app_settings import (
     PACKAGE_MONITOR_EXCLUDE_PACKAGES,
     PACKAGE_MONITOR_INCLUDE_PACKAGES,
     PACKAGE_MONITOR_NOTIFICATIONS_ENABLED,
     PACKAGE_MONITOR_SHOW_ALL_PACKAGES,
     PACKAGE_MONITOR_SHOW_EDITABLE_PACKAGES,
 )
-from .core import (
+from .core.distribution_packages import (
     DistributionPackage,
     compile_package_requirements,
     gather_distribution_packages,
-    update_packages_from_pypi,
 )
+from .core.pypi import update_packages_from_pypi
 
 TERMINAL_MAX_LINE_LENGTH = 4095
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class DistributionQuerySet(models.QuerySet):
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/models.py` & `aa_package_monitor-1.9.1/package_monitor/models.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/views.py` & `aa_package_monitor-1.9.1/package_monitor/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import render
 from django.utils.html import format_html
 from django.utils.translation import gettext_lazy as _
 
-from app_utils.views import link_html, yesno_str
+from app_utils.views import link_html, yesnonone_str
 
 from . import __title__
 from .app_settings import (
     PACKAGE_MONITOR_INCLUDE_PACKAGES,
     PACKAGE_MONITOR_SHOW_ALL_PACKAGES,
 )
 from .models import Distribution
@@ -120,15 +120,15 @@
                 "name": dist.name,
                 "name_link": name_link_html,
                 "apps": apps_html,
                 "used_by": used_by_html,
                 "current": dist.installed_version,
                 "latest": latest_html,
                 "is_outdated": dist.is_outdated,
-                "is_outdated_str": yesno_str(dist.is_outdated),
+                "is_outdated_str": yesnonone_str(dist.is_outdated),
                 "description": description,
             }
         )
 
     return JsonResponse(data, safe=False)
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/django.pot` & `aa_package_monitor-1.9.1/package_monitor/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/de/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/en/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/en/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/es/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/fr_FR/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/it_IT/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/ja/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/ko_KR/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.mo` & `aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/ru/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,26 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.mo` & `aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/uk/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/uk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n % 10 == 1 && n % 100 != "
 "11 ? 0 : n % 1 == 0 && n % 10 >= 2 && n % 10 <= 4 && (n % 100 < 12 || n % "
 "100 > 14) ? 1 : n % 1 == 0 && (n % 10 ==0 || (n % 10 >=5 && n % 10 <=9) || "
 "(n % 100 >=11 && n % 100 <=14 )) ? 2: 3);\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_package_monitor-1.9.1/package_monitor/locale/ru/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-22 21:18+0200\n"
+"POT-Creation-Date: 2023-04-23 21:44+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
+"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
+"(n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: templates/package_monitor/index.html:9
-msgid "never"
+msgid "not yet"
 msgstr ""
 
 #: templates/package_monitor/index.html:10
 msgid "Last updated"
 msgstr ""
 
 #: templates/package_monitor/index.html:16
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/management/commands/package_monitor_refresh.py` & `aa_package_monitor-1.9.1/package_monitor/management/commands/package_monitor_refresh.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/migrations/0001_initial.py` & `aa_package_monitor-1.9.1/package_monitor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py` & `aa_package_monitor-1.9.1/package_monitor/migrations/0002_add_editable_and_refactor_json_fields.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/migrations/0003_add_update_notifications.py` & `aa_package_monitor-1.9.1/package_monitor/migrations/0003_add_update_notifications.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/global.css` & `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/css/package_list.css` & `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/css/package_list.css`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif` & `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif` & `aa_package_monitor-1.9.1/package_monitor/static/package_monitor/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/templates/package_monitor/index.html` & `aa_package_monitor-1.9.1/package_monitor/templates/package_monitor/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load i18n %}
 {% load humanize %}
 {% load static %}
 
 {% block details %}
 
     <span class="pull-right">
-        {% translate "never" as never_text %}
+        {% translate "not yet" as never_text %}
         {% translate 'Last updated' %} {{ updated_at|naturaltime|default_if_none:never_text }}&nbsp;&nbsp;
         <button
             type="button"
             class="btn btn-success btn-tabs"
             data-toggle="modal"
             data-target="#modalRefreshingDistributions"
             title="{% translate 'Refresh data now' %}">
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/test_commands.py` & `aa_package_monitor-1.9.1/package_monitor/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/test_integration.py` & `aa_package_monitor-1.9.1/package_monitor/tests/test_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from unittest import mock
 
 import requests_mock
 
 from app_utils.testing import NoSocketsTestCase
 
 from package_monitor import tasks
-from package_monitor.core import DistributionPackage
+from package_monitor.core.distribution_packages import DistributionPackage
 from package_monitor.models import Distribution
 
-from .factories import ImportlibDistributionStubFactory, PypiFactory, PypiReleaseFactory
+from .factories import MetadataDistributionStubFactory, PypiFactory, PypiReleaseFactory
 
+CORE_PATH = "package_monitor.core.distribution_packages"
+CORE_HELPERS_PATH = "package_monitor.core.metadata_helpers"
+MANAGERS_PATH = "package_monitor.managers"
 
-@mock.patch("package_monitor.managers.PACKAGE_MONITOR_NOTIFICATIONS_ENABLED", False)
-@mock.patch("package_monitor.core.django_apps", spec=True)
-@mock.patch("package_monitor.core.importlib_metadata.distributions", spec=True)
+
+@mock.patch(MANAGERS_PATH + ".PACKAGE_MONITOR_NOTIFICATIONS_ENABLED", False)
+@mock.patch(CORE_HELPERS_PATH + ".django_apps", spec=True)
+@mock.patch(CORE_PATH + ".importlib_metadata.distributions", spec=True)
 @requests_mock.Mocker()
 class TestUpdatePackagesFromPyPi(NoSocketsTestCase):
     def test_should_update_packages(
         self, mock_distributions, mock_django_apps, requests_mocker
     ):
         # given
-        dist_alpha = ImportlibDistributionStubFactory(name="alpha", version="1.0.0")
+        dist_alpha = MetadataDistributionStubFactory(name="alpha", version="1.0.0")
         distributions = lambda: iter([dist_alpha])  # noqa: E731
         mock_distributions.side_effect = distributions
         mock_django_apps.get_app_configs.return_value = []
         pypi_alpha = PypiFactory(
-            distribution=DistributionPackage.create_from_distribution(dist_alpha)
+            distribution=DistributionPackage.create_from_metadata_distribution(
+                dist_alpha
+            )
         )
         pypi_alpha.releases["1.1.0"] = [PypiReleaseFactory()]
         requests_mocker.register_uri(
             "GET", "https://pypi.org/pypi/alpha/json", json=pypi_alpha.asdict()
         )
         # when
         tasks.update_distributions()
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/test_managers.py` & `aa_package_monitor-1.9.1/package_monitor/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/test_models.py` & `aa_package_monitor-1.9.1/package_monitor/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/test_views.py` & `aa_package_monitor-1.9.1/package_monitor/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/factories/factories.py` & `aa_package_monitor-1.9.1/package_monitor/tests/factories/factories.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Iterable
 
 import factory
 import factory.fuzzy
 from packaging.requirements import Requirement
 
-from package_monitor.core import DistributionPackage
+from package_monitor.core.distribution_packages import DistributionPackage
 from package_monitor.models import Distribution
 
-from .stubs import ImportlibDistributionStub, Pypi, PypiInfo, PypiRelease, PypiUrl
+from .stubs import MetadataDistributionStub, Pypi, PypiInfo, PypiRelease, PypiUrl
 
 faker = factory.faker.faker.Faker()
 
 
 class PypiReleaseFactory(factory.Factory):
     class Meta:
         model = PypiRelease
@@ -31,14 +31,16 @@
     class Meta:
         model = PypiInfo
 
     project_url = factory.LazyAttribute(lambda o: f"https://pypi.org/project/{o.name}/")
 
 
 class PypiFactory(factory.Factory):
+    """A data object on PyPI. Create from DistributionPackage"""
+
     class Meta:
         model = Pypi
         exclude = ("distribution",)
 
     info = factory.LazyAttribute(
         lambda o: PypiInfoFactory(
             name=o.distribution.name,
@@ -54,17 +56,17 @@
     requires_python = "~=3.7"
     releases = factory.LazyAttribute(
         lambda o: {o.distribution.current: [PypiReleaseFactory()]}
     )
     urls = factory.LazyAttribute(lambda o: [PypiUrlFactory()])
 
 
-class ImportlibDistributionStubFactory(factory.Factory):
+class MetadataDistributionStubFactory(factory.Factory):
     class Meta:
-        model = ImportlibDistributionStub
+        model = MetadataDistributionStub
 
     name = factory.Faker("last_name")
     # files = ["dummy_1/file_1.py", "dummy_1/__init__.py"]
     homepage_url = factory.Faker("url")
     summary = factory.Faker("sentence")
 
     @factory.lazy_attribute
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/factories/stubs.py` & `aa_package_monitor-1.9.1/package_monitor/tests/factories/stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 class PackageMetadataStub(MutableMapping):
     """A PackageMetadata stub implementing the interface
     for importlib_metadata.PackageMetadata.
 
     This is a dict-like type, which allows multiple values per key.
     """
 
-    def __init__(self, init_d: dict = None):
+    def __init__(self, init_d: Optional[dict] = None):
         self._d = defaultdict(list)
         if init_d:
             for k, v in init_d.items():
                 self[k] = v
 
     def __setitem__(self, key, value):
         self._d[key].append(value)
@@ -108,21 +108,21 @@
     def get_all(self, key) -> Optional[list]:
         v = self._d[key]
         if not v:
             return None
         return v
 
 
-class ImportlibDistributionStub:
+class MetadataDistributionStub:
     def __init__(
         self,
         name: str,
         version: str,
         files: list,
-        requires: list = None,
+        requires: Optional[list] = None,
         homepage_url: str = "",
         summary: str = "",
     ) -> None:
         self.metadata = PackageMetadataStub(
             {
                 "Name": name,
                 "Home-page": homepage_url if homepage_url != "" else "UNKNOWN",
```

### Comparing `aa_package_monitor-1.9.0/package_monitor/tests/factories/tests.py` & `aa_package_monitor-1.9.1/package_monitor/tests/factories/tests.py`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/LICENSE` & `aa_package_monitor-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/README.md` & `aa_package_monitor-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_package_monitor-1.9.0/pyproject.toml` & `aa_package_monitor-1.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dependencies = [
     "allianceauth>=3",
-    "allianceauth-app-utils>=1.8",
+    "allianceauth-app-utils>=1.17.1",
     "importlib_metadata",
     "requests",
 ]
 
 [project.urls]
 Homepage = "https://gitlab.com/ErikKalkoken/aa-package-monitor"
 Source = "https://gitlab.com/ErikKalkoken/aa-package-monitor"
```

### Comparing `aa_package_monitor-1.9.0/PKG-INFO` & `aa_package_monitor-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-package-monitor
-Version: 1.9.0
+Version: 1.9.1
 Summary: An app that helps keep track of installed packages and outstanding updates for Alliance Auth
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-package-monitor
 Project-URL: Source, https://gitlab.com/ErikKalkoken/aa-package-monitor
 Project-URL: Changelog, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/blob/master/CHANGELOG.md
 Project-URL: Tracker, https://gitlab.com/ErikKalkoken/aa-package-monitor/-/issues
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 License-Expression: MIT
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-Requires-Dist: allianceauth-app-utils>=1.8
+Requires-Dist: allianceauth-app-utils>=1.17.1
 Requires-Dist: allianceauth>=3
 Requires-Dist: importlib-metadata
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # Package Monitor
```

