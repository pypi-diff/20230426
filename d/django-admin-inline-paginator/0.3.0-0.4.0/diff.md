# Comparing `tmp/django-admin-inline-paginator-0.3.0.tar.gz` & `tmp/django-admin-inline-paginator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-admin-inline-paginator-0.3.0.tar", last modified: Sun Dec 26 19:26:44 2021, max compression
+gzip compressed data, was "django-admin-inline-paginator-0.4.0.tar", last modified: Wed Apr 26 18:11:04 2023, max compression
```

## Comparing `django-admin-inline-paginator-0.3.0.tar` & `django-admin-inline-paginator-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,27 @@
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1076 2021-06-08 01:41:13.000000 django-admin-inline-paginator-0.3.0/LICENSE
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      259 2021-06-08 01:41:13.000000 django-admin-inline-paginator-0.3.0/MANIFEST.in
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3516 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/PKG-INFO
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1798 2021-06-08 02:09:53.000000 django-admin-inline-paginator-0.3.0/README.md
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.809781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      251 2021-12-26 19:04:40.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/__init__.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     2567 2021-12-26 19:04:15.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/admin.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      263 2021-12-26 19:04:15.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/apps.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.809781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/static/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.809781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/static/django_admin_inline_paginator/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      379 2021-06-08 01:41:13.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/static/django_admin_inline_paginator/paginator.css
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.809781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templates/
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templates/admin/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      149 2021-06-08 03:37:38.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templates/admin/tabular_paginated.html
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     2064 2021-06-08 01:41:13.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templates/admin/tabular_paginator.html
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templatetags/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        0 2021-06-08 01:47:11.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templatetags/__init__.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      517 2021-12-26 19:04:15.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templatetags/paginated_inline.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/tests/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      696 2021-06-08 01:41:13.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/tests/__init__.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1286 2021-12-26 19:04:15.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/tests/admin_unit_test.py
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      754 2021-12-26 19:04:15.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/tests/apps_test.py
-drwxrwxr-x   0 shinneider  (1000) shinneider  (1000)        0 2021-12-26 19:26:44.809781 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     3516 2021-12-26 19:26:44.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/PKG-INFO
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      920 2021-12-26 19:26:44.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/SOURCES.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)        1 2021-12-26 19:26:44.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/dependency_links.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       93 2021-12-26 19:26:44.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/requires.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)       30 2021-12-26 19:26:44.000000 django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/top_level.txt
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)      116 2021-12-26 19:26:44.813781 django-admin-inline-paginator-0.3.0/setup.cfg
--rw-rw-r--   0 shinneider  (1000) shinneider  (1000)     1714 2021-11-06 08:58:05.000000 django-admin-inline-paginator-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/static/django_admin_inline_paginator/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/static/django_admin_inline_paginator/paginator.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templates/admin/tabular_paginated.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templates/admin/tabular_paginator.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templatetags/paginated_inline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-04-26 18:11:04.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-26 18:11:04.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:11:04.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-26 18:11:04.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-26 18:11:04.000000 django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 18:11:04.359964 django-admin-inline-paginator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-26 18:10:39.000000 django-admin-inline-paginator-0.4.0/setup.py
```

### Comparing `django-admin-inline-paginator-0.3.0/LICENSE` & `django-admin-inline-paginator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-admin-inline-paginator-0.3.0/PKG-INFO` & `django-admin-inline-paginator-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-inline-paginator
-Version: 0.3.0
+Version: 0.4.0
 Summary: The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
 Home-page: https://github.com/shinneider/django-admin-inline-paginator
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
-Description: Django Admin Inline Paginator
-        =============================
-        
-        The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
-        
-        If you use or like the project, click `Star` and `Watch` to generate metrics and i evaluate project continuity.
-        
-        # Install:
-        
-        ```
-        pip install django-admin-inline-paginator
-        ```
-        
-        # Usage:
-        
-        1. Add to your INSTALLED_APPS, in settings.py:
-        
-           ```
-           INSTALLED_APPS = [
-               ...
-               'django_admin_inline_paginator',
-               ...
-           ]
-           ```
-        2. Create your model inline:
-        
-           ```
-           from django_admin_inline_paginator.admin import TabularInlinePaginated
-        
-           class ModelWithFKAdminInline(TabularInlinePaginated):
-               fields = (...)
-               per_page = 1
-               model = ModelWithFK
-           ```
-        3. Create main model admin and use inline:
-        
-            ```
-            @register(YourModel)
-            class YourModelAdmin(ModelAdmin):
-                fields = (...)
-                inlines = (ModelWithFKAdminInline, )
-                model = YourModel
-            ```
-        
-        # Advanced Usage:
-        
-        1. Paginate multiples inlines:
-            
-            ```
-            class ModelWithFKInline(TabularInlinePaginated):
-            fields = ('name', 'active')
-            per_page = 2
-            model = ModelWithFK
-            pagination_key = 'page-model'  # make sure it's unique for page inline
-        
-            class AnotherModelWithFKInline(TabularInlinePaginated):
-            fields = ('name', 'active')
-            per_page = 2
-            model = AnotherModelWithFK
-            pagination_key = 'page-another-model'  # make sure it's unique for page inline
-            ```
-        
-        2. Use previous inlines
-            
-            ```
-            @register(YourModel)
-            class YourModelAdmin(ModelAdmin):
-                fields = (...)
-                inlines = (ModelWithFKAdminInline, AnotherModelWithFKInline)
-                model = YourModel
-            ```
-        
-        # Images:
-        
-        ![image](https://user-images.githubusercontent.com/30196992/98023167-706ca880-1dfe-11eb-89fe-c056741f0d5b.png)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -96,7 +19,90 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: code-quality
+License-File: LICENSE
+
+Django Admin Inline Paginator
+=============================
+
+The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
+
+If you use or like the project, click `Star` and `Watch` to generate metrics and i evaluate project continuity.
+
+# Install:
+
+```
+pip install django-admin-inline-paginator
+```
+
+# Usage:
+
+1. Add to your INSTALLED_APPS, in settings.py:
+
+   ```
+   INSTALLED_APPS = [
+       ...
+       'django_admin_inline_paginator',
+       ...
+   ]
+   ```
+2. Create your model inline:
+
+   ```
+   from django_admin_inline_paginator.admin import TabularInlinePaginated
+
+   class ModelWithFKAdminInline(TabularInlinePaginated):
+       fields = (...)
+       per_page = 1
+       model = ModelWithFK
+   ```
+3. Create main model admin and use inline:
+
+    ```
+    @register(YourModel)
+    class YourModelAdmin(ModelAdmin):
+        fields = (...)
+        inlines = (ModelWithFKAdminInline, )
+        model = YourModel
+    ```
+
+# Advanced Usage:
+
+1. Paginate multiples inlines:
+    
+    ```
+    class ModelWithFKInline(TabularInlinePaginated):
+    fields = ('name', 'active')
+    per_page = 2
+    model = ModelWithFK
+    pagination_key = 'page-model'  # make sure it's unique for page inline
+
+    class AnotherModelWithFKInline(TabularInlinePaginated):
+    fields = ('name', 'active')
+    per_page = 2
+    model = AnotherModelWithFK
+    pagination_key = 'page-another-model'  # make sure it's unique for page inline
+    ```
+
+2. Use previous inlines
+    
+    ```
+    @register(YourModel)
+    class YourModelAdmin(ModelAdmin):
+        fields = (...)
+        inlines = (ModelWithFKAdminInline, AnotherModelWithFKInline)
+        model = YourModel
+    ```
+
+# Images:
+
+![image](https://user-images.githubusercontent.com/30196992/98023167-706ca880-1dfe-11eb-89fe-c056741f0d5b.png)
+
+# Need a Maintainer
+ In the last months i don't have much time, health problemas, change of country and others problems.  
+ i have some surgeries for first part of 2022, and all of my current project don't use django-admin.  
+ for these reasons, i need a help for a project continuation!!
```

### Comparing `django-admin-inline-paginator-0.3.0/README.md` & `django-admin-inline-paginator-0.4.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -69,7 +69,12 @@
         inlines = (ModelWithFKAdminInline, AnotherModelWithFKInline)
         model = YourModel
     ```
 
 # Images:
 
 ![image](https://user-images.githubusercontent.com/30196992/98023167-706ca880-1dfe-11eb-89fe-c056741f0d5b.png)
+
+# Need a Maintainer
+ In the last months i don't have much time, health problemas, change of country and others problems.  
+ i have some surgeries for first part of 2022, and all of my current project don't use django-admin.  
+ for these reasons, i need a help for a project continuation!!
```

### Comparing `django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/admin.py` & `django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/admin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Optional
+
 from django.contrib.admin import TabularInline
 from django.contrib.admin.views.main import ChangeList
+from django.contrib.contenttypes.admin import GenericTabularInline
 from django.core.paginator import Paginator
-from django.http import HttpRequest
 from django.db.models import QuerySet
+from django.http import HttpRequest
 
 
 class InlineChangeList:
     """
         Used by template to construct the paginator
     """
     can_show_all = True
@@ -56,24 +58,28 @@
         self._queryset = self.page.object_list
 
     def __init__(self, *args, **kwargs):
         super(PaginationFormSetBase, self).__init__(*args, **kwargs)
         self.mount_paginator()
         self.mount_queryset()
 
-
-class TabularInlinePaginated(TabularInline):
+class InlinePaginated:
     pagination_key = 'page'
     template = 'admin/tabular_paginated.html'
     per_page = 20
     extra = 0
-    can_delete = False
 
     def get_formset(self, request, obj=None, **kwargs):
         formset_class = super().get_formset(request, obj, **kwargs)
 
         class PaginationFormSet(PaginationFormSetBase, formset_class):
             pagination_key = self.pagination_key
 
         PaginationFormSet.request = request
         PaginationFormSet.per_page = self.per_page
         return PaginationFormSet
+
+class TabularInlinePaginated(InlinePaginated, TabularInline):
+    pass
+
+class GenericTabularInlinePaginated(InlinePaginated, GenericTabularInline):
+    pass
```

### Comparing `django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templates/admin/tabular_paginator.html` & `django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templates/admin/tabular_paginator.html`

 * *Files identical despite different names*

### Comparing `django-admin-inline-paginator-0.3.0/django_admin_inline_paginator/templatetags/paginated_inline.py` & `django-admin-inline-paginator-0.4.0/django_admin_inline_paginator/templatetags/paginated_inline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import urllib.parse
 
 from django import template
 
-
 register = template.Library()
 
 
 @register.simple_tag
 def modify_pagination_path(full_path: str, key: str, value: str) -> str:
     get_params = full_path
     if get_params.find('?') > -1:
```

### Comparing `django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/PKG-INFO` & `django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,15 @@
 Metadata-Version: 2.1
 Name: django-admin-inline-paginator
-Version: 0.3.0
+Version: 0.4.0
 Summary: The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
 Home-page: https://github.com/shinneider/django-admin-inline-paginator
 Author: Shinneider Libanio da Silva
 Author-email: shinneider-libanio@hotmail.com
 License: MIT
-Description: Django Admin Inline Paginator
-        =============================
-        
-        The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
-        
-        If you use or like the project, click `Star` and `Watch` to generate metrics and i evaluate project continuity.
-        
-        # Install:
-        
-        ```
-        pip install django-admin-inline-paginator
-        ```
-        
-        # Usage:
-        
-        1. Add to your INSTALLED_APPS, in settings.py:
-        
-           ```
-           INSTALLED_APPS = [
-               ...
-               'django_admin_inline_paginator',
-               ...
-           ]
-           ```
-        2. Create your model inline:
-        
-           ```
-           from django_admin_inline_paginator.admin import TabularInlinePaginated
-        
-           class ModelWithFKAdminInline(TabularInlinePaginated):
-               fields = (...)
-               per_page = 1
-               model = ModelWithFK
-           ```
-        3. Create main model admin and use inline:
-        
-            ```
-            @register(YourModel)
-            class YourModelAdmin(ModelAdmin):
-                fields = (...)
-                inlines = (ModelWithFKAdminInline, )
-                model = YourModel
-            ```
-        
-        # Advanced Usage:
-        
-        1. Paginate multiples inlines:
-            
-            ```
-            class ModelWithFKInline(TabularInlinePaginated):
-            fields = ('name', 'active')
-            per_page = 2
-            model = ModelWithFK
-            pagination_key = 'page-model'  # make sure it's unique for page inline
-        
-            class AnotherModelWithFKInline(TabularInlinePaginated):
-            fields = ('name', 'active')
-            per_page = 2
-            model = AnotherModelWithFK
-            pagination_key = 'page-another-model'  # make sure it's unique for page inline
-            ```
-        
-        2. Use previous inlines
-            
-            ```
-            @register(YourModel)
-            class YourModelAdmin(ModelAdmin):
-                fields = (...)
-                inlines = (ModelWithFKAdminInline, AnotherModelWithFKInline)
-                model = YourModel
-            ```
-        
-        # Images:
-        
-        ![image](https://user-images.githubusercontent.com/30196992/98023167-706ca880-1dfe-11eb-89fe-c056741f0d5b.png)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -96,7 +19,90 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: code-quality
+License-File: LICENSE
+
+Django Admin Inline Paginator
+=============================
+
+The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin
+
+If you use or like the project, click `Star` and `Watch` to generate metrics and i evaluate project continuity.
+
+# Install:
+
+```
+pip install django-admin-inline-paginator
+```
+
+# Usage:
+
+1. Add to your INSTALLED_APPS, in settings.py:
+
+   ```
+   INSTALLED_APPS = [
+       ...
+       'django_admin_inline_paginator',
+       ...
+   ]
+   ```
+2. Create your model inline:
+
+   ```
+   from django_admin_inline_paginator.admin import TabularInlinePaginated
+
+   class ModelWithFKAdminInline(TabularInlinePaginated):
+       fields = (...)
+       per_page = 1
+       model = ModelWithFK
+   ```
+3. Create main model admin and use inline:
+
+    ```
+    @register(YourModel)
+    class YourModelAdmin(ModelAdmin):
+        fields = (...)
+        inlines = (ModelWithFKAdminInline, )
+        model = YourModel
+    ```
+
+# Advanced Usage:
+
+1. Paginate multiples inlines:
+    
+    ```
+    class ModelWithFKInline(TabularInlinePaginated):
+    fields = ('name', 'active')
+    per_page = 2
+    model = ModelWithFK
+    pagination_key = 'page-model'  # make sure it's unique for page inline
+
+    class AnotherModelWithFKInline(TabularInlinePaginated):
+    fields = ('name', 'active')
+    per_page = 2
+    model = AnotherModelWithFK
+    pagination_key = 'page-another-model'  # make sure it's unique for page inline
+    ```
+
+2. Use previous inlines
+    
+    ```
+    @register(YourModel)
+    class YourModelAdmin(ModelAdmin):
+        fields = (...)
+        inlines = (ModelWithFKAdminInline, AnotherModelWithFKInline)
+        model = YourModel
+    ```
+
+# Images:
+
+![image](https://user-images.githubusercontent.com/30196992/98023167-706ca880-1dfe-11eb-89fe-c056741f0d5b.png)
+
+# Need a Maintainer
+ In the last months i don't have much time, health problemas, change of country and others problems.  
+ i have some surgeries for first part of 2022, and all of my current project don't use django-admin.  
+ for these reasons, i need a help for a project continuation!!
```

### Comparing `django-admin-inline-paginator-0.3.0/django_admin_inline_paginator.egg-info/SOURCES.txt` & `django-admin-inline-paginator-0.4.0/django_admin_inline_paginator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,11 +11,8 @@
 django_admin_inline_paginator.egg-info/dependency_links.txt
 django_admin_inline_paginator.egg-info/requires.txt
 django_admin_inline_paginator.egg-info/top_level.txt
 django_admin_inline_paginator/static/django_admin_inline_paginator/paginator.css
 django_admin_inline_paginator/templates/admin/tabular_paginated.html
 django_admin_inline_paginator/templates/admin/tabular_paginator.html
 django_admin_inline_paginator/templatetags/__init__.py
-django_admin_inline_paginator/templatetags/paginated_inline.py
-django_admin_inline_paginator/tests/__init__.py
-django_admin_inline_paginator/tests/admin_unit_test.py
-django_admin_inline_paginator/tests/apps_test.py
+django_admin_inline_paginator/templatetags/paginated_inline.py
```

### Comparing `django-admin-inline-paginator-0.3.0/setup.py` & `django-admin-inline-paginator-0.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-# -*- coding: utf-8 -*-
-#!/usr/bin/env python
+import sys
 from io import open
 
 from setuptools import find_packages, setup
 
-from django_admin_inline_paginator import __version__
 
 extras_require = {
     'dev': [
         'django',
         'django_mock_queries',
         'pylint',
         'pytest-pylint',
         'pytest',
         'pytest-cov',
-        'pytest-watch'
-    ]
+        'pytest-watch',
+        'tox'
+    ],
+    'code-quality': [
+        'isort',
+        'bandit',
+        'xenon',
+    ],
 }
 
+
+def get_version():
+    version = '0.0'
+    for arg in sys.argv:
+        if arg.startswith('--version'):
+            version = arg.split("=")[1]
+            sys.argv.remove(arg)
+            break
+
+    return version if version[0] != 'v' else version[1:]
+
+
 setup(
     name='django-admin-inline-paginator',
-    version=__version__,
+    version=get_version(),
     description='The "Django Admin Inline Paginator" is simple way to paginate your inline in django admin',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Shinneider Libanio da Silva',
     author_email='shinneider-libanio@hotmail.com',
     url='https://github.com/shinneider/django-admin-inline-paginator',
     license='MIT',
```

