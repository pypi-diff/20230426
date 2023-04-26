# Comparing `tmp/tksheet-6.0.1.tar.gz` & `tmp/tksheet-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-6.0.1.tar", last modified: Mon Apr 24 17:39:04 2023, max compression
+gzip compressed data, was "tksheet-6.0.2.tar", last modified: Wed Apr 26 17:06:09 2023, max compression
```

## Comparing `tksheet-6.0.1.tar` & `tksheet-6.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/
--rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2882 2023-04-24 17:39:04.375100 tksheet-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2232 2023-04-18 08:24:22.000000 tksheet-6.0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 17:39:04.375100 tksheet-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-04-23 07:10:11.000000 tksheet-6.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/tksheet/
--rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.1/tksheet/__init__.py
--rw-rw-rw-   0        0        0   164503 2023-04-24 17:34:13.000000 tksheet-6.0.1/tksheet/_tksheet.py
--rw-rw-rw-   0        0        0    99275 2023-04-24 11:22:20.000000 tksheet-6.0.1/tksheet/_tksheet_column_headers.py
--rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.1/tksheet/_tksheet_formatters.py
--rw-rw-rw-   0        0        0   328996 2023-04-24 16:00:43.000000 tksheet-6.0.1/tksheet/_tksheet_main_table.py
--rw-rw-rw-   0        0        0    12952 2023-04-24 11:27:55.000000 tksheet-6.0.1/tksheet/_tksheet_other_classes.py
--rw-rw-rw-   0        0        0    99038 2023-04-24 11:22:38.000000 tksheet-6.0.1/tksheet/_tksheet_row_index.py
--rw-rw-rw-   0        0        0     5642 2023-04-20 08:50:10.000000 tksheet-6.0.1/tksheet/_tksheet_top_left_rectangle.py
--rw-rw-rw-   0        0        0    52264 2023-04-22 08:42:39.000000 tksheet-6.0.1/tksheet/_tksheet_vars.py
-drwxrwxrwx   0        0        0        0 2023-04-24 17:39:04.375100 tksheet-6.0.1/tksheet.egg-info/
--rw-rw-rw-   0        0        0     2882 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 17:39:04.000000 tksheet-6.0.1/tksheet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.864195 tksheet-6.0.2/
+-rw-rw-rw-   0        0        0     1101 2023-04-13 09:47:22.000000 tksheet-6.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     3003 2023-04-26 17:06:09.864195 tksheet-6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2353 2023-04-24 17:49:11.000000 tksheet-6.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-26 17:06:09.864195 tksheet-6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-04-24 17:51:18.000000 tksheet-6.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.848570 tksheet-6.0.2/tksheet/
+-rw-rw-rw-   0        0        0      351 2023-04-13 08:55:45.000000 tksheet-6.0.2/tksheet/__init__.py
+-rw-rw-rw-   0        0        0   164503 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet.py
+-rw-rw-rw-   0        0        0    99400 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_column_headers.py
+-rw-rw-rw-   0        0        0    10233 2023-04-24 07:09:26.000000 tksheet-6.0.2/tksheet/_tksheet_formatters.py
+-rw-rw-rw-   0        0        0   329896 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_main_table.py
+-rw-rw-rw-   0        0        0    12952 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_other_classes.py
+-rw-rw-rw-   0        0        0    99164 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_row_index.py
+-rw-rw-rw-   0        0        0     5642 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_top_left_rectangle.py
+-rw-rw-rw-   0        0        0    52264 2023-04-26 16:31:48.000000 tksheet-6.0.2/tksheet/_tksheet_vars.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:06:09.864195 tksheet-6.0.2/tksheet.egg-info/
+-rw-rw-rw-   0        0        0     3003 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-26 17:06:09.000000 tksheet-6.0.2/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-6.0.1/LICENSE.txt` & `tksheet-6.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/PKG-INFO` & `tksheet-6.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -48,14 +48,15 @@
 - Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
 ----
 
 ![alt text](https://i.imgur.com/ojU3IQi.jpeg)
```

### Comparing `tksheet-6.0.1/README.md` & `tksheet-6.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 - Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
 ----
 
 ![alt text](https://i.imgur.com/ojU3IQi.jpeg)
```

### Comparing `tksheet-6.0.1/setup.py` & `tksheet-6.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
     long_description = f.read()
 
 setup(
   name = 'tksheet',
   packages = ['tksheet'],
-  version = '6.0.1',
+  version = '6.0.2',
   python_requires = '>=3.6',
   license = 'MIT',
   description = 'Tkinter table / sheet widget',
   long_description = long_description,
   long_description_content_type = 'text/markdown',
   author = 'ragardner',
   author_email = 'github@ragardner.simplelogin.com',
   url = 'https://github.com/ragardner/tksheet',
-  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz',
+  download_url = 'https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz',
   keywords = ['tkinter', 'table', 'widget', 'sheet', 'grid', 'tk'],
   install_requires = [],
   classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License'
```

### Comparing `tksheet-6.0.1/tksheet/_tksheet.py` & `tksheet-6.0.2/tksheet/_tksheet.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/tksheet/_tksheet_column_headers.py` & `tksheet-6.0.2/tksheet/_tksheet_column_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,14 +552,15 @@
                                                                                 int(new_selected[0]),        #2
                                                                                 int(new_selected[-1]),       #3
                                                                                 sorted(orig_selected),  #4
                                                                                 dispset))))                  #5
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ch_extra_end_drag_drop_func is not None:
                         self.ch_extra_end_drag_drop_func(EndDragDropEvent("end_column_header_drag_drop", tuple(orig_selected), new_selected, int(c)))
