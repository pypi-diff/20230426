# Comparing `tmp/gamepadx-1.0.0.tar.gz` & `tmp/gamepadx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamepadx-1.0.0.tar", last modified: Mon Apr 24 13:27:11 2023, max compression
+gzip compressed data, was "gamepadx-1.0.1.tar", last modified: Wed Apr 26 09:15:08 2023, max compression
```

## Comparing `gamepadx-1.0.0.tar` & `gamepadx-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:11.671875 gamepadx-1.0.0/
--rw-rw-rw-   0        0        0     1064 2023-04-22 20:02:18.000000 gamepadx-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       38 2023-04-22 21:07:41.000000 gamepadx-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2261 2023-04-24 13:27:11.670872 gamepadx-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1652 2023-04-24 13:17:03.000000 gamepadx-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:11.599866 gamepadx-1.0.0/gamepadx/
--rw-rw-rw-   0        0        0       53 2023-04-24 09:57:47.000000 gamepadx-1.0.0/gamepadx/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-04-24 12:24:26.000000 gamepadx-1.0.0/gamepadx/commons.py
--rw-rw-rw-   0        0        0     3520 2023-04-24 13:07:58.000000 gamepadx-1.0.0/gamepadx/gamepad.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:11.666871 gamepadx-1.0.0/gamepadx/vigem/
--rw-rw-rw-   0        0        0   140800 2023-04-19 19:20:44.000000 gamepadx-1.0.0/gamepadx/vigem/ViGEmClient.dll
--rw-rw-rw-   0        0        0        0 2023-04-24 09:06:40.000000 gamepadx-1.0.0/gamepadx/vigem/__init__.py
--rw-rw-rw-   0        0        0     1866 2023-04-24 09:58:06.000000 gamepadx-1.0.0/gamepadx/vigem/lib.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:27:11.626869 gamepadx-1.0.0/gamepadx.egg-info/
--rw-rw-rw-   0        0        0     2261 2023-04-24 13:27:11.000000 gamepadx-1.0.0/gamepadx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-24 13:27:11.000000 gamepadx-1.0.0/gamepadx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:27:11.000000 gamepadx-1.0.0/gamepadx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 13:27:11.000000 gamepadx-1.0.0/gamepadx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      608 2023-04-24 13:25:31.000000 gamepadx-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 13:27:11.672872 gamepadx-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 09:15:08.401514 gamepadx-1.0.1/
+-rw-rw-rw-   0        0        0     1064 2023-04-26 09:06:38.000000 gamepadx-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-04-26 09:06:38.000000 gamepadx-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2323 2023-04-26 09:15:08.399515 gamepadx-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1713 2023-04-26 09:11:29.000000 gamepadx-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 09:15:08.317508 gamepadx-1.0.1/gamepadx/
+-rw-rw-rw-   0        0        0       53 2023-04-26 09:07:39.000000 gamepadx-1.0.1/gamepadx/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-04-26 09:07:37.000000 gamepadx-1.0.1/gamepadx/commons.py
+-rw-rw-rw-   0        0        0     3520 2023-04-26 09:07:32.000000 gamepadx-1.0.1/gamepadx/gamepad.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:15:08.396516 gamepadx-1.0.1/gamepadx/vigem/
+-rw-rw-rw-   0        0        0   140800 2023-04-26 09:06:38.000000 gamepadx-1.0.1/gamepadx/vigem/ViGEmClient.dll
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:07:53.000000 gamepadx-1.0.1/gamepadx/vigem/__init__.py
+-rw-rw-rw-   0        0        0     1867 2023-04-26 09:09:00.000000 gamepadx-1.0.1/gamepadx/vigem/lib.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:15:08.344509 gamepadx-1.0.1/gamepadx.egg-info/
+-rw-rw-rw-   0        0        0     2323 2023-04-26 09:15:08.000000 gamepadx-1.0.1/gamepadx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-26 09:15:08.000000 gamepadx-1.0.1/gamepadx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:15:08.000000 gamepadx-1.0.1/gamepadx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 09:15:08.000000 gamepadx-1.0.1/gamepadx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      608 2023-04-26 09:13:52.000000 gamepadx-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:15:08.401514 gamepadx-1.0.1/setup.cfg
```

### Comparing `gamepadx-1.0.0/LICENSE` & `gamepadx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gamepadx-1.0.0/PKG-INFO` & `gamepadx-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamepadx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Read and emulate an Xbox controller
 Author-email: Foralich <76852996+foralich@users.noreply.github.com>
 Project-URL: Bug Tracker, https://github.com/foralich/gamepadx/issues
 Project-URL: Source, https://github.com/foralich/gamepadx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,24 +22,25 @@
 
 You will need to download the [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus/releases/latest) to emulate a controller.
 
 You must have Python >= 3.11
 
 ## Installation
 
-```console
+```powershell
 pip install gamepadx
 ```
 ## Usage
 
 ```python
-from gamepadx import Gamepad, VirtualGamepad
-from gamepadx.commons import XInputButtons, XInputTriggers, XInputThumbs
 from time import sleep
 
+from gamepadx import Gamepad, VirtualGamepad
+from gamepadx.commons import XInputButtons, XInputThumbs, XInputTriggers
+
 
 def main():
     gamepad = Gamepad()
 
     gamepad.update()
 
     print(gamepad.is_button_pressed(XInputButtons.A))
@@ -63,14 +64,14 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## Contributing
 
