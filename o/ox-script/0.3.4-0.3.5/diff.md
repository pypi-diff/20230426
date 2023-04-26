# Comparing `tmp/ox_script-0.3.4.tar.gz` & `tmp/ox_script-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ox_script-0.3.4.tar", last modified: Sat Apr 22 22:41:55 2023, max compression
+gzip compressed data, was "dist/ox_script-0.3.5.tar", last modified: Wed Apr 26 16:55:48 2023, max compression
```

## Comparing `ox_script-0.3.4.tar` & `ox_script-0.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:41:55.000000 ox_script-0.3.4/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 22:41:55.000000 ox_script-0.3.4/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.4/MANIFEST.in
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script/
--rw-------   0 jarvislu   (501) staff       (20)    12241 2023-04-22 22:41:41.000000 ox_script-0.3.4/ox_script/general_purpose_apis.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 22:41:41.000000 ox_script-0.3.4/ox_script/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    25033 2023-04-22 22:41:41.000000 ox_script-0.3.4/ox_script/printer_specific_apis.py
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      275 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       10 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-22 22:41:55.000000 ox_script-0.3.4/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-22 22:41:47.000000 ox_script-0.3.4/setup.py
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-22 22:41:55.000000 ox_script-0.3.4/setup.cfg
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-26 16:55:48.000000 ox_script-0.3.5/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-26 16:55:48.000000 ox_script-0.3.5/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-0.3.5/MANIFEST.in
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script/
+-rw-------   0 jarvislu   (501) staff       (20)    12256 2023-04-26 16:53:14.000000 ox_script-0.3.5/ox_script/general_purpose_apis.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 22:41:41.000000 ox_script-0.3.5/ox_script/__init__.py
+-rw-------   0 jarvislu   (501) staff       (20)    36772 2023-04-26 16:51:23.000000 ox_script-0.3.5/ox_script/printer_specific_apis.py
+drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/
+-rw-r--r--   0 jarvislu   (501) staff       (20)      743 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/PKG-INFO
+-rw-r--r--   0 jarvislu   (501) staff       (20)      275 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/SOURCES.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       16 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/requires.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)       10 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/top_level.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)        1 2023-04-26 16:55:48.000000 ox_script-0.3.5/ox_script.egg-info/dependency_links.txt
+-rw-r--r--   0 jarvislu   (501) staff       (20)      875 2023-04-26 16:55:46.000000 ox_script-0.3.5/setup.py
+-rw-r--r--   0 jarvislu   (501) staff       (20)       38 2023-04-26 16:55:48.000000 ox_script-0.3.5/setup.cfg
```

### Comparing `ox_script-0.3.4/PKG-INFO` & `ox_script-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox_script
-Version: 0.3.4
+Version: 0.3.5
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.4/ox_script/general_purpose_apis.py` & `ox_script-0.3.5/ox_script/general_purpose_apis.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # ===========================================================#
 # General purpose functions
 # These functions can be executed directly on your device
 # and is designed to help you with data parsing, connecting to
 # databases, and getting data in the format to be printed
 # ===========================================================#
 
-import pandas
+from pandas import DataFrame
 import openpyxl
 import os
 import re
 
 # This class defines the basis of a database to be used like this
 # data_base = PTKDataBase()
 # data_base.read_excel_file("example/path/example_file.xlsx")
@@ -58,15 +58,15 @@
         return self.data.__str__()
 
     def pprint(self, col_spacing=10) -> str:
         returnStr = "{"
         for key in self.data:
             returnStr += "\n"
             returnStr += f"  Table Name : {key} \n"
