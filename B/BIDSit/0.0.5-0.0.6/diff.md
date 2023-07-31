# Comparing `tmp/BIDSit-0.0.5.tar.gz` & `tmp/BIDSit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BIDSit-0.0.5.tar", last modified: Fri Apr 28 21:50:18 2023, max compression
+gzip compressed data, was "BIDSit-0.0.6.tar", last modified: Mon Jul 31 22:21:16 2023, max compression
```

## Comparing `BIDSit-0.0.5.tar` & `BIDSit-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.366238 BIDSit-0.0.5/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-28 21:50:18.365973 BIDSit-0.0.5/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.5/README.rst
--rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-04-28 21:50:18.366325 BIDSit-0.0.5/setup.cfg
--rw-r--r--   0 labmanager   (501) staff       (20)     2447 2023-04-25 20:42:57.000000 BIDSit-0.0.5/setup.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.360793 BIDSit-0.0.5/src/
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.363938 BIDSit-0.0.5/src/BIDSit/
--rw-r--r--   0 labmanager   (501) staff       (20)     4701 2023-04-28 21:36:44.000000 BIDSit-0.0.5/src/BIDSit/Test_script.py
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.5/src/BIDSit/__init__.py
--rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-04-19 23:11:33.000000 BIDSit-0.0.5/src/BIDSit/__main__ .py
--rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.5/src/BIDSit/dicom_to_bids2.py
--rw-r--r--   0 labmanager   (501) staff       (20)    53467 2023-04-28 21:31:25.000000 BIDSit-0.0.5/src/BIDSit/go.py
--rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-04-28 21:37:08.000000 BIDSit-0.0.5/src/BIDSit/version.py
-drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-04-28 21:50:18.365573 BIDSit-0.0.5/src/BIDSit.egg-info/
--rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/PKG-INFO
--rw-r--r--   0 labmanager   (501) staff       (20)      329 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/SOURCES.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/dependency_links.txt
--rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/requires.txt
--rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-04-28 21:50:18.000000 BIDSit-0.0.5/src/BIDSit.egg-info/top_level.txt
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.411529 BIDSit-0.0.6/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:21:16.411140 BIDSit-0.0.6/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      762 2023-04-19 23:00:43.000000 BIDSit-0.0.6/README.rst
+-rw-r--r--   0 labmanager   (501) staff       (20)       38 2023-07-31 22:21:16.411671 BIDSit-0.0.6/setup.cfg
+-rw-r--r--   0 labmanager   (501) staff       (20)     2068 2023-07-31 20:54:57.000000 BIDSit-0.0.6/setup.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.405954 BIDSit-0.0.6/src/
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.409013 BIDSit-0.0.6/src/BIDSit/
+-rw-r--r--   0 labmanager   (501) staff       (20)     5330 2023-06-28 22:32:23.000000 BIDSit-0.0.6/src/BIDSit/Test_script.py
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-03-23 19:34:37.000000 BIDSit-0.0.6/src/BIDSit/__init__.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    24979 2023-04-26 21:48:18.000000 BIDSit-0.0.6/src/BIDSit/dicom_to_bids2.py
+-rw-r--r--   0 labmanager   (501) staff       (20)    68398 2023-07-31 21:09:49.000000 BIDSit-0.0.6/src/BIDSit/go.py
+-rw-r--r--   0 labmanager   (501) staff       (20)       83 2023-07-31 20:13:14.000000 BIDSit-0.0.6/src/BIDSit/main.py
+-rw-r--r--   0 labmanager   (501) staff       (20)      576 2023-07-31 20:27:12.000000 BIDSit-0.0.6/src/BIDSit/version.py
+drwxr-xr-x   0 labmanager   (501) staff       (20)        0 2023-07-31 22:21:16.410724 BIDSit-0.0.6/src/BIDSit.egg-info/
+-rw-r--r--   0 labmanager   (501) staff       (20)     1213 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/PKG-INFO
+-rw-r--r--   0 labmanager   (501) staff       (20)      324 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/SOURCES.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        1 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/dependency_links.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)       54 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/requires.txt
+-rw-r--r--   0 labmanager   (501) staff       (20)        7 2023-07-31 22:21:16.000000 BIDSit-0.0.6/src/BIDSit.egg-info/top_level.txt
```

### Comparing `BIDSit-0.0.5/PKG-INFO` & `BIDSit-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `BIDSit-0.0.5/README.rst` & `BIDSit-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.5/setup.py` & `BIDSit-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -58,23 +58,7 @@
     extras_require={
         "dev": [
             "pytest>=3.7",
         ],
     },
 )
 
-
-
-### --- BEFORE PUBLISHING --- ###
-# check-manifest --create
-# git add MANIFEST.in
-
-# python setup.py sdist # to do source distribution
-# tar tzf dist/BIDSit-0.0.1.tar.gz # should show lots of files see pic
-
-### --- TO PUBLISH --- ###
-# python3 setup.py bdist_wheel sdist
-# pip install twine
-# twine upload dist/*
-
-### --- TO UPDATE --- ###
-#twine upload --skip-existing dist/*
```

### Comparing `BIDSit-0.0.5/src/BIDSit/Test_script.py` & `BIDSit-0.0.6/src/BIDSit/Test_script.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,40 @@
 from BIDSit import *
 path = "/Users/labmanager/Resilience/BIDSit/info"
 import PySimpleGUI as sg
 import re
 import os
 import json
 import shutil
+import glob
+from natsort import natsorted
 user_info = {'in_dir': '/Users/labmanager/Resilience/data', 'out_dir': '/Users/labmanager/Resilience', 'dcm2niix': False, 'bids_it': True, 'copy': 'Yes', 'func': {'input_Task-1': 'Thought', 'menu_1': 'bold', 'input_Task-2': 'Word', 'menu_2': 'bold', '0': True, '1': False, '2': True, '3': False, '4': False, '5': True, '6': False, '7': True, 'input_acq Input 1': '1', 'list_acq Input 1': ['Scan 1', 'Scan 3'], 'input_acq Input 2': '2', 'list_acq Input 2': ['Scan 2', 'Scan 4'], 'input_ce Input 1': '1', 'list_ce Input 1': ['Scan 1', 'Scan 3'], 'input_ce Input 2': '2', 'list_ce Input 2': ['Scan 2', 'Scan 4'], 'input_desc Input 1': '1', 'list_desc Input 1': ['Scan 1', 'Scan 3'], 'input_desc Input 2': '2', 'list_desc Input 2': ['Scan 2', 'Scan 4'], 'input_dir Input 1': '1', 'list_dir Input 1': ['Scan 1', 'Scan 3'], 'input_dir Input 2': '2', 'list_dir Input 2': ['Scan 2', 'Scan 4'], 'input_echo Input 1': '1', 'list_echo Input 1': ['Scan 1', 'Scan 3'], 'input_echo Input 2': '2', 'list_echo Input 2': ['Scan 2', 'Scan 4'], 'input_rec Input 1': '1', 'list_rec Input 1': ['Scan 1', 'Scan 3'], 'input_rec Input 2': '2', 'list_rec Input 2': ['Scan 2', 'Scan 4']}, 'anat': {'menu_1': 'T1w', 'menu_2': 'T2w', 'menu_3': 'FLAIR', '0': False, '1': True, '2': False, '3': False, '4': False, '5': True, '6': True, '7': False, '8': False, 'input_acq Input 1': '1', 'list_acq Input 1': ['Scan 1'], 'input_acq Input 2': '2', 'list_acq Input 2': ['Scan 2'], 'input_acq Input 3': '3', 'list_acq Input 3': ['Scan 3'], 'input_ce Input 1': '1', 'list_ce Input 1': ['Scan 1'], 'input_ce Input 2': '2', 'list_ce Input 2': ['Scan 2'], 'input_ce Input 3': '3', 'list_ce Input 3': ['Scan 3'], 'input_desc Input 1': '1', 'list_desc Input 1': ['Scan 1'], 'input_desc Input 2': '2', 'list_desc Input 2': ['Scan 2'], 'input_desc Input 3': '3', 'list_desc Input 3': ['Scan 3'], 'input_dir Input 1': '1', 'list_dir Input 1': ['Scan 1'], 'input_dir Input 2': '2', 'list_dir Input 2': ['Scan 2'], 'input_dir Input 3': '3', 'list_dir Input 3': ['Scan 3'], 'input_rec Input 1': '1', 'list_rec Input 1': ['Scan 1'], 'input_rec Input 2': '2', 'list_rec Input 2': ['Scan 2'], 'input_rec Input 3': '3', 'list_rec Input 3': ['Scan 3']}, 'dwi': False, 'fmap': {'menu_1': 'epi (AP)', '-list_1-': ['func scan 1', 'func scan 2'], 'menu_2': 'epi (PA)', '-list_2-': ['func scan 1', 'func scan 2'], '0': True, '1': False, '2': False, '3': True, 'input_acq Input 1': '1', 'list_acq Input 1': ['Scan 1'], 'input_acq Input 2': '2', 'list_acq Input 2': ['Scan 2'], 'input_desc Input 1': '1', 'list_desc Input 1': ['Scan 1'], 'input_desc Input 2': '2', 'list_desc Input 2': ['Scan 2']}, 'perf': False, 'ses': 'Yes', 'WDIR': '/Users/labmanager/Resilience/data', 'func_task_num': '2', 'func_scan_num': '4', 'anat_task_num': '3', 'anat_scan_num': '3', 'fmap_task_num': '2', 'fmap_scan_num': '2', 'exp_name': 'Resilience', 'scans': {'Scan 1': ['acq-1', 'ce-1', 'rec-1', 'dir-1', 'desc-1'], 'Scan 3': ['acq-1', 'ce-1', 'rec-1', 'dir-1', 'desc-1'], 'Scan 2': ['acq-2', 'ce-2', 'rec-2', 'dir-2', 'desc-2'], 'Scan 4': ['acq-2', 'ce-2', 'rec-2', 'dir-2', 'desc-2'], 'general': {'task_order': [0, 1, 0, 1]}}}
 variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task'], 'exts': ['.json']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['T1','T2','FLAIR','PD','UNIT1','angio'], 'exts': ['.json']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['dwi', 'DWI', 'dti', 'DTI', 'hardi', 'HARDI', 'sbref', 'SBREF'], 'exts': ['.json', '.bvec', '.bval']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['rev', 'epi','EPI', 'fieldmap', 'mag', 'ph', 'MAG', 'PH'], 'exts': ['.json']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2'], 'exts': ['.json', '.tsv']}}
