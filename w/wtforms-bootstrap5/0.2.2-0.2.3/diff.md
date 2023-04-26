# Comparing `tmp/wtforms-bootstrap5-0.2.2.tar.gz` & `tmp/wtforms-bootstrap5-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtforms-bootstrap5-0.2.2.tar", max compression
+gzip compressed data, was "wtforms-bootstrap5-0.2.3.tar", max compression
```

## Comparing `wtforms-bootstrap5-0.2.2.tar` & `wtforms-bootstrap5-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/LICENSE
--rw-r--r--   0        0        0     9454 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/README.md
--rw-r--r--   0        0        0      532 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      305 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/__init__.py
--rw-r--r--   0        0        0     6272 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/context.py
--rw-r--r--   0        0        0      805 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/helpers.py
--rw-r--r--   0        0        0     1837 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/registry.py
--rw-r--r--   0        0        0     7099 2023-04-16 05:44:19.467137 wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/renderers.py
--rw-r--r--   0        0        0    10457 2023-04-16 05:44:23.115712 wtforms-bootstrap5-0.2.2/setup.py
--rw-r--r--   0        0        0    10176 2023-04-16 05:44:23.116550 wtforms-bootstrap5-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/LICENSE
+-rw-r--r--   0        0        0     9454 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/README.md
+-rw-r--r--   0        0        0      532 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      305 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/__init__.py
+-rw-r--r--   0        0        0     6287 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/context.py
+-rw-r--r--   0        0        0      805 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/helpers.py
+-rw-r--r--   0        0        0     1837 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/registry.py
+-rw-r--r--   0        0        0     7106 2023-04-26 05:33:28.129495 wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/renderers.py
+-rw-r--r--   0        0        0    10457 2023-04-26 05:33:32.296094 wtforms-bootstrap5-0.2.3/setup.py
+-rw-r--r--   0        0        0    10176 2023-04-26 05:33:32.296905 wtforms-bootstrap5-0.2.3/PKG-INFO
```

### Comparing `wtforms-bootstrap5-0.2.2/LICENSE` & `wtforms-bootstrap5-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.2.2/README.md` & `wtforms-bootstrap5-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.2.2/pyproject.toml` & `wtforms-bootstrap5-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wtforms-bootstrap5"
-version = "0.2.2"
+version = "0.2.3"
 description = "Simple library for rendering WTForms in HTML as Bootstrap 5 form controls"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/wtforms-bootstrap5"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/context.py` & `wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,28 +123,28 @@
         self.registry = registry
         self.field_options: typing.Dict[str, FieldOptions] = {}
         self.submit_field_cls = submit_field_cls
         self.extra_fields: typing.List[UnboundField] = []
 
     def form(self, **kwargs) -> RendererContext:
         old_options = dataclasses.asdict(self.form_options)
-        self.form_options = FormOptions(**(old_options | kwargs))
+        self.form_options = FormOptions(**dict(old_options, **kwargs))
         return self
 
     def field(self, *names: str, **kwargs: str) -> RendererContext:
         for name in names:
             old_options = dataclasses.asdict(
                 self.field_options.get(name, self.default_field_options)
             )
-            self.field_options[name] = FieldOptions(**(old_options | kwargs))
+            self.field_options[name] = FieldOptions(**dict(old_options, **kwargs))
         return self
 
     def default_field(self, **kwargs: str) -> RendererContext:
         self.default_field_options = FieldOptions(
-            **(dataclasses.asdict(self.default_field_options) | kwargs)
+            **dict(dataclasses.asdict(self.default_field_options), **kwargs)
         )
         return self
 
     def add_field(self, name: str, field: UnboundField) -> RendererContext:
         self.extra_fields.append(ExtraField(name=name, field=field))
         return self
```

### Comparing `wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/helpers.py` & `wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/helpers.py`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/registry.py` & `wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/registry.py`

 * *Files identical despite different names*

### Comparing `wtforms-bootstrap5-0.2.2/wtforms_bootstrap5/renderers.py` & `wtforms-bootstrap5-0.2.3/wtforms_bootstrap5/renderers.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         base_attrs["method"] = form_options.method
     if form_options.enctype is not None:
         base_attrs["enctype"] = form_options.enctype
     return wrap_with(
         content,
         enabled=form_options.form_enabled,
         class_name=form_options.form_class,
-        attrs=base_attrs | form_options.form_attrs,
+        attrs=dict(base_attrs, **form_options.form_attrs),
         tag="form",
     )
 
 
 @register(target_cls=Field)
 def render_field(context: RendererContext, element: FormElement) -> Markup:
     field: Field = element
