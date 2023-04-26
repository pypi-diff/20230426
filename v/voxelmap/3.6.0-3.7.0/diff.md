# Comparing `tmp/voxelmap-3.6.0.tar.gz` & `tmp/voxelmap-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelmap-3.6.0.tar", max compression
+gzip compressed data, was "voxelmap-3.7.0.tar", max compression
```

## Comparing `voxelmap-3.6.0.tar` & `voxelmap-3.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-3.6.0/LICENSE
--rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-3.6.0/README.md
--rw-r--r--   0        0        0      591 2023-04-02 16:34:25.566115 voxelmap-3.6.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-3.6.0/voxelmap/__init__.py
--rw-r--r--   0        0        0    17220 2023-03-31 17:25:56.067763 voxelmap-3.6.0/voxelmap/annex.py
--rwxr-xr-x   0        0        0    26636 2023-04-02 23:19:22.019369 voxelmap-3.6.0/voxelmap/jotunn.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-3.6.0/setup.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-01-14 04:48:56.741276 voxelmap-3.7.0/LICENSE
+-rw-r--r--   0        0        0     1762 2023-03-28 06:03:09.266535 voxelmap-3.7.0/README.md
+-rw-r--r--   0        0        0      591 2023-04-26 18:14:30.951974 voxelmap-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-04-02 23:36:39.545755 voxelmap-3.7.0/voxelmap/__init__.py
+-rw-r--r--   0        0        0    17220 2023-03-31 17:25:56.067763 voxelmap-3.7.0/voxelmap/annex.py
+-rwxr-xr-x   0        0        0    29140 2023-04-26 18:13:03.766171 voxelmap-3.7.0/voxelmap/jotunn.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 voxelmap-3.7.0/setup.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 voxelmap-3.7.0/PKG-INFO
```

### Comparing `voxelmap-3.6.0/LICENSE` & `voxelmap-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelmap-3.6.0/README.md` & `voxelmap-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `voxelmap-3.6.0/pyproject.toml` & `voxelmap-3.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voxelmap"
-version = "3.6.0"
+version = "3.7.0"
 description = "A Python library for making voxel and 3D models from NumPy arrays."
 authors = ["andrewrgarcia <garcia.gtr@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `voxelmap-3.6.0/voxelmap/annex.py` & `voxelmap-3.7.0/voxelmap/annex.py`

 * *Files identical despite different names*

### Comparing `voxelmap-3.6.0/voxelmap/jotunn.py` & `voxelmap-3.7.0/voxelmap/jotunn.py`

 * *Files 3% similar despite different names*

```diff
@@ -352,17 +352,20 @@
     def draw(self, coloring='none', geometry = 'voxels', scalars='', background_color='#cccccc', wireframe=False, window_size=[1024, 768],voxel_spacing=(1,1,1)):
         '''Draws voxel model after building it with the provided `array` with PyVista library
 
         Parameters
         ----------
         coloring: string  
             voxel coloring scheme
-                * 'custom' --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
-                * 'custom: #8599A6' -->  color all voxel types with the #8599A6 hex color (bluish dark gray) and an alpha transparency of 1.0 (default)
-                * 'custom: red, alpha: 0.24' --> color all voxel types red and with an alpha transparency of 0.24
+                * 'custom'                      --> colors voxel model based on the provided keys to its array integers, defined in the `hashblocks` variable from the `Model` class
+                * 'custom: #8599A6'             -->  color all voxel types with the #8599A6 hex color (bluish dark gray) and an alpha transparency of 1.0 (default)
+                * 'custom: red, alpha: 0.24'    --> color all voxel types red and with an alpha transparency of 0.24
+                * 'cmap : {colormap name}' :        colors voxel model based on a colormap; assigns colors from the chosen colormap to the defined array integers
+                * 'cmap : viridis'              --> colormap voxel assignment with the viridis colormap
+                * 'cmap : hot', alpha: 0.56     --> voxel assignment with the hot colormap with an alpha transparency of 0.56
                 * 'none'   --> no coloring 
                 * 'cool'      cool colormap
                 * 'fire'      fire colormap
                 * and so on...
         geometry: string  
             voxel geometry. Choose voxels to have a box geometry with geometry='voxels' or spherical one with geometry='particles'
         scalars : list
@@ -370,55 +373,101 @@
         background_color : string / hex
             background color of pyvista plot
         window_size : (float,float)
             defines plot window dimensions. Defaults to [1024, 768], unless set differently in the relevant theme’s window_size property [pyvista.Plotter]
         voxel_spacing : (float,float,float)
             changes voxel spacing by defining length scales of x y and z directions (default:(1,1,1)).
         '''
