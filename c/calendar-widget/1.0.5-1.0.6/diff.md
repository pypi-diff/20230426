# Comparing `tmp/calendar_widget-1.0.5.tar.gz` & `tmp/calendar_widget-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_widget-1.0.5.tar", last modified: Sat Apr 22 00:39:35 2023, max compression
+gzip compressed data, was "calendar_widget-1.0.6.tar", last modified: Tue Apr 25 22:45:42 2023, max compression
```

## Comparing `calendar_widget-1.0.5.tar` & `calendar_widget-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 00:39:35.721624 calendar_widget-1.0.5/
--rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.5/LICENSE.md
--rw-rw-rw-   0        0        0     8084 2023-04-22 00:39:35.721624 calendar_widget-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     7204 2023-04-22 00:29:44.000000 calendar_widget-1.0.5/README.md
--rw-rw-rw-   0        0        0      763 2023-04-22 00:39:00.000000 calendar_widget-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-22 00:39:35.721624 calendar_widget-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-22 00:39:35.612243 calendar_widget-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-22 00:39:35.659119 calendar_widget-1.0.5/src/calendar_widget/
--rw-rw-rw-   0        0        0   127185 2023-04-22 00:36:07.000000 calendar_widget-1.0.5/src/calendar_widget/Calendar_Widget.py
--rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.5/src/calendar_widget/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 00:39:35.721624 calendar_widget-1.0.5/src/calendar_widget.egg-info/
--rw-rw-rw-   0        0        0     8084 2023-04-22 00:39:35.000000 calendar_widget-1.0.5/src/calendar_widget.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-04-22 00:39:35.000000 calendar_widget-1.0.5/src/calendar_widget.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 00:39:35.000000 calendar_widget-1.0.5/src/calendar_widget.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-22 00:39:35.000000 calendar_widget-1.0.5/src/calendar_widget.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-22 00:39:35.721624 calendar_widget-1.0.5/tests/
--rw-rw-rw-   0        0        0      397 2023-04-22 00:35:42.000000 calendar_widget-1.0.5/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/
+-rw-rw-rw-   0        0        0    26526 2023-04-14 15:16:21.000000 calendar_widget-1.0.6/LICENSE.md
+-rw-rw-rw-   0        0        0     9419 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     8530 2023-04-25 22:44:21.000000 calendar_widget-1.0.6/README.md
+-rw-rw-rw-   0        0        0      763 2023-04-25 22:44:34.000000 calendar_widget-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:45:42.856694 calendar_widget-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.700430 calendar_widget-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.778563 calendar_widget-1.0.6/src/calendar_widget/
+-rw-rw-rw-   0        0        0   127902 2023-04-25 22:28:54.000000 calendar_widget-1.0.6/src/calendar_widget/Calendar_Widget.py
+-rw-rw-rw-   0        0        0       37 2023-04-15 01:39:22.000000 calendar_widget-1.0.6/src/calendar_widget/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.794188 calendar_widget-1.0.6/src/calendar_widget.egg-info/
+-rw-rw-rw-   0        0        0     9419 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-25 22:45:42.000000 calendar_widget-1.0.6/src/calendar_widget.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 22:45:42.809814 calendar_widget-1.0.6/tests/
+-rw-rw-rw-   0        0        0      628 2023-04-25 22:29:34.000000 calendar_widget-1.0.6/tests/test.py
```

### Comparing `calendar_widget-1.0.5/LICENSE.md` & `calendar_widget-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `calendar_widget-1.0.5/PKG-INFO` & `calendar_widget-1.0.6/src/calendar_widget.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calendar_widget
-Version: 1.0.5
+Name: calendar-widget
+Version: 1.0.6
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -171,19 +171,28 @@
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
 | weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. |
 | weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. |
 | weekday_width= | Sets the width of the boxes that hold the weekday headings. |
 | weekday_font_fill= | Sets the colour of the text associated with the weekday headings. |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts) |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold' |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic' |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False |
 | calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020) |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts) |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold' |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic' |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False |
 | date_text_fill= | Sets the colour of the text numbers associated with the month dates. |
-| date_text_font_family= | Sets the font type used to create the month dates. |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts) |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold' |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic' |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False |
 | trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. |
 | trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. |
 | date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. |
 | text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. |
 | user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. |
 | user_highlight_text= | Sets the colour of the text associated with the user highlight. |
```

