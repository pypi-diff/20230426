# Comparing `tmp/geo_api_gouv_fr-0.5.0.tar.gz` & `tmp/geo_api_gouv_fr-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_api_gouv_fr-0.5.0.tar", max compression
+gzip compressed data, was "geo_api_gouv_fr-1.0.0.tar", max compression
```

## Comparing `geo_api_gouv_fr-0.5.0.tar` & `geo_api_gouv_fr-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0      364 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/README.md
--rw-r--r--   0        0        0      214 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/__init__.py
--rw-r--r--   0        0        0       90 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/adress/__init__.py
--rw-r--r--   0        0        0     1803 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/adress/api.py
--rw-r--r--   0        0        0     2343 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/adress/schemas.py
--rw-r--r--   0        0        0       78 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/department/__init__.py
--rw-r--r--   0        0        0      938 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/department/api.py
--rw-r--r--   0        0        0      599 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/department/schemas.py
--rw-r--r--   0        0        0       74 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/region/__init__.py
--rw-r--r--   0        0        0      639 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/region/api.py
--rw-r--r--   0        0        0      367 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/region/schemas.py
--rw-r--r--   0        0        0        0 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/__init__.py
--rw-r--r--   0        0        0      195 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/data/reverse.csv
--rw-r--r--   0        0        0      294 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/data/search.csv
--rw-r--r--   0        0        0     2627 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/test_adresse.py
--rw-r--r--   0        0        0      988 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/test_department.py
--rw-r--r--   0        0        0      751 2023-03-07 09:16:57.490987 geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/test_region.py
--rw-r--r--   0        0        0     1581 2023-03-07 09:17:59.483642 geo_api_gouv_fr-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 geo_api_gouv_fr-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      364 2023-04-26 09:43:22.519370 geo_api_gouv_fr-1.0.0/README.md
+-rw-r--r--   0        0        0      279 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/__init__.py
+-rw-r--r--   0        0        0       90 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/__init__.py
+-rw-r--r--   0        0        0     2768 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/api.py
+-rw-r--r--   0        0        0     4114 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/adress/schemas.py
+-rw-r--r--   0        0        0       75 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/__init__.py
+-rw-r--r--   0        0        0     1544 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/api.py
+-rw-r--r--   0        0        0     1862 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/schemas.py
+-rw-r--r--   0        0        0       78 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/__init__.py
+-rw-r--r--   0        0        0     1268 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/api.py
+-rw-r--r--   0        0        0      962 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/department/schemas.py
+-rw-r--r--   0        0        0       74 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/__init__.py
+-rw-r--r--   0        0        0      864 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/api.py
+-rw-r--r--   0        0        0      552 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/schemas.py
+-rw-r--r--   0        0        0        0 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/data/reverse.csv
+-rw-r--r--   0        0        0      294 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/data/search.csv
+-rw-r--r--   0        0        0     4435 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_adresse.py
+-rw-r--r--   0        0        0     1335 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_commune.py
+-rw-r--r--   0        0        0      982 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_department.py
+-rw-r--r--   0        0        0      751 2023-04-26 09:43:22.523370 geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_region.py
+-rw-r--r--   0        0        0     1636 2023-04-26 10:14:49.091133 geo_api_gouv_fr-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 geo_api_gouv_fr-1.0.0/PKG-INFO
```

### Comparing `geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/adress/schemas.py` & `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/commune/schemas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-from pydantic import BaseModel, validator
-from typing import List, Optional
+from pydantic import BaseModel
+from typing import Optional, List
+from enum import Enum
+
+
+class GeoFormat(Enum):
+    """
+    Attributes:
+        type:
+        fields:
+        format:
+    """
+    json = "json"
+    geojson = "geojson"
+
+
+class CommunesParams(BaseModel):
+    """
+    Attributes:
+        codePostal:
+        lon:
+        lat:
+        nom:
+        boost:
+        code:
+        siren:
+        codeEpci:
+        codeDepartement:
+        codeRegion:
+        zone:
+        type:
+        fields:
+        format:
+        geometry:
+        limit:
 
-
-class SearchParams(BaseModel):
-    q: Optional[str]
-    limit: Optional[int]
-    autocomplete: Optional[int]
-    type: Optional[str]
-    postcode: Optional[int]
-    lat: Optional[float]
+    """
+    codePostal: Optional[str]
     lon: Optional[float]
