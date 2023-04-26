# Comparing `tmp/pafts-0.0.0.tar.gz` & `tmp/pafts-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pafts-0.0.0.tar", last modified: Thu Apr 20 15:20:00 2023, max compression
+gzip compressed data, was "pafts-0.0.1.tar", last modified: Wed Apr 26 06:20:10 2023, max compression
```

## Comparing `pafts-0.0.0.tar` & `pafts-0.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.722805 pafts-0.0.0/
--rw-rw-rw-   0        0        0     1089 2023-03-22 04:46:53.000000 pafts-0.0.0/LICENSE
--rw-rw-rw-   0        0        0     6564 2023-04-20 15:20:00.722805 pafts-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5889 2023-04-20 07:26:52.000000 pafts-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.666727 pafts-0.0.0/pafts/
--rw-rw-rw-   0        0        0       81 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.706819 pafts-0.0.0/pafts/cleaner/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:23:56.000000 pafts-0.0.0/pafts/cleaner/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/cleaner/delete_bgm.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.710808 pafts-0.0.0/pafts/datasets/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:24:13.000000 pafts-0.0.0/pafts/datasets/__init__.py
--rw-rw-rw-   0        0        0     3336 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/datasets/dataset.py
--rw-rw-rw-   0        0        0     7445 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/pafts.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.714805 pafts-0.0.0/pafts/stt/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:24:28.000000 pafts-0.0.0/pafts/stt/__init__.py
--rw-rw-rw-   0        0        0     7585 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/stt/stt_apis.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.718806 pafts-0.0.0/pafts/utils/
--rw-rw-rw-   0        0        0        0 2023-04-18 01:25:00.000000 pafts-0.0.0/pafts/utils/__init__.py
--rw-rw-rw-   0        0        0      756 2023-04-12 05:45:25.000000 pafts-0.0.0/pafts/utils/data_info.py
--rw-rw-rw-   0        0        0     2390 2023-04-18 06:43:10.000000 pafts-0.0.0/pafts/utils/file_utils.py
--rw-rw-rw-   0        0        0     1124 2023-04-20 07:37:11.000000 pafts-0.0.0/pafts/utils/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-20 15:20:00.702838 pafts-0.0.0/pafts.egg-info/
--rw-rw-rw-   0        0        0     6564 2023-04-20 15:20:00.000000 pafts-0.0.0/pafts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-20 15:20:00.000000 pafts-0.0.0/pafts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 15:20:00.000000 pafts-0.0.0/pafts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-04-20 15:20:00.000000 pafts-0.0.0/pafts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 15:20:00.000000 pafts-0.0.0/pafts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 15:20:00.722805 pafts-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1027 2023-04-20 15:08:59.000000 pafts-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.793007 pafts-0.0.1/
+-rw-rw-rw-   0        0        0     1089 2023-03-22 04:46:53.000000 pafts-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0     7594 2023-04-26 06:20:10.793007 pafts-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6745 2023-04-26 01:38:59.000000 pafts-0.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.770069 pafts-0.0.1/pafts/
+-rw-rw-rw-   0        0        0       81 2023-04-20 07:37:11.000000 pafts-0.0.1/pafts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.782037 pafts-0.0.1/pafts/cleaner/
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:23:56.000000 pafts-0.0.1/pafts/cleaner/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-04-25 15:39:40.000000 pafts-0.0.1/pafts/cleaner/delete_bgm.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.784031 pafts-0.0.1/pafts/datasets/
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:24:13.000000 pafts-0.0.1/pafts/datasets/__init__.py
+-rw-rw-rw-   0        0        0     3381 2023-04-23 11:45:33.000000 pafts-0.0.1/pafts/datasets/dataset.py
+-rw-rw-rw-   0        0        0     7811 2023-04-26 01:07:58.000000 pafts-0.0.1/pafts/pafts.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.786026 pafts-0.0.1/pafts/stt/
+-rw-rw-rw-   0        0        0        0 2023-04-18 01:24:28.000000 pafts-0.0.1/pafts/stt/__init__.py
+-rw-rw-rw-   0        0        0     7585 2023-04-20 07:37:11.000000 pafts-0.0.1/pafts/stt/stt_apis.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.791013 pafts-0.0.1/pafts/utils/
+-rw-rw-rw-   0        0        0      101 2023-04-25 14:40:14.000000 pafts-0.0.1/pafts/utils/__init__.py
+-rw-rw-rw-   0        0        0      698 2023-04-25 02:23:29.000000 pafts-0.0.1/pafts/utils/data_info.py
+-rw-rw-rw-   0        0        0     2390 2023-04-18 06:43:10.000000 pafts-0.0.1/pafts/utils/file_utils.py
+-rw-rw-rw-   0        0        0     1597 2023-04-25 07:09:03.000000 pafts-0.0.1/pafts/utils/transform.py
+drwxrwxrwx   0        0        0        0 2023-04-26 06:20:10.780043 pafts-0.0.1/pafts.egg-info/
+-rw-rw-rw-   0        0        0     7594 2023-04-26 06:20:10.000000 pafts-0.0.1/pafts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-26 06:20:10.000000 pafts-0.0.1/pafts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 06:20:10.000000 pafts-0.0.1/pafts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-04-26 06:20:10.000000 pafts-0.0.1/pafts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 06:20:10.000000 pafts-0.0.1/pafts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 06:20:10.794004 pafts-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-04-26 02:20:06.000000 pafts-0.0.1/setup.py
```

### Comparing `pafts-0.0.0/LICENSE` & `pafts-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pafts-0.0.0/PKG-INFO` & `pafts-0.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pafts
-Version: 0.0.0
-Summary: Library That Preprocessing Audio For TTS.
-Home-page: https://github.com/harmlessman/PAFTS
-Author: harmlessman
-Author-email: harmlessman17@gmail.com
-License: MIT License
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PAFTS
 
 ### Library That Preprocessing Audio For TTS.
 
 PAFTS is a library for making Text-to-Speech dataset.
 TTS data basically requires clean audio files and a text file with text corresponding to each audio file. 
 This library makes audio files clean and creates text file with text corresponding to each audio file.