-WDIR = '/mnt/d/jen_test/rest_test/tempdata'
-WDIR_og = '/mnt/d/jen_test/rest_test/sourcedata'
+in_dir = '/Users/labmanager/Resilience/tempdata'
+in_dir_og = '/Users/labmanager/Resilience/data'
+og_sub = 'RESILIENCE_01/T1'
+exts = ['TR', 'fmri', 'fMRI', 'FMRI', 'task']
+files = []
+for ext in exts:
+    files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
+files = natsorted([item for sub_list in files for item in sub_list])
+#files = glob.glob(f"{in_dir.split('tempdata')[0] + in_dir_og.rsplit('/',1)[1]}/{og_sub}/*{ext}*.nii*")
+print(files)
 
-WDIR = in_dir.split('tempdata')[0] + in_dir_og.rsplit('/',1)[1]
-print(WDIR)
+## GIVE
+i
+user_info
+tasksLookedAt
+exts
+endings
+menu
+scans
+
+## RETURN
+tasksLookedAt (reg not echo)
+file_log
+
+def BIDSname(i, user_info, tasksLookedAt, exts, endings, menu, scans):
+    # - find and name files for each scan - #
+Return = return for types
+Done = no more files of this types
+Next = next scan/echo
```

### Comparing `BIDSit-0.0.5/src/BIDSit/dicom_to_bids2.py` & `BIDSit-0.0.6/src/BIDSit/dicom_to_bids2.py`

 * *Files identical despite different names*

### Comparing `BIDSit-0.0.5/src/BIDSit/go.py` & `BIDSit-0.0.6/src/BIDSit/go.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # Script Name: BIDSit.py                                                 #
 #                                                                        #
 # Description: This script converts user inputted data based on BIDS     #
 #              specifications                                            #
 #                                                                        #
 # Authors:     Jen Burrell & Justin Andrushko  (March 28th, 2023)        #
 #========================================================================#
-# json make direction match blips
 #------------------------------------------------#
 #        Import script dependency packages       #
 #------------------------------------------------#
 import subprocess
 import os
 import sys
 import re
@@ -24,26 +23,22 @@
 import shutil
 import json
 import errno
 
 
 def main():
     # - get user input - #
+    sg.theme('GreenTan')
     user_info = start_gui()
-#    print(user_info)
     
     # - define variables in use - #
     in_dir = user_info['in_dir'] # in_dir is where the input files are
     out_dir = user_info['out_dir'] # out_dir is where the output files will go
     WDIR = in_dir # WDIR is wherever we are working at the time
     user_info['WDIR'] = WDIR
-        
-    if user_info['bids_it']:
-        bids_info = BIDSit_gui(user_info)
-        user_info = {**user_info, **bids_info}
     
     ### --- convert files to NIFTIs --- ###
     if user_info['dcm2niix']:
         WDIR = out_dir
         sub_folders = glob.glob(f"{in_dir}/*/")
         ses_folders = []
         for sub in sub_folders:
@@ -74,32 +69,35 @@
                 else:
                     copy_it(WDIR+'/'+sub, out_dir + "/sourcedata/"+sub)
         else:
             copy_it(WDIR, out_dir + "/sourcedata")
     
     ### --- BIDSit --- ###
     if user_info['bids_it']:
+        bids_info = BIDSit_gui(user_info) # get BIDS information from GUI
+        user_info = {**user_info, **bids_info}
         sub_list = listdir(WDIR)
         for entry in sub_list:
             if user_info['ses'] =='Yes':
                 for file in listdir(os.path.join(WDIR,entry)):
                     if os.path.isdir(os.path.join(WDIR,entry,file)):
                         if entry in sub_list:
                             sub_list = [entry.replace(entry,os.path.join(entry,file))]
                         else:
                             sub_list.append(os.path.join(entry,file))
             else:
                 if os.path.isdir(os.path.join(WDIR,entry)):
                     continue
                 else:
                     sub_list.remove(entry)
-        for sub in sub_list:
+        for sub in natsorted(sub_list):
             BIDSit(sub, user_info)
         # - multiprocessing - #
-#        pool = Pool() # Create a multiprocessing Pool
+        ### not working with glob, wont find files ###
+#        pool = Pool(len(sub_list)) # Create a multiprocessing Pool
 #        pool.starmap(BIDSit, zip(sub_list, repeat(user_info))) # BIDSit for each participant or time point
 #        # - Close the pool, keep the kids safe - #
 #        pool.close()
 #        pool.join()
         
         ### --- make all the other files --- ###
         if out_dir != WDIR:
@@ -121,60 +119,71 @@
                     continue
                 else:
                     shutil.copytree(WDIR+'/rawdata/'+sub, der_dir+'/'+sub, ignore=ignore_files)
         else:
             shutil.copytree(WDIR+'/rawdata', der_dir, ignore=ignore_files)
         
         # - dataset_description.json file - #
-        if not os.path.exists(os.path.join(WDIR, "dataset_description.json")):
+        if not os.path.exists(os.path.join(WDIR+'/rawdata', "dataset_description.json")):
             dataset_description = {
                 "Name": user_info['exp_name'],
                 "BIDSVersion": "1.6.0",
                 "License": "Your dataset license",
                 "Authors": ["Your name"],
                 "Acknowledgements": "Your acknowledgements",
                 "HowToAcknowledge": "Your how to acknowledge",
-                "Funding": "Your funding",
+                "Funding": ["Your funding"],
                 "ReferencesAndLinks": ["Your references and links"],
                 "DatasetDOI": "Your dataset DOI"
             }
-            with open(os.path.join(WDIR, "dataset_description.json"), "w") as f:
+            with open(os.path.join(WDIR+'/rawdata', "dataset_description.json"), "w") as f:
                 json.dump(dataset_description, f, indent=4)
                 print("dataset_description.json created successfully!")
         else:
             print("dataset_description.json already exists in the directory.")
 
         # - README file - #
-        if not os.path.exists(WDIR + '/README.md'):
+        if not os.path.exists(WDIR + '/rawdata' + '/README.md'):
             # Create a new README file in BIDS format
-            with open(WDIR + '/README.md', 'w') as f:
+            with open(WDIR + '/rawdata' + '/README.md', 'w') as f:
                 f.write('# ' + os.path.basename(WDIR) + 'My Project\n\nThis is a project in BIDS format.\n\n## Introduction\n\n## Data\n\n## Code\n\n## Results\n\n## Conclusion\n\n## References\n\n')
                 print('README.md file created successfully!')
         else:
             print('README.md file already exists.')
 
         # - participants.tsv file - #
