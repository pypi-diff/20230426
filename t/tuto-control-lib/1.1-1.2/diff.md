# Comparing `tmp/tuto_control_lib-1.1-py3-none-any.whl.zip` & `tmp/tuto_control_lib-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6916 bytes, number of entries: 13
+Zip file size: 7002 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        1 b- defN 80-Jan-02 00:00 tuto_control_lib/__init__.py
--rw-r--r--  2.0 unx     1134 b- defN 80-Jan-02 00:00 tuto_control_lib/plot.py
--rw-r--r--  2.0 unx      767 b- defN 80-Jan-02 00:00 tuto_control_lib/systems.py
+-rw-r--r--  2.0 unx     1330 b- defN 80-Jan-02 00:00 tuto_control_lib/plot.py
+-rw-r--r--  2.0 unx      885 b- defN 80-Jan-02 00:00 tuto_control_lib/systems.py
 -rw-r--r--  2.0 unx     1784 b- defN 80-Jan-02 00:00 tuto_control_lib/cigri/__init__.py
 -rw-r--r--  2.0 unx     2467 b- defN 80-Jan-02 00:00 tuto_control_lib/cigri/cigri.py
 -rw-r--r--  2.0 unx     1656 b- defN 80-Jan-02 00:00 tuto_control_lib/cigri/events.py
 -rw-r--r--  2.0 unx     2105 b- defN 80-Jan-02 00:00 tuto_control_lib/cigri/jobs.py
 -rw-r--r--  2.0 unx     1617 b- defN 80-Jan-02 00:00 tuto_control_lib/cigri/oar.py
--rw-r--r--  2.0 unx     1075 b- defN 80-Jan-02 00:00 tuto_control_lib-1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      359 b- defN 80-Jan-02 00:00 tuto_control_lib-1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 80-Jan-02 00:00 tuto_control_lib-1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 80-Jan-02 00:00 tuto_control_lib-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1107 b- defN 80-Jan-02 00:00 tuto_control_lib-1.1.dist-info/RECORD
-13 files, 14181 bytes uncompressed, 5048 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1075 b- defN 80-Jan-02 00:00 tuto_control_lib-1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      359 b- defN 80-Jan-02 00:00 tuto_control_lib-1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 80-Jan-02 00:00 tuto_control_lib-1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 80-Jan-02 00:00 tuto_control_lib-1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1107 b- defN 80-Jan-02 00:00 tuto_control_lib-1.2.dist-info/RECORD
+13 files, 14495 bytes uncompressed, 5134 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: tuto_control_lib/cigri/jobs.py
 Comment: 
 
 Filename: tuto_control_lib/cigri/oar.py
 Comment: 
 
-Filename: tuto_control_lib-1.1.dist-info/LICENSE
+Filename: tuto_control_lib-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: tuto_control_lib-1.1.dist-info/METADATA
+Filename: tuto_control_lib-1.2.dist-info/METADATA
 Comment: 
 
-Filename: tuto_control_lib-1.1.dist-info/WHEEL
+Filename: tuto_control_lib-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: tuto_control_lib-1.1.dist-info/top_level.txt
+Filename: tuto_control_lib-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: tuto_control_lib-1.1.dist-info/RECORD
+Filename: tuto_control_lib-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tuto_control_lib/plot.py

```diff
@@ -3,43 +3,45 @@
 
 
 def plot_y(y_values):
     max_iter = len(y_values)
     xpoints = np.array(range(max_iter))
     ypoints = np.array(y_values)
 
-    plt.plot(xpoints, ypoints)
+    plt.plot(xpoints, ypoints, marker='.', linestyle='None')
+    plt.vlines(xpoints, [0], ypoints)
     plt.xlabel("Iterations")
     plt.ylabel("Sensor Output")
     plt.show()
 
 def plot_u_y(u_values, y_values, reference_value=None):
     max_iter = len(y_values)
     xpoints = np.array(range(max_iter))
     ypoints = np.array(y_values)
     upoints = np.array(u_values)
 
     plt.subplot(2, 1, 1)
-    plt.plot(xpoints, ypoints)
+    plt.plot(xpoints, ypoints, marker=".", linestyle='None')
+    plt.vlines(xpoints, [0], ypoints)
     if reference_value:
         plt.plot(xpoints, [reference_value for _ in range(max_iter)])
     plt.xlabel("Iterations")
     plt.ylabel("Sensor Output")
     plt.subplot(2, 1, 2)
-    plt.plot(xpoints, upoints)
+    plt.step(xpoints, upoints, ls='-', marker='.')
     plt.xlabel("Iterations")
     plt.ylabel("Input")
 
     plt.show()
 
 def plot_model_compa(y_values, model):
     max_iter = len(y_values)
     xpoints = np.array(range(max_iter))
     ypoints = np.array(y_values)
     modelpoints = np.array(model)
 
-    plt.plot(xpoints, ypoints)
-    plt.plot(xpoints, modelpoints)
+    plt.plot(xpoints, ypoints, ls='-', marker='.')
+    plt.plot(xpoints, modelpoints, ls='-', marker='.')
     plt.xlabel("Iterations")
     plt.ylabel("Sensor Output")
     plt.show()
```

