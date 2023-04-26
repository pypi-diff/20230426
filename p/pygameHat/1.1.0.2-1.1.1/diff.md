# Comparing `tmp/pygameHat-1.1.0.2.tar.gz` & `tmp/pygameHat-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.1.0.2.tar", last modified: Mon Apr 17 15:21:39 2023, max compression
+gzip compressed data, was "pygameHat-1.1.1.tar", last modified: Wed Apr 26 17:55:18 2023, max compression
```

## Comparing `pygameHat-1.1.0.2.tar` & `pygameHat-1.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 15:21:39.081035 pygameHat-1.1.0.2/
--rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      545 2023-04-17 15:21:39.081035 pygameHat-1.1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 15:21:38.991025 pygameHat-1.1.0.2/pygameHat/
--rw-rw-rw-   0        0        0    41091 2023-04-17 15:21:05.000000 pygameHat-1.1.0.2/pygameHat/__init__.py
--rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.0.2/pygameHat/pygameHat.py
-drwxrwxrwx   0        0        0        0 2023-04-17 15:21:39.072017 pygameHat-1.1.0.2/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      545 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 15:21:38.000000 pygameHat-1.1.0.2/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 15:21:39.087015 pygameHat-1.1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-17 15:20:14.000000 pygameHat-1.1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.575534 pygameHat-1.1.1/
+-rw-rw-rw-   0        0        0       29 2023-04-17 15:20:38.000000 pygameHat-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-04-26 17:55:18.575534 pygameHat-1.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.404569 pygameHat-1.1.1/pygameHat/
+-rw-rw-rw-   0        0        0    42191 2023-04-26 17:54:14.000000 pygameHat-1.1.1/pygameHat/__init__.py
+-rw-rw-rw-   0        0        0       11 2023-04-17 14:59:31.000000 pygameHat-1.1.1/pygameHat/pygameHat.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:55:18.568535 pygameHat-1.1.1/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 17:55:17.000000 pygameHat-1.1.1/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 17:55:18.580534 pygameHat-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-04-26 17:54:25.000000 pygameHat-1.1.1/setup.py
```

### Comparing `pygameHat-1.1.0.2/PKG-INFO` & `pygameHat-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.0.2
+Version: 1.1.1
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

### Comparing `pygameHat-1.1.0.2/pygameHat/__init__.py` & `pygameHat-1.1.1/pygameHat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pygame, sys, time, base64, os
 
 #pygame initialization
-version = "Beta 1.1.0.2"
+version = "Beta 1.1.1"
 print(f"\nAdditional hello from pygameHat {version} :D")
 print("\nThis version is not backwards compatible with pygameHat <= 1.0.7")
 
 pygame.init()
 pygame.font.init()
 try:
     pygame.mixer.init()
@@ -66,30 +66,29 @@
         else:
             self.index = pygame.image.load(index).convert_alpha()
 
         self.speed = speed
         self.x_frames, self.y_frames = spritesheet_data
 
         if size:
-            sx, sy = size
-            self.index = pygame.transform.scale(self.index, (int(sx*self.x_frames), int(sy*self.y_frames)))
+            resize_sprite(self, size)
 
         self.x_size, self.y_size = self.index.get_width()/(self.x_frames), self.index.get_height()/(self.y_frames)
         
         self.x_frames -= 1
         self.y_frames -= 1
 
         self.current_x_frame = 0
         self.current_y_frame = 0
         self.timer = 1/self.speed
         self.loop = looping
         self.on_last_frame = False
 
         self.collision = collision
-        self.collision_shape = self.index.get_rect(width=self.x_size, height=self.y_size)
+        self.collision_shape = self.reload_collision_shape()
     
         #Setting sprite offset
         if offset == "middle-center":
             self.x_offset, self.y_offset = self.x_size/2, self.y_size/2
         elif offset == "upper-left":
             self.x_offset, self.y_offset = 0, 0
         elif offset == "upper-center":
@@ -113,36 +112,44 @@
 
         self.collision_shape.x = self.x_offset
         self.collision_shape.y = self.y_offset
 
     def play(self):
         self.on_last_frame = False
         self.current_x_frame = 0
