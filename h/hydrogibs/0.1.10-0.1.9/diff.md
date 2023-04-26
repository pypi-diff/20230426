# Comparing `tmp/hydrogibs-0.1.10.tar.gz` & `tmp/hydrogibs-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrogibs-0.1.10.tar", last modified: Wed Apr 26 08:25:10 2023, max compression
+gzip compressed data, was "hydrogibs-0.1.9.tar", last modified: Tue Apr 25 13:36:59 2023, max compression
```

## Comparing `hydrogibs-0.1.10.tar` & `hydrogibs-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-26 08:25:10.716876 hydrogibs-0.1.10/
--rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.10/LICENSE
--rw-rw-r--   0 axel      (1000) axel      (1000)      538 2023-04-26 08:25:10.716876 hydrogibs-0.1.10/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.10/README.md
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-26 08:25:10.712876 hydrogibs-0.1.10/hydrogibs/
--rw-rw-r--   0 axel      (1000) axel      (1000)    22271 2023-04-26 08:21:36.000000 hydrogibs-0.1.10/hydrogibs/GR4.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.10/hydrogibs/QDF.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.10/hydrogibs/RationalMethod.py
--rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.10/hydrogibs/SoCoSe.py
--rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.10/hydrogibs/__init__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.10/hydrogibs/__main__.py
--rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.10/hydrogibs/misc.py
-drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-26 08:25:10.716876 hydrogibs-0.1.10/hydrogibs.egg-info/
--rw-rw-r--   0 axel      (1000) axel      (1000)      538 2023-04-26 08:25:10.000000 hydrogibs-0.1.10/hydrogibs.egg-info/PKG-INFO
--rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-26 08:25:10.000000 hydrogibs-0.1.10/hydrogibs.egg-info/SOURCES.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-26 08:25:10.000000 hydrogibs-0.1.10/hydrogibs.egg-info/dependency_links.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-26 08:25:10.000000 hydrogibs-0.1.10/hydrogibs.egg-info/top_level.txt
--rw-rw-r--   0 axel      (1000) axel      (1000)      486 2023-04-26 08:24:55.000000 hydrogibs-0.1.10/pyproject.toml
--rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-26 08:25:10.716876 hydrogibs-0.1.10/setup.cfg
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/
+-rw-rw-r--   0 axel      (1000) axel      (1000)     1073 2023-04-23 13:58:07.000000 hydrogibs-0.1.9/LICENSE
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)       37 2023-04-23 13:57:53.000000 hydrogibs-0.1.9/README.md
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/hydrogibs/
+-rw-rw-r--   0 axel      (1000) axel      (1000)    21938 2023-04-25 13:35:15.000000 hydrogibs-0.1.9/hydrogibs/GR4.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     2926 2023-04-25 12:03:41.000000 hydrogibs-0.1.9/hydrogibs/QDF.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      982 2023-04-25 11:49:20.000000 hydrogibs-0.1.9/hydrogibs/RationalMethod.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)      874 2023-04-25 11:52:06.000000 hydrogibs-0.1.9/hydrogibs/SoCoSe.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)       61 2023-04-25 12:03:58.000000 hydrogibs-0.1.9/hydrogibs/__init__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)        0 2023-04-25 12:12:22.000000 hydrogibs-0.1.9/hydrogibs/__main__.py
+-rw-rw-r--   0 axel      (1000) axel      (1000)     4748 2023-04-25 11:52:25.000000 hydrogibs-0.1.9/hydrogibs/misc.py
+drwxrwxr-x   0 axel      (1000) axel      (1000)        0 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/hydrogibs.egg-info/
+-rw-rw-r--   0 axel      (1000) axel      (1000)      537 2023-04-25 13:36:58.000000 hydrogibs-0.1.9/hydrogibs.egg-info/PKG-INFO
+-rw-rw-r--   0 axel      (1000) axel      (1000)      308 2023-04-25 13:36:59.000000 hydrogibs-0.1.9/hydrogibs.egg-info/SOURCES.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)        1 2023-04-25 13:36:58.000000 hydrogibs-0.1.9/hydrogibs.egg-info/dependency_links.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)       10 2023-04-25 13:36:59.000000 hydrogibs-0.1.9/hydrogibs.egg-info/top_level.txt
+-rw-rw-r--   0 axel      (1000) axel      (1000)      485 2023-04-25 13:36:12.000000 hydrogibs-0.1.9/pyproject.toml
+-rw-rw-r--   0 axel      (1000) axel      (1000)       38 2023-04-25 13:36:59.021605 hydrogibs-0.1.9/setup.cfg
```

### Comparing `hydrogibs-0.1.10/LICENSE` & `hydrogibs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.10/PKG-INFO` & `hydrogibs-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.10
+Version: 0.1.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hydrogibs-0.1.10/hydrogibs/GR4.py` & `hydrogibs-0.1.9/hydrogibs/GR4.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg,\
     NavigationToolbar2Tk
 from matplotlib.backend_bases import key_press_handler
 import customtkinter as ctk