### Comparing `calendar_widget-1.0.5/README.md` & `calendar_widget-1.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -155,19 +155,28 @@
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
 | weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. |
 | weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. |
 | weekday_width= | Sets the width of the boxes that hold the weekday headings. |
 | weekday_font_fill= | Sets the colour of the text associated with the weekday headings. |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts) |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold' |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic' |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False |
 | calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020) |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts) |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold' |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic' |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False |
 | date_text_fill= | Sets the colour of the text numbers associated with the month dates. |
-| date_text_font_family= | Sets the font type used to create the month dates. |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts) |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold' |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic' |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False |
 | trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. |
 | trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. |
 | date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. |
 | text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. |
 | user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. |
 | user_highlight_text= | Sets the colour of the text associated with the user highlight. |
```

### Comparing `calendar_widget-1.0.5/pyproject.toml` & `calendar_widget-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calendar_widget"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Spartanlasergun", email="bns360@live.com" },
 ]
 description = "Calendar widget for use with python tkinter"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `calendar_widget-1.0.5/src/calendar_widget/Calendar_Widget.py` & `calendar_widget-1.0.6/src/calendar_widget/Calendar_Widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,25 @@
             calendar_date_title="black",
             date_text_fill="black",
             trail_box_fill="gray83",
             trail_text_fill="black",
             date_highlight="orange",
             text_highlight_fill="black",
             weekday_font_family="Algerian",
+            weekday_font_weight='normal',
+            weekday_font_slant='roman',
+            weekday_font_underline=False,
             date_heading_font_family="Garamond",
+            date_heading_font_weight='normal',
+            date_heading_font_slant='roman',
+            date_heading_font_underline=False,
             date_text_font_family="Arial CE",
+            date_text_font_weight='normal',
+            date_text_font_slant='roman',
+            date_text_font_underline=False,
             user_highlight_colour="gray75",
             user_highlight_text="black",
             img_pos_x=0,
             img_pos_y=0,
             img_anchor='nw'):
 
         self.command = command   # create global instance of user command for use within the click binding
@@ -181,15 +190,16 @@
                                            outline=weekday_border,
                                            fill=weekday_fill,
                                            width=weekday_width,
                                            tags=weekdays[heading_inc])
             heading_inc = heading_inc + 1
 
         font_size = int((box_depth * 0.75) * 0.75)
-        weekday_font = font.Font(family=weekday_font_family, size=font_size)
+        weekday_font = font.Font(family=weekday_font_family, size=font_size, 
+            weight=weekday_font_weight, slant=weekday_font_slant, underline=weekday_font_underline)
         for day in weekdays:
             weekday_coords = self.Calendar.coords(day)
             letter_x = (weekday_coords[0] + weekday_coords[2]) / 2
             letter_y = (weekday_coords[1] + weekday_coords[3]) / 2
             letter = day[0]
             self.Calendar.create_text(letter_x, letter_y, text=letter, anchor="center",
                                       font=weekday_font, fill=weekday_font_fill)
@@ -214,30 +224,32 @@
         self.day_num = None
 
         # create calendar date heading (ex: Aug 2022)
         arrow_box_coords = self.Calendar.coords("arrow_box")
         self.arrow_date_x = (arrow_box_coords[0] + arrow_box_coords[2]) / 2
         self.arrow_date_y = (arrow_box_coords[1] + arrow_box_coords[3]) / 2
         font_size = int((self.arrow_date_y * 0.75) * 0.5)
-        self.date_heading_font = font.Font(family=date_heading_font_family, size=font_size)
+        self.date_heading_font = font.Font(family=date_heading_font_family, size=font_size, 
+            weight=date_heading_font_weight, slant=date_heading_font_slant, underline=date_heading_font_underline)
         self.Calendar.create_text(self.arrow_date_x, self.arrow_date_y, text=self.date_today, anchor="center",
                                   font=self.date_heading_font,
                                   fill=self.calendar_date_title, tags="arrow_box_date")
 
         # create date boxes for days of the month
         # The date boxes make up the monthly date grid into which the relevant dates are placed. The tags for the date
         # boxes are globally stored and are used to define the position of the text on the grid.
         box_width = ((size - (padding * 2)) * 0.144)
         box_depth = ((depth - padding) - (padding + (depth * 0.25))) * 0.1428
         box_y_start = (padding + (depth * 0.25)) + box_depth
         width_inc = 0
         depth_inc = 0
         box_count = 0
         self.date_box_font_size = int(((box_depth) * 0.75) * 0.6)
-        self.date_text_font = font.Font(family=date_text_font_family, size=self.date_box_font_size)
+        self.date_text_font = font.Font(family=date_text_font_family, size=self.date_box_font_size, 
+            weight=date_text_font_weight, slant=date_text_font_slant, underline=date_text_font_underline)
         self.date_box_tags = []
         while box_count != 42:
             box_tag = "date_box_" + str(box_count)
             self.Calendar.create_rectangle((padding + (box_width * width_inc)),
                                            (box_y_start + (box_depth * depth_inc)),
                                            (padding + (box_width * (width_inc + 1))),
                                            (box_y_start + (box_depth * (depth_inc + 1))),
```