-        if not os.path.exists(WDIR + '/participants.tsv'):
+        if not os.path.exists(WDIR + '/rawdata' + '/participants.tsv'):
             # Create a new participants.tsv file in BIDS format
-            with open(WDIR + '/participants.tsv', 'w') as f:
+            with open(WDIR + '/rawdata' + '/participants.tsv', 'w') as f:
                 f.write('participant_id\tage\tsex\n')
+                for sub in natsorted(sub_list):
+                    sub = sub.split('/')[0]
+                    f.write(f"{sub}\t \t \n")
                 print('participants.tsv file created successfully!')
         else:
             print('participants.tsv file already exists.')
 
         # - participants.json file - #
-        if not os.path.exists(WDIR + '/participants.json'):
+        if not os.path.exists(WDIR + '/rawdata' + '/participants.json'):
             # Create a new participants.json file in BIDS format
-            data = {
-                "participant_id": {
-                    "age": "",
-                    "sex": ""
-                }
-            }
-            with open(WDIR + '/participants.json', 'w') as f:
+            data={}
+            for sub in natsorted(sub_list):
+                data = {
+                    "age": {
+                        "Description": "age of the participant",
+                        "Units": "years"
+                    },
+                    "sex": {
+                        "Description": "sex of the participant as reported by the participant",
+                        "Levels": {
+                            "M": "male",
+                            "F": "female"
+                        }
+                    }}
+            with open(WDIR + '/rawdata' + '/participants.json', 'w') as f:
                 json.dump(data, f, indent=4)
                 print('participants.json file created successfully!')
         else:
             print('participants.json file already exists.')
     else: # when not doing BIDSit, rename tempdata to sourcedata and delete tempdata
         WDIR = WDIR.rsplit('/',1)[0]
         dir = listdir(WDIR)
