# Comparing `tmp/segment-geospatial-0.2.0.tar.gz` & `tmp/segment-geospatial-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.2.0.tar", last modified: Fri Apr 21 13:57:28 2023, max compression
+gzip compressed data, was "segment-geospatial-0.3.0.tar", last modified: Wed Apr 26 15:21:47 2023, max compression
```

## Comparing `segment-geospatial-0.2.0.tar` & `segment-geospatial-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22613 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 13:57:28.000000 segment-geospatial-0.2.0/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-21 13:57:28.709675 segment-geospatial-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-21 13:57:17.000000 segment-geospatial-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29015 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 15:21:47.000000 segment-geospatial-0.3.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-26 15:21:47.364898 segment-geospatial-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-26 15:21:30.000000 segment-geospatial-0.3.0/setup.py
```

### Comparing `segment-geospatial-0.2.0/LICENSE` & `segment-geospatial-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.2.0/PKG-INFO` & `segment-geospatial-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.2.0
+Version: 0.3.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,19 @@
 -   Free software: MIT license
 -   Documentation: https://samgeo.gishub.org
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+
+## Examples
+
+- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.2.0/README.md` & `segment-geospatial-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 -   Free software: MIT license
 -   Documentation: https://samgeo.gishub.org
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+
+## Examples
+
+- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.2.0/samgeo/common.py` & `segment-geospatial-0.3.0/samgeo/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -114,14 +114,15 @@
         overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
         subfolder (bool, optional): Create a subfolder with the same name as the file. Defaults to False.
 
     Returns:
         str: The output file path.
     """
     import zipfile
+
     try:
         import gdown
     except ImportError:
         print(
             "The gdown package is required for this function. Use `pip install gdown` to install it."
         )
         return
@@ -167,15 +168,15 @@
     return os.path.abspath(output)
 
 
 def download_checkpoint(url=None, output=None, overwrite=False, **kwargs):
     """Download a checkpoint from URL. It can be one of the following: sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth.
 
     Args:
-        url (str, optional): The checkpoint URL. Defaults to None. 
+        url (str, optional): The checkpoint URL. Defaults to None.
         output (str, optional): The output file path. Defaults to None.
         overwrite (bool, optional): Overwrite the file if it already exists. Defaults to False.
 
     Returns:
         str: The output file path.
     """
     checkpoints = {
@@ -189,15 +190,15 @@
 
     if url is None:
         url = checkpoints['sam_vit_h_4b8939.pth']
 
     if output is None:
         output = os.path.basename(url)
 
-    return download_file(url, output,overwrite=overwrite, **kwargs)
+    return download_file(url, output, overwrite=overwrite, **kwargs)
 
 
 def image_to_cog(source, dst_path=None, profile="deflate", **kwargs):
     """Converts an image to a COG file.
 
     Args:
         source (str): A dataset path, URL or rasterio.io.DatasetReader object.
@@ -231,20 +232,78 @@
 
     dst_path = check_file_path(dst_path)
 
     dst_profile = cog_profiles.get(profile)
     cog_translate(source, dst_path, dst_profile, **kwargs)
 
 