+                    self.event_generate("<<SheetDataChangeEvent>>")
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x = event.x)
             if c is not None and c < len(self.MT.col_positions) - 1 and c == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
                 canvasx = self.canvasx(event.x)
                 if (event.y < self.MT.hdr_txt_h + 5 and
                     (
@@ -1221,15 +1222,15 @@
             if text is None:
                 return False
             else:
                 text = text if isinstance(text, str) else f"{text}"
         text = "" if text is None else text
         if self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
-                self.set_current_height_to_cell(datacn)
+                self.set_current_height_to_text(text, datacn)
             self.set_col_width_run_binding(c)
         self.select_col(c = c, keep_other_selections = True)
         self.create_text_editor(c = c, text = text, set_data_on_close = True, dropdown = dropdown)
         return True
     
     # displayed indexes
     def get_cell_align(self, c):
@@ -1432,18 +1433,19 @@
                     self.MT.undo_storage.append(zlib.compress(pickle.dumps(("edit_header",
                                                                             {datacn: self.MT._headers[datacn]},
                                                                             (((0, c, len(self.MT.row_positions) - 1, c + 1), "columns"), ),
                                                                             self.MT.currently_selected()))))
                 self.set_cell_data(datacn = datacn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
-                self.set_current_height_to_cell(datacn)
+                self.set_current_height_to_text(value, datacn)
             self.set_col_width_run_binding(c)
         if redraw:
             self.MT.refresh()
+        self.event_generate("<<SheetDataChangeEvent>>")
     
     def set_cell_data(self, datacn = None, value = ""):
         if isinstance(self.MT._headers, int):
             self.MT.set_cell_data(datarn = self.MT._headers, datacn = datacn, value = value)
         else:
             self.fix_header(datacn)
             if datacn in self.cell_options and 'checkbox' in self.cell_options[datacn]:
@@ -1608,18 +1610,18 @@
             win_h = space_bot - 1
         if win_h < self.MT.hdr_txt_h + 5:
             win_h = self.MT.hdr_txt_h + 5
         elif win_h > win_h2:
             win_h = win_h2
         return win_h, "nw"
 
-    def set_current_height_to_cell(self, datacn):
+    def set_current_height_to_text(self, text, datacn):
         x = self.MT.txt_measure_canvas.create_text(0,
                                                    0,
-                                                   text = self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True) if isinstance(self.MT._headers, int) else self.MT._headers[datacn],
+                                                   text = self.MT.get_valid_cell_data_as_str(self.MT._headers, datacn, get_displayed = True) if isinstance(self.MT._headers, int) else text,
                                                    font = self.MT._hdr_font)
         b = self.MT.txt_measure_canvas.bbox(x)
         self.MT.txt_measure_canvas.delete(x)
         new_height = b[3] - b[1] + 5
         space_bot = self.MT.get_space_bot(0)
         if new_height > space_bot:
             new_height = space_bot
```

### Comparing `tksheet-6.0.1/tksheet/_tksheet_formatters.py` & `tksheet-6.0.2/tksheet/_tksheet_formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/tksheet/_tksheet_main_table.py` & `tksheet-6.0.2/tksheet/_tksheet_main_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,14 +504,15 @@
         self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
         for r1, c1, r2, c2 in boxes:
             self.show_ctrl_outline(canvas = "table", start_cell = (c1, r1), end_cell = (c2, r2))
         if self.extra_end_ctrl_x_func is not None:
             self.extra_end_ctrl_x_func(CtrlKeyEvent("end_ctrl_x", boxes, currently_selected, rows))
+        self.event_generate("<<SheetDataChangeEvent>>")
 
     def find_last_selected_box_with_current(self, currently_selected):
         if currently_selected.type_ in ("cell", "column"):
             boxes, maxrows = self.get_ctrl_x_c_boxes()
         else:
             boxes = self.get_ctrl_x_c_boxes()
         for (r1, c1, r2, c2), type_ in boxes.items():
@@ -632,14 +633,15 @@
                                                                  added_rows_cols))))
         self.create_selected(selected_r, selected_c, selected_r + numrows, selected_c + numcols, "cells")
         self.create_current(selected_r, selected_c, type_ = "cell", inside = True if numrows > 1 or numcols > 1 else False)
         self.see(r = selected_r, c = selected_c, keep_yscroll = False, keep_xscroll = False, bottom_right_corner = False, check_cell_visibility = True, redraw = False)
         self.refresh()
         if self.extra_end_ctrl_v_func is not None:
             self.extra_end_ctrl_v_func(PasteEvent("end_ctrl_v", currently_selected, rows))
