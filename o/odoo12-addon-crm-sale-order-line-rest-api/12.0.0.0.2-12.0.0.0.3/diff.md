# Comparing `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3879 bytes, number of entries: 10
+Zip file size: 3904 bytes, number of entries: 10
 -rwxr-xr-x  2.0 unx      149 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/README.rst
 -rwxr-xr-x  2.0 unx       23 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/__init__.py
--rwxr-xr-x  2.0 unx      501 b- defN 23-Apr-21 13:16 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
+-rwxr-xr-x  2.0 unx      501 b- defN 23-Apr-26 11:08 odoo/addons/crm_sale_order_line_rest_api/__manifest__.py
 -rwxr-xr-x  2.0 unx       32 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py
--rwxr-xr-x  2.0 unx      790 b- defN 23-Apr-21 07:41 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
+-rwxr-xr-x  2.0 unx      906 b- defN 23-Apr-26 11:04 odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
 -rwxr-xr-x  2.0 unx      332 b- defN 23-Apr-21 12:57 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
--rw-r--r--  2.0 unx      592 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-21 13:23 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD
-10 files, 3652 bytes uncompressed, 1829 bytes compressed:  49.9%
+-rw-r--r--  2.0 unx      592 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1136 b- defN 23-Apr-26 11:10 odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD
+10 files, 3768 bytes uncompressed, 1854 bytes compressed:  50.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py
 Comment: 
 
 Filename: odoo/addons/crm_sale_order_line_rest_api/services/schemas.py
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD
+Filename: odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_sale_order_line_rest_api/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Expose CRM order lines on the Rest API""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'api',
-    'version': '12.0.0.0.2',
+    'version': '12.0.0.0.3',
 
     # any module necessary for this one to work correctly
     'depends': [
         'base',
         'crm_rest_api',
         'crm_sale_order_line'
     ],
```

## odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py

```diff
@@ -9,16 +9,18 @@
     def _validator_create(self):
         validator_schema = super()._validator_create().copy()
         validator_schema.update(schemas.S_CRM_LEAD_CREATE)
         return validator_schema
 
     def _prepare_create(self, params):
         create_dict = super()._prepare_create(params)
-        crm_order_lines_args = [
-            line
-            for line in params["order_lines"]
-        ]
-        crm_order_lines = self.env["crm.sale.order.line"].create(
-            crm_order_lines_args)
-        create_dict['crm_order_line_ids'] = [
-            (6, 0, [line.id for line in crm_order_lines])]
+        form_order_lines = params.get('order_lines', False)
+        if form_order_lines:
+            crm_order_lines_args = [
+                line
+                for line in form_order_lines
+            ]
+            crm_order_lines = self.env["crm.sale.order.line"].create(
+                crm_order_lines_args)
+            create_dict['crm_order_line_ids'] = [
+                (6, 0, [line.id for line in crm_order_lines])]
         return create_dict
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-sale-order-line-rest-api
-Version: 12.0.0.0.2
+Version: 12.0.0.0.3
 Summary: Expose CRM order lines on the Rest API
 Home-page: 
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD` & `odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 odoo/addons/crm_sale_order_line_rest_api/README.rst,sha256=TbC3DjY4NLfKhsHanGsOWW_jEi0eFHD4Hbq0nKihPxY,149
 odoo/addons/crm_sale_order_line_rest_api/__init__.py,sha256=qksdRxAxHhEXpY0NZlTEolhxFILjRI5o7J0O4UrAE04,23
-odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=L3_O_HLNw_nTD0E6u2zPTbDutkAIi0sw35GBPwdF9WY,501
+odoo/addons/crm_sale_order_line_rest_api/__manifest__.py,sha256=lYNqTgDrk9rvF8fgkG1cZNDa2PFcoB152MGrjKFVGwA,501
 odoo/addons/crm_sale_order_line_rest_api/services/__init__.py,sha256=gyXaE_NlVgF1KawzsiRb0DeYYTT13kmL4Ya1LgcRg5c,32
-odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py,sha256=e1GEjo_Q2qz2ucNj1oQhQHhnm-pVEH1os47aFE3-x-M,790
+odoo/addons/crm_sale_order_line_rest_api/services/crm_lead_services.py,sha256=xMr4PV_YLnn_2OB51WCNEzhQ3Xn7yASMzVievYjHKbQ,906
 odoo/addons/crm_sale_order_line_rest_api/services/schemas.py,sha256=tTudvFX7WOVnZ_58fjiEzl4m8LnXuvw2j_gGgqcmIEE,332
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/METADATA,sha256=0j9w1ZOc_ybJP6eVej-tSjXzksZPPZFsSm1YsYq5JvU,592
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.2.dist-info/RECORD,,
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/METADATA,sha256=WRkQGka89YJLYDD6bua03mhbiV4sRANAjKACmz5rJEE,592
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_sale_order_line_rest_api-12.0.0.0.3.dist-info/RECORD,,
```

