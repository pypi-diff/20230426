# Comparing `tmp/tbpy-1.1.tar.gz` & `tmp/tbpy-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbpy-1.1.tar", last modified: Tue Apr 25 21:32:16 2023, max compression
+gzip compressed data, was "tbpy-1.2.tar", last modified: Tue Apr 25 21:49:27 2023, max compression
```

## Comparing `tbpy-1.1.tar` & `tbpy-1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:32:16.887280 tbpy-1.1/
--rw-rw-rw-   0        0        0     1091 2022-11-08 18:13:24.000000 tbpy-1.1/LICENSE
--rw-rw-rw-   0        0        0      848 2023-04-25 21:32:16.887280 tbpy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0      256 2023-04-23 21:50:50.000000 tbpy-1.1/README.md
--rw-rw-rw-   0        0        0      506 2023-04-25 21:28:38.000000 tbpy-1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-25 21:32:16.887280 tbpy-1.1/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-04-25 21:28:41.000000 tbpy-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:32:16.835975 tbpy-1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 21:32:16.857829 tbpy-1.1/src/tbpy/
--rw-rw-rw-   0        0        0    10585 2023-04-25 21:28:26.000000 tbpy-1.1/src/tbpy/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-04-23 17:14:55.000000 tbpy-1.1/src/tbpy/test.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:32:16.877465 tbpy-1.1/src/tbpy.egg-info/
--rw-rw-rw-   0        0        0      848 2023-04-25 21:32:16.000000 tbpy-1.1/src/tbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-04-25 21:32:16.000000 tbpy-1.1/src/tbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:32:16.000000 tbpy-1.1/src/tbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 21:32:16.000000 tbpy-1.1/src/tbpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-25 21:32:16.000000 tbpy-1.1/src/tbpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 21:32:16.881471 tbpy-1.1/tests/
--rw-rw-rw-   0        0        0       88 2023-04-25 20:57:58.000000 tbpy-1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.790647 tbpy-1.2/
+-rw-rw-rw-   0        0        0     1091 2022-11-08 18:13:24.000000 tbpy-1.2/LICENSE
+-rw-rw-rw-   0        0        0      830 2023-04-25 21:49:27.789649 tbpy-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-04-25 21:35:19.000000 tbpy-1.2/README.md
+-rw-rw-rw-   0        0        0      506 2023-04-25 21:48:33.000000 tbpy-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:49:27.790647 tbpy-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-04-25 21:48:38.000000 tbpy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.699295 tbpy-1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.735033 tbpy-1.2/src/tbpy/
+-rw-rw-rw-   0        0        0    10628 2023-04-25 21:46:44.000000 tbpy-1.2/src/tbpy/__init__.py
+-rw-rw-rw-   0        0        0     1254 2023-04-25 21:47:51.000000 tbpy-1.2/src/tbpy/test.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.778653 tbpy-1.2/src/tbpy.egg-info/
+-rw-rw-rw-   0        0        0      830 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-25 21:49:27.000000 tbpy-1.2/src/tbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 21:49:27.786684 tbpy-1.2/tests/
+-rw-rw-rw-   0        0        0       88 2023-04-25 20:57:58.000000 tbpy-1.2/tests/test.py
```

### Comparing `tbpy-1.1/LICENSE` & `tbpy-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tbpy-1.1/PKG-INFO` & `tbpy-1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbpy
-Version: 1.1
+Version: 1.2
 Summary: Welcome to terminalbreaker
 Home-page: https://github.com/Ellicode/terminalbreaker
 Author: Ellicode
 Author-email: Ellicode <ellicode22@gmail.com>
 Project-URL: Homepage, https://github.com/Ellicode/terminalbreaker
 Project-URL: Bug Tracker, https://github.com/Ellicode/terminalbreaker/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 ![screen recording](screenrecord.gif)
 
