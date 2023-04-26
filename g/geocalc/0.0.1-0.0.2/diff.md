# Comparing `tmp/geocalc-0.0.1.tar.gz` & `tmp/geocalc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocalc-0.0.1.tar", last modified: Wed Apr 26 15:11:08 2023, max compression
+gzip compressed data, was "geocalc-0.0.2.tar", last modified: Wed Apr 26 15:15:53 2023, max compression
```

## Comparing `geocalc-0.0.1.tar` & `geocalc-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:11:08.863374 geocalc-0.0.1/
--rw-r--r--   0 mac        (501) admin       (80)     1071 2023-04-25 19:55:11.000000 geocalc-0.0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) admin       (80)    12453 2023-04-26 15:11:08.863222 geocalc-0.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)    10068 2023-04-25 19:09:41.000000 geocalc-0.0.1/README.md
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:11:08.863014 geocalc-0.0.1/geocalc.egg-info/
--rw-r--r--   0 mac        (501) admin       (80)    12453 2023-04-26 15:11:08.000000 geocalc-0.0.1/geocalc.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)      199 2023-04-26 15:11:08.000000 geocalc-0.0.1/geocalc.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:11:08.000000 geocalc-0.0.1/geocalc.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) admin       (80)       24 2023-04-26 15:11:08.000000 geocalc-0.0.1/geocalc.egg-info/requires.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:11:08.000000 geocalc-0.0.1/geocalc.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) admin       (80)     1373 2023-04-26 15:10:55.000000 geocalc-0.0.1/pyproject.toml
--rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-26 15:11:08.863417 geocalc-0.0.1/setup.cfg
--rw-r--r--   0 mac        (501) admin       (80)     1998 2023-04-26 15:10:52.000000 geocalc-0.0.1/setup.py
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:15:53.365402 geocalc-0.0.2/
+-rw-r--r--   0 mac        (501) admin       (80)     1071 2023-04-25 19:55:11.000000 geocalc-0.0.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) admin       (80)    12465 2023-04-26 15:15:53.365241 geocalc-0.0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)    10080 2023-04-26 15:15:02.000000 geocalc-0.0.2/README.md
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:15:53.365056 geocalc-0.0.2/geocalc.egg-info/
+-rw-r--r--   0 mac        (501) admin       (80)    12465 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)      199 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) admin       (80)       24 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) admin       (80)     1373 2023-04-26 15:15:28.000000 geocalc-0.0.2/pyproject.toml
+-rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-26 15:15:53.365442 geocalc-0.0.2/setup.cfg
+-rw-r--r--   0 mac        (501) admin       (80)     1998 2023-04-26 15:10:52.000000 geocalc-0.0.2/setup.py
```

### Comparing `geocalc-0.0.1/LICENSE.txt` & `geocalc-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geocalc-0.0.1/PKG-INFO` & `geocalc-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocalc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for geometric calculations
 Author: Charles Gameti
 Author-email: Charles Gameti <gameticharles@gmail.com>
 Maintainer-email: Charles Gameti <gameticharles@gmail.com>, "Fiifi O. Turkson" <fiiturkson@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Charles Gameti
@@ -41,41 +41,41 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Geomat
+# GeoCalc
 
-Geomat is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
+GeoCalc is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
 
 ## Features
 
 - Compute various curve parameters for horizontal curves (Simple, Circular, and Spiral) and Vertical Curves. Calculate the Point of Intersection (PI), Point of Curvature (PC), and Point of Tangency (PT). Calculate chainages and convert between meters and chainage strings. Support for both metric and imperial units
 - Angle computations and conversions, including degree-minute-second (DMS) and decimal degrees
 - Triangle calculations including area, perimeter, and angles
 - Polygon calculations including area and perimeter
 - Levelling calculations for elevation and height differences
 - Geodesy calculations for distance and bearing
 
 ## Installation
 