@@ -298,14 +307,15 @@
     
     main_tab_layout = [
         [sg.Text("What is the experiment name? "), sg.Push(), sg.In(enable_events=True, key='-exp_name-')],
         ]
     func_layout = [
         [sg.Text("Number of types of functional scans in your dataset"), sg.Push(), sg.In(enable_events=True, key='func_task_num', default_text=2)],
         [sg.Text("Total number of scans in your functional data"), sg.Push(), sg.In(enable_events=True, key='func_scan_num', default_text=4)],
+        [sg.Text("Do you have multi-echo data?"), sg.Push(), sg.OptionMenu(['Yes', 'No'], default_value="No", key='echo')],
         [sg.VPush()],
         [sg.Push(), sg.Button('Specify Task Order', key='-func_butt-'), sg.Push()]
         ]
     anat_layout = [
         [sg.Text("Number of types of anatomical scans in your dataset"), sg.Push(), sg.In(enable_events=True, key='anat_task_num', default_text=2)],
         [sg.Text("Total number of scans in your anatomical data"), sg.Push(), sg.In(enable_events=True, key='anat_scan_num', default_text=4)],
         [sg.VPush()],
@@ -356,15 +366,16 @@
             load_info = load_gui()
             if load_info:
                 info = {**info, **load_info}
                 window.close()
         elif event == '-func_butt-':
             info['func_task_num'] = values['func_task_num']
             info['func_scan_num'] = values['func_scan_num']
-            info['func'] = func_butt(values['func_task_num'], values['func_scan_num'])
+            info['echo'] = values['echo']
+            info['func'] = func_butt(values['func_task_num'], values['func_scan_num'], values['echo'])
         elif event == '-anat_butt-':
             info['anat_task_num'] = values['anat_task_num']
             info['anat_scan_num'] = values['anat_scan_num']
             info['anat'] = anat_butt(values['anat_task_num'], values['anat_scan_num'])
         elif event == '-dwi_butt-':
             info['dwi_task_num'] = values['dwi_task_num']
             info['dwi_scan_num'] = values['dwi_scan_num']
@@ -417,88 +428,97 @@
         elif event == '-WINDOW CLOSE ATTEMPTED-':
             exit("User exited BIDSit")
         elif event == 'Load':
             load_file = values['-load-']
             if file_exists(load_file):
                 with open(load_file) as load_file:
                     info = json.load(load_file)
-#                    info = info[0]
                 window.close()
             else:
                 sg.popup_no_border("Load file not found :( \nPlease try again or select data through data selection window")
     window.close()
     return info
 
 # - gui to specify func data parameters - #
-def func_butt(task_num, scan_num):
+def func_butt(task_num, scan_num, echo):
     info = {}
-    ents =['acq','ce', 'rec', 'dir', 'echo', 'desc']
-    files = ['bold', 'cbv']
+    ents =['acq','ce', 'rec', 'dir', 'part'] # BIDS entities + echo
+    files = ['bold', 'cbv']  # types of files supported by BIDS
     s_list = [scan_num for scan_num in range(1, int(task_num)+1)]
     the_list=[]
-    for scan in s_list:
+    for scan in s_list: # make list for each entity for every scan (in theory each scan could have different entity)
         [the_list.append(f"{ent} Input {scan}") for ent in ents]
     the_list = sorted(the_list)
-    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]}
-    for task_num in range(1, int(task_num)+1):
-        boxes[f"task-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)] # generate number of checkboxes for scan number
+    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]} # dict of text elements for each scan
+    for task_num in range(1, int(task_num)+1):  # generate number of checkboxes for scan number
+        boxes[f"task-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)]
     dropdown = {}
-    for ent in the_list:
+    for ent in the_list: # list all entities and text elements for user input and have user select which scan to apply to
         dropdown[f"{ent}"] = [sg.Text(f"-{ent}"), sg.Push(), input_element(ent), f_list_element(scan_num, ent)]
-    
     col3 = [drop for drop in dropdown.values()]
-
+    if echo == 'Yes':
+        scan_types = [[[text_element(f"Name of Task {num}"), input_element(f"Task-{num}")], [text_element("What kind of func image is this Task?"), menu(files, num)], [text_element(f"Number of echos in Task {num}"), input_element(f"Task-{num}-echo")]] for num in range(1, int(task_num)+1)]
+    else:
+        scan_types = [[[text_element(f"Name of Task {num}"), input_element(f"Task-{num}")], [text_element("What kind of func image is this Task?"), menu(files, num)]] for num in range(1, int(task_num)+1)]
+    scan_types = [item for sublist in scan_types for item in sublist]
+    # - layout - #
     func_layout_2 = [
-        [[[text_element(f"Name of Task {num}"), input_element(f"Task-{num}")], [text_element("What kind of func image is this Task?"), menu(files, num)]] for num in range(1, int(task_num)+1)],
+        [sg.Column(scan_types, scrollable=True, expand_x=True, vertical_scroll_only=True, size=(None,200))],
         [sg.vbottom(sg.Column([[text_element(f"Order of Task {task_num}")] for task_num in range(1, int(task_num)+1)],
             key='COLUMN 1')),
         sg.Column([box for box in boxes.values()],expand_x=True, key='COLUMN 2')],
         [sg.Text('BIDS entities:'), sg.Push(), sg.Text('Select all that apply')],
-        [sg.Column(col3, scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
+        [sg.Column(col3, size=(None,200), scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
         [sg.Button('Go'), sg.Button('Cancel')]
     ]
     window_2 = sg.Window("Functional Images Order", func_layout_2, resizable=True)
     while True:
         event, values = window_2.read()
         if event == 'Cancel':
             window_2.close()
-        if event == sg.WIN_CLOSED:
+        elif event == sg.WIN_CLOSED:
             break
-        if event == 'Go':
+        elif event == 'Go':
+            info = values
+            flag = False
+            if echo == 'Yes':
+                for num in range(1, int(task_num)+1):
+                    if not values[f"input_Task-{num}-echo"] or int(values[f"input_Task-{num}-echo"]) < 1:
+                        values[f"input_Task-{num}-echo"] = sg.popup_get_text(f"Number of echos for Task {num} must be >= 1 n\Please enter number of echos for Task {num}", title="Oops")
             info = values
             window_2.close()
     return info
     window_2.close()
     
 # - gui to specify anat data parameters - #
 def anat_butt(task_num, scan_num):
     info = {}
-    ents = ['acq','ce', 'rec', 'dir', 'desc']
-    files = ['T1w', 'T2starw', 'T2w', 'FLAIR', 'PDT2', 'PDw', 'UNIT1', 'angio', 'inplaneT1', 'inplaneT2']
+    ents = ['acq','ce', 'rec', 'dir', 'part'] # BIDS entities
+    files = ['T1w', 'T2starw', 'T2w', 'FLAIR', 'PDT2', 'PDw', 'UNIT1', 'angio', 'inplaneT1', 'inplaneT2'] # types of files supported by BIDS
     s_list = [scan_num for scan_num in range(1, int(task_num)+1)]
     the_list=[]
-    for scan in s_list:
+    for scan in s_list: # make list for each entity for every scan (in theory each scan could have different entity)
         [the_list.append(f"{ent} Input {scan}") for ent in ents]
     the_list = sorted(the_list)
-    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]}
-    for task_num in range(1, int(task_num)+1):
-        boxes[f"scan_type-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)] # generate number of checkboxes for scan number
+    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]} # dict of text elements for each scan
+    for task_num in range(1, int(task_num)+1): # generate number of checkboxes for scan number
+        boxes[f"scan_type-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)]
     dropdown = {}
-    for ent in the_list:
+    for ent in the_list: # list all entities and text elements for user input and have user select which scan to apply to
         dropdown[f"{ent}"] = [sg.Text(f"-{ent}"), sg.Push(), input_element(ent), f_list_element(scan_num, ent)]
     
     col3 = [drop for drop in dropdown.values()]
 
     layout_2 = [
         [[text_element(f"What kind of anat image is scan type {num}?"), menu(files, num)] for num in range(1, int(task_num)+1)],
         [sg.vbottom(sg.Column([[text_element(f"Order of scan type {task_num}")] for task_num in range(1, int(task_num)+1)],
             key='COLUMN 1')),
         sg.Column([box for box in boxes.values()],expand_x=True, key='COLUMN 2')],
         [sg.Text('BIDS entities:'), sg.Push(), sg.Text('Select all that apply')],
-        [sg.Column(col3, scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
+        [sg.Column(col3, size=(None,200), scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
         [sg.Button('Go'), sg.Button('Cancel')]
     ]
     window_2 = sg.Window("Anatomical Images Order", layout_2, resizable=True)
     while True:
         event, values = window_2.read()
         if event == 'Cancel':
             window_2.close()
@@ -509,37 +529,37 @@
             window_2.close()
     return info
     window_2.close()
     
 # - gui to specify dwi data parameters - #
 def dwi_butt(task_num, scan_num):
     info = {}
-    ents = ['acq', 'rec', 'dir', 'desc']
-    files = ['dwi', 'sbref']
+    ents = ['acq', 'rec', 'dir', 'part'] # BIDS entities
+    files = ['dwi', 'sbref'] # types of files supported by BIDS
     s_list = [scan_num for scan_num in range(1, int(task_num)+1)]
     the_list=[]
-    for scan in s_list:
+    for scan in s_list: # make list for each entity for every scan (in theory each scan could have different entity)
         [the_list.append(f"{ent} Input {scan}") for ent in ents]
     the_list = sorted(the_list)
-    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]}
-    for task_num in range(1, int(task_num)+1):
-        boxes[f"scan_type-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)] # generate number of checkboxes for scan number
+    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]} # dict of text elements for each scan
+    for task_num in range(1, int(task_num)+1): # generate number of checkboxes for scan number
+        boxes[f"scan_type-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)]
     dropdown = {}
-    for ent in the_list:
+    for ent in the_list: # list all entities and text elements for user input and have user select which scan to apply to
         dropdown[f"{ent}"] = [sg.Text(f"-{ent}"), sg.Push(), input_element(ent), f_list_element(scan_num, ent)]
     
     col3 = [drop for drop in dropdown.values()]
-
+    
     layout_2 = [
         [[text_element(f"What kind of DWI image is scan type {num}?"), menu(files, num)] for num in range(1, int(task_num)+1)],
         [sg.vbottom(sg.Column([[text_element(f"Order of scan type {task_num}")] for task_num in range(1, int(task_num)+1)],
             key='COLUMN 1')),
         sg.Column([box for box in boxes.values()],expand_x=True, key='COLUMN 2')],
         [sg.Text('BIDS entities:'), sg.Push(), sg.Text('Select all that apply')],
-        [sg.Column(col3, scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
+        [sg.Column(col3, scrollable=True, vertical_scroll_only=True, size=(None,200), expand_x=True, expand_y=True)],
         [sg.Button('Go'), sg.Button('Cancel')]
     ]
     window_2 = sg.Window("DWI Images Order", layout_2, resizable=True)
     while True:
         event, values = window_2.read()
         if event == 'Cancel':
             window_2.close()
@@ -550,26 +570,26 @@
             window_2.close()
     return info
     window_2.close()
     
 # - gui to specify fmap data parameters - #
 def fmap_butt(task_num, scan_num, user_info):
     info = {}
-    ents = ['acq', 'desc']
-    files = ['epi (AP)', 'epi (PA)', 'epi (rev-b0)', 'fieldmap', 'magnitude', 'magnitude1', 'magnitude2', 'phasediff', 'phase1', 'phase2']
+    ents = ['acq', 'run'] # BIDS entities
+    files = ['epi (AP)', 'epi (PA)', 'epi (rev-b0)', 'fieldmap', 'magnitude', 'magnitude1', 'magnitude2', 'phasediff', 'phase1', 'phase2'] # types of files supported by BIDS
     s_list = [scan_num for scan_num in range(1, int(task_num)+1)]
     the_list=[]
-    for scan in s_list:
+    for scan in s_list: # make list for each entity for every scan (in theory each scan could have different entity)
         [the_list.append(f"{ent} Input {scan}") for ent in ents]
     the_list = sorted(the_list)
-    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]}
-    for task_num in range(1, int(task_num)+1):
-        boxes[f"task-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)] # generate number of checkboxes for scan number
+    boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]} # dict of text elements for each scan
+    for task_num in range(1, int(task_num)+1): # generate number of checkboxes for scan number
+        boxes[f"task-{task_num}"] = [f_cbox_element(scan_num, task_num) for scan_num in range(1, int(scan_num)+1)]
     dropdown = {}
-    for ent in the_list:
+    for ent in the_list: # list all entities and text elements for user input and have user select which scan to apply to
         dropdown[f"{ent}"] = [sg.Text(f"-{ent}"), sg.Push(), input_element(ent), f_list_element(scan_num, ent)]
     
     col3 = [drop for drop in dropdown.values()]
 
     # - get list of scans - #
     scan_list = []
     scan_key = []
@@ -586,22 +606,23 @@
     for i, type in enumerate(scan_key):
         if type == 'func':
             for i in range(scan_list[i]):
                 type_list.append(type + ' scan ' + str(i+1))
         else:
             for i in range(scan_list[i]):
                 type_list.append(type + ' scan type ' + str(i+1))
+    scan_types = [[[text_element(f"What kind of fmap image is scan type {num}?"), menu(files, num)], [text_element(f"What images is scan type {num} intended for? (select all that apply)"), sg.Push(), list_element(type_list, num)]] for num in range(1, int(task_num)+1)]
+    scan_types = [item for sublist in scan_types for item in sublist]
     layout_2 = [
-        [[[text_element(f"What kind of fmap image is scan type {num}?"), menu(files, num)], [text_element(f"What images is scan type {num} intended for? (select all that apply)"), sg.Push(), list_element(type_list, num)]] for num in range(1, int(task_num)+1)],
+        [sg.Column(scan_types, scrollable=True, expand_x=True, vertical_scroll_only=True, size=(None,200))],
         [sg.Button('Info', key='-info-')],
-        [sg.vbottom(sg.Column([[text_element(f"Order for scan type {task_num}")] for task_num in range(1, int(task_num)+1)],
-            key='COLUMN 1')),
-        sg.Column([box for box in boxes.values()],expand_x=True, key='COLUMN 2')],
+        [sg.vbottom(sg.Column([[text_element(f"Order for scan type {task_num}")] for task_num in range(1, int(task_num)+1)], key='COLUMN 1')),
+        sg.Column([box for box in boxes.values()], expand_x=True, key='COLUMN 2')],
         [sg.Text('BIDS entities:'), sg.Push(), sg.Text('Select all that apply')],
-        [sg.Column(col3, scrollable=True, vertical_scroll_only=True, expand_x=True, expand_y=True)],
+        [sg.Column(col3, scrollable=True, expand_x=True, vertical_scroll_only=True, size=(None,200))],
         [sg.Button('Go'), sg.Button('Cancel')]
     ]
     window_2 = sg.Window("Fieldmap Images Order", layout_2, resizable=True)
     while True:
         event, values = window_2.read()
         if event == 'Cancel':
             window_2.close()
@@ -631,15 +652,15 @@
     return info
     window_2.close()
     
 # - gui to specify perf data parameters - #
 def perf_butt(task_num, scan_num):
     ##### NOT DONE #####
     info = {}
-    ents = ['acq', 'rec', 'dir', 'desc']
+    ents = ['acq', 'rec', 'dir']
     files = ['CASL', 'PCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan']
     s_list = [scan_num for scan_num in range(1, int(task_num)+1)]
     the_list=[]
     for scan in s_list:
         [the_list.append(f"{ent} Input {scan}") for ent in ents]
     the_list = sorted(the_list)
     boxes = {'text': [text_element(f"Scan {scan_num}") for scan_num in range(1, int(scan_num)+1)]}
@@ -683,53 +704,361 @@
         WDIR = WDIR + '/' + in_dir.split('/')[-2] + '/' + in_dir.split('/')[-1]
     else:
         WDIR = WDIR + '/' + in_dir.split('/')[-1]
     mkdir(WDIR)
     subprocess.call(['dcm2niix', '-b', 'y', '-ba', 'y', '-z', 'y', '-f', '%x_%p_%t_%s', '-o', WDIR, in_dir]) # (%a=antenna (coil) name, %b=basename, %c=comments, %d=description, %e=echo number, %f=folder name, %i=ID of patient, %j=seriesInstanceUID, %k=studyInstanceUID, %m=manufacturer, %n=name of patient, %o=mediaObjectInstanceUID, %p=protocol, %r=instance number, %s=series number, %t=time, %u=acquisition number, %v=vendor, %x=study ID; %z=sequence name; default '%f_%p_%t_%s')
 
 ### --- organize NIFTIs into BIDS --- ###
+# - find and name files for each scan - #
+def BIDSgo(sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, *echo):
+    # - define variables in use - #
+    WDIR = user_info['out_dir'] # file output (where the work is done)
+    mkdir(WDIR, 'rawdata')
+    mkdir(WDIR, 'derivatives')
+    in_dir = user_info['WDIR'] # file input
+    in_dir_og = in_dir
+    if not 'tempdata' in in_dir: # make tempdata the folder we are editing to make sure we dont mess things up
+        new_indir = in_dir.rsplit('/', 1)[0] + "/tempdata"
+        if not dir_exists(new_indir):
+            shutil.copytree(in_dir, new_indir)
+        in_dir = new_indir
+
+    og_sub = sub # subject folder name from provided data
+    if user_info['ses'] =='Yes': # split up ses and sub info if there are sessions
+        sub = 'sub-'+''.join(re.findall(r'\d+',sub.split('/')[0]))+ '_ses-'+''.join(re.findall(r'\d+',sub.split('/')[1]))
+        f_sub = sub.split('_')[0]+'/'+sub.split('_')[1] # file naming subject variable 'sub-<label>/ses-<label>'
+        sub_solo = sub.split('_')[0] # subject variable that only has sub information 'sub-<label>'
+    else:
+        num = re.findall(r'\d+',sub)
+        if not any(num):
+            sub = 'sub-'+ sub
+        else:
+            sub = 'sub-'+''.join(num)
+        sub_solo = sub # subject variable that only has sub information
+        f_sub = sub # file naming subject variable
+            
+    task_num = int(user_info[f"{file_type}_task_num"])
+    scan_num = int(user_info[f"{file_type}_scan_num"])
+    
+    
+    if echo and isinstance(echo[0], int): # check to see if it is an intended for file or an echo file or both
+        echo_num = echo[0]
+        if len(echo) > 1:
+            types = echo[1]
+        else:
+            types = {}
+    elif echo and isinstance(echo, tuple):
+        types = echo[0]
+        echo_num = 1
+        echo = {}
+    else:
+        types = echo
+        echo_num = 1
+        echo = {}
+        
+    files =[]
+    file = ''
+    if types:
+        i = types[1]
+        for ext in exts:
+            files.append(glob.glob(f"{in_dir.split('tempdata')[0] + in_dir_og.rsplit('/',1)[1]}/{og_sub}/*{ext}*.nii*"))
+    else:
+        for ext in exts:
+            files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
+            
+    # sort files by numbers at end to get scan order
+    files = natsorted([item for sub_list in files for item in sub_list])
+    if file_type in ['func','fmap']: # sorts files based on aquisition number at end of file
+        file_list = []
+        for file in files:
+            if "_ph." in file: # might cause an issue for phase map files. If they are signaled by dxm2nii with ph. as end of file name
+                continue
+            if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1:
+                file_list.append('_'.join(file.rsplit('_',2)[-2:]).split('.')[0])
+            else:
+                file_list.append(file.rsplit('_',1)[-1].split('.')[0])
+                
+        file_list = natsorted(file_list)
+        files_full = files
+        files = []
+        for file in file_list:
+            flag = False
+            for f in files_full:
+                if file in f:
+                    files.append(f)
+                    flag = True
+                    break
+            if flag == True:
+                continue
+    if not files:
+        print(f"No more {file_type} files were found in {in_dir}/{og_sub}, with search terms: {exts}")
+        return tasksLookedAt, file_log, "Done"
+    file_list = []
+    for f in files:
+        if 'AX' in f and 'REF' in f:
+            continue
+        else:
+            file_list.append(f)
+            
+    if file_type == 'fmap': # removes any files with _ph. in ending if not a phase map image
+        if not 'phase' in menu[i]:
+            file_list_full = file_list
+            file_list = []
+            for file in file_list_full:
+                if not '_ph.' in file:
+                    file_list.append(file)
+    if file_type != 'func': # if there isnt the right number of files to indicated scans, it looks for menu term (e.g. EPI or BOLD) in file name and takes the first matching file
+        if (scan_num - i) != len([item for item in file_list]):
+            for end in user_info[file_type][f"menu_{i+1}"].split('w')[0].split('('): # anat/fmap
+                end = end.split(')')[0].split()[0]
+                for f in file_list:
+                    f_full = f
+                    f = f.rsplit('/')[-1].lower()
+                    if end in f:
+                        file = f_full
+                        break
+                    else:
+                        file = ''
+                    f = f_full.rsplit('/')[-1].upper()
+                    if end in f:
+                        file = f_full
+                        break
+                    else:
+                        file = ''
+                break
+        else:
+            file = file_list[0]
+    else: # for func files, removes fmap files that are commonly mistaken as func files
+        file_list_full = file_list
+        file_list = []
+        for file in file_list_full:
+            if not 'EPI' in file:
+                file_list.append(file)
+        if not file_list:
+            file = ''
+        else:
+            file = file_list[0]
+    if not file: # if no files are found
+        if types:
+            return tasksLookedAt, file_log, "Return"
+        if file_type == 'func':
+            print(f"No more func files for {og_sub}")
+        else:
+            print(f"No files for {og_sub} matching", user_info[file_type][f"menu_{i+1}"])
+        return tasksLookedAt, file_log, "Next"
+    mkdir(WDIR, f"rawdata/{f_sub}/{file_type}") # make the folder for the file type
+    task_cat = task_ord[i] # task number (-1)
+    f_type = menu[task_cat] # type of file
+    endings[i] = endings[i] + '_' + f_type # adds file type to ending
+    fill_it = '_'+'_'.join(scans[f"Scan {i+1}"]) # makes string of all the scan parameters specified by user
+    if fill_it == '_': # if no scan parameters, empty the string
+        fill_it = ''
+    # - counting - #
+    if echo:
+        if types:
+            numb = task_ord[:i+1].count(task_ord[i])
+            run_num = numb
+        else:
+            occur = tasksLookedAt.count(task_cat) # counts occurance of task
+            run_num = occur + 1 # run number based on how many times that task occured
+            if echo_num == int(user_info[file_type][f"input_Task-{task_cat+1}-echo"]):
+                tasksLookedAt.append(task_cat) # add current occurance to task list
+    else:
+        occur = tasksLookedAt.count(task_cat) # counts occurance of task
+        run_num = occur + 1 # run number based on how many times that task occured
+        tasksLookedAt.append(task_cat) # add current occurance to task list
+    
+    # - naming - #
+    if file_type == 'func':
+        task_name = ''.join(task_names[task_cat].split()) # task name
+        if scan_num == task_num:
+            new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task-{task_name}{fill_it}{endings[i]}.nii.gz" # new name for file
+        else:
+            new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task-{task_name}{fill_it}_run-{run_num}{endings[i]}.nii.gz" # new name for file
+        if echo:
+            new = ''.join([new.rsplit("_",1)[0], f"_echo-{echo_num}_", new.rsplit("_",1)[-1]])
+        if 'part' in new or 'echo' in new: # organize entities into correct order
+            new_list = new.split('_')
+            final_list = []
+            i_part = False
+            i_echo = False
+            for ind, val in enumerate(new_list):
+                if 'part' in val:
+                    i_part = ind
+                    continue
+                elif 'echo' in val:
+                    i_echo = ind
+                    continue
+                elif 'bold' in val:
+                    continue
+                final_list.append(val)
+            if i_echo is not False:
+                final_list.append(new_list[i_echo])
+            if i_part is not False:
+                final_list.append(new_list[i_part])
+            final_list.append(new.rsplit("_",1)[-1])
+            new = '_'.join(final_list)
+        if echo:
+            file_log['changes'][f"scan {i+1} echo {echo_num} old"] = file # add old name to change file
+            file_log['changes'][f"scan {i+1} echo {echo_num} new"] = new # add new name to change file
+        else:
+            file_log['changes'][f"scan {i+1} old"] = file # add old name to change file
+            file_log['changes'][f"scan {i+1} new"] = new # add new name to change file
+        print("file:", file)
+        print("new:", new)
+        if types:
+            shutil.copy(file, new) # copy file to new location if doing so for fmap 'intended for'
+        else:
+            os.rename(file, new) # rename file
+        json_file = file.replace('.nii.gz','.json') # get .json file assocated
+        json_new = new.replace('.nii.gz','.json') # new name for .json file
+        if not file_exists(json_new):
+            if types:
+                shutil.copy(json_file, json_new) # copy file to new location if doing so for fmap 'intended for'
+            else:
+                os.rename(json_file, json_new) # rename file
+            json_edit(json_new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
+        elif not types:
+            with open(json_new, 'r') as file:
+                data = json.load(file)
+            if 'PhaseEncodingDirection' in data.keys():
+                PhaseEncodingDirection = data['PhaseEncodingDirection']
+            os.rename(json_file, json_new) # rename file
+            json_edit(json_new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
+            with open(json_new, 'r') as file:
+                datum = json.load(file)
+            datum['PhaseEncodingDirection'] = PhaseEncodingDirection
+            with open(json_new, 'w') as this:
+                json.dump(datum, this, indent=4)
+    else:
+        new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}.nii.gz" # new name for file
+        if 'part' in new or 'echo' in new: # organize entities into correct order
+            new_list = new.split('_')
+            final_list = []
+            i_part = False
+            i_echo = False
+            for ind, val in enumerate(new_list):
+                if 'part' in val:
+                    i_part = ind
+                    continue
+                if 'echo' in val:
+                    i_echo = ind
+                    continue
+                final_list.append(val)
+            if i_echo is not False:
+                final_list.insert(-1, new_list[i_echo])
+            if i_part is not False:
+                final_list.insert(-1, new_list[i_part])
+            new = '_'.join(final_list)
+        if echo:
+            file_log['changes'][f"scan {i+1} echo {echo_num} old"] = file # add old name to change file
+            file_log['changes'][f"scan {i+1} echo {echo_num} new"] = new # add new name to change file
+        else:
+            file_log['changes'][f"scan {i+1} old"] = file # add old name to change file
+            file_log['changes'][f"scan {i+1} new"] = new # add new name to change file
+        print("file:", file)
+        print("new:", new)
+        if types:
+            shutil.copy(file, new) # copy file to new location if doing so for fmap 'intended for'
+        else:
+            os.rename(file, new) # rename file
+        if file_type == 'fmap':
+            add_dict = {user_info['fmap'][f"menu_{i+1}"]: user_info['fmap'][f"-list_{i+1}-"]}
+        else:
+            add_dict = {}
+        for ext in variables[file_type]['exts']: # make all the file extensions
+            if 'nii.gz' in file:
+                file = file.rsplit('.',2)[0] + ext
+            else:
+                file = file.rsplit('.',1)[0] + ext
+            new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}{ext}" # new name for file
+            if 'part' in new or 'echo' in new: # organize entities into correct order
+                new_list = new.split('_')
+                final_list = []
+                i_part = False
+                i_echo = False
+                for ind, val in enumerate(new_list):
+                    if 'part' in val:
+                        i_part = ind
+                        continue
+                    if 'echo' in val:
+                        i_echo = ind
+                        continue
+                    final_list.append(val)
+                if i_echo is not False:
+                    final_list.insert(-1, new_list[i_echo])
+                if i_part is not False:
+                    final_list.insert(-1, new_list[i_part])
+                new = '_'.join(final_list)
+            if not file_exists(new):
+                buf = False
+                if types:
+                    shutil.copy(file, new) # copy file to new location if doing so for fmap 'intended for'
+                else:
+                    os.rename(file, new) # rename file
+            else:
+                buf = True
+            if ext == '.json':
+                if buf and not types:
+                    with open(new, 'r') as this:
+                        data = json.load(this)
+                    PhaseEncodingDirection = data['PhaseEncodingDirection']
+                    os.rename(file, new) # rename file
+                    json_edit(new, file_type, f_sub, og_sub, user_info) # edit json files to include necessary information
+                    with open(new, 'r') as this:
+                        datum = json.load(this)
+                    datum['PhaseEncodingDirection'] = PhaseEncodingDirection
+                    with open(new, 'w') as this:
+                        json.dump(datum, this, indent=4)
+                else:
+                    json_edit(new, file_type, f_sub, og_sub, user_info, add_dict) # edit json files to include necessary information
+    return tasksLookedAt, file_log, "Next"
+        
+                
+# - organize all data and call function to find and rename files - #
 def BIDSit(sub, user_info, *types):
-    print(user_info)
+    print(sub)
     # - define variables in use - #
     WDIR = user_info['out_dir'] # file output (where the work is done)
     mkdir(WDIR, 'rawdata')
+    mkdir(WDIR, 'derivatives')
     in_dir = user_info['WDIR'] # file input
     in_dir_og = in_dir
-    if not 'tempdata' in in_dir:
+    if not 'tempdata' in in_dir: # make tempdata the folder we are editing to make sure we dont mess things up
         new_indir = in_dir.rsplit('/', 1)[0] + "/tempdata"
         if not dir_exists(new_indir):
             shutil.copytree(in_dir, new_indir)
         in_dir = new_indir
 
-    og_sub = sub
-    if user_info['ses'] =='Yes':
+    og_sub = sub # subject folder name from provided data
+    if user_info['ses'] =='Yes': # split up ses and sub info if there are sessions
         sub = 'sub-'+''.join(re.findall(r'\d+',sub.split('/')[0]))+ '_ses-'+''.join(re.findall(r'\d+',sub.split('/')[1]))
-        f_sub = sub.split('_')[0]+'/'+sub.split('_')[1]
-        sub_solo = sub.split('_')[0]
+        f_sub = sub.split('_')[0]+'/'+sub.split('_')[1] # file naming subject variable 'sub-<label>/ses-<label>'
+        sub_solo = sub.split('_')[0] # subject variable that only has sub information 'sub-<label>'
     else:
         num = re.findall(r'\d+',sub)
         if not any(num):
             sub = 'sub-'+ sub
         else:
             sub = 'sub-'+''.join(num)
-        sub_solo = sub
-        f_sub = sub
+        sub_solo = sub # subject variable that only has sub information
+        f_sub = sub # file naming subject variable
     
-    # - make folders - #
+    # - what type of files are we processing - #
     process_og = ['fmap', 'func', 'anat', 'dwi'] # add perf once complete
     process = []
     for key in process_og:
         if key in user_info:
             if not user_info[key]:
                 continue
             else:
                 process.append(key)
     
     ### --- organize in BIDS --- ###
-    variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task'], 'exts': ['.json']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['T1','T2','FLAIR','PD','UNIT1','angio'], 'exts': ['.json']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['dwi', 'DWI', 'dti', 'DTI', 'hardi', 'HARDI', 'sbref', 'SBREF'], 'exts': ['.json', '.bvec', '.bval']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['rev', 'epi','EPI', 'fieldmap', 'mag', 'ph', 'MAG', 'PH'], 'exts': ['.json']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2'], 'exts': ['.json', '.tsv']}}
+    variables = {'func': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'echo':{'names':[],'scans':[]}, 'part':{'names':[],'scans':[]}}, 'key_words': ['TR', 'fmri','fMRI','FMRI', 'task'], 'exts': ['.json']}, 'anat': {'ents': {'acq':{'names':[],'scans':[]}, 'ce':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'part':{'names':[],'scans':[]}}, 'key_words': ['T1','T2','FLAIR','PD','UNIT1','angio'], 'exts': ['.json']}, 'dwi': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'part':{'names':[],'scans':[]}}, 'key_words': ['dwi', 'DWI', 'dti', 'DTI', 'hardi', 'HARDI', 'sbref', 'SBREF'], 'exts': ['.json', '.bvec', '.bval']}, 'fmap': {'ents': {'acq':{'names':[],'scans':[]}, 'run':{'names':[],'scans':[]}}, 'key_words': ['rev', 'epi','EPI', 'fieldmap', 'mag', 'ph', 'MAG', 'PH'], 'exts': ['.json']}, 'perf': {'ents': {'acq':{'names':[],'scans':[]}, 'rec':{'names':[],'scans':[]}, 'dir':{'names':[],'scans':[]}, 'desc':{'names':[],'scans':[]}}, 'key_words': ['CASL', 'pCASL', 'FAIR', 'EPISTAR', 'PICORE', 'm0scan', 'phase1', 'phase2'], 'exts': ['.json', '.tsv']}}
     map_dict = {}
     for file_type in process:
         if types:
             file_type = types[0]
             
         file_log = {"Scan type": file_type, 'changes':{}}
         task_num = int(user_info[f"{file_type}_task_num"])
