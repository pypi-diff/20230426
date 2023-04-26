# Comparing `tmp/frascii-3.1.tar.gz` & `tmp/frascii-3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frascii-3.1.tar", last modified: Wed Apr 26 08:09:30 2023, max compression
+gzip compressed data, was "frascii-3.2.tar", last modified: Wed Apr 26 12:54:33 2023, max compression
```

## Comparing `frascii-3.1.tar` & `frascii-3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 08:09:30.832856 frascii-3.1/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 08:09:30.832856 frascii-3.1/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-3.1/README.md
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 08:09:30.832856 frascii-3.1/frascii/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-26 08:09:19.000000 frascii-3.1/frascii/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-3.1/frascii/commands.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 08:09:30.832856 frascii-3.1/frascii/fractals/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.1/frascii/fractals/__init__.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.1/frascii/fractals/cantor.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.1/frascii/fractals/dragon_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.1/frascii/fractals/fibonacci.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.1/frascii/fractals/hilbert_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3851 2023-04-26 08:08:49.000000 frascii-3.1/frascii/fractals/julia.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.1/frascii/fractals/koch.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-12 12:34:18.000000 frascii-3.1/frascii/fractals/l_system.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3715 2023-04-26 08:09:03.000000 frascii-3.1/frascii/fractals/mandelbrot.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.1/frascii/fractals/peano_curve.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.1/frascii/fractals/sierpinski_carpet.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.1/frascii/fractals/sierpinski_triangle.py
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.1/frascii/fractals/vicsek.py
-drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 08:09:30.832856 frascii-3.1/frascii.egg-info/
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 08:09:30.000000 frascii-3.1/frascii.egg-info/PKG-INFO
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-26 08:09:30.000000 frascii-3.1/frascii.egg-info/SOURCES.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-26 08:09:30.000000 frascii-3.1/frascii.egg-info/dependency_links.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-26 08:09:30.000000 frascii-3.1/frascii.egg-info/entry_points.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-26 08:09:30.000000 frascii-3.1/frascii.egg-info/top_level.txt
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-26 08:09:30.832856 frascii-3.1/setup.cfg
--rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.1/setup.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 12:54:33.170385 frascii-3.2/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    12812 2023-04-25 07:40:51.000000 frascii-3.2/README.md
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1942 2023-04-26 12:54:11.000000 frascii-3.2/frascii/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     7769 2023-04-25 07:40:17.000000 frascii-3.2/frascii/commands.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii/fractals/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        0 2023-02-24 11:27:22.000000 frascii-3.2/frascii/fractals/__init__.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      306 2023-03-03 18:15:44.000000 frascii-3.2/frascii/fractals/cantor.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2224 2023-02-28 08:13:57.000000 frascii-3.2/frascii/fractals/dragon_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1263 2023-03-03 18:15:51.000000 frascii-3.2/frascii/fractals/fibonacci.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     1816 2023-02-28 08:12:17.000000 frascii-3.2/frascii/fractals/hilbert_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3880 2023-04-26 12:53:36.000000 frascii-3.2/frascii/fractals/julia.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2078 2023-03-01 08:32:48.000000 frascii-3.2/frascii/fractals/koch.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2937 2023-04-26 10:11:08.000000 frascii-3.2/frascii/fractals/l_system.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     3743 2023-04-26 12:53:19.000000 frascii-3.2/frascii/fractals/mandelbrot.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)     2072 2023-02-26 23:51:55.000000 frascii-3.2/frascii/fractals/peano_curve.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      553 2023-02-24 11:50:58.000000 frascii-3.2/frascii/fractals/sierpinski_carpet.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      395 2023-02-28 09:01:32.000000 frascii-3.2/frascii/fractals/sierpinski_triangle.py
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      494 2023-02-28 14:05:15.000000 frascii-3.2/frascii/fractals/vicsek.py
+drwxrwxr-x   0 kingkong  (1000) kingkong  (1000)        0 2023-04-26 12:54:33.170385 frascii-3.2/frascii.egg-info/
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)    14878 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/PKG-INFO
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      627 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/SOURCES.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        1 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/dependency_links.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       55 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/entry_points.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)        8 2023-04-26 12:54:33.000000 frascii-3.2/frascii.egg-info/top_level.txt
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)       79 2023-04-26 12:54:33.170385 frascii-3.2/setup.cfg
+-rw-rw-r--   0 kingkong  (1000) kingkong  (1000)      572 2023-04-26 07:39:57.000000 frascii-3.2/setup.py
```

### Comparing `frascii-3.1/PKG-INFO` & `frascii-3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.1
+Version: 3.2
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.1/README.md` & `frascii-3.2/README.md`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/__init__.py` & `frascii-3.2/frascii/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from frascii.fractals.vicsek import vicsek_string
 from frascii.fractals.hilbert_curve import hilbert_curve_string
 from frascii.fractals.peano_curve import peano_curve_string
 from frascii.fractals.dragon_curve import dragon_curve_string
 from frascii.fractals.fibonacci import fibonacci_string
 from frascii.fractals.l_system import l_system_string
 
-__version__ = '3.1'
+__version__ = '3.2'
 
 def mandelbrot(x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
 	if explore:
 		x, y, x_radius, y_radius, stepsize, max_iter, style, grid = mandelbrot_explore(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 	return mandelbrot_string(x, y, x_radius, y_radius, stepsize, max_iter, style, grid)
 
 def julia(f, x, y, x_radius, y_radius, stepsize, max_iter, style, grid, explore):
```

