# Comparing `tmp/ipyautoui-0.5.1.tar.gz` & `tmp/ipyautoui-0.5.2.tar.gz`

## Comparing `ipyautoui-0.5.1.tar` & `ipyautoui-0.5.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_dev_sys_path_append.py
--rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_utils.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_utils_debounce.py
--rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/_version.py
--rw-r--r--   0        0        0    31429 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autodisplay.py
--rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autodisplay_renderers.py
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autoipywidget.py
--rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/automapschema.py
--rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autoui.py
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autovjsf.py
--rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/autowidgets.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/basemodel.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/constants.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/env.py
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/mydocstring_display.py
--rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/test_schema.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/vjsf.vue
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/__init__.py
--rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/autogrid.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/buttonbars.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/decision_branch.py
--rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/editgrid.py
--rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/filechooser.py
--rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/filesindir.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/fileupload.py
--rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/iterable.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/loadproject.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/markdown_widget.py
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/modelrun.py
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/multiselect_search.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/outputlogging.py
--rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/selectdir.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/showhide.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/title_description.py
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/urlimagelink.py
--rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/widgetcaller_error.py
--rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/custom/workingdir.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/__init__.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/complex_serialization.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/core_ipywidgets.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/editable_datagrid.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/override_ipywidgets.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array_enum.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_enum.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_simple.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/src/ipyautoui/demo_schemas/ruleset.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/LICENSE
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/README.md
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_dev_sys_path_append.py
+-rw-r--r--   0        0        0    13120 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_utils.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_utils_debounce.py
+-rw-r--r--   0        0        0    18450 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/_version.py
+-rw-r--r--   0        0        0    31684 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autodisplay.py
+-rw-r--r--   0        0        0    14138 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autodisplay_renderers.py
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autoipywidget.py
+-rw-r--r--   0        0        0    21441 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/automapschema.py
+-rw-r--r--   0        0        0    12894 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autoui.py
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autovjsf.py
+-rw-r--r--   0        0        0    14967 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/autowidgets.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/basemodel.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/constants.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/env.py
+-rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/mydocstring_display.py
+-rw-r--r--   0        0        0     7425 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/test_schema.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/vjsf.vue
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/__init__.py
+-rw-r--r--   0        0        0    40881 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/autogrid.py
+-rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/buttonbars.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/decision_branch.py
+-rw-r--r--   0        0        0    25164 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/editgrid.py
+-rw-r--r--   0        0        0     3393 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/filechooser.py
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/filesindir.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/fileupload.py
+-rw-r--r--   0        0        0    30632 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/iterable.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/loadproject.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/markdown_widget.py
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/modelrun.py
+-rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/multiselect_search.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/outputlogging.py
+-rw-r--r--   0        0        0     8598 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/selectdir.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/showhide.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/showopenurl.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/title_description.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/urlimagelink.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/widgetcaller_error.py
+-rw-r--r--   0        0        0    12975 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/custom/workingdir.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/__init__.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/complex_serialization.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/core_ipywidgets.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/editable_datagrid.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested_editable_datagrid.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/override_ipywidgets.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array_enum.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_enum.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_simple.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/src/ipyautoui/demo_schemas/ruleset.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/README.md
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     8582 2020-02-02 00:00:00.000000 ipyautoui-0.5.2/PKG-INFO
```

### Comparing `ipyautoui-0.5.1/src/ipyautoui/__init__.py` & `ipyautoui-0.5.2/src/ipyautoui/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/_dev_sys_path_append.py` & `ipyautoui-0.5.2/src/ipyautoui/_dev_sys_path_append.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/_utils.py` & `ipyautoui-0.5.2/src/ipyautoui/_utils.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/_utils_debounce.py` & `ipyautoui-0.5.2/src/ipyautoui/_utils_debounce.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/_version.py` & `ipyautoui-0.5.2/src/ipyautoui/_version.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autodisplay.py` & `ipyautoui-0.5.2/src/ipyautoui/autodisplay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # -*- coding: utf-8 -*-
 # ---
 # jupyter:
 #   jupytext:
-#     formats: py:light
+#     custom_cell_magics: kql
+#     formats: py:percent
 #     text_representation:
 #       extension: .py