-
-    @validator('q')
-    def add_smaller_than_200(cls, v):
-        return v[:200]
-
-    @validator('type')
-    def type_must_be_in(cls, v):
-        values = ["housenumber", "street", "locality", "municipality"]
-        if v not in values:
-            raise ValueError(f"Type value must be in {values}")
-        return v
-
-
-class SearchCSVParams(BaseModel):
-    columns: Optional[List[str]]
-    result_columns: Optional[List[str]]
-    postcode: Optional[str] = ""
-    citycode: Optional[str] = ""
-
-
-class ReverseParams(BaseModel):
-    lat: float
-    lon: float
+    lat: Optional[float]
+    nom: Optional[str]
+    boost: Optional[str]
+    code: Optional[str]
+    siren: Optional[str]
+    codeEpci: Optional[str]
+    codeDepartement: Optional[str]
+    codeRegion: Optional[str]
+    zone: Optional[str]
     type: Optional[str]
+    fields: Optional[List[str]]
+    format: Optional[GeoFormat] = GeoFormat.json
+    geometry: Optional[str]
     limit: Optional[int]
 
 
-# results ( everything optional in order to avoid mistakes)
-
-class GpsCoordinate(BaseModel):
-    latitude: float
-    longitude: float
-
-
-class Geometry(BaseModel):
-    type: Optional[str]
-    coordinates: Optional[List]
-
-    @validator('coordinates')
-    def coord_must_have_lat_lon(cls, v):
-
-        if not len(v) == 2:
-            raise ValueError("Coordinates muse have latitude & longitude")
-
-        if v[0] > 180 or v[0] < -180:
-            raise ValueError("Latitude value must be in [-180, 180]")
-
-        if v[1] > 90 or v[1] < -90:
-            raise ValueError("Longitude value must be in [-90, 90]")
-
-        return v
-
-
-class Properties(BaseModel):
-    label: Optional[str]
-    score: Optional[float]
-    housenumber: Optional[str]
-    id: Optional[str]
-    type: Optional[str]
-    name: Optional[str]
-    postcode: Optional[str]
-    citycode: Optional[str]
-    x: Optional[float]
-    y: Optional[float]
-    city: Optional[str]
-    context: Optional[str]
-    importance: Optional[float]
-    street: Optional[str]
-    population: Optional[int]
-
+class CommuneCodeParams(BaseModel):
+    """
+    Attributes:
+        code:
+        limit:
+        fields:
+        format:
+        geometry:
+    """
+    code: Optional[str]
+    fields: Optional[list]
+    geometry: Optional[str]
+    format: Optional[GeoFormat] = GeoFormat.json
+    limit: Optional[int]
 
-class AddressFeature(BaseModel):
-    geometry: Optional[Geometry]
-    properties: Optional[Properties]
 
-    def get_coords(self):
-        return GpsCoordinate(latitude=self.geometry.coordinates[0], longitude=self.geometry.coordinates[1])
+class EpcisCodeParams(CommuneCodeParams):
+    pass
 
 
-class ReverseResponse(BaseModel):
-    type: str
-    version: str
-    features: List[AddressFeature]
+class DepartmentCommuneCodeParams(CommuneCodeParams):
+    pass
 
 
-class SearchResponse(ReverseResponse):
-    pass
+class CommunesResponse(BaseModel):
+    """
+    Attributes:
+        nom:
+        code:
+        codePostaux:
+        codeEpci:
+        codeDepartement:
+        codeRegion:
+        population:
+        _score:
+    """
+    nom: str
+    code: int
+    codePostaux: Optional[List[str]]
+    codeEpci: Optional[str]
+    codeDepartement: Optional[str]
+    codeRegion: Optional[str]
+    population: Optional[str]
+    _score: Optional[float]
```

### Comparing `geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/department/api.py` & `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/region/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import requests
 
 from .schemas import (
-    DepartmentsParams,
-    DepartmentCodeParams,
-    RegionDepartmentCodeParams
+    RegionsParams,
+    RegionCodeParams
 )
 
 
 class Api:
-    """
-    Documentation : https://adresse.data.gouv.fr/api-doc/adresse
+    """ This is the api to interact with the regions
+
+    Documentation : https://geo.api.gouv.fr/decoupage-administratif/regions
+
     """
 
     def __init__(self, **kwargs):
         self.url = kwargs.pop("url", "https://geo.api.gouv.fr")
 
-    def departements(self, **kwargs) -> requests.Response:
-        params = DepartmentsParams(**kwargs)
-        return requests.get(self.url + "/departements", params=params.dict())
-
-    def departements_by_code(self, **kwargs) -> requests.Response:
-        params = DepartmentCodeParams(**kwargs)
-        return requests.get(self.url + "/departements/" + params.code, params=params.dict())
-
-    def departements_by_region(self, **kwargs) -> requests.Response:
-        params = RegionDepartmentCodeParams(**kwargs)
-        return requests.get(self.url + f"/regions/{params.regioncode}/departements", params=params.dict())
+    def regions(self, **kwargs) -> requests.Response:
+        """
+        Parameters:
+            **kwargs (RegionsParams):
+        """
+        params = RegionsParams(**kwargs)
+        return requests.get(self.url + "/regions", params=params.dict())
+
+    def regions_by_code(self, **kwargs) -> requests.Response:
+        """
+        Parameters:
+            **kwargs (RegionCodeParams):
+        """
+        params = RegionCodeParams(**kwargs)
+        return requests.get(self.url + "/regions/" + params.code, params=params.dict())
```

### Comparing `geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/test_department.py` & `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_department.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     def test_departements_by_code(self) -> None:
         time.sleep(WAIT_TIME)
         r = self.api.departements_by_code(code=92)
         self.assertTrue(r.status_code == 200)
 
     def test_departements_by_region(self) -> None:
         time.sleep(WAIT_TIME)
-        r = self.api.departements_by_region(regioncode=28)
+        r = self.api.departements_by_region(code=28)
         self.assertTrue(r.status_code == 200)
 
     def test_departements_response(self) -> None:
         results = [DepartmentsResponse(**r) for r in self.test_departements().json()]
         self.assertTrue(True)
```

### Comparing `geo_api_gouv_fr-0.5.0/geo_api_gouv_fr/tests/test_region.py` & `geo_api_gouv_fr-1.0.0/geo_api_gouv_fr/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `geo_api_gouv_fr-0.5.0/pyproject.toml` & `geo_api_gouv_fr-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geo-api-gouv-fr"
-version = "0.5.0"
+version = "1.0.0"
 description = "Python package to use geoapi.gouv.fr api"
 authors = ["La Bonne Boite <labonneboite@pole-emploi.fr>"]
 license  = "GPL-3.0-only"
 keywords = ["geoapi", "geoapi.gouv", "geoapi.gouv.fr"]
 readme = "README.md"
 packages = [
     { include = "geo_api_gouv_fr" }
@@ -32,26 +32,26 @@
 coverage = "^6.4.4"
 pytest-html = "^3.1.1"
 
 
 [tool.poetry.group.help.dependencies]
 mkdocs = "^1.4.1"
 mkdocs-material = "^8.5.6"
-
+mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--cov"
 testpaths = [
-    "poleemploi_io_api/tests"
+    "geo_api_gouv_fr/tests"
 ]
 python_files = "test_*.py"
 
 env = []
 
 
 [tool.coverage.run]
```

### Comparing `geo_api_gouv_fr-0.5.0/PKG-INFO` & `geo_api_gouv_fr-1.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-api-gouv-fr
-Version: 0.5.0
+Version: 1.0.0
 Summary: Python package to use geoapi.gouv.fr api
 Home-page: https://github.com/StartupsPoleEmploi/geo-api-gouv-fr
 License: GPL-3.0-only
 Keywords: geoapi,geoapi.gouv,geoapi.gouv.fr
 Author: La Bonne Boite
 Author-email: labonneboite@pole-emploi.fr
 Requires-Python: >=3.10,<4.0
```