@@ -741,15 +1070,15 @@
             entsc_list.append(variables[file_type]['ents'][ent]['scans'])
             ents.append(ent)
             
         # - get pattern of tasks from True/False list - #
         for key, val in user_info[file_type].items():
             if str(key).isnumeric():
                 task_ord.append(val) # True False list
-            if isinstance(key, str) and 'input_Task' in key:
+            if isinstance(key, str) and 'input_Task' in key and 'echo' not in key:
                 task_names.append(val)  # list of task names
             if isinstance(key, str) and 'menu' in key:
                 menu.append(val) # file type
             for i, ent in enumerate(ent_list):
                 if isinstance(key, str) and f"input_{ents[i]}" in key:
                     ent.append(f"{ents[i]}-{val}")
             for j, ent_scan in enumerate(entsc_list):
@@ -775,29 +1104,26 @@
         scans = dict_it(ent_scan, tity_list) # mapping for user_input
         user_info['scans'] = scans
         
         if not scans: #if no mapping is required
             for scan in range(1,scan_num+1):
                 scans[f"Scan {scan}"] = []
         scans['general'] = {'task_order': task_ord}
+        
         # - get dir and ending for fmap files - #
         if file_type == 'fmap':
             for i, type in enumerate(task_ord):
                 if menu[type] == 'epi (rev-b0)':
