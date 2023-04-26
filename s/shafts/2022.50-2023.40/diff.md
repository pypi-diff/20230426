# Comparing `tmp/shafts-2022.50-py3-none-any.whl.zip` & `tmp/shafts-2023.40-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,29 +1,32 @@
-Zip file size: 77847 bytes, number of entries: 27
--rw-rw-rw-  2.0 fat    44503 b- defN 22-May-30 12:23 shafts/DL_dataset.py
--rw-rw-rw-  2.0 fat    65236 b- defN 22-May-30 12:23 shafts/DL_model.py
--rw-rw-rw-  2.0 fat    11973 b- defN 22-May-30 12:23 shafts/DL_module.py
--rw-rw-rw-  2.0 fat    52669 b- defN 22-May-30 12:23 shafts/DL_train.py
--rw-rw-rw-  2.0 fat      167 b- defN 22-May-30 12:23 shafts/__init__.py
--rw-rw-rw-  2.0 fat      120 b- defN 22-May-30 12:23 shafts/_env.py
--rw-rw-rw-  2.0 fat    31478 b- defN 22-May-30 12:23 shafts/dataset.py
--rw-rw-rw-  2.0 fat    80396 b- defN 22-May-30 12:23 shafts/inference.py
--rw-rw-rw-  2.0 fat    19131 b- defN 22-May-30 12:23 shafts/mathexpr.py
--rw-rw-rw-  2.0 fat    10683 b- defN 22-May-30 12:23 shafts/model.py
--rw-rw-rw-  2.0 fat      101 b- defN 22-May-30 12:23 shafts/shaft_version.json
--rw-rw-rw-  2.0 fat    48480 b- defN 22-May-30 12:23 shafts/train.py
--rw-rw-rw-  2.0 fat     9132 b- defN 22-May-30 12:23 shafts/testCase/test_shaft.py
--rw-rw-rw-  2.0 fat     2334 b- defN 22-May-30 12:23 shafts/utils/GEE_Download_2021.csv
--rw-rw-rw-  2.0 fat      199 b- defN 22-May-30 12:23 shafts/utils/GEE_Download_2021_case.csv
--rw-rw-rw-  2.0 fat    23607 b- defN 22-May-30 12:23 shafts/utils/GEE_ops.py
--rw-rw-rw-  2.0 fat     3330 b- defN 22-May-30 12:23 shafts/utils/HeightGen.csv
--rw-rw-rw-  2.0 fat     2155 b- defN 22-May-30 12:23 shafts/utils/HeightGen_back.csv
--rw-rw-rw-  2.0 fat      187 b- defN 22-May-30 12:23 shafts/utils/README.md
--rw-rw-rw-  2.0 fat      401 b- defN 22-May-30 12:23 shafts/utils/__init__.py
--rw-rw-rw-  2.0 fat      341 b- defN 22-May-30 12:23 shafts/utils/ee_download.sh
--rw-rw-rw-  2.0 fat    42992 b- defN 22-May-30 12:23 shafts/utils/gdal_ops.py
--rw-rw-rw-  2.0 fat    41918 b- defN 22-May-30 12:23 shafts/utils/postprocessing.py
--rw-rw-rw-  2.0 fat     1228 b- defN 22-May-30 12:35 shafts-2022.50.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-May-30 12:35 shafts-2022.50.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 22-May-30 12:35 shafts-2022.50.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2142 b- defN 22-May-30 12:35 shafts-2022.50.dist-info/RECORD
-27 files, 495002 bytes uncompressed, 74459 bytes compressed:  85.0%
+Zip file size: 94081 bytes, number of entries: 30
+-rw-rw-rw-  2.0 fat    44587 b- defN 23-Apr-25 22:08 shafts/DL_dataset.py
+-rw-rw-rw-  2.0 fat    64176 b- defN 23-Apr-25 22:08 shafts/DL_model.py
+-rw-rw-rw-  2.0 fat    50518 b- defN 23-Apr-25 22:08 shafts/DL_model_tf.py
+-rw-rw-rw-  2.0 fat    11973 b- defN 23-Apr-25 22:08 shafts/DL_module.py
+-rw-rw-rw-  2.0 fat    52669 b- defN 23-Apr-25 22:08 shafts/DL_train.py
+-rw-rw-rw-  2.0 fat      224 b- defN 23-Apr-25 22:08 shafts/__init__.py
+-rw-rw-rw-  2.0 fat      120 b- defN 23-Apr-25 22:08 shafts/_env.py
+-rw-rw-rw-  2.0 fat    31478 b- defN 23-Apr-25 22:08 shafts/dataset.py
+-rw-rw-rw-  2.0 fat    80396 b- defN 23-Apr-25 22:08 shafts/inference.py
+-rw-rw-rw-  2.0 fat    38962 b- defN 23-Apr-25 22:08 shafts/inference_gcloud.py
+-rw-rw-rw-  2.0 fat    19131 b- defN 23-Apr-25 22:08 shafts/mathexpr.py
+-rw-rw-rw-  2.0 fat    10683 b- defN 23-Apr-25 22:08 shafts/model.py
+-rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-25 22:08 shafts/shaft_version.json
+-rw-rw-rw-  2.0 fat    48480 b- defN 23-Apr-25 22:08 shafts/train.py
+-rw-rw-rw-  2.0 fat     9132 b- defN 23-Apr-25 22:08 shafts/testCase/test_shaft.py
+-rw-rw-rw-  2.0 fat     2334 b- defN 23-Apr-25 22:08 shafts/utils/GEE_Download_2021.csv
+-rw-rw-rw-  2.0 fat      199 b- defN 23-Apr-25 22:08 shafts/utils/GEE_Download_2021_case.csv
+-rw-rw-rw-  2.0 fat    23607 b- defN 23-Apr-25 22:08 shafts/utils/GEE_ops.py
+-rw-rw-rw-  2.0 fat     3330 b- defN 23-Apr-25 22:08 shafts/utils/HeightGen.csv
+-rw-rw-rw-  2.0 fat     2155 b- defN 23-Apr-25 22:08 shafts/utils/HeightGen_back.csv
+-rw-rw-rw-  2.0 fat      187 b- defN 23-Apr-25 22:08 shafts/utils/README.md
+-rw-rw-rw-  2.0 fat      495 b- defN 23-Apr-25 22:08 shafts/utils/__init__.py
+-rw-rw-rw-  2.0 fat      341 b- defN 23-Apr-25 22:08 shafts/utils/ee_download.sh
+-rw-rw-rw-  2.0 fat     3529 b- defN 23-Apr-25 22:08 shafts/utils/ee_ops.py
+-rw-rw-rw-  2.0 fat    42992 b- defN 23-Apr-25 22:08 shafts/utils/gdal_ops.py
+-rw-rw-rw-  2.0 fat    41918 b- defN 23-Apr-25 22:08 shafts/utils/postprocessing.py
+-rw-rw-rw-  2.0 fat     1329 b- defN 23-Apr-25 22:24 shafts-2023.40.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 22:24 shafts-2023.40.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-25 22:24 shafts-2023.40.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2384 b- defN 23-Apr-25 22:24 shafts-2023.40.dist-info/RECORD
+30 files, 587529 bytes uncompressed, 90327 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: shafts/DL_dataset.py
 Comment: 
 
 Filename: shafts/DL_model.py
 Comment: 
 
