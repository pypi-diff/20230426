# Comparing `tmp/easybio-0.1.0.tar.gz` & `tmp/easybio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easybio-0.1.0.tar", last modified: Sat Apr 22 17:45:52 2023, max compression
+gzip compressed data, was "easybio-0.3.1.tar", last modified: Wed Apr 26 08:00:24 2023, max compression
```

## Comparing `easybio-0.1.0.tar` & `easybio-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-22 17:45:52.355439 easybio-0.1.0/
--rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-22 17:45:52.351439 easybio-0.1.0/PKG-INFO
--rwxrwxr-x   0 lei       (1003) lei       (1004)       30 2023-04-21 05:50:43.000000 easybio-0.1.0/README.md
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-22 17:45:52.351439 easybio-0.1.0/easyBio/
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-22 17:45:52.351439 easybio-0.1.0/easyBio/Utils/
--rw-rw-r--   0 lei       (1003) lei       (1004)      289 2023-04-22 11:24:17.000000 easybio-0.1.0/easyBio/Utils/__init__.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     8089 2023-04-22 12:59:53.000000 easybio-0.1.0/easyBio/Utils/download.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     3661 2023-04-22 11:27:45.000000 easybio-0.1.0/easyBio/Utils/downloadUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     3305 2023-04-22 13:35:03.000000 easybio-0.1.0/easyBio/Utils/easyBioUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     2045 2023-04-21 18:02:00.000000 easybio-0.1.0/easyBio/Utils/netUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1044 2023-04-21 15:56:59.000000 easybio-0.1.0/easyBio/Utils/toolsUtils.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      245 2023-04-22 12:33:23.000000 easybio-0.1.0/easyBio/__init__.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1247 2023-04-22 12:35:42.000000 easybio-0.1.0/easyBio/changeNameSRA.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1093 2023-04-22 13:14:40.000000 easybio-0.1.0/easyBio/downloadSRA.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      128 2023-04-21 17:04:20.000000 easybio-0.1.0/easyBio/easyBio.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     3389 2023-04-22 13:36:57.000000 easybio-0.1.0/easyBio/pipline.py
--rw-rw-r--   0 lei       (1003) lei       (1004)      342 2023-04-21 18:11:01.000000 easybio-0.1.0/easyBio/run_cellranger.py
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-21 05:39:47.000000 easybio-0.1.0/easyBio/run_test.py
--rw-rw-r--   0 lei       (1003) lei       (1004)     1473 2023-04-22 13:36:43.000000 easybio-0.1.0/easyBio/splitSRA.py
-drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-22 17:45:52.351439 easybio-0.1.0/easybio.egg-info/
--rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/PKG-INFO
--rw-rw-r--   0 lei       (1003) lei       (1004)      575 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/SOURCES.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/dependency_links.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)      129 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/entry_points.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/not-zip-safe
--rw-rw-r--   0 lei       (1003) lei       (1004)       29 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/requires.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-04-22 17:45:52.000000 easybio-0.1.0/easybio.egg-info/top_level.txt
--rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-22 17:45:52.355439 easybio-0.1.0/setup.cfg
--rw-rw-r--   0 lei       (1003) lei       (1004)     1222 2023-04-22 16:58:18.000000 easybio-0.1.0/setup.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.486647 easybio-0.3.1/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-26 08:00:24.482647 easybio-0.3.1/PKG-INFO
+-rwxrwxr-x   0 lei       (1003) lei       (1004)       30 2023-04-21 05:50:43.000000 easybio-0.3.1/README.md
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easyBio/
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easyBio/Utils/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      337 2023-04-25 14:52:14.000000 easybio-0.3.1/easyBio/Utils/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     8089 2023-04-22 12:59:53.000000 easybio-0.3.1/easyBio/Utils/download.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3640 2023-04-25 14:49:11.000000 easybio-0.3.1/easyBio/Utils/downloadUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     7183 2023-04-26 07:57:47.000000 easybio-0.3.1/easyBio/Utils/easyBioUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2045 2023-04-21 18:02:00.000000 easybio-0.3.1/easyBio/Utils/netUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1044 2023-04-25 14:49:13.000000 easybio-0.3.1/easyBio/Utils/toolsUtils.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      234 2023-04-25 14:49:00.000000 easybio-0.3.1/easyBio/__init__.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     3809 2023-04-24 05:43:51.000000 easybio-0.3.1/easyBio/changeSRAName.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1093 2023-04-22 13:14:40.000000 easybio-0.3.1/easyBio/downloadSRA.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      128 2023-04-21 17:04:20.000000 easybio-0.3.1/easyBio/easyBio.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     2914 2023-04-25 14:54:28.000000 easybio-0.3.1/easyBio/pipline.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)      816 2023-04-24 09:50:20.000000 easybio-0.3.1/easyBio/run_cellranger.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-21 05:39:47.000000 easybio-0.3.1/easyBio/run_test.py
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1490 2023-04-25 14:48:41.000000 easybio-0.3.1/easyBio/splitSRA.py
+drwxrwxr-x   0 lei       (1003) lei       (1004)        0 2023-04-26 08:00:24.482647 easybio-0.3.1/easybio.egg-info/
+-rw-rw-r--   0 lei       (1003) lei       (1004)      536 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/PKG-INFO
+-rw-rw-r--   0 lei       (1003) lei       (1004)      575 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/SOURCES.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/dependency_links.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)      261 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/entry_points.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        1 2023-04-22 17:45:52.000000 easybio-0.3.1/easybio.egg-info/not-zip-safe
+-rw-rw-r--   0 lei       (1003) lei       (1004)       29 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/requires.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)        8 2023-04-26 08:00:24.000000 easybio-0.3.1/easybio.egg-info/top_level.txt
+-rw-rw-r--   0 lei       (1003) lei       (1004)       38 2023-04-26 08:00:24.486647 easybio-0.3.1/setup.cfg
+-rw-rw-r--   0 lei       (1003) lei       (1004)     1393 2023-04-26 08:00:06.000000 easybio-0.3.1/setup.py
```

### Comparing `easybio-0.1.0/PKG-INFO` & `easybio-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.1.0
+Version: 0.3.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.1.0/easyBio/Utils/download.py` & `easybio-0.3.1/easyBio/Utils/download.py`

 * *Files identical despite different names*

### Comparing `easybio-0.1.0/easyBio/Utils/downloadUtils.py` & `easybio-0.3.1/easyBio/Utils/downloadUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import math
 import os
 from .netUtils import requestGet
 from .download import Download
