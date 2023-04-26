# Comparing `tmp/django-ninja-passwordreset-1.0.0.tar.gz` & `tmp/django-ninja-passwordreset-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ninja-passwordreset-1.0.0.tar", last modified: Mon Nov 22 20:35:54 2021, max compression
+gzip compressed data, was "django-ninja-passwordreset-1.2.4.tar", last modified: Tue Apr 25 19:24:40 2023, max compression
```

## Comparing `django-ninja-passwordreset-1.0.0.tar` & `django-ninja-passwordreset-1.2.4.tar`

### file list

```diff
@@ -1,51 +1,50 @@
--rw-r--r--   0        0        0    53248 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.coverage
--rw-r--r--   0        0        0      120 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.flake8
--rw-r--r--   0        0        0      401 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      541 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0        0        0      570 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      545 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1278 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.github/workflows/test_full.yml
--rw-r--r--   0        0        0       88 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.gitignore
--rw-r--r--   0        0        0       53 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.isort.cfg
--rw-r--r--   0        0        0      559 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0     1976 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1571 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/LICENSE
--rw-r--r--   0        0        0       58 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0      939 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/Makefile
--rw-r--r--   0        0        0    12488 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/README.md
--rw-r--r--   0        0        0    12115 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/coverage.xml
--rw-r--r--   0        0        0      203 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/__init__.py
--rw-r--r--   0        0        0      287 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/admin.py
--rw-r--r--   0        0        0      328 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/apps.py
--rw-r--r--   0        0        0     6809 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/controller.py
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/management/__init__.py
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/management/commands/__init__.py
--rw-r--r--   0        0        0      549 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py
--rw-r--r--   0        0        0     2077 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0001_initial.py
--rw-r--r--   0        0        0     3023 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0002_pk_migration.py
--rw-r--r--   0        0        0      894 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/__init__.py
--rw-r--r--   0        0        0     3667 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/models.py
--rw-r--r--   0        0        0     1788 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/schema.py
--rw-r--r--   0        0        0       13 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/serializers.py
--rw-r--r--   0        0        0      362 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/signals.py
--rw-r--r--   0        0        0     2838 2021-11-22 20:35:37.481681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/tokens.py
--rw-r--r--   0        0        0       14 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/urls.py
--rw-r--r--   0        0        0        7 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/django_rest_passwordreset/views.py
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/docs/.gitkeep
--rw-r--r--   0        0        0    58293 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/docs/browsable_api_email_validation.png
--rw-r--r--   0        0        0    60179 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/docs/browsable_api_password_validation.png
--rw-r--r--   0        0        0    79223 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/docs/coreapi_docs.png
--rw-r--r--   0        0        0     2065 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/pyproject.toml
--rwxr-xr-x   0        0        0       78 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/pytest.ini
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/.gitkeep
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      216 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/api.py
--rw-r--r--   0        0        0     2277 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/test/__init__.py
--rw-r--r--   0        0        0     2754 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/test/helpers.py
--rw-r--r--   0        0        0    18969 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/test/test_auth_test_case.py
--rw-r--r--   0        0        0     5558 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/test/test_token_generators.py
--rw-r--r--   0        0        0      197 2021-11-22 20:35:37.485681 django-ninja-passwordreset-1.0.0/tests/urls.py
--rw-r--r--   0        0        0    14674 1970-01-01 00:00:00.000000 django-ninja-passwordreset-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    53248 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.coverage
+-rw-r--r--   0        0        0      120 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.flake8
+-rw-r--r--   0        0        0      401 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      541 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0        0        0      570 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      545 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1291 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0       88 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.gitignore
+-rw-r--r--   0        0        0       53 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.isort.cfg
+-rw-r--r--   0        0        0     1069 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      559 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/.vscode/launch.json
+-rw-r--r--   0        0        0     1976 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1571 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/LICENSE
+-rw-r--r--   0        0        0       58 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/MANIFEST.in
+-rw-r--r--   0        0        0      974 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/Makefile
+-rw-r--r--   0        0        0    12488 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/README.md
+-rw-r--r--   0        0        0    12115 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/coverage.xml
+-rw-r--r--   0        0        0      203 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/__init__.py
+-rw-r--r--   0        0        0      287 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/admin.py
+-rw-r--r--   0        0        0      328 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/apps.py
+-rw-r--r--   0        0        0     6828 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/controller.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/management/commands/__init__.py
+-rw-r--r--   0        0        0      549 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py
+-rw-r--r--   0        0        0     2077 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3023 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0002_pk_migration.py
+-rw-r--r--   0        0        0      894 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/__init__.py
+-rw-r--r--   0        0        0     3667 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/models.py
+-rw-r--r--   0        0        0     1781 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/schema.py
+-rw-r--r--   0        0        0      362 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/signals.py
+-rw-r--r--   0        0        0     2838 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/tokens.py
+-rw-r--r--   0        0        0       14 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/django_rest_passwordreset/urls.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/docs/.gitkeep
+-rw-r--r--   0        0        0    58293 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/docs/browsable_api_email_validation.png
+-rw-r--r--   0        0        0    60179 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/docs/browsable_api_password_validation.png
+-rw-r--r--   0        0        0    79223 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/docs/coreapi_docs.png
+-rw-r--r--   0        0        0     2242 2023-04-25 19:24:27.693446 django-ninja-passwordreset-1.2.4/pyproject.toml
+-rwxr-xr-x   0        0        0       78 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/pytest.ini
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/.gitkeep
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      216 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/api.py
+-rw-r--r--   0        0        0     2277 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/test/__init__.py
+-rw-r--r--   0        0        0     2754 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/test/helpers.py
+-rw-r--r--   0        0        0    18969 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/test/test_auth_test_case.py
+-rw-r--r--   0        0        0     5558 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/test/test_token_generators.py
+-rw-r--r--   0        0        0      197 2023-04-25 19:24:27.697446 django-ninja-passwordreset-1.2.4/tests/urls.py
+-rw-r--r--   0        0        0    14892 1970-01-01 00:00:00.000000 django-ninja-passwordreset-1.2.4/PKG-INFO
```

### Comparing `django-ninja-passwordreset-1.0.0/.coverage` & `django-ninja-passwordreset-1.2.4/.coverage`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `django-ninja-passwordreset-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md` & `django-ninja-passwordreset-1.2.4/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/.github/workflows/publish.yml` & `django-ninja-passwordreset-1.2.4/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python
         uses: actions/setup-python@v1
         with:
