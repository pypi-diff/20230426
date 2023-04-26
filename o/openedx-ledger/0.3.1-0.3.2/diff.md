# Comparing `tmp/openedx-ledger-0.3.1.tar.gz` & `tmp/openedx-ledger-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openedx-ledger-0.3.1.tar", last modified: Fri Apr  7 18:21:56 2023, max compression
+gzip compressed data, was "openedx-ledger-0.3.2.tar", last modified: Wed Apr 26 20:38:40 2023, max compression
```

## Comparing `openedx-ledger-0.3.1.tar` & `openedx-ledger-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2696 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5185 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
--rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
--rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py
--rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/0006_auto_20230404_1744.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15474 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/base.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/openedx_ledger/test_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/test_utils/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)      329 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/openedx_ledger/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.214021 openedx-ledger-0.3.1/openedx_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1131 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-07 18:21:56.000000 openedx-ledger-0.3.1/openedx_ledger.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 18:21:56.218021 openedx-ledger-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-04-07 18:21:53.000000 openedx-ledger-0.3.1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5962 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3884 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5326 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      220 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12708 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4291 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/0006_auto_20230404_1744.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15474 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/signals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/signals/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.230926 openedx-ledger-0.3.2/openedx_ledger/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      831 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/base.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/openedx_ledger/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2301 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/test_utils/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/openedx_ledger/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.238926 openedx-ledger-0.3.2/openedx_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8415 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1267 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-26 20:38:40.000000 openedx-ledger-0.3.2/openedx_ledger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      304 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5100 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 20:38:40.242926 openedx-ledger-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2209 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4515 2023-04-26 20:38:35.000000 openedx-ledger-0.3.2/tests/test_models.py
```

### Comparing `openedx-ledger-0.3.1/CHANGELOG.rst` & `openedx-ledger-0.3.2/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-Nothing
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+  
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.1/LICENSE.txt` & `openedx-ledger-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/PKG-INFO` & `openedx-ledger-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.1
+Version: 0.3.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,16 +204,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-Nothing
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+  
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.1/README.rst` & `openedx-ledger-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/admin.py` & `openedx-ledger-0.3.2/openedx_ledger/admin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Admin configuration for openedx_ledger models.
 """
 from django.conf import settings
 from django.contrib import admin
+from django.http import HttpResponseRedirect
+from django.urls import re_path, reverse
+from django_object_actions import DjangoObjectActions
 from simple_history.admin import SimpleHistoryAdmin
 
-from openedx_ledger import models
+from openedx_ledger import models, views
 
 
 def can_modify():
     getattr(settings, 'ALLOW_LEDGER_MODIFICATION', False)
 
 
 @admin.register(models.Ledger)
@@ -61,15 +64,15 @@
     """
     Inline admin configuration for the ExternalTransactionReference model.
     """
     model = models.ExternalTransactionReference
 
 
 @admin.register(models.Transaction)
-class TransactionAdmin(SimpleHistoryAdmin):
+class TransactionAdmin(DjangoObjectActions, SimpleHistoryAdmin):
     """
     Admin configuration for the Transaction model.
     """
 
     class Meta:
         """
         Metaclass for TransactionAdmin.
@@ -86,14 +89,42 @@
             'created',
             'modified',
         )
     else:
         readonly_fields = _all_fields
     inlines = [ExternalTransactionReferenceInlineAdmin]
 
+    change_actions = ('reverse_transaction',)
+
+    def reverse_transaction(self, request, obj):
+        """
+        Redirect to the reverse transaction view.
+        """
+        # url names coming from get_urls are prefixed with 'admin' namespace
+        reverse_transaction_url = reverse("admin:reverse_transaction", args=(obj.uuid,))
+        return HttpResponseRedirect(reverse_transaction_url)
+
+    reverse_transaction.label = "Unenroll & Refund"
+    reverse_transaction.short_description = (
+        "Reverse a transaction and unenroll the learner from the platform representation of the course."
+    )
+
+    def get_urls(self):
+        """
+        Returns the additional urls used by DjangoObjectActions.
+        """
+        customer_urls = [
+            re_path(
+                r"^([^/]+)/reverse_transaction$",
+                self.admin_site.admin_view(views.ReverseTransactionView.as_view()),
+                name="reverse_transaction"
+            )
+        ]
+        return customer_urls + super().get_urls()
+
 
 @admin.register(models.Reversal)
 class ReversalAdmin(SimpleHistoryAdmin):
     """
     Admin configuration for the Reversal model.
     """