+def reproject(
+    image, output, dst_crs="EPSG:4326", resampling="nearest", to_cog=True, **kwargs
+):
+    """Reprojects an image.
+
+    Args:
+        image (str): The input image filepath.
+        output (str): The output image filepath.
+        dst_crs (str, optional): The destination CRS. Defaults to "EPSG:4326".
+        resampling (Resampling, optional): The resampling method. Defaults to "nearest".
+        to_cog (bool, optional): Whether to convert the output image to a Cloud Optimized GeoTIFF. Defaults to True.
+        **kwargs: Additional keyword arguments to pass to rasterio.open.
+
+    """
+    import rasterio as rio
+    from rasterio.warp import calculate_default_transform, reproject, Resampling
+
+    if isinstance(resampling, str):
+        resampling = getattr(Resampling, resampling)
+
+    image = os.path.abspath(image)
+    output = os.path.abspath(output)
+
+    if not os.path.exists(os.path.dirname(output)):
+        os.makedirs(os.path.dirname(output))
+
+    with rio.open(image, **kwargs) as src:
+        transform, width, height = calculate_default_transform(
+            src.crs, dst_crs, src.width, src.height, *src.bounds
+        )
+        kwargs = src.meta.copy()
+        kwargs.update(
+            {
+                "crs": dst_crs,
+                "transform": transform,
+                "width": width,
+                "height": height,
+            }
+        )
+
+        with rio.open(output, "w", **kwargs) as dst:
+            for i in range(1, src.count + 1):
+                reproject(
+                    source=rio.band(src, i),
+                    destination=rio.band(dst, i),
+                    src_transform=src.transform,
+                    src_crs=src.crs,
+                    dst_transform=transform,
+                    dst_crs=dst_crs,
+                    resampling=resampling,
+                    **kwargs,
+                )
+
+    if to_cog:
+        image_to_cog(output, output)
+
+
 def tms_to_geotiff(
     output,
     bbox,
     zoom=None,
     resolution=None,
     source="OpenStreetMap",
+    crs="EPSG:3857",
     to_cog=False,
     return_image=False,
     overwrite=False,
     quiet=False,
     **kwargs,
 ):
     """Download TMS tiles and convert them to a GeoTIFF. The source is adapted from https://github.com/gumblex/tms2geotiff.
@@ -253,14 +312,15 @@
     Args:
         output (str): The output GeoTIFF file.
         bbox (list): The bounding box [minx, miny, maxx, maxy], e.g., [-122.5216, 37.733, -122.3661, 37.8095]
         zoom (int, optional): The map zoom level. Defaults to None.
         resolution (float, optional): The resolution in meters. Defaults to None.
         source (str, optional): The tile source. It can be one of the following: "OPENSTREETMAP", "ROADMAP",
             "SATELLITE", "TERRAIN", "HYBRID", or an HTTP URL. Defaults to "OpenStreetMap".
+        crs (str, optional): The output CRS. Defaults to "EPSG:3857".
         to_cog (bool, optional): Convert to Cloud Optimized GeoTIFF. Defaults to False.
         return_image (bool, optional): Return the image as PIL.Image. Defaults to False.
         overwrite (bool, optional): Overwrite the output file if it already exists. Defaults to False.
         quiet (bool, optional): Suppress output. Defaults to False.
         **kwargs: Additional arguments to pass to gdal.GetDriverByName("GTiff").Create().
 
     """
@@ -285,49 +345,36 @@
         SESSION = httpx.Client()
     except ImportError:
         import requests
 
         SESSION = requests.Session()
 
     if not overwrite and os.path.exists(output):
-        print(f"The output file {output} already exists. Use `overwrite=True` to overwrite it.")
+        print(
+            f"The output file {output} already exists. Use `overwrite=True` to overwrite it."
+        )
         return
 
     xyz_tiles = {
-        "OPENSTREETMAP": {
-            "url": "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
-            "attribution": "OpenStreetMap",
-            "name": "OpenStreetMap",
-        },
-        "ROADMAP": {
-            "url": "https://mt1.google.com/vt/lyrs=m&x={x}&y={y}&z={z}",
-            "attribution": "Google",
-            "name": "Google Maps",
-        },
-        "SATELLITE": {
-            "url": "https://mt1.google.com/vt/lyrs=s&x={x}&y={y}&z={z}",
-            "attribution": "Google",
-            "name": "Google Satellite",
-        },
-        "TERRAIN": {
-            "url": "https://mt1.google.com/vt/lyrs=p&x={x}&y={y}&z={z}",
-            "attribution": "Google",
-            "name": "Google Terrain",
-        },
-        "HYBRID": {
-            "url": "https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}",
-            "attribution": "Google",
-            "name": "Google Satellite",
-        },
+        "OPENSTREETMAP": "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
+        "ROADMAP": "https://mt1.google.com/vt/lyrs=m&x={x}&y={y}&z={z}",
+        "SATELLITE": "https://mt1.google.com/vt/lyrs=s&x={x}&y={y}&z={z}",
+        "TERRAIN": "https://mt1.google.com/vt/lyrs=p&x={x}&y={y}&z={z}",
+        "HYBRID": "https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}",
     }
 
