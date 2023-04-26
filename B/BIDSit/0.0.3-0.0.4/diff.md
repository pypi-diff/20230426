# Comparing `tmp/BIDSit-0.0.3.tar.gz` & `tmp/BIDSit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.3.tar", last modified: Wed Apr 19 23:01:18 2023, max compression
+gzip compressed data, was "BIDSit-0.0.4.tar", last modified: Tue Apr 25 22:30:08 2023, max compression
```

## Comparing `BIDSit-0.0.3.tar` & `BIDSit-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.844223 BIDSit-0.0.3/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-19 23:01:18.843960 BIDSit-0.0.3/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.3/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-19 23:01:18.844320 BIDSit-0.0.3/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2421 2023-04-18 00:01:02.000000 BIDSit-0.0.3/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.838538 BIDSit-0.0.3/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.841817 BIDSit-0.0.3/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)    21664 2023-04-17 22:02:10.000000 BIDSit-0.0.3/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.3/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)    49255 2023-04-18 00:00:52.000000 BIDSit-0.0.3/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-18 00:01:08.000000 BIDSit-0.0.3/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-19 23:01:18.843551 BIDSit-0.0.3/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      276 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       39 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-19 23:01:18.000000 BIDSit-0.0.3/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.945249 BIDSit-0.0.4/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-25 22:30:08.944880 BIDSit-0.0.4/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.4/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-25 22:30:08.945356 BIDSit-0.0.4/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2447 2023-04-25 20:42:57.000000 BIDSit-0.0.4/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.938160 BIDSit-0.0.4/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.941739 BIDSit-0.0.4/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)    25705 2023-04-25 21:38:02.000000 BIDSit-0.0.4/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.4/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-04-19 23:11:33.000000 BIDSit-0.0.4/src/BIDSit/__main__ .py
+-rw-r--r--   0 labmanager   (501) staff       (20)    49871 2023-04-25 22:29:01.000000 BIDSit-0.0.4/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-25 20:54:59.000000 BIDSit-0.0.4/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-25 22:30:08.944275 BIDSit-0.0.4/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      300 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-25 22:30:08.000000 BIDSit-0.0.4/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.3/PKG-INFO` & `BIDSit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BIDSit-0.0.3/README.rst` & `BIDSit-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.3/setup.py` & `BIDSit-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     'Programming Language :: Python :: 3.10',
     'Operating System :: OS Independent',
     'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     
     install_requires=[
         'PySimpleGUI>=4.60.4',
+        'natsort>=8.3.1',
     ],
     extras_require={
         "dev": [
             "pytest>=3.7",
         ],
     },
 )
```

### Comparing `BIDSit-0.0.3/src/BIDSit/Test_script.py` & `BIDSit-0.0.4/src/BIDSit/Test_script.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,96 @@
 
 from BIDSit import *
 path = "/Users/labmanager/Resilience/BIDSit/info"
 import PySimpleGUI as sg
 import re
+import os
+
+import shutil
 #user_info = {'WDIR': '/Users/labmanager/Resilience/temp_data','in_dir': '/Users/labmanager/Resilience/raw', 'dcm2niix': True, 'func_task_num': '1', 'func_scan_num': '2', 'func': {'input_Task-1': 'RS', 'menu_1': 'bold', '0': True, '1': True, 'input_acq Input 1': '', 'list_acq Input 1': [], 'input_ce Input 1': '', 'list_ce Input 1': [], 'input_desc Input 1': '', 'list_desc Input 1': [], 'input_dir Input 1': '', 'list_dir Input 1': [], 'input_echo Input 1': '', 'list_echo Input 1': [], 'input_rec Input 1': '', 'list_rec Input 1': []}, 'anat_task_num': '3', 'anat_scan_num': '3', 'anat': {'menu_1': 'FLAIR', 'menu_2': 'T1w', 'menu_3': 'T2w', '0': True, '1': False, '2': False, '3': False, '4': True, '5': False, '6': False, '7': False, '8': True, 'input_acq Input 1': '', 'list_acq Input 1': [], 'input_acq Input 2': '', 'list_acq Input 2': [], 'input_acq Input 3': '', 'list_acq Input 3': [], 'input_ce Input 1': '', 'list_ce Input 1': [], 'input_ce Input 2': '', 'list_ce Input 2': [], 'input_ce Input 3': '', 'list_ce Input 3': [], 'input_desc Input 1': '', 'list_desc Input 1': [], 'input_desc Input 2': '', 'list_desc Input 2': [], 'input_desc Input 3': '', 'list_desc Input 3': [], 'input_dir Input 1': '', 'list_dir Input 1': [], 'input_dir Input 2': '', 'list_dir Input 2': [], 'input_dir Input 3': '', 'list_dir Input 3': [], 'input_rec Input 1': '', 'list_rec Input 1': [], 'input_rec Input 2': '', 'list_rec Input 2': [], 'input_rec Input 3': '', 'list_rec Input 3': []}, 'fmap_task_num': '2', 'fmap_scan_num': '2', 'fmap': {'menu_1': 'epi (rev-b0)', '-list_1-': ['func task 1'], 'menu_2': 'epi (PA)', '-list_2-': ['func task 1'], '0': True, '1': False, '2': False, '3': True, 'input_acq Input 1': '', 'list_acq Input 1': [], 'input_acq Input 2': '', 'list_acq Input 2': [], 'input_desc Input 1': '', 'list_desc Input 1': [], 'input_desc Input 2': '', 'list_desc Input 2': [], 'rev-b0': 'AP'}, 'exp_name': 'Resilience', 'ses': 'Yes'}
 #variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task','TASK', 'MB']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}}, 'key_words': ['T1','t1','T2','t2','FLAIR','flair','PD','pd','UNIT1','unit1','angio']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}}, 'key_words': ['dwi','DWI', 'dti','DTI', 'hardi','HARDI', 'sbref']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}}, 'key_words': ['rev','REV', 'epi','EPI', 'fieldmap', 'mag','MAG', 'PH', 'ph']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2']}} # ADD DESC