@@ -29,15 +10,15 @@
 ## Description 
 
 PAFTS consist of three main operations.
 1. Transform 
 2. Delete BGM
 3. STT
 
-Transform operations changes the sampling rate(sr), channel, and format of the audio files.
+Transform operation changes the sampling rate(sr), channel, and format of the audio files.
 
 Delete BGM operation removes background music from audio files.
 
 STT operation generates text corresponding to the audio files.
 
 
 ```
@@ -67,52 +48,58 @@
               '1_002.wav' : "I want to eat chicken.",
               '1_003.wav' : "...",
               '1_004.wav' : "...",
               'abc.wav' : "...",   
         }
 ```
 
+
+### Supported Audio Formats
+
+* **wav, mp3, ogg, flac**
+* **Recommend using wav format** because it is much faster in Transform operation and Delete BGM operation.
+* STT operation support **wav, flac** formats.
+
+
 ### Note
+
 * Audio files are not provided. Please prepare your own audio files.
 * Audio files are appropriate to say one or two sentences for 3 to 10 seconds.
 * If the background music is music with lyrics, the background music cannot be removed clearly.
 * Google Web Speech is free, but the quality is low, so if you want high quality, use Google Cloud Speech API or Azure STT API
 
 
 ## Features
 
-
 * Use the [spleeter](https://github.com/deezer/spleeter) to remove background music.
 * In STT, you can use [Google Web Speech](https://wicg.github.io/speech-api/), [Google Cloud Speech](https://cloud.google.com/speech-to-text) and [Azure STT](https://azure.microsoft.com/products/cognitive-services/speech-to-text/).
 * If you use Google Cloud Speech API or Azure STT API, you need API key.
-* ****❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.****
-* ****❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.****
+* **❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.**
+* **❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.**
+* **❗❗ We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.**
 
 ## Requirements
 
-
 * python >= 3.8
 * spleeter
 * pydub
 * SpeechRecognition
 * tqdm
 
 
 
 ## Installation
 
-
 ```
 pip install pafts
 ```
 
 
 ## Usage
 
-
 * Quick start:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language')
     pafts.run()
     
   
@@ -124,57 +111,61 @@
     )
     pafts.run()
   
   
   
   
     >> Run...
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    > Transform items...
-    | > sr : 22050
-    | > channel : 1
-    | > format : wav
-    
-    > Delete BGM...
-    | > Number of items : 5
-    | > Path : C:\Users\82109\Desktop\dataset
-    abc.wav: 100%|██████████| 5/5 [00:13<00:00,  2.62s/it]
-    | > Number of Success items : 5
-    | > Number of failure items : 0
-    
-    > Preparing STT API...
-    | > STT API : google web speech
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    abc.wav: 100%|██████████| 5/5 [00:11<00:00,  2.27s/it]
-
-    | > Numbers of deleted files : 0
-    Saved at C:\Users\82109\Desktop\dataset\text.json
-    Successfully Completed.
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  > Transform items...
+  | > format : wav
+  | > sr : 22050
+  | > channel : 1
+  change_format: 100%|██████████| 5/5 [00:00<00:00, 337.68it/s]
+  change_sr: 100%|██████████| 5/5 [00:00<00:00, 141.79it/s]
+  change_channel: 100%|██████████| 5/5 [00:00<00:00, 166.22it/s]
+          
+  > Delete BGM...
+  | > Number of items : 5
+  | > Path : C:\Users\82109\Desktop\dataset
+  abc.wav: 100%|██████████| 5/5 [00:08<00:00,  1.65s/it]
+  | > Number of Success items : 5
+  | > Number of failure items : 0
+  
+  > Preparing STT API...
+  | > STT API : google web speech
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  abc.wav: 100%|██████████| 5/5 [00:10<00:00,  2.02s/it]
+  
+  | > Numbers of deleted files : 0
+  Saved at C:\Users\82109\Desktop\dataset\text.json
+  Successfully Completed.
+
     ```
   
     'dataset_path' is your audio files path.
     'language' is BCP 47 tag.
     You can add a detailed option to the argument of run(). Please refer to the document of the run() for more information.
 
 
 * If you want to task step by step:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language', dataset_name='dataset name', key_path='api key path')
-    pafts.transform_items(sr=22050, channel=1, formats='audio format')
+    pafts.transform_items(formats='audio format', sr=22050, channel=1)
     pafts.delete_bgm()
     dic = pafts.stt(stt_api_name='stt api name')
     pafts.save(dic=dic, output_name='text.json')
     ```
 
 * If you want to make key file:
     ```
@@ -228,11 +219,18 @@
             ├── b_1.wav
             ├── b_2.wav
             ├── 1.wav
             ├── 2.wav
             └── c_d_1.wav
     ```
 
+## License
+
+The code of **PAFTS** is [MIT-licensed](LICENSE)
+
 
+## Disclaimer
 
+We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.
 
+You agree that you use [PAFTS](https://github.com/harmlessman/PAFTS) at your own risk.
```

### Comparing `pafts-0.0.0/README.md` & `pafts-0.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: pafts
+Version: 0.0.1
+Summary: Library That Preprocessing Audio For TTS.
+Home-page: https://github.com/harmlessman/PAFTS
+Author: harmlessman
+Author-email: harmlessman17@gmail.com
+License: MIT License
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PAFTS
 
 ### Library That Preprocessing Audio For TTS.
 
 PAFTS is a library for making Text-to-Speech dataset.
 TTS data basically requires clean audio files and a text file with text corresponding to each audio file. 
 This library makes audio files clean and creates text file with text corresponding to each audio file.
@@ -10,15 +32,15 @@
 ## Description 
 
 PAFTS consist of three main operations.
 1. Transform 
 2. Delete BGM
 3. STT
 
-Transform operations changes the sampling rate(sr), channel, and format of the audio files.
+Transform operation changes the sampling rate(sr), channel, and format of the audio files.
 
 Delete BGM operation removes background music from audio files.
 
 STT operation generates text corresponding to the audio files.
 
 
 ```
@@ -48,52 +70,58 @@
               '1_002.wav' : "I want to eat chicken.",
               '1_003.wav' : "...",
               '1_004.wav' : "...",
               'abc.wav' : "...",   
         }
 ```
 
+
+### Supported Audio Formats
+
+* **wav, mp3, ogg, flac**
+* **Recommend using wav format** because it is much faster in Transform operation and Delete BGM operation.
+* STT operation support **wav, flac** formats.
+
+
 ### Note
+
 * Audio files are not provided. Please prepare your own audio files.
 * Audio files are appropriate to say one or two sentences for 3 to 10 seconds.
 * If the background music is music with lyrics, the background music cannot be removed clearly.
 * Google Web Speech is free, but the quality is low, so if you want high quality, use Google Cloud Speech API or Azure STT API
 
 
 ## Features
 
-
 * Use the [spleeter](https://github.com/deezer/spleeter) to remove background music.
 * In STT, you can use [Google Web Speech](https://wicg.github.io/speech-api/), [Google Cloud Speech](https://cloud.google.com/speech-to-text) and [Azure STT](https://azure.microsoft.com/products/cognitive-services/speech-to-text/).
 * If you use Google Cloud Speech API or Azure STT API, you need API key.
-* ****❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.****
-* ****❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.****
+* **❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.**
+* **❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.**
+* **❗❗ We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.**
 
 ## Requirements
 
-
 * python >= 3.8
 * spleeter
 * pydub
 * SpeechRecognition
 * tqdm
 
 
 
 ## Installation
 
-
 ```
 pip install pafts
 ```
 
 
 ## Usage
 
-
 * Quick start:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language')
     pafts.run()
     
   
@@ -105,57 +133,61 @@
     )
     pafts.run()
   
   
   
   
     >> Run...
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    > Transform items...
-    | > sr : 22050
-    | > channel : 1
-    | > format : wav
-    
-    > Delete BGM...
-    | > Number of items : 5
-    | > Path : C:\Users\82109\Desktop\dataset
-    abc.wav: 100%|██████████| 5/5 [00:13<00:00,  2.62s/it]
-    | > Number of Success items : 5
-    | > Number of failure items : 0
-    
-    > Preparing STT API...
-    | > STT API : google web speech
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    abc.wav: 100%|██████████| 5/5 [00:11<00:00,  2.27s/it]
-
-    | > Numbers of deleted files : 0
-    Saved at C:\Users\82109\Desktop\dataset\text.json
-    Successfully Completed.
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  > Transform items...
+  | > format : wav
+  | > sr : 22050
+  | > channel : 1
+  change_format: 100%|██████████| 5/5 [00:00<00:00, 337.68it/s]
+  change_sr: 100%|██████████| 5/5 [00:00<00:00, 141.79it/s]
+  change_channel: 100%|██████████| 5/5 [00:00<00:00, 166.22it/s]
+          
+  > Delete BGM...
+  | > Number of items : 5
+  | > Path : C:\Users\82109\Desktop\dataset
+  abc.wav: 100%|██████████| 5/5 [00:08<00:00,  1.65s/it]
+  | > Number of Success items : 5
+  | > Number of failure items : 0
+  
+  > Preparing STT API...
+  | > STT API : google web speech
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  abc.wav: 100%|██████████| 5/5 [00:10<00:00,  2.02s/it]
+  
+  | > Numbers of deleted files : 0
+  Saved at C:\Users\82109\Desktop\dataset\text.json
+  Successfully Completed.
+
     ```
   
     'dataset_path' is your audio files path.
     'language' is BCP 47 tag.
     You can add a detailed option to the argument of run(). Please refer to the document of the run() for more information.
 
 
 * If you want to task step by step:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language', dataset_name='dataset name', key_path='api key path')
-    pafts.transform_items(sr=22050, channel=1, formats='audio format')
+    pafts.transform_items(formats='audio format', sr=22050, channel=1)
     pafts.delete_bgm()
     dic = pafts.stt(stt_api_name='stt api name')
     pafts.save(dic=dic, output_name='text.json')
     ```
 
 * If you want to make key file:
     ```
@@ -209,11 +241,18 @@
             ├── b_1.wav
             ├── b_2.wav
             ├── 1.wav
             ├── 2.wav
             └── c_d_1.wav
     ```
 
+## License
+
+The code of **PAFTS** is [MIT-licensed](LICENSE)
+
 
+## Disclaimer
 
+We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.
 
+You agree that you use [PAFTS](https://github.com/harmlessman/PAFTS) at your own risk.
```

### Comparing `pafts-0.0.0/pafts/cleaner/delete_bgm.py` & `pafts-0.0.1/pafts/cleaner/delete_bgm.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,53 +8,58 @@
 
 from pafts.datasets.dataset import Dataset
 
 logger.setLevel(logging.WARNING)
 logging.getLogger('tensorflow').setLevel(logging.CRITICAL)
 
 
-def delete_bgm(dataset: Dataset):
+def delete_bgm(dataset: Dataset, multiprocess: bool = False):
     """
     Remove BGM from the audio file and save audio file as a same file name.
     Please note that the original file will be deleted.
 
     Spleeter library was used to remove the BGM.
 
     Args:
         dataset (Dataset): Dataset.
+        multiprocess (bool): Multiprocessing Delete BGM. Defaults to False.
     """
 
     freeze_support()
 
     print(f'> Delete BGM...')
     print(f'| > Number of items : {dataset.get_file_num()}')
     print(f'| > Path : {dataset.path}')
 
     items = dataset.get_audio_file()
 
-    separator = Separator('spleeter:2stems')
-    accompaniment = Path('accompaniment.wav')
-    vocal = Path('vocals.wav')
+    separator = Separator('spleeter:2stems', multiprocess=multiprocess)
 
     bar = tqdm(items,
                total=len(items),
                desc='spleeter_progress',
                leave=True,
                )
 
     success = 0
     failure = []
 
     for item in bar:
+        formats = item.suffix
+
+        accompaniment = Path('accompaniment').with_suffix(formats)
+        vocal = Path('vocals').with_suffix(formats)
+
         bar.set_description(item.name)
         try:
             separator.separate_to_file(
                 str(item),
                 str(dataset.path),
-                filename_format='{instrument}.{codec}'
+                filename_format='{instrument}.{codec}',
+                codec=formats[1:],
             )
             success += 1
 
         except:
             failure.append(item)
             continue
```

### Comparing `pafts-0.0.0/pafts/datasets/dataset.py` & `pafts-0.0.1/pafts/datasets/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+import datetime
 
 from pafts.utils.data_info import is_audio, get_duration
 from pafts.utils.file_utils import rmtree
 
 
 class Dataset:
     """
@@ -108,9 +109,9 @@
             rmtree(d)
 
     def print_info(self):
         print(f'| > Dataset name : {self.dataset_name}')
         print(f'| > Path : {self.path}')
         print(f'| > language : {self.language}')
         print(f'| > Number of files : {self.get_file_num()}')
-        print(f'| > Total duration : {self.get_total_duration()}')
+        print(f'| > Total duration : {datetime.timedelta(seconds=self.get_total_duration())}')
         print()
```

### Comparing `pafts-0.0.0/pafts/pafts.py` & `pafts-0.0.1/pafts/pafts.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             >>> from pafts.pafts import PAFTS
             >>> pafts = PAFTS(dataset_path="your dataset path", language='language')
             >>> pafts.run()
 
         If you want to task step by step:
             >>> from pafts.pafts import PAFTS
             >>> pafts = PAFTS(dataset_path="your dataset path", language='language', dataset_name='dataset name', key_path='api key path')
-            >>> pafts.transform_items(sr=22050, channel=1, formats='audio format')
+            >>> pafts.transform_items(formats='audio format', sr=22050, channel=1)
             >>> pafts.delete_bgm()
             >>> dic = pafts.stt(stt_api_name='stt api name')
             >>> pafts.save(dic=dic, file_name='text.json')
 
         """
 
     def __init__(
@@ -52,37 +52,40 @@
 
     def flatten(self):
         """Flatten directory structure."""
         print(f'> Flatten directory structure.')
         print()
         self.dataset.flatten()
 
-    def transform_items(self, sr: int = 22050, channel: int = 1, formats: str = 'wav'):
+    def transform_items(self, formats: str = 'wav', sr: int = 22050, channel: int = 1):
         """
-        Change sampling rate, channel, format
+        Change format, sampling rate, channel
 
         Args:
+            formats (str, optional): Audio file's format. Defaults to 'wav'.
             sr (int, optional): Audio file's sampling rate. Defaults to 22050.
             channel (int, optional): Audio file's channel. Defaults to 1.
-            formats (str, optional): Audio file's format. Defaults to 'wav'.
         """
 
-        print(f'> Transform items...')
-        print(f'| > sr : {sr}')
-        print(f'| > channel : {channel}')
-        print(f'| > format : {formats}')
+        print(f'> Transform items...\n| > format : {formats}\n| > sr : {sr}\n| > channel : {channel}')
+
+        change_format(self.dataset, formats=formats)
         change_sr(self.dataset, sr=sr)
         change_channel(self.dataset, channel=channel)
-        change_format(self.dataset, formats=formats)
         print()
 
-    def delete_bgm(self):
-        """Delete BGM from audio file"""
+    def delete_bgm(self, multiprocess: bool = False):
+        """
+        Delete BGM from audio file
 
-        delete_bgm(self.dataset)
+        Args:
+            multiprocess (bool): Multiprocessing Delete BGM. Defaults to False.
+        """
+
+        delete_bgm(self.dataset, multiprocess=multiprocess)
 
     def stt(self, stt_api_name: str = 'google_web_speech', abs_path: bool = False):
         """
         Get text values for audio files using STT API and Return key-value pairs.
 
         Args:
             stt_api_name (str, optional): Name of the api to use. Defaults to 'google_web_speech'.
@@ -133,29 +136,33 @@
             raise Exception('[!] Audio file does not exist.')
 
         if stt_api_name not in STT_API_LIST:
             raise Exception(
                 '[!] Unsupported api. Please choose one of these.\n google_web_speech, azure_stt, google_cloud_stt')
 
         if stt_api_name != 'google_web_speech':
-            if not Path(self.key_path).exists() or not self.key_path:
+            if not self.key_path:
+                raise Exception('[!] Key path does not exist!')
+
+            if not Path(self.key_path).exists():
                 raise Exception('[!] Key path is not correct!')
 
             with open(self.key_path, 'r', encoding="utf-8") as f:
                 key = json.load(f)
 
             if stt_api_name not in key or not key[stt_api_name]:
                 raise Exception(f'[!] The api key for {stt_api_name} does not exist!')
 
     def run(
             self,
             flat: bool = False,
+            formats: str = 'wav',
             sr: int = 22050,
             channel: int = 1,
-            formats: str = 'wav',
+            multiprocess: bool = False,
             stt_api_name: str = 'google_web_speech',
             file_name: str = 'text.json',
             delete_none: bool = True
 
     ):
         """
         Make audio files into a dataset for TTS.
@@ -164,33 +171,33 @@
             1. Transform items.
             2. Delete BGM.
             3. STT. (Create audio and text pairs)
             4. Save dict.
 
         Args:
             flat (bool, optional): Flatten directory structure. Defaults to False.
+            formats (str, optional): Audio file's format. Defaults to 'wav'.
             sr (int, optional): Audio file's sampling rate. Defaults to 22050.
             channel (int, optional): Audio file's channel. Defaults to 1.
-            formats (str, optional): Audio file's format. Defaults to 'wav'.
+            multiprocess (bool): Multiprocessing Delete BGM. Defaults to False.
             stt_api_name (str, optional): Name of the speech to text api to use. Defaults to 'google_web_speech'.
             file_name (str, optional): Output text file name. Defaults to 'text.json'.
             delete_none (bool, optional): Delete the none value of the dic. Defaults to True.
-
         """
         print('>> Run...')
 
         self.dataset.print_info()
 
         self.check_args(stt_api_name)
 
         if flat:
             self.flatten()
 
-        self.transform_items(sr, channel, formats)
+        self.transform_items(formats=formats, sr=sr, channel=channel)
 
-        self.delete_bgm()
+        self.delete_bgm(multiprocess=multiprocess)
 
         dic = self.stt(stt_api_name=stt_api_name)
 
         self.save(dic=dic, file_name=file_name, delete_none=delete_none)
 
         print('Successfully Completed.')
```

### Comparing `pafts-0.0.0/pafts/stt/stt_apis.py` & `pafts-0.0.1/pafts/stt/stt_apis.py`

 * *Files identical despite different names*

### Comparing `pafts-0.0.0/pafts/utils/data_info.py` & `pafts-0.0.1/pafts/utils/data_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,16 @@
 
 from pydub import AudioSegment
 from pathlib import Path
-
-AUDIO_FILE_EXT = [
-    'wav',
-    'mp3',
-    'raw',
-    'pcm',
-    'mp4',
-    'mkv'
-]
+from pafts.utils import AUDIO_FORMATS
 
 
 def is_audio(path):
     file = Path(path)
-    if file.suffix[1:] in AUDIO_FILE_EXT:
+    if file.suffix[1:] in AUDIO_FORMATS:
         return True
     return False
 
 
 def get_duration(path):
     audio = AudioSegment.from_file(path)
     return audio.duration_seconds
```

### Comparing `pafts-0.0.0/pafts/utils/file_utils.py` & `pafts-0.0.1/pafts/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `pafts-0.0.0/pafts.egg-info/PKG-INFO` & `pafts-0.0.1/pafts.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: pafts
-Version: 0.0.0
+Version: 0.0.1
 Summary: Library That Preprocessing Audio For TTS.
 Home-page: https://github.com/harmlessman/PAFTS
 Author: harmlessman
 Author-email: harmlessman17@gmail.com
 License: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
@@ -29,15 +32,15 @@
 ## Description 
 
 PAFTS consist of three main operations.
 1. Transform 
 2. Delete BGM
 3. STT
 
-Transform operations changes the sampling rate(sr), channel, and format of the audio files.
+Transform operation changes the sampling rate(sr), channel, and format of the audio files.
 
 Delete BGM operation removes background music from audio files.
 
 STT operation generates text corresponding to the audio files.
 
 
 ```
@@ -67,52 +70,58 @@
               '1_002.wav' : "I want to eat chicken.",
               '1_003.wav' : "...",
               '1_004.wav' : "...",
               'abc.wav' : "...",   
         }
 ```
 
+
+### Supported Audio Formats
+
+* **wav, mp3, ogg, flac**
+* **Recommend using wav format** because it is much faster in Transform operation and Delete BGM operation.
+* STT operation support **wav, flac** formats.
+
+
 ### Note
+
 * Audio files are not provided. Please prepare your own audio files.
 * Audio files are appropriate to say one or two sentences for 3 to 10 seconds.
 * If the background music is music with lyrics, the background music cannot be removed clearly.
 * Google Web Speech is free, but the quality is low, so if you want high quality, use Google Cloud Speech API or Azure STT API
 
 
 ## Features
 
-
 * Use the [spleeter](https://github.com/deezer/spleeter) to remove background music.
 * In STT, you can use [Google Web Speech](https://wicg.github.io/speech-api/), [Google Cloud Speech](https://cloud.google.com/speech-to-text) and [Azure STT](https://azure.microsoft.com/products/cognitive-services/speech-to-text/).
 * If you use Google Cloud Speech API or Azure STT API, you need API key.
-* ****❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.****
-* ****❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.****
+* **❗ The audio files may be modified or changed during the Transform process and Delete BGM process, so please back up the original audio files.**
+* **❗ Google Cloud Speech API and Azure STT API will be charged if they exceed the free usage, so please check the price options carefully.**
+* **❗❗ We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.**
 
 ## Requirements
 
-
 * python >= 3.8
 * spleeter
 * pydub
 * SpeechRecognition
 * tqdm
 
 
 
 ## Installation
 
-
 ```
 pip install pafts
 ```
 
 
 ## Usage
 
-
 * Quick start:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language')
     pafts.run()
     
   
@@ -124,57 +133,61 @@
     )
     pafts.run()
   
   
   
   
     >> Run...
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    > Transform items...
-    | > sr : 22050
-    | > channel : 1
-    | > format : wav
-    
-    > Delete BGM...
-    | > Number of items : 5
-    | > Path : C:\Users\82109\Desktop\dataset
-    abc.wav: 100%|██████████| 5/5 [00:13<00:00,  2.62s/it]
-    | > Number of Success items : 5
-    | > Number of failure items : 0
-    
-    > Preparing STT API...
-    | > STT API : google web speech
-    | > Dataset name : dataset
-    | > Path : C:\Users\82109\Desktop\dataset
-    | > language : en-us
-    | > Number of files : 5
-    | > Total duration : 14.760000000000002
-    
-    abc.wav: 100%|██████████| 5/5 [00:11<00:00,  2.27s/it]
-
-    | > Numbers of deleted files : 0
-    Saved at C:\Users\82109\Desktop\dataset\text.json
-    Successfully Completed.
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  > Transform items...
+  | > format : wav
+  | > sr : 22050
+  | > channel : 1
+  change_format: 100%|██████████| 5/5 [00:00<00:00, 337.68it/s]
+  change_sr: 100%|██████████| 5/5 [00:00<00:00, 141.79it/s]
+  change_channel: 100%|██████████| 5/5 [00:00<00:00, 166.22it/s]
+          
+  > Delete BGM...
+  | > Number of items : 5
+  | > Path : C:\Users\82109\Desktop\dataset
+  abc.wav: 100%|██████████| 5/5 [00:08<00:00,  1.65s/it]
+  | > Number of Success items : 5
+  | > Number of failure items : 0
+  
+  > Preparing STT API...
+  | > STT API : google web speech
+  | > Dataset name : dataset
+  | > Path : C:\Users\82109\Desktop\dataset
+  | > language : en-us
+  | > Number of files : 5
+  | > Total duration : 0:00:14.760000
+  
+  abc.wav: 100%|██████████| 5/5 [00:10<00:00,  2.02s/it]
+  
+  | > Numbers of deleted files : 0
+  Saved at C:\Users\82109\Desktop\dataset\text.json
+  Successfully Completed.
+
     ```
   
     'dataset_path' is your audio files path.
     'language' is BCP 47 tag.
     You can add a detailed option to the argument of run(). Please refer to the document of the run() for more information.
 
 
 * If you want to task step by step:
     ```
     from pafts import PAFTS
     pafts = PAFTS(dataset_path="your dataset path", language='language', dataset_name='dataset name', key_path='api key path')
-    pafts.transform_items(sr=22050, channel=1, formats='audio format')
+    pafts.transform_items(formats='audio format', sr=22050, channel=1)
     pafts.delete_bgm()
     dic = pafts.stt(stt_api_name='stt api name')
     pafts.save(dic=dic, output_name='text.json')
     ```
 
 * If you want to make key file:
     ```
@@ -228,11 +241,18 @@
             ├── b_1.wav
             ├── b_2.wav
             ├── 1.wav
             ├── 2.wav
             └── c_d_1.wav
     ```
 
+## License
+
+The code of **PAFTS** is [MIT-licensed](LICENSE)
+
 
+## Disclaimer
 
+We are not responsible for the transformation of audio files due to the use of PAFTS or the payment of fees due to the use of STT API.
 
+You agree that you use [PAFTS](https://github.com/harmlessman/PAFTS) at your own risk.
```

### Comparing `pafts-0.0.0/setup.py` & `pafts-0.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,31 @@
     readme = f.read()
 
 with open("requirements.txt", 'r', encoding='utf-8') as f:
     requirements = f.read()
 
 setup(
     name='pafts',
-    version='0.0.0',
+    version='0.0.1',
     author='harmlessman',
     author_email="harmlessman17@gmail.com",
     description='Library That Preprocessing Audio For TTS.',
     install_requires=requirements,
     license='MIT License',
     long_description=readme,
     long_description_content_type="text/markdown",
     url='https://github.com/harmlessman/PAFTS',
     python_requires=">=3.8, <3.11",
     packages=find_packages(),
     classifiers=[
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ]
```