-#       format_name: light
-#       format_version: '1.5'
+#       format_name: percent
+#       format_version: '1.3'
 #       jupytext_version: 1.14.0
 #   kernelspec:
 #     display_name: Python 3 (ipykernel)
 #     language: python
 #     name: python3
 # ---
 
+# %%
 """
 displayfile is used to display certain types of files.
 The module lets us preview a file, open a file, and open its directory.
 
 Example:
     ::#
 
@@ -34,15 +36,15 @@
         display(d)
 
 """
 # %run _dev_sys_path_append.py
 # %run __init__.py
 # %load_ext lab_black
 
-# +
+# %%
 import pathlib
 import functools
 from IPython.display import (
     display,
     clear_output,
     Markdown,
 )
@@ -80,37 +82,36 @@
 # from mf library
 # try:
 #     from xlsxtemplater import from_excel
 # except:
 #     pass
 
 
-# -
-
-
+# %%
 def merge_default_renderers(
     renderers: dict[str, ty.Callable],
     default_renderers: frozenmap[str, ty.Callable] = DEFAULT_FILE_RENDERERS,
 ) -> dict[str, ty.Callable]:
     return {**dict(default_renderers), **renderers}
 
 
+# %%
 def get_renderers(
     renderers: ty.Optional[dict[str, ty.Callable]],
     extend_default_renderers: bool = True,
 ) -> dict[str, ty.Callable]:
     if renderers is None and not extend_default_renderers:
         raise ValueError("renderers must be given if extend_default_renderers is False")
     if renderers is not None and extend_default_renderers:
         return merge_default_renderers(renderers)
     else:
         return dict(DEFAULT_FILE_RENDERERS)
 
 
-# +
+# %%
 class DisplayObjectActions(BaseModel):
     """base object with callables for creating a display object"""
 
     renderers: dict[str, ty.Callable] = dict(DEFAULT_FILE_RENDERERS)
     path: ty.Union[str, pathlib.Path, HttpUrl, ty.Callable]
     ext: str = None
     name: str = None
@@ -267,21 +268,20 @@
     def _name(cls, v, values):
         if v is not None:
             return v
         else:
             return values["path"].__name__
 
 
-# -
-
+# %%
 if __name__ == "__main__":
     d = DisplayFromPath(path="__init__.py")
     display(d.renderer())
 
-# +
+# %%
 # TODO: separate out the bit that is display data and display from path...
 # TODO: probs useful to have a `value` trait (allowing the object to be updated instead of remade)
 #       this probably means having DisplayObject as a base class and extending it for display file...
 
 ORDER_DEFAULT = ("exists", "openpreview", "openfile", "openfolder", "name")
 ORDER_NOTPATH = ("exists", "openpreview", "name")
 
