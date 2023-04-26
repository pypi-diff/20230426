# Comparing `tmp/extended_tk-0.11.0-py3-none-any.whl.zip` & `tmp/extended_tk-0.12.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7071 bytes, number of entries: 7
+Zip file size: 7174 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat     9452 b- defN 23-Apr-24 19:44 TkPlus/__init__.py
--rw-rw-rw-  2.0 fat     9452 b- defN 23-Apr-24 19:44 extended_tk/__init__.py
--rw-rw-rw-  2.0 fat      243 b- defN 23-Apr-24 20:18 extended_tk-0.11.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      810 b- defN 23-Apr-24 20:18 extended_tk-0.11.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-24 20:18 extended_tk-0.11.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-24 20:18 extended_tk-0.11.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-Apr-24 20:18 extended_tk-0.11.0.dist-info/RECORD
-7 files, 20625 bytes uncompressed, 6067 bytes compressed:  70.6%
+-rw-rw-rw-  2.0 fat     9652 b- defN 23-Apr-25 19:02 extended_tk/__init__.py
+-rw-rw-rw-  2.0 fat      243 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      810 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/RECORD
+7 files, 20825 bytes uncompressed, 6170 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: TkPlus/__init__.py
 Comment: 
 
 Filename: extended_tk/__init__.py
 Comment: 
 
-Filename: extended_tk-0.11.0.dist-info/LICENSE
+Filename: extended_tk-0.12.0.dist-info/LICENSE
 Comment: 
 
-Filename: extended_tk-0.11.0.dist-info/METADATA
+Filename: extended_tk-0.12.0.dist-info/METADATA
 Comment: 
 
-Filename: extended_tk-0.11.0.dist-info/WHEEL
+Filename: extended_tk-0.12.0.dist-info/WHEEL
 Comment: 
 
-Filename: extended_tk-0.11.0.dist-info/top_level.txt
+Filename: extended_tk-0.12.0.dist-info/top_level.txt
 Comment: 
 
-Filename: extended_tk-0.11.0.dist-info/RECORD
+Filename: extended_tk-0.12.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extended_tk/__init__.py

```diff
@@ -28,20 +28,27 @@
         self.delete = Button(
             master, text='-',
             font=(textFont, int((textSize)*scale)),
             state=DISABLED, width=self.add['width'],
             command=self.__del_row
         )
         self.delete.grid(row=master.grid_size()[1]-1, column=master.grid_size()[0]+1)
-    
+        
+    def __copiable(self, item):
+        no_copy = [Button, Frame]
+        for type in no_copy:
+            if isinstance(item, type):
+                return False
+        return True
+            
     def __add_row(self):
         '''
         Adds a new row with the same items in the row below
         '''
-        to_copy = [i for i in self.__dic if not isinstance(i, Button) and i.grid_info()['row']==self.__row-1]
+        to_copy = [i for i in self.__dic if self.__copiable(i) and i.grid_info()['row']==self.__row-1]
         for item in to_copy:
             new = type(item)(self.master)
             for key in list(item.keys())[:-1]:
                 try:
                     new.config({key: item[key]})
                     try:
                         new.current(0)
```

## Comparing `extended_tk-0.11.0.dist-info/METADATA` & `extended_tk-0.12.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extended-tk
-Version: 0.11.0
+Version: 0.12.0
 Summary: An add on for the tkinter package
 Home-page: UNKNOWN
 Author: Elidas
 License: GNUGPLv3
 Keywords: Tkinter
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `extended_tk-0.11.0.dist-info/RECORD` & `extended_tk-0.12.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 TkPlus/__init__.py,sha256=fAwcO_zH-AjYKskxRbSUn8TYHsPlVYhs-EybaQDFEw0,9452
-extended_tk/__init__.py,sha256=fAwcO_zH-AjYKskxRbSUn8TYHsPlVYhs-EybaQDFEw0,9452
-extended_tk-0.11.0.dist-info/LICENSE,sha256=EEAxqxJsjMTyZM0BicuoXjdyUB4VE45rvk83t_jv4uw,243
-extended_tk-0.11.0.dist-info/METADATA,sha256=_pPC8J5KdP7sVdc68O27oEpY-X0XmiJCSECxjV5yVyY,810
-extended_tk-0.11.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extended_tk-0.11.0.dist-info/top_level.txt,sha256=A40P8PzvnRpYXa0VqJc51K-aiI4LicWN2h8yzvJfO9Q,12
-extended_tk-0.11.0.dist-info/RECORD,,
+extended_tk/__init__.py,sha256=hBnVgf6-6YS2jsCQlBWwgv-TwoJXteJ-9brF_9hrceQ,9652
+extended_tk-0.12.0.dist-info/LICENSE,sha256=EEAxqxJsjMTyZM0BicuoXjdyUB4VE45rvk83t_jv4uw,243
+extended_tk-0.12.0.dist-info/METADATA,sha256=cKFl3HvBI3azW7EVInA9Pl6uywDlHzuHCgY1U-4ITDI,810
+extended_tk-0.12.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extended_tk-0.12.0.dist-info/top_level.txt,sha256=A40P8PzvnRpYXa0VqJc51K-aiI4LicWN2h8yzvJfO9Q,12
+extended_tk-0.12.0.dist-info/RECORD,,
```

