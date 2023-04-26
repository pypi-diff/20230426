# Comparing `tmp/genie.libs.health-23.3-py3-none-any.whl.zip` & `tmp/genie.libs.health-23.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
 Zip file size: 20772 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1676 b- defN 23-Mar-29 18:45 genie.libs.health-23.3-py3.9-nspkg.pth
--rw-r--r--  2.0 unx      425 b- defN 23-Mar-29 18:08 genie/libs/health/__init__.py
--rw-r--r--  2.0 unx    47472 b- defN 23-Mar-29 18:06 genie/libs/health/health.py
--rw-r--r--  2.0 unx    24099 b- defN 23-Mar-29 18:06 genie/libs/health/plugin.py
--rw-r--r--  2.0 unx      190 b- defN 23-Mar-29 18:06 genie/libs/health/health_yamls/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Mar-29 18:06 genie/libs/health/health_yamls/health_config.yaml
--rw-r--r--  2.0 unx     9079 b- defN 23-Mar-29 18:06 genie/libs/health/health_yamls/pyats_health.yaml
--rw-r--r--  2.0 unx     3597 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1206 b- defN 23-Mar-29 18:45 genie.libs.health-23.3.dist-info/RECORD
+-rw-r--r--  2.0 unx     1676 b- defN 23-Apr-21 18:43 genie.libs.health-23.4-py3.9-nspkg.pth
+-rw-r--r--  2.0 unx      425 b- defN 23-Apr-21 18:08 genie/libs/health/__init__.py
+-rw-r--r--  2.0 unx    47472 b- defN 23-Apr-21 18:06 genie/libs/health/health.py
+-rw-r--r--  2.0 unx    24099 b- defN 23-Apr-21 18:06 genie/libs/health/plugin.py
+-rw-r--r--  2.0 unx      190 b- defN 23-Apr-21 18:06 genie/libs/health/health_yamls/__init__.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Apr-21 18:06 genie/libs/health/health_yamls/health_config.yaml
+-rw-r--r--  2.0 unx     9079 b- defN 23-Apr-21 18:06 genie/libs/health/health_yamls/pyats_health.yaml
+-rw-r--r--  2.0 unx     3597 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1206 b- defN 23-Apr-21 18:43 genie.libs.health-23.4.dist-info/RECORD
 13 files, 88977 bytes uncompressed, 18706 bytes compressed:  79.0%
```

## zipnote {}

```diff
@@ -1,8 +1,8 @@
-Filename: genie.libs.health-23.3-py3.9-nspkg.pth
+Filename: genie.libs.health-23.4-py3.9-nspkg.pth
 Comment: 
 
 Filename: genie/libs/health/__init__.py
 Comment: 
 
 Filename: genie/libs/health/health.py
 Comment: 
@@ -15,26 +15,26 @@
 
 Filename: genie/libs/health/health_yamls/health_config.yaml
 Comment: 
 
 Filename: genie/libs/health/health_yamls/pyats_health.yaml
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/METADATA
+Filename: genie.libs.health-23.4.dist-info/METADATA
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/WHEEL
+Filename: genie.libs.health-23.4.dist-info/WHEEL
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/entry_points.txt
+Filename: genie.libs.health-23.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/namespace_packages.txt
+Filename: genie.libs.health-23.4.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/top_level.txt
+Filename: genie.libs.health-23.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genie.libs.health-23.3.dist-info/RECORD
+Filename: genie.libs.health-23.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genie/libs/health/__init__.py

```diff
@@ -4,15 +4,15 @@
 
     Description:
         This is the sub-component of Genie for `genie.libs.health`.
 
 '''
 
 # metadata
-__version__ = '23.3'
+__version__ = '23.4'
 __author__ = 'Cisco Systems Inc.'
 __contact__ = ['asg-genie-support@cisco.com', 'pyats-support-ext@cisco.com']
 __copyright__ = 'Copyright (c) 2020, Cisco Systems Inc.'
 
 from genie import abstract
 abstract.declare_package(__name__)
```