-
         xx, yy, zz, voxid = arr2crds(self.array, -1).T
 
         centers = np.vstack((xx.ravel(), yy.ravel(), zz.ravel())).T
 
         pl = pyvista.Plotter(window_size=window_size)
 
         if background_color != "":
             pl.background_color = background_color
 
+        # Custom Coloring Code Block
         if coloring[:6] == 'custom':
             color_details= coloring.split(':')
 
             if len(color_details) > 1:
                 if len(color_details) > 2:
                     color_all = color_details[1].split(',')[0].strip()
                     alpha_all  = float(color_details[2])
                 else: 
                     color_all = color_details[1].strip()
                     alpha_all  = 1.0
 
-                iterlist = np.unique(self.array[self.array!=0]) if len(self.hashblocks)==0 else self.hashblocks.keys()      #iterate list over all non-zero integer types 
+                # iterate list over all non-zero integer types 
+                voxel_types = np.unique(self.array[self.array!=0]) if len(self.hashblocks)==0 else self.hashblocks.keys()      
 
-                for i in iterlist:
+                for i in voxel_types:
                     self.hashblocks[i] = [color_all,alpha_all] 
                         
             print('Voxelmap draw. Using custom colors:\nself.hashblocks =\n',self.hashblocks)
 
+        # Colormap Coloring Code Block
+        if coloring[:4] == 'cmap':
+            color_details= coloring.split(':')
+
+            if len(color_details) > 1:
+                if len(color_details) > 2:
+                    colormap = color_details[1].split(',')[0].strip()
+                    alpha_all  = float(color_details[2])
+                else: 
+                    colormap = color_details[1].strip()
+                    alpha_all  = 1.0
+
+                # iterate list over all non-zero integer types 
+                voxel_types = np.unique(self.array[self.array!=0]) 
+
+                try:
+                    memory_blocks = False
+                    if len(self.hashblocks)!=0:
+                        #keep defined hashblocks in memory
+                        memory_blocks = self.hashblocks.copy()
+                        for j in memory_blocks.keys():
+                            voxel_types = voxel_types[voxel_types != j]
+
+                    cmap = eval('plt.cm.'+colormap)
+                    norm = plt.Normalize(vmin=voxel_types.min(), vmax=voxel_types.max())  # data normalization (0,1)
+                    colorlist = cmap(norm(voxel_types))
+                    hex_colors = [colors.rgb2hex(color) for color in colorlist]
+
+                    for i in range(len(voxel_types)):
+                        k = voxel_types[i]
+                        col = hex_colors[i]
+                        self.hashblocks[k] = [col,alpha_all] 
+
+                    if memory_blocks:
+                        #add custom hashblocks from memory here
+                        for j in memory_blocks.keys():
+                            self.hashblocks[j] = memory_blocks[j]                            
+                    
+                    print('Voxelmap draw. Using custom colormap: ',colormap)
+
+                except: 
+                    print('ERROR: colormap {} does not exist / is not available ',colormap)
+
+
         for i in range(len(centers)):
 
             x_len,y_len,z_len = voxel_spacing
 
+            # Voxel Geometry
             if geometry == 'particles':
                 voxel = pyvista.Sphere(center=centers[i],radius=0.5)
                 smooth = True
             else:
                 voxel = pyvista.Cube(center=centers[i],x_length=x_len, y_length=y_len, z_length=z_len)
                 smooth= None
 
-            if coloring[:6] == 'custom' :
-
+            # Mesh creation and coloring
+            if coloring[:6] == 'custom' or coloring[:4] == 'cmap' :
                 voxel_color, voxel_alpha = self.hashblocks[voxid[i]]
                 pl.add_mesh(voxel, color=voxel_color, smooth_shading=smooth, opacity=voxel_alpha,show_edges=True if wireframe else False)
             elif coloring == 'none':
                 pl.add_mesh(voxel,smooth_shading=smooth, show_edges=True if wireframe else False)
             else:
                 pl.add_mesh(voxel, scalars=[i for i in range(
                     8)] if scalars == '' else scalars,smooth_shading=smooth, show_edges=True if wireframe else False, cmap=coloring)
