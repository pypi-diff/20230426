# Comparing `tmp/iqmma-0.1.3-py3-none-any.whl.zip` & `tmp/iqmma-0.1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 28808 bytes, number of entries: 10
+Zip file size: 29002 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Feb-26 14:17 iqmma/__init__.py
 -rw-r--r--  2.0 unx     1051 b- defN 23-Feb-26 14:17 iqmma/default.ini
--rw-r--r--  2.0 unx    38208 b- defN 23-Mar-17 14:45 iqmma/iqmma.py
--rw-r--r--  2.0 unx    42290 b- defN 23-Mar-07 14:07 iqmma/utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    11848 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      759 b- defN 23-Mar-17 14:50 iqmma-0.1.3.dist-info/RECORD
-10 files, 105653 bytes uncompressed, 27528 bytes compressed:  73.9%
+-rw-r--r--  2.0 unx    38425 b- defN 23-Apr-25 12:41 iqmma/iqmma.py
+-rw-r--r--  2.0 unx    42493 b- defN 23-Apr-25 13:34 iqmma/utils.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12164 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      771 b- defN 23-Apr-25 16:27 iqmma-0.1.3.1.dist-info/RECORD
+10 files, 106401 bytes uncompressed, 27698 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: iqmma/iqmma.py
 Comment: 
 
 Filename: iqmma/utils.py
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/LICENSE
+Filename: iqmma-0.1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/METADATA
+Filename: iqmma-0.1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/WHEEL
+Filename: iqmma-0.1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/entry_points.txt
+Filename: iqmma-0.1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/top_level.txt
+Filename: iqmma-0.1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: iqmma-0.1.3.dist-info/RECORD
+Filename: iqmma-0.1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iqmma/iqmma.py

```diff
@@ -59,15 +59,15 @@
     parser.add_argument('-logs', nargs='?', help='level of logging, (DEBUG, INFO, WARNING, ERROR, CRITICAL)', type=str, default='INFO', const='INFO', choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL', 'NOTSET', 'debug', 'info', 'warning', 'error', 'critical', 'nonset'])
     parser.add_argument('-log_path', nargs='?', help='path to logging file', type=str, default='./iqmma.log', const='./iqmma.log')
     parser.add_argument('-cfg', nargs='?', help='path to config .ini file', type=str, default='', const='')
     parser.add_argument('-cfg_category', nargs='?', help='name of category to prioritize in the .ini file, default: DEFAULT', type=str, default='DEFAULT', const='DEFAULT')
     parser.add_argument('-example_cfg', nargs='?', help='Path to create example config .ini file or not if not stated', type=str, default='', const='')
     parser.add_argument('-dif', nargs='?', help='path to Diffacto', type=str, default='', const='')
 #    parser.add_argument('-scav2dif', help='path to scav2diffacto')
-    parser.add_argument('-s1', nargs='+', help='input mzML files for sample 1 (also file names are the keys for searching other needed files)', type=str, default='', )
+    parser.add_argument('-s1', nargs='*', help='input mzML files for sample 1 (also file names are the keys for searching other needed files)', type=str, default='', )
     parser.add_argument('-s2', nargs='*', help='input mzML files for sample 2 (also file names are the keys for searching other needed files)', type=str, default='', )
 #    parser.add_argument('-sampleNames', nargs='+', help='short names for samples for inner structure of results')
     parser.add_argument('-psm_folder', nargs='?', help='path to the folder with PSMs files', type=str, default='', const='')
     parser.add_argument('-psm_format', nargs='?', help='format or suffix to search PSMs files (may be PSMs_full.tsv or identipy.pep.xml for example)', type=str, default='PSMs_full.tsv', const='PSMs_full.tsv')
     parser.add_argument('-pept_folder', nargs='?', help='path to folder with files (filename starts with the name of .mzML and ends with peptides.tsv) with peptides filtered on certain FDR (default: searching for them near PSMs)', type=str, default='', const='')
     parser.add_argument('-prot_folder', nargs='?', help='path to folder with files (filename starts with the name of .mzML and ends with proteins.tsv) with proteins filtered on certain FDR (default: searching for them near PSMs)', type=str, default='', const='')
     
@@ -124,15 +124,14 @@
     
     args = default_config
     if users_config :
         for k in users_keys :
             args.update({k: users_config[k]})
     for k in console_keys :
         args.update({k: console_config[k]})
-        
     
     loglevel = args['logs'].upper()
     numeric_level = getattr(logging, loglevel, None)
     if not isinstance(numeric_level, int):
         raise ValueError('Invalid log level: %s' % loglevel)
 
     logger = logging.getLogger('logger')
@@ -166,14 +165,18 @@
             return 0
         else :
             logger.warning('Invalid path for example cfg creation. Directory does not exist')
             return 1
     
     logger.debug(args)
     
+    if not args['s1'] :
+        logger.critical('At least one file in the argument is needed: -s1 {}'.format(args['s1']))
+        raise ValueError('At least one file in the argument is needed: -s1 {}'.format(args['s1']))
+    
     mode = None
     if not args['s2'] :
         sample_nums = ['s1']
         logger.info('mode = feature matching')
         mode = 'feature matching'
     else :
         sample_nums = ['s1', 's2']
```

