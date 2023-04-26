# Comparing `tmp/vsquickview-0.2.5.tar.gz` & `tmp/vsquickview-0.2.6.tar.gz`

## Comparing `vsquickview-0.2.5.tar` & `vsquickview-0.2.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/__init__.py
--rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/colourbars.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/fakevsquickview.py
--rw-r--r--   0        0        0    14623 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/vsquickview.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 vsquickview-0.2.5/vsquickview/vsquickview.qml
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.2.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.2.5/LICENSE
--rw-r--r--   0        0        0     5948 2020-02-02 00:00:00.000000 vsquickview-0.2.5/README.md
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     6801 2020-02-02 00:00:00.000000 vsquickview-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/__init__.py
+-rw-r--r--   0        0        0    10243 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/colourbars.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/fakevsquickview.py
+-rw-r--r--   0        0        0    14624 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/vsquickview.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 vsquickview-0.2.6/vsquickview/vsquickview.qml
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 vsquickview-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 vsquickview-0.2.6/LICENSE
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 vsquickview-0.2.6/README.md
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 vsquickview-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 vsquickview-0.2.6/PKG-INFO
```

### Comparing `vsquickview-0.2.5/vsquickview/__init__.py` & `vsquickview-0.2.6/vsquickview/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
                                  SetIndex, \
                                  SetPreviewGroup, \
                                  ClearPreviewGroup, \
                                  PreviewGroup, \
                                  Show, \
                                  Hide
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `vsquickview-0.2.5/vsquickview/colourbars.py` & `vsquickview-0.2.6/vsquickview/colourbars.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.5/vsquickview/fakevsquickview.py` & `vsquickview-0.2.6/vsquickview/fakevsquickview.py`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.5/vsquickview/vsquickview.py` & `vsquickview-0.2.6/vsquickview/vsquickview.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,15 +396,15 @@
     backend.switchFrame(frame)
 def SetIndex(clip: Union[vs.VideoNode, int, None]=None, index: Optional[int]=None):
     if index == None:
         index = clip
     assert(type(index) == int and 0 <= index < 10)
 
     backend.switchIndex(index)
-def SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None):
+def SetPreviewGroup(clip: Union[vs.VideoNode, list, None]=None, group: Optional[list]=None):
     if group == None:
         group = clip
     assert(type(group) == list and all([type(item) == int and item >= 0 for item in group]))
 
     group = list(set(group))
     group.sort()
```

### Comparing `vsquickview-0.2.5/vsquickview/vsquickview.qml` & `vsquickview-0.2.6/vsquickview/vsquickview.qml`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.5/LICENSE` & `vsquickview-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.5/README.md` & `vsquickview-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -86,38 +86,38 @@
 You can switch to another frame using `G` key. Press `G` key and type in the frame number, then press `Enter` to switch to a new frame. You can also use the `Left` or `Right` key to go to previous or next frame.    
 
 You can cycle between clips using the right mouse button. If you have more than one clip loaded and available at the specific frame number, press the right mouse button and the same frame of the next available clip will be displayed. Press `Shift` and the right mouse button and the clip will be cycled backwards.  
 
 Other usages are listed below:  
 
 * `Left Mouse Button` or `Middle Mouse Button`: Pan the clip preview.  
-* `Scroll Wheel`: Zoom the preview at 100%, 200%, 300%, or 400%.  
+* `Scroll Wheel`: Zoom the preview.  
 * `Right Mouse Button` or `Space`: Switch to the next available clip. `Shift` and `Right Mouse Button` or `Space`: Switch to the previous available clip.  
 * `Alt`: Toggle the label at the bottom-left corner of the screen.  
 * `0`, `1`, `2` … `9`: Switch to the clip at the specific index.  
 * `G`: Press `G` key and type the frame number followed by `Enter` key to go to a specific frame.  
 * `Left` Key or `Right` Key: Go to the previous or the next frame.  
 * `Ctrl` and `Left` Key or `Right` Key: Jump 12 frames backwards or forwards.  
 * `Up` Key or `Down` Key: Go to the next or previous clip, but not cycling the clips.  
 * `F` or `F11`: Toggle fullscreen.  
 
 vsquickview will be closed when you terminate or restart the Jupyter Notebook section. If you close the vsquickview window by accident, you can reopen it by calling function `vsquickview.Show()`.  
 
 ### Using preview group
 
-Additionally, you can also create preview group for a selecteds list of frames you want to compare.  
+Additionally, you can also create preview group for a selected list of frames you want to compare.  
 
 Set preview group using the `vsquickview.SetPreviewGroup()` function:  
 ```py
 vsqv.SetPreviewGroup([1934, 6849, 13226, 21647, 25374, 26811, 28499, 29111])
 ```
 
 In the vsquickview GUI, use `Shift` Key and `Left` Key or `Right` Key to go to the previous or next frame in the set preview group.  
 
 You can also add frame to or remove frame from the preview group using `R` Key from GUI. Afterwards, you can retrieve the current preview group using the `vsquickview.PreviewGroup()` function.  
 
 Here is a short list of functions and their definitions for preview group:  
 ```py
-SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None)
+SetPreviewGroup(clip: Union[vs.VideoNode, list, None]=None, group: Optional[list]=None)
 ClearPreviewGroup(clip: Optional[vs.VideoNode]=None)
 PreviewGroup(clip: Optional[vs.VideoNode]=None)
 ```
```

### Comparing `vsquickview-0.2.5/pyproject.toml` & `vsquickview-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vsquickview-0.2.5/PKG-INFO` & `vsquickview-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsquickview
-Version: 0.2.5
+Version: 0.2.6
 Summary: VapourSynth preview script
 Project-URL: Documentation, https://github.com/Akatmks/vsquickview
 Project-URL: Issues, https://github.com/Akatmks/vsquickview/issues
 Project-URL: Source, https://github.com/Akatmks/vsquickview
 Author-email: Akatsumekusa <Akatsumekusa@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -109,38 +109,38 @@
 You can switch to another frame using `G` key. Press `G` key and type in the frame number, then press `Enter` to switch to a new frame. You can also use the `Left` or `Right` key to go to previous or next frame.    
 
 You can cycle between clips using the right mouse button. If you have more than one clip loaded and available at the specific frame number, press the right mouse button and the same frame of the next available clip will be displayed. Press `Shift` and the right mouse button and the clip will be cycled backwards.  
 
 Other usages are listed below:  
 
 * `Left Mouse Button` or `Middle Mouse Button`: Pan the clip preview.  
-* `Scroll Wheel`: Zoom the preview at 100%, 200%, 300%, or 400%.  
+* `Scroll Wheel`: Zoom the preview.  
 * `Right Mouse Button` or `Space`: Switch to the next available clip. `Shift` and `Right Mouse Button` or `Space`: Switch to the previous available clip.  
 * `Alt`: Toggle the label at the bottom-left corner of the screen.  
 * `0`, `1`, `2` … `9`: Switch to the clip at the specific index.  
 * `G`: Press `G` key and type the frame number followed by `Enter` key to go to a specific frame.  
 * `Left` Key or `Right` Key: Go to the previous or the next frame.  
 * `Ctrl` and `Left` Key or `Right` Key: Jump 12 frames backwards or forwards.  
 * `Up` Key or `Down` Key: Go to the next or previous clip, but not cycling the clips.  
 * `F` or `F11`: Toggle fullscreen.  
 
 vsquickview will be closed when you terminate or restart the Jupyter Notebook section. If you close the vsquickview window by accident, you can reopen it by calling function `vsquickview.Show()`.  
 
 ### Using preview group
 
-Additionally, you can also create preview group for a selecteds list of frames you want to compare.  
+Additionally, you can also create preview group for a selected list of frames you want to compare.  
 
 Set preview group using the `vsquickview.SetPreviewGroup()` function:  
 ```py
 vsqv.SetPreviewGroup([1934, 6849, 13226, 21647, 25374, 26811, 28499, 29111])
 ```
 
 In the vsquickview GUI, use `Shift` Key and `Left` Key or `Right` Key to go to the previous or next frame in the set preview group.  
 
 You can also add frame to or remove frame from the preview group using `R` Key from GUI. Afterwards, you can retrieve the current preview group using the `vsquickview.PreviewGroup()` function.  
 
 Here is a short list of functions and their definitions for preview group:  
 ```py
-SetPreviewGroup(clip: Union[vs.VideoNode, int, None]=None, group: Optional[list]=None)
+SetPreviewGroup(clip: Union[vs.VideoNode, list, None]=None, group: Optional[list]=None)
 ClearPreviewGroup(clip: Optional[vs.VideoNode]=None)
 PreviewGroup(clip: Optional[vs.VideoNode]=None)
 ```
```