```

### Comparing `voxelmap-3.6.0/setup.py` & `voxelmap-3.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'scikit-image>=0.19.3,<0.20.0',
  'scipy>=1.10.0,<2.0.0',
  'sphinx-rtd-theme>=1.2.0,<2.0.0',
  'sphinx>=6.1.3,<7.0.0']
 
 setup_kwargs = {
     'name': 'voxelmap',
-    'version': '3.6.0',
+    'version': '3.7.0',
     'description': 'A Python library for making voxel and 3D models from NumPy arrays.',
     'long_description': '# voxelmap\n\n[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[![Documentation Status](https://readthedocs.org/projects/voxelmap/badge/?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA Python library for making voxel and three-dimensional models from NumPy arrays. \n\n<a href="https://voxelmap.readthedocs.io/en/latest/">\n<img src="https://github.com/andrewrgarcia/voxelmap/blob/main/voxelmap.svg?raw=true" width="250"></a>\n\n## Installation and Local Usage \n\n```ruby\npip install voxelmap\n```\n\nIt is recommended you run voxelmap using a `virtualenv` virtual environment. To do so, follow the below simple protocol to create the virtual environment, run it, and install the package there:\n\n```ruby \nvirtualenv venv\nsource venv/bin/activate\npip install voxelmap\npython [your-voxelmap-script.py]\n```\nTo exit the virtual environment, simply type `deactivate`. To access it at any other time again, enter with the above `source venv...` command. \n\n## Just starting? Remote Usage with a Colab notebook (click below)\n\n<a href="https://colab.research.google.com/drive/1RMEMgZHlk_tKAzfS4QfXLJV9joDgdh8N?usp=sharing">\n<img src="https://raw.githubusercontent.com/andrewrgarcia/voxelmap/main/docs/img/colaboratory.png" width="500" ></a>\n\n\n## Disclaimer: Use At Your Own Risk\n\nThis program is free software. It comes without any warranty, to the extent permitted by applicable law. You can redistribute it and/or modify it under the terms of the MIT LICENSE, as published by Andrew Garcia. See LICENSE below for more details.\n\n**[MIT license](./LICENSE)** Copyright 2022 © <a href="https://github.com/andrewrgarcia" target="_blank">Andrew Garcia</a>.\n',
     'author': 'andrewrgarcia',
     'author_email': 'garcia.gtr@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['voxelmap']
 package_data = \ {'': ['*']} install_requires = \ ['colorcet>=3.0.1,<4.0.0',
 'matplotlib>=3.6.2,<4.0.0', 'numpy>=1.24.1,<2.0.0', 'opencv-
 python>=4.7.0.68,<5.0.0.0', 'pandas>=1.5.2,<2.0.0', 'pytest>=7.2.0,<8.0.0',
 'pyvista>=0.38.2,<0.39.0', 'scikit-image>=0.19.3,<0.20.0',
 'scipy>=1.10.0,<2.0.0', 'sphinx-rtd-theme>=1.2.0,<2.0.0',
 'sphinx>=6.1.3,<7.0.0'] setup_kwargs = { 'name': 'voxelmap', 'version':
-'3.6.0', 'description': 'A Python library for making voxel and 3D models from
+'3.7.0', 'description': 'A Python library for making voxel and 3D models from
 NumPy arrays.', 'long_description': '# voxelmap\n\n[![License](http://
 img.shields.io/:license-mit-blue.svg?style=flat-square)](https://
 raw.githubusercontent.com/andrewrgarcia/voxelmap/main/LICENSE)\n[!
 [Documentation Status](https://readthedocs.org/projects/voxelmap/badge/
 ?version=latest)](https://voxelmap.readthedocs.io/en/latest/?badge=latest)\n\nA
 Python library for making voxel and three-dimensional models from NumPy arrays.
 \n\n\n[https://github.com/andrewrgarcia/voxelmap/blob/main/
```

### Comparing `voxelmap-3.6.0/PKG-INFO` & `voxelmap-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelmap
-Version: 3.6.0
+Version: 3.7.0
 Summary: A Python library for making voxel and 3D models from NumPy arrays.
 License: MIT
 Author: andrewrgarcia
 Author-email: garcia.gtr@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: voxelmap Version: 3.6.0 Summary: A Python library
+Metadata-Version: 2.1 Name: voxelmap Version: 3.7.0 Summary: A Python library
 for making voxel and 3D models from NumPy arrays. License: MIT Author:
 andrewrgarcia Author-email: garcia.gtr@gmail.com Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorcet (>=3.0.1,<4.0.0) Requires-Dist: matplotlib
```