+        self.event_generate("<<SheetDataChangeEvent>>")
 
     def delete_key(self, event = None):
         if self.anything_selected():
             currently_selected = self.currently_selected()
             undo_storage = {}
             boxes = {}
             for item in chain(self.find_withtag("CellSelectFill"), self.find_withtag("RowSelectFill"), self.find_withtag("ColSelectFill"), self.find_withtag("Current_Outside")):
@@ -668,14 +670,15 @@
                             self.set_cell_data(datarn, datacn, "")
                             changes += 1
             if self.extra_end_delete_key_func is not None:
                 self.extra_end_delete_key_func(CtrlKeyEvent("end_delete_key", boxes, currently_selected, undo_storage))
             if changes and self.undo_enabled:
                 self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells", undo_storage, tuple(boxes.items()), currently_selected))))
             self.refresh()
+            self.event_generate("<<SheetDataChangeEvent>>")
             
     def move_columns_adjust_options_dict(self, col, to_move_min, num_cols, move_data = True, create_selections = True):
         c = int(col)
         to_move_max = to_move_min + num_cols
         to_del = to_move_max + num_cols
         orig_selected = list(range(to_move_min, to_move_min + num_cols))
         self.deselect("all", redraw = False)
@@ -1124,14 +1127,15 @@
                     self._headers.insert(cn, v)
                 except:
                     continue
             self.reselect_from_get_boxes(undo_storage[1]['selection_boxes'])
         self.refresh()
         if self.extra_end_ctrl_z_func is not None:
             self.extra_end_ctrl_z_func(UndoEvent("end_ctrl_z", undo_storage[0], undo_storage))
+        self.event_generate("<<SheetDataChangeEvent>>")
 
     def bind_arrowkeys(self, keys: dict = {}):
         for canvas in (self, self.parentframe, self.CH, self.RI, self.TL):
             for k, func in keys.items():
                 canvas.bind(f"<{arrowkey_bindings_helper[k.lower()]}>", func)
 
     def unbind_arrowkeys(self, keys: dict = {}):