### Comparing `frascii-3.1/frascii/commands.py` & `frascii-3.2/frascii/commands.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/dragon_curve.py` & `frascii-3.2/frascii/fractals/dragon_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/fibonacci.py` & `frascii-3.2/frascii/fractals/fibonacci.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/hilbert_curve.py` & `frascii-3.2/frascii/fractals/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/julia.py` & `frascii-3.2/frascii/fractals/julia.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 			elif key == ord('.'):
 				i += 1
 			elif key == ord('-'):
 				si = 1 - si
 			elif key == curses.KEY_MOUSE:
 				_, mx, my, _, _ = curses.getmouse()
 				x += ((mx if grid == "rect" else mx//2) - x_rad)*s
-				y += (-my + y_rad)*s
+				y += (-my + y_rad)*(2*s if grid == "rect" else s)
 			elif key == 27 or key == ord('x'):
 				break
 			elif key == ord('h'):
 				stdscr.clear()
 				stdscr.addstr(0, 0, ("CONTROLS:\n\nARROWS       : navigate complex plane\nPAGE-UP/DOWN : zoom in/out\n',' and '.'  :")+
 									(" change max-iterations\n'-'          : change style\nESC and 'x'  : leave explore mode and print to screen.\n\n")+
 									(f"CURRENT COMMAND:\nfrascii julia -x {x} -y {y} -x_radius {x_rad} -y_radius {y_rad} -stepsize {s}")+
```

### Comparing `frascii-3.1/frascii/fractals/koch.py` & `frascii-3.2/frascii/fractals/koch.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/l_system.py` & `frascii-3.2/frascii/fractals/l_system.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/mandelbrot.py` & `frascii-3.2/frascii/fractals/mandelbrot.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,16 +86,16 @@
 				i = max(i,1)
 			elif key == ord('.'):
 				i += 1
 			elif key == ord('-'):
 				si = 1 - si
 			elif key == curses.KEY_MOUSE:
 				_, mx, my, _, _ = curses.getmouse()
-				x += ((mx if grid == "rect" else mx//2) - x_rad)*s
-				y += (-my + y_rad)*s
+				x += ((mx if grid == "rect" else mx/2) - x_rad)*s
+				y += (-my + y_rad)*(2*s if grid == "rect" else s)
 			elif key == 27 or key == ord('x'):
 				break
 			elif key == ord('h'):
 				stdscr.clear()
 				stdscr.addstr(0, 0, ("CONTROLS:\n\nARROWS       : navigate complex plane\nPAGE-UP/DOWN : zoom in/out\n',' and '.'  :")+
 									(" change max-iterations\n'-'          : change style\nESC and 'x'  : leave explore mode and print to screen.\n\n")+
 									(f"CURRENT COMMAND:\nfrascii mandelbrot -x {x} -y {y} -x_radius {x_rad} -y_radius {y_rad} -stepsize {s}")+
```

### Comparing `frascii-3.1/frascii/fractals/peano_curve.py` & `frascii-3.2/frascii/fractals/peano_curve.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii/fractals/sierpinski_carpet.py` & `frascii-3.2/frascii/fractals/sierpinski_carpet.py`

 * *Files identical despite different names*

### Comparing `frascii-3.1/frascii.egg-info/PKG-INFO` & `frascii-3.2/frascii.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frascii
-Version: 3.1
+Version: 3.2
 Summary: UNKNOWN
 Home-page: https://github.com/LuggiStruggi/Frascii.git
 Author: Lukas König
 Author-email: lukasmkoenig@gmx.net
 License: UNKNOWN
 Description: # Frascii
         ASCII-visualizations of Fractals for the Ubuntu (or other) Terminal
```

### Comparing `frascii-3.1/frascii.egg-info/SOURCES.txt` & `frascii-3.2/frascii.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frascii-3.1/setup.py` & `frascii-3.2/setup.py`

 * *Files identical despite different names*