-        self.current_y_frame = 0
-        
+        self.current_y_frame = 0      
+
+    def set_alpha(self, value):
+        self.index.set_alpha(value)
+
     def animate(self):
         self.timer -= delta_time
         if self.timer <= 0:
             if self.current_x_frame < self.x_frames:
                 self.current_x_frame += 1
             elif self.current_y_frame < self.y_frames:
                 self.current_x_frame = 0
                 self.current_y_frame += 1
             elif self.loop:
                 self.play()
             else:
                 self.on_last_frame = True
             self.timer = 1/self.speed
 
-    def update_collision_shape(self, x, y):
+    def update_collision_shape_position(self, x, y):
         self.collision_shape.x = x-self.x_offset
         self.collision_shape.y = y-self.y_offset
 
         return self.collision_shape
 
+    def reload_collision_shape(self):
+        self.x_size, self.y_size = self.index.get_width()/(self.x_frames+1), self.index.get_height()/(self.y_frames+1)
+        self.collision_shape = self.index.get_rect(width=self.x_size, height=self.y_size)
+        return self.collision_shape
+
 class Sound:
     def __init__(self, file, large=False):
         if pygame.mixer.get_init():
             if large:
                 self.sound = pygame.mixer_music.load(file)
 
             self.sound = pygame.mixer.Sound(file)
@@ -163,14 +170,17 @@
         if path == "default":
             self.font = pygame.font.Font(None, size)
         else:
            self.font = pygame.font.Font(path, size)
         
         self.color = color
         self.background_color = background_color
+    
+    def measure_size(self, text_to_measure):
+        return self.font.render(text_to_measure, True, (0, 0, 0)).get_size()
 
 class Camera:
     def __init__(self):
         self.x = 0
         self.y = 0
 
 class Console:
@@ -229,14 +239,17 @@
     icon = None
     enable_console = True
     fps = 60
     font = "default"
 
     shameless_ad = True
 
+class RoomGotChanged(Exception):
+    pass
+
 temp_icon = surfaceStringifier.to_surface("7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f//v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//39/f/9/f3//f39//+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/+/ksP/v5LD/7+Sw/+/ksP+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V//v5LD/7+Sw/+/ksP/v5LD/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/uXpX/7l6V/+5elf/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv//////cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7//////3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw//////////////////////9wkr7/cJK+/3CSvv9wkr7/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP9wkr7/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/cJK+/3CSvv9wkr7/cJK+/3CSvv9wkr7/cJK+///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD///IA///yAP//8gD///IA///yAP//8gD///IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw///yAP//8gD///IA///yAP//////////////////////7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD///IA///yAP//8gD///IA///yAP////////IA///yAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/AAAA/wAAAP8AAAD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw///yAP//8gD///IA///yAP//8gD////////yAP//8gD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP8AAAD/AAAA/wAAAP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/wAAAP8AAAD/AAAA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP//8gD///IA///yAP//8gD///IA///yAP//8gD///IA/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/+/ksP/v5LD/7+Sw/w==", (70, 70))
 
 #first initializations
 debug_font = pygame.font.Font
 title_font = pygame.font.Font
 console_opened = False
 console = Console()
@@ -244,14 +257,15 @@
 current_time = 0
 
 screen = pygame.surface.Surface(Settings.window_size)
 camera = Camera()
 screen_size = (0, 0)
 
 current_room = Room()
+changed_room = False
 
 def init():
     global screen, screen_size, debug_font, title_font
 
     if Settings.font == "default":
         debug_font = pygame.font.Font(None, 25)
         title_font = pygame.font.Font(None, 100)
@@ -315,26 +329,26 @@
         else:
             return found_objects[-1]
     else:
         return None
 
 def collide_objects(object1, object2):
     if object1 != object2 and object1.sprite and object1.sprite.collision and object2.sprite and object2.sprite.collision:
-        object1_shape = object1.sprite.update_collision_shape(object1.x, object1.y)
-        object2_shape = object2.sprite.update_collision_shape(object2.x, object2.y)
+        object1_shape = object1.sprite.update_collision_shape_position(object1.x, object1.y)
+        object2_shape = object2.sprite.update_collision_shape_position(object2.x, object2.y)
         if object1_shape.colliderect(object2_shape):
             return object2
 
 def collide_point(point, object):
     pointX, pointY = point
     pointX += camera.x
     pointY += camera.y
 
     if object.sprite and object.sprite.collision:
-        object_shape = object.sprite.update_collision_shape(object.x, object.y)
+        object_shape = object.sprite.update_collision_shape_position(object.x, object.y)
 
         if object_shape.collidepoint((pointX, pointY)):
             return object
 
 def screen_position_to_ingame_position(position):
     pX, pY = position
     rSX, rSY = Settings.room_size
@@ -359,39 +373,48 @@
                 current_room.layers[layer].remove(instance)
 
 def draw_sprite(sprite, x, y):
         if sprite:
             screen.blit(sprite.index, (x-camera.x-sprite.x_offset, y-camera.y-sprite.y_offset), (sprite.x_size*sprite.current_x_frame, sprite.y_size*sprite.current_y_frame, sprite.x_size, sprite.y_size))
             sprite.animate()
 
+def resize_sprite(sprite, dimensions):
+    #:todo fix offset
+    sx, sy = dimensions
+    sprite.index = pygame.transform.scale(sprite.index, (int(sx*(sprite.x_frames+1)), int(sy*(sprite.y_frames+1))))
+    sprite.reload_collision_shape()
+
+    return sprite
+
 def draw_font(position, font, text, color="default", background_color="default"):
     if color == "default":
         color = font.color
     else:
         color = color
     if background_color == "default":
         bg_color = font.background_color
     else:
         bg_color = background_color
 
     x, y = position
     screen.blit(font.font.render(text, True, color, bg_color), (x-camera.x, y-camera.y))
 
 def change_room(room):
-    global current_room
-
+    global current_room, changed_room
     current_room = room
+    changed_room = True
 
 
 def start():
     timeB = 0
     last_input = None
     last_input_released = None
     global delta_time, current_time
     global screen, screen_size
+    global changed_room
 
     if Settings.fullscreen:
         monitor = pygame.display.set_mode(Settings.window_size, pygame.FULLSCREEN)
     else:
         monitor = pygame.display.set_mode(Settings.window_size, pygame.RESIZABLE)
 
     running = True
@@ -427,32 +450,39 @@
         #background                
         if type(current_room.background) == Sprite:
             draw_sprite(current_room.background, 0, 0)
         else:
             screen.fill(current_room.background)
     
         #object handling
-        for layer in current_room.layers:
-            for instance in current_room.layers[layer]:
-                #object drawing and processing
-                if instance.visible:
-                    instance.draw()
-                instance.step()
-                instance.decrement_active_timers()
-                #collision processing
-                for layer2 in current_room.layers:
-                    for instance2 in current_room.layers[layer2]:
-                        obj = collide_objects(instance, instance2)
-                        if obj:
-                            instance.is_colliding(obj)
-                #inputs
-                if last_input:
-                    instance.key_just_pressed(last_input)
-                if last_input_released:
-                    instance.key_just_released(last_input_released)
+        try:
+            for layer in current_room.layers:
+                for instance in current_room.layers[layer]:
+                    #object drawing and processing
+                    if instance.visible:
+                        instance.draw()
+                    instance.step()
+                    instance.decrement_active_timers()
+                    #collision processing
+                    for layer2 in current_room.layers:
+                        for instance2 in current_room.layers[layer2]:
+                            obj = collide_objects(instance, instance2)
+                            if obj:
+                                instance.is_colliding(obj)
+                    #inputs
+                    if last_input:
+                        instance.key_just_pressed(last_input)
+                    if last_input_released:
+                        instance.key_just_released(last_input_released)
+                    
+                    if changed_room:
+                        raise RoomGotChanged
+        except RoomGotChanged:
+            changed_room = False
+            screen.fill(current_room.background)
         
         console.display()
 
         monitor.blit(pygame.transform.scale(screen, screen_size), (0, 0))
         pygame.display.flip()
 
         last_input = None
```

### Comparing `pygameHat-1.1.0.2/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.1.1/pygameHat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.1.0.2
+Version: 1.1.1
 Summary: Pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,engine,pygame,game,maker
```