-from typing import Callable, Literal
+from typing import Callable
+from dataclasses import dataclass
 
 
-def _transfer_func(X4: float, num: int) -> np.ndarray:  # m/km/s
+def _transfer_func(n: float, X4: float):  # m/km/s
     """
     This function will make the transition between the
     water flow and the discharge through a convolution
 
     discharge = convolution(_transfer_func(water_flow, time/X4))
-
-    Args:
-        - X4  (float): the hydrogram's raising time
-        - num  (int) : the number of elements to give to the array
-
-    Returns:
-        - f (np.ndarray): = 3/(2*X4) * n**2            if n <= 1
-                            3/(2*X4) * (2-n[n > 1])**2 if n >  1
     """
-    n = np.linspace(0, 2, num)
-    f = 3/(2*X4) * n**2
-    f[n > 1] = 3/(2*X4) * (2-n[n > 1])**2
-    return f
+    if n < 1:
+        return 3/(2*X4) * n**2
+    if n < 2:
+        return 3/(2*X4) * (2-n)**2
+    return 0
 
 
 class Rain:
     """
     Rain object to apply to a Catchment object.
 
     Args:
@@ -38,18 +32,19 @@
 
     Creates a GR4h object when called with a Catchment object:
     >>> gr4h = GR4h(catchment, rain)
     Creates an Event object when applied to a catchment
     >>> event = rain @ catchment
     """
 
-    def __init__(self, time: np.ndarray, rainfall: np.ndarray) -> None:
+    def __init__(self, time: np.ndarray, rain_func: Callable) -> None:
 
-        self.time = np.asarray(time)
-        self.rainfall = np.asarray(rainfall)
+        self.time = time
+        self.rain_func = rain_func
+        self.rainfall = np.array([rain_func(t) for t in time])
         self.timestep = time[1] - time[0]
 
     def __matmul__(self, catchment):
         return GR4h(catchment, self).apply()
 
 
 class BlockRain(Rain):
@@ -114,59 +109,45 @@
     def __init__(self,
                  X1: float,
                  X2: float,
                  X3: float,
                  X4: float,
                  surface: float = 1,
                  initial_volume: float = 0,
-                 transfer_function: Callable = None) -> None:
+                 transfer_function: Callable = _transfer_func) -> None:
 
         self.X1 = X1
         self.X2 = X2
         self.X3 = X3
         self.X4 = X4
         self.surface = surface
-        self.transfer_function = (transfer_function
-                                  if transfer_function is not None
-                                  else _transfer_func)
+        self.transfer_function = transfer_function
         self.initial_volume = initial_volume
 
         assert 0 <= X1 <= 1, "Runoff coefficient must be within [0 : 1]"
         assert 0 <= X2, "Initial abstraction must be positive"
         assert 0 <= X3 <= 1, "Emptying rate must be within [0 : 1]"
         assert 0 <= X4, "Raising time must be positive"
 
     def __matmul__(self, rain):
         return rain @ self
 
 
+@dataclass
 class Event:
-    """
-    Stores all relevant results of a GR4h calculation
-
-    basic class instead of dataclass, namedtuple or dataframe is used
-    for speed reasons (an event will be created at every diagram update)
-    """
-
-    def __init__(self,
-                 time: np.ndarray,
-                 rainfall: np.ndarray,
-                 volume: np.ndarray,
-                 water_flow: np.ndarray,
-                 discharge_rain: np.ndarray,
-                 discharge_volume: np.ndarray,
-                 discharge: np.ndarray) -> None:
 