-## `pip install terminalbreaker-python`
+## `pip install tbpy`
 
 TerminalBreaker is a python module to create better guis, forms and more.
 
 [Documentation](https://ellicode.github.io/terminalbreaker)
 
 </div>
```

### Comparing `tbpy-1.1/setup.py` & `tbpy-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "tbpy",
-    version = "1.1",
+    version = "1.2",
     author = "Ellicode",
     author_email = "ellicode22@gmail.com",
     description = "Welcome to terminalbreaker!",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/Ellicode/terminalbreaker",
     project_urls = {
```

### Comparing `tbpy-1.1/src/tbpy/__init__.py` & `tbpy-1.2/src/tbpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         #self.height = int((rows + (len(text.split("\n")) + 4 + len(fields) if fields else 0 + 1 if buttons else 0)))
         self.width = width
         self.fields = fields
         self.tabs = self.buttons + (self.fields if self.fields else [])
         self.text_to_print = ""
 
         self.text_to_print += colorama.Fore.BLUE + (("█" * columns) + "\n") * int(self.pady-5) +  colorama.Style.RESET_ALL
-        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "╭─"  + colorama.Fore.BLACK + Style.BRIGHT + str(name) + Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "─" * ((self.width - 1) - len(str(name))) + "╮"+ colorama.Fore.BLUE + ("█" * (self.padx)) + "█" +  colorama.Style.RESET_ALL +"\n"
+        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "╭─"  + colorama.Fore.BLACK + Style.BRIGHT + str(name) + Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "─" * ((self.width - 1) - len(str(name))) + "╮"+ colorama.Fore.BLUE + ("█" * (self.padx)) + "██" +  colorama.Style.RESET_ALL +"\n"
         if self.fields:
             a=0
             for i in text.split("\n"):
                 if len(str(i)) >= (self.width - 1):
                     raise ValueError("To much text! Text must be less than {} characters (line {})".format(self.width,a))
                 else:
                     self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│ " + colorama.Fore.BLACK + str(i) + " " * ((self.width - 1) - len(str(i))) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX  + "│"+ colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL  + "\n"
@@ -98,29 +98,29 @@
                     raise ValueError("To much text! Text must be less than {} characters (line {})".format(self.width,a))
                 else:
                     self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│ " + colorama.Fore.BLACK + str(i) + " " * ((self.width - 1) - len(str(i))) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│"+ colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL  + "\n"
                 a+=1
             self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│ " + colorama.Fore.BLACK + str(text.split("\n")[-1]) + " " * ((self.width - 1) - len(str(text.split("\n")[-1]))) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│" + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL 
 
         
-        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "├"+ ("─" * self.width) + "┤" + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL  + "\n"
+        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) + "█" +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "├"+ ("─" * self.width) + "┤" + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) + "█" +  colorama.Style.RESET_ALL  + "\n"
         self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "│ "
         self.buttonpad = 1
         for i in self.buttons:
             if self.tabindex == self.tabs.index(i):
                 self.text_to_print += colorama.Back.BLUE + "< " + str(i["text"]) + " >" + Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "     "
                 self.buttonpad+=len(str( "< " + str(i["text"]) + " >" + "     "))
             else:
                 self.text_to_print += colorama.Fore.BLACK + "< "+ str(i["text"]) + " >" + Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "     "
                 self.buttonpad+=len(str( "< " + str(i["text"]) + " >" + "     "))
             #  + " " * ((self.width - 1) - len(str(i))) + "│\n"
             # + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL  + "\n"
-        self.text_to_print += (width - int(self.buttonpad))*" " +  "│"+ colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL + "\n"
-        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "╰" + ("─" * self.width) + "╯" + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL  + "\n"
-        self.text_to_print += colorama.Fore.BLUE + ("█" * (self.padx+1)) +  colorama.Style.RESET_ALL + colorama.Fore.BLACK + colorama.Back.BLUE + ("▀" * self.width) + "▀▀" + colorama.Fore.BLUE + ("█" * (self.padx)) +  colorama.Style.RESET_ALL + "\n"
+        self.text_to_print += (width - int(self.buttonpad))*" " +  "│"+ colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) + "█" +  colorama.Style.RESET_ALL + "\n"
+        self.text_to_print += colorama.Fore.BLUE + ("█" * self.padx) +  colorama.Style.RESET_ALL + colorama.Back.LIGHTWHITE_EX + "╰" + ("─" * self.width) + "╯" + colorama.Fore.BLACK + "█" + colorama.Fore.BLUE + ("█" * (self.padx)) + "█" +  colorama.Style.RESET_ALL  + "\n"
+        self.text_to_print += colorama.Fore.BLUE + ("█" * (self.padx+1)) +  colorama.Style.RESET_ALL + colorama.Fore.BLACK + colorama.Back.BLUE + ("▀" * self.width) + "▀▀" + colorama.Fore.BLUE + ("█" * (self.padx)) + "█" +  colorama.Style.RESET_ALL + "\n"
         self.text_to_print += colorama.Fore.BLUE + ("█" * columns) * self.pady +  colorama.Style.RESET_ALL
         if not self.destroyed:
             # for i in range(len(self.text_to_print.split("\n"))):
             #     delete_last_line()
             print(self.text_to_print,end="\r"*self.height)