-    if isinstance(source, str) and source.upper() in xyz_tiles:
-        source = xyz_tiles[source.upper()]["url"]
-    elif isinstance(source, str) and source.startswith("http"):
-        pass
+    basemaps = get_basemaps()
+
+    if isinstance(source, str):
+        if source.upper() in xyz_tiles:
+            source = xyz_tiles[source.upper()]
+        elif source in basemaps:
+            source = basemaps[source]
+        elif source.startswith("http"):
+            pass
     else:
         raise ValueError(
             'source must be one of "OpenStreetMap", "ROADMAP", "SATELLITE", "TERRAIN", "HYBRID", or a URL'
         )
 
     def resolution_to_zoom_level(resolution):
         """
@@ -521,15 +568,17 @@
 
     try:
         image = draw_tile(
             source, south, west, north, east, zoom, output, quiet, **kwargs
         )
         if return_image:
             return image
-        if to_cog:
+        if crs.upper() != "EPSG:3857":
+            reproject(output, output, crs, to_cog=to_cog)
+        elif to_cog:
             image_to_cog(output, output)
     except Exception as e:
         raise Exception(e)
 
 
 def chw_to_hwc(block):
     # Grab first 3 channels
@@ -702,7 +751,152 @@
         source=source,
         to_cog=False,
         return_image=True,
         quiet=False,
         **kwargs,
     )
     return image
+
+
+def tiff_to_vector(tiff_path, output, simplify_tolerance=None, **kwargs):
+    """Convert a tiff file to a gpkg file.
+
+    Args:
+        tiff_path (str): The path to the tiff file.
+        output (str): The path to the vector file.
+        simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+            The higher this value, the smaller the number of vertices in the resulting geometry.
+    """
+
+    with rasterio.open(tiff_path) as src:
+        band = src.read()
+
+        mask = band != 0
+        shapes = features.shapes(band, mask=mask, transform=src.transform)
+
+    fc = [
+        {"geometry": shapely.geometry.shape(shape), "properties": {"value": value}}
+        for shape, value in shapes
+    ]
+    if simplify_tolerance is not None:
+        for i in fc:
+            i["geometry"] = i["geometry"].simplify(tolerance=simplify_tolerance)
+
+    gdf = gpd.GeoDataFrame.from_features(fc)
+    if src.crs is not None:
+        gdf.set_crs(crs=src.crs, inplace=True)
+    gdf.to_file(output, **kwargs)
+
+
+def tiff_to_gpkg(tiff_path, output, simplify_tolerance=None, **kwargs):
+    """Convert a tiff file to a gpkg file.
+
+    Args:
+        tiff_path (str): The path to the tiff file.
+        output (str): The path to the gpkg file.
+        simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+            The higher this value, the smaller the number of vertices in the resulting geometry.
+    """
+
+    if not output.endswith(".gpkg"):
+        output += ".gpkg"
+
+    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+
+
+def tiff_to_shp(tiff_path, output, simplify_tolerance=None, **kwargs):
+    """Convert a tiff file to a shapefile.
+
+    Args:
+        tiff_path (str): The path to the tiff file.
+        output (str): The path to the shapefile.
+        simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+            The higher this value, the smaller the number of vertices in the resulting geometry.
+    """
+
+    if not output.endswith(".shp"):
+        output += ".shp"
+
+    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+
+
+def tiff_to_geojson(tiff_path, output, simplify_tolerance=None, **kwargs):
+    """Convert a tiff file to a GeoJSON file.
+
+    Args:
+        tiff_path (str): The path to the tiff file.
+        output (str): The path to the GeoJSON file.
+        simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+            The higher this value, the smaller the number of vertices in the resulting geometry.
+    """
+
+    if not output.endswith(".geojson"):
+        output += ".geojson"
+
+    tiff_to_vector(tiff_path, output, simplify_tolerance=simplify_tolerance, **kwargs)
+
+
+def get_xyz_dict(free_only=True):
+    """Returns a dictionary of xyz services.
+
+    Args:
+        free_only (bool, optional): Whether to return only free xyz tile services that do not require an access token. Defaults to True.
+
+    Returns:
+        dict: A dictionary of xyz services.
+    """
+    import collections
+    import xyzservices.providers as xyz
+
+    def _unpack_sub_parameters(var, param):
+        temp = var
+        for sub_param in param.split("."):
+            temp = getattr(temp, sub_param)
+        return temp
+
+    xyz_dict = {}
+    for item in xyz.values():
+        try:
+            name = item["name"]
+            tile = _unpack_sub_parameters(xyz, name)
+            if _unpack_sub_parameters(xyz, name).requires_token():
+                if free_only:
+                    pass
+                else:
+                    xyz_dict[name] = tile
+            else:
+                xyz_dict[name] = tile
+
+        except Exception:
+            for sub_item in item:
+                name = item[sub_item]["name"]
+                tile = _unpack_sub_parameters(xyz, name)
+                if _unpack_sub_parameters(xyz, name).requires_token():
+                    if free_only:
+                        pass
+                    else:
+                        xyz_dict[name] = tile
+                else:
+                    xyz_dict[name] = tile
+
+    xyz_dict = collections.OrderedDict(sorted(xyz_dict.items()))
+    return xyz_dict
+
+
+def get_basemaps(free_only=True):
+    """Returns a dictionary of xyz basemaps.
+
+    Args:
+        free_only (bool, optional): Whether to return only free xyz tile services that do not require an access token. Defaults to True.
+
+    Returns:
+        dict: A dictionary of xyz basemaps.
+    """
+
+    basemaps = {}
+    xyz_dict = get_xyz_dict(free_only=free_only)
+    for item in xyz_dict:
+        name = xyz_dict[item].name
+        url = xyz_dict[item].build_url()
+        basemaps[name] = url
+
+    return basemaps
```

### Comparing `segment-geospatial-0.2.0/samgeo/samgeo.py` & `segment-geospatial-0.3.0/samgeo/samgeo.py`

 * *Files 27% similar despite different names*

```diff
@@ -28,43 +28,42 @@
 # crop_n_points_downscale_factor: int = 1,
 # point_grids: Optional[List[np.ndarray]] = None,
 # min_mask_region_area: int = 0,
 # output_mode: str = "binary_mask",
 
 
 class SamGeo:
-    """The main class for segmenting geospatial data with the Segment Anything Model (SAM). See 
-        https://github.com/facebookresearch/segment-anything
+    """The main class for segmenting geospatial data with the Segment Anything Model (SAM). See
+    https://github.com/facebookresearch/segment-anything
     """
 
     def __init__(
         self,
         checkpoint="sam_vit_h_4b8939.pth",
         model_type='vit_h',
         device='cpu',
         erosion_kernel=(3, 3),
         mask_multiplier=255,
         sam_kwargs=None,
     ):
