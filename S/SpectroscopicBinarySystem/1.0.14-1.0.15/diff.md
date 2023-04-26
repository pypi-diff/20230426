# Comparing `tmp/SpectroscopicBinarySystem-1.0.14.tar.gz` & `tmp/SpectroscopicBinarySystem-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpectroscopicBinarySystem-1.0.14.tar", last modified: Tue Apr 25 14:46:01 2023, max compression
+gzip compressed data, was "SpectroscopicBinarySystem-1.0.15.tar", last modified: Tue Apr 25 15:58:03 2023, max compression
```

## Comparing `SpectroscopicBinarySystem-1.0.14.tar` & `SpectroscopicBinarySystem-1.0.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:01.199662 SpectroscopicBinarySystem-1.0.14/
--rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.14/LICENSE
--rw-rw-rw-   0        0        0     1812 2023-04-25 14:46:01.199662 SpectroscopicBinarySystem-1.0.14/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2023-04-25 12:20:47.000000 SpectroscopicBinarySystem-1.0.14/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:01.199662 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/
--rw-rw-rw-   0        0        0     1812 2023-04-25 14:46:01.000000 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-04-25 14:46:01.000000 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 14:46:01.000000 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-04-25 14:46:01.000000 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-25 14:46:01.000000 SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.14/pyproject.toml
--rw-rw-rw-   0        0        0      724 2023-04-25 14:46:01.206527 SpectroscopicBinarySystem-1.0.14/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 14:46:01.199662 SpectroscopicBinarySystem-1.0.14/spectroscopicbinarysystem/
--rw-rw-rw-   0        0        0    24156 2023-04-25 14:44:13.000000 SpectroscopicBinarySystem-1.0.14/spectroscopicbinarysystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/
+-rw-rw-rw-   0        0        0     1533 2023-04-25 10:21:18.000000 SpectroscopicBinarySystem-1.0.15/LICENSE
+-rw-rw-rw-   0        0        0     1727 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/PKG-INFO
+-rw-rw-rw-   0        0        0     1336 2023-04-25 14:55:51.000000 SpectroscopicBinarySystem-1.0.15/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.949714 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/
+-rw-rw-rw-   0        0        0     1727 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-25 15:58:03.000000 SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-04-25 13:20:57.000000 SpectroscopicBinarySystem-1.0.15/pyproject.toml
+-rw-rw-rw-   0        0        0      724 2023-04-25 15:58:03.957713 SpectroscopicBinarySystem-1.0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 15:58:03.949714 SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/
+-rw-rw-rw-   0        0        0    24777 2023-04-25 15:56:36.000000 SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/__init__.py
```

### Comparing `SpectroscopicBinarySystem-1.0.14/LICENSE` & `SpectroscopicBinarySystem-1.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `SpectroscopicBinarySystem-1.0.14/PKG-INFO` & `SpectroscopicBinarySystem-1.0.15/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.14
+Version: 1.0.15
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -33,19 +33,20 @@
 Download sample data (see **/examples/alphadra** directory)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-sbs = SpectroscopicBinarySystem('hd123299', 
-                                './examples/alphadra/', 
-                                t0=2451441.804, 
-                                period_guess=51, 
-                                debug=True)
+sbs = SpectroscopicBinarySystem(
+    object_name='hd123299',
+    spectra_path='./examples/alphadra/',
+    t0=2451441.804,
+    period_guess=51,
+    debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
```