```

### Comparing `tbpy-1.1/src/tbpy/test.py` & `tbpy-1.2/src/tbpy/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from __init__ import *
+from tbpy import *
 
-# def window1(init = False):
-#     global win
-#     if not init:
-#         win2.destroy()
+def window1(init = False):
+    global win
+    if not init:
+        win2.destroy()
 
-#     win = __init__.Window("Window 1",f"""Lorem ipsum dolor sit amet, consectetur adipiscing elit,
-# sed do eiusmod tempor incididunt ut labore et dolore magna
-# aliqua. Ut ornare lectus sit amet est. Interdum
-# consectetur libero id faucibus nisl tincidunt eget nullam
-# non. Et ultrices neque ornare aenean euismod elementum 
-# nisi. Ac placerat vestibulum lectus mauris ultrices eros.
-# Hendrerit dolor magna eget est. Sed viverra tellus in hac
-# habitasse. Ut tristique et egestas quis ipsum suspendisse
-# ultrices gravida. Sit amet purus gravida quis blandit
-# turpis cursus. Gravida neque convallis a cras semper
-# auctor neque.""",
-#     width=70,
-#     buttons = [{"text":"Switch","type":"button","action":window2}],
-#     fields=[{"name":"Username","type":"field", "hide": False},{"name":"Password","type":"field","hide":True}]
-#     )
-#     win.mainloop()
-# def window2():
-#     global win2
-#     win.destroy()
-#     win2 = __init__.Window("Window 2","""Hello!""",
-#     width=40,
-#     buttons = [{"text":"Switch","type":"button","action":window1}],
-#     )
-#     win2.mainloop()
-# window1(init=True)
+    win = Window("Window 1",f"""Lorem ipsum dolor sit amet, consectetur adipiscing elit,
+sed do eiusmod tempor incididunt ut labore et dolore magna
+aliqua. Ut ornare lectus sit amet est. Interdum
+consectetur libero id faucibus nisl tincidunt eget nullam
+non. Et ultrices neque ornare aenean euismod elementum 
+nisi. Ac placerat vestibulum lectus mauris ultrices eros.
+Hendrerit dolor magna eget est. Sed viverra tellus in hac
+habitasse. Ut tristique et egestas quis ipsum suspendisse
+ultrices gravida. Sit amet purus gravida quis blandit
+turpis cursus. Gravida neque convallis a cras semper
+auctor neque.""",
+    width=70,
+    buttons = [{"text":"Switch","type":"button","action":window2}],
+    fields=[{"name":"Username","type":"field", "hide": False},{"name":"Password","type":"field","hide":True}]
+    )
+    win.mainloop()
+def window2():
+    global win2
+    win.destroy()
+    win2 = Window("Window 2","""Hello!""",
+    width=40,
+    buttons = [{"text":"Switch","type":"button","action":window1}],
+    )
+    win2.mainloop()
+window1(init=True)
 
-win = Window("Title of the window", "Hello, world!")
-win.mainloop()
+# win = Window("Title of the window", "Hello, world!")
+# win.mainloop()
```

### Comparing `tbpy-1.1/src/tbpy.egg-info/PKG-INFO` & `tbpy-1.2/src/tbpy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tbpy
-Version: 1.1
+Version: 1.2
 Summary: Welcome to terminalbreaker
 Home-page: https://github.com/Ellicode/terminalbreaker
 Author: Ellicode
 Author-email: Ellicode <ellicode22@gmail.com>
 Project-URL: Homepage, https://github.com/Ellicode/terminalbreaker
 Project-URL: Bug Tracker, https://github.com/Ellicode/terminalbreaker/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,14 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
 
 ![screen recording](screenrecord.gif)
 
-## `pip install terminalbreaker-python`
+## `pip install tbpy`
 
 TerminalBreaker is a python module to create better guis, forms and more.
 
 [Documentation](https://ellicode.github.io/terminalbreaker)
 
 </div>
```