-        """Initialize the class. 
+        """Initialize the class.
 
         Args:
             checkpoint (str, optional): The path to the checkpoint. It can be one of the following:
                 sam_vit_h_4b8939.pth, sam_vit_l_0b3195.pth, sam_vit_b_01ec64.pth. Defaults to "sam_vit_h_4b8939.pth".
             model_type (str, optional): The model type. It can be one of the following: vit_h, vit_l, vit_l. Defaults to 'vit_h'.
             device (str, optional): The device to use. It can be one of the following: cpu, cuda. Defaults to 'cpu'.
             erosion_kernel (tuple, optional): The erosion kernel. Defaults to (3, 3).
             mask_multiplier (int, optional): The mask multiplier. Defaults to 255.
             sam_kwargs (_type_, optional): The arguments for the SAM model. Defaults to None.
-        """        
+        """
         if not os.path.exists(checkpoint):
             print(f'Checkpoint {checkpoint} does not exist.')
             download_checkpoint(output=checkpoint)
 
-
         self.checkpoint = checkpoint
         self.model_type = model_type
         self.device = device
         self.sam_kwargs = sam_kwargs
         self.reinit_sam()
 
         self.erosion_kernel = erosion_kernel
@@ -115,61 +114,54 @@
     def image_to_image(self, image, **kwargs):
         return image_to_image(image, self, **kwargs)
 
     def download_tms_as_tiff(self, source, pt1, pt2, zoom, dist):
         image = draw_tile(source, pt1[0], pt1[1], pt2[0], pt2[1], zoom, dist)
         return image
 
