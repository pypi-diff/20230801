# Comparing `tmp/wormcat_batch-1.1.0.tar.gz` & `tmp/wormcat_batch-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wormcat_batch-1.1.0.tar", last modified: Mon Jul 31 21:03:05 2023, max compression
+gzip compressed data, was "wormcat_batch-1.1.1.tar", last modified: Tue Aug  1 20:00:28 2023, max compression
```

## Comparing `wormcat_batch-1.1.0.tar` & `wormcat_batch-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.353602 wormcat_batch-1.1.0/
--rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.1.0/MANIFEST.in
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 21:03:05.353464 wormcat_batch-1.1.0/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2382 2023-07-31 16:03:44.000000 wormcat_batch-1.1.0/README.md
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-31 21:03:05.353643 wormcat_batch-1.1.0/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)      702 2023-07-31 21:01:44.000000 wormcat_batch-1.1.0/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.352328 wormcat_batch-1.1.0/wormcat_batch/
--rw-r--r--   0 dan        (501) staff       (20)     2109 2023-07-31 17:33:31.000000 wormcat_batch-1.1.0/wormcat_batch/create_wormcat_xlsx.py
--rw-r--r--   0 dan        (501) staff       (20)     2443 2023-07-31 16:16:50.000000 wormcat_batch-1.1.0/wormcat_batch/execute_r.py
--rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.0/wormcat_batch/is_wormcat_installed.R
--rwxr-xr-x   0 dan        (501) staff       (20)     8566 2023-07-31 20:54:46.000000 wormcat_batch-1.1.0/wormcat_batch/run_wormcat_batch.py
--rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.0/wormcat_batch/worm_cat.R
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-31 21:03:05.353299 wormcat_batch-1.1.0/wormcat_batch.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)      226 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)      451 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)       69 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/entry_points.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/not-zip-safe
--rw-r--r--   0 dan        (501) staff       (20)       32 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       14 2023-07-31 21:03:05.000000 wormcat_batch-1.1.0/wormcat_batch.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.128959 wormcat_batch-1.1.1/
+-rw-r--r--   0 dan        (501) staff       (20)       95 2022-08-16 12:41:26.000000 wormcat_batch-1.1.1/MANIFEST.in
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-01 20:00:28.128807 wormcat_batch-1.1.1/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2733 2023-08-01 19:34:44.000000 wormcat_batch-1.1.1/README.md
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-08-01 20:00:28.129001 wormcat_batch-1.1.1/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)      692 2023-08-01 18:25:58.000000 wormcat_batch-1.1.1/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.127594 wormcat_batch-1.1.1/wormcat_batch/
+-rw-r--r--   0 dan        (501) staff       (20)     3947 2023-08-01 17:11:31.000000 wormcat_batch-1.1.1/wormcat_batch/create_wormcat_xlsx.py
+-rw-r--r--   0 dan        (501) staff       (20)     2522 2023-08-01 19:01:04.000000 wormcat_batch-1.1.1/wormcat_batch/execute_r.py
+-rwxr-xr-x   0 dan        (501) staff       (20)       46 2022-08-16 12:41:26.000000 wormcat_batch-1.1.1/wormcat_batch/is_wormcat_installed.R
+-rwxr-xr-x   0 dan        (501) staff       (20)     8507 2023-08-01 18:54:19.000000 wormcat_batch-1.1.1/wormcat_batch/run_wormcat_batch.py
+-rwxr-xr-x   0 dan        (501) staff       (20)     1484 2023-07-31 16:25:55.000000 wormcat_batch-1.1.1/wormcat_batch/worm_cat.R
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-08-01 20:00:28.128575 wormcat_batch-1.1.1/wormcat_batch.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)      226 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)      451 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)       69 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/entry_points.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/not-zip-safe
+-rw-r--r--   0 dan        (501) staff       (20)       23 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       14 2023-08-01 20:00:28.000000 wormcat_batch-1.1.1/wormcat_batch.egg-info/top_level.txt
```

### Comparing `wormcat_batch-1.1.0/README.md` & `wormcat_batch-1.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 # Wormcat Batch
 
 ### Overview
 *Wormcat Batch* is a command line tool that allows you to batch multiple