-You can install Geomat using pip:
+You can install GeoCalc using pip:
 
 ```bash
-pip install geomat
+pip install geocalc
 ```
 
 ## Usage
 
 # Horizontal Curves
 
 ```python
-from geomat import HorizontalCurve, CircularCurves, SpiralCurves
+from geocalc import HorizontalCurve, CircularCurves, SpiralCurves
 
 # Create a circular curve
 
 curve = CircularCurve(radius=400, central_angle=24.533333)
 starting_chainage = 4545.500
 interval = 20
 print(curve)
@@ -105,15 +105,15 @@
 
 spiral_degree_of_curve = spiral_curve.spiral_degree_of_curve(Ls=20)
 ```
 
 # Vertical Curves
 
 ```python
-from geomat import VerticalCurve
+from geocalc import VerticalCurve
 
 # Create a vertical curve
 
 vertical_curve = VerticalCurve(PVI_elevation=100, grade_in=2, grade_out=-3, length=200)
 
 # Calculate curve parameters
 
@@ -121,15 +121,15 @@
 ```
 
 # Angles
 
 ```python
 # Example usage
 
-from geomat import Angle
+from geocalc import Angle
 
 angle_deg = Angle(45, 'deg')
 print("DMS:", angle_deg.dms)
 print("Degrees:", angle_deg.deg)
 print("Radians:", angle_deg.rad)
 print("Grads:", angle_deg.grad)
 
@@ -172,15 +172,15 @@
 ```
 
 # Triangle
 
 ## Example usage
 
 ```python
-from geomat import Triangle
+from geocalc import Triangle
 
 triangle = Triangle(a=3, b=4, c=5, A=(0, 0), B=(3, 0))
 vertex_c1, vertex_c2 = triangle.calculate_other_coordinates()
 
 print("Possible third vertex coordinates:", vertex_c1, vertex_c2)
 ```
 
@@ -213,15 +213,15 @@
 # Trigonometric formula
 print("Trigonometric formula:", triangle.trigonometric())
 ```
 
 # Polygon
 
 ```python
-from geomat import Polygon
+from geocalc import Polygon
 
 #Create a polygon with coordinates
 vertices = [(1613.26, 2418.11), (1806.71, 2523.16), (1942.17, 2366.84), (1901.89, 2203.18), (1652.08, 2259.26)]
 
 polygon = Polygon(vertices)
 print("Shoelace formula: ", polygon.shoelace())
 print("Triangulation: ", polygon.triangulation())
@@ -276,15 +276,15 @@
 print("Side length from circumradius:", polygon.get_side_length(circumradius=circumradius))
 print("Side length from inradius:", polygon.get_side_length(inradius=inradius))
 ```
 
 # Levelling
 
 ```python