-indir = '/Users/labmanager/Resilience/raw'
-ses = True
-BIDSit = False
-in_dir = '/Users/labmanager/Resilience/parrec/RESILIENCE_02/T2/'
-WDIR = '/Users/labmanager/Resilience'
-WDIR = WDIR + '/tempdata'
-if ses:
-    WDIR = WDIR + '/' + in_dir.split('/')[-3] + '/' + in_dir.split('/')[-2]
-else:
-    WDIR = WDIR + '/' + in_dir.split('/')[-2]
-print(WDIR)
-print(ses)
+def start_gui():
+    info = {}
+    center_column = [[sg.Text("Welcome to BIDSit")]]
+    buttons = [[sg.Button('Go'), sg.Button('Exit')]]
+    content = [
+        [sg.Text("Select the directory containing the subject folders of DICOM or converted NIFTI files:")],
+        [sg.In(enable_events=True, key='-in_dir-'), sg.FolderBrowse('Select'), sg.Push(), sg.Button("info")],
+        [sg.Text("If different from 'rawdata' in the parent directory of above input, select the output directory or name of directory to be created:")],
+        [sg.In(enable_events=True, key='-WDIR-'),sg.FolderBrowse('Select')],
+        [sg.Text("Select processing options below:")],
+        [sg.Checkbox("Convert files to NIFTI", key='-dcm2niix-')],
+        [sg.Checkbox("Put NIFTI into BIDs format", enable_events=True, key='-bids_it-')],
+        [sg.Text("Does your data contain sessions? "), sg.Push(), sg.OptionMenu(['Yes', 'No'], default_value="...", key='-ses-')],
+        [sg.Text("Select the types of files to process below:", visible=False, key='-text-')],
+        [sg.Checkbox("Functional images", key='-func-', visible=False)],
+        [sg.Checkbox("Structural images", key='-anat-', visible=False)],
+        [sg.Checkbox("DTI structural images", key='-dwi-', visible=False)],
+        [sg.Checkbox("fmap images", key='-fmap-', visible=False)],
+        [sg.Checkbox("Perf images", key='-perf-', visible=False)],
+        ]
+    layout = [
+        [sg.Push(), sg.Column(center_column,element_justification='c'), sg.Push()],
+        [sg.Push()],
+        [content],
+        [sg.VPush()],
+        [sg.Push(), sg.Column(buttons,element_justification='c'), sg.Push()],
+        ]
+    window = sg.Window('BIDSit', layout, resizable=True, enable_close_attempted_event=True)
+    while True:
+        event, values = window.read()
+        if event == sg.WIN_CLOSED:
+            break
+        elif event == 'Exit' or event == '-WINDOW CLOSE ATTEMPTED-':
+            exit("User exited BIDSit")
+        elif event == 'info':
+            sg.popup_no_border("Specification of where your subject folders of DICOM or PAR/REC files are found. If no input is specified for the second directory, BIDSit will rename this folder to 'sourcedata' and create 'rawdata' and 'derivatives' folders within the parent directory. Subject folders must contain the numeric values associated with the subject number.")
+        elif event == '-bids_it-':
+            window['-text-'].update(visible=True)
+            window['-func-'].update(visible=True)
+            window['-anat-'].update(visible=True)
+            window['-dwi-'].update(visible=True)
+            window['-fmap-'].update(visible=True)
+#            window['-perf-'].update(visible=True)
+        elif event == 'Go':
+            if not any(values['-in_dir-']) and not any(values['-WDIR-']):
+                sg.popup_no_border("Please specify the directory containing your subject folders")
+                continue
+            if values['-dcm2niix-'] and not any(values['-in_dir-']):
+                sg.popup_no_border("Please specify the directory containing your subject folders for conversion")
+                continue
+            if any(values['-in_dir-']):
+                info['in_dir'] = values['-in_dir-'].split()[0]
+            else:
+                info['in_dir'] = ''
+            if any(values['-WDIR-']):
+                info['out_dir'] = values['-WDIR-'].split()[0]
+#                mkdir(info['out_dir'])
+            else:
+                info['out_dir'] = info['in_dir'].split()[0].rsplit('/', 1)[0]
+#                mkdir(info['out_dir'])
+            info['dcm2niix'] = values['-dcm2niix-']
+            info['bids_it'] = values['-bids_it-']
+            if info['bids_it']:
+                info['copy'] = sg.popup_yes_no(f"Do you want to copy your NIFTI files to a 'sourcedata' folder in {info['out_dir']}")
+            info['func'] = values['-func-']
+            info['anat'] = values['-anat-']
+            info['dwi'] = values['-dwi-']
+            info['fmap'] = values['-fmap-']
+            info['perf'] = values['-perf-']
+            if values['-ses-'] == '...':
+                sg.popup_no_border("Please indicate if your data has mutliple sessions per participant.")
+                continue
+            info['ses'] = values['-ses-']
+            window.close()
+    window.close()
+    return info
+    
+info = start_gui()
+print(info['ses'])
 exit()
 
 
 sub = 'Resilience_01/T2'
 og_sub = sub
 if user_info['ses'] =='Yes':
     sub = 'sub-'+''.join(re.findall(r'\d+',sub.split('/')[0]))+ '_ses-'+''.join(re.findall(r'\d+',sub.split('/')[1]))