-          python-version: 3.6
+          python-version: 3.8
       - name: Install Flit
         run: pip install flit
       - name: Install Dependencies
         run: flit install --symlink
       - name: Publish
         env:
           FLIT_USERNAME: ${{ secrets.FLIT_USERNAME }}
```

### Comparing `django-ninja-passwordreset-1.0.0/.github/workflows/test.yml` & `django-ninja-passwordreset-1.2.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/.github/workflows/test_full.yml` & `django-ninja-passwordreset-1.2.4/.github/workflows/test_full.yml`

 * *Files 17% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ['3.6', '3.7', '3.8', '3.9']
-        django-version: ['<2.1', '<2.2', '<3.0', '<3.1', '<3.2', '<3.3']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        django-version: ['<3.0', '<3.1', '<3.2', '<3.3', '<4.1', '<4.2']
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python
-        uses: actions/setup-python@v1
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install core
         run: pip install "Django${{ matrix.django-version }}"
       - name: Install tests
-        run: pip install pytest ninja-schema pytest-django django-ninja-extra pyjwt[crypto]
+        run: pip install pytest pytest-django django-ninja-extra pyjwt[crypto] pydantic[email]
       - name: Test
         run: pytest
   codestyle:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v2
@@ -40,8 +40,8 @@
       - name: Install Dependencies
         run: flit install --symlink
       - name: Black
         run: black --check django_rest_passwordreset tests
       - name: isort
         run: isort --check django_rest_passwordreset tests
       - name: Flake8
-        run: flake8 django_rest_passwordreset tests
+        run: flake8 django_rest_passwordreset tests
```

