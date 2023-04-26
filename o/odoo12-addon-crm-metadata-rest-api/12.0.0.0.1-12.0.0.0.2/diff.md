# Comparing `tmp/odoo12_addon_crm_metadata_rest_api-12.0.0.0.1-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_metadata_rest_api-12.0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3699 bytes, number of entries: 10
--rwxr-xr-x  2.0 unx      146 b- defN 23-Mar-07 17:36 odoo/addons/crm_metadata_rest_api/README.rst
+Zip file size: 3723 bytes, number of entries: 10
+-rwxr-xr-x  2.0 unx      146 b- defN 23-Apr-21 07:41 odoo/addons/crm_metadata_rest_api/README.rst
 -rwxrwxr-x  2.0 unx       23 b- defN 23-Feb-13 10:37 odoo/addons/crm_metadata_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      484 b- defN 23-Apr-19 16:23 odoo/addons/crm_metadata_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx      484 b- defN 23-Apr-26 11:08 odoo/addons/crm_metadata_rest_api/__manifest__.py
 -rwxrwxr-x  2.0 unx       32 b- defN 23-Feb-13 17:54 odoo/addons/crm_metadata_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      801 b- defN 23-Mar-07 17:36 odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
--rwxr-xr-x  2.0 unx      314 b- defN 23-Apr-19 15:51 odoo/addons/crm_metadata_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      572 b- defN 23-Apr-19 16:29 odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 16:29 odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-19 16:29 odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-19 16:29 odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/RECORD
-10 files, 3535 bytes uncompressed, 1789 bytes compressed:  49.4%
+-rwxr-xr-x  2.0 unx      911 b- defN 23-Apr-26 11:07 odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx      314 b- defN 23-Apr-21 07:41 odoo/addons/crm_metadata_rest_api/services/schemas.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Apr-26 11:10 odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 11:10 odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-26 11:10 odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Apr-26 11:10 odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/RECORD
+10 files, 3645 bytes uncompressed, 1813 bytes compressed:  50.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_metadata_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/METADATA
+Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/WHEEL
+Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/top_level.txt
+Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/RECORD
+Filename: odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_metadata_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM Metadata on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '12.0.0.0.1',
+    'version': '12.0.0.0.2',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_metadata',
         'crm_rest_api'
     ],
```

## odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py

```diff
@@ -9,16 +9,18 @@
     def _validator_create(self):
         validator_schema = super()._validator_create().copy()
         validator_schema.update(schemas.S_CRM_LEAD_CREATE)
         return validator_schema
 
     def _prepare_create(self, params):
         create_dict = super()._prepare_create(params)
-        crm_metadata_lines_args = [
-            line
-            for line in params["metadata"]
-        ]
-        crm_metadata_lines = self.env["crm.lead.metadata.line"].create(
-            crm_metadata_lines_args)
-        create_dict['metadata_line_ids'] = [
-            (6, 0, [line.id for line in crm_metadata_lines])]
+        form_metadatas = params.get('metadata', False)
+        if form_metadatas:
+            crm_metadata_lines_args = [
+                line
+                for line in form_metadatas
+            ]
+            crm_metadata_lines = self.env["crm.lead.metadata.line"].create(
+                crm_metadata_lines_args)
+            create_dict['metadata_line_ids'] = [
+                (6, 0, [line.id for line in crm_metadata_lines])]
         return create_dict
```

## Comparing `odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/METADATA` & `odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-metadata-rest-api
-Version: 12.0.0.0.1
+Version: 12.0.0.0.2
 Summary: Expose CRM Metadata on the Rest API
 Home-page: 
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/RECORD` & `odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_metadata_rest_api/README.rst,sha256=DvbD63tEN89Nk3TUJBQVhpPF5cL1CMXdJT5kbvLfOWg,146
 odoo/addons/crm_metadata_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_metadata_rest_api/__manifest__.py,sha256=QbAkesI6hc4rZ31NUyNyEmveQYQRlJ4UNPZyyGWEobc,484
+odoo/addons/crm_metadata_rest_api/__manifest__.py,sha256=p-2CKbw8yHumomYpvlxi-PbzYVJ5dBBKlQXYGY0pdtg,484
 odoo/addons/crm_metadata_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
-odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py,sha256=8Nhhyld-Zh9utvsdYroBrl4-LVf6w1xAsSZJIsu_wS0,801
+odoo/addons/crm_metadata_rest_api/services/crm_lead_services.py,sha256=faCwYuAG0Byu3ef1aonpYjhaXdWBlQhNFLsvwEO29gw,911
 odoo/addons/crm_metadata_rest_api/services/schemas.py,sha256=9VEyt5XaHTZk6z1CnaKwXHKaVTWN8047TvlIDZtWE4k,314
-odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/METADATA,sha256=CsiQUJZn4kllzTwy-YF6iJEradlswh-1t1DmZT0xkTA,572
-odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_metadata_rest_api-12.0.0.0.1.dist-info/RECORD,,
+odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/METADATA,sha256=13_6Phmtj8p2vkmCPlRUfyv1MK-72Ufe111DiabR1i8,572
+odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_metadata_rest_api-12.0.0.0.2.dist-info/RECORD,,
```

