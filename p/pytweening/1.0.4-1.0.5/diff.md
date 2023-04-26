# Comparing `tmp/pytweening-1.0.4.tar.gz` & `tmp/pytweening-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytweening-1.0.4.tar", last modified: Tue Sep 14 03:34:02 2021, max compression
+gzip compressed data, was "pytweening-1.0.5.tar", last modified: Tue Apr 25 21:57:08 2023, max compression
```

## Comparing `pytweening-1.0.4.tar` & `pytweening-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxrwxrwx   0        0        0        0 2021-09-14 03:34:02.526808 pytweening-1.0.4/
--rw-rw-rw-   0        0        0      369 2018-07-20 21:24:57.000000 pytweening-1.0.4/AUTHORS.txt
--rw-rw-rw-   0        0        0     1514 2014-07-17 23:32:58.000000 pytweening-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      199 2014-08-04 08:56:55.000000 pytweening-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3115 2021-09-14 03:34:02.523822 pytweening-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-09-14 03:34:02.313379 pytweening-1.0.4/PyTweening.egg-info/
--rw-rw-rw-   0        0        0     3115 2021-09-14 03:34:01.000000 pytweening-1.0.4/PyTweening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2021-09-14 03:34:02.000000 pytweening-1.0.4/PyTweening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-09-14 03:34:01.000000 pytweening-1.0.4/PyTweening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2021-09-14 03:34:01.000000 pytweening-1.0.4/PyTweening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1519 2021-09-01 21:18:54.000000 pytweening-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2021-09-14 03:34:02.473950 pytweening-1.0.4/docs/
--rw-rw-rw-   0        0        0     6778 2014-08-04 08:42:22.000000 pytweening-1.0.4/docs/Makefile
--rw-rw-rw-   0        0        0     8443 2014-08-04 08:42:22.000000 pytweening-1.0.4/docs/conf.py
--rw-rw-rw-   0        0        0      457 2014-08-04 08:42:22.000000 pytweening-1.0.4/docs/index.rst
--rwxrwxrwx   0        0        0     6709 2014-08-04 08:42:22.000000 pytweening-1.0.4/docs/make.bat
-drwxrwxrwx   0        0        0        0 2021-09-14 03:34:02.477939 pytweening-1.0.4/pytweening/
--rw-rw-rw-   0        0        0    16939 2021-09-14 03:21:41.000000 pytweening-1.0.4/pytweening/__init__.py
--rw-rw-rw-   0        0        0       42 2021-09-14 03:34:02.527811 pytweening-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1899 2021-09-14 03:29:42.000000 pytweening-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-09-14 03:34:02.515837 pytweening-1.0.4/tests/
--rw-rw-rw-   0        0        0     4584 2015-09-09 18:30:07.000000 pytweening-1.0.4/tests/basicTests.py
--rw-rw-rw-   0        0        0     3229 2015-09-09 18:30:07.000000 pytweening-1.0.4/tests/generateExcelGraphs.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.360048 pytweening-1.0.5/
+-rw-rw-rw-   0        0        0      117 2018-09-24 23:55:11.000000 pytweening-1.0.5/.gitignore
+-rw-rw-rw-   0        0        0      463 2023-04-25 21:47:28.000000 pytweening-1.0.5/AUTHORS.txt
+-rw-rw-rw-   0        0        0      248 2015-10-28 23:47:22.000000 pytweening-1.0.5/CHANGES.txt
+-rw-rw-rw-   0        0        0     1514 2014-07-17 23:32:58.000000 pytweening-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      222 2021-09-14 17:31:54.000000 pytweening-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4868 2023-04-25 21:57:08.360048 pytweening-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1519 2021-09-01 21:18:54.000000 pytweening-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.298032 pytweening-1.0.5/docs/
+-rw-rw-rw-   0        0        0     6778 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/Makefile
+-rw-rw-rw-   0        0        0     8443 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/conf.py
+-rw-rw-rw-   0        0        0      457 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/index.rst
+-rwxrwxrwx   0        0        0     6709 2014-08-04 08:42:22.000000 pytweening-1.0.5/docs/make.bat
+-rw-rw-rw-   0        0        0     1735 2023-04-25 21:52:51.000000 pytweening-1.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.302026 pytweening-1.0.5/pytweening/
+-rw-rw-rw-   0        0        0    18638 2023-04-25 21:52:10.000000 pytweening-1.0.5/pytweening/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.326040 pytweening-1.0.5/pytweening.egg-info/
+-rw-rw-rw-   0        0        0     4868 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      403 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 21:57:08.000000 pytweening-1.0.5/pytweening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:57:08.364054 pytweening-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 21:57:08.356047 pytweening-1.0.5/tests/
+-rw-rw-rw-   0        0        0     4989 2023-04-25 21:43:19.000000 pytweening-1.0.5/tests/basicTests.py
+-rw-rw-rw-   0        0        0     3229 2015-09-09 18:30:07.000000 pytweening-1.0.5/tests/generateExcelGraphs.py
+-rw-rw-rw-   0        0        0   606728 2015-09-09 18:30:07.000000 pytweening-1.0.5/tests/graphs.ipynb
+-rw-rw-rw-   0        0        0   118762 2015-09-09 18:31:30.000000 pytweening-1.0.5/tests/graphs.xlsx
+-rw-rw-rw-   0        0        0     1816 2023-04-25 16:35:05.000000 pytweening-1.0.5/tests/seeGraphs.py
```

### Comparing `pytweening-1.0.4/LICENSE.txt` & `pytweening-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.4/README.md` & `pytweening-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.4/docs/Makefile` & `pytweening-1.0.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.4/docs/conf.py` & `pytweening-1.0.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.4/docs/make.bat` & `pytweening-1.0.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytweening-1.0.4/pytweening/__init__.py` & `pytweening-1.0.5/pytweening/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import division
 
 import math
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 
 # from http://www.roguebasin.com/index.php?title=Bresenham%27s_Line_Algorithm#Python
 def getLine(x1, y1, x2, y2):
     """Returns a list of (x, y) tuples of every point on a line between
     (x1, y1) and (x2, y2). The x and y values inside the tuple are integers.
 
@@ -27,25 +27,25 @@
     >>> getLine(0, 0, 3, 6)
     [(0, 0), (0, 1), (1, 2), (1, 3), (2, 4), (2, 5), (3, 6)]
     >>> getLine(3, 3, -3, -3)
     [(3, 3), (2, 2), (1, 1), (0, 0), (-1, -1), (-2, -2), (-3, -3)]
     """
     x1, y1, x2, y2 = int(x1), int(y1), int(x2), int(y2)
     points = []