### Comparing `django-ninja-passwordreset-1.0.0/.vscode/launch.json` & `django-ninja-passwordreset-1.2.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/CHANGELOG.md` & `django-ninja-passwordreset-1.2.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/LICENSE` & `django-ninja-passwordreset-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/Makefile` & `django-ninja-passwordreset-1.2.4/Makefile`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 clean: ## Removing cached python compiled files
 	find . -name \*pyc  | xargs  rm -fv
 	find . -name \*pyo | xargs  rm -fv
 	find . -name \*~  | xargs  rm -fv
 	find . -name __pycache__  | xargs  rm -rfv
 
 install: ## Install dependencies
+	make clean
 	flit install --deps develop --symlink
+	pre-commit install -f
 
 lint: ## Run code linters
 	make clean
 	black --check django_rest_passwordreset tests
 	isort --check django_rest_passwordreset tests
 	flake8 django_rest_passwordreset tests
 # 	mypy  ninja_jwt
```

### Comparing `django-ninja-passwordreset-1.0.0/README.md` & `django-ninja-passwordreset-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/coverage.xml` & `django-ninja-passwordreset-1.2.4/coverage.xml`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/controller.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from django.contrib.auth.password_validation import (
     get_password_validators,
     validate_password,
 )
 from django.core.exceptions import ValidationError
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
-from ninja_extra import APIController, exceptions, route, router
+from ninja_extra import ControllerBase, api_controller, exceptions, http_post
 
 from .models import (
     ResetPasswordToken,
     clear_expired,
     get_password_reset_lookup_field,
     get_password_reset_token_expiry_time,
 )
@@ -45,26 +45,26 @@
     """
     normalized1 = unicodedata.normalize("NFKC", s1)
     normalized2 = unicodedata.normalize("NFKC", s2)
 
     return normalized1.casefold() == normalized2.casefold()
 
 
-@router("password_reset/", tags=["Password Reset"])
-class ResetPasswordController(APIController):
+@api_controller("password_reset/", tags=["Password Reset"])
+class ResetPasswordController(ControllerBase):
     auto_import = False
 
-    @route.post("validate_token/", url_name="reset-password-validate")
+    @http_post("validate_token/", url_name="reset-password-validate")
     def validate_token(self, reset_token: ResetTokenSerializer):
         """
         An Api View which provides a method to verify that a token is valid
         """
         return self.create_response({"status": "OK"})
 
-    @route.post("confirm/", url_name="reset-password-confirm")
+    @http_post("confirm/", url_name="reset-password-confirm")
     def password_confirm(self, password_token: PasswordTokenSerializer):
         password = password_token.password
         token = password_token.token
 
         # find token
         reset_password_token = ResetPasswordToken.objects.filter(key=token).first()
 
@@ -93,15 +93,15 @@
             )
 
         # Delete all password reset tokens for this user
         ResetPasswordToken.objects.filter(user=reset_password_token.user).delete()
 
         return self.create_response({"status": "OK"})
 
-    @route.post("", url_name="reset-password-request")
+    @http_post("", url_name="reset-password-request")
     def password_request_token(self, email_data: EmailSerializer):
         email = email_data.email
 
         # before we continue, delete all existing expired tokens
         password_reset_token_validation_time = get_password_reset_token_expiry_time()
 
         # datetime.now minus expiry hours
```

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/management/commands/clearresetpasswodtokens.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0001_initial.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0002_pk_migration.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0002_pk_migration.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/migrations/0003_allow_blank_and_null_fields.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/models.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/models.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/schema.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import timedelta
 
 from django.core.exceptions import ValidationError
 from django.http import Http404
 from django.shortcuts import get_object_or_404 as _get_object_or_404
 from django.utils import timezone
 from django.utils.translation import gettext_lazy as _
