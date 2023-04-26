# Comparing `tmp/drf_nested_browsable-0.1.2.tar.gz` & `tmp/drf_nested_browsable-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_nested_browsable-0.1.2.tar", max compression
+gzip compressed data, was "drf_nested_browsable-0.2.1.tar", max compression
```

## Comparing `drf_nested_browsable-0.1.2.tar` & `drf_nested_browsable-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1361 2023-04-24 15:12:49.325818 drf_nested_browsable-0.1.2/README.md
--rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.1.2/drf_nested_browsable/__init__.py
--rw-r--r--   0        0        0     4385 2023-04-23 08:23:30.043605 drf_nested_browsable-0.1.2/drf_nested_browsable/serializers.py
--rw-r--r--   0        0        0     3463 2023-04-24 15:10:03.715669 drf_nested_browsable-0.1.2/drf_nested_browsable/templates/writable_list.html
--rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.1.2/drf_nested_browsable/templatetags/__init__.py
--rw-r--r--   0        0        0     1809 2023-04-24 14:57:46.511666 drf_nested_browsable-0.1.2/drf_nested_browsable/templatetags/drf_nested_browsable.py
--rw-r--r--   0        0        0     1099 2023-04-24 15:13:47.335870 drf_nested_browsable-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.2/setup.py
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 drf_nested_browsable-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1361 2023-04-24 15:12:49.325818 drf_nested_browsable-0.2.1/README.md
+-rw-r--r--   0        0        0      213 2023-04-23 08:13:02.976124 drf_nested_browsable-0.2.1/drf_nested_browsable/__init__.py
+-rw-r--r--   0        0        0     5122 2023-04-26 09:30:40.887333 drf_nested_browsable-0.2.1/drf_nested_browsable/serializers.py
+-rw-r--r--   0        0        0     3463 2023-04-26 07:51:44.002578 drf_nested_browsable-0.2.1/drf_nested_browsable/templates/writable_list.html
+-rw-r--r--   0        0        0        0 2023-04-21 13:53:21.631214 drf_nested_browsable-0.2.1/drf_nested_browsable/templatetags/__init__.py
+-rw-r--r--   0        0        0     1809 2023-04-26 07:48:30.548905 drf_nested_browsable-0.2.1/drf_nested_browsable/templatetags/drf_nested_browsable.py
+-rw-r--r--   0        0        0     1099 2023-04-26 09:30:58.520686 drf_nested_browsable-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2240 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.1/setup.py
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 drf_nested_browsable-0.2.1/PKG-INFO
```

### Comparing `drf_nested_browsable-0.1.2/README.md` & `drf_nested_browsable-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.2/drf_nested_browsable/serializers.py` & `drf_nested_browsable-0.2.1/drf_nested_browsable/serializers.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Using these serializers requires a little more configuration than basic
 serializers.
 TODO: Mettre au propre
 """
 from rest_framework.serializers import ListSerializer, ModelSerializer
 
+
 class WritableNestedListSerializer(ListSerializer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._parent_instance = None
         self._parent_field_name = None
 
@@ -73,15 +74,15 @@
                 full_elem = {**new_elem, **self.parent_data}
 
                 try:
                     elem = instance.get(
                         **{
                             key: new_elem[key] for key in keys if key in new_elem.keys()
                         },
-                        **self.parent_data
+                        **self.parent_data,
                     )
                     elem = self.child.update(elem, full_elem)
                 except instance.model.DoesNotExist:
                     elem = self.child.create(full_elem)
                 updated_ids.append(elem.id)
 
             instance.exclude(id__in=updated_ids).delete()
@@ -97,14 +98,31 @@
             or self.Meta.model_related_name is None
         ):
             raise ValueError(
                 "You must define `model_related_name` when you inherit from"
                 "`WritableNestedModelSerializer`"
             )
 
+        for field_name, field in self._declared_fields.items():
+            if (
+                isinstance(field, WritableNestedListSerializer)
+                and self.Meta.model_related_name in field.child.fields.keys()
+            ):
+                new_fields = []
+                for old_field in field.child.__class__.Meta.fields:
+                    if old_field != self.Meta.model_related_name:
+                        new_fields.append(old_field)
+
+                class NewChild(field.child.__class__):
+                    class Meta(field.child.__class__.Meta):
+                        fields = new_fields
+
+                NewChild.__name__ = field.child.__class__.__name__
+                field.child.__class__ = NewChild
+
         super().__init__(*args, **kwargs)
 
     def create(self, validated_data):
         many_children = {}
         for k, ser in self.fields.items():
             if isinstance(ser, WritableNestedListSerializer):
                 many_children.update({k: (ser, validated_data.pop(k, None))})
```

### Comparing `drf_nested_browsable-0.1.2/drf_nested_browsable/templates/writable_list.html` & `drf_nested_browsable-0.2.1/drf_nested_browsable/templates/writable_list.html`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.2/drf_nested_browsable/templatetags/drf_nested_browsable.py` & `drf_nested_browsable-0.2.1/drf_nested_browsable/templatetags/drf_nested_browsable.py`

 * *Files identical despite different names*

### Comparing `drf_nested_browsable-0.1.2/pyproject.toml` & `drf_nested_browsable-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-nested-browsable"
-version = "0.1.2"
+version = "0.2.1"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Framework :: Django",
     "Intended Audience :: Developers"
 ]
 description = "Writable nested serializers with forms for the Browsable API"
 keywords = ["django", "rest framework", "drf", "browsable api", "nested serializers"]
```

### Comparing `drf_nested_browsable-0.1.2/setup.py` & `drf_nested_browsable-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'drf_nested_browsable': ['templates/*']}
 
 install_requires = \
 ['django>=4.2,<5.0', 'djangorestframework>=3.14.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'drf-nested-browsable',
-    'version': '0.1.2',
+    'version': '0.2.1',
     'description': 'Writable nested serializers with forms for the Browsable API',
     'long_description': ":warning: Work In Progress :warning:\n\n# Writable Nested Serializers with Browsable API Forms\n\nThis plugin is intended to provide writable nested serializers (similar to [the recommended plugin from DRF documentation](https://github.com/beda-software/drf-nested-browsable.git)) that bring their own forms for the Browsable API renderer.\n\n## Try it out\n\nThis project's dependencies are managed using [`poetry`](https://python-poetry.org/)\n\n```bash\ngit clone https://github.com/pcouy/drf-nested-browsable\ncd drf-nested-browsable\npoetry install\ncd example\npython manage.py migrate\npython manage.py runserver\n```\n\nThe above commands will install the dependencies, run the DB migrations, and launch a development server of the example project that uses the provided serializers.\n\n## Current state of the project\n\n### Done\n\n* Ability to write to a reverse `ForeignKey` relationship using serializer `Meta` class\n* Dynamic form for `WritableNestedListSerializer` that allows adding and removing children from the Browsable API\n* Basic example\n\n### To do\n\n* Make the current example work :\n  * Do not show `parent` select list when showing forms as children of another form\n  * Show `details` (`HyperlinkedIdentityField`) when displayed as a child Serializer\n* Write documentation / Auto-generate it from the docstrings ([pdoc](https://pdoc.dev/) ?)\n* Write tests/specs\n",
     'author': 'Pierre Couy',
     'author_email': 'contact@pierre-couy.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pierre-couy.dev/projects/drf-nested-browsable.html',
```

### Comparing `drf_nested_browsable-0.1.2/PKG-INFO` & `drf_nested_browsable-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-nested-browsable
-Version: 0.1.2
+Version: 0.2.1
 Summary: Writable nested serializers with forms for the Browsable API
 Home-page: https://pierre-couy.dev/projects/drf-nested-browsable.html
 License: MIT
 Keywords: django,rest framework,drf,browsable api,nested serializers
 Author: Pierre Couy
 Author-email: contact@pierre-couy.dev
 Requires-Python: >=3.10,<4.0
```