@@ -2979,14 +2983,15 @@
                        newdataref = None, 
                        reset_col_positions = True, 
                        reset_row_positions = True,
                        redraw = False, 
                        return_id = True,
                        keep_formatting = True):
         if isinstance(newdataref, (list, tuple)):
+            newdataref = [["" if c is None else c for c in row] for row in newdataref]        
             self.data = newdataref
             if keep_formatting:
                 self.reapply_formatting()
             else:
                 self.delete_all_formatting(clear_values = False)
             self.undo_storage = deque(maxlen = self.max_undos)
             if reset_col_positions:
@@ -3348,14 +3353,15 @@
             self.undo_storage.append(zlib.compress(pickle.dumps(("insert_col", {"data_col_num": data_ins_col,
                                                                                 "displayed_columns": saved_displayed_columns,
                                                                                 "sheet_col_num": displayed_ins_col,
                                                                                 "numcols": numcols}))))
         self.refresh()
         if self.extra_end_insert_cols_rc_func is not None:
             self.extra_end_insert_cols_rc_func(InsertEvent("end_insert_columns", data_ins_col, displayed_ins_col, numcols))
+        self.event_generate("<<SheetDataChangeEvent>>")
 
     def insert_row_rc(self, event = None):
         if self.anything_selected(exclude_columns = True, exclude_cells = True):
             selrows = self.get_selected_rows()
             numrows = len(selrows)
             stidx = min(selrows) if event == "above" else max(selrows) + 1
             posidx = int(stidx)
@@ -3397,14 +3403,15 @@
         if self.undo_enabled:
             self.undo_storage.append(zlib.compress(pickle.dumps(("insert_row", {"data_row_num": stidx,
                                                                                 "sheet_row_num": posidx,
                                                                                 "numrows": numrows}))))
         self.refresh()
         if self.extra_end_insert_rows_rc_func is not None:
             self.extra_end_insert_rows_rc_func(InsertEvent("end_insert_rows", stidx, posidx, numrows))
+        self.event_generate("<<SheetDataChangeEvent>>")
             
     def del_cols_rc(self, event = None):
         seld_cols = sorted(self.get_selected_cols())
         if seld_cols:
             if self.extra_begin_del_cols_rc_func is not None:
                 try:
                     self.extra_begin_del_cols_rc_func(DeleteRowColumnEvent("begin_delete_columns", seld_cols))
@@ -3465,24 +3472,25 @@
             if not self.all_columns_displayed:
                 self.displayed_columns = [c for c in self.displayed_columns if c not in seldset]
                 for c in sorted(seldset):
                     self.displayed_columns = [dc if c > dc else dc - 1 for dc in self.displayed_columns]
             self.refresh()
             if self.extra_end_del_cols_rc_func is not None:
                 self.extra_end_del_cols_rc_func(DeleteRowColumnEvent("end_delete_columns", seld_cols))
+            self.event_generate('<<SheetDataChangeEvent>>')
 
     def del_rows_rc(self, event = None):
         seld_rows = sorted(self.get_selected_rows())
         if seld_rows:
             if self.extra_begin_del_rows_rc_func is not None:
                 try:
                     self.extra_begin_del_rows_rc_func(DeleteRowColumnEvent("begin_delete_rows", seld_rows))
                 except:
                     return
