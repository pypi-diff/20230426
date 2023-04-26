# Comparing `tmp/tkinteruserinput-0.10.tar.gz` & `tmp/tkinteruserinput-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkinteruserinput-0.10.tar", last modified: Sat Apr  1 13:45:22 2023, max compression
+gzip compressed data, was "tkinteruserinput-0.11.tar", last modified: Wed Apr 26 05:36:51 2023, max compression
```

## Comparing `tkinteruserinput-0.10.tar` & `tkinteruserinput-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 13:45:22.723340 tkinteruserinput-0.10/
--rw-rw-rw-   0        0        0     1148 2023-04-01 13:45:21.000000 tkinteruserinput-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      153 2023-04-01 13:45:20.000000 tkinteruserinput-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     3581 2023-04-01 13:45:22.723340 tkinteruserinput-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     2808 2023-04-01 13:42:56.000000 tkinteruserinput-0.10/README.md
--rw-rw-rw-   0        0        0      115 2023-04-01 13:45:22.724338 tkinteruserinput-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1194 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 13:45:22.716359 tkinteruserinput-0.10/tkinteruserinput/
--rw-rw-rw-   0        0        0     1090 2023-03-31 02:03:52.000000 tkinteruserinput-0.10/tkinteruserinput/LICENSE
--rw-rw-rw-   0        0        0     2808 2023-04-01 13:42:56.000000 tkinteruserinput-0.10/tkinteruserinput/README.MD
--rw-rw-rw-   0        0        0     8365 2023-04-01 13:34:00.000000 tkinteruserinput-0.10/tkinteruserinput/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-01 13:45:22.721346 tkinteruserinput-0.10/tkinteruserinput.egg-info/
--rw-rw-rw-   0        0        0     3581 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-01 13:45:22.000000 tkinteruserinput-0.10/tkinteruserinput.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 05:36:51.484457 tkinteruserinput-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-04-26 05:36:47.000000 tkinteruserinput-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      153 2023-04-26 05:36:46.000000 tkinteruserinput-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     3426 2023-04-26 05:36:51.485454 tkinteruserinput-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2808 2023-04-15 00:17:27.000000 tkinteruserinput-0.11/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-26 05:36:51.485454 tkinteruserinput-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1271 2023-04-26 05:36:50.000000 tkinteruserinput-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 05:36:51.481465 tkinteruserinput-0.11/tkinteruserinput/
+-rw-rw-rw-   0        0        0     1090 2023-04-15 00:17:27.000000 tkinteruserinput-0.11/tkinteruserinput/LICENSE
+-rw-rw-rw-   0        0        0     2808 2023-04-15 00:17:27.000000 tkinteruserinput-0.11/tkinteruserinput/README.MD
+-rw-rw-rw-   0        0        0     8875 2023-04-26 05:34:14.000000 tkinteruserinput-0.11/tkinteruserinput/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 05:36:50.000000 tkinteruserinput-0.11/tkinteruserinput/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 05:36:50.000000 tkinteruserinput-0.11/tkinteruserinput/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-26 05:36:51.483459 tkinteruserinput-0.11/tkinteruserinput.egg-info/
+-rw-rw-rw-   0        0        0     3426 2023-04-26 05:36:51.000000 tkinteruserinput-0.11/tkinteruserinput.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-04-26 05:36:51.000000 tkinteruserinput-0.11/tkinteruserinput.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 05:36:51.000000 tkinteruserinput-0.11/tkinteruserinput.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-26 05:36:51.000000 tkinteruserinput-0.11/tkinteruserinput.egg-info/top_level.txt
```

### Comparing `tkinteruserinput-0.10/LICENSE.rst` & `tkinteruserinput-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `tkinteruserinput-0.10/PKG-INFO` & `tkinteruserinput-0.11/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 Metadata-Version: 2.1
 Name: tkinteruserinput
-Version: 0.10
+Version: 0.11
 Summary: Pop-ups to get input from the user - tkinter
 Home-page: https://github.com/hansalemaos/tkinteruserinput
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: tkinter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Pop-ups to get input from the user - tkinter 
 
-# Pop-ups to get input from the user - tkinter 
-
-## pip install tkinteruserinput
-
-### Tested against Windows 10 / Python 3.10 / Anaconda 
-
-
-
-
-```python
-
-from tkinteruserinput import get_user_input, get_user_input_varbuttons, get_user_input_checkbox, get_user_input_radio, \
-    show_info, show_error, show_warning
-
-if __name__ == '__main__':
-    ################################################
-
-    user_input = get_user_input(
-        linesinputbox=1,
-        size="300x150",
-        title="Input Box Example",
-        textabovebox="Enter your text below:",
-        submitbutton="Submit",
-        regexcheck=r"\d+",
-        showerror=("Error", "This is not a number! Try again!"),
-        showinfo=None,
-        showwarning=None,
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico",
-    )
-    print("User input:", user_input)
-
-    ################################################
-
-    options = ["Option 1", "Option 2", "Option 3"]
-    user_input = get_user_input_varbuttons(
-        options=options,
-        size="300x350",
-        title="Your input",
-        textabovebox="Click a button",
-        buttonwidth=15,
-        buttonheight=3,
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-
-    )
-    print("User input:", user_input)
-    ################################################
-
-    user_input = get_user_input_checkbox(
-        checkbox_options=("Option 1", "Option 2", "Option 3", "Option 4"),
-        size="300x350",
-        title="Your input",
-        textabovebox="Select checkboxes:",
-        submitbutton="Submit",
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-
-    )
-    print("User input:", user_input)
-    ################################################
-    user_input = get_user_input_radio(
-        radio_options=("Option 1", "Option 2", "Option 3", "Option 4"),
-        indexdefault=0,
-        size="300x350",
-        title="Your input",
-        textabovebox="Select a radio button",
-        submitbutton="Submit",
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-    )
-    print("User input:", user_input)
-    ################################################
-    show_info("Titel", "Message")
-    show_error("Titel", "Message")
-    show_warning("Titel", "Message")
-
-
-
-```
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput1.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput2.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/checkboxes.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/clickabutton.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/radiobutton.png?raw=true)
+## pip install tkinteruserinput
+
+### Tested against Windows 10 / Python 3.10 / Anaconda 
+
+
+
+
+```python
+
+from tkinteruserinput import get_user_input, get_user_input_varbuttons, get_user_input_checkbox, get_user_input_radio, \
+    show_info, show_error, show_warning
+
+if __name__ == '__main__':
+    ################################################
+
+    user_input = get_user_input(
+        linesinputbox=1,
+        size="300x150",
+        title="Input Box Example",
+        textabovebox="Enter your text below:",
+        submitbutton="Submit",
+        regexcheck=r"\d+",
+        showerror=("Error", "This is not a number! Try again!"),
+        showinfo=None,
+        showwarning=None,
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico",
+    )
+    print("User input:", user_input)
+
+    ################################################
+
+    options = ["Option 1", "Option 2", "Option 3"]
+    user_input = get_user_input_varbuttons(
+        options=options,
+        size="300x350",
+        title="Your input",
+        textabovebox="Click a button",
+        buttonwidth=15,
+        buttonheight=3,
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+
+    )
+    print("User input:", user_input)
+    ################################################
+
+    user_input = get_user_input_checkbox(
+        checkbox_options=("Option 1", "Option 2", "Option 3", "Option 4"),
+        size="300x350",
+        title="Your input",
+        textabovebox="Select checkboxes:",
+        submitbutton="Submit",
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+
+    )
+    print("User input:", user_input)
+    ################################################
+    user_input = get_user_input_radio(
+        radio_options=("Option 1", "Option 2", "Option 3", "Option 4"),
+        indexdefault=0,
+        size="300x350",
+        title="Your input",
+        textabovebox="Select a radio button",
+        submitbutton="Submit",
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+    )
+    print("User input:", user_input)
+    ################################################
+    show_info("Titel", "Message")
+    show_error("Titel", "Message")
+    show_warning("Titel", "Message")
+
+
+
+```
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput1.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput2.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/checkboxes.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/clickabutton.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/radiobutton.png?raw=true)
```