### Comparing `SpectroscopicBinarySystem-1.0.14/README.md` & `SpectroscopicBinarySystem-1.0.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 Download sample data (see **/examples/alphadra** directory)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-sbs = SpectroscopicBinarySystem('hd123299', 
-                                './examples/alphadra/', 
-                                t0=2451441.804, 
-                                period_guess=51, 
-                                debug=True)
+sbs = SpectroscopicBinarySystem(
+    object_name='hd123299',
+    spectra_path='./examples/alphadra/',
+    t0=2451441.804,
+    period_guess=51,
+    debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
```

### Comparing `SpectroscopicBinarySystem-1.0.14/SpectroscopicBinarySystem.egg-info/PKG-INFO` & `SpectroscopicBinarySystem-1.0.15/SpectroscopicBinarySystem.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SpectroscopicBinarySystem
-Version: 1.0.14
+Version: 1.0.15
 Summary: Python astronomy tools for spectroscopic binary system
 Author: Guillaume Bertrand
 Author-email: gbe.io@pm.me
 License: BSD-3-Clause
 Keywords: astronomy,astrophysics,science,fits,models,fitting,spectroscopy,spectrum
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -33,19 +33,20 @@
 Download sample data (see **/examples/alphadra** directory)
 
 And run this code :
 
 ```python
 from spectroscopicbinarysystem import SpectroscopicBinarySystem
 
-sbs = SpectroscopicBinarySystem('hd123299', 
-                                './examples/alphadra/', 
-                                t0=2451441.804, 
-                                period_guess=51, 
-                                debug=True)
+sbs = SpectroscopicBinarySystem(
+    object_name='hd123299',
+    spectra_path='./examples/alphadra/',
+    t0=2451441.804,
+    period_guess=51,
+    debug=True)
 
 # plot result with matplotlib and save the results
 sbs.plotRadialVelocityCurve(title="α Dra - HD123299 - Phased radial velocities", savefig=True)
 
 # display result with plotly
 sbs.plotlyRadialVelocityCurve(
     title="α Dra - HD123299 - Phased radial velocities")
```

### Comparing `SpectroscopicBinarySystem-1.0.14/setup.cfg` & `SpectroscopicBinarySystem-1.0.15/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2053 7065 6374 726f 7363 6f70 6963   = Spectroscopic
 00000020: 4269 6e61 7279 5379 7374 656d 0d0a 7665  BinarySystem..ve
-00000030: 7273 696f 6e20 3d20 312e 302e 3134 0d0a  rsion = 1.0.14..
+00000030: 7273 696f 6e20 3d20 312e 302e 3135 0d0a  rsion = 1.0.15..
 00000040: 6175 7468 6f72 203d 2047 7569 6c6c 6175  author = Guillau
 00000050: 6d65 2042 6572 7472 616e 640d 0a61 7574  me Bertrand..aut
 00000060: 686f 725f 656d 6169 6c20 3d20 6762 652e  hor_email = gbe.
 00000070: 696f 4070 6d2e 6d65 0d0a 6465 7363 7269  io@pm.me..descri
 00000080: 7074 696f 6e20 3d20 5079 7468 6f6e 2061  ption = Python a
 00000090: 7374 726f 6e6f 6d79 2074 6f6f 6c73 2066  stronomy tools f
 000000a0: 6f72 2073 7065 6374 726f 7363 6f70 6963  or spectroscopic
```

### Comparing `SpectroscopicBinarySystem-1.0.14/spectroscopicbinarysystem/__init__.py` & `SpectroscopicBinarySystem-1.0.15/spectroscopicbinarysystem/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -399,16 +399,16 @@
                 observers[obs] = colors[color_number]
                 color_number += 1
             color = observers[obs]
 
             # get the instrument
 
             label = f"{obs} - {s.getInstrument()[:30]}…"
-            if (label not in instruments.keys()):
-                if not obs in marker_index:
+            if label not in instruments.keys():
+                if obs not in marker_index:
                     marker_index[obs] = 0
                 instruments[label] = markers_style[marker_index[obs]]
                 marker_index[obs] += 1
                 axs[0].errorbar(s.getPhase(), s.getRV(
                 ), yerr=0, label=label, ecolor='k', capsize=0, fmt=instruments[label], color=color, lw=0.7, markersize=4)
             else:
                 axs[0].errorbar(s.getPhase(), s.getRV(), yerr=0,
@@ -434,15 +434,15 @@
                           labelpad=None, fontname='monospace', size=8)
         axs[0].grid(color='grey', alpha=0.2, linestyle='-',
                     linewidth=0.5, axis='both', which='both')
         axs[1].grid(color='grey', alpha=0.2, linestyle='-',
                     linewidth=0.5, axis='both', which='both')
 
         # If self._t0 compute phase delta between T0 of the model and the fixed value
-        if (self._t0):
+        if self._t0:
             t0 = self._t0
             phase1 = self.__getPhase(
                 t0, self._orbital_solution[0][5], self._orbital_solution[0][4]+2400000)
             phase2 = 1.0
             v0 = phase1 - phase2
         # Else use t0 compute by the model
         else:
@@ -476,23 +476,19 @@
                       frameon=False, prop={'size': 8})
         plt.tight_layout(pad=1, w_pad=0, h_pad=1)
         plt.xticks(np.arange(0, 1.01, 0.1))
         if savefig:
             plt.savefig(f'{self._spectra_path}/sbs_phased_result.png', dpi=dpi)
         plt.show()
 