@@ -341,110 +341,54 @@
             display_actions (ty.Type[DisplayObjectActions]): actions used to display object
             auto_open (bool, optional): automatically display object data (i.e. auto-preview file). Defaults to False.
             order (tuple, optional): defines UI controls appearance. Defaults to None.
                 allowed values are: ("exists", "openpreview", "openfile", "openfolder", "name")
                 default is: ("exists", "openpreview", "openfile", "openfolder", "name")
                 reduce tuple to hide components
         """
-
         self._init_form()  # generic form only
         self._init_controls()
         super().__init__(display_actions=display_actions, **kwargs)
         self._update_bx_bar(self.order)
         self.children = [self.bx_bar, self.bx_out]
 
     def _update_bx_bar(self, order):
-        self.bx_bar.children = [getattr(self, l) for l in order]
-
-    @classmethod
-    def from_path(
-        cls,
-        path,
-        renderers=None,
-        extend_default_renderers=True,
-        auto_open=False,
-    ):
-        renderers = get_renderers(
-            renderers=renderers, extend_default_renderers=extend_default_renderers
-        )
-        display_actions = DisplayFromPath(path=path, renderers=renderers)
-        return cls(display_actions=display_actions, auto_open=auto_open)
-
-    @classmethod
-    def from_request(
-        cls,
-        path,
-        ext,
-        renderers=None,
-        extend_default_renderers=True,
-        auto_open=False,
-    ):
-        renderers = get_renderers(
-            renderers=renderers, extend_default_renderers=extend_default_renderers
-        )
-        display_actions = DisplayFromRequest(path=path, ext=ext, renderers=renderers)
-        return cls(display_actions=display_actions, auto_open=auto_open)
-
-    @classmethod
-    def from_callable(
-        cls,
-        path,
-        ext,
-        renderers=None,
-        extend_default_renderers=True,
-        auto_open=False,
-    ):
-        renderers = get_renderers(
-            renderers=renderers, extend_default_renderers=extend_default_renderers
-        )
-        display_actions = DisplayFromCallable(path=path, ext=ext, renderers=renderers)
-        return cls(display_actions=display_actions, auto_open=auto_open)
-
-    def tooltip_openpath(self, path):
-        return str(make_new_path(path))
+        li = []
+        for l in order:
+            try:
+                li.append(getattr(self, l))
+            except:
+                pass
+        self.bx_bar.children = li
 
     def _init_form(self):
         self.exists = w.Valid(
             value=False,
             disabled=True,
             readout="-",
             tooltip="indicates if file exists",
             layout=w.Layout(width="20px", height=BUTTON_HEIGHT_MIN),
         )
         self.openpreview = w.ToggleButton(**KWARGS_OPENPREVIEW)
-        self.openfile = w.Button(**KWARGS_OPENFILE)
-        self.openfolder = w.Button(**KWARGS_OPENFOLDER)
         self.name = w.HTML(
             layout=w.Layout(justify_items="center"),
         )
         self.out_caller = w.Output()
         self.out = w.Output()
         self.out_caller.layout.display = "none"
         self.out.layout.display = "none"
         self.bx_bar = w.HBox()
-
         self.bx_out = w.VBox()
         self.bx_out.children = [self.out_caller, self.out]
 
     def _update_form(self):
-        if isinstance(self.display_actions.path, pathlib.PurePath):
-            self.openfile.tooltip = f"""
-open file:
-{self.tooltip_openpath(self.display_actions.path)}
-"""
-            self.openfolder.tooltip = f"""
-open folder:
-{self.tooltip_openpath(self.display_actions.path.parent)}
-"""
         self.name.value = "<b>{0}</b>".format(self.display_actions.name)
         self.check_exists()
 
     def _init_controls(self):
-        self.openfile.on_click(self._openfile)
-        self.openfolder.on_click(self._openfolder)
         self.openpreview.observe(self._openpreview, names="value")
 
     def check_exists(self):
         if self.display_actions.check_exists is None:
             self.exists.value = False
         elif not self.display_actions.check_exists():
             self.exists.value = False
@@ -468,98 +412,167 @@
                     display(Markdown("file does not exist"))
         else:
             self.openpreview.icon = "eye"
             self.out.layout.display = "none"
             with self.out:
                 clear_output()
 
-    def _openfile(self, sender):
-        self.out_caller.layout.display = ""
-        with self.out_caller:
-            clear_output()
-            self.display_actions.open_file()
-            time.sleep(5)
-            clear_output()
-        self.out_caller.layout.display = "none"
 
-    def _openfolder(self, sender):
-        self.out_caller.layout.display = ""
-        with self.out_caller:
-            clear_output()
-            self.display_actions.open_folder()
-            time.sleep(5)
-            clear_output()
-        self.out_caller.layout.display = "none"
+class DisplayCallable(DisplayObject):
+    def __init__(
+        self,
+        value,
+        ext,
+        renderers=None,
+        extend_default_renderers=True,
+        **kwargs,
+    ):
+
+        renderers = get_renderers(
+            renderers=renderers, extend_default_renderers=extend_default_renderers
+        )
+        display_actions = DisplayFromCallable(path=value, ext=ext, renderers=renderers)
+        super().__init__(display_actions=display_actions, **kwargs)
+
+
+class DisplayRequest(DisplayObject):
+    def __init__(
+        self,
+        value,
+        ext,
+        renderers=None,
+        extend_default_renderers=True,
+        **kwargs,
+    ):
+
+        renderers = get_renderers(
+            renderers=renderers, extend_default_renderers=extend_default_renderers
+        )
+        display_actions = DisplayFromRequest(path=path, ext=ext, renderers=renderers)
+        super().__init__(display_actions=display_actions, **kwargs)
 
 
 class DisplayPath(DisplayObject):
     _value = tr.Unicode(default_value="")
 
+    @tr.default("order")
+    def _default_order(self):
+        return ORDER_DEFAULT
+
     def __init__(
         self,
         value,
         renderers=None,
         extend_default_renderers=True,
         **kwargs,
     ):
         self.renderers = get_renderers(
             renderers=renderers, extend_default_renderers=extend_default_renderers
         )
         display_actions = DisplayFromPath(path=value, renderers=self.renderers)
+        self._update_form_DisplayPath()
         super().__init__(display_actions=display_actions, **kwargs)
+        self._init_controls_DisplayPath()
+        self._update_path_tooltips()
+
+    def _update_form_DisplayPath(self):
+        self.openfile = w.Button(**KWARGS_OPENFILE)
+        self.openfolder = w.Button(**KWARGS_OPENFOLDER)
+
+    def _update_path_tooltips(self):
+        new_path = lambda path: str(make_new_path(path))
+        if isinstance(self.display_actions.path, pathlib.PurePath):
+            self.openfile.tooltip = f"""
+open file:
+{new_path(self.display_actions.path)}
+"""
+            self.openfolder.tooltip = f"""
+open folder:
+{new_path(self.display_actions.path.parent)}
+"""
+
+    def _init_controls_DisplayPath(self):
+        self.openfile.on_click(self._openfile)
+        self.openfolder.on_click(self._openfolder)
+
+    @property
+    def path(self):
+        return pathlib.Path(self.value)
+
+    @path.setter
+    def path(self, value):
+        self.value = str(value)
 
     @property
     def value(self):
         return self._value
 
     @value.setter
     def value(self, value):
-        self._value = ""
         self.display_actions = DisplayFromPath(path=value, renderers=self.renderers)
 
+    def _openfile(self, sender):
+        self.out_caller.layout.display = ""
+        with self.out_caller:
+            clear_output()
+            self.display_actions.open_file()
+            time.sleep(5)
+            clear_output()
+        self.out_caller.layout.display = "none"
 
-# -
+    def _openfolder(self, sender):
+        self.out_caller.layout.display = ""
+        with self.out_caller:
+            clear_output()
+            self.display_actions.open_folder()
+            time.sleep(5)
+            clear_output()
+        self.out_caller.layout.display = "none"
+# %%
 if __name__ == "__main__":
     d = DisplayFromPath(path="__init__.py")
     do = DisplayObject(d)
     display(do)
 
-# +
-# from maplocal import maplocal
-
-# maplocal(pathlib.Path("__init__.py"))
-# -
+# %%
+if __name__ == "__main__":
+    DisplayPath(value="__init__.py")
 
+# %%
 if __name__ == "__main__":
     path = "https://catfact.ninja/fact"
     ext = ".json"
     display(DisplayFromRequest(path=path, ext=ext).renderer())
 
 
+# %%
 if __name__ == "__main__":
     path = "https://catfact.ninja/fact"
     ext = ".json"
 
     def get_catfact():
         return requests.get(path).content
 
     display(DisplayFromCallable(path=get_catfact, ext=ext).renderer())
 
+# %%
 if __name__ == "__main__":
 
     path = "https://catfact.ninja/fact"
     ext = ".json"
-    display(DisplayObject.from_request(path=path, ext=ext))
+    display(DisplayRequest(value=path, ext=ext, order=ORDER_DEFAULT))
 
+# %%
 if __name__ == "__main__":
 
     ext = ".json"
-    dobj = DisplayObject.from_callable(path=get_catfact, ext=ext)
+    dobj = DisplayCallable(value=get_catfact, ext=ext)
     display(dobj)
 
+# %%
 if __name__ == "__main__":
     import json
     from datetime import datetime
 
     def display_catfact(path):
         if callable(path):
             di = json.loads(path())
@@ -571,60 +584,61 @@
 {di['fact']}
 
 *{datetime.now().strftime("%Y-%m-%d, %H:%M:%S")} - https://cat-fact.herokuapp.com/#/*"""
         return Markdown(s)
 
     path = "https://catfact.ninja/fact"
     ext = ".catfact"