+Filename: shafts/DL_model_tf.py
+Comment: 
+
 Filename: shafts/DL_module.py
 Comment: 
 
 Filename: shafts/DL_train.py
 Comment: 
 
 Filename: shafts/__init__.py
@@ -18,14 +21,17 @@
 
 Filename: shafts/dataset.py
 Comment: 
 
 Filename: shafts/inference.py
 Comment: 
 
+Filename: shafts/inference_gcloud.py
+Comment: 
+
 Filename: shafts/mathexpr.py
 Comment: 
 
 Filename: shafts/model.py
 Comment: 
 
 Filename: shafts/shaft_version.json
@@ -57,26 +63,29 @@
 
 Filename: shafts/utils/__init__.py
 Comment: 
 
 Filename: shafts/utils/ee_download.sh
 Comment: 
 
+Filename: shafts/utils/ee_ops.py
+Comment: 
+
 Filename: shafts/utils/gdal_ops.py
 Comment: 
 
 Filename: shafts/utils/postprocessing.py
 Comment: 
 
-Filename: shafts-2022.50.dist-info/METADATA
+Filename: shafts-2023.40.dist-info/METADATA
 Comment: 
 
-Filename: shafts-2022.50.dist-info/WHEEL
+Filename: shafts-2023.40.dist-info/WHEEL
 Comment: 
 