## iqmma/utils.py

```diff
@@ -44,39 +44,42 @@
                 key = key_value[0]
                 value = None
             keys.append(key)
             key = '-' + key
             final.append(key)
 
             if value :
-                if not value.startswith('"') or not value.startswith("'") :
+                if value.startswith('\"') or value.startswith("\'") :
+                    final.append(value)
+                else :
                     vals = value.split()
                     for v in vals :
                         final.append(v)
-                else :
-                    final.append(value)
     return final, keys
 
 
 def write_example_cfg(path, dct_args):
     with open(path, 'w') as f :
         f.write('#encoding=\'utf-8\'\n')
         f.write('[DEFAULT]\n')
         for k, v in dct_args.items() :
             if type(v) != list :
-                f.write(k + ' = ' + str(v) + '\n')
+                if type(v) == str and v.startswith('-') :
+                    f.write(k + ' = ' + '\"' + str(v) + '\"' + '\n')
+                else :
+                    f.write(k + ' = ' + str(v) + '\n')
             else :
                 f.write(k + ' = ' + ' '.join([str(el) for el in v]) + '\n')
         f.write('\n[users_category]\n')
         f.write('# here you can set your parameters\n')
 
 
 def call_Dinosaur(path_to_fd, mzml_path, outdir, outname, str_of_other_args, logger = logging.getLogger('function') ) :
     if str_of_other_args :
-        other_args = ['--' + x.strip().replace(' ', '=') for x in str_of_other_args.strip('"').split('--')]
+        other_args = ['--' + x.strip().replace(' ', '=') for x in str_of_other_args.strip('"').strip("'").split('--')]
     else :
         other_args = []
     if path_to_fd.lower().endswith('jar') :
         final_args = ['java', '-jar', path_to_fd, mzml_path, '--outDir='+outdir, '--outName='+outname, ] + other_args
     else :
         final_args = [path_to_fd, mzml_path, '--outDir='+outdir, '--outName='+outname, ] + other_args
     final_args = list(filter(lambda x: False if x=='--' else True, final_args))
@@ -87,30 +90,30 @@
         log_subprocess_output(process.stdout, logger=logger)
     exitscore = process.wait()
     os.rename(os.path.join(outdir, outname + '.features.tsv'),  os.path.join(outdir, outname) )
     return exitscore
 
 def call_Biosaur2(path_to_fd, mzml_path, outpath, str_of_other_args, logger = logging.getLogger('function')) :
     if str_of_other_args :
-        other_args = [x.strip() for x in str_of_other_args.strip('"').split(' ')]
+        other_args = [x.strip() for x in str_of_other_args.strip('"').strip("'").split(' ')]
     else :
         other_args = []
     final_args = [path_to_fd, mzml_path, '-o', outpath, ] + other_args
     final_args = list(filter(lambda x: False if x=='' else True, final_args))
     process = subprocess.Popen(final_args, 
                                stdout=subprocess.PIPE, 
                                stderr=subprocess.STDOUT)
     with process.stdout:
         log_subprocess_output(process.stdout, logger=logger)
     exitscore = process.wait()
     return exitscore
 
 def call_OpenMS(path_to_fd, mzml_path, outpath, str_of_other_args, logger = logging.getLogger('function')) :
     if str_of_other_args :
-        other_args = [x.strip() for x in str_of_other_args.strip('"').split(' ')]
+        other_args = [x.strip() for x in str_of_other_args.strip('"').strip("'").split(' ')]
     else :
         other_args = []
     final_args = [path_to_fd, 
                   '-in', mzml_path, 
                   '-out', outpath, 
                   ] + other_args
     final_args = list(filter(lambda x: False if x=='' else True, final_args))
@@ -277,15 +280,15 @@
         for sample in samples_dict[sample_num] :
             label = sample
             out.write(label + '\t' + sample_num + '\n')
             logger.info(label + '\t' + sample_num)
     out.close()
     logger.info('DONE')
     
-    other_args = [x.strip() for x in str_of_other_args.split(' ')]
+    other_args = [x.strip() for x in str_of_other_args.strip("'").strip('"').split(' ')]
     final_args = [diffacto_path, 
                   '-i', peptide_path, 
                   '-out', out_path, 
                   '-samples', sample_path, ] + ['-min_samples', min_samples] + other_args
     final_args = list(filter(lambda x: False if x=='' else True, final_args))
     final_args = [str(x) for x in final_args]
     logger.info('Diffacto START')
```

