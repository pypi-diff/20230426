# Comparing `tmp/etsy-apiv3-1.7.6.tar.gz` & `tmp/etsy-apiv3-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy-apiv3-1.7.6.tar", last modified: Thu Apr  6 12:41:17 2023, max compression
+gzip compressed data, was "etsy-apiv3-1.7.7.tar", last modified: Tue Apr 25 14:31:18 2023, max compression
```

## Comparing `etsy-apiv3-1.7.6.tar` & `etsy-apiv3-1.7.7.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:17.201452 etsy-apiv3-1.7.6/
--rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.7.6/LICENSE
--rw-rw-rw-   0        0        0      342 2023-04-06 12:41:17.200452 etsy-apiv3-1.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.7.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:16.819314 etsy-apiv3-1.7.6/etsy_apiv3/
--rw-rw-rw-   0        0        0       23 2023-04-06 12:41:03.000000 etsy-apiv3-1.7.6/etsy_apiv3/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:17.076453 etsy-apiv3-1.7.6/etsy_apiv3/models/
--rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/Auth.py
--rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/File.py
--rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ListingImageModel.py
--rw-rw-rw-   0        0        0     3624 2023-03-09 13:16:20.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ListingModel.py
--rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ListingPropertyModel.py
--rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/OfferingModel.py
--rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/PaymentModel.py
--rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/PriceModel.py
--rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ProductModel.py
--rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ProductionPartnerModel.py
--rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/PropertyValueModel.py
--rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ReceiptModel.py
--rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/RefundModel.py
--rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ReturnPolicyModel.py
--rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ReviewModel.py
--rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShipmentModel.py
--rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingCarrierModel.py
--rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingProfileDestinationModel.py
--rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingProfileModel.py
--rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingProfileUpgradeModel.py
--rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShopModel.py
--rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/ShopSection.py
--rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/TaxonomyModel.py
--rw-rw-rw-   0        0        0      165 2022-10-15 08:41:32.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/TokenModel.py
--rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/TransactionModel.py
--rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/TranslationModel.py
--rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/UserModel.py
--rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/VariationModel.py
--rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.7.6/etsy_apiv3/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:17.157453 etsy-apiv3-1.7.6/etsy_apiv3/resources/
--rw-rw-rw-   0        0        0    17670 2023-04-06 12:40:39.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ListingResource.py
--rw-rw-rw-   0        0        0     2546 2023-01-12 13:52:03.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/PaymentResource.py
--rw-rw-rw-   0        0        0     5868 2023-03-31 08:47:12.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ReceiptResource.py
--rw-rw-rw-   0        0        0     1315 2022-11-29 15:23:31.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ReviewResource.py
--rw-rw-rw-   0        0        0     6035 2023-01-28 10:23:31.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ShippingProfileResource.py
--rw-rw-rw-   0        0        0     2721 2023-01-28 10:45:52.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ShopPolicyResource.py
--rw-rw-rw-   0        0        0     3758 2023-02-02 08:42:56.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/ShopResource.py
--rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/UserResource.py
--rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.7.6/etsy_apiv3/resources/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:17.163457 etsy-apiv3-1.7.6/etsy_apiv3/utils/
--rw-rw-rw-   0        0        0     4087 2023-04-06 08:26:38.000000 etsy-apiv3-1.7.6/etsy_apiv3/utils/APIV3.py
--rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.7.6/etsy_apiv3/utils/RequestException.py
--rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.7.6/etsy_apiv3/utils/Response.py
--rw-rw-rw-   0        0        0       84 2022-11-29 14:45:38.000000 etsy-apiv3-1.7.6/etsy_apiv3/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:16.855325 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/
--rw-rw-rw-   0        0        0      342 2023-04-06 12:41:16.000000 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1847 2023-04-06 12:41:16.000000 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 12:41:16.000000 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-04-06 12:41:16.000000 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-06 12:41:16.000000 etsy-apiv3-1.7.6/etsy_apiv3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 12:41:17.201452 etsy-apiv3-1.7.6/setup.cfg
--rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 12:41:17.199458 etsy-apiv3-1.7.6/tests/
--rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.7.6/tests/Payment.py
--rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.7.6/tests/Receipt.py
--rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.7.6/tests/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.7.6/tests/taxonomy_test.py
--rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.7.6/tests/test_credentials.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:18.062085 etsy-apiv3-1.7.7/
+-rw-rw-rw-   0        0        0     1089 2022-11-29 15:57:22.000000 etsy-apiv3-1.7.7/LICENSE
+-rw-rw-rw-   0        0        0      342 2023-04-25 14:31:18.062085 etsy-apiv3-1.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1120 2022-12-02 14:38:46.000000 etsy-apiv3-1.7.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:17.593229 etsy-apiv3-1.7.7/etsy_apiv3/
+-rw-rw-rw-   0        0        0       23 2023-04-25 14:31:14.000000 etsy-apiv3-1.7.7/etsy_apiv3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:17.863772 etsy-apiv3-1.7.7/etsy_apiv3/models/
+-rw-rw-rw-   0        0        0      126 2023-01-05 12:58:42.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/Auth.py
+-rw-rw-rw-   0        0        0      293 2023-01-05 11:18:24.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/File.py
+-rw-rw-rw-   0        0        0      604 2022-06-06 13:20:33.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ListingImageModel.py
+-rw-rw-rw-   0        0        0     3966 2023-04-25 14:30:59.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ListingModel.py
+-rw-rw-rw-   0        0        0      293 2022-04-23 21:35:29.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ListingPropertyModel.py
+-rw-rw-rw-   0        0        0      255 2022-11-29 15:27:15.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/OfferingModel.py
+-rw-rw-rw-   0        0        0     2124 2023-01-12 13:28:51.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/PaymentModel.py
+-rw-rw-rw-   0        0        0      116 2022-04-04 14:44:43.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/PriceModel.py
+-rw-rw-rw-   0        0        0      334 2022-11-29 15:27:25.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ProductModel.py
+-rw-rw-rw-   0        0        0      143 2022-04-05 14:24:47.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ProductionPartnerModel.py
+-rw-rw-rw-   0        0        0      303 2022-07-02 07:06:56.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/PropertyValueModel.py
+-rw-rw-rw-   0        0        0     1961 2022-11-29 15:27:49.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ReceiptModel.py
+-rw-rw-rw-   0        0        0      199 2022-11-29 15:27:55.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/RefundModel.py
+-rw-rw-rw-   0        0        0      245 2023-01-05 13:51:36.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ReturnPolicyModel.py
+-rw-rw-rw-   0        0        0      394 2022-04-23 16:26:45.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ReviewModel.py
+-rw-rw-rw-   0        0        0      254 2022-10-15 18:09:39.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShipmentModel.py
+-rw-rw-rw-   0        0        0      293 2023-01-06 08:26:38.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingCarrierModel.py
+-rw-rw-rw-   0        0        0      537 2023-01-28 10:35:20.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingProfileDestinationModel.py
+-rw-rw-rw-   0        0        0      698 2022-11-29 15:28:16.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingProfileModel.py
+-rw-rw-rw-   0        0        0      381 2022-11-29 15:28:31.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingProfileUpgradeModel.py
+-rw-rw-rw-   0        0        0     1609 2022-07-02 07:49:17.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShopModel.py
+-rw-rw-rw-   0        0        0      171 2023-01-05 13:22:47.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/ShopSection.py
+-rw-rw-rw-   0        0        0      930 2023-01-06 07:39:02.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/TaxonomyModel.py
+-rw-rw-rw-   0        0        0      165 2022-10-15 08:41:32.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/TokenModel.py
+-rw-rw-rw-   0        0        0      974 2023-02-18 13:56:54.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/TransactionModel.py
+-rw-rw-rw-   0        0        0      187 2022-04-05 14:20:33.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/TranslationModel.py
+-rw-rw-rw-   0        0        0      728 2023-01-05 12:33:05.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/UserModel.py
+-rw-rw-rw-   0        0        0      202 2022-04-05 14:03:40.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/VariationModel.py
+-rw-rw-rw-   0        0        0     1224 2023-01-06 12:04:29.000000 etsy-apiv3-1.7.7/etsy_apiv3/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:17.982777 etsy-apiv3-1.7.7/etsy_apiv3/resources/
+-rw-rw-rw-   0        0        0    17694 2023-04-07 07:20:56.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ListingResource.py
+-rw-rw-rw-   0        0        0     2546 2023-01-12 13:52:03.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/PaymentResource.py
+-rw-rw-rw-   0        0        0     5868 2023-03-31 08:47:12.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ReceiptResource.py
+-rw-rw-rw-   0        0        0     1315 2022-11-29 15:23:31.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ReviewResource.py
+-rw-rw-rw-   0        0        0     6035 2023-01-28 10:23:31.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ShippingProfileResource.py
+-rw-rw-rw-   0        0        0     2721 2023-01-28 10:45:52.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ShopPolicyResource.py
+-rw-rw-rw-   0        0        0     3758 2023-02-02 08:42:56.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/ShopResource.py
+-rw-rw-rw-   0        0        0      190 2023-01-06 12:19:53.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/UserResource.py
+-rw-rw-rw-   0        0        0      222 2023-01-12 13:29:03.000000 etsy-apiv3-1.7.7/etsy_apiv3/resources/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:18.004774 etsy-apiv3-1.7.7/etsy_apiv3/utils/
+-rw-rw-rw-   0        0        0     4091 2023-04-06 13:41:59.000000 etsy-apiv3-1.7.7/etsy_apiv3/utils/APIV3.py
+-rw-rw-rw-   0        0        0      474 2022-04-22 20:27:32.000000 etsy-apiv3-1.7.7/etsy_apiv3/utils/RequestException.py
+-rw-rw-rw-   0        0        0      218 2022-07-02 14:30:58.000000 etsy-apiv3-1.7.7/etsy_apiv3/utils/Response.py
+-rw-rw-rw-   0        0        0       84 2022-11-29 14:45:38.000000 etsy-apiv3-1.7.7/etsy_apiv3/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:17.629279 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-04-25 14:31:16.000000 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1847 2023-04-25 14:31:17.000000 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:31:16.000000 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-04-25 14:31:17.000000 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-04-25 14:31:17.000000 etsy-apiv3-1.7.7/etsy_apiv3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 14:31:18.063086 etsy-apiv3-1.7.7/setup.cfg
+-rw-rw-rw-   0        0        0      746 2023-02-18 14:12:46.000000 etsy-apiv3-1.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:31:18.061087 etsy-apiv3-1.7.7/tests/
+-rw-rw-rw-   0        0        0     2246 2023-01-12 13:49:46.000000 etsy-apiv3-1.7.7/tests/Payment.py
+-rw-rw-rw-   0        0        0     3880 2023-03-15 09:02:53.000000 etsy-apiv3-1.7.7/tests/Receipt.py
+-rw-rw-rw-   0        0        0        0 2023-03-15 09:02:44.000000 etsy-apiv3-1.7.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-13 08:43:06.000000 etsy-apiv3-1.7.7/tests/taxonomy_test.py
+-rw-rw-rw-   0        0        0      426 2023-01-12 11:25:14.000000 etsy-apiv3-1.7.7/tests/test_credentials.py
```

### Comparing `etsy-apiv3-1.7.6/LICENSE` & `etsy-apiv3-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/README.md` & `etsy-apiv3-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ListingImageModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ListingImageModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ListingModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ListingModel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
-from typing import List, Optional
-from pydantic import BaseModel
+import html
+from typing import Annotated, List, Optional
+from pydantic import BaseModel, validator
 
 from .ListingImageModel import ListingImage 
 from .ProductionPartnerModel import ProductionPartner
 from .ShippingProfileModel import ShippingProfile
 from .ShopModel import Shop
 from .TranslationModel import Translation
 from .UserModel import User
 from .PriceModel import Price
 from .ProductModel import Product
 