-    def tiff_to_gpkg(self, tiff_path, gpkg_path, simplify_tolerance=None, **kwargs):
+    def tiff_to_vector(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a gpkg file.
 
         Args:
             tiff_path (str): The path to the tiff file.
-            gpkg_path (str): The path to the gpkg file.
-            simplify_tolerance (_type_, optional): The simplify tolerance. Defaults to None.
+            output (str): The path to the vector file.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
         """
-    
-        with rasterio.open(tiff_path) as src:
-            band = src.read()
-
-            mask = band != 0
-            shapes = features.shapes(band, mask=mask, transform=src.transform)
-
-        fc = [
-            {"geometry": shapely.geometry.shape(shape), "properties": {"value": value}}
-            for shape, value in shapes
-        ]
-        if simplify_tolerance is not None:
-            for i in fc:
-                i["geometry"] = i["geometry"].simplify(tolerance=simplify_tolerance)
-
-        gdf = gpd.GeoDataFrame.from_features(fc)
-        gdf.set_crs(epsg=src.crs.to_epsg(), inplace=True)
-        gdf.to_file(gpkg_path, driver='GPKG', **kwargs)
 
+        tiff_to_vector(tiff_path, output, simplify_tolerance=None, **kwargs)
 
-    def tiff_to_vector(self, tiff_path, output, simplify_tolerance=None, **kwargs):
+    def tiff_to_gpkg(self, tiff_path, output, simplify_tolerance=None, **kwargs):
         """Convert a tiff file to a gpkg file.
 
         Args:
             tiff_path (str): The path to the tiff file.
-            output (str): The path to the vector file.
-            simplify_tolerance (_type_, optional): The simplify tolerance. Defaults to None.
+            output (str): The path to the gpkg file.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
         """
-    
-        with rasterio.open(tiff_path) as src:
-            band = src.read()
-
-            mask = band != 0
-            shapes = features.shapes(band, mask=mask, transform=src.transform)
-
-        fc = [
-            {"geometry": shapely.geometry.shape(shape), "properties": {"value": value}}
-            for shape, value in shapes
-        ]
-        if simplify_tolerance is not None:
-            for i in fc:
-                i["geometry"] = i["geometry"].simplify(tolerance=simplify_tolerance)
-
-        gdf = gpd.GeoDataFrame.from_features(fc)
-        gdf.set_crs(epsg=src.crs.to_epsg(), inplace=True)
-        gdf.to_file(output, **kwargs)
+
+        tiff_to_gpkg(tiff_path, output, simplify_tolerance=None, **kwargs)
+
+    def tiff_to_shp(self, tiff_path, output, simplify_tolerance=None, **kwargs):
+        """Convert a tiff file to a shapefile.
+
+        Args:
+            tiff_path (str): The path to the tiff file.
+            output (str): The path to the shapefile.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
+        """
+
+        tiff_to_shp(tiff_path, output, simplify_tolerance=None, **kwargs)
+
+    def tiff_to_geojson(self, tiff_path, output, simplify_tolerance=None, **kwargs):
+        """Convert a tiff file to a GeoJSON file.
+
+        Args:
+            tiff_path (str): The path to the tiff file.
+            output (str): The path to the GeoJSON file.
+            simplify_tolerance (float, optional): The maximum allowed geometry displacement.
+                The higher this value, the smaller the number of vertices in the resulting geometry.
+        """
+
+        tiff_to_geojson(tiff_path, output, simplify_tolerance=None, **kwargs)
```

### Comparing `segment-geospatial-0.2.0/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.3.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.2.0
+Version: 0.3.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -34,14 +34,19 @@
 -   Free software: MIT license
 -   Documentation: https://samgeo.gishub.org
 
 ## Features
 
 -   Download map tiles from Tile Map Service (TMS) servers and create GeoTIFF files
 -   Segment GeoTIFF files using the Segment Anything Model (SAM)
+-   Save segmentation results as common vector formats (GeoPackage, Shapefile, GeoJSON, etc.)
+
+## Examples
+
+- [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 
 ## Acknowledgements
 
 This package was made possible by the following open source projects. Credit goes to the developers of these projects.
 
 -   [segment-anything](https://github.com/facebookresearch/segment-anything)
 -   [segment-anything-eo](https://github.com/aliaksandr960/segment-anything-eo)
```

### Comparing `segment-geospatial-0.2.0/setup.py` & `segment-geospatial-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='samgeo',
     name='segment-geospatial',
     packages=find_packages(include=['samgeo', 'samgeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/segment-geospatial',
-    version='0.2.0',
+    version='0.3.0',
     zip_safe=False,
 )
```