```

### Comparing `BIDSit-0.0.3/src/BIDSit/go.py` & `BIDSit-0.0.4/src/BIDSit/go.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import os
 import sys
 import re
 import PySimpleGUI as sg
 from datetime import datetime
 from multiprocessing import Pool
 from itertools import repeat
+from natsort import natsorted
 import filecmp
 import glob
 import shutil
 import json
 import errno
 
 
@@ -60,15 +61,24 @@
         pool.join()
         # - set WDIR to where the new files are - #
         user_info['WDIR'] = WDIR + '/tempdata'
         WDIR = user_info['WDIR']
         
     ### --- sourcedata folder --- ###
     if user_info['copy'] == "Yes":
-        copy_it(WDIR, out_dir + "/sourcedata")
+        if dir_exists(out_dir + "/sourcedata"):
+            dir = listdir(WDIR)
+            der_fld = listdir(out_dir + "/sourcedata")
+            for sub in dir:
+                if sub in der_fld:
+                    continue
+                else:
+                    copy_it(WDIR+'/'+sub, out_dir + "/sourcedata/"+sub)
+        else:
+            copy_it(WDIR, out_dir + "/sourcedata")
     
     ### --- BIDSit --- ###
     if user_info['bids_it']:
         sub_list = listdir(WDIR)
         for entry in sub_list:
             if user_info['ses'] =='Yes':
                 for file in listdir(os.path.join(WDIR,entry)):
@@ -78,34 +88,44 @@
                         else:
                             sub_list.append(os.path.join(entry,file))
             else:
                 if os.path.isdir(os.path.join(WDIR,entry)):
                     continue
                 else:
                     sub_list.remove(entry)
+                    
         # - multiprocessing - #
         pool = Pool() # Create a multiprocessing Pool
-        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # process gets masks
+        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # BIDSit for each participant or time point
         # - Close the pool, keep the kids safe - #
         pool.close()
         pool.join()
         
         ### --- make all the other files --- ###
-        if 'tempdata' in WDIR:
-            WDIR = WDIR.rsplit('/',1)[0]
+        if out_dir != WDIR:
+            WDIR = out_dir
         dir = listdir(WDIR)
         for fld in dir:
             if 'tempdata' in fld:
                 shutil.rmtree(WDIR+'/'+fld)
                 
         # - make derivatives folder - #
         der_dir = f"{WDIR}/derivatives"
         def ignore_files(dir, files):
             return [f for f in files if os.path.isfile(os.path.join(dir, f))]