-Filename: shafts-2022.50.dist-info/top_level.txt
+Filename: shafts-2023.40.dist-info/top_level.txt
 Comment: 
 
-Filename: shafts-2022.50.dist-info/RECORD
+Filename: shafts-2023.40.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shafts/DL_dataset.py

```diff
@@ -253,15 +253,15 @@
                 s1_vh_patch = gray_scale_data_transforms["valid"](image=s1_vh_coef_patch.astype(np.uint8))["image"]
                 s2_rgb_patch = rgb_scale_data_transforms["valid"](image=s2_rgb_patch.astype(np.uint8))["image"]
                 s2_nir_patch = gray_scale_data_transforms["valid"](image=s2_nir_patch.astype(np.uint8))["image"]
                 patch = np.concatenate([s1_vv_patch, s1_vh_patch, s2_rgb_patch, s2_nir_patch], axis=-1)
             else:
                 raise NotImplementedError
 
-            # ---------convert numpy.ndarray of shape [H, W, C] to torch.tensor [C, H, W]
+            # ---------convert numpy.ndarray of shape [H, W, C] in the range [0, 255] to torch.tensor [C, H, W] in the range [0, 1]
             patch = tensor_transform(patch).type(torch.FloatTensor)
 
             patch_multi_band.append(patch)
 
         feat = torch.cat(patch_multi_band, dim=0)
 
         # ------get target information
@@ -382,15 +382,15 @@
                 s1_vh_patch = gray_scale_data_transforms["valid"](image=s1_vh_coef_patch.astype(np.uint8))["image"]
                 s2_rgb_patch = rgb_scale_data_transforms["valid"](image=s2_rgb_patch.astype(np.uint8))["image"]
                 s2_nir_patch = gray_scale_data_transforms["valid"](image=s2_nir_patch.astype(np.uint8))["image"]
                 patch = np.concatenate([s1_vv_patch, s1_vh_patch, s2_rgb_patch, s2_nir_patch], axis=-1)
             else:
                 raise NotImplementedError
 
-            # ---------convert numpy.ndarray of shape [H, W, C] to torch.tensor [C, H, W]
+            # ---------convert numpy.ndarray of shape [H, W, C] in the range [0, 255] to torch.tensor [C, H, W] in the range [0, 1]
             patch = tensor_transform(patch).type(torch.FloatTensor)
 
             patch_multi_band.append(patch)
 
         feat = torch.cat(patch_multi_band, dim=0)
 
         # ------get target information
```

## shafts/DL_model.py

```diff
@@ -1458,35 +1458,13 @@
     total_num = sum(p.numel() for p in model.parameters())
     trainable_num = sum(p.numel() for p in model.parameters() if p.requires_grad)
     print("Total parameter of CBAMResNetMTL: ", total_num, " Trainable parameter of CBAMResNetMTL: ", trainable_num)
     return model
 
 
 if __name__ == "__main__":
-    #pretrained_weight = os.path.join("DL_run", "res_file", "check_pt_cbam_100m", "experiment_2", "checkpoint.pth.tar")
-
-    # m = model_ResNet(in_plane=64, input_channels=6, input_size=30, num_block=4)
-    # m = model_ResNet_aux(in_plane=64, input_channels=6, input_size=30, aux_input_size=30, num_block=1, num_aux=1)
-    # m = model_ResNetMTL(in_plane=64, input_channels=6, input_size=30, num_block=4)
     m = model_ResNetMTL_aux(in_plane=64, input_channels=6, input_size=30, aux_input_size=30, num_block=1, num_aux=1)
-    # m = model_SEResNet(in_plane=64, input_channels=6, input_size=15, num_block=4, trained_record=pretrained_weight)
-    # m = model_CBAMResNet(in_plane=64, input_channels=6, input_size=60, num_block=3, trained_record=pretrained_weight)
-
     m.eval()
     '''
     for name, param in m.state_dict().items():
         print(name)
-    '''
-
-    test_dta = torch.ones(8, 6, 120, 120)
-
-    test_aux = torch.ones(8, 1, 120, 120) * 2
-    test_aux[1] = test_aux[1] * 2
-    test_aux[2] = test_aux[2] * 4
-    test_aux[4] = test_aux[4] * 8
-
-    # test_out = m(test_dta)
-    # test_out = m(test_dta, test_aux)
-    # test_out, test_out_b = m(test_dta)
-    test_out, test_out_b = m(test_dta, test_aux)
-    print(test_out)
-    print(test_out_b)
+    '''
```