```

### Comparing `openedx-ledger-0.3.1/openedx_ledger/api.py` & `openedx-ledger-0.3.2/openedx_ledger/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The openedx_ledger python API.
 """
 from django.db.transaction import atomic, get_connection
 
 from openedx_ledger import models, utils
+from openedx_ledger.signals.signals import TRANSACTION_REVERSED
 
 
 class LedgerBalanceExceeded(Exception):
     """
     Exception for when a transaction could not be created because it would exceed the ledger balance.
     """
 
@@ -89,14 +90,15 @@
             transaction=transaction,
             idempotency_key=idempotency_key,
             defaults={
                 'quantity': transaction.quantity * -1,
                 'metadata': metadata,
             },
         )
+        TRANSACTION_REVERSED.send(sender=models.Reversal, reversal=reversal)
         return reversal
 
 
 def create_ledger(unit=None, idempotency_key=None, subsidy_uuid=None, initial_deposit=None, **metadata):
     """
     Primary interface for creating a Ledger record.
```

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0001_initial.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0003_field_updates_20230216_1605.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0003_field_updates_20230216_1605.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0004_ledger_idpkey_blankable.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0005_help_text_and_more_indices.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0005_help_text_and_more_indices.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/migrations/0006_auto_20230404_1744.py` & `openedx-ledger-0.3.2/openedx_ledger/migrations/0006_auto_20230404_1744.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/models.py` & `openedx-ledger-0.3.2/openedx_ledger/models.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/templates/edx_ledger/base.html` & `openedx-ledger-0.3.2/openedx_ledger/templates/edx_ledger/base.html`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/test_utils/factories.py` & `openedx-ledger-0.3.2/openedx_ledger/test_utils/factories.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger/utils.py` & `openedx-ledger-0.3.2/openedx_ledger/utils.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/openedx_ledger.egg-info/PKG-INFO` & `openedx-ledger-0.3.2/openedx_ledger.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openedx-ledger
-Version: 0.3.1
+Version: 0.3.2
 Summary: Records transactions against a ledger, denominated in units of value.
 Home-page: https://github.com/openedx/openedx-ledger
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -204,16 +204,19 @@
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
-Nothing
 
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated.  See https://github.com/openedx/edx-sphinx-theme/issues/184 for
+  more details.
+  
 [0.2.2]
 *******
 * Add many help_text fields to model fields.
 * Add some useful composite table indices.
 * Add a "failed" transaction state.
 
 [0.2.0]
```

### Comparing `openedx-ledger-0.3.1/openedx_ledger.egg-info/SOURCES.txt` & `openedx-ledger-0.3.2/openedx_ledger.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 openedx_ledger/migrations/0001_initial.py
 openedx_ledger/migrations/0002_historicalledger_historicalreversal_historicaltransaction.py
 openedx_ledger/migrations/0003_field_updates_20230216_1605.py
 openedx_ledger/migrations/0004_ledger_idpkey_blankable.py
 openedx_ledger/migrations/0005_help_text_and_more_indices.py
 openedx_ledger/migrations/0006_auto_20230404_1744.py
 openedx_ledger/migrations/__init__.py
+openedx_ledger/signals/__init__.py
+openedx_ledger/signals/signals.py
 openedx_ledger/templates/edx_ledger/base.html
+openedx_ledger/templates/edx_ledger/admin/reverse_transaction.html
 openedx_ledger/test_utils/__init__.py
 openedx_ledger/test_utils/factories.py
 requirements/base.in
 requirements/constraints.txt
 tests/test_api.py
 tests/test_models.py
```

### Comparing `openedx-ledger-0.3.1/requirements/constraints.txt` & `openedx-ledger-0.3.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/setup.py` & `openedx-ledger-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/tests/test_api.py` & `openedx-ledger-0.3.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openedx-ledger-0.3.1/tests/test_models.py` & `openedx-ledger-0.3.2/tests/test_models.py`

 * *Files identical despite different names*

