# Comparing `tmp/arrendatools.plantillas-0.1.0.tar.gz` & `tmp/arrendatools.plantillas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.plantillas-0.1.0.tar", last modified: Wed Apr 19 17:49:56 2023, max compression
+gzip compressed data, was "arrendatools.plantillas-0.2.0.tar", last modified: Wed Apr 26 20:03:34 2023, max compression
```

## Comparing `arrendatools.plantillas-0.1.0.tar` & `arrendatools.plantillas-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:49:56.969947 arrendatools.plantillas-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-19 17:49:56.973947 arrendatools.plantillas-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:49:56.965947 arrendatools.plantillas-0.1.0/arrendatools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:49:56.969947 arrendatools.plantillas-0.1.0/arrendatools/plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:49:56.969947 arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/fechas.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/numeros.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-04-19 17:49:53.000000 arrendatools.plantillas-0.1.0/arrendatools/plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:49:56.969947 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-19 17:49:56.000000 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-19 17:49:56.000000 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:49:56.000000 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-04-19 17:49:56.000000 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-19 17:49:56.000000 arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-19 17:49:56.973947 arrendatools.plantillas-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2023-04-19 17:49:54.000000 arrendatools.plantillas-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.470889 arrendatools.plantillas-0.2.0/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools/plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/fechas.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/numeros.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-04-26 20:03:32.000000 arrendatools.plantillas-0.2.0/setup.py
```

### Comparing `arrendatools.plantillas-0.1.0/LICENSE` & `arrendatools.plantillas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.1.0/PKG-INFO` & `arrendatools.plantillas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.1.0
+Version: 0.2.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.1.0/README.md` & `arrendatools.plantillas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/fechas.py` & `arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/fechas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import calendar
-from dateutil import parser
+from datetime import datetime, timedelta
 from babel.dates import format_datetime, get_timezone
 
 
 def dias_del_año(año):
     """
     Calcula los dias que tiene un año teniendo en cuenta si es bisiesto o no
 
@@ -22,21 +22,28 @@
 
 def formato_fecha(fecha_hora=None, formato='medium', tzinfo='Europe/Madrid', locale='es_ES'):
     """
     Convierte una fecha dada en formato ISO8601 al formato especificado. Ver https://docs.python.org/3/library/datetime.html#strftime-and-strptime-behavior
 
     Args:
 
-        fecha_hora (): fecha en formato ISO8601. Si no se pasa ninguna se usa la fecha y hora actual
-        formato (): uno de  “full”, “long”, “medium”, o “short”, o un patron datetime personalizado. "medium" por defecto.
-        tzinfo (): la zona horaria a aplicar para dar formato a la fecha-hora. "Europe/Madrid" por defecto.
-        locale (): identificador de locale. es_ES por defecto.
+        fecha_hora (str): fecha en formato ISO8601. Si no se pasa ninguna se usa la fecha y hora actual
+        formato (str): uno de  “full”, “long”, “medium”, o “short”, o un patron datetime personalizado. "medium" por defecto.
+        tzinfo (str): la zona horaria a aplicar para dar formato a la fecha-hora. "Europe/Madrid" por defecto.
+        locale (str): identificador de locale. es_ES por defecto.
 
     Returns:
         str: La fecha en texto con el formato indicado
     """
     date = None
     time_zone = get_timezone(tzinfo)
     if isinstance(fecha_hora, str):
-        date = parser.parse(fecha_hora)
+        date = datetime.fromisoformat(fecha_hora)
 
     return format_datetime(date, formato, time_zone, locale)
+
+
+def aplicar_timedelta(fecha, semanas=0, dias=0, horas=0, minutos=0, segundos=0):
+    fecha_obj = datetime.fromisoformat(fecha)
+    delta = timedelta(days=dias, hours=horas, minutes=minutos, seconds=segundos, weeks=semanas)
+    nueva_fecha = fecha_obj + delta
+    return nueva_fecha.isoformat()
```

### Comparing `arrendatools.plantillas-0.1.0/arrendatools/plantillas/filters/numeros.py` & `arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/numeros.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.1.0/arrendatools.plantillas.egg-info/PKG-INFO` & `arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.1.0
+Version: 0.2.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.1.0/setup.py` & `arrendatools.plantillas-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 import pkg_resources
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 with open('LICENSE', encoding='utf-8') as f:
     license = f.read()
```