## tuto_control_lib/systems.py

```diff
@@ -1,25 +1,30 @@
 import random
 
 class System:
     def __init__(self, a, b, y0=0, noise=False):
         self.y = y0
         self.noise = noise
         self.f = lambda y, u: a * y + b * u
+        self.iteration = 0
         
     def sense(self):
         if self.noise:
             y = self.y + random.random() / 10
             self.y = y if y > 0 else 0 
         return self.y
     
     def apply(self, u):
         self.y = self.f(self.y, u)
+        self.iteration += 1
         return self
         
+    def get_time(self):
+        return self.iteration
+        
 class IntroSystem(System):
     def __init__(self):
         System.__init__(self, 0.8, 0.5, y0=0, noise=False)
 
 class NoisySystem(System):
     def __init__(self):
         System.__init__(self, 0.8, 0.5, y0=0, noise=True)
```

## Comparing `tuto_control_lib-1.1.dist-info/LICENSE` & `tuto_control_lib-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tuto_control_lib-1.1.dist-info/RECORD` & `tuto_control_lib-1.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 tuto_control_lib/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-tuto_control_lib/plot.py,sha256=cZMQYHQRP_ag0jOmXMz3poDXfZBt2eJkfzD9wnFvGb0,1134
-tuto_control_lib/systems.py,sha256=dJolQwulVsU16z5a8ql0qy4XMfUfTMEzFukxHjn8Y3o,767
+tuto_control_lib/plot.py,sha256=OPWsT2a4KTjQk9tT9aCjN0e4t26HMj6Z9717pUPwTkQ,1330
+tuto_control_lib/systems.py,sha256=DioEAuWHaWvn84Kn1gZ58AJcFUQARdcMs7CkUcbe4qQ,885
 tuto_control_lib/cigri/__init__.py,sha256=I1-F0eCJccEr39Ux8u6JJyq76YhGg_qXUWx-L8sc830,1784
 tuto_control_lib/cigri/cigri.py,sha256=kmyP0GH2oyvd9p5MO0bS11cFz-rWZlLyGmWVwFdRcrs,2467
 tuto_control_lib/cigri/events.py,sha256=73VaMYikvjcsBpV-f5M4xovxWSMO0ttgi6N5q8jsIqU,1656
 tuto_control_lib/cigri/jobs.py,sha256=Z51_SIBbyQ05iGUPKlDL-yX1wbnzCbZw6R5Bzhkysds,2105
 tuto_control_lib/cigri/oar.py,sha256=lzWXw0IxSaoGaolXi1xP3Ef2TBMqG9l2HndAso9qEZA,1617
-tuto_control_lib-1.1.dist-info/LICENSE,sha256=kKZw2E5NzPGyNmdVyHbMRRrczPRqlvqKv0JY0I-fGWg,1075
-tuto_control_lib-1.1.dist-info/METADATA,sha256=3uabtbWDHS72QKOf_vVZ-Yhz__Q5EnLcQrTuQ330SvY,359
-tuto_control_lib-1.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-tuto_control_lib-1.1.dist-info/top_level.txt,sha256=_313QaXmQ_goOMhswYVKmKUDc_7iIRxYuiOnWfZpLr0,17
-tuto_control_lib-1.1.dist-info/RECORD,,
+tuto_control_lib-1.2.dist-info/LICENSE,sha256=kKZw2E5NzPGyNmdVyHbMRRrczPRqlvqKv0JY0I-fGWg,1075
+tuto_control_lib-1.2.dist-info/METADATA,sha256=Q1gn2xz2n_PNO6XwDY3Q7KN_vtSodiRit5OqJoxp8WQ,359
+tuto_control_lib-1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+tuto_control_lib-1.2.dist-info/top_level.txt,sha256=_313QaXmQ_goOMhswYVKmKUDc_7iIRxYuiOnWfZpLr0,17
+tuto_control_lib-1.2.dist-info/RECORD,,
```