## shafts/__init__.py

```diff
@@ -1,8 +1,12 @@
 from . import utils
 
 from .inference import (
     pred_height_from_tiff_DL_patch,
-    pred_height_from_tiff_DL_patch_MTL
+    pred_height_from_tiff_DL_patch_MTL,
+)
+
+from .inference_gcloud import (
+    GBuildingMap
 )
 
 from ._env import _path_shaft_module
```

## shafts/shaft_version.json

### Pretty-printed

 * *Similarity: 0.625%*

 * *Differences: {"'ver_major'": '4', "'ver_milestone'": '2023', "'ver_minor'": '25'}*

```diff
@@ -1,6 +1,6 @@
 {
-    "ver_major": 5,
-    "ver_milestone": 2022,
-    "ver_minor": 30,
+    "ver_major": 4,
+    "ver_milestone": 2023,
+    "ver_minor": 25,
     "ver_remark": ".0"
 }
```

## shafts/utils/__init__.py

```diff
@@ -12,8 +12,13 @@
 from .GEE_ops import (
     srtm_download_by_extent,
     srtm_download,
     sentinel1_download_by_extent,
     sentinel1_download,
     sentinel2_download_by_extent,
     sentinel2_download
+)
+
+from .ee_ops import (
+    add_cloud_shadow_mask_infer,
+    computeQualityScore_infer,
 )
```

## Comparing `shafts-2022.50.dist-info/RECORD` & `shafts-2023.40.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-shafts/DL_dataset.py,sha256=7HOFAhm2HKTnAhlFbHStX23Z9zh8rMrEjozEkg1B7Cg,44503
-shafts/DL_model.py,sha256=bPMa3pUcb1FgcD8kqWwv07i93RSdpAzOB2Q6inbiU1o,65236
+shafts/DL_dataset.py,sha256=OSkxOpUuqpMW7Crg-b2V3ewLT2tsTCjL7SEo5d7wFeg,44587
+shafts/DL_model.py,sha256=DsP38rBCpk0eu9vfmTx0JHyJM-RtqhkcO8Z6I8tj6rk,64176
+shafts/DL_model_tf.py,sha256=N-BJIFKaPJn2vj71829J9bGjunHsgEzWA_b5gFVPM2s,50518
 shafts/DL_module.py,sha256=Ig9qSjhlomJ9DcEv1rmtFp-LcCEbdM-lKnKEmXKZSc8,11973
 shafts/DL_train.py,sha256=L2Pv7GHIK1-Xz_iID2n7jOmehgN63fqRQmHDxL4wmTk,52669
-shafts/__init__.py,sha256=ldASIY6ZENzLrqUIX2b90u9Vo5TMCpjKrfwXYyLaaIA,167
+shafts/__init__.py,sha256=lkeszEf98agltIqBBciR5Fp3cZvBzRGNxQqC56Y04Es,224
 shafts/_env.py,sha256=0bW2mLwIBzvyBZqdfksxGsMZNLvgfKuhuTEDdomAMyw,120
 shafts/dataset.py,sha256=WF0KnRl2wL8ta-p5D_Uf8MeBEvNAhnkAtZsU9T1G0os,31478
 shafts/inference.py,sha256=n19C8oQiOAslpXLkZDlcBVq9Kk7DWEotpXnzH9mCv8Y,80396