-            seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[c] for r in seld_rows)
+            seldset = set(seld_rows) if self.all_rows_displayed else set(self.displayed_rows[r] for r in seld_rows)
             list_of_coords = tuple((r, c) for (r, c) in self.cell_options if r in seldset)
             if self.undo_enabled:
                 undo_storage = {'deleted_rows': [],
                                 'rowheights': {},
                                 'deleted_index_values': [],
                                 'selection_boxes': self.get_boxes(),
                                 'displayed_rows': list(self.displayed_rows) if not isinstance(self.displayed_rows, int) else int(self.displayed_rows),
@@ -3522,14 +3530,15 @@
             self.row_options = {rn if rn < idx else rn - numrows: t for rn, t in self.row_options.items()}
             self.RI.cell_options = {rn if rn < idx else rn - numrows: t for rn, t in self.RI.cell_options.items()}
             self.deselect("allrows", redraw = False)
             self.set_current_to_last()
             self.refresh()
             if self.extra_end_del_rows_rc_func is not None:
                 self.extra_end_del_rows_rc_func(DeleteRowColumnEvent("end_delete_rows", seld_rows))
+            self.event_generate('<<SheetDataChangeEvent>>')
 
     def move_row_position(self, idx1, idx2):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
                 height = self.row_positions[idx1 + 1] - self.row_positions[idx1]
                 self.row_positions.insert(idx2 + 1, self.row_positions.pop(idx1 + 1))
                 for i in range(idx1 + 1, idx2 + 1):
@@ -5319,17 +5328,20 @@
                 self.undo_storage.append(zlib.compress(pickle.dumps(("edit_cells",
                                                                     {(datarn, datacn): self.get_cell_data(datarn, datacn)},
                                                                     (((r, c, r + 1, c + 1), "cells"), ),
                                                                     self.currently_selected()))))
             self.set_cell_data(datarn, datacn, value)
         if cell_resize and self.cell_auto_resize_enabled:
             self.set_cell_size_to_text(r, c, only_set_if_too_small = True, redraw = redraw, run_binding = True)
+        self.event_generate('<<SheetDataChangeEvent>>')
         return True
     
     def set_cell_data(self, datarn, datacn, value, kwargs = {}, expand_sheet = True):
+        if value is None:
+            value = ""
         if expand_sheet:
             if datarn >= len(self.data):
                 self.data.extend([list(repeat("", datacn + 1)) for i in range((datarn + 1) - len(self.data))])
             elif datacn >= len(self.data[datarn]):
                 self.data[datarn].extend(list(repeat("", (datacn + 1) - len(self.data[datarn]))))
         if expand_sheet or (len(self.data) > datarn and len(self.data[datarn]) > datacn):
             if (datarn, datacn) in self.cell_options and 'checkbox' in self.cell_options[(datarn, datacn)]:
@@ -5411,46 +5423,50 @@
         else:
             v = self.get_cell_data(datarn, datacn)
         kwargs = self.format_fix_kwargs(kwargs)
         if (datarn, datacn) not in self.cell_options:
             self.cell_options[(datarn, datacn)] = {}
         self.cell_options[(datarn, datacn)]['format'] = kwargs
         self.set_cell_data(datarn, datacn, value = v, kwargs = kwargs)
+        self.event_generate('<<SheetDataChangeEvent>>')
         
     def format_row(self, datarn, **kwargs):
         kwargs = self.format_fix_kwargs(kwargs)
         if datarn not in self.row_options:
             self.row_options[datarn] = {}
         self.row_options[datarn]['format'] = kwargs
         for datacn in range(self.total_data_cols()):
             self.set_cell_data(datarn, 
                                datacn,
                                value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                kwargs = kwargs)
+        self.event_generate('<<SheetDataChangeEvent>>')
             
     def format_column(self, datacn, **kwargs):
         kwargs = self.format_fix_kwargs(kwargs)
         if datacn not in self.col_options:
             self.col_options[datacn] = {}
         self.col_options[datacn]['format'] = kwargs
         for datarn in range(self.total_data_rows()):
             self.set_cell_data(datarn, 
                                datacn,
                                value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                kwargs = kwargs)
+        self.event_generate('<<SheetDataChangeEvent>>')
             
     def format_sheet(self, **kwargs):
         kwargs = self.format_fix_kwargs(kwargs)
         self.sheet_options['format'] = kwargs
         for datarn in range(self.total_data_rows()):
             for datacn in range(self.total_data_cols()):
                 self.set_cell_data(datarn, 
                                    datacn,
                                    value = kwargs['value'] if 'value' in kwargs else self.get_cell_data(datarn, datacn),
                                    kwargs = kwargs)
+        self.event_generate('<<SheetDataChangeEvent>>')
 
     def format_fix_kwargs(self, kwargs):
         if kwargs['formatter'] is None:
             if kwargs['nullable']:
                 if isinstance(kwargs['datatypes'], (list, tuple)):
                     kwargs['datatypes'] = tuple(kwargs['datatypes']) + (type(None), )
                 else:
```

### Comparing `tksheet-6.0.1/tksheet/_tksheet_other_classes.py` & `tksheet-6.0.2/tksheet/_tksheet_other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/tksheet/_tksheet_row_index.py` & `tksheet-6.0.2/tksheet/_tksheet_row_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,14 +540,15 @@
                                                                                 min(orig_selected),
                                                                                 new_selected[0],
                                                                                 new_selected[-1],
                                                                                 sorted(orig_selected)))))
                     self.MT.main_table_redraw_grid_and_text(redraw_header = True, redraw_row_index = True)
                     if self.ri_extra_end_drag_drop_func is not None:
                         self.ri_extra_end_drag_drop_func(EndDragDropEvent("end_row_index_drag_drop", tuple(orig_selected), new_selected, int(r)))
