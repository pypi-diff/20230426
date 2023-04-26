# Comparing `tmp/hance-1.0.5-py3-none-win_amd64.whl.zip` & `tmp/hance-1.0.6-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 8919974 bytes, number of entries: 11
+Zip file size: 8919980 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      304 b- defN 23-Feb-27 13:47 hance/__init__.py
 -rw-r--r--  2.0 unx     8676 b- defN 23-Feb-28 13:15 hance/hance.py
--rw-r--r--  2.0 unx     3495 b- defN 23-Feb-28 16:45 hance/hance_file.py
--rw-r--r--  2.0 unx       21 b- defN 23-Apr-25 17:45 hance/version.py
+-rw-r--r--  2.0 unx     3502 b- defN 23-Apr-25 18:20 hance/hance_file.py
+-rw-r--r--  2.0 unx       21 b- defN 23-Apr-25 18:21 hance/version.py
 -rw-rw-r--  2.0 unx  5592576 b- defN 23-Apr-23 14:46 hance/bin/Windows_x64/HanceEngine.dll
 -rw-rw-r--  2.0 unx  3753426 b- defN 23-Apr-23 14:46 hance/models/speech-denoise.hance
 -rw-rw-r--  2.0 unx  3753426 b- defN 23-Apr-23 14:46 hance/models/speech-dereverb.hance
--rw-r--r--  2.0 unx     5933 b- defN 23-Apr-25 17:45 hance-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       98 b- defN 23-Apr-25 17:45 hance-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-25 17:45 hance-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      864 b- defN 23-Apr-25 17:45 hance-1.0.5.dist-info/RECORD
-11 files, 13118825 bytes uncompressed, 8918536 bytes compressed:  32.0%
+-rw-r--r--  2.0 unx     5933 b- defN 23-Apr-25 18:21 hance-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       98 b- defN 23-Apr-25 18:21 hance-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-25 18:21 hance-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      864 b- defN 23-Apr-25 18:21 hance-1.0.6.dist-info/RECORD
+11 files, 13118832 bytes uncompressed, 8918542 bytes compressed:  32.0%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: hance/models/speech-denoise.hance
 Comment: 
 
 Filename: hance/models/speech-dereverb.hance
 Comment: 
 
-Filename: hance-1.0.5.dist-info/METADATA
+Filename: hance-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: hance-1.0.5.dist-info/WHEEL
+Filename: hance-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: hance-1.0.5.dist-info/top_level.txt
+Filename: hance-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hance-1.0.5.dist-info/RECORD
+Filename: hance-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hance/hance_file.py

```diff
@@ -64,19 +64,21 @@
         audio_out = processor.process(silent_audio)
         if len (audio_out) > in_file_info.frames - num_of_samples_written:
             audio_out = audio_out[0:in_file_info.frames - num_of_samples_written,:]
             output_file.write(audio_out)
         num_of_samples_written += len(audio_out)
     """
 
+    
+
     #Rewritten to support older versions of pysoundfile,
     #which doesn't have the in_file_info.frames attribute.
     silent_audio = np.zeros([block_size, in_file_info.channels])
     num_of_samples = len(in_file_info) // in_file_info.channels
-    num_of_samples_written = 0
+    #num_of_samples_written = 0
 
     while num_of_samples_written < num_of_samples:
         remaining_samples = num_of_samples - num_of_samples_written
         samples_to_process = min(block_size, remaining_samples)
         audio_out = processor.process(silent_audio[:samples_to_process])
         
         output_file.write(audio_out)
```

## hance/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

## Comparing `hance-1.0.5.dist-info/METADATA` & `hance-1.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hance
-Version: 1.0.5
+Version: 1.0.6
 Summary: The Python API to the HANCE engine, which offers realtime audio enhancement.
 Home-page: https://hance.ai
 Author: HANCE
 Author-email: HANCE <mail@hance.ai>
 Project-URL: Homepage, https://hance.ai
 Keywords: hance,audio enhancement,noise reduction
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `hance-1.0.5.dist-info/RECORD` & `hance-1.0.6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 hance/__init__.py,sha256=2Ku1H1PqCYx5YP8lyaC5iYmcdNUuJC-B8UNTvKQdAFU,304
 hance/hance.py,sha256=h9-br4WzizzhGKL7yVDVpONlIw5mgLeF2D0vNcdkGZ0,8676
-hance/hance_file.py,sha256=zimv0abzKPT9r-7aJ1AW4dqNNr0KnqjkDB5PCyL4MsM,3495
-hance/version.py,sha256=ZR1VA9cGs0vIK6cWK4YKLfBTnmUCAcDaaP9ARPPYxEs,21
+hance/hance_file.py,sha256=8sRPZv8knz9AJXiBn5xTW2Lxh5MIRyOTtmAu7oSY2HU,3502
+hance/version.py,sha256=fCDDAyG3nMZcE_hvt1RHdxkiFN3DfNSyU_k-rLUDrpE,21
 hance/bin/Windows_x64/HanceEngine.dll,sha256=sNQoL6TVXeRcBz1JBWjtIUOXsL1ejuTF3WT0VJ_O1JM,5592576
 hance/models/speech-denoise.hance,sha256=wjcFFdSmz0qMfI_xvLx6-LHphxOGYzaHQe48fHejx54,3753426
 hance/models/speech-dereverb.hance,sha256=7X5tPL_CoBTpAIY1wrlGTrwG4zBgHfWauI5ZhpaUm3A,3753426
-hance-1.0.5.dist-info/METADATA,sha256=I4RIEnJ4y68XmVDGgHPwXbjqFhZxW0VEp1RHMuO6VUI,5933
-hance-1.0.5.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
-hance-1.0.5.dist-info/top_level.txt,sha256=5hVoKN0Oc5C--RMWz-DrSRV0f1Zr-JgP5woqZyNqJEo,6
-hance-1.0.5.dist-info/RECORD,,
+hance-1.0.6.dist-info/METADATA,sha256=egN1dhSjpy8uTo4B_wehXIDS22RX_vv9WzbHG7un73I,5933
+hance-1.0.6.dist-info/WHEEL,sha256=i9qQj8KaD8_YEW0Vc2oS56fKju23RkQ-FVz-QmzVakQ,98
+hance-1.0.6.dist-info/top_level.txt,sha256=5hVoKN0Oc5C--RMWz-DrSRV0f1Zr-JgP5woqZyNqJEo,6
+hance-1.0.6.dist-info/RECORD,,
```

