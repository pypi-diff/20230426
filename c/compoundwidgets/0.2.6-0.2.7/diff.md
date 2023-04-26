# Comparing `tmp/compoundwidgets-0.2.6.tar.gz` & `tmp/compoundwidgets-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compoundwidgets-0.2.6.tar", last modified: Fri Apr 21 14:46:26 2023, max compression
+gzip compressed data, was "compoundwidgets-0.2.7.tar", last modified: Wed Apr 26 10:08:27 2023, max compression
```

## Comparing `compoundwidgets-0.2.6.tar` & `compoundwidgets-0.2.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.899505 compoundwidgets-0.2.6/
--rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      332 2023-04-21 14:46:26.898505 compoundwidgets-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.781096 compoundwidgets-0.2.6/compoundwidgets/
--rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
--rw-rw-rw-   0        0        0    54563 2023-04-21 14:44:57.000000 compoundwidgets-0.2.6/compoundwidgets/COMPOUND_WIDGETS.py
--rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/CUSTOM_BUTTONS.py
--rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.6/compoundwidgets/CUSTOM_FRAMES.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.830821 compoundwidgets-0.2.6/compoundwidgets/IMAGES/
--rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/__init__.py
--rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_new.png
--rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_to_form.png
--rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/back.png
--rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/calculate.png
--rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/clear.png
--rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/edit_form.png
--rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/help.png
--rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/no.png
--rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/quit.png
--rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/remove_from_form.png
--rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/save.png
--rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/trash_can.png
--rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.6/compoundwidgets/IMAGES/yes.png
--rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.6/compoundwidgets/LED_BUTTONS.py
--rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.6/compoundwidgets/MESSAGE_BOX_WIDGETS.py
--rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.6/compoundwidgets/SCRIPTS.py
--rw-rw-rw-   0        0        0     1843 2023-04-21 14:46:23.000000 compoundwidgets-0.2.6/compoundwidgets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.798107 compoundwidgets-0.2.6/compoundwidgets.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-21 14:46:26.000000 compoundwidgets-0.2.6/compoundwidgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 14:46:26.900504 compoundwidgets-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      576 2023-04-21 14:46:23.000000 compoundwidgets-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:46:26.897490 compoundwidgets-0.2.6/test/
--rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.6/test/autocomplete_widget_test.py
--rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.6/test/compound_widgets_test_1.py
--rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.6/test/compound_widgets_test_2.py
--rw-rw-rw-   0        0        0      981 2023-04-07 20:22:34.000000 compoundwidgets-0.2.6/test/custom_buttons_test.py
--rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.6/test/custom_frames_test_1.py
--rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.6/test/custom_frames_test_2.py
--rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.6/test/custom_frames_test_3.py
--rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.6/test/custom_frames_test_4.py
--rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.6/test/led_buttons_test.py
--rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.6/test/message_box_test.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.503050 compoundwidgets-0.2.7/
+-rw-rw-rw-   0        0        0     1062 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0      538 2023-03-10 20:29:07.000000 compoundwidgets-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      332 2023-04-26 10:08:27.502051 compoundwidgets-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1161 2023-04-21 13:55:20.000000 compoundwidgets-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.369835 compoundwidgets-0.2.7/compoundwidgets/
+-rw-rw-rw-   0        0        0     7179 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/AUTOCOMPLETE_WIDGETS.py
+-rw-rw-rw-   0        0        0    54792 2023-04-26 10:05:01.000000 compoundwidgets-0.2.7/compoundwidgets/COMPOUND_WIDGETS.py
+-rw-rw-rw-   0        0        0     7766 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/CUSTOM_BUTTONS.py
+-rw-rw-rw-   0        0        0    16474 2023-04-17 20:34:54.000000 compoundwidgets-0.2.7/compoundwidgets/CUSTOM_FRAMES.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.436095 compoundwidgets-0.2.7/compoundwidgets/IMAGES/
+-rw-rw-rw-   0        0        0        0 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/__init__.py
+-rw-rw-rw-   0        0        0     3203 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_new.png
+-rw-rw-rw-   0        0        0     7038 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_to_form.png
+-rw-rw-rw-   0        0        0    56482 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/back.png
+-rw-rw-rw-   0        0        0    14398 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/calculate.png
+-rw-rw-rw-   0        0        0     7680 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/clear.png
+-rw-rw-rw-   0        0        0     4075 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/edit_form.png
+-rw-rw-rw-   0        0        0    17569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/help.png
+-rw-rw-rw-   0        0        0    20256 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/no.png
+-rw-rw-rw-   0        0        0    13946 2023-03-06 16:15:17.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/quit.png
+-rw-rw-rw-   0        0        0     6569 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/remove_from_form.png
+-rw-rw-rw-   0        0        0     4873 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/save.png
+-rw-rw-rw-   0        0        0     8180 2022-11-25 10:54:32.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/trash_can.png
+-rw-rw-rw-   0        0        0     5433 2023-04-07 20:00:14.000000 compoundwidgets-0.2.7/compoundwidgets/IMAGES/yes.png
+-rw-rw-rw-   0        0        0    15883 2023-04-12 10:10:39.000000 compoundwidgets-0.2.7/compoundwidgets/LED_BUTTONS.py
+-rw-rw-rw-   0        0        0    15192 2023-04-12 13:54:57.000000 compoundwidgets-0.2.7/compoundwidgets/MESSAGE_BOX_WIDGETS.py
+-rw-rw-rw-   0        0        0     2272 2023-04-12 10:28:05.000000 compoundwidgets-0.2.7/compoundwidgets/SCRIPTS.py
+-rw-rw-rw-   0        0        0     1843 2023-04-26 10:08:19.000000 compoundwidgets-0.2.7/compoundwidgets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.411755 compoundwidgets-0.2.7/compoundwidgets.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-26 10:08:27.000000 compoundwidgets-0.2.7/compoundwidgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 10:08:27.503050 compoundwidgets-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      576 2023-04-26 10:08:19.000000 compoundwidgets-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 10:08:27.501052 compoundwidgets-0.2.7/test/
+-rw-rw-rw-   0        0        0     2815 2023-04-07 11:49:55.000000 compoundwidgets-0.2.7/test/autocomplete_widget_test.py
+-rw-rw-rw-   0        0        0    10106 2023-04-17 13:00:19.000000 compoundwidgets-0.2.7/test/compound_widgets_test_1.py
+-rw-rw-rw-   0        0        0     7306 2023-04-17 12:42:39.000000 compoundwidgets-0.2.7/test/compound_widgets_test_2.py
+-rw-rw-rw-   0        0        0      991 2023-04-26 10:06:43.000000 compoundwidgets-0.2.7/test/custom_buttons_test.py
+-rw-rw-rw-   0        0        0     2517 2023-04-07 21:26:04.000000 compoundwidgets-0.2.7/test/custom_frames_test_1.py
+-rw-rw-rw-   0        0        0     2495 2023-04-07 21:32:27.000000 compoundwidgets-0.2.7/test/custom_frames_test_2.py
+-rw-rw-rw-   0        0        0      888 2023-04-07 22:03:48.000000 compoundwidgets-0.2.7/test/custom_frames_test_3.py
+-rw-rw-rw-   0        0        0     2745 2023-04-17 20:15:42.000000 compoundwidgets-0.2.7/test/custom_frames_test_4.py
+-rw-rw-rw-   0        0        0     4541 2023-04-12 10:11:28.000000 compoundwidgets-0.2.7/test/led_buttons_test.py
+-rw-rw-rw-   0        0        0     3937 2023-04-12 13:58:27.000000 compoundwidgets-0.2.7/test/message_box_test.py
```

### Comparing `compoundwidgets-0.2.6/LICENSE.txt` & `compoundwidgets-0.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/MANIFEST.in` & `compoundwidgets-0.2.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/README.md` & `compoundwidgets-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/AUTOCOMPLETE_WIDGETS.py` & `compoundwidgets-0.2.7/compoundwidgets/AUTOCOMPLETE_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/COMPOUND_WIDGETS.py` & `compoundwidgets-0.2.7/compoundwidgets/COMPOUND_WIDGETS.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,16 @@
         enable(): turns the whole widget 'on'
         readonly(): turn the whole widget 'readonly' (non-editable)
     """
 
     def __init__(self, parent,
                  label_text='label:', label_anchor='e', label_width=None,
                  entry_value='', entry_numeric=False, entry_width=None,
-                 entry_max_char=None, entry_method=None, font=None, precision=2):
+                 entry_max_char=None, entry_method=None, font=None, precision=2,
+                 trace_variable=False):
 
         # Parent class initialization
         super().__init__(parent)
 
         # Entry validation for numbers
         validate_numbers = self.register(float_only)
         validate_chars = self.register(max_chars)
@@ -168,16 +169,17 @@
             if entry_max_char:
                 entry_value = str(entry_value[:entry_max_char])
                 self.variable.set(entry_value)
                 self.entry.config(validate='all', validatecommand=(validate_chars, '%d', '%P', entry_max_char))
 
         # Bind method
         if True:
+            if trace_variable:
+                self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry_method = entry_method
-            self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry.bind("<Return>", entry_method)
             self.entry.bind("<FocusOut>", entry_method)
 
     def _update_value(self, name, index, mode):
         if self.entry_method:
             self.entry.event_generate("<Return>")
 
@@ -357,16 +359,15 @@
         readonly(): turn the whole widget 'readonly' (non-editable)
         """
 
     def __init__(self, parent,
                  label_text='label:', label_anchor='e', label_width=None,
                  entry_value=None, entry_width=None, entry_method=None, entry_type='float',
                  spin_start=0, spin_end=10, spin_increment=1, spin_precision=2,
-                 font=None
-                 ):
+                 font=None, trace_variable=False):
 
         # Parent class initialization
         super().__init__(parent)
 
         # Spinbox atributes initialization
         self.start = spin_start
         self.end = spin_end