-If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
+If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and [isort](https://github.com/PyCQA/isort) import order and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
 
 ## Acknowledgements
 
 - [Xbox Controller Mapper](https://github.com/izdwuut/xbox-mapper-tutorial)
 - [Virtual Gamepad](https://github.com/yannbouteiller/vgamepad)
 - [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus)
```

### Comparing `gamepadx-1.0.0/README.md` & `gamepadx-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 
 You will need to download the [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus/releases/latest) to emulate a controller.
 
 You must have Python >= 3.11
 
 ## Installation
 
-```console
+```powershell
 pip install gamepadx
 ```
 ## Usage
 
 ```python
-from gamepadx import Gamepad, VirtualGamepad
-from gamepadx.commons import XInputButtons, XInputTriggers, XInputThumbs
 from time import sleep
 
+from gamepadx import Gamepad, VirtualGamepad
+from gamepadx.commons import XInputButtons, XInputThumbs, XInputTriggers
+
 
 def main():
     gamepad = Gamepad()
 
     gamepad.update()
 
     print(gamepad.is_button_pressed(XInputButtons.A))
@@ -49,14 +50,14 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## Contributing
 
-If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
+If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and [isort](https://github.com/PyCQA/isort) import order and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
 
 ## Acknowledgements
 
 - [Xbox Controller Mapper](https://github.com/izdwuut/xbox-mapper-tutorial)
 - [Virtual Gamepad](https://github.com/yannbouteiller/vgamepad)
 - [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus)
```

### Comparing `gamepadx-1.0.0/gamepadx/commons.py` & `gamepadx-1.0.1/gamepadx/commons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ctypes import Structure, c_uint
-from ctypes.wintypes import WORD, BYTE, SHORT, DWORD
-from enum import IntFlag, StrEnum, IntEnum
+from ctypes.wintypes import BYTE, DWORD, SHORT, WORD
+from enum import IntEnum, IntFlag, StrEnum
 
 
 class XInputGamepad(Structure):
     """
     Describes the current state of the Xbox 360 Controller
     """
```

### Comparing `gamepadx-1.0.0/gamepadx/gamepad.py` & `gamepadx-1.0.1/gamepadx/gamepad.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from gamepadx.commons import *
-from ctypes import windll, pointer, c_void_p
+from ctypes import c_void_p, pointer, windll
 from ctypes.wintypes import WORD
-import gamepadx.vigem.lib as vigem_lib
 
+import gamepadx.vigem.lib as vigem_lib
+from gamepadx.commons import *
 
 TRIGGER_MAGNITUDE = 256
 THUMB_MAGNITUDE = 32768
 
 
 class Gamepad:
     """
```

### Comparing `gamepadx-1.0.0/gamepadx/vigem/ViGEmClient.dll` & `gamepadx-1.0.1/gamepadx/vigem/ViGEmClient.dll`

 * *Files identical despite different names*

### Comparing `gamepadx-1.0.0/gamepadx/vigem/lib.py` & `gamepadx-1.0.1/gamepadx/vigem/lib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from ctypes import CDLL, c_uint, c_void_p
 from pathlib import Path
-from ctypes import CDLL, c_void_p, c_uint
+
 from gamepadx.commons import XInputGamepad
 
 path = Path(__file__).parent.absolute() / "ViGEmClient.dll"
 api = CDLL(str(path))
 
 """
 Allocates an object representing a driver connection
```

### Comparing `gamepadx-1.0.0/gamepadx.egg-info/PKG-INFO` & `gamepadx-1.0.1/gamepadx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamepadx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Read and emulate an Xbox controller
 Author-email: Foralich <76852996+foralich@users.noreply.github.com>
 Project-URL: Bug Tracker, https://github.com/foralich/gamepadx/issues
 Project-URL: Source, https://github.com/foralich/gamepadx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -22,24 +22,25 @@
 
 You will need to download the [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus/releases/latest) to emulate a controller.
 
 You must have Python >= 3.11
 
 ## Installation
 
-```console
+```powershell
 pip install gamepadx
 ```
 ## Usage
 
 ```python
-from gamepadx import Gamepad, VirtualGamepad
-from gamepadx.commons import XInputButtons, XInputTriggers, XInputThumbs
 from time import sleep
 
+from gamepadx import Gamepad, VirtualGamepad
+from gamepadx.commons import XInputButtons, XInputThumbs, XInputTriggers
+
 
 def main():
     gamepad = Gamepad()
 
     gamepad.update()
 
     print(gamepad.is_button_pressed(XInputButtons.A))
@@ -63,14 +64,14 @@
 
 if __name__ == "__main__":
     main()
 ```
 
 ## Contributing
 
-If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
+If you would like to contribute to GamepadX, please ensure that your code follows the [Black](https://github.com/psf/black) style guide and [isort](https://github.com/PyCQA/isort) import order and submit a pull request on GitHub. Don't forget to add unwanted files and folders to the `.gitignore`
 
 ## Acknowledgements
 
 - [Xbox Controller Mapper](https://github.com/izdwuut/xbox-mapper-tutorial)
 - [Virtual Gamepad](https://github.com/yannbouteiller/vgamepad)
 - [ViGEm Bus Driver](https://github.com/ViGEm/ViGEmBus)
```

### Comparing `gamepadx-1.0.0/pyproject.toml` & `gamepadx-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gamepadx"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="Foralich", email="76852996+foralich@users.noreply.github.com" }
 ]
 description = "Read and emulate an Xbox controller"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

