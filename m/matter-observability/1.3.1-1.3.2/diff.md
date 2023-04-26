# Comparing `tmp/matter_observability-1.3.1-py3-none-any.whl.zip` & `tmp/matter_observability-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
 Zip file size: 11242 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_observability/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_observability/__init__.py
--rw-r--r--  2.0 unx      287 b- defN 20-Feb-02 00:00 matter_observability/config.py
+-rw-r--r--  2.0 unx      286 b- defN 20-Feb-02 00:00 matter_observability/config.py
 -rw-r--r--  2.0 unx      132 b- defN 20-Feb-02 00:00 matter_observability/exceptions.py
 -rw-r--r--  2.0 unx      133 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 20-Feb-02 00:00 matter_observability/fastapi/request_id.py
 -rw-r--r--  2.0 unx      817 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
 -rw-r--r--  2.0 unx       73 b- defN 20-Feb-02 00:00 matter_observability/logging/__init__.py
 -rw-r--r--  2.0 unx     1671 b- defN 20-Feb-02 00:00 matter_observability/logging/logging_config.py
 -rw-r--r--  2.0 unx      316 b- defN 20-Feb-02 00:00 matter_observability/metrics/__init__.py
 -rw-r--r--  2.0 unx      761 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
 -rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/metrics/decorators.py
 -rw-r--r--  2.0 unx      473 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_counter.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge.py
 -rw-r--r--  2.0 unx      708 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge_duration.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_metric.py
 -rw-r--r--  2.0 unx      903 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
-?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.3.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.3.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.3.1.dist-info/RECORD
-21 files, 19505 bytes uncompressed, 7876 bytes compressed:  59.6%
+?rw-r--r--  2.0 unx     5852 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-1.3.2.dist-info/RECORD
+21 files, 19504 bytes uncompressed, 7876 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: matter_observability/metrics/labeled_metric.py
 Comment: 
 
 Filename: matter_observability/metrics/utils.py
 Comment: 
 
-Filename: matter_observability-1.3.1.dist-info/METADATA
+Filename: matter_observability-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: matter_observability-1.3.1.dist-info/WHEEL
+Filename: matter_observability-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: matter_observability-1.3.1.dist-info/licenses/LICENSE
+Filename: matter_observability-1.3.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_observability-1.3.1.dist-info/RECORD
+Filename: matter_observability-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_observability/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "1.3.1"
+__version__ = "1.3.2"
```

## matter_observability/config.py

```diff
@@ -1,8 +1,8 @@
 import os
 
 
 class Config:
     ENABLE_METRICS = os.getenv("ENABLE_METRICS", "true").lower() == "true"
     SERVER_LOG_LEVEL = os.getenv("SERVER_LOG_LEVEL", "info")
     PROMETHEUS_PUSH_GATEWAY_HOST = os.getenv("PROMETHEUS_PUSH_GATEWAY_HOST")
-    INSTANCE_NAME = os.environ["INSTANCE_NAME"]
+    INSTANCE_NAME = os.getenv("INSTANCE_NAME")
```

## Comparing `matter_observability-1.3.1.dist-info/METADATA` & `matter_observability-1.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matter-observability
-Version: 1.3.1
+Version: 1.3.2
 Summary: A template for Matter's observability library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-observability#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-observability/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-observability
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
```

## Comparing `matter_observability-1.3.1.dist-info/licenses/LICENSE` & `matter_observability-1.3.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_observability-1.3.1.dist-info/RECORD` & `matter_observability-1.3.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-matter_observability/__about__.py,sha256=CPW6PjbggONszi5BcwHEGpcFeuh818A6qDuwiucl_cQ,134
+matter_observability/__about__.py,sha256=fc-P5LivZGhUVIEsmnCKHspv8lP88anHwfDV_1BaFuk,134
 matter_observability/__init__.py,sha256=3w1lcMfVq_KzRTAJVSrwL5vGSnu2BzERE4WFHCGvzFY,112
-matter_observability/config.py,sha256=fv7xrBqG99_Ptkw9ObF9ZSEC8zYJWhgbp2ScBR2BcCA,287
+matter_observability/config.py,sha256=m55Od1HaB8neBOYLhCJc2uwTSUlXT54JtOR5FzpqEQk,286
 matter_observability/exceptions.py,sha256=vc3AZT1ZsrkTgnkeoiOFsAgsSIlCkywHryUnm-APVQo,132
 matter_observability/fastapi/__init__.py,sha256=TBGRRAMg7Q2Ov_a6sUZuWIoH9ITxWF036CYLVn-K25g,133
 matter_observability/fastapi/request_id.py,sha256=frjbfIr6U3J6ElbA5ZDnNFiz7eKerCGStevHHZu78P0,641
 matter_observability/fastapi/utils.py,sha256=7_42_uQDpMliYsSz-K5txWLJMUySmPKThdmS559moKw,817
 matter_observability/logging/__init__.py,sha256=Xz1akGf5QHmMHjF9PpQ6Ljx8V5VI28N1tjom11jEKnQ,73
 matter_observability/logging/logging_config.py,sha256=TMRD_8nqEzO9TGu7r8p8ID0C10xUJNWPLygBIEP5q-E,1671
 matter_observability/metrics/__init__.py,sha256=CRAS0OI8AddFdIZFa66JvVam2tTjbfw-CLLEFRiwxnU,316
 matter_observability/metrics/custom_metrics.py,sha256=4WufeO-g14BzVfj0PEOWhaSug52K9vMNM5ZIVxlzESk,761
 matter_observability/metrics/decorators.py,sha256=DU-3lQZLYjSv_pTf36W_kdAvSZsOBrS61aPN7o8ryeM,2428
 matter_observability/metrics/labeled_counter.py,sha256=9ziI7Xlu1ApKo-eQcEVCSyAId_xvqo8jm6y3yLGT9ak,473
 matter_observability/metrics/labeled_gauge.py,sha256=MYJRPuqsvrjdBmDIiBaxzA66CUjJVI1KOGvzRRhDas0,489
 matter_observability/metrics/labeled_gauge_duration.py,sha256=-Xaxskzx2NytzBnLtbm6tJWjfHiBuqlNZ1WcG7HW7wA,708
 matter_observability/metrics/labeled_metric.py,sha256=Qn4psWuJJTyALay8-wU0vK2Y0epp25JWPSoZ8BQK8hM,421
 matter_observability/metrics/utils.py,sha256=TTe2pIfrr8R9F9_YNex9Klr_akQ_Ej-FUHEsNWjDwg0,903
-matter_observability-1.3.1.dist-info/METADATA,sha256=yGVL4QcFRxo6fI108Yr_V_8_cQRpKdfsnaDN7iI_M-U,5852
-matter_observability-1.3.1.dist-info/WHEEL,sha256=EI2JsGydwUL5GP9t6kzZv7G3HDPi7FuZDDf9In6amRM,87
-matter_observability-1.3.1.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_observability-1.3.1.dist-info/RECORD,,
+matter_observability-1.3.2.dist-info/METADATA,sha256=5ShYErRlzlh3LDNqgrOmT9d5JypUwI-5eSuNzAo2Lt8,5852
+matter_observability-1.3.2.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+matter_observability-1.3.2.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_observability-1.3.2.dist-info/RECORD,,
```