+shafts/inference_gcloud.py,sha256=BWz3XsAdJ1Wmp0bigo1m_IYdIlmWo6Z_h-CgKhF2Ipk,38962
 shafts/mathexpr.py,sha256=S0kcWatbVrYSq2ZeIe1LgoSYHcq061zXGIyTfMb5jnk,19131
 shafts/model.py,sha256=yXvv2hvOIggIFYkn6fq_nHzBWfCvtIW0xKiCgfESYvA,10683
-shafts/shaft_version.json,sha256=hf47DSh1jmTenXuxB0FzNcB0LD2yr6aoBxxdvFYzYvo,101
+shafts/shaft_version.json,sha256=4XPPj8DvzPSvsJhmkeY4HG5nNbPdMD18KLVntp8GmYA,101
 shafts/train.py,sha256=mpnEgT4Hpw4McyEMEIycR3mowgGGqIDyJuENZ_3V05M,48480
 shafts/testCase/test_shaft.py,sha256=cfE7aTYn4r-_pf_AJjXDCEyd0af5JssBjta4nzqAWic,9132
 shafts/utils/GEE_Download_2021.csv,sha256=LLVXsLDo_wMRbS2uqjHXdEDxwnWkNs8YcwN4LyJNGzk,2334
 shafts/utils/GEE_Download_2021_case.csv,sha256=ETKgN4juIscUwTtfYhNAcsjmMmB3_kouKUSKJk-cs8c,199
 shafts/utils/GEE_ops.py,sha256=L_7CUAK-mEVJNRFNXOJAhZuU6tfniZToEjPAk4vvXR8,23607
 shafts/utils/HeightGen.csv,sha256=8hvQnZKlFhIz5h2qDmRhOP_8auxC_-mcWJtx6004GRo,3330
 shafts/utils/HeightGen_back.csv,sha256=nWhRtX0kDVY7KWA-DLrLVyWS3kFcxIZ09Ddj6SulRvI,2155
 shafts/utils/README.md,sha256=Tpmi5MU1M6z4uvp30nb8Gy02VZlhsHRnnzk2xFVQH6c,187
-shafts/utils/__init__.py,sha256=eb4BUeoPOVd-599WXpkx4hJt_IJCmdC_a-VAy1q5DR8,401
+shafts/utils/__init__.py,sha256=Zn7E4wMYNEAvuIc7GEcbruN5RML54Yi5ljECMmZzE14,495
 shafts/utils/ee_download.sh,sha256=Jh1C72OV2ckV4YRbZzzIej2Qc7o7IYWs6yKrUBhbiPo,341
+shafts/utils/ee_ops.py,sha256=TNkEgBKK4iLMF8WU7gqipCNoMBHkRbj8B9_VpxSio1Q,3529
 shafts/utils/gdal_ops.py,sha256=NcK75LQBKdDox2Xhbf7vM0pAWdxmEGutnrMGx9pJRL4,42992
 shafts/utils/postprocessing.py,sha256=JcWElqy_j20SscSggNDbXA2hkeKn-5gvmXot2IvmIjY,41918
-shafts-2022.50.dist-info/METADATA,sha256=ilwgqRsuaklY0HDrl4E-NlO14c50Dsb4LTtqxkdqS-0,1228
-shafts-2022.50.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-shafts-2022.50.dist-info/top_level.txt,sha256=ACDrZ2caxqogj_TulbpBjpBkHskgOu-3HHx1wxbEV-U,7
-shafts-2022.50.dist-info/RECORD,,
+shafts-2023.40.dist-info/METADATA,sha256=AjlYxF2YAq3lJFInZnGSpkHcVUf7IamDJbOOAhFZAsw,1329
+shafts-2023.40.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+shafts-2023.40.dist-info/top_level.txt,sha256=ACDrZ2caxqogj_TulbpBjpBkHskgOu-3HHx1wxbEV-U,7
+shafts-2023.40.dist-info/RECORD,,
```