+                    if not 'acq' in scans[f"Scan {i+1}"]:
+                        scans[f"Scan {i+1}"].append("acq-revb0")
                     if not 'dir' in scans[f"Scan {i+1}"]:
                         scans[f"Scan {i+1}"].append(f"dir-{user_info['fmap']['rev-b0']['rev-dir']}")
-                    for j, entry in enumerate(scans[f"Scan {i+1}"]):
-                        if 'acq' in entry:
-                            scans[f"Scan {i+1}"][j] = entry+'-revb0'
-                            acq = True
-                            break
-                        else:
-                            acq = False
-                    if not acq:
-                        scans[f"Scan {i+1}"].append('acq-revb0')
+                    else:
+                        if not 'desc' in scans[f"Scan {i+1}"]:
+                            scans[f"Scan {i+1}"].append("desc-revb0")
                 else:
                     scans[f"Scan {i+1}"].append('dir-'+menu[type].split('(')[-1].split(')')[0])
             menu = [menu[i].split(' ')[0] for i in range(task_num)]
                 
         # - get endings for files - #
         endings = []
         for i, (key, val) in enumerate(scans.items()):
@@ -806,150 +1132,67 @@
                     endings.append('_' + value)
                     val.remove(value)
             if len(endings)-1 != i:
                 endings.append('')
     
         # - Rename files - #
         exts = variables[file_type]['key_words']
