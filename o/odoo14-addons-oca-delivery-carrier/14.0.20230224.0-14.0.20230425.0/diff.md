# Comparing `tmp/odoo14_addons_oca_delivery_carrier-14.0.20230224.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_delivery_carrier-14.0.20230425.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1761 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2448 b- defN 23-Feb-25 04:03 odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 04:03 odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-25 04:03 odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      445 b- defN 23-Feb-25 04:03 odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/RECORD
-4 files, 2986 bytes uncompressed, 883 bytes compressed:  70.4%
+Zip file size: 1773 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2509 b- defN 23-Apr-26 03:53 odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 03:53 odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-26 03:53 odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      445 b- defN 23-Apr-26 03:53 odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/RECORD
+4 files, 3047 bytes uncompressed, 895 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/METADATA
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/RECORD
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_delivery_carrier-14.0.20230224.0.dist-info/METADATA` & `odoo14_addons_oca_delivery_carrier-14.0.20230425.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-delivery-carrier
-Version: 14.0.20230224.0
+Version: 14.0.20230425.0
 Summary: Meta package for oca-delivery-carrier Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -35,14 +35,15 @@
 Requires-Dist: odoo14-addon-delivery-postlogistics-server-env
 Requires-Dist: odoo14-addon-delivery-price-method
 Requires-Dist: odoo14-addon-delivery-price-rule-untaxed
 Requires-Dist: odoo14-addon-delivery-roulier
 Requires-Dist: odoo14-addon-delivery-roulier-laposte-fr
 Requires-Dist: odoo14-addon-delivery-roulier-option
 Requires-Dist: odoo14-addon-delivery-schenker
+Requires-Dist: odoo14-addon-delivery-schenker-picking-volume
 Requires-Dist: odoo14-addon-delivery-send-to-shipper-at-operation
 Requires-Dist: odoo14-addon-delivery-state
 Requires-Dist: odoo14-addon-delivery-tnt-oca
 Requires-Dist: odoo14-addon-partner-default-delivery-carrier
 Requires-Dist: odoo14-addon-partner-delivery-zone
 Requires-Dist: odoo14-addon-server-environment-delivery
 Requires-Dist: odoo14-addon-stock-picking-carrier-from-rule
```