## Comparing `iqmma-0.1.3.dist-info/LICENSE` & `iqmma-0.1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `iqmma-0.1.3.dist-info/METADATA` & `iqmma-0.1.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iqmma
-Version: 0.1.3
+Version: 0.1.3.1
 Summary: A MS1 feature mapping for MS2 spectra identifications.
 Author: Valeriy Postoenko & Leyla Garibova
 Author-email: pyteomics@googlegroups.com
 License: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
@@ -64,27 +64,33 @@
 
 ### Advanced example
 
 Full quantitation mode (Linux-based example):
 
     iqmma -bio2 /usr/bin/biosaur2 -dino /home/user/downloads/Dinosaur-1.2.0.free.jar -dif /usr/bin/diffacto -s1 /home/user/downloads/sample1_rep1.mzml /home/user/downloads/sample1_rep2.mzml -s2 /home/user/downloads/sample2_rep1.mzml /home/user/downloads/sample2_rep2.mzml -logs INFO -log_path /home/user/iqmma_logs/logs_N.log -mbr 1 -overwrite_matching 1 -mixed 1 -fc_threshold 2.5 -pval_threshold 0.01
     
-Here, two samples with two replicas per sample compared against each other in quantitation mode. `-psm_folder` and `-psm_format` are not specified so `iqmma` will search peptide identifications in folder `/home/user/downloads` (near .mzml default for `-psm_folder`) by searching files which names start for example with `sample1_rep1` (and other names of .mzml files) and end with `PSMs_full.tsv` (default value of `-psm_format`, for Scavager results). More than one feature detection is available so by default mixed algorithm would also be turned on (`-mixed 1` is default). `-mbr 1` turns on match between runs, so matching needs to be overwritten not to use old files without matching between runs. `-logs` and `-log_path` specify level of logging messages and where to store them. `-fc_threshold 2.5` and `-pval_threshold 0.01` specifies thresholds on Fold Change and p-value to apply to differentially expressed proteins in final filtering.
+Here, two samples with two replicas per sample compared against each other in quantitation mode. At least two replicas per sample are needed for statistical tests in Diffacto to work, without it Diffato output would be empty and quantitation wouldn't work. `-psm_folder` and `-psm_format` are not specified so `iqmma` will search peptide identifications in folder `/home/user/downloads` (near .mzml default for `-psm_folder`) by searching files which names start for example with `sample1_rep1` (and other names of .mzml files) and end with `PSMs_full.tsv` (default value of `-psm_format`, for Scavager results). More than one feature detection is available so by default mixed algorithm would also be turned on (`-mixed 1` is default). `-mbr 1` turns on match between runs, so matching needs to be overwritten not to use old files without matching between runs. `-logs` and `-log_path` specify level of logging messages and where to store them. `-fc_threshold 2.5` and `-pval_threshold 0.01` specifies thresholds on Fold Change and p-value to apply to differentially expressed proteins in final filtering.
 
 Matching mode (Anaconda, Windows paths):
     
     iqmma -dino c:\user\downloads\dinosaur-1.2.0.free.jar -bio2 c:\user\anaconda3\scripts\biosaur2.exe -dif c:\user\Anaconda3\Scripts\diffacto.exe -s1 c:\user\downloads\sample1_rep1.mzml c:\user\downloads\sample2_rep1.mzml -outdir c:\user\iqmma_analysis\out_1 -logs info -log_path  c:\user\iqmma_analysis\out_1\logs.log -psm_folder c:\user\downloads\mzid_peptides -psm_format .mzid 
 
 Here there are two samples in one replica each to match on peptides identifications that are stored in files `-psm_folder` + `\` + (.mzml filename) + `-psm_format` which results in `c:\user\downloads\mzid_peptides\` + `sample1_rep1` + `.mzid`. Two feature detections are given (paths to executable files are given), so there would be two rows of matched files in the `-outdir` in the end: Dinosaur-generated features matched (ends with `_dino.tsv`) on peptides and Biosaur2-generated (ends with `_bio2.tsv`) features matched on peptides.
 
 Full quantitation mode with peptides and proteins filtering (Linux-based example):
 
     iqmma -bio2 /usr/bin/biosaur2 -dino /home/user/downloads/Dinosaur-1.2.0.free.jar -dif /usr/bin/diffacto -s1 /home/user/downloads/sample1_rep1.mzml /home/user/downloads/sample1_rep2.mzml -s2 /home/user/downloads/sample2_rep1.mzml /home/user/downloads/sample2_rep2.mzml -logs INFO -log_path /home/user/iqmma_logs/logs_N.log -prot_folder /home/user/downloads/post_search -pept_folder /home/user/downloads/post_search
 
-Here, same samples, as in the first example, but user made additional post search analysis and received files (for example as in Scavager: one per .mzML file) with peptides and proteins filtered at 1% FDR, for example. `-pept_folder` parameters allow to point directories where `iqmma` could find that files to use only 1%FDR peptides in quantitation. If `-pept_folder` parameter is applied, `iqmma` will try to find all files which name starts with the name of one of .mzML files and ends with `peptides.tsv` (here these names would be like `sample1_rep1*peptides.tsv`) then read from that file only the column (`peptide`) with peptide sequences and join all peptides from all files that were found in one set, and then only peptides from that set will be allowed to quantification. `-prot_folder` parameter behaves similarly with column name `dbname` and filename suffix `proteins.tsv`. So, for custom usage, one file (like `/home/user/downloads/post_search/sample1_rep1*peptides.tsv`) with all needed peptides is enough.
+Here, same samples, as in the first example, but user made additional post search analysis and received files (for example as in Scavager: one per .mzML file) with peptides and proteins filtered at 1% FDR, for example. `-pept_folder` parameters allow to point directories where `iqmma` could find that files to use only 1%FDR peptides in quantitation. If `-pept_folder` parameter is applied, `iqmma` will try to find all files which name starts with the name of one of .mzML files and ends with `peptides.tsv` (here these names would be like `sample1_rep1*peptides.tsv`) then read from that file only the column (`peptide`) with peptide sequences and join all peptides from all files that were found in one set, and then only peptides from that set will be allowed to quantification. `-prot_folder` parameter behaves similarly with column name `dbname` and filename suffix `proteins.tsv`. So, for custom usage, one file (like `/home/user/downloads/post_search/sample1_rep1*peptides.tsv`) with all needed peptides is enough. Example structure where `\n` :
+
+    /home/user/downloads/post_search/sample1_rep1*peptides.tsv file:
+    peptide\n
+    AAABBBCCC\n
+    AABBBDDD\n
+    ...
 
 Note 1: Paths to feature detections or Diffacto should be paths to its executable files. In Linux-based systems, executable files are usually stored in `/usr/bin/`; on Windows with Anaconda - in `C:\User\Anaconda3\Scripts` or `C:\User\Anaconda3\envs\current_environment\Scripts`.
 
 Note 2: To use Dinosaur, java should be installed in the environment.
 
 Note 3: Since Windows has a case-insensitive file system, despite `iqmma`'s overall compatibility some options related to other used programs (`-diffacto_args`, `-dino_args` to be precise) could not work properly according to Diffacto and Dinosaur case-sensitive option's names. With that fact in mind, it is recommended to use `iqmma` on Linux-based system.
```