### Comparing `calendar_widget-1.0.5/src/calendar_widget.egg-info/PKG-INFO` & `calendar_widget-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calendar-widget
-Version: 1.0.5
+Name: calendar_widget
+Version: 1.0.6
 Summary: Calendar widget for use with python tkinter
 Author-email: Spartanlasergun <bns360@live.com>
 Project-URL: Homepage, https://github.com/Spartanlasergun/calendar_widget
 Project-URL: Bug Tracker, https://github.com/Spartanlasergun/calendar_widget/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -171,19 +171,28 @@
 | arrow_fill= | Sets the colour of the calendar arrows. |
 | arrow_thickness= | Sets the thickness of the calendar arrows. |
 | arrow_active= | Sets the colour for the active highlight when the mouse hovers over the calendar arrows. |
 | weekday_border= | Sets the colour for the outline of the boxes that hold the weekday headings. |
 | weekday_fill= | Sets the colour for the background of the boxes that hold the weekday headings. |
 | weekday_width= | Sets the width of the boxes that hold the weekday headings. |
 | weekday_font_fill= | Sets the colour of the text associated with the weekday headings. |
-| weekday_font_family= | Sets the type of font used to create the weekday headings. |
+| weekday_font_family= | Sets the type of font used to create the weekday headings. (Accepts any of the valid native tkinter fonts) |
+| weekday_font_weight= | Sets the weight of the font used to create the weekday headings. Valid options are 'normal' or 'bold' |
+| weekday_font_slant= | Sets the slant of the font used to create the weekday headings. Valid options are 'roman' or 'italic' |
+| weekday_font_underline= | Sets the underline of the font used to creates the weekday heading. Valid options are True or False |
 | calendar_date_title= | Sets the colour of the text associated with the calendar title (ex: Aug 2020) |
-| date_heading_font_family= | Sets the font type for the Calendar date heading. |
+| date_heading_font_family= | Sets the font type for the Calendar date heading. (Accepts any of the valid native tkinter fonts) |
+| date_heading_font_weight= | Sets the weight of the font used to create the Calendar date heading. Valid options are 'normal' or 'bold' |
+| date_heading_font_slant= | Sets the slant of the font used to create the Calendar date heading. Valid options are 'roman' or 'italic' |
+| date_heading_font_underline= | Sets the underline of the font used to create the Calendar date heading. Valid options are True or False |
 | date_text_fill= | Sets the colour of the text numbers associated with the month dates. |
-| date_text_font_family= | Sets the font type used to create the month dates. |
+| date_text_font_family= | Sets the font type used to create the month dates. (Accepts any of the valid native tkinter fonts) |
+| date_text_font_weight= | Sets the weight of the font used to create the month dates. Valid options are 'normal' or 'bold' |
+| date_text_font_slant= | Sets the slant of the font used to create the month dates. Valid options are 'roman' or 'italic' |
+| date_text_font_underline= | Sets the underline of the font used to create the month dates. Valid options are True or False |
 | trail_box_fill= | Sets the colour of the background of the date boxes that trail into the previous and following months. |
 | trail_text_fill= | Sets the colour of the text numbers associated with the trailing date boxes. |
 | date_highlight= | Sets the colour of the permanent date highlight associated with the current date retrieved from the OS. |
 | text_highlight_fill= | Sets the colour of the text associated with the permanent date highlight. |
 | user_highlight_colour= | Sets the colour of the highlight that is created when the user clicks on a month date. |
 | user_highlight_text= | Sets the colour of the text associated with the user highlight. |
```