@@ -419,15 +420,16 @@
             if entry_width:
                 self.spin['width'] = entry_width
             if font:
                 self.spin.config(font=font)
 
         # Bind method
         if True:
-            self.variable.trace_add(["read", "write", "unset"], self._update_value)
+            if trace_variable:
+                self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry_method = entry_method
             self.spin.bind("<Return>", entry_method, add='+')
             self.spin.bind("<Return>", self._check_user_value, add='+')
             self.spin.bind("<FocusOut>", entry_method, add='+')
             self.spin.bind("<FocusOut>", self._check_user_value, add='+')
             self.spin.bind("<<Increment>>", self._do_on_increment)
             self.spin.bind("<<Decrement>>", self._do_on_decrement)
@@ -774,15 +776,15 @@
 
     # imperial_unit_list[index] * conversion[index] => metric_unit_list[index]
 
     def __init__(self, parent,
                  label_text='Label:', label_anchor='e', label_width=None,
                  entry_value='', entry_width=None, entry_method=None,
                  combobox_unit=None, combobox_unit_width=8, combobox_unit_conversion=False,
-                 font=None, precision=2):
+                 font=None, precision=2, trace_variable=False):
 
         # Parent class initialization
         super().__init__(parent)
 
         # Entry validation for numbers
         validate_numbers = self.register(float_only)
 