-    def plotlyRadialVelocityCurve(self, title, subtitle="", rv_y_multiple=10, residual_y_multiple=0.5,
-                                  font_family='monospace', font_size=9, show=True):
+    def plotlyRadialVelocityCurve(self, title, font_family='monospace', font_size=9, show=True, group_by_instrument=True):
         """
         Plot the radial velocity curve using plotly
         # Todo : update parameters and link to yaml config file
         :param title:
-        :param subtitle:
-        :param rv_y_multiple:
-        :param residual_y_multiple:
         :param font_family:
         :param font_size:
         :param show:
         :return: fig
         """
 
         if not self._orbital_solution:
@@ -551,31 +547,52 @@
             if (obs not in observers.keys()):
                 rgb = colors[color_number][:3] * 255
                 str_rgb = ",".join([str(rgb[0]), str(rgb[1]), str(rgb[2])])
                 observers[obs] = f'rgba({str_rgb}, {colors[color_number][3]})'
                 color_number += 1
             color = observers[obs]
 
-            # set label
-            label = f"{obs} - {s.getDate()}"
-
-            # get the instrument
-            label = f"{obs} - {s.getInstrument()[:30]}…"
-            if (label not in instruments.keys()):
-                if not obs in marker_index:
-                    marker_index[obs] = 0
-                instruments[label] = markers_style[marker_index[obs]]
-                marker_index[obs] += 1
-                fig.add_trace(
-                    go.Scatter(x=[phase], y=[s.getRV()], mode='markers', name=label, marker_symbol=instruments[label], marker=dict(color=color,
-                                                                                                                                   size=8), showlegend=True))
-            else:
+            if group_by_instrument:
+                # get the instrument
+                label = f"{obs} - {s.getInstrument()[:30]}…"
+                if label in instruments:
+                    fig.add_trace(
+                        go.Scatter(x=[phase],
+                                   y=[s.getRV()],
+                                   mode='markers',
+                                   marker_symbol=instruments[label],
+                                   marker=dict(color=color,
+                                               size=8),
+                                   showlegend=False))
+                else:
+                    if obs not in marker_index:
+                        marker_index[obs] = 0
+                    instruments[label] = markers_style[marker_index[obs]]
+                    marker_index[obs] += 1
+                    fig.add_trace(
+                        go.Scatter(x=[phase],
+                                   y=[s.getRV()],
+                                   mode='markers',
+                                   name=label,
+                                   marker_symbol=instruments[label],
+                                   marker=dict(color=color,
+                                               size=8),
+                                   showlegend=True))
+            else: # no grouping
+                # set label to date
+                label = f"{obs} - {s.getDate()}"
                 fig.add_trace(
-                    go.Scatter(x=[phase], y=[s.getRV()], mode='markers', marker_symbol=instruments[label], marker=dict(color=color,
-                                                                                                                       size=8), showlegend=False))
+                    go.Scatter(x=[phase],
+                               y=[s.getRV()],
+                               mode='markers',
+                               name=label,
+                               marker_symbol='circle',
+                               marker=dict(color=color,
+                                           size=8),
+                               showlegend=False))
 
             # set hover text size
             fig.update_traces(hovertemplate=None,
                               hoverlabel=dict(font_size=16))
 
             # set hover text config
             fig.update_layout(hovermode="x unified",
@@ -595,26 +612,26 @@
                 tickvals=np.arange(0, 1.01, 0.1),
                 gridcolor='lightgrey',
                 linecolor='black',
                 ticktext=[f'{round(i, 2)}' for i in np.arange(0, 1.01, 0.1)],
                 mirror=True
             ),
             xaxis_title="Phase",
-            yaxis_title="Radial velocity [km $s^{-1}$]",
+            yaxis_title="Radial Velocity (km/s)",
             yaxis=dict(
                 ticks='outside',
                 showline=True,
                 linecolor='black',
                 gridcolor='lightgrey',
                 mirror=True
             ),
             font=dict(
                 family=font_family,
                 size=int(font_size)+2,
-                color="black"
+                color="black",
             )
         )
 
         # plot
         if show:
             fig.show()
```