-        tasksLookedAt=[]
-        map_dict = {f"{file_type}": {'task_ord': task_ord, 'scans': scans}, 'WDIR': WDIR, 'f_sub': f_sub}
+        if types:
+            tasksLookedAt=types[2]
+        else:
+            tasksLookedAt=[]
         for i in range(scan_num):
-            files =[]
-            file = ''
-            if types:
-                i = types[1]
-                for ext in exts:
-                    files.append(glob.glob(f"{in_dir.split('tempdata')[0] + in_dir_og.rsplit('/',1)[1]}/{og_sub}/*{ext}*.nii*"))
-            else:
-                for ext in exts:
-                    files.append(glob.glob(f"{in_dir}/{og_sub}/*{ext}*.nii*"))
-            files = natsorted([item for sub_list in files for item in sub_list])
-            if not files:
-                print(f"No {file_type} files were found in {in_dir}/{og_sub}")
-                break
-            file_list = []
-            for f in files:
-                if 'AX' in f and 'REF' in f:
-                    continue
-                else:
-                    file_list.append(f)
-                    
-            if file_type != 'func':
-                if (scan_num - i) != len([item for sublist in file_list for item in sublist]):
-                    for end in user_info[file_type][f"menu_{i+1}"].split('w')[0].split('('):
-                        end = end.split(')')[0]
-                        end = end.split()[0]
-                        for f in file_list:
-                            f_full = f
-                            f = f.rsplit('/')[-1].lower()
-                            if end in f:
-                                file = f_full
-                                break
-                            else:
-                                file = ''
-                            f = f.rsplit('/')[-1].upper()
-                            if end in f:
-                                file = f_full
-                                break
-                            else:
-                                file = ''
+            stop = False
+            if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # if multi-echo data
+                for echo in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1):
+                    tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, echo)
+                    if code == 'Done':
+                        stop = True
                         break
-                else:
-                    file = file_list[0]
-            else:
-                if (scan_num - i) != len([item for sublist in file_list for item in sublist]):
-                    file_list_full = file_list
-                    file_list = []
-                    for file in file_list_full:
-                        if not 'EPI' in file:
-                            file_list.append(file)
-                if not file_list:
-                    file = ''
-                else:
-                    file = file_list[0]
-            
-            if not file:
-                if types:
+            elif types: # if working for "intended for"
+                i = types[1]
+                if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # if multi-echo data
+                    for echo in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1):
+                        tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, echo, types)
+                        if code == 'Done':
+                            stop = True
+                            break
+                else: # if single echo data
+                    tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables, types)
+                if code == 'Return':
                     return
-                if file_type == 'func':
-                    print(f"No more func files for {og_sub}")
-                else:
-                    print(f"No files for {og_sub} matching", user_info[file_type][f"menu_{i+1}"])
-                continue
-            mkdir(WDIR, f"rawdata/{f_sub}/{file_type}")
-            task_cat = task_ord[i] # task number (-1)
-            f_type = menu[task_cat] # type of file
-            endings[i] = endings[i] + '_' + f_type # adds file type to ending
-            fill_it = '_'+'_'.join(scans[f"Scan {i+1}"])
-            if fill_it == '_':
-                fill_it = ''
-            # - counting - #
-            occur = tasksLookedAt.count(task_cat) # counts occurance of task
-            run_num = occur + 1 # run number based on how many times that task occured
-            tasksLookedAt.append(task_cat) # add current occurance to task list
-            # - naming - #
-            if file_type == 'func':
-                task_name = ''.join(task_names[task_cat].split()) # task name
-                new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run-{run_num}{endings[i]}.nii.gz" # new name for file
-                file_log['changes'][f"scan {i+1} old"] = file
-                file_log['changes'][f"scan {i+1} new"] = new
-                print("file:", file)
-                print("new:", new)
-                if types:
-                    shutil.copy(file, new)
-                else:
-                    os.rename(file, new) # rename file
-                json_file = file.replace('.nii.gz','.json') # get .json file assocated
-                json_new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}_task_{task_name}{fill_it}_run-{run_num}{endings[i]}.json" # new name for .json file
-                if types:
-                    shutil.copy(json_file, json_new)
-                else:
-                    os.rename(json_file, json_new) # rename file
-                json_edit(json_new, file_type, f_sub, og_sub, user_info)
-            else:
-                new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}.nii.gz" # new name for file
-                file_log['changes'][f"scan {i+1} old"] = file
-                file_log['changes'][f"scan {i+1} new"] = new
-                print("file:", file)
-                print("new:", new)
-                if types:
-                    shutil.copy(file, new)
-                else:
-                    os.rename(file, new) # rename file
-                if file_type == 'fmap':
-                    add_dict = {user_info['fmap'][f"menu_{i+1}"]: user_info['fmap'][f"-list_{i+1}-"]}
-                else:
-                    add_dict = {}
-                for ext in variables[file_type]['exts']:
-                    if 'nii.gz' in file:
-                        file = file.rsplit('.',2)[0] + ext
-                    else:
-                        file = file.rsplit('.',1)[0] + ext
-                    new = f"{WDIR}/rawdata/{f_sub}/{file_type}/{sub}{fill_it}{endings[i]}{ext}" # new name for file
-                    if types:
-                        shutil.copy(file, new)
-                    else:
-                        os.rename(file, new) # rename file
-                    if ext == '.json':
-                        json_edit(new, file_type, f_sub, og_sub, user_info, add_dict)
-            if types:
-                if dir_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}"):
-                    if file_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json"):
-                        with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'r') as file:
+                if dir_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}"): # add to change_log file
+                    if file_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json"):
+                        with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'r') as file:
                             data_add = json.load(file)
                             file_log['changes'] = {**data_add['changes'], **file_log['changes']}