-        self.time = time
-        self.rainfall = rainfall
-        self.volume = volume
-        self.water_flow = water_flow
-        self.discharge_rain = discharge_rain
-        self.discharge_volume = discharge_volume
-        self.discharge = discharge
+    time: np.ndarray
+    rainfall: np.ndarray
+    volume: np.ndarray
+    water_flow_rain: np.ndarray
+    water_flow_volume: np.ndarray
+    water_flow: np.ndarray
+    discharge_rain: np.ndarray
+    discharge_volume: np.ndarray
+    discharge: np.ndarray
 
     def diagram(self, *args, **kwargs):
         return GR4diagram(self, *args, **kwargs)
 
 
 class GR4diagram:
 
@@ -426,30 +407,35 @@
     i = time[np.cumsum(dP)*dt >= X2 - V0]
     t1 = i[0] if i.size else float("inf")
 
     dP_effective = dP.copy()
     dP_effective[time < t1] = 0
 
     # solution to the differential equation V' = -X3*V + (1-X1)*P
-    integral = np.cumsum(np.exp(X3*time) * dP_effective) * dt
-    cond_init = V0 * np.exp(-X3*time)
-    V = np.exp(-X3*time) * (1-X1) * integral + cond_init
+    V = (
+        np.exp(-X3*time) * (1-X1) *
+        np.cumsum(np.exp(X3*time) * dP_effective) * dt
+    )
+    V = V + V0 * np.exp(-X3*time)
 
     t_abstraction = time < t1
     dTp = X1*dP
-    dTv = X3*V
     dTp[t_abstraction] = 0
+    dTv = X3*V
     dTv[t_abstraction] = 0
 
-    q = catchment.transfer_function(X4, num=(time <= 2*X4).sum())
+    q = np.array([
+        catchment.transfer_function(ni, X4)
+        for ni in time[time <= 2*X4]/X4
+    ])
 
     Qp = S * np.convolve(dTp, q)[:time.size] * dt
     Qv = S * np.convolve(dTv, q)[:time.size] * dt
 
