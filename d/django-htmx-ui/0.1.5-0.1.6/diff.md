# Comparing `tmp/django_htmx_ui-0.1.5.tar.gz` & `tmp/django_htmx_ui-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_htmx_ui-0.1.5.tar", last modified: Mon Apr 24 09:31:21 2023, max compression
+gzip compressed data, was "django_htmx_ui-0.1.6.tar", last modified: Tue Apr 25 13:50:36 2023, max compression
```

## Comparing `django_htmx_ui-0.1.5.tar` & `django_htmx_ui-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-27 22:03:36.000000 django_htmx_ui-0.1.5/LICENSE
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30627 2023-04-24 09:25:54.000000 django_htmx_ui-0.1.5/README.md
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-04-24 09:25:30.000000 django_htmx_ui-0.1.5/pyproject.toml
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/setup.cfg
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/admin.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/apps.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/forms.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1305 2023-03-11 08:30:48.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/jinja.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/middleware.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/migrations/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/migrations/__init__.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/models.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/tests.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/urls.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     7519 2023-04-20 08:28:01.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/utils.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui/views/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-26 11:45:23.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/crud.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     6947 2023-04-24 08:59:54.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/generic.py
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     7441 2023-04-23 16:59:32.000000 django_htmx_ui-0.1.5/src/django_htmx_ui/views/mixins.py
-drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-24 09:31:21.301876 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/PKG-INFO
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/dependency_links.txt
--rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/requires.txt
--rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-04-24 09:31:21.000000 django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/top_level.txt
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1075 2023-02-27 22:03:36.000000 django_htmx_ui-0.1.6/LICENSE
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/PKG-INFO
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    30627 2023-04-24 09:25:54.000000 django_htmx_ui-0.1.6/README.md
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      721 2023-04-25 13:47:35.000000 django_htmx_ui-0.1.6/pyproject.toml
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       38 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/setup.cfg
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:35.997534 django_htmx_ui-0.1.6/src/
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/src/django_htmx_ui/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/__init__.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/admin.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      158 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/apps.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/forms.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1305 2023-03-11 08:30:48.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/jinja.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1744 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/middleware.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/src/django_htmx_ui/migrations/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/migrations/__init__.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/models.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       60 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/tests.py
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        0 2023-02-08 11:09:09.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/urls.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7557 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/utils.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/src/django_htmx_ui/views/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)     1929 2023-02-26 11:45:23.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/views/crud.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7167 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/views/generic.py
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)     7764 2023-04-25 13:45:56.000000 django_htmx_ui-0.1.6/src/django_htmx_ui/views/mixins.py
+drwxr-xr-x   0 nikalexis  (1000) nikalexis  (1000)        0 2023-04-25 13:50:36.007534 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)    31177 2023-04-25 13:50:35.000000 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)      674 2023-04-25 13:50:35.000000 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)        1 2023-04-25 13:50:35.000000 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 nikalexis  (1000) nikalexis  (1000)       50 2023-04-25 13:50:35.000000 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/requires.txt
+-rw-rw-r--   0 nikalexis  (1000) nikalexis  (1000)       15 2023-04-25 13:50:35.000000 django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/top_level.txt
```

### Comparing `django_htmx_ui-0.1.5/LICENSE` & `django_htmx_ui-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.5/PKG-INFO` & `django_htmx_ui-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_htmx_ui
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django - HTMX - Jinja powerful combination library
 Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
 Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
 Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_htmx_ui-0.1.5/README.md` & `django_htmx_ui-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.5/pyproject.toml` & `django_htmx_ui-0.1.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_htmx_ui"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Nikalexis Nikolaos", email="nikalexis@gmail.com" },
 ]
 description = "Django - HTMX - Jinja powerful combination library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/jinja.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/jinja.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/middleware.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/middleware.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/utils.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         self.view_ref = view_ref
         self.args = args
         self.kwargs = kwargs
 
     def update(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
-        del self._url
+        if hasattr(self, '_url'):
+            del self._url
         return self
 
     @functools.cached_property
     def _url(self):
         return Url.create(self.view_ref, *self.args, **self.kwargs)
 
     @property
```

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/views/crud.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/views/crud.py`

 * *Files identical despite different names*

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/views/generic.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/views/generic.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from django.contrib import messages
 from django.contrib.auth.mixins import LoginRequiredMixin
 from django.http import HttpResponse
 from django.shortcuts import redirect
 from django.template import engines
 from django.urls import re_path
 from django.views.generic import TemplateView, RedirectView
+from django.utils.cache import patch_vary_headers
 from django_htmx.http import HttpResponseLocation, trigger_client_event, HttpResponseClientRedirect
 
 from django_htmx_ui.utils import ContextProperty, ContextCachedProperty, merge, to_snake_case, UrlView, Location
 from django_htmx_ui.views.mixins import OriginTemplateMixin
 
 
 class BaseTemplateView(TemplateView):
     response = None
+    vary_headers = ("Hx-Request",)
 
     def setup(self, request, *args, **kwargs):
         self.headers = {}
         self.triggers = []
         self.request = request
         self.location_bar = Location.create_from_url(self.bar_url())
         self.location_req = Location.create_from_url(request.get_full_path())
@@ -67,14 +69,16 @@
         for func in (self.apply_triggers, self.apply_headers, self.apply_location):
             response = func(response)
         return response
 
     def apply_headers(self, response):
         for key, value in self.headers.items():
             response[key] = value
+        if self.vary_headers:
+            patch_vary_headers(response, self.vary_headers)
         return response
 
     def apply_triggers(self, response):
         for args, kwargs in self.triggers:
             trigger_client_event(response, *args, **kwargs)
         return response
 
@@ -103,15 +107,15 @@
         return {
             **super().get_context_data(**kwargs),
             **self.decorators_context(),
             **getattr(self, '_context', {}),
         }
 
     def get_template_names(self):
-        if not self.request.htmx:
+        if not self.request.htmx or self.request.htmx.history_restore_request:
             return self.template_origin
         else:
             return super().get_template_names()
 
     def add_context(self, key, value):
         setattr(self, '_context', merge(getattr(self, '_context', {}), {key: value}))
```

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui/views/mixins.py` & `django_htmx_ui-0.1.6/src/django_htmx_ui/views/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     @classmethod
     @property
     def path_route(cls):
         return '(?P<pk>\w+)/' + super().path_route
 
     @ContextProperty
     def url(self):
-        return UrlView(self, self.instance.pk)
+        return super().url(self, self.instance.pk)
 
     @ContextCachedProperty
     def instance(self):
         return self.module.MODEL.objects.get(pk=self.request.resolver_match.kwargs['pk'])
 
     @property
     def instance_slug(self):
@@ -138,15 +138,15 @@
             self.selected = selected
             self.remember = remember
             self.links = links
 
             for i, l in enumerate(self.links):
                 l.index = i
                 if titles_slugify and l._slug is None:
-                    l._slug = slugify(l.title) or None
+                    l._slug = slugify(l.title).replace('-', '_') or None
                     if l._slug in [ls.slug for ls in self.links if ls.index != l.index]:
                         l._slug = None
 
         @property
         def active(self):
             return self.links[self.selected]
 
@@ -172,25 +172,34 @@
     @property
     def tab_session_key(self):
         return f'tabs-remember-{self.slug_tab}'
     
     @property
     def tab_selected_candidates(self):
         return [
-            self.request.resolver_match.kwargs.get(self.slug_tab),
             self.location_req.query.get(self.tab_query_var, True),
             self.location_bar.query.get(self.tab_query_var, True),
+            self.request.resolver_match.kwargs.get(self.slug_tab),
             self.request.session.get(self.tab_session_key),
         ]
 
     @classmethod
     @property
     def path_route(cls):
         return super().path_route + f'(?:(?P<{cls.slug_tab}>\w+)/)?'
 
+    @ContextProperty
+    def url(self):
+        url = super().url
+        slug = self.request.resolver_match.kwargs.get(self.slug_tab)
+        if slug:
+            return url(self, *(url.args + (slug,)))
+        else:
+            return super().url
+
     def on_get(self, request, *args, **kwargs):
         super().on_get(request, *args, **kwargs)
 
         if self.request.session.get(self.tab_session_key) not in [None] + [l.slug for l in self.tabs.links]:
             del self.request.session[self.tab_session_key]
 
         for c in self.tab_selected_candidates:
@@ -200,15 +209,15 @@
                         self.tabs.selected = link.index
                         break
                 else:
                     raise ValueError(f"Tab slug '{c}' not found.")
                 break
 
         if self.location_bar.resolver_match.view_name == self.url.resolver_match.view_name:
-            new_path = self.url(**{self.slug_tab: self.tabs.active.slug})
+            new_path = self.url().update(**{**self.request.resolver_match.kwargs, **{self.slug_tab: self.tabs.active.slug}})
             self.location_bar(path=new_path).query.remove(self.tab_query_var)
         else:
             current_slug = self.location_bar.query.get(self.tab_query_var)
             if current_slug != self.tabs.active.slug:
                 push = current_slug is not None
                 self.location_bar(push=push).query(**{self.tab_query_var: self.tabs.active.slug})
```

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/PKG-INFO` & `django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-ui
-Version: 0.1.5
+Version: 0.1.6
 Summary: Django - HTMX - Jinja powerful combination library
 Author-email: Nikalexis Nikolaos <nikalexis@gmail.com>
 Project-URL: Homepage, https://github.com/nikalexis/django_htmx_ui
 Project-URL: Bug Tracker, https://github.com/nikalexis/django_htmx_ui/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `django_htmx_ui-0.1.5/src/django_htmx_ui.egg-info/SOURCES.txt` & `django_htmx_ui-0.1.6/src/django_htmx_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