-
 class Video(BaseModel):
     video_id: int
     height: int
     width: int
     thumbnail_url: str
     video_url: str
     video_state: str
@@ -66,15 +66,15 @@
     is_supply: bool
     is_customizable: bool
     should_auto_renew: bool
     is_taxable: bool
     type: str = "physical"
     
 class Listing(BaseModel):
-    listing_id: int
+    listing_id: Annotated[int, "listing_id"]
     user_id: int
     shop_id: int
     title: str
     description: str
     state: str
     creation_timestamp: int
     ending_timestamp: int
@@ -120,9 +120,20 @@
     shop: Optional[Shop]
     images: Optional[List[ListingImage]]
     production_partners: List[ProductionPartner]
     skus: List[str]
     translations: Optional[List[Translation]]
     inventory: Optional[Inventory]
     views: Optional[int]
+
+    @validator("title")
+    def title_validator(cls, value):
+        new_value = html.unescape(value)
+        return new_value
     
+    @validator("description")
+    def description_validator(cls, value):
+        new_value = html.unescape(value)
+        return new_value
+    
+
 Inventory.update_forward_refs()
```

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/PaymentModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/PaymentModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ReceiptModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ReceiptModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingProfileDestinationModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingProfileDestinationModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ShippingProfileModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ShippingProfileModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/ShopModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/ShopModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/TaxonomyModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/TaxonomyModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/TransactionModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/TransactionModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/UserModel.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/UserModel.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/models/__init__.py` & `etsy-apiv3-1.7.7/etsy_apiv3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ListingResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ListingResource.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         Returns:
             Listing: A Single Listing Object
         """
         endpoint = f"listings/{listing_id}"
         json = self.session.request(endpoint, params={"includes":includes})
         return Listing(**json)
 
-    def find_all_active_listings(self, limit=25, offset=0, keywords="", sort_on="created", sort_order="desc", min_price=None, max_price=None, taxonomy_id=None, shop_location="United States"):
+    def find_all_active_listings(self, limit=25, offset=0, keywords="", sort_on="created", sort_order="desc", min_price=None, max_price=None, taxonomy_id=None, shop_location="United States", _as="pydantic"):
         """
         Find All Active Listings By Keywords, Min price, Max Price Or Shop Location
 
         Args:
             limit (int, optional): Result Limit. Defaults to 25, Max 100.
             offset (int, optional): Result Offset. Defaults to 0.
             keywords (str, optional): Keywords For Active Listings. Defaults to "".
@@ -55,15 +55,15 @@
         params = {
             "limit":limit, "offset":offset, "keywords":keywords, "sort_on":sort_on,
             "sort_order":sort_order, "min_price":min_price, "max_price":max_price,
             "taxonomy_id":taxonomy_id, "shop_location":shop_location
         }
         
         json = self.session.request(endpoint, params=params)
-
+        
         return Response[Listing](**json)
     
     def find_all_active_listings_by_shop(self, shop_id: int, limit: int = 25, sort_on: str = "created", sort_order: str = "desc", offset: int = 0, keywords: str = ""):
         endpoint = f"shops/{shop_id}/listings/active"
         
         params = {"limit": limit, "sort_on": sort_on, "sort_order": sort_order,
                   "offset": offset, "keywords": keywords
```

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/PaymentResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/PaymentResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ReceiptResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ReceiptResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ReviewResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ReviewResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ShippingProfileResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ShippingProfileResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ShopPolicyResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ShopPolicyResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/resources/ShopResource.py` & `etsy-apiv3-1.7.7/etsy_apiv3/resources/ShopResource.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3/utils/APIV3.py` & `etsy-apiv3-1.7.7/etsy_apiv3/utils/APIV3.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         return session
     
     @property
     def me(self) -> Me:
         if self.__me is None:
             self.__me = Me(**self.request(f"users/me"))
         return self.__me
-
+    
     @staticmethod
     def create_response(response: requests.Response):
         json: dict = response.json()
 
         if "error" in json.keys():
             raise EtsyRequestException(response.status_code, json["error"])
```

### Comparing `etsy-apiv3-1.7.6/etsy_apiv3.egg-info/SOURCES.txt` & `etsy-apiv3-1.7.7/etsy_apiv3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/setup.py` & `etsy-apiv3-1.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/tests/Payment.py` & `etsy-apiv3-1.7.7/tests/Payment.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/tests/Receipt.py` & `etsy-apiv3-1.7.7/tests/Receipt.py`

 * *Files identical despite different names*

### Comparing `etsy-apiv3-1.7.6/tests/taxonomy_test.py` & `etsy-apiv3-1.7.7/tests/taxonomy_test.py`

 * *Files identical despite different names*