```

### Comparing `wtforms-bootstrap5-0.2.2/setup.py` & `wtforms-bootstrap5-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['WTForms>=3.0.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'wtforms-bootstrap5',
-    'version': '0.2.2',
+    'version': '0.2.3',
     'description': 'Simple library for rendering WTForms in HTML as Bootstrap 5 form controls',
     'long_description': '# WTForms-Bootstrap5\nSimple library for rendering WTForms in HTML as Bootstrap 5 form controls\n\n**Notice: this project is still in very early stage, the API may change a lots rapidly**\n\n## Features\n\n- **MIT licensed** - it doesn\'t infect your code\n- **Light weight** - not much code and little dependencies\n- **Latest Bootstrap 5** - generates forms in latest Bootstrap 5 style \n- **Highly customizable** - you can generate different kind of Bootstrap 5 form controls and layouts\n- **Template engine friendly** - chained method calls making it easy to integrate with template engine\n- **Covered with automatic tests** - yep, we have test cases\n\n## Why?\n\nEverytime I build a website with [WTForms](https://wtforms.readthedocs.io), I spend way too much time in writing HTML and [Jinja template](https://jinja.palletsprojects.com/) for rendering a form as [Bootstrap 5 form controls](https://getbootstrap.com/docs/5.2/forms/overview/).\nWork smart is an important value we have here at [Launch Platform](https://launchplatform.com), so I wonder why not make a library for making rendering Bootstrap 5 style WTForms controls easily?\nSo here you go, wtforms-bootstrap5 is created, open sourced under MIT license.\nIt\'s a simple Python library for rendering WTForms in Bootstrap 5 favor.\n\n## Install\n\nTo install the formatter, simply run\n\n```bash\npip install wtforms-bootstrap5\n```\n\n## Example\n\nFirst, you define your form as you would usually do with WTForms:\n\n```python\nfrom wtforms import Form\nfrom wtforms import EmailField\nfrom wtforms import PasswordField\nfrom wtforms import SelectField\nfrom wtforms import BooleanField\nfrom wtforms import SubmitField\n\n\nclass MyForm(Form):\n    email = EmailField("Email", render_kw=dict(placeholder="Foobar"))\n    password = PasswordField("Password", description="Your super secret password")\n    city = SelectField("City", choices=["Los Angle", "San Francisco", "New York"])\n    agree_terms = BooleanField("I agrees to terms and service")\n    submit = SubmitField()\n\n```\n\nThen you can use `RenderContext` for rendering your form like this\n\n```python\nfrom wtforms_bootstrap5 import RendererContext\n\nform = MyForm()\ncontext = RendererContext()\nhtml = context.render(form)\n```\n\nThe form will be rendered as HTML like\n\n```html\n<form method="POST"><div class="mb-3"><label class="form-label" for="email">Email</label><input class="form-control" id="email" name="email" type="email" value=""></div>\n<div class="mb-3"><label class="form-label" for="password">Password</label><input class="form-control" id="password" name="password" type="password" value=""><div class="form-text">Your super secret password</div></div>\n<div class="mb-3"><label class="form-label" for="city">City</label><select class="form-select" id="city" name="city"><option value="Los Angle">Los Angle</option><option value="San Francisco">San Francisco</option><option value="New York">New York</option></select></div>\n<div class="mb-3"><div class="form-check"><label class="form-check-label" for="agree_terms">I agrees to terms and service</label><input class="form-check-input" id="agree_terms" name="agree_terms" type="checkbox" value="y"></div></div>\n<div class="mb-3"><input class="btn btn-primary" id="submit" name="submit" type="submit" value="Submit"></div></form>\n```\n\nAnd it will look like this\n\n<p align="center">\n  <img src="assets/default-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nBy default, a sensible simple layout style will be used.\n\n## Customize the form\n\nThere are many similar open source libraries out there, but most of them are very hard to customize.\nOnce you adopt it, then you can only render your form in a specific style.\nAs a result, I found myself writing HTML manually without using the library to save time.\n\nTo avoid the same mistake, we want to make wtforms-bootstrap5 very easy to customize without compromising too much of its reusability.\nHere\'s an example how you can turn the example above into a column based form.\n\n```python\nhtml = (\n    renderer_context\n    .form(action="/sign-up")\n    .default_field(\n        row_class="row mb-3",\n        label_class="form-label col-2",\n        field_wrapper_class="col-10",\n        field_wrapper_enabled=True,\n    )\n    .field(\n        "agree_terms",\n        wrapper_class="offset-2",\n        wrapper_enabled=True,\n        field_wrapper_enabled=False,\n    )\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nAnd this is how it looks like\n\n<p align="center">\n  <img src="assets/column-style-example.png?raw=true" alt="Form rendered in Bootstrap 5 favor" />\n</p>\n\nAs you can see in the example, we use `default_field` method for overwriting the options of all fields by default.\nWe also use `field` method for overwriting the options for a specific field.\nThe `field` method takes multiple input name arguments, so that you can overwrite options for multiple fields at once like this\n\n```python\nhtml = (context\n    .field("email", "password", label_class="my-custom-class", ...)\n)\n```\n\nPlease notice that, **the order of `default_field` and `field` method calls matter**.\nWhen `field` is called, the current default field options will be used as the default values.\nSo if you make the calls in order like this\n\n```python\nhtml = (context\n    .field("email", row_class="row")\n    .default_field(label_class="my-custom-class")\n)\n```\n\nThe `label_class` for `email` field here will be `form-label` instead of `my-custom-class` since when it\'s called, the original default value was still `form-label`.\n\nTo customize the form element, you can use the `form` method like this\n\n```python\nhtml = (context\n    .form(\n        method="POST",\n        action="/sign-up",\n        enctype="application/x-www-form-urlencoded",\n        form_class="my-form",\n        form_attrs=dict(custom="value")\n    )\n)\n```\n\n### Add submit button or other fields\n\nSometimes, define a submit button for each form is not desirable.\nOr, the form could be automatically generated and doesn\'t come with a submit button.\nIn those cases, you can use `add_field` to add any extra fields into the end of the form.\nLike this:\n\n```python\nhtml = (\n    renderer_context\n    .add_field("submit", SubmitField())\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nSince adding a submit button is very common, so you can also use `add_submit` instead if the field to add is a `SubmitField`.\nThe default submit field name is `submit`, so you don\'t need to provide it if you want to make it `submit`.\nArguments of `SubmitField` can be passed in, such as `label`.\n\n```python\nhtml = (\n    renderer_context\n    .add_submit(label="Update")\n    .field(\n        "submit",\n        field_wrapper_class="offset-2",\n        field_wrapper_enabled=True,\n    )\n).render(form)\n```\n\nAs you can see in the example, the decorate options also work for the newly added submit field.\nIf you want to change the default submit field class, you can pass in `submit_field_cls` argument when creating the context like this.\n\n```python\nhtml = (\n    RenderContext(submit_field_cls=SubmitButton)\n    .add_submit()\n).render(form)\n```\n\n### Field HTML structure\n\nIn general, the field HTML structure can be controlled by the option values and it looks like this\n\n```html\n<!-- enabled by .row_enabled, default: true -->\n<div class=".row_class" {.row_attrs}>\n  <!-- enabled by .wrapper_enabled, default: false -->\n  <div class=".wrapper_class" {.wrapper_attrs}>\n    <!-- enabled by .label_enabled, default: true -->\n    <label class=".label_class" for="email" {.label_attrs}>Email</label>\n    <!-- enabled by .field_wrapper_enabled, default: false -->\n    <div class=".field_wrapper" {.field_wrapper_attrs}>\n      <input class=".field_class" id="email" name="email" type="email" value="" {.field_attrs}>\n      <!-- enabled by .help_enabled, default: true -->\n      <div class=".help_class" {.helper_attrs}>Your super secret password</div>\n      <!-- enabled by .error_enabled, default: true -->\n      <div class=".error_class" {.error_attrs}>Bad password</div>\n    </div>\n  </div>\n</div>\n```\n\n## Integrate with template engine\n\nWe want to make it as easy as possible to integrate with template engine such as [Jinja](https://jinja.palletsprojects.com/).\nThat\'s why we use chained method calls for customizing the form.\nYou should be able to pass the `form` and `RenderContext` objects and write all your form customization from the template.\nThis way, you don\'t get your view relative code pollute your controller code.\nFor example, after passing `form` and `render_context` object, you can write this in Jinja:\n\n```html\n<h1>New user</h1>\n\n{{\n    renderer_context\n        .default_field(\n            row_class="row mb-3",\n            label_class="form-label col-2",\n            field_wrapper_class="col-10",\n            field_wrapper_enabled=True,\n        )\n        .field(\n            "agree_terms",\n            wrapper_class="offset-2",\n            wrapper_enabled=True,\n            field_wrapper_enabled=False,\n        )\n        .field(\n            "submit",\n            field_wrapper_class="offset-2",\n            field_wrapper_enabled=True,\n        )\n    ).render(form)\n}}\n```\n\n## Feedbacks\n\nFeedbacks, bugs reporting or feature requests are welcome 🙌, just please open an issue.\nNo guarantee we have time to deal with them, but will see what we can do.\n',
     'author': 'Fang-Pen Lin',
     'author_email': 'fangpen@launchplatform.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/LaunchPlatform/wtforms-bootstrap5',
```

### Comparing `wtforms-bootstrap5-0.2.2/PKG-INFO` & `wtforms-bootstrap5-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtforms-bootstrap5
-Version: 0.2.2
+Version: 0.2.3
 Summary: Simple library for rendering WTForms in HTML as Bootstrap 5 form controls
 Home-page: https://github.com/LaunchPlatform/wtforms-bootstrap5
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