@@ -837,16 +839,17 @@
             self.unit_combo.grid(row=0, column=2, sticky='ew', padx=2)
             self.last_unit = self.unit_combo.values[0]
             self.combobox_variable = self.unit_combo.variable
             self.is_locked = False
 
         # Bind methods
         if True:
+            if trace_variable:
+                self.entry_variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry_method = entry_method
-            self.entry_variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry.bind("<Return>", entry_method)
             self.entry.bind("<FocusOut>", entry_method)
 
             if not self.combobox_unit_conversion:
                 self.unit_combo.bind("<<ComboboxSelected>>", entry_method)
             else:
                 self.unit_combo.bind("<<ComboboxSelected>>", self._convert_to_selected_unit)
@@ -1180,15 +1183,15 @@
     """
 
     def __init__(self, parent,
                  label_text='label:', label_anchor='e', label_width=None,
                  entry_value='', entry_numeric=False, entry_width=None,
                  entry_max_char=None, entry_method=None,
                  button_text='', button_width=None, button_method=None,
-                 font=None, precision=2):
+                 font=None, precision=2, trace_variable=False):
 
         # Parent class initialization
         super().__init__(parent)
 
         # Entry validation for numbers
         validate_numbers = self.register(float_only)
         validate_chars = self.register(max_chars)
@@ -1243,16 +1246,16 @@
             self.button.grid(row=0, column=2, sticky='ew', padx=2)
 
         # Bind methods
         if True:
             self.button_method = button_method
             if button_method:
                 self.button.configure(command=button_method)
-
-            self.variable.trace_add(["read", "write", "unset"], self._update_value)
+            if trace_variable:
+                self.variable.trace_add(["read", "write", "unset"], self._update_value)
             self.entry_method = entry_method
             if entry_method:
                 self.entry.bind("<Return>", entry_method)
                 self.entry.bind("<FocusOut>", entry_method)
 
     def _update_value(self, name, index, mode):
         if self.entry_method:
```

### Comparing `compoundwidgets-0.2.6/compoundwidgets/CUSTOM_BUTTONS.py` & `compoundwidgets-0.2.7/compoundwidgets/CUSTOM_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/CUSTOM_FRAMES.py` & `compoundwidgets-0.2.7/compoundwidgets/CUSTOM_FRAMES.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_new.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_new.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/add_to_form.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/add_to_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/back.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/back.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/calculate.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/calculate.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/clear.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/clear.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/edit_form.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/edit_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/help.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/help.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/no.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/no.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/quit.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/quit.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/remove_from_form.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/remove_from_form.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/save.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/save.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/trash_can.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/trash_can.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/IMAGES/yes.png` & `compoundwidgets-0.2.7/compoundwidgets/IMAGES/yes.png`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/LED_BUTTONS.py` & `compoundwidgets-0.2.7/compoundwidgets/LED_BUTTONS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/MESSAGE_BOX_WIDGETS.py` & `compoundwidgets-0.2.7/compoundwidgets/MESSAGE_BOX_WIDGETS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/SCRIPTS.py` & `compoundwidgets-0.2.7/compoundwidgets/SCRIPTS.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/compoundwidgets/__init__.py` & `compoundwidgets-0.2.7/compoundwidgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.06"
+__version__ = "0.2.07"
 __author__ = 'Andre Mariano'
 __all__ = ['AUTOCOMPLETE_WIDGETS',
            'COMPOUND_WIDGETS',
            'CUSTOM_BUTTONS',
            'CUSTOM_FRAMES',
            'MESSAGE_BOX_WIDGETS',
            'IMAGES',
```

### Comparing `compoundwidgets-0.2.6/compoundwidgets.egg-info/SOURCES.txt` & `compoundwidgets-0.2.7/compoundwidgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/setup.py` & `compoundwidgets-0.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='compoundwidgets',
-    version='0.2.06',
+    version='0.2.07',
     author='Andre Mariano',
     license="MIT",
     url='https://github.com/AndreMariano100/CompoundWidgets.git',
     description='Compound TTK Widgets with ttkbootstrap',
     author_email='andremariano100@gmail.com',
     packages=['compoundwidgets', 'compoundwidgets.IMAGES'],
     install_requires=['ttkbootstrap', 'Pillow'],
```

### Comparing `compoundwidgets-0.2.6/test/autocomplete_widget_test.py` & `compoundwidgets-0.2.7/test/autocomplete_widget_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/compound_widgets_test_1.py` & `compoundwidgets-0.2.7/test/compound_widgets_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/compound_widgets_test_2.py` & `compoundwidgets-0.2.7/test/compound_widgets_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/custom_buttons_test.py` & `compoundwidgets-0.2.7/test/custom_buttons_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     cw.EditReport,
     cw.RemoveFromReport,
     cw.AddNewButton,
     cw.EraseButton,
     cw.QuitButton
 )
 for i, widget in enumerate(all_buttons):
-    widget(root).grid(row=i, column=0, padx=10, pady=2)
+    widget(root, width=12).grid(row=i, column=0, padx=10, pady=2)
 
 for i, widget in enumerate(all_buttons):
     widget(root, language='br').grid(row=i, column=1, padx=10, pady=2)
 
 for i, widget in enumerate(all_buttons):
     widget(root, language='en', style='primary', padding=1).grid(row=i, column=2, padx=10, pady=2)
```

### Comparing `compoundwidgets-0.2.6/test/custom_frames_test_1.py` & `compoundwidgets-0.2.7/test/custom_frames_test_1.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/custom_frames_test_2.py` & `compoundwidgets-0.2.7/test/custom_frames_test_2.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/custom_frames_test_3.py` & `compoundwidgets-0.2.7/test/custom_frames_test_3.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/custom_frames_test_4.py` & `compoundwidgets-0.2.7/test/custom_frames_test_4.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/led_buttons_test.py` & `compoundwidgets-0.2.7/test/led_buttons_test.py`

 * *Files identical despite different names*

### Comparing `compoundwidgets-0.2.6/test/message_box_test.py` & `compoundwidgets-0.2.7/test/message_box_test.py`

 * *Files identical despite different names*