-from ninja_schema import Schema
+from ninja import Schema
 from pydantic import EmailStr, root_validator
 
 from . import models
 
 __all__ = [
     "EmailSerializer",
     "PasswordTokenSerializer",
```

### Comparing `django-ninja-passwordreset-1.0.0/django_rest_passwordreset/tokens.py` & `django-ninja-passwordreset-1.2.4/django_rest_passwordreset/tokens.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/docs/browsable_api_email_validation.png` & `django-ninja-passwordreset-1.2.4/docs/browsable_api_email_validation.png`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/docs/browsable_api_password_validation.png` & `django-ninja-passwordreset-1.2.4/docs/browsable_api_password_validation.png`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/docs/coreapi_docs.png` & `django-ninja-passwordreset-1.2.4/docs/coreapi_docs.png`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/pyproject.toml` & `django-ninja-passwordreset-1.2.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project]
 name = "django-ninja-passwordreset"
 authors = [
    {name = "Christian Kreuzberger", email = "ckreuzberger@anexia-it.com"},
    {name = "Ezeudoh Tochukwu", email = "tochukwu.ezeudoh@gmail.com"},
 ]
 dynamic = ["version", "description"]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 readme = "README.md"
 home-page = "https://github.com/eadwinCode/django-ninja-passwordreset"
 classifiers = [
     "Intended Audience :: Information Technology",
     "Intended Audience :: System Administrators",
     "Operating System :: OS Independent",
     "Topic :: Internet",
@@ -26,45 +26,49 @@
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development",
     "Typing :: Typed",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
     "Framework :: Django",
     "Framework :: Django :: 2.1",
     "Framework :: Django :: 2.2",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 dependencies = [
     "Django >=2.1",
     "django-ninja-extra",
-    "ninja-schema",
-    "pyjwt[crypto]"
+    "pyjwt[crypto]",
+    "pydantic[email]"
 ]
 
 
 [project.urls]
 Documentation = "https://github.com/eadwinCode/django-ninja-passwordreset"
 Source = "https://github.com/eadwinCode/django-ninja-passwordreset"
 
 [project.optional-dependencies]
 test = [
-    "black",
-    "isort",
-    "flake8",
+    "black==21.12b0",
+    "isort >=5.0.6,<6.0.0",
+    "flake8 >=3.8.3,<7.0.0",
+    "click==8.0.4",
     "pytest",
     "pytest-django",
     "pytest-cov",
 ]
 doc = []
```

### Comparing `django-ninja-passwordreset-1.0.0/tests/conftest.py` & `django-ninja-passwordreset-1.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/tests/test/helpers.py` & `django-ninja-passwordreset-1.2.4/tests/test/helpers.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/tests/test/test_auth_test_case.py` & `django-ninja-passwordreset-1.2.4/tests/test/test_auth_test_case.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/tests/test/test_token_generators.py` & `django-ninja-passwordreset-1.2.4/tests/test/test_token_generators.py`

 * *Files identical despite different names*

### Comparing `django-ninja-passwordreset-1.0.0/PKG-INFO` & `django-ninja-passwordreset-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 Metadata-Version: 2.1
 Name: django-ninja-passwordreset
-Version: 1.0.0
+Version: 1.2.4
 Summary: An extension of django ninja framework, providing a configurable password reset strategy
 Author-email: Christian Kreuzberger <ckreuzberger@anexia-it.com>, Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: Django >=2.1
 Requires-Dist: django-ninja-extra
-Requires-Dist: ninja-schema
 Requires-Dist: pyjwt[crypto]
-Requires-Dist: black ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: pydantic[email]
+Requires-Dist: black==21.12b0 ; extra == "test"
+Requires-Dist: isort >=5.0.6,<6.0.0 ; extra == "test"
+Requires-Dist: flake8 >=3.8.3,<7.0.0 ; extra == "test"
+Requires-Dist: click==8.0.4 ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Project-URL: Documentation, https://github.com/eadwinCode/django-ninja-passwordreset
 Project-URL: Source, https://github.com/eadwinCode/django-ninja-passwordreset
 Provides-Extra: doc
 Provides-Extra: test
```