-    return Event(time, dP, V, dTp+dTv, Qp, Qv, Qp+Qv)
+    return Event(time, dP, V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
 def gr4_block_rain(catchment, block_rain) -> dict:
     """
     This method is fit for block events
     (constant rainfall intensity during a defined duration)
 
@@ -482,41 +468,41 @@
     X2 = catchment.X2
     X3 = catchment.X3
     X4 = catchment.X4
 
     S = catchment.surface
     V0 = catchment.initial_volume
 
+    transfer_function = catchment.transfer_function
+
     # Unpack rain attributes
     dt = block_rain.timestep
     t0 = block_rain.duration
     tf = block_rain.observation_span
 
     I0 = block_rain.intensity
     rainfall = block_rain.rainfall
 
-    dtype = np.float16
-
     # Initializing time
     tf = 10*t0 if tf is None else tf
     t = np.arange(start=0, stop=tf, step=dt)
 
     # End of abstraction
     t1 = X2/I0
 
     # Initialize volume
-    V = np.zeros_like(t, dtype=dtype)
+    V = np.zeros_like(t, dtype=np.float32)
     V += V0
 
-    dTp = np.zeros_like(t, dtype=dtype)
-    dTv = np.zeros_like(t, dtype=dtype)
+    dTp = np.zeros_like(t, dtype=np.float128)
+    dTv = np.zeros_like(t, dtype=np.float128)
 
     # Initial abstraction
     i = t < t1
-    A = np.zeros_like(t, dtype=dtype)
+    A = np.zeros_like(t, dtype=np.float16)
     A[i] = I0*t[i]
     A[t >= t1] = A[i][-1]
 
     # Runoff + rain
     i = (t >= t1) & (t <= t0)
     V[i] += I0*(1-X1)/X3 * (1 - np.exp(-(t[i]-t1)*X3))
     V1 = V[i][-1] if V[i].size else 0
@@ -526,21 +512,23 @@
 
     # Runoff, no more rain
     i = t >= t0
     V[i] = V1 * np.exp(-(t[i]-t0)*X3)
     dTv[i] = X3*V[i]
 
     # Evaluate transfer function
-    q = catchment.transfer_function(X4, num=(t <= 2*X4).sum())
-
+    q = np.array([
+        transfer_function(ni, X4)
+        for ni in t[t <= 2*X4]/X4
+    ])
     # Convolve
     Qp = S * np.convolve(dTp, q)[:t.size] * dt
     Qv = S * np.convolve(dTv, q)[:t.size] * dt
 
-    return Event(t, rainfall, V, dTp+dTv, Qp, Qv, Qp+Qv)
+    return Event(t, rainfall, V, dTp, dTv, dTp+dTv, Qp, Qv, Qp+Qv)
 
 
 class GR4App:
 
     def __init__(self, gr4: GR4h,
                  appearance: str = "dark",
                  color_theme: str = "dark-blue",
@@ -552,23 +540,33 @@
 
         ctk.set_appearance_mode(appearance)
         ctk.set_default_color_theme(color_theme)
 
         self.root = ctk.CTk()
         self.root.title("Génie Rural 4")
         self.root.bind('<Return>', self.entries_update)
+        # self.ww = self.root.winfo_screenwidth()
+        # self.wh = self.root.winfo_screenheight()
+        # self.root.geometry(f"{self.ww*0.8:.0f}x{self.wh*0.5:.0f}")
 
         self.dframe = ctk.CTkFrame(master=self.root)
         self.dframe.grid(row=0, column=1, sticky="NSEW")
 
         self.init_diagram(style=style, *args, **kwargs)
 
         self.pframe = ctk.CTkFrame(master=self.root)
         self.pframe.grid(column=0, row=0, sticky="NSEW")
 
+        # entryframe = ctk.CTkLabel(text="GR4 parameters",
+        #                           master=self.pframe,
+        #                           font=("monospace", 24))
+        # entryframe.grid(row=0, column=0,
+        #                 sticky="NSEW",
+        #                 ipadx=5, ipady=10)
+
         self.entries = dict()
         self.define_entry("X1", "-")
         self.define_entry("X2", "mm")
         self.define_entry("X3", "1/h")
         self.define_entry("X4", "h")
         self.define_entry("surface", "km²", "S")
         self.define_entry("initial_volume", "mm", "V0")
@@ -698,23 +696,21 @@
     def update(self):
 
         self.gr4.apply()
         self.diagram.update(self.gr4.event, self.gr4.rain)
         self.canvas.draw()
 
 
-def GR4_demo(kind: str = "array"):
+def GR4_demo(kind="block"):
 
     if kind == "block":
         rain = BlockRain(50, duration=1.8)
     else:
-        time = np.linspace(0, 10, 1000)
-        rainfall = np.array([50 if t < 2 else 0 for t in time])
         rain = Rain(
-            time=time,
-            rainfall=rainfall
+            time=np.linspace(0, 10, 1000),
+            rain_func=lambda t: 50 if t < 2 else 0
         )
     GR4h(Catchment(8/100, 40, 0.1, 1), rain).App()
 
 
 if __name__ == "__main__":
-    GR4_demo("block")
+    GR4_demo()
```

### Comparing `hydrogibs-0.1.10/hydrogibs/QDF.py` & `hydrogibs-0.1.9/hydrogibs/QDF.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.10/hydrogibs/RationalMethod.py` & `hydrogibs-0.1.9/hydrogibs/RationalMethod.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.10/hydrogibs/SoCoSe.py` & `hydrogibs-0.1.9/hydrogibs/SoCoSe.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.10/hydrogibs/misc.py` & `hydrogibs-0.1.9/hydrogibs/misc.py`

 * *Files identical despite different names*

### Comparing `hydrogibs-0.1.10/hydrogibs.egg-info/PKG-INFO` & `hydrogibs-0.1.9/hydrogibs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrogibs
-Version: 0.1.10
+Version: 0.1.9
 Summary: A small hydrology package
 Author-email: axel Giboulot <axel.giboulot@epfl.ch>
 Project-URL: Homepage, https://github.com/giboul/hydrogibs
 Project-URL: Bug Tracker, https://github.com/giboul/hydrogibs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