-    d = DisplayObject.from_request(
-        path=path, ext=ext, renderers={".catfact": display_catfact}
-    )
+    d = DisplayRequest(value=path, ext=ext, renderers={".catfact": display_catfact})
     display(d)
 
+# %%
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
     from ipyautoui.autoui import AutoUi
     from ipyautoui.constants import load_test_constants
 
     tests_constants = load_test_constants()
     DIR_FILETYPES = load_test_constants().DIR_FILETYPES
     paths = list(pathlib.Path(DIR_FILETYPES).glob("*"))
     path = paths[6]
-    d = DisplayObject.from_path(path)
+    d = DisplayPath(path)
     display(d)
     # ------------------
 
 
-if __name__ == "__main__":
-    d1 = DisplayPath(path)
-    display(d1)
-
+# %%
 if __name__ == "__main__":
     d.order = (
         "openpreview",
         "name",
     )
     d.auto_open = True
 
+# %%
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
 
     user_file_renderers = AutoUi.create_autodisplay_map(
         ext=".aui.json", schema=TestAutoLogic
     )
     path1 = tests_constants.PATH_TEST_AUI
 
-    d = DisplayObject.from_path(path1, renderers=user_file_renderers)
+    d = DisplayPath(path1, renderers=user_file_renderers)
     d.order = ORDER_DEFAULT
     display(d)
 