### Comparing `tkinteruserinput-0.10/README.md` & `tkinteruserinput-0.11/README.md`

 * *Files identical despite different names*

### Comparing `tkinteruserinput-0.10/setup.py` & `tkinteruserinput-0.11/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
-import codecs
-import os
+# import codecs
+# import os
+# 
+# here = os.path.abspath(os.path.dirname(__file__))
+# 
+# with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+#     long_description = "\n" + fh.read()\
 
-#change to dict
-here = os.path.abspath(os.path.dirname(__file__))
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.10'
-DESCRIPTION = "Pop-ups to get input from the user - tkinter"
+VERSION = '''0.11'''
+DESCRIPTION = '''Pop-ups to get input from the user - tkinter'''
 
 # Setting up
 setup(
     name="tkinteruserinput",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/tkinteruserinput',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
+long_description = long_description,
+long_description_content_type="text/markdown",
     #packages=[],
     keywords=['tkinter'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
     install_requires=[],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```

### Comparing `tkinteruserinput-0.10/tkinteruserinput/LICENSE` & `tkinteruserinput-0.11/tkinteruserinput/LICENSE`

 * *Files identical despite different names*

### Comparing `tkinteruserinput-0.10/tkinteruserinput/README.MD` & `tkinteruserinput-0.11/tkinteruserinput/README.MD`

 * *Files identical despite different names*

### Comparing `tkinteruserinput-0.10/tkinteruserinput/__init__.py` & `tkinteruserinput-0.11/tkinteruserinput/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import tkinter as tk
 import re
-from tkinter import messagebox
+from tkinter import messagebox, font
 from typing import Optional, Tuple, Union
 
 
+
 def show_warning(title: str, message: str):
     """
     Displays a warning message box with the given title and message.
 
     Args:
         title (str): The title of the warning message box.
         message (str): The message to be displayed in the warning message box.
@@ -94,14 +95,17 @@
             if showinfo:
                 messagebox.showinfo(*showinfo)
             if showwarning:
                 messagebox.showwarning(*showwarning)
 
     user_input = None
     root = tk.Tk()
+    default_font = tk.font.Font(family="Courier New", size=10, weight="normal")
+
+    root.option_add("*Font", default_font)
     if icon:
         root.iconbitmap(os.path.normpath(icon))
     root.geometry(size)
     root.title(title)
     instructions_label = tk.Label(root, text=textabovebox)
     instructions_label.pack(pady=5)
     input_box = tk.Text(root, height=linesinputbox)
@@ -120,14 +124,16 @@
     title: str = "Your input",
     textabovebox: str = "Enter your text below:",
     submitbutton: str = "Submit",
         icon=None,
 ):
     user_input = []
     root = tk.Tk()
+    default_font = tk.font.Font(family="Courier New", size=10, weight="normal")
+    root.option_add("*Font", default_font)
     if icon:
         root.iconbitmap(os.path.normpath(icon))
     root.geometry(size)
     root.title(title)
 
     # Define the checkbox options
 
@@ -171,14 +177,16 @@
     title: str = "Your input",
     textabovebox: str = "Enter your text below:",
     submitbutton: str = "Submit",
 icon=None,
 ):
     user_input = None
     root = tk.Tk()
+    default_font = tk.font.Font(family="Courier New", size=10, weight="normal")
+    root.option_add("*Font", default_font)
     if icon:
         root.iconbitmap(os.path.normpath(icon))
     root.geometry(size)
     root.title(title)
 
     # Define the radio button options
     radio_button_options = radio_options
@@ -226,14 +234,16 @@
 
     def select_option(option):
         nonlocal user_input
         user_input = option
         root.destroy()
 
     root = tk.Tk()
+    default_font = tk.font.Font(family="Courier New", size=10, weight="normal")
+    root.option_add("*Font", default_font)
     if icon:
         root.iconbitmap(os.path.normpath(icon))
     root.geometry(size)
     root.title(title)
 
     instructions_label = tk.Label(root, text=textabovebox)
     instructions_label.pack(pady=5)
```

### Comparing `tkinteruserinput-0.10/tkinteruserinput.egg-info/PKG-INFO` & `tkinteruserinput-0.11/tkinteruserinput.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,106 @@
 Metadata-Version: 2.1
 Name: tkinteruserinput
-Version: 0.10
+Version: 0.11
 Summary: Pop-ups to get input from the user - tkinter
 Home-page: https://github.com/hansalemaos/tkinteruserinput
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: tkinter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
+# Pop-ups to get input from the user - tkinter 
 
-# Pop-ups to get input from the user - tkinter 
-
-## pip install tkinteruserinput
-
-### Tested against Windows 10 / Python 3.10 / Anaconda 
-
-
-
-
-```python
-
-from tkinteruserinput import get_user_input, get_user_input_varbuttons, get_user_input_checkbox, get_user_input_radio, \
-    show_info, show_error, show_warning
-
-if __name__ == '__main__':
-    ################################################
-
-    user_input = get_user_input(
-        linesinputbox=1,
-        size="300x150",
-        title="Input Box Example",
-        textabovebox="Enter your text below:",
-        submitbutton="Submit",
-        regexcheck=r"\d+",
-        showerror=("Error", "This is not a number! Try again!"),
-        showinfo=None,
-        showwarning=None,
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico",
-    )
-    print("User input:", user_input)
-
-    ################################################
-
-    options = ["Option 1", "Option 2", "Option 3"]
-    user_input = get_user_input_varbuttons(
-        options=options,
-        size="300x350",
-        title="Your input",
-        textabovebox="Click a button",
-        buttonwidth=15,
-        buttonheight=3,
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-
-    )
-    print("User input:", user_input)
-    ################################################
-
-    user_input = get_user_input_checkbox(
-        checkbox_options=("Option 1", "Option 2", "Option 3", "Option 4"),
-        size="300x350",
-        title="Your input",
-        textabovebox="Select checkboxes:",
-        submitbutton="Submit",
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-
-    )
-    print("User input:", user_input)
-    ################################################
-    user_input = get_user_input_radio(
-        radio_options=("Option 1", "Option 2", "Option 3", "Option 4"),
-        indexdefault=0,
-        size="300x350",
-        title="Your input",
-        textabovebox="Select a radio button",
-        submitbutton="Submit",
-        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
-    )
-    print("User input:", user_input)
-    ################################################
-    show_info("Titel", "Message")
-    show_error("Titel", "Message")
-    show_warning("Titel", "Message")
-
-
-
-```
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput1.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput2.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/checkboxes.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/clickabutton.png?raw=true)
-
-
-![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/radiobutton.png?raw=true)
+## pip install tkinteruserinput
+
+### Tested against Windows 10 / Python 3.10 / Anaconda 
+
+
+
+
+```python
+
+from tkinteruserinput import get_user_input, get_user_input_varbuttons, get_user_input_checkbox, get_user_input_radio, \
+    show_info, show_error, show_warning
+
+if __name__ == '__main__':
+    ################################################
+
+    user_input = get_user_input(
+        linesinputbox=1,
+        size="300x150",
+        title="Input Box Example",
+        textabovebox="Enter your text below:",
+        submitbutton="Submit",
+        regexcheck=r"\d+",
+        showerror=("Error", "This is not a number! Try again!"),
+        showinfo=None,
+        showwarning=None,
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico",
+    )
+    print("User input:", user_input)
+
+    ################################################
+
+    options = ["Option 1", "Option 2", "Option 3"]
+    user_input = get_user_input_varbuttons(
+        options=options,
+        size="300x350",
+        title="Your input",
+        textabovebox="Click a button",
+        buttonwidth=15,
+        buttonheight=3,
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+
+    )
+    print("User input:", user_input)
+    ################################################
+
+    user_input = get_user_input_checkbox(
+        checkbox_options=("Option 1", "Option 2", "Option 3", "Option 4"),
+        size="300x350",
+        title="Your input",
+        textabovebox="Select checkboxes:",
+        submitbutton="Submit",
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+
+    )
+    print("User input:", user_input)
+    ################################################
+    user_input = get_user_input_radio(
+        radio_options=("Option 1", "Option 2", "Option 3", "Option 4"),
+        indexdefault=0,
+        size="300x350",
+        title="Your input",
+        textabovebox="Select a radio button",
+        submitbutton="Submit",
+        icon=r"C:\Users\hansc\Pictures\regiondf.ico"
+    )
+    print("User input:", user_input)
+    ################################################
+    show_info("Titel", "Message")
+    show_error("Titel", "Message")
+    show_warning("Titel", "Message")
+
+
+
+```
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput1.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/textinput2.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/checkboxes.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/clickabutton.png?raw=true)
+
+
+![](https://github.com/hansalemaos/screenshots/blob/main/tkinteruserinput/radiobutton.png?raw=true)
```