-                    with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'w') as file:
+                    with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
+                        json.dump(file_log, file, indent=4)
+                else:
+                    mkdir(f"{WDIR}/BIDSit/Change_logs/{f_sub}")
+                    with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
                         json.dump(file_log, file, indent=4)
-                return new
-        if dir_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}"):
-            if file_exists(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json"):
-                with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'r') as file:
+                if f"input_Task-{task_ord[i]+1}-echo" in user_info[file_type].keys() and int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"]) >1: # send back file names to .json edit
+                    return [file_log['changes'][f"scan {i+1} echo {echo_num} new"] for echo_num in range(1, int(user_info[file_type][f"input_Task-{task_ord[i]+1}-echo"])+1)]
+                else:
+                    return [[file_log['changes'][f"scan {i+1} new"]], tasksLookedAt]
+            else: # all other data
+                tasksLookedAt, file_log, code = BIDSgo(og_sub, i, user_info, file_type, tasksLookedAt, exts, endings, menu, scans, task_ord, task_names, file_log, variables)
+            if stop:
+                break
+        if dir_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}"): # add to change_log file
+            if file_exists(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json"):
+                with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'r') as file:
                     data_add = json.load(file)
                     file_log['changes'] = {**data_add['changes'], **file_log['changes']}
-            with open(f"{WDIR}/rawdata/{f_sub}/{file_type}/change_log.json", 'w') as file:
+            with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
+                json.dump(file_log, file, indent=4)
+        else:
+            mkdir(f"{WDIR}/BIDSit/Change_logs/{f_sub}")
+            with open(f"{WDIR}/BIDSit/Change_logs/{f_sub}/{file_type}_change_log.json", 'w') as file:
                 json.dump(file_log, file, indent=4)
                 
 # - Edit json files - #
 def json_edit(json_f, file_type, f_sub, og_sub, info, *dicts):
     sub_solo = f_sub.split('/')[0]
     dic = {}
     for dict in dicts:
@@ -1000,60 +1243,66 @@
                 data['PhaseEncodingDirection'] = "j-" # Anterior to Posterior Phase Encoding Direction
             elif 'dir-PA' in json_f:
                  data['PhaseEncodingDirection'] = "j" # Posterior to Anterior Phase Encoding Direction
             if 'dir-LR' in json_f:
                 data['PhaseEncodingDirection'] = "i-" # Left to Right Phase Encoding Direction
             elif 'dir-RL' in json_f:
                  data['PhaseEncodingDirection'] = "i" # Right to Left Phase Encoding Direction
+        flag = False
         if file_type == 'fmap':
-            if 'rev' in json_f: # rev has to happen before in order to catch correctly
-                for key in dic:
-                    if 'rev' in key:
-                        f_list = dic[key] #AP
-                        files = []
-                        for item in f_list:
-                            file_t = item.split()[0] # file type to look at
-                            t_num = int(item.split()[-1])-1 # scan to look at
-                            if file_t in info:
-                                print(f"running BIDSit for on {file_t} for {og_sub}")
-                                files.append(BIDSit(og_sub, info, file_t, t_num))
-                        data['IntendedFor'] = files
-                        print(data['IntendedFor'])
-                        break
-            else:
-                for key in dic:
-                    f_list = dic[key] #AP
-                    files = []
-                    for item in f_list:
-                        file_t = item.split()[0] # file type to look at
-                        t_num = int(item.split()[-1])-1 # scan to look at
-                        if file_t in info:
-                            print(f"running BIDSit for on {file_t} for {og_sub}")
-                            files.append(BIDSit(og_sub, info, file_t, t_num))
-                    data['IntendedFor'] = files
-                    print(data['IntendedFor'])
+            flag = True
+            for key in dic:
+                f_list = dic[key] #AP
+                files = []
+                files_full = []
+                tasksLookedAt = []
+                for item in f_list:
+                    file_t = item.split()[0] # file type to look at
+                    t_num = int(item.split()[-1])-1 # scan to look at
+                    if file_t in info:
+                        print(f"running BIDSit for on {file_t} {t_num} for {og_sub}")
+                        these, tasksLookedAt = BIDSit(og_sub, info, file_t, t_num, tasksLookedAt)
+                        that = []
+                        for f in these:
+                            that.append("bids::" + f.split('rawdata/')[-1])
+                        files = files + that
+                        files_full = files_full + these
+                data['IntendedFor'] = files
+                break
+        elif file_type == 'func':
+            task_name = json_f.rsplit('/',1)[-1].split('_')
+            for unit in task_name:
+                if 'task' in unit:
+                    data['TaskName'] = unit.split('-')[-1]
                     break
+            
     with open(json_f, 'w') as file:
         json.dump(data, file, indent=4)
-    if 'IntendedFor' in data.keys():
-        for item in files:
-            item = item.split('.')[0] + ".json"
-            with open(item, 'r') as this:
-                datum = json.load(this)
-                if data['PhaseEncodingDirection'] == "j-":
-                    dict_add = {'PhaseEncodingDirection': "j"}
-                if data['PhaseEncodingDirection'] == "j":
-                    dict_add = {'PhaseEncodingDirection': "j-"}
-                if data['PhaseEncodingDirection'] == "i-":
-                    dict_add = {'PhaseEncodingDirection': "i"}
-                if data['PhaseEncodingDirection'] == "i":
-                    dict_add = {'PhaseEncodingDirection': "i-"}
-            datum = {**datum, **dict_add}
-            with open(item, 'w') as this:
-                json.dump(datum, this, indent=4)
+    if flag:
+        if 'IntendedFor' in data.keys():
+            for item in files_full:
+                item = item.split('.')[0] + ".json"
+                with open(item, 'r') as this:
+                    datum = json.load(this)
+                    if "Unknown" in datum['PhaseEncodingDirection']:
+                        if data['PhaseEncodingDirection'] == "j-":
+                            dict_add = {'PhaseEncodingDirection': "j"}
+                        elif data['PhaseEncodingDirection'] == "j":
+                            dict_add = {'PhaseEncodingDirection': "j-"}
+                        elif data['PhaseEncodingDirection'] == "i-":
+                            dict_add = {'PhaseEncodingDirection': "i"}
+                        elif data['PhaseEncodingDirection'] == "i":
+                            dict_add = {'PhaseEncodingDirection': "i-"}
+                        datum = {**datum, **dict_add}
+                        print("Changed PhaseEncodingDirection to: ", datum['PhaseEncodingDirection'] )
+                    else:
+                        print("Changed PhaseEncodingDirection to: ", datum['PhaseEncodingDirection'] )
+                with open(item, 'w') as this:
+                    json.dump(datum, this, indent=4)
+                    
 ### --- MISC Functions --- ###
 # - make a directory - #
 def mkdir(path,extension=''):
     path = os.path.join(path, extension)
     if not os.path.exists(path):
         os.makedirs(path)
 
@@ -1099,8 +1348,7 @@
     except OSError as exc:
         if exc.errno in (errno.ENOTDIR, errno.EINVAL):
             shutil.copy(src, dst)
         else: raise
     
 if __name__ == '__main__':
     main()
-
```

### Comparing `BIDSit-0.0.5/src/BIDSit/version.py` & `BIDSit-0.0.6/src/BIDSit/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 # Script Name: version.py                                                    #
 #                                                                            #
 # Description: specifies version for BIDSit                                  #
 #                                                                            #
 # Author:      Jen Burrell (April 17th, 2023)                                #
 #============================================================================#
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

### Comparing `BIDSit-0.0.5/src/BIDSit.egg-info/PKG-INFO` & `BIDSit-0.0.6/src/BIDSit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BIDSit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A BIDS conversion tool for fMRI data
 Home-page: https://github.com/jenburrell/BIDSit
 Author: Jen Burrell
 Author-email: jenbur@psych.ubc.ca
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