+                    self.event_generate("<<SheetDataChangeEvent>>")
                         
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y = event.y)
             if r is not None and r < len(self.MT.row_positions) - 1 and r == self.b1_pressed_loc and self.b1_pressed_loc != self.closed_dropdown:
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 if (self.canvasy(event.y) < self.MT.row_positions[r] + self.MT.txt_h and
                     (
@@ -1467,14 +1468,15 @@
                                                                             (((r, 0, r + 1, len(self.MT.col_positions) - 1), "rows"), ),
                                                                             self.MT.currently_selected()))))
                 self.set_cell_data(datarn = datarn, value = value)
         if cell_resize and self.MT.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r, only_set_if_too_small = False)
         if redraw:
             self.MT.refresh()
+        self.event_generate('<<SheetDataChangeEvent>>')
 
     def set_cell_data(self, datarn = None, value = ""):
         if isinstance(self.MT._row_index, int):
             self.MT.set_cell_data(datarn = datarn, datacn = self.MT._row_index, value = value)
         else:
             self.fix_index(datarn)
             if datarn in self.cell_options and 'checkbox' in self.cell_options[datarn]:
```

### Comparing `tksheet-6.0.1/tksheet/_tksheet_top_left_rectangle.py` & `tksheet-6.0.2/tksheet/_tksheet_top_left_rectangle.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/tksheet/_tksheet_vars.py` & `tksheet-6.0.2/tksheet/_tksheet_vars.py`

 * *Files identical despite different names*

### Comparing `tksheet-6.0.1/tksheet.egg-info/PKG-INFO` & `tksheet-6.0.2/tksheet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tkinter table / sheet widget
 Home-page: https://github.com/ragardner/tksheet
-Download-URL: https://github.com/ragardner/tksheet/archive/6.0.1.tar.gz
+Download-URL: https://github.com/ragardner/tksheet/archive/6.0.2.tar.gz
 Author: ragardner
 Author-email: github@ragardner.simplelogin.com
 License: MIT
 Keywords: tkinter,table,widget,sheet,grid,tk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -48,14 +48,15 @@
 - Cell values can potentially be [any class](https://github.com/ragardner/tksheet/wiki#cell-formatting), the default is any class with a `__str__` method
 - Drag and drop columns and rows
 - Multiple line header and index cells
 - Expand row heights and column widths
 - Change fonts and font size (not for individual cells)
 - Change any colors in the sheet
 - Create an unlimited number of high performance dropdown and check boxes
+- [Hide rows and/or columns](https://github.com/ragardner/tksheet/wiki#example-header-dropdown-boxes-and-row-filtering)
 - Left `"w"`, Center `"center"` or Right `"e"` text alignment for any cell/row/column
 
 ### **light blue theme**
 ----
 
 ![alt text](https://i.imgur.com/ojU3IQi.jpeg)
```