-runs of Wormcat from a Microsoft Excel File.
+runs of [Wormcat](http://wormcat.com) from a Microsoft Excel File or a directory path with wormcat formatted csv files.
 
+**Note:** You can also run Wormcat Batch as a docker container. Find more information on running Wormcat Batch as a Docker container [here](https://hub.docker.com/repository/docker/danhumassmed/wormcat_batch/general).
 
 ### Prerequisites
 
 *Wormcat Batch* requires Python 3.5+ and R 3.4.1+ with a Wormcat
 package installed.
 
-If you are unsure if you have Wormcat installed you can run
+If you are unsure if you have Wormcat installed, you can run
 `find.package("wormcat")` from an R command prompt.
 
-If *Wormcat* is not install you can follow the directions
+If *Wormcat* is not installed, you can follow the directions
 [here](https://github.com/dphiggs01/Wormcat/blob/master/README.md)
-to install Wormcat. Note: Wormcat can be installed as an R package you
+to install Wormcat. 
+
+**Note:** Wormcat can be installed as an R package you;
 do NOT need to checkout the source unless you intend to modify Wormcat.
 The readme file explains how to install Wormcat as an R package.
 
 
 ### Excel spreadsheet Naming Conventions
 
-Once you have the R package installed you will create an Excel
+Once you have the R package installed, you will create an Excel
 Spreadsheet with the required data for batch execution.
 
 See the file `Example/Murphy_TS.xsl` for details.
 
 <img src="./Images/Sample_Input.png"  height="405" width="500"/>
 
-Note:
+**Note:**
 
 * The Spreadsheet Name should ONLY be composed of Letters, Numbers and
 Underscores (_) and has an extension .xlsx, .xlt, .xls
 * The Sheet Names within the spreadsheet should ONLY be composed of
-Letters, Numbers and Underscores (_) other characters may cause the
+Letters, Numbers, and Underscores (_) other characters may cause the
 batch process to fail!
 * Each sheet requires a column name 'Sequence ID' or 'Wormbase ID'
-(This column name is case sensitive)
+(This column name is case-sensitive)
 
 ### To Run the Batch Process
 
-To run the batch process open a terminal window, change directory to your
+To run the batch process, open a terminal window, change the directory to your
 project directory.
 
 ```
 $pip install wormcat_batch
-$wormcat_cli
+$wormcat_cli --help
 ```
 
 <img src="./Images/Example_Run.png"  height="288" width="800"/>
 
 
-After execution the Output Directory will contain all the Wormcat run data and a
+After execution, the Output Directory will contain all the Wormcat run data and a
 summary Excel spreadsheet.
 
 
 
 ### Sample Output
 
 
 <img src="./Images/Sample_Output.png"  height="415" width="800"/>
 
 ### Local development /test hints
 
 #### Setup to test
-conda activate <appropriate_env>
-pip install .
+* conda activate <appropriate_env>
+* pip install .
 
 #### Test
-cd /Users/dan/delme #some working directory
-wormcat_cli --input-excel /Users/dan/Code/Python/Wormcat_batch/Example/Murphy_TS.xlsx --output-path ./output  
+* cd /Users/dan/delme #some working directory
+* wormcat_cli --input-excel ${PROJ_HOME}/Example/Murphy_TS.xlsx --output-path ./output  
 
 #### Deploy
-advance version='1.0.9' in setup.py
-conda deactivate # twine is installed in base env
-cd in project directory
-rm -rf ./dist
-rm -rf ./wormcat_batch.egg-info
-python setup.py sdist
-twine check dist/*
-twine upload --repository pypi dist/*
-git add .
-git commit -m "some comment"
-git push
+* Advance the version number in setup.py
+* `conda deactivate # twine is installed in base env`
+* `cd <project directory>`
+* `rm -rf ./dist`
+* `rm -rf ./wormcat_batch.egg-info`
+* `python setup.py sdist`
+* `twine check dist/*`
+* `twine upload --repository pypi dist/*`
+* `git add .`
+* `git commit -m "some comment"`
+* `git push`
```

### Comparing `wormcat_batch-1.1.0/setup.py` & `wormcat_batch-1.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 # rm -rf dist
 # python setup.py sdist
-#pip install dist/wormcat_batch-1.0.1.tar.gz
+# pip install dist/wormcat_batch-1.0.1.tar.gz
 # twine check dist/*
 # twine upload --repository pypi dist/*
 
 setup(name='wormcat_batch',
-      version='1.1.0',
+      version='1.1.1',
       description='Batch processing for Wormcat data',
       url='https://github.com/dphiggs01/Wormcat_batch',
       author='Dan Higgins',
       author_email='daniel.higgins@yahoo.com',
       license='MIT',
 
       packages=['wormcat_batch'],
-      install_requires=['pandas','xlrd','xlsxwriter','openpyxl'],
+      install_requires=['pandas','xlrd','xlsxwriter'],
       entry_points={
           'console_scripts': ['wormcat_cli=wormcat_batch.run_wormcat_batch:main'],
       },
       include_package_data=True,
       zip_safe=False)
```

### Comparing `wormcat_batch-1.1.0/wormcat_batch/execute_r.py` & `wormcat_batch-1.1.1/wormcat_batch/execute_r.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 
     def wormcat_library_path_fun(self):
         ret_val = self.run(self.wormcat_library_path,"")
         return ret_val
 
     def worm_cat_fun(self, file_name, out_dir, title, annotation_file, input_type):
+        print(f"Calling Wormcat with {os.path.basename(file_name)[:-4]} data")
         ret_val = self.run(self.worm_cat_function, file_name, title, out_dir, "False", annotation_file, input_type, "False")
         return ret_val
 
     def run(self, arg_list, *args):
         try:
             processed_args = self.process_args(arg_list, *args)
             process = Popen(processed_args, stdout=PIPE)
```

### Comparing `wormcat_batch-1.1.0/wormcat_batch/run_wormcat_batch.py` & `wormcat_batch-1.1.1/wormcat_batch/run_wormcat_batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import sys
 import argparse
 import pandas as pd
 import shutil
 import zipfile
-import json
 import importlib.metadata
 from datetime import datetime
 from wormcat_batch.execute_r import ExecuteR
 from wormcat_batch.create_wormcat_xlsx import process_category_files
 
 import warnings
 warnings.filterwarnings('ignore', category=UserWarning, module='openpyxl')
@@ -39,16 +38,17 @@
             wormcat_output_dir = f'{wormcat_out_path}{os.path.sep}{file_nm_wo_ext}'
             executeR = ExecuteR()
             executeR.worm_cat_fun(conetnt_full_path, wormcat_output_dir, title, annotation_file, wormcat_input_type)
     return wormcat_out_path
 
 def create_summary_spreadsheet(wormcat_out_path, annotation_file, out_xsl_file_nm):
     '''
-    After all the sheets on the Excel have been executed create a dataframe that can be used to summarize the results
-    this dataframe is used to create the output Excel
+    After all the sheets on the Excel have been executed or CSV files processed 
+    create a dataframe that can be used to summarize the results.
+    This dataframe is used to create the output Excel.
     '''
     process_lst = []
     for dir_nm in os.listdir(wormcat_out_path):
         for cat_num in [1,2,3]:
             rgs_fisher = f"{wormcat_out_path}{os.path.sep}{dir_nm}{os.path.sep}rgs_fisher_cat{cat_num}.csv"
             cat_nm = f"Cat{cat_num}"
             row = {'sheet': cat_nm, 'category': cat_num, 'file': rgs_fisher,'label': dir_nm}
@@ -68,20 +68,20 @@
     if path:
         first_quote=path.find('"')
         last_quote=path.rfind('"')
         if last_quote == -1:
             print("Wormcat is not installed or cannot be found.")
             exit(-1)
         path = path[first_quote+1:last_quote]
-    print(f"wormcat_lib_path={path}")
+    # print(f"wormcat_lib_path={path}")
     return path
 
 def get_category_files(path):
     '''
-    get the list of available annotation files for Wormcat.
+    Get the list of available annotation files for Wormcat.
     These files exist in the R wormcat install under the "extdata" directory
     '''
     category_files=[]
     index=1
     path = "{}{}extdata".format(path, os.path.sep)
     for root, dirs, files in os.walk(path):
         for filename in files:
@@ -93,43 +93,44 @@
 ## Utility functions
 
 def create_directory(directory, with_backup=False):
     '''
     Utility function to create a directory and backup the original if it exists and has content
     '''
     if with_backup and os.path.exists(directory) and os.listdir(directory):
-        print(f"Directory exists with content [{directory}]")
+        print(f"Creating backup of existing directory [{directory}]")
         # Create backup directory name with a unique timestamp suffix
         timestamp = datetime.now().strftime("%Y%m%d-%H%M%S")
         backup_dir = f"{directory}_{timestamp}.bk"
-        # Create a backup of the existing directory
         shutil.move(directory, backup_dir)
 
-    # Create a new empty directory
     os.makedirs(directory, exist_ok=True)
 
 def zip_directory(directory_path, zip_file_name):
+    '''
+    Compress the content of a directory in zip format.
+    '''
     with zipfile.ZipFile(zip_file_name, 'w') as zipf:
         for root, _, files in os.walk(directory_path):
             for file in files:
                 file_path = os.path.join(root, file)
                 zipf.write(file_path, os.path.relpath(file_path, directory_path))
 
 
 ##########################################################
 
 def main():
-    print("Wormcat Batch")
+    print("Starting Wormcat Batch")
     parser = argparse.ArgumentParser()
     help_statement="wormcat_cli --input-excel <path_to_excel> | --input-csv-path <path_to_csv> --output-path <path_to_out_dir> --annotation-file 'whole_genome_v2_nov-11-2021.csv' --clean-temp False"
     parser.add_argument('-i', '--input-excel', help='Input file in Excel/Wormcat format')
     parser.add_argument('-c', '--input-csv-path', help='Input path to a collection of CSV files in Wormcat format')
     parser.add_argument('-o', '--output-path', help='Output path')
     parser.add_argument('-a', '--annotation-file', default='whole_genome_v2_nov-11-2021.csv', help='Annotation file name or path default=whole_genome_v2_nov-11-2021.csv')
-    parser.add_argument('-t', '--clean-temp', default=False, help='Remove files created while processing default=False')
+    parser.add_argument('-t', '--clean-temp', default='False', help='Remove files created while processing default=False')
 
     parser.add_argument('-v', '--version', action='version', version=f'%(prog)s v{importlib.metadata.version("wormcat_batch")}')
     args = parser.parse_args()
 
     if not args.input_excel and not args.input_csv_path:
         print(help_statement)
         print("An Excel Input file or a path to CSV files is required.")
@@ -150,18 +151,18 @@
         if not args.annotation_file or not args.annotation_file in annotation_files:
             print(help_statement)
             print("Missing or incorrect annotation-file-nm.")
             print("Available names: {}".format(annotation_files))
             return
         annotation_file_path = f"{wormcat_path}{os.path.sep}extdata{os.path.sep}{args.annotation_file}"
     
-    print("Input Excel:", args.input_excel)
-    print("Input CSV Path:", args.input_csv_path)
-    print("Output Path:", args.output_path)
-    print("Annotation File:", args.annotation_file)
+    if args.clean_temp.lower().title() == 'True':
+        clean_temp = True
+    else:
+        clean_temp = False
 
     # Create the output directory if it does not exsist
     # Create a backup of the directory if it does exist and has content
     create_directory(args.output_path, with_backup=True)
 
     # If needed Extract the sreadsheet data
     if args.input_csv_path:
@@ -192,14 +193,14 @@
     create_summary_spreadsheet(wormcat_out_path, annotation_file_path, out_xsl_file_nm)
     
     # Zip the results
     zip_dir_nm = f"{args.output_path}{os.path.sep}{output_base_dir}.zip"
     zip_directory(wormcat_out_path, zip_dir_nm)
     
     # If set Remove files created while processing
-    if args.clean_temp:
+    if clean_temp:
         shutil.rmtree(wormcat_out_path)
         if args.input_excel:
             shutil.rmtree(csv_file_path)
 
 if __name__ == '__main__':
     main()
```

### Comparing `wormcat_batch-1.1.0/wormcat_batch/worm_cat.R` & `wormcat_batch-1.1.1/wormcat_batch/worm_cat.R`

 * *Files identical despite different names*