-from .toolsUtils import createDir
 
 
 def getbioproject(gsenumber):
     """
     This function retrieves the BioProject identifier for a given GSE number.
     The BioProject identifier is a unique identifier assigned to a biological project in the NCBI BioProject database.
 
@@ -54,16 +53,16 @@
     print("\033[1;33m{}\033[0m".format("*" * 80))   # 黄
     threads = min(50, math.ceil(threads / 2))
     bioproject = getbioproject(gsenumber)
     pjurl = f"https://www.ebi.ac.uk/ena/portal/api/filereport?result=read_run&accession={bioproject}&offset=0&limit=1000&format=json&fields=study_accession,secondary_study_accession,sample_accession,secondary_sample_accession,experiment_accession,run_accession,submission_accession,tax_id,scientific_name,instrument_platform,instrument_model,library_name,nominal_length,library_layout,library_strategy,library_source,library_selection,read_count,base_count,center_name,first_public,last_updated,experiment_title,study_title,study_alias,experiment_alias,run_alias,fastq_bytes,fastq_md5,fastq_ftp,fastq_aspera,fastq_galaxy,submitted_bytes,submitted_md5,submitted_ftp,submitted_aspera,submitted_galaxy,submitted_format,sra_bytes,sra_md5,sra_ftp,sra_aspera,sra_galaxy,cram_index_ftp,cram_index_aspera,cram_index_galaxy,sample_alias,broker_name,sample_title,nominal_sdev,first_created"
     pjre = requestGet(pjurl)
     results = pjre.json()
     filedirs = f"{dirs}/{gsenumber}/raw/sra"
-    createDir(filedirs)
-    
+    os.makedirs(filedirs, exist_ok=True)
+
     if idDownloadAll(results, filedirs):
         print("\033[32mAll files have been successfully downloaded. Exiting or entering the fastq-dump program...\033[0m")
         return True
     
     for study in results:
         run_accession = study["run_accession"]
         print("\033[33mrun_accession: {}\033[0m".format(run_accession))
```

### Comparing `easybio-0.1.0/easyBio/Utils/netUtils.py` & `easybio-0.3.1/easyBio/Utils/netUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.1.0/easyBio/Utils/toolsUtils.py` & `easybio-0.3.1/easyBio/Utils/toolsUtils.py`

 * *Files identical despite different names*

### Comparing `easybio-0.1.0/easyBio/downloadSRA.py` & `easybio-0.3.1/easyBio/downloadSRA.py`

 * *Files identical despite different names*

### Comparing `easybio-0.1.0/easyBio/splitSRA.py` & `easybio-0.3.1/easyBio/splitSRA.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,13 +30,13 @@
     
     print("\033[1;32m GSE folder:\033[0m \033[32m{}\033[0m".format(folder))
     print("\033[1;32m outdir:\033[0m \033[32m{}\033[0m".format(outdir))
     print("\033[1;32m threads:\033[0m \033[32m{}\033[0m".format(threads))
     print("\033[1;32m kind:\033[0m \033[32m{}\033[0m".format(kind))
 
     # Create output directory if it doesn't exist
-    createDir(outdir)
+    os.makedirs(outdir, exist_ok=True)
     splitSRAfun(folder, outdir, threads, kind)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `easybio-0.1.0/easybio.egg-info/PKG-INFO` & `easybio-0.3.1/easybio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easybio
-Version: 0.1.0
+Version: 0.3.1
 Summary: The purpose of the creation of this package is to make bioinformatics analysis simpler.
 Home-page: https://github.com/xleizi/easyBio_conda
 Author: Lei Cui
 Author-email: cuilei798@qq.com
 Maintainer: Lei Cui
 Maintainer-email: cuilei798@qq.com
 License: MIT License
```

### Comparing `easybio-0.1.0/easybio.egg-info/SOURCES.txt` & `easybio-0.3.1/easybio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 README.md
 setup.py
 easyBio/__init__.py
-easyBio/changeNameSRA.py
+easyBio/changeSRAName.py
 easyBio/downloadSRA.py
 easyBio/easyBio.py
 easyBio/pipline.py
 easyBio/run_cellranger.py
 easyBio/run_test.py
 easyBio/splitSRA.py
 easyBio/Utils/__init__.py
```

### Comparing `easybio-0.1.0/setup.py` & `easybio-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.3.1'
 
 setup(
     name='easybio',  # package name
     version=VERSION,  # package version
     author='Lei Cui',
     author_email='cuilei798@qq.com',
     maintainer='Lei Cui',
@@ -19,14 +19,17 @@
     packages=find_packages(),
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'easyBio=easyBio.easyBio:main',
             'easydownloadSRA=easyBio.downloadSRA:main',
             'easysplitSRA=easyBio.splitSRA:main',
+            'easychangeSRAName=easyBio.changeSRAName:main',
+            'easycellranger=easyBio.run_cellranger:main',
+            'easyscGEOpipline=easyBio.pipline:main',
         ]
     },
     install_requires=[
         # 'biopython',
         'threadpool',
         'requests',
         'argparse'
```