-# +
-
 
+# %%
 class AutoDisplay(tr.HasTraits):
+    order = tr.Tuple(default_value=ORDER_NOTPATH, allow_none=False)
+    
+    @tr.observe("order")
+    def _observe_order(self, change):
+        self._update_bx_bar(change["new"])
     """
     displays the contents of a file in the notebook.
     comes with the following default renderers:
     DEFAULT_FILE_RENDERERS = {
         '.csv': csv_prev,
         '.json': json_prev,
         '.plotly': plotlyjson_prev,
@@ -667,15 +681,14 @@
 
 
         """
         self._init_form()
         self._init_controls()
         self.title = title
         self._display_objects_actions = display_objects_actions
-
         self.display_objects_actions = display_objects_actions
         self.display_showhide = display_showhide
         self.patterns = patterns
 
     @classmethod
     def from_paths(
         cls,
@@ -965,31 +978,32 @@
     def _activate_waiting(self):
         [d._activate_waiting() for d in self.display_objects]
 
     def _update_files(self):
         [d._update_file() for d in self.display_objects]
 
 
-# +
+# %%
 # TODO: render pdf update the relative path
 
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
     from ipyautoui.autoui import AutoUi
     from ipyautoui.constants import load_test_constants
 
     tests_constants = load_test_constants()
     DIR_FILETYPES = load_test_constants().DIR_FILETYPES
     paths = list(pathlib.Path(DIR_FILETYPES).glob("*"))
     ad = AutoDisplay.from_paths(paths, patterns="*.csv")
     display(ad)
-# -
+# %%
 if __name__ == "__main__":
     ad.order = ORDER_DEFAULT
 
+# %%
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
 
     user_file_renderers = AutoUi.create_autodisplay_map(
         ext=".aui.json", schema=TestAutoLogic
     )
 
@@ -997,28 +1011,30 @@
         paths=[tests_constants.PATH_TEST_AUI],
         renderers=user_file_renderers,
         display_showhide=False,
     )
 
     display(test_ui)
 
+# %%
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
 
     test_ui = AutoDisplay.from_requests(
         map_requests={
             ".catfact": "https://catfact.ninja/fact",
             ".json": "https://official-joke-api.appspot.com/random_joke",
         },
         renderers={".catfact": display_catfact},
         display_showhide=False,
     )
 
     display(test_ui)
 