-            lines = pandas.DataFrame(
+            lines = DataFrame(
                 self.data[key].data_table).to_string(col_space=col_spacing)
             for line in lines.split("\n"):
                 returnStr += f"\n\t{line}"
             returnStr += "\n\n"
             returnStr += "------------------------------------------------------------"
             returnStr += "\n"
         returnStr = returnStr.rsplit(
@@ -90,16 +90,14 @@
                 else:
                     column.append(str(cell[0].value).strip())
             if column_name != "" and len(column) != 0:
                 temp[column_name] = column
         self.data[base_path] = DataBaseEntry(temp)
 
 # This class defines the basis for an entry in the data base, not to be used directly
-
-
 class DataBaseEntry:
     def __init__(self, data_table: map):
         self.data_table = data_table
 
     def __str__(self) -> str:
         return self.data_table.__str__()
 
@@ -223,18 +221,18 @@
 # the data on the label
 # ===========================================================#
 
 
 basepath = ""
 
 
-def get_all_form_variables(filepath) -> dict:
+def PTK_GetAllFormVariables(filepath) -> dict:
     """
-    get_all_form_variables is used to retrive all the variables in the form so they can be
-        updated with the update_all_form_variables function.
+    PTK_GetAllFormVariables is used to retrive all the variables in the form so they can be
+        updated with the PTK_UpdateAllFormVariables function.
 
     Parameters:
         filepath (string): The path to the form file. The form file can be generated by
             label editing softwares and just place the form file next to the script so
             the relative path can be accessed
 
     Returns:
@@ -271,41 +269,41 @@
                                         "line": line,
                                         "replacement_key": key,
                                     }
                                 )
         return variable_locations
 
 
-def update_all_form_variables(filename, **kwargs) -> str:
+def PTK_UpdateAllFormVariables(filename, **kwargs) -> str:
     """
-    update_all_form_variables is used to update all the variables in the form
+    PTK_UpdateAllFormVariables is used to update all the variables in the form
 
     Parameters:
         filename (string): The name of the form file. The form file can be generaed by
             label editing softwares and just place the form file next to the script so
             the relative path can be accessed
         **kwargs: The key value pair of the variables to be updated
 
     e.x.:
-        cmd = update_all_form_variables(
+        cmd = PTK_UpdateAllFormVariables(
                 'command1.txt',
                 Input1=data[0],
                 Input2=data[1],
             )
         PTK_SendCmdToPrinter(cmd)
         where 'command1.txt' is the form file name and 'Input1' and 'Input2' are the variables
             name defined when the form file is generated
 
     Returns:
         str: The updated form file in string that can be sent to the printer through the function
             PTK_SendCmdToPrinter
     """
     filepath = basepath + filename
     if os.access(filepath, os.F_OK):
-        variable_locations = get_all_form_variables(filepath)
+        variable_locations = PTK_GetAllFormVariables()(filepath)
         with open(filepath, "r") as text_file:
             lines = [line for line in text_file]
             for key, value in kwargs.items():
                 if key in variable_locations.keys():
                     for items in variable_locations[key]:
                         position = items["position"]
                         line = items["line"]
```

### Comparing `ox_script-0.3.4/ox_script/printer_specific_apis.py` & `ox_script-0.3.5/ox_script/printer_specific_apis.py`

 * *Files 27% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # The functions are marked with pass only because they are meanted to be executed on the printer and will not function
 # correctly on your device. Please use the runtime environment on Postek printers for most accurate results
 
 
 # --coding: utf-8 --
 import string
 
+
 def debuglog(info: str):
     """
     Log the information to the debug log file stored inside the printer
 
     Parameters:
         info (str): The information to be logged
     """
@@ -48,14 +49,27 @@
 
     Parameters:
         unit (int): The unit of measurement to be used. 0 -> mm, 1 -> dots
     """
     pass
 
 
+def mmOrDots(value):
+    """
+    mmOrDots is used to convert the value to the unit of measurement that is currently being used
+
+    Parameters:
+        value (float): The value to be converted
+
+    Returns:
+        int: The converted value
+    """
+    return int(value)
+
+
 def PTK_GetErrorInfo():
     """
     PTK_GetErrorInfo is used to get the error information from the printer
 
     """
     pass
 
@@ -175,15 +189,20 @@
     Returns:
         int: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
 
-def PTK_SetLabelHeight(height: int, gapH=1) -> bool:
+GAP_MODE = 0
+SPECIAL_MODE = 1
+BLACK_LINE_MODE = 2
+
+
+def PTK_SetLabelHeight(height, mode=GAP_MODE, gapH=3) -> bool:
     """
     PTK_SetLabelHeight is used to set the height of the label.
 
     Parameters:
         height (int): The height of the label in mm
         gapH (int): The gap between the labels in mm
 
@@ -260,49 +279,47 @@
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
 
 def PTK_DrawText(
-    x_coordinate: int,
-    y_coordinate: int,
-    fonts: string,
-    font_size: int,
+    x_coordinate: float,
+    y_coordinate: float,
     data: string,
+    fonts="1",
+    font_size=3,
     text_style="N",
     rotation=0,
-    horizontal_multiplier=-1,
 ) -> bool:
     """
     PTK_DrawText is used to print text on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the text
         y_coordinate (int): The y coordinate of the text
+        data (string): The text to be printed
         fonts (string): The font to be used. i.e "Inter", the Font should be stored in the fonts folder on the printer
         font_size (int): The size of the font
-        data (string): The text to be printed
         text_style (string): The style of the text. "N" -> Normal, "R" -> Reverse
         rotation (int): The rotation of the text. The range is 0 to 360
-        horizontal_multiplier (int): The horizontal multiplier of the text. The range is 1 to 10
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
 # ===========================================================#
 # 2D Barcode related functions
 # ===========================================================#
 
 
 def PTK_DrawBar2D_DATAMATRIX(
-    x_coordinate: int, y_coordinate: int, multiplier: int, data: string, rotation=0
+    x_coordinate: float, y_coordinate: float, multiplier: int, data: string, rotation=0
 ) -> bool:
     """
     PTK_DrawBar2D_DATAMATRIX is used to print a DataMatrix barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
@@ -353,58 +370,56 @@
 
 
 UPS = 1
 NOT_UPS = 0
 
 
 def PTK_DrawBar2D_MaxiCode(
-    x_coordinate: int, y_coordinate: int, mode: int, is_ups_data: int, data: string
+    x_coordinate: float, y_coordinate: float, is_ups_data: int, data: string, mode=4
 ) -> bool:
     """
     PTK_DrawBar2D_MaxiCode is used to print a MaxiCode barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
-        mode (int): The mode of the barcode. The range is 2 to 4
         is_ups_data (int): The ups data of the barcode. 0 -> Not UPS, 1 -> UPS
         data (string): The data to be printed in the barcode
+        mode (int): The mode of the barcode. The range is 2 to 4
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
 
 def PTK_DrawBar2D_Pdf417(
-    x_coordinate: int,
-    y_coordinate: int,
+    x_coordinate: float,
+    y_coordinate: float,
     correction_level: int,
-    data_compression_level: int,
     px: int,
     py: int,
-    maxrow: int,
-    maxcolumn: int,
+    encode_row: int,
+    encode_column: int,
     t: int,
     data: string,
     rotation=0,
 ) -> bool:
     """
     PTK_DrawBar2D_Pdf417 is used to print a Pdf417 barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
         y_coordinate (int): The y coordinate of the barcode
         correction_level (int): The correction level of the barcode. The range is 0 to 8
-        data_compression_level (int): The data compression level of the barcode. The range is 0 to 1
         px (int): The px of the barcode. The range is 2 to 9
         py (int): The py of the barcode. The range is 4 to 99
-        maxrow (int): The maxrow of the barcode. The range is 3 to 90
-        maxcolumn (int): The maxcolumn of the barcode. The range is 1 to 30
+        encode_row (int): The maxrow of the barcode. The range is 3 to 90
+        encode_column (int): The maxcolumn of the barcode. The range is 1 to 30
         t (int): Truncation of the barcode. i.e 0 -> No truncation, 1 -> Truncation
         data (string): The data to be printed in the barcode
         rotation (int): The rotation of the barcode. The range is 0 to 3 where
             0 = 0 degree, 1 = 90 degree, 2 = 180 degree, 3 = 270 degree
 
     Returns:
         bool: The function executed successfully
@@ -450,22 +465,22 @@
 # ===========================================================#
 
 NO_TEXT = "N"
 TEXT = "B"
 
 
 def PTK_DrawBarcode(
-    x_coordinate: int,
-    y_coordinate: int,
+    x_coordinate: float,
+    y_coordinate: float,
     barcode_type: string,
-    narrow_unit_width: int,
     wide_unit_width: int,
+    barcode_height: int,
     data: string,
     human_readable=TEXT,
-    bar_height=10,
+    narrow_unit_width=0.1,
     rotation=0,
 ) -> bool:
     """
     PTK_DrawBarcode is used to print a 1D barcode on the label
 
     Parameters:
         x_coordinate (int): The x coordinate of the barcode
@@ -521,29 +536,48 @@
     return True
 
 
 # ===========================================================#
 # Printing graphics
 # ===========================================================#
 
-def PTK_DrawGraphics(x, y, graphic_name):
+def PTK_DrawGraphics(x, y, graphic_name) -> bool:
     """
     PTK_DrawGraphics is used to print a graphic on the label
 
     Parameters:
         x (int): The x coordinate of the graphic
         y (int): The y coordinate of the graphic
         graphic_name (string): The name of the graphic that is stored in the printer
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
+
+def PTK_DrawGraphicsFromBytes(x, y, graphic_data, isbase64=False):
+    """
+    PTK_DrawGraphicsFromBytes
+    PTK_DrawGraphicsFromBytes is used to print a graphic on the label
+
+    Parameters:
+        x (int): The x coordinate of the graphic
+        y (int): The y coordinate of the graphic
+        isbase64 (bool): If the Data is base64 encoded, is it is the function will
+            perform a base64 decode on the data before sending it to the printer
+        graphic_data (string): The data of the graphic
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
 # ===========================================================#
 # Printing lines
 # ===========================================================#
 
 
 def PTK_DrawDiagonal(
     x_coordinate: int,
@@ -630,151 +664,489 @@
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
+
 def PTK_MediaCalibration() -> bool:
     """
     PTK_MediaCalibration is used to calibrate the media. If the calibration is successful the
     media size information will be stored and used for the next printjob unless specificed through
     PTK_SetLabelHeight or specificed through print job configuration
 
     Returns:
         bool: The function executed successfully
         String: The error message in string if an error occured
     """
     return True
 
 # ===========================================================#
+# RFID打印标签
+# ===========================================================#
+
+
+def PTK_RFIDCalibrate() -> bool:
+    """
+    PTK_RFIDCalibrate is used to calibrate the RFID tag. If the calibration is successful the
+    RFID tag information will be stored and used for the next printjob unless specificed through
+    print job configuration
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
+
+def PTK_RWRFIDLabel(RWMode, WForm, StartBlock, WDataNum, WArea, data) -> bool:
+    """
+    PTK_RWRFIDLabel is used to read and write data to the RFID tag
+
+    Parameters:
+        RWMode (int): 0 = read, 1 = write
+        WForm (int): 0 = ASCII, 1 = HEX
+        StartBlock (int): The start block to read or write
+        WDataNum (int): The number of blocks to read or write
+        WArea (int): 0 = EPC, 1 = TID, 2 = USER
+        data (string): The data to be written to the RFID tag
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
+
+def PTK_SetRFLabelPWAndLockRFLabel(OperationMode, OperationArea, data) -> bool:
+    """
+    PTK_SetRFLabelPWAndLockRFLabel is used to set the password and lock the RFID tag
+
+    Parameters:
+        OperationMode (int): 0 = set password, 1 = lock
+        OperationArea (int): 0 = EPC, 1 = TID, 2 = USER
+        data (string): The password to be set
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
+
+def PTK_SetRFID(
+    ReservationParameters,
+    ReadWriteLocation,
+    ReadWriteArea,
+    MaxErrNum,
+    ErrProcessingMethod,
+) -> bool:
+    """
+    PTK_SetRFID is used to set the RFID tag parameters
+
+    Parameters:
+        ReservationParameters (int): 0 = no reservation, 1 = reservation
+        ReadWriteLocation (int): 0 = read and write, 1 = read only
+        ReadWriteArea (int): 0 = EPC, 1 = TID, 2 = USER
+        MaxErrNum (int): The maximum number of errors allowed
+        ErrProcessingMethod (int): 0 = stop printing, 1 = continue printing
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
+
+def PTK_SetRFIDCmdMode(flag) -> bool:
+    """
+    PTK_SetRFIDCmdMode is used to set the RFID command mode
+
+    Parameters:
+        flag (int): 0 = normal mode, 1 = command mode
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return True
+
+
+TID = 0
+EPC = 1
+TID_EPC = 2
+USER = 3
+TID_USER = 4
+RESERVED = 5
+TID_RESERVED = 6
+PORT_SCRIPT = 3
+
+
+def PTK_SetPortback(port=PORT_SCRIPT) -> bool:
+    """
+    PTK_SetPortback is used to set the port to return information
+
+    Parameters:
+        port (int): defined as follows:
+            TID = 0
+            EPC = 1
+            TID_EPC = 2
+            USER = 3
+            TID_USER = 4
+            RESERVED = 5
+            TID_RESERVED = 6
+            PORT_SCRIPT = 3
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+
+    """
+    return True
+
+
+def PTK_GetPrinterStatus() -> bool:
+    """
+    PTK_GetPrinterStatus is used to get the printer status
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+    """
+    return False
+
+
+def PTK_ReadRFID(block=TID, comm_mode=3, auto_foward=False, len=10):
+    """
+    PTK_ReadRFID is used to read the RFID tag
+
+    Parameters:
+        block (int): 0 = TID, 1 = EPC, 2 = USER
+        comm_mode (int): 0 = 9600, 1 = 19200, 2 = 38400, 3 = 57600, 4 = 115200
+        auto_foward (bool): 0 = no auto forward, 1 = auto forward
+        len (int): The length of the data to be read
+    """
+    return "RFID Data will be read on printer"
+
+
+def PTK_SetEPCBlock(allnum, p1, p2, p3, p4, p5, p6):
+    """
+    PTK_SetEPCBlock is used to set the EPC block
+
+    Parameters:
+        allnum (int): The total number of blocks
+        p1 (int): The first block
+        p2 (int): The second block
+        p3 (int): The third block
+        p4 (int): The fourth block
+        p5 (int): The fifth block
+        p6 (int): The sixth block
+
+    Returns:
+        bool: The function executed successfully
+
+    """
+    return True
+
+
+def PTK_WriteRFID(data_mode, start_addr, len, block, data):
+    """
+    PTK_WriteRFID is used to write data to the RFID tag
+
+    Parameters:
+        data_mode (int): 0 = ASCII, 1 = HEX
+        start_addr (int): The start address to write
+        len (int): The length of the data to be written
+        block (int): 0 = TID, 1 = EPC, 2 = USER
+        data (string): The data to be written to the RFID tag
+
+    Returns:
+        bool: The function executed successfully
+        String: The error message in string if an error occured
+
+    """
+    return True
+
+# ===========================================================#
 # Functions to display information on the printer screen
 # ===========================================================#
 
 # Parent class of all UI elements
 # This shouldn't be used directly
+
+
 class UIWidgets:
     def __init__(self, name, value, Onpressed):
-        pass
+        self.value = value
+        self.name = name
+        self.Onpressed = Onpressed
+        self.id = 0
+        self.enabled = True
+
+
+    def update(self, value):
+        """
+        update is used to update the value of the UI element on the printer screen
+
+        Parameters:
+            value (string): The value to be updated
+        
+        """
+        self.value = value
+
+    def enable(self):
+        """
+        enable is used to enable the UI element on the printer screen. A disabled UI element 
+            is still visible but can't be interacted with on the printer screen
+
+        """
+        self.enabled = True
+
+    def disable(self):
+        """
+        disable is used to disable the UI element on the printer screen. A disabled UI element 
+            is still visible but can't be interacted with on the printer screen
+
+        """
+        self.enabled = False
 
 # Button class used for creating a button on the printer screen
 # To create UI Elements use UIInit and UIPage
-class UIButton(UIWidgets):
-    def __init__(self, Onpressed, name="测试按钮", visible=True):
-        pass
+class PTK_UIButton(UIWidgets):
+    def __init__(self, Onpressed, title="button", visible=True, enabled=True, name=""):
+        """
+        Parameters:
+            Onpressed (function): The function to be called when the button is pressed
+            title (string): The title of the button that will be displayed on screen
+            visible (bool): Whether the button is visible on the printer screen
+            enabled (bool): Whether the button is enabled on the printer screen
+            name (string): A custom name for button that can be used to identify the button
+        """
+
+        self.type = "button"
+        self.Onpressed = Onpressed
+        self.title = title
+        self.name = name
+        self.value = "0"
+        self.visible = visible
+        self.enabled = enabled
+        self.id = 0
 
 
 # Text class used for just displaying text on the printer screen
 # To create UI Elements use UIInit and UIPage
-class UIText(UIWidgets):
-    def __init__(self, value="--", name="测试文本", visible=True):
-        pass
+class PTK_UIText(UIWidgets):
+    def __init__(self, title="text", visible=True, enabled=True, name=""):
+        """
+        Parameters:
+            title (string): The title of the button that will be displayed on screen
+            visible (bool): Whether the button is visible on the printer screen
+            enabled (bool): Whether the button is enabled on the printer screen
+            name (string): A custom name for button that can be used to identify the button
+        """
+                
+        self.type = "text"
+        self.title = title
+        self.name = name
+        self.visible = visible
+        self.enabled = enabled
+        self.id = 0
+
+
+class PTK_UITextbox(UIWidgets):
+    def __init__(self, value="--", title="Textbox", visible=True, enabled=True, name=""):
+        """
+        Parameters:
+            title (string): The title of the button that will be displayed on screen
+            visible (bool): Whether the button is visible on the printer screen
+            enabled (bool): Whether the button is enabled on the printer screen
+            name (string): A custom name for button that can be used to identify the button
+        """
+        self.type = "text"
+        self.value = value
+        self.title = title
+        self.name = name
+        self.visible = visible
+        self.enabled = enabled
+        self.id = 0
 
 # List class that can be used to create a drop down list on the printer screen
 # To create UI Elements use UIInit and UIPage
-class UIList(UIWidgets):
+class PTK_UIList(UIWidgets):
     def __init__(
         self,
         Onpressed,
-        items,
-        name="testing list",
-        value="0",
+        items=['Add Custom List Items', '0', '1'],
+        title="list",
+        value=["Add Custom List Items"],
         valueType="int",
         valueMax="1",
         valueMin="0",
         visible=True,
-    ):
-        pass
+        enabled=True,
+        name="",
+    ):        
+        """
+        Parameters:
+            Onpressed (function): The function to be called when the button is pressed
+            items (list): The list of items to be displayed in the drop down list
+            title (string): The title of the button that will be displayed on screen
+            value (list): The default value of the drop down list
+            valueType (string): The type of the value of the drop down list
+            valueMax (string): The maximum value of the drop down list
+            valueMin (string): The minimum value of the drop down list
+            visible (bool): Whether the button is visible on the printer screen
+            enabled (bool): Whether the button is enabled on the printer screen
+            name (string): A custom name for button that can be used to identify the button
+        """
+        self.type = "list"
+        self.Onpressed = Onpressed
+        self.items = items
+        self.title = title
+        self.name = name
+        self.value = value
+        self.valueType = valueType
+        self.valueMax = valueMax
+        self.valueMin = valueMin
+        self.visible = visible
+        self.enabled = enabled
+        self.id = 0
 
 # Input class that can be used to create a input box on the printer screen
 # To create UI Elements use UIInit and UIPage
-class UIInput(UIWidgets):
+class PTK_UIInput(UIWidgets):
     def __init__(
         self,
-        Onpressed,
-        name="测试输入",
+        Onsubmit,
+        Onchange="",
+        title="input",
         value="0",
         valueType="double",
         valueMax="10.0",
         valueMin="-10.0",
         dotNum=1,
         visible=True,
+        enabled=True,
+        name="",
     ):
-        pass
+        """
+        Parameters:
+            Onsubmit (function): The function to be called when the button is pressed
+            ONchange (function): The function to be called when the value of the input box is changed
+            title (string): The title of the button that will be displayed on screen
+            value (list): The default value of the drop down list
+            valueType (string): The type of the value of the drop down list
+            valueMax (string): The maximum value of the drop down list
+            valueMin (string): The minimum value of the drop down list
+            visible (bool): Whether the button is visible on the printer screen
+            enabled (bool): Whether the button is enabled on the printer screen
+            name (string): A custom name for button that can be used to identify the button
+        """
+        self.type = "input"
+        self.Onsubmit = Onsubmit
+        self.Onchange = Onchange
+        self.title = title
+        self.name = name
+        self.value = value
+        self.valueType = valueType
+        self.valueMax = valueMax
+        self.valueMin = valueMin
+        self.visible = visible
+        self.dotNum = dotNum
+        self.id = 0
+        self.enabled = enabled
 
 # Checkbox class that can be used to create a checkbox on the printer screen
 # To create UI Elements use UIInit and UIPage
-class UICheckbox(UIWidgets):
+class PTK_UICheckbox(UIWidgets):
     def __init__(
         self,
         Onpressed,
-        name="测试复选框",
+        title="checkbox",
         value="0",
         valueType="bool",
         valueMax="1",
         valueMin="0",
         visible=True,
+        enabled=True,
+        name="",
     ):
-        pass
+        
+        self.type = "checkbox"
+        self.Onpressed = Onpressed
+        self.title = title
+        self.name = name
+        self.value = value
+        self.valueType = valueType
+        self.valueMax = valueMax
+        self.valueMin = valueMin
+        self.visible = visible
+        self.id = 0
+        self.enabled = enabled
 
 
-def UIchangePage(pagenum):
+def PTK_UIchangePage(pagenum):
     """
     UIchangePage can be used to change the page on the printer screen as
         a ox script can be used to create multiple pages
 
     Parameters:
         pagenum (int): The page number to be displayed
     """
     pass
 
-def UIPage(*args) -> dict:
+
+def PTK_UIPage(*args) -> dict:
     """
     UIPage is used to create a page on the printer screen. A page is used to
         group UI elements together. UI elements have to be added to a page to be displayed
         on the printer screen. UI elements needs to be added in the following way
 
-    controller = UIInit(
-        UIPage(
+    controller = PTK_UIInit(
+        PTK_UIPage(
             UIText(name="Barcode One:", value="--"),
             UIText(name="Barcode Two:", value="--"),
         ),
     )
 
     Parameters:
         *args (UIWidgets): The UI elements to be added to the page
 
     Returns:
-        dict: The page in dictionary format, it is meanted to be used with UIInit and not
+        dict: The page in dictionary format, it is meanted to be used with PTK_UIInit and not
             used directly by the user
 
     """
     return {}
 
 # UI初始化
-def UIInit(*params, require_execute_confirmation=True) -> dict:
+
+
+def PTK_UIInit(*params, require_execute_confirmation=True) -> dict:
     """
-    UIInit is used to initialize the UI elements on the printer screen. 
+    PTK_UIInit is used to initialize the UI elements on the printer screen. 
 
     Parameters:
         *params (dict): The pages to be displayed on the printer screen, it should be used in the
             way shown below. The user can create multiple pages and add UI elements to each page
         require_execute_confirmation (bool, optional): If the printer screen should require
-            confirmation before executing the script. Defaults to True.
+            confirmation before executing the script. Defaults to True which requires the user to press 
+            the run script button on the bottom right of the pop up window
 
-    controller = UIInit(
-        UIPage(
+    controller = PTK_UIInit(
+        PTK_UIPage(
             UIText(name="Barcode One:", value="--"),
             UIText(name="Barcode Two:", value="--"),
         ),
-        UIPage(
+        PTK_UIPage(
             UIText(name="Barcode Three:", value="--"),
             UIText(name="Barcode Four:", value="--"),
         ),
     )
-            
+
     Returns:
         controller (dict): The controller for the UI elements. The user can use the controllers
             to change the values of the UI elements on the printer screen
 
     """
-    return {}
+    return {}
```

### Comparing `ox_script-0.3.4/ox_script.egg-info/PKG-INFO` & `ox_script-0.3.5/ox_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: ox-script
-Version: 0.3.4
+Version: 0.3.5
 Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
 Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
 Home-page: https://github.com/POSTEK-OX-Script
 Author: Postek Electronics Co., Ltd.
 Author-email: support@postek.com.cn
 License: MIT
 Description: UNKNOWN
```

### Comparing `ox_script-0.3.4/setup.py` & `ox_script-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ox_script',
-    version='0.3.4',
+    version='0.3.5',
     author='Postek Electronics Co., Ltd.',
     author_email='support@postek.com.cn',
     packages=find_packages(),
     license="MIT",
     description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
     url="https://github.com/POSTEK-OX-Script",
     install_requires=[
```