-        shutil.copytree(WDIR+'/rawdata', der_dir, ignore=ignore_files)
+        if dir_exists(der_dir):
+            dir = listdir(WDIR+'/rawdata')
+            der_fld = listdir(der_dir)
+            for sub in dir:
+                if sub in der_fld:
+                    continue
+                else:
+                    shutil.copytree(WDIR+'/rawdata/'+sub, der_dir+'/'+sub, ignore=ignore_files)
+        else:
+            shutil.copytree(WDIR+'/rawdata', der_dir, ignore=ignore_files)
         
         # - dataset_description.json file - #
         if not os.path.exists(os.path.join(WDIR, "dataset_description.json")):
             dataset_description = {
                 "Name": user_info['exp_name'],
                 "BIDSVersion": "1.6.0",
                 "License": "Your dataset license",
@@ -151,15 +171,14 @@
             }
             with open(WDIR + '/participants.json', 'w') as f:
                 json.dump(data, f, indent=4)
                 print('participants.json file created successfully!')
         else:
             print('participants.json file already exists.')
     else: # when not doing BIDSit, rename tempdata to sourcedata and delete tempdata
-        copy_it(WDIR, out_dir + "/sourcedata")
         WDIR = WDIR.rsplit('/',1)[0]
         dir = listdir(WDIR)
         for fld in dir:
             if 'tempdata' in fld:
                 shutil.rmtree(WDIR+'/'+fld)
     return
     
@@ -330,16 +349,17 @@
                 window[f"-{pro}_tab-"].update(visible=True)
         if event == sg.WIN_CLOSED:
             break
         elif event == 'Exit' or event == '-WINDOW CLOSE ATTEMPTED-':
             exit("User exited BIDSit")
         elif event == 'Load':
             load_info = load_gui()
-            info = {**info, **load_info}
-            window.close()
+            if load_info:
+                info = {**info, **load_info}
+                window.close()
         elif event == '-func_butt-':
             info['func_task_num'] = values['func_task_num']
             info['func_scan_num'] = values['func_scan_num']
             info['func'] = func_butt(values['func_task_num'], values['func_scan_num'])
         elif event == '-anat_butt-':
             info['anat_task_num'] = values['anat_task_num']
             info['anat_scan_num'] = values['anat_scan_num']
@@ -761,29 +781,29 @@
             menu = [menu[i].split(' ')[0] for i in range(task_num)]
         
         # - get endings for files - #
         endings = []
         for i, (key, val) in enumerate(scans.items()):
             for value in val:
                 if 'echo' in value:
-                    endings.append('_'+value)
+                    endings.append(value)
                     val.remove(value)
             if len(endings)-1 != i:
                 endings.append('')
     
         # - Rename files - #
         exts = variables[file_type]['key_words']
         tasksLookedAt=[]
         map_dict = {f"file_type": {'task_ord': task_ord, 'scans': scans}, 'WDIR': WDIR, 'f_sub':f_sub}
         for i in range(scan_num):
             files =[]
             file = ''
             for ext in exts:
                 files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
-            files = sorted([item for sub_list in files for item in sub_list])
+            files = natsorted([item for sub_list in files for item in sub_list])
             if not files:
                 print(f"No {file_type} files were found in {in_dir}/{og_sub}")
                 break
             file_list = []
             for f in files:
                 if 'AX' in f and 'REF' in f:
                     continue
@@ -817,15 +837,16 @@
                 print(f"No files for {og_sub} matching", user_info[file_type][f"menu_{i+1}"])
                 continue
             mkdir(WDIR, f"rawdata/{f_sub}/{file_type}")
             task_cat = task_ord[i] # task number (-1)
             f_type = menu[task_cat] # type of file
             endings[i] = endings[i] + '_' + f_type # adds file type to ending
             fill_it = '_'+'_'.join(scans[f"Scan {i+1}"])
-            
+            if fill_it == '_':
+                fill_it = ''
             # - counting - #
             occur = tasksLookedAt.count(task_cat) # counts occurance of task
             run_num = occur + 1 # run number based on how many times that task occured
             tasksLookedAt.append(task_cat) # add current occurance to task list
             # - naming - #
             if file_type == 'func':
                 task_name = ''.join(task_names[task_cat].split()) # task name
@@ -849,17 +870,14 @@
                     if 'nii.gz' in file:
                         file = file.rsplit('.',2)[0] + ext
                     else:
                         file = file.rsplit('.',1)[0] + ext
                     new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}{ext}" # new name for file
                     os.rename(file, new) # rename file
                     if ext == '.json':
-#                        if file_type == 'fmap':
-#                            json_edit(new, file_type, map_dict, int_dict)
-#                        else:
                         json_edit(new, file_type, map_dict)
         if dir_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}"):
             with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'w') as file:
                 json.dump(file_log, file, indent=4)
         
 # - Edit json files - #
 def json_edit(json_f, file_type, m_dict, *dicts):
```

### Comparing `BIDSit-0.0.3/src/BIDSit/version.py` & `BIDSit-0.0.4/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.3'
+__version__ = '0.0.4'
```

### Comparing `BIDSit-0.0.3/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.4/src/BIDSit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.3
+Version: 0.0.4
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