+# %%
 if __name__ == "__main__":
     from ipyautoui.test_schema import TestAutoLogic
     from pydantic import parse_obj_as
 
     test_ui = AutoDisplay.from_any(
         paths=[
             {".catfact": parse_obj_as(HttpUrl, "https://catfact.ninja/fact")},
@@ -1028,14 +1044,15 @@
         renderers={".catfact": display_catfact},
         display_showhide=False,
         patterns="get_catfact",
     )
 
     display(test_ui)
 
+# %%
 if __name__ == "__main__":
     import json
     from datetime import datetime
 
     def display_catfact(path):
         di = json.loads(requests.get(path).content)
         s = f"""
@@ -1053,7 +1070,9 @@
     path = "https://official-joke-api.appspot.com/random_joke"
     ext = ".json"
     d2 = DisplayFromRequest(path=path, ext=ext)
 
     test_display = AutoDisplay([d1, d2])
     display(Markdown("### From requests: "))
     display(test_display)
+
+# %%
```

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autodisplay_renderers.py` & `ipyautoui-0.5.2/src/ipyautoui/autodisplay_renderers.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autoipywidget.py` & `ipyautoui-0.5.2/src/ipyautoui/autoipywidget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/automapschema.py` & `ipyautoui-0.5.2/src/ipyautoui/automapschema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autoui.py` & `ipyautoui-0.5.2/src/ipyautoui/autoui.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autovjsf.py` & `ipyautoui-0.5.2/src/ipyautoui/autovjsf.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/autowidgets.py` & `ipyautoui-0.5.2/src/ipyautoui/autowidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/basemodel.py` & `ipyautoui-0.5.2/src/ipyautoui/basemodel.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/constants.py` & `ipyautoui-0.5.2/src/ipyautoui/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     tooltip="open folder in file-browser",
     style={"font_weight": "bold"},  # , "button_color": OPEN_BN_COLOR},
 )
 
 KWARGS_DISPLAY = frozenmap(
     icon="plus",
     tooltip="display all files",
-    layout={"width": BUTTON_WIDTH_MIN, "height": BUTTON_HEIGHT_MIN},
+    layout={"width": BUTTON_WIDTH_MIN},  # , "height": BUTTON_HEIGHT_MIN
     disabled=False,
 )
 KWARGS_DISPLAY_ALL_FILES = frozenmap(
     {**dict(KWARGS_DISPLAY), **{"tooltip": "display all files"}}
 )
 
 KWARGS_COLLAPSE = frozenmap(
```

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo.py` & `ipyautoui-0.5.2/src/ipyautoui/demo.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/env.py` & `ipyautoui-0.5.2/src/ipyautoui/env.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/mydocstring_display.py` & `ipyautoui-0.5.2/src/ipyautoui/mydocstring_display.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/test_schema.py` & `ipyautoui-0.5.2/src/ipyautoui/test_schema.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/vjsf.vue` & `ipyautoui-0.5.2/src/ipyautoui/vjsf.vue`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/autogrid.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/autogrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/buttonbars.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/buttonbars.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/decision_branch.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/decision_branch.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/editgrid.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/editgrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/filechooser.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/filechooser.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/filesindir.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/filesindir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/fileupload.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/fileupload.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/iterable.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/iterable.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/loadproject.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/loadproject.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/markdown_widget.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/markdown_widget.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/modelrun.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/modelrun.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/multiselect_search.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/multiselect_search.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/outputlogging.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/outputlogging.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/selectdir.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/selectdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/showhide.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/showhide.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/title_description.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/title_description.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/urlimagelink.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/urlimagelink.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/widgetcaller_error.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/widgetcaller_error.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/custom/workingdir.py` & `ipyautoui-0.5.2/src/ipyautoui/custom/workingdir.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/__init__.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/complex_serialization.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/complex_serialization.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/core_ipywidgets.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/editable_datagrid.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nested_editable_datagrid.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nested_editable_datagrid.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/nullable_core_ipywidgets.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_array_enum.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_array_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/root_enum.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/root_enum.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/src/ipyautoui/demo_schemas/ruleset.py` & `ipyautoui-0.5.2/src/ipyautoui/demo_schemas/ruleset.py`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/.gitignore` & `ipyautoui-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/LICENSE` & `ipyautoui-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/README.md` & `ipyautoui-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/pyproject.toml` & `ipyautoui-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ipyautoui-0.5.1/PKG-INFO` & `ipyautoui-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyautoui
-Version: 0.5.1
+Version: 0.5.2
 Summary: wrapper that sits on top of ipywidgets and other ipy widget libraries to template / automate the creation of widget forms. Uses pydantic to create defined data-container and serialisation to JSON. Includes example patterns for adding new custom widgets.
 Project-URL: Homepage, https://github.com/maxfordham/ipyautoui
 Author-email: John Gunstone <gunstone.john@gmail.com>
 License-File: LICENSE
 Keywords: ipyautoui
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