-    issteep = abs(y2-y1) > abs(x2-x1)
+    issteep = abs(y2 - y1) > abs(x2 - x1)
     if issteep:
         x1, y1 = y1, x1
         x2, y2 = y2, x2
     rev = False
     if x1 > x2:
         x1, x2 = x2, x1
         y1, y2 = y2, y1
         rev = True
     deltax = x2 - x1
-    deltay = abs(y2-y1)
+    deltay = abs(y2 - y1)
     error = int(deltax / 2)
     y = y1
     ystep = None
     if y1 < y2:
         ystep = 1
     else:
         ystep = -1
@@ -96,16 +96,15 @@
     """
     x = ((x2 - x1) * n) + x1
     y = ((y2 - y1) * n) + y1
     return (x, y)
 
 
 def _checkRange(n):
-    """Raises ValueError if the argument is not between 0.0 and 1.0.
-    """
+    """Raises ValueError if the argument is not between 0.0 and 1.0."""
     if not 0.0 <= n <= 1.0:
         raise ValueError('Argument must be between 0.0 and 1.0.')
 
 
 def linear(n):
     """A linear tween function
 
@@ -146,15 +145,15 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    return -n * (n-2)
+    return -n * (n - 2)
 
 
 def easeInOutQuad(n):
     """A quadratic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -163,15 +162,15 @@
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     if n < 0.5:
         return 2 * n**2
     else:
         n = n * 2 - 1
-        return -0.5 * (n*(n-2) - 1)
+        return -0.5 * (n * (n - 2) - 1)
 
 
 def easeInCubic(n):
     """A cubic tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -189,33 +188,33 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n - 1
+    n -= 1
     return n**3 + 1
 
 
 def easeInOutCubic(n):
     """A cubic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = 2 * n
+    n *= 2
     if n < 1:
         return 0.5 * n**3
     else:
-        n = n - 2
+        n -= 2
         return 0.5 * (n**3 + 2)
 
 
 def easeInQuart(n):
     """A quartic tween function that begins slow and then accelerates.
 
     Args:
@@ -234,33 +233,33 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n - 1
+    n -= 1
     return -(n**4 - 1)
 
 
 def easeInOutQuart(n):
     """A quartic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = 2 * n
+    n *= 2
     if n < 1:
         return 0.5 * n**4
     else:
-        n = n - 2
+        n -= 2
         return -0.5 * (n**4 - 2)
 
 
 def easeInQuint(n):
     """A quintic tween function that begins slow and then accelerates.
 
     Args:
@@ -279,36 +278,87 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n - 1
+    n -= 1
     return n**5 + 1
 
 
 def easeInOutQuint(n):
     """A quintic tween function that accelerates, reaches the midpoint, and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = 2 * n
+    n *= 2
     if n < 1:
         return 0.5 * n**5
     else:
-        n = n - 2
+        n -= 2
         return 0.5 * (n**5 + 2)
 
 
+def easeInPoly(n, degree=2):
+    """A polynomial tween function of given degree that begins slow and then accelerates.
+
+    Args:
+      n (float): The time progress, starting at 0.0 and ending at 1.0.
+
+    Returns:
+      (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
+    """
+    _checkRange(n)
+    if not isinstance(degree, (int, float)) or degree < 0:
+        raise ValueError('degree argument must be a positive number.')
+    return n**degree
+
+
+def easeOutPoly(n, degree=2):
+    """A polynomial tween function of given degree that begins fast and then decelerates.
+
+    Args:
+      n (float): The time progress, starting at 0.0 and ending at 1.0.
+
+    Returns:
+      (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
+    """
+    _checkRange(n)
+    if not isinstance(degree, (int, float)) or degree < 0:
+        raise ValueError('degree argument must be a positive number.')
+    return 1 - abs((n - 1) ** degree)
+
+
+def easeInOutPoly(n, degree=2):
+    """A polynomial tween function of given degree that accelerates, reaches the midpoint, and then decelerates.
+
+    Args:
+      n (float): The time progress, starting at 0.0 and ending at 1.0.
+
+    Returns:
+      (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
+    """
+    _checkRange(n)
+    if not isinstance(degree, (int, float)) or degree < 0:
+        raise ValueError('degree argument must be a positive number.')
+
+    n *= 2
+    if n < 1:
+        return 0.5 * n**degree
+    else:
+        n -= 2
+        return 1 - 0.5 * abs(n**degree)
+
+
 def easeInSine(n):
     """A sinusoidal tween function that begins slow and then accelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
@@ -353,15 +403,15 @@
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     if n == 0:
         return 0
     else:
-        return 2**(10 * (n - 1))
+        return 2 ** (10 * (n - 1))
 
 
 def easeOutExpo(n):
     """An exponential tween function that begins fast and then decelerates.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -387,17 +437,17 @@
     """
     _checkRange(n)
     if n == 0:
         return 0
     elif n == 1:
         return 1
     else:
-        n = n * 2
+        n *= 2
         if n < 1:
-            return 0.5 * 2**(10 * (n - 1))
+            return 0.5 * 2 ** (10 * (n - 1))
         else:
             n -= 1
             # 0.5 * (-() + 2)
             return 0.5 * (-1 * (2 ** (-10 * n)) + 2)
 
 
 def easeInCirc(n):
@@ -433,33 +483,33 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n * 2
+    n *= 2
     if n < 1:
         return -0.5 * (math.sqrt(1 - n**2) - 1)
     else:
-        n = n - 2
+        n -= 2
         return 0.5 * (math.sqrt(1 - n**2) + 1)
 
 
 def easeInElastic(n, amplitude=1, period=0.3):
     """An elastic tween function that begins with an increasing wobble and then snaps into the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    return 1 - easeOutElastic(1-n, amplitude=amplitude, period=period)
+    return 1 - easeOutElastic(1 - n, amplitude=amplitude, period=period)
 
 
 def easeOutElastic(n, amplitude=1, period=0.3):
     """An elastic tween function that overshoots the destination and then "rubber bands" into the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -471,15 +521,15 @@
 
     if amplitude < 1:
         amplitude = 1
         s = period / 4
     else:
         s = period / (2 * math.pi) * math.asin(1 / amplitude)
 
-    return amplitude * 2**(-10*n) * math.sin((n-s)*(2*math.pi / period)) + 1
+    return amplitude * 2 ** (-10 * n) * math.sin((n - s) * (2 * math.pi / period)) + 1
 
 
 def easeInOutElastic(n, amplitude=1, period=0.5):
     """An elastic tween function wobbles towards the midpoint.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -488,15 +538,15 @@
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
     n *= 2
     if n < 1:
         return easeInElastic(n, amplitude=amplitude, period=period) / 2
     else:
-        return easeOutElastic(n-1, amplitude=amplitude, period=period) / 2 + 0.5
+        return easeOutElastic(n - 1, amplitude=amplitude, period=period) / 2 + 0.5
 
 
 def easeInBack(n, s=1.70158):
     """A tween function that backs up first at the start and then goes to the destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
@@ -514,29 +564,29 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n - 1
+    n -= 1
     return n * n * ((s + 1) * n + s) + 1
 
 
 def easeInOutBack(n, s=1.70158):
     """A "back-in" tween function that overshoots both the start and destination.
 
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    n = n * 2
+    n *= 2
     if n < 1:
         s *= 1.525
         return 0.5 * (n * n * ((s + 1) * n - s))
     else:
         n -= 2
         s *= 1.525
         return 0.5 * (n * n * ((s + 1) * n + s) + 2)
@@ -561,24 +611,24 @@
     Args:
       n (float): The time progress, starting at 0.0 and ending at 1.0.
 
     Returns:
       (float) The line progress, starting at 0.0 and ending at 1.0. Suitable for passing to getPointOnLine().
     """
     _checkRange(n)
-    if n < (1/2.75):
+    if n < (1 / 2.75):
         return 7.5625 * n * n
-    elif n < (2/2.75):
-        n -= (1.5/2.75)
+    elif n < (2 / 2.75):
+        n -= 1.5 / 2.75
         return 7.5625 * n * n + 0.75
-    elif n < (2.5/2.75):
-        n -= (2.25/2.75)
+    elif n < (2.5 / 2.75):
+        n -= 2.25 / 2.75
         return 7.5625 * n * n + 0.9375
     else:
-        n -= (2.65/2.75)
+        n -= 2.65 / 2.75
         return 7.5625 * n * n + 0.984375
 
 
 def easeInOutBounce(n):
     """A bouncing tween function that bounces at the start and end.
 
     Args:
```

### Comparing `pytweening-1.0.4/tests/basicTests.py` & `pytweening-1.0.5/tests/basicTests.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     'easeInOutElastic',
     'easeInBack',
     'easeOutBack',
     'easeInOutBack',
     'easeInBounce',
     'easeOutBounce',
     'easeInOutBounce',
+    'easeInPoly',
+    'easeOutPoly',
+    'easeInOutPoly',
 ]
 
 
 # https://stackoverflow.com/q/6655724/
 class CustomAssertions(object):
     def assertFuncValue(self, func, param, expected, funcname='function', extra_msg='', **kwargs):
         """Asserts that func(param) == expected.
@@ -73,44 +76,53 @@
                 self.assertEqual((int(x), int(y)), (linePoints[0][0], linePoints[0][1]), 'Start point of getPointOnLine() is not the same as the line\'s start point.')
                 x, y = pytweening.getPointOnLine(startPoint[0], startPoint[1], endPoint[0], endPoint[1], 1.0)
                 self.assertEqual((int(x), int(y)), (linePoints[-1][0], linePoints[-1][1]), 'End point of getPointOnLine() is not the same as the line\'s end point.')
 
 
 class TestAll(unittest.TestCase, CustomAssertions):
     def test_zero(self):
+        delta = 2 ** -15  # i.e. VERY small
         for name in TWEENS:
             func = getattr(pytweening, name)
-            delta = 2 ** -15  # i.e. VERY small
             if name in ['easeInElastic', 'easeInOutElastic']:
                 delta = 2 ** -11  # around 0.0005
             elif name in ['easeInBounce', 'easeInOutBounce']:
                 delta = 2 ** -7  # around 0.0078
             self.assertFuncValue(func,   0, 0, name, delta=delta)
             self.assertFuncValue(func, 0.0, 0, name, delta=delta)
 
     def test_one(self):
+        delta = 2 ** -15  # i.e. VERY small
         for name in TWEENS:
             func = getattr(pytweening, name)
-            delta = 2 ** -15  # i.e. VERY small
             if name in ['easeOutElastic', 'easeInOutElastic']:
                 delta = 2 ** -11  # around 0.0005
             elif name in ['easeOutBounce', 'easeInOutBounce']:
                 delta = 2 ** -7  # around 0.0078
             self.assertFuncValue(func,   1, 1, name, delta=delta)
             self.assertFuncValue(func, 1.0, 1, name, delta=delta)
 
+    def test_halfway(self):
+        # Check that all the easeInOut* functions are halfway when passed 0.5.
+        delta = 2 ** -15  # i.e. VERY small
+        for name in TWEENS:
+            func = getattr(pytweening, name)
+            if name.startswith('easeInOut'):
+                self.assertFuncValue(func, 0.5, 0.5, name, delta=delta)
+
     def test_wrong_input(self):
         for name in TWEENS:
             func = getattr(pytweening, name)
             for input in [-1, -0.5, 1.5, 2]:
                 kwargs = {}
                 if sys.version_info.major >= 3 and sys.version_info.minor >= 3:
                     # msg parameter was added in Python 3.3:
                     # https://docs.python.org/3/library/unittest.html#unittest.TestCase.assertRaises
                     kwargs['msg'] = '{0}({1}) should raise ValueError'.format(name, input)
 
                 with self.assertRaises(ValueError, **kwargs):
                     func(input)
 
 
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pytweening-1.0.4/tests/generateExcelGraphs.py` & `pytweening-1.0.5/tests/generateExcelGraphs.py`

 * *Files identical despite different names*