-from geomat import Levelling
+from geocalc import Levelling
 
 starting_tbm = 100.000
 closing_tbm = 98.050
 data =  [
     ('A', 1.751, None, None),  
     ('B', None, 0.540, None),
     ('C', 0.300, None, 2.100),
@@ -344,15 +344,15 @@
 print("Rise & Fall:\n",leveling.get_dataFrame(roundDigits=5))
 
 ```
 
 # Geodesy
 
 ```python
-from geomat import Geodesy
+from geocalc import Geodesy
 
 # Calculate distance and bearing between two points
 point_a = (12.4924, 41.8902)  # Colosseum, Rome
 point_b = (2.2945, 48.8582)   # Eiffel Tower, Paris
 
 distance, bearing = Geodesy.distance_and_bearing(point_a, point_b)
 ```
@@ -372,12 +372,12 @@
 polygon_coordinates = [(30, 0), (30, 10), (40, 10), (40, 0)]
 area = geodesy.area_of_geodesic_polygon(polygon_coordinates)
 print(f"Area of geodesic polygon: {area} square meters")
 ```
 
 ## Contributing
 
-If you'd like to contribute to Geomat, please open an issue or submit a pull request on the GitHub repository.
+If you'd like to contribute to GeoCalc, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `geocalc-0.0.1/README.md` & `geocalc-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Geomat
+# GeoCalc
 
-Geomat is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
+GeoCalc is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
 
 ## Features
 
 - Compute various curve parameters for horizontal curves (Simple, Circular, and Spiral) and Vertical Curves. Calculate the Point of Intersection (PI), Point of Curvature (PC), and Point of Tangency (PT). Calculate chainages and convert between meters and chainage strings. Support for both metric and imperial units
 - Angle computations and conversions, including degree-minute-second (DMS) and decimal degrees
 - Triangle calculations including area, perimeter, and angles
 - Polygon calculations including area and perimeter
 - Levelling calculations for elevation and height differences
 - Geodesy calculations for distance and bearing
 
 ## Installation
 
-You can install Geomat using pip:
+You can install GeoCalc using pip:
 
 ```bash
-pip install geomat
+pip install geocalc
 ```
 
 ## Usage
 
 # Horizontal Curves
 
 ```python
-from geomat import HorizontalCurve, CircularCurves, SpiralCurves
+from geocalc import HorizontalCurve, CircularCurves, SpiralCurves
 
 # Create a circular curve
 
 curve = CircularCurve(radius=400, central_angle=24.533333)
 starting_chainage = 4545.500
 interval = 20
 print(curve)
@@ -58,15 +58,15 @@
 
 spiral_degree_of_curve = spiral_curve.spiral_degree_of_curve(Ls=20)
 ```
 
 # Vertical Curves
 
 ```python
-from geomat import VerticalCurve
+from geocalc import VerticalCurve
 
 # Create a vertical curve
 
 vertical_curve = VerticalCurve(PVI_elevation=100, grade_in=2, grade_out=-3, length=200)
 
 # Calculate curve parameters
 
@@ -74,15 +74,15 @@
 ```
 
 # Angles
 
 ```python
 # Example usage
 
-from geomat import Angle
+from geocalc import Angle
 
 angle_deg = Angle(45, 'deg')
 print("DMS:", angle_deg.dms)
 print("Degrees:", angle_deg.deg)
 print("Radians:", angle_deg.rad)
 print("Grads:", angle_deg.grad)
 
@@ -125,15 +125,15 @@
 ```
 
 # Triangle
 
 ## Example usage
 
 ```python
-from geomat import Triangle
+from geocalc import Triangle
 
 triangle = Triangle(a=3, b=4, c=5, A=(0, 0), B=(3, 0))
 vertex_c1, vertex_c2 = triangle.calculate_other_coordinates()
 
 print("Possible third vertex coordinates:", vertex_c1, vertex_c2)
 ```
 
@@ -166,15 +166,15 @@
 # Trigonometric formula
 print("Trigonometric formula:", triangle.trigonometric())
 ```
 
 # Polygon
 
 ```python
-from geomat import Polygon
+from geocalc import Polygon
 
 #Create a polygon with coordinates
 vertices = [(1613.26, 2418.11), (1806.71, 2523.16), (1942.17, 2366.84), (1901.89, 2203.18), (1652.08, 2259.26)]
 
 polygon = Polygon(vertices)
 print("Shoelace formula: ", polygon.shoelace())
 print("Triangulation: ", polygon.triangulation())
@@ -229,15 +229,15 @@
 print("Side length from circumradius:", polygon.get_side_length(circumradius=circumradius))
 print("Side length from inradius:", polygon.get_side_length(inradius=inradius))
 ```
 
 # Levelling
 
 ```python
-from geomat import Levelling
+from geocalc import Levelling
 
 starting_tbm = 100.000
 closing_tbm = 98.050
 data =  [
     ('A', 1.751, None, None),  
     ('B', None, 0.540, None),
     ('C', 0.300, None, 2.100),
@@ -297,15 +297,15 @@
 print("Rise & Fall:\n",leveling.get_dataFrame(roundDigits=5))
 
 ```
 
 # Geodesy
 
 ```python
-from geomat import Geodesy
+from geocalc import Geodesy
 
 # Calculate distance and bearing between two points
 point_a = (12.4924, 41.8902)  # Colosseum, Rome
 point_b = (2.2945, 48.8582)   # Eiffel Tower, Paris
 
 distance, bearing = Geodesy.distance_and_bearing(point_a, point_b)
 ```
@@ -325,12 +325,12 @@
 polygon_coordinates = [(30, 0), (30, 10), (40, 10), (40, 0)]
 area = geodesy.area_of_geodesic_polygon(polygon_coordinates)
 print(f"Area of geodesic polygon: {area} square meters")
 ```
 
 ## Contributing
 
-If you'd like to contribute to Geomat, please open an issue or submit a pull request on the GitHub repository.
+If you'd like to contribute to GeoCalc, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `geocalc-0.0.1/geocalc.egg-info/PKG-INFO` & `geocalc-0.0.2/geocalc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocalc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for geometric calculations
 Author: Charles Gameti
 Author-email: Charles Gameti <gameticharles@gmail.com>
 Maintainer-email: Charles Gameti <gameticharles@gmail.com>, "Fiifi O. Turkson" <fiiturkson@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Charles Gameti
@@ -41,41 +41,41 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Geomat
+# GeoCalc
 
-Geomat is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
+GeoCalc is a Python library for geometric calculations, focusing on horizontal and vertical curves, angles, triangles, polygons, leveling, and geodesy in transportation engineering and surveying. The library provides various classes and functions for computing and setting out curves, angles, and more.
 
 ## Features
 
 - Compute various curve parameters for horizontal curves (Simple, Circular, and Spiral) and Vertical Curves. Calculate the Point of Intersection (PI), Point of Curvature (PC), and Point of Tangency (PT). Calculate chainages and convert between meters and chainage strings. Support for both metric and imperial units
 - Angle computations and conversions, including degree-minute-second (DMS) and decimal degrees
 - Triangle calculations including area, perimeter, and angles
 - Polygon calculations including area and perimeter
 - Levelling calculations for elevation and height differences
 - Geodesy calculations for distance and bearing
 
 ## Installation
 
-You can install Geomat using pip:
+You can install GeoCalc using pip:
 
 ```bash
-pip install geomat
+pip install geocalc
 ```
 
 ## Usage
 
 # Horizontal Curves
 
 ```python
-from geomat import HorizontalCurve, CircularCurves, SpiralCurves
+from geocalc import HorizontalCurve, CircularCurves, SpiralCurves
 
 # Create a circular curve
 
 curve = CircularCurve(radius=400, central_angle=24.533333)
 starting_chainage = 4545.500
 interval = 20
 print(curve)
@@ -105,15 +105,15 @@
 
 spiral_degree_of_curve = spiral_curve.spiral_degree_of_curve(Ls=20)
 ```
 
 # Vertical Curves
 
 ```python
-from geomat import VerticalCurve
+from geocalc import VerticalCurve
 
 # Create a vertical curve
 
 vertical_curve = VerticalCurve(PVI_elevation=100, grade_in=2, grade_out=-3, length=200)
 
 # Calculate curve parameters
 
@@ -121,15 +121,15 @@
 ```
 
 # Angles
 
 ```python
 # Example usage
 
-from geomat import Angle
+from geocalc import Angle
 
 angle_deg = Angle(45, 'deg')
 print("DMS:", angle_deg.dms)
 print("Degrees:", angle_deg.deg)
 print("Radians:", angle_deg.rad)
 print("Grads:", angle_deg.grad)
 
@@ -172,15 +172,15 @@
 ```
 
 # Triangle
 
 ## Example usage
 
 ```python
-from geomat import Triangle
+from geocalc import Triangle
 
 triangle = Triangle(a=3, b=4, c=5, A=(0, 0), B=(3, 0))
 vertex_c1, vertex_c2 = triangle.calculate_other_coordinates()
 
 print("Possible third vertex coordinates:", vertex_c1, vertex_c2)
 ```
 
@@ -213,15 +213,15 @@
 # Trigonometric formula
 print("Trigonometric formula:", triangle.trigonometric())
 ```
 
 # Polygon
 
 ```python
-from geomat import Polygon
+from geocalc import Polygon
 
 #Create a polygon with coordinates
 vertices = [(1613.26, 2418.11), (1806.71, 2523.16), (1942.17, 2366.84), (1901.89, 2203.18), (1652.08, 2259.26)]
 
 polygon = Polygon(vertices)
 print("Shoelace formula: ", polygon.shoelace())
 print("Triangulation: ", polygon.triangulation())
@@ -276,15 +276,15 @@
 print("Side length from circumradius:", polygon.get_side_length(circumradius=circumradius))
 print("Side length from inradius:", polygon.get_side_length(inradius=inradius))
 ```
 
 # Levelling
 
 ```python
-from geomat import Levelling
+from geocalc import Levelling
 
 starting_tbm = 100.000
 closing_tbm = 98.050
 data =  [
     ('A', 1.751, None, None),  
     ('B', None, 0.540, None),
     ('C', 0.300, None, 2.100),
@@ -344,15 +344,15 @@
 print("Rise & Fall:\n",leveling.get_dataFrame(roundDigits=5))
 
 ```
 
 # Geodesy
 
 ```python
-from geomat import Geodesy
+from geocalc import Geodesy
 
 # Calculate distance and bearing between two points
 point_a = (12.4924, 41.8902)  # Colosseum, Rome
 point_b = (2.2945, 48.8582)   # Eiffel Tower, Paris
 
 distance, bearing = Geodesy.distance_and_bearing(point_a, point_b)
 ```
@@ -372,12 +372,12 @@
 polygon_coordinates = [(30, 0), (30, 10), (40, 10), (40, 0)]
 area = geodesy.area_of_geodesic_polygon(polygon_coordinates)
 print(f"Area of geodesic polygon: {area} square meters")
 ```
 
 ## Contributing
 
-If you'd like to contribute to Geomat, please open an issue or submit a pull request on the GitHub repository.
+If you'd like to contribute to GeoCalc, please open an issue or submit a pull request on the GitHub repository.
 
 ## License
 
 This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `geocalc-0.0.1/pyproject.toml` & `geocalc-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geocalc"
-version = "0.0.1"
+version = "0.0.2"
 license = {file = "LICENSE.txt"}
 keywords = ["python", "geomatic", "levelling", "curves", "geodesy", "polygon", "triangle", "horizontal", "vertical"]
 authors = [
   { name="Charles Gameti", email="gameticharles@gmail.com" },
 ]
 description = "A library for geometric calculations"
 readme = "README.md"
```

### Comparing `geocalc-0.0.1/setup.py` & `geocalc-0.0.2/setup.py`

 * *Files identical despite different names*