## Comparing `genie.libs.health-23.3-py3.9-nspkg.pth` & `genie.libs.health-23.4-py3.9-nspkg.pth`

 * *Files identical despite different names*

## Comparing `genie.libs.health-23.3.dist-info/METADATA` & `genie.libs.health-23.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genie.libs.health
-Version: 23.3
+Version: 23.4
 Summary: pyATS Health Check for monitoring device health status
 Home-page: https://developer.cisco.com/pyats
 Author: Cisco Systems Inc.
 Author-email: pyats-support-ext@cisco.com
 License: Apache 2.0
 Keywords: genie health pyats cisco
 Classifier: Development Status :: 6 - Mature
```

## Comparing `genie.libs.health-23.3.dist-info/RECORD` & `genie.libs.health-23.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-genie.libs.health-23.3-py3.9-nspkg.pth,sha256=ObYoD8sL3pc4avNcQOL6mdv2IdNlOmFr3c3nD1iDADQ,1676
-genie/libs/health/__init__.py,sha256=tpEqLB8bhL6d2IFAyqOv4VCKowWP-j4blwe03RJuRoA,425
+genie.libs.health-23.4-py3.9-nspkg.pth,sha256=ObYoD8sL3pc4avNcQOL6mdv2IdNlOmFr3c3nD1iDADQ,1676
+genie/libs/health/__init__.py,sha256=-93vzRb3TnpGWrRD6PJuPC2hEtTguF6qW6jJureCdF8,425
 genie/libs/health/health.py,sha256=iL3oXc9Jn399pNntZMaIIxsZ7YC4_LkAQ4T_czZEruQ,47472
 genie/libs/health/plugin.py,sha256=wAhhAW3mOHSxTc4YyF3Ch5kPtiBQ4awvQJS-V8EU0y0,24099
 genie/libs/health/health_yamls/__init__.py,sha256=IJLXnIm6k9OxWweGLf5P7D54ixDBWjg_akrvZbiNLp0,190
 genie/libs/health/health_yamls/health_config.yaml,sha256=KuIk9fzsqv83GZbSniGrnyby2xRFUUlE6LL5eNsVPnE,1047
 genie/libs/health/health_yamls/pyats_health.yaml,sha256=RitDHPAeJSibrwjGZ_Et4RXhW8VKeSgcNwLLx1ggYQ4,9079
-genie.libs.health-23.3.dist-info/METADATA,sha256=zfM31bLZrnZaOSmZVMSlgQ2jqP-Ro5cPOfJ7y60G03o,3597
-genie.libs.health-23.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-genie.libs.health-23.3.dist-info/entry_points.txt,sha256=nok2ESU1_NDPqONDaaD2ylzaaS49M1LCOElYzunD3Ro,71
-genie.libs.health-23.3.dist-info/namespace_packages.txt,sha256=k0OxVAETbf7Ou2EqqjuxO-JdrIdJtxZsUDHdrIkrOFE,17
-genie.libs.health-23.3.dist-info/top_level.txt,sha256=EW4swMMBmuGW5VFCUGsl828kVUhrmMZJGHXfzmOidSg,6
-genie.libs.health-23.3.dist-info/RECORD,,
+genie.libs.health-23.4.dist-info/METADATA,sha256=Y2-2exbt_rNw9efP7TgI2qvv91KZZW0ImVclej_GtS4,3597
+genie.libs.health-23.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+genie.libs.health-23.4.dist-info/entry_points.txt,sha256=nok2ESU1_NDPqONDaaD2ylzaaS49M1LCOElYzunD3Ro,71
+genie.libs.health-23.4.dist-info/namespace_packages.txt,sha256=k0OxVAETbf7Ou2EqqjuxO-JdrIdJtxZsUDHdrIkrOFE,17
+genie.libs.health-23.4.dist-info/top_level.txt,sha256=EW4swMMBmuGW5VFCUGsl828kVUhrmMZJGHXfzmOidSg,6
+genie.libs.health-23.4.dist-info/RECORD,,
```

