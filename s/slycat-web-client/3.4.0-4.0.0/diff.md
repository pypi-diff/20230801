# Comparing `tmp/slycat-web-client-3.4.0.tar.gz` & `tmp/slycat-web-client-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slycat-web-client-3.4.0.tar", last modified: Tue Mar 14 15:45:25 2023, max compression
+gzip compressed data, was "slycat-web-client-4.0.0.tar", last modified: Tue Aug  1 14:02:06 2023, max compression
```

## Comparing `slycat-web-client-3.4.0.tar` & `slycat-web-client-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)        0 2023-03-14 15:45:25.857522 slycat-web-client-3.4.0/
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     3372 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/LICENSE
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)       94 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/MANIFEST.in
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     9616 2023-03-14 15:45:25.857209 slycat-web-client-3.4.0/PKG-INFO
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     9148 2022-10-25 21:25:07.000000 slycat-web-client-3.4.0/README.md
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)       38 2023-03-14 15:45:25.857622 slycat-web-client-3.4.0/setup.cfg
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     3281 2023-03-13 15:09:59.000000 slycat-web-client-3.4.0/setup.py
-drwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)        0 2023-03-14 15:45:25.849081 slycat-web-client-3.4.0/slycat/
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)      286 2023-03-14 15:45:24.000000 slycat-web-client-3.4.0/slycat/__init__.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     8099 2023-03-14 15:45:24.000000 slycat-web-client-3.4.0/slycat/darray.py
-drwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)        0 2023-03-14 15:45:25.849428 slycat-web-client-3.4.0/slycat/web/
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)      265 2023-03-14 15:45:24.000000 slycat-web-client-3.4.0/slycat/web/__init__.py
-drwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)        0 2023-03-14 15:45:25.854511 slycat-web-client-3.4.0/slycat/web/client/
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)    49325 2023-03-14 15:45:24.000000 slycat-web-client-3.4.0/slycat/web/client/__init__.py
--rwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)     4903 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/cca_csv.py
--rwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)     6270 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/cca_random.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     1562 2022-10-24 22:12:42.000000 slycat-web-client-3.4.0/slycat/web/client/dac_defaults.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     4045 2023-03-02 17:10:49.000000 slycat-web-client-3.4.0/slycat/web/client/dac_gen.py
--rwxr-x---   0 smartin  (20160) SANDIA\Domain Users (1049671531)    31315 2023-03-14 15:35:42.000000 slycat-web-client-3.4.0/slycat/web/client/dac_run_chart.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)    14562 2023-03-02 17:12:24.000000 slycat-web-client-3.4.0/slycat/web/client/dac_tdms.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     3940 2021-08-03 13:50:40.000000 slycat-web-client-3.4.0/slycat/web/client/dac_tdms_batch.py
--rwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)      620 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/get_model.py
--rwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)      633 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/get_project.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     1445 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/list_markings.py
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     1015 2021-07-15 15:56:26.000000 slycat-web-client-3.4.0/slycat/web/client/list_projects.py
--rwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)     9289 2023-03-02 17:12:21.000000 slycat-web-client-3.4.0/slycat/web/client/ps_csv.py
-drwxr-xr-x   0 smartin  (20160) SANDIA\Domain Users (1049671531)        0 2023-03-14 15:45:25.856706 slycat-web-client-3.4.0/slycat_web_client.egg-info/
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)     9616 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/PKG-INFO
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)      762 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/SOURCES.txt
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)        1 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/dependency_links.txt
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)      196 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/entry_points.txt
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)       64 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/requires.txt
--rw-r--r--   0 smartin  (20160) SANDIA\Domain Users (1049671531)        7 2023-03-14 15:45:25.000000 slycat-web-client-3.4.0/slycat_web_client.egg-info/top_level.txt
+drwxr-xr-x   0 smartin  (20160) 1049671531        0 2023-08-01 14:02:06.623293 slycat-web-client-4.0.0/
+-rw-r--r--   0 smartin  (20160) 1049671531     3372 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/LICENSE
+-rw-r--r--   0 smartin  (20160) 1049671531       94 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/MANIFEST.in
+-rw-r--r--   0 smartin  (20160) 1049671531     9974 2023-08-01 14:02:06.622748 slycat-web-client-4.0.0/PKG-INFO
+-rw-r--r--   0 smartin  (20160) 1049671531     9506 2023-07-31 21:10:21.000000 slycat-web-client-4.0.0/README.md
+-rw-r--r--   0 smartin  (20160) 1049671531       38 2023-08-01 14:02:06.623497 slycat-web-client-4.0.0/setup.cfg
+-rw-r--r--   0 smartin  (20160) 1049671531     3480 2023-08-01 13:59:09.000000 slycat-web-client-4.0.0/setup.py
+drwxr-xr-x   0 smartin  (20160) 1049671531        0 2023-08-01 14:02:06.601693 slycat-web-client-4.0.0/slycat/
+-rw-r--r--   0 smartin  (20160) 1049671531      286 2023-08-01 14:02:05.000000 slycat-web-client-4.0.0/slycat/__init__.py
+-rw-r--r--   0 smartin  (20160) 1049671531     8099 2023-08-01 14:02:05.000000 slycat-web-client-4.0.0/slycat/darray.py
+-rw-r--r--   0 smartin  (20160) 1049671531     4928 2023-08-01 14:02:05.000000 slycat-web-client-4.0.0/slycat/pandas_util.py
+drwxr-xr-x   0 smartin  (20160) 1049671531        0 2023-08-01 14:02:06.602321 slycat-web-client-4.0.0/slycat/web/
+-rw-r--r--   0 smartin  (20160) 1049671531      265 2023-08-01 14:02:05.000000 slycat-web-client-4.0.0/slycat/web/__init__.py
+drwxr-xr-x   0 smartin  (20160) 1049671531        0 2023-08-01 14:02:06.616119 slycat-web-client-4.0.0/slycat/web/client/
+-rw-r--r--   0 smartin  (20160) 1049671531    49325 2023-08-01 14:02:05.000000 slycat-web-client-4.0.0/slycat/web/client/__init__.py
+-rwxr-xr-x   0 smartin  (20160) 1049671531     4903 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/cca_csv.py
+-rwxr-xr-x   0 smartin  (20160) 1049671531     6270 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/cca_random.py
+-rw-r--r--   0 smartin  (20160) 1049671531     1562 2022-10-24 22:12:42.000000 slycat-web-client-4.0.0/slycat/web/client/dac_defaults.py
+-rw-r--r--   0 smartin  (20160) 1049671531     4045 2023-03-02 17:10:49.000000 slycat-web-client-4.0.0/slycat/web/client/dac_gen.py
+-rwxr-x---   0 smartin  (20160) 1049671531    25928 2023-07-31 20:27:22.000000 slycat-web-client-4.0.0/slycat/web/client/dac_run_chart.py
+-rw-r--r--   0 smartin  (20160) 1049671531     9995 2023-07-31 19:49:21.000000 slycat-web-client-4.0.0/slycat/web/client/dac_tdms.py
+-rw-r--r--   0 smartin  (20160) 1049671531     6982 2023-07-31 20:00:37.000000 slycat-web-client-4.0.0/slycat/web/client/dac_tdms_batch.py
+-rw-r--r--   0 smartin  (20160) 1049671531     4169 2023-07-31 21:00:38.000000 slycat-web-client-4.0.0/slycat/web/client/dac_tdms_batch_file.py
+-rw-r--r--   0 smartin  (20160) 1049671531    11283 2023-07-31 18:16:49.000000 slycat-web-client-4.0.0/slycat/web/client/dac_tdms_util.py
+-rwxr-xr-x   0 smartin  (20160) 1049671531      620 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/get_model.py
+-rwxr-xr-x   0 smartin  (20160) 1049671531      633 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/get_project.py
+-rw-r--r--   0 smartin  (20160) 1049671531     1445 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/list_markings.py
+-rw-r--r--   0 smartin  (20160) 1049671531     1015 2021-07-15 15:56:26.000000 slycat-web-client-4.0.0/slycat/web/client/list_projects.py
+-rwxr-xr-x   0 smartin  (20160) 1049671531     9878 2023-08-01 13:47:45.000000 slycat-web-client-4.0.0/slycat/web/client/ps_csv.py
+drwxr-xr-x   0 smartin  (20160) 1049671531        0 2023-08-01 14:02:06.621900 slycat-web-client-4.0.0/slycat_web_client.egg-info/
+-rw-r--r--   0 smartin  (20160) 1049671531     9974 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/PKG-INFO
+-rw-r--r--   0 smartin  (20160) 1049671531      860 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/SOURCES.txt
+-rw-r--r--   0 smartin  (20160) 1049671531        1 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/dependency_links.txt
+-rw-r--r--   0 smartin  (20160) 1049671531      261 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/entry_points.txt
+-rw-r--r--   0 smartin  (20160) 1049671531       76 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/requires.txt
+-rw-r--r--   0 smartin  (20160) 1049671531        7 2023-08-01 14:02:06.000000 slycat-web-client-4.0.0/slycat_web_client.egg-info/top_level.txt
```

### Comparing `slycat-web-client-3.4.0/LICENSE` & `slycat-web-client-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/PKG-INFO` & `slycat-web-client-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slycat-web-client
-Version: 3.4.0
+Version: 4.0.0
 Summary: Slycat web client utilties for interacting with the Slycat data analysis and visualization server.
 Home-page: https://github.com/sandialabs/slycat
 Author: Shawn Martin
 Author-email: smartin@sandia.gov
 License: Sandia
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -67,24 +67,23 @@
 
 or
 
 ```sh
 $ python -m slycat.web.client.list_markings
 ```
 
-In addition, there are two entry points defined for the Slycat Dial-A-Cluster plugin
+In addition, there are two main entry points defined for the Slycat Dial-A-Cluster plugin
 
 ```sh
 $ dac_tdms
 ```
-
 and
 
 ```sh
-$ dac_tdms_batch
+$ dac_gen
 ```
 
 These are described in greater detail below.
 
 ## User Authentication
 
 The Slycat server requires user authentication.  The slycat.web.client
@@ -208,36 +207,45 @@
 
 This will create a model from a single .TDM file.  You can also use .TDMS
 files and .zip archives containing .tdms files.  The options available
 for the creation of the models are the same as the options available using
 the DAC model creation wizard in the browser.  To see the options use
 the "--help" flag when calling the script.
 
-In addition, a batch script is available for uploading multiple DAC TDMS
-models.  To use this script, you must first create a file containing the
-options for each model.  The file has the following format.
+In addition, there are two methods for uploading batches of multiple DAC
+TDMS models.  The first method uses the dac_tdms_batch script.  This script
+takes as input a part-num match (see also dac_run_chart) and creates
+the corresponding batches.  For example,
+
+```sh
+$ dac_tdms_batch root-data-directory part-num
+```
+
+The second method uses the dac_tdms_batch_file script.  To use this script, 
+you must first create a file containing the options for each model.  The file 
+has the following format.
 
 Line 1 contains the authentication information for the Slycat server that
 you would pass to the dac_tdms script, but separated by commas.
 For example,
 
-    --user,smartin,--kerberos
+    --user,user-name,--kerberos
 
 If authentication information is unnecessary, just leave the line blank.
 
 Line 2 contains the project information for the project that will contain
 the DAC models to be created, e.g.
 
     --project-name,Batch TDMS Models
 
 Line 2 can also be left blank.  It will default to "Batch TDMS Models".
 Lines 3 and beyond contain the model information for each model, such as
 
-    model-data-file-1.tdms,--model-name,Model 1
-    model-data-file-2.tdms,--model-name,Model 2
+    model-data-file-1.tdms,--model-name,Model 1,--project-name,Batch TDMS Models
+    model-data-file-2.tdms,--model-name,Model 2,--project-name,Batch TDMS Models
 
 Note that you must supply a model file (or multiple files) in accordance
 with the dac_tdms script for each model.  Also note that if 
 you want to put models into different projects, you can override the 
 original project given in line 2, by using the "--project-name" flag 
 again, e.g.
```

### Comparing `slycat-web-client-3.4.0/README.md` & `slycat-web-client-4.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,24 +53,23 @@
 
 or
 
 ```sh
 $ python -m slycat.web.client.list_markings
 ```
 
-In addition, there are two entry points defined for the Slycat Dial-A-Cluster plugin
+In addition, there are two main entry points defined for the Slycat Dial-A-Cluster plugin
 
 ```sh
 $ dac_tdms
 ```
-
 and
 
 ```sh
-$ dac_tdms_batch
+$ dac_gen
 ```
 
 These are described in greater detail below.
 
 ## User Authentication
 
 The Slycat server requires user authentication.  The slycat.web.client
@@ -194,36 +193,45 @@
 
 This will create a model from a single .TDM file.  You can also use .TDMS
 files and .zip archives containing .tdms files.  The options available
 for the creation of the models are the same as the options available using
 the DAC model creation wizard in the browser.  To see the options use
 the "--help" flag when calling the script.
 
-In addition, a batch script is available for uploading multiple DAC TDMS
-models.  To use this script, you must first create a file containing the
-options for each model.  The file has the following format.
+In addition, there are two methods for uploading batches of multiple DAC
+TDMS models.  The first method uses the dac_tdms_batch script.  This script
+takes as input a part-num match (see also dac_run_chart) and creates
+the corresponding batches.  For example,
+
+```sh
+$ dac_tdms_batch root-data-directory part-num
+```
+
+The second method uses the dac_tdms_batch_file script.  To use this script, 
+you must first create a file containing the options for each model.  The file 
+has the following format.
 
 Line 1 contains the authentication information for the Slycat server that
 you would pass to the dac_tdms script, but separated by commas.
 For example,
 
-    --user,smartin,--kerberos
+    --user,user-name,--kerberos
 
 If authentication information is unnecessary, just leave the line blank.
 
 Line 2 contains the project information for the project that will contain
 the DAC models to be created, e.g.
 
     --project-name,Batch TDMS Models
 
 Line 2 can also be left blank.  It will default to "Batch TDMS Models".
 Lines 3 and beyond contain the model information for each model, such as
 
-    model-data-file-1.tdms,--model-name,Model 1
-    model-data-file-2.tdms,--model-name,Model 2
+    model-data-file-1.tdms,--model-name,Model 1,--project-name,Batch TDMS Models
+    model-data-file-2.tdms,--model-name,Model 2,--project-name,Batch TDMS Models
 
 Note that you must supply a model file (or multiple files) in accordance
 with the dac_tdms script for each model.  Also note that if 
 you want to put models into different projects, you can override the 
 original project given in line 2, by using the "--project-name" flag 
 again, e.g.
```

### Comparing `slycat-web-client-3.4.0/setup.py` & `slycat-web-client-4.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,21 +39,24 @@
 copyfile('../packages/slycat/web/client/__init__.py', 'slycat/web/client/__init__.py')
 copyfile('../packages/slycat/darray.py', 'slycat/darray.py')
 
 # also copy the __init__.py files, which include the Slycat version number
 copyfile('../packages/slycat/__init__.py', 'slycat/__init__.py')
 copyfile('../packages/slycat/web/__init__.py', 'slycat/web/__init__.py')
 
+# we also need the slycat csv parser
+copyfile('../packages/slycat/pandas_util.py', 'slycat/pandas_util.py')
+
 # get Slycat version
 import slycat
 VERSION = slycat.__version__
 
 # development version
 # VERSION = VERSION
-VERSION = "3.4.0"
+VERSION = "4.0.0"
 
 # get README.md
 import pathlib
 
 # directory containing this file
 HERE = pathlib.Path(__file__).parent
 
@@ -80,18 +83,19 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
     ],
     packages=setuptools.find_packages(),
     include_package_data=True,
     install_requires=["requests", "requests-kerberos",
-                      "numpy", "cherrypy", "sklearn", 
-                      "nptdms", "pandas"],
+                      "numpy", "cherrypy", "scikit-learn", 
+                      "nptdms==1.6.0", "pandas"],
     entry_points={
         "console_scripts": [
             "dac_tdms=slycat.web.client.dac_tdms:main",
             "dac_tdms_batch=slycat.web.client.dac_tdms_batch:main",
+            "dac_tdms_batch_file=slycat.web.client.dac_tdms_batch_file:main",
             "ps_csv=slycat.web.client.ps_csv:main",
             "dac_gen=slycat.web.client.dac_gen:main"
         ]
     },
 )
```

### Comparing `slycat-web-client-3.4.0/slycat/darray.py` & `slycat-web-client-4.0.0/slycat/darray.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/__init__.py` & `slycat-web-client-4.0.0/slycat/web/client/__init__.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/cca_csv.py` & `slycat-web-client-4.0.0/slycat/web/client/cca_csv.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/cca_random.py` & `slycat-web-client-4.0.0/slycat/web/client/cca_random.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/dac_defaults.py` & `slycat-web-client-4.0.0/slycat/web/client/dac_defaults.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/dac_gen.py` & `slycat-web-client-4.0.0/slycat/web/client/dac_gen.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/dac_run_chart.py` & `slycat-web-client-4.0.0/slycat/web/client/dac_run_chart.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,17 +11,20 @@
 
 # connection to Slycat server
 import slycat.web.client
 
 # DAC upload
 import slycat.web.client.dac_gen as dac_gen
 
+# common tdms operations
+import slycat.web.client.dac_tdms_util as dac_tdms_util
+from slycat.web.client.dac_tdms_util import TDMSUploadError
+
 # file name manipulation
 import os
-import fnmatch
 
 # manipulating command line arguments
 from argparse import Namespace
 
 # processing tables
 import numpy as np
 
@@ -32,161 +35,26 @@
 import nptdms
 import pandas as pd
 
 # output zip file
 from zipfile import ZipFile
 
 # the tdms file types allowed
-TDMS_MATCHES = ['Factory_Trigger', 'Acceptance_Trigger', 'Pulse_Life', 
+TDMS_MATCHES = ['Factory_Trigger', 'Acceptance_Trigger', 'PL', 'Pulse_Life', 
                 'Extended_Pulse_Life', 'Probe_Age']
 
 # the group run chart variables allowed
 RUN_CHART_MATCHES = ['TAD', 'Rp', 'Ip', 'DBV']
 RUN_CHART_UNITS = ['nsec', 'kOhms', 'Amps', 'V']
 
-# TDMS error handling
-class TDMSUploadError (Exception):
-
-    # exception for TDMS upload problems
-    def __init__(self, message):
-        self.message = message
-
-# parse test data subdirectory
-def parse_run_chart (run_chart):
-
-    # default return is None
-    run_chart_id = None
-
-    # split run_chart string on "_" to get identifiers
-    run_chart_id = run_chart.split("_")
-
-    # there should be four identifiers
-    if len(run_chart_id) != 4:
-        run_chart_id = None
-    
-    return run_chart_id
-
 # organize tdms files based on command line inputs
 def catalog_tdms_files (arguments, log):
 
-    # gather data directories for given part number
-    root_dir = arguments.input_data_dir
-    part_num_match = arguments.part_num_match
-
-    # check that root dir exists
-    if not os.path.isdir(root_dir):
-        raise TDMSUploadError("Input data directory does not exist.  Please provide " +
-              "a different directory and try again.")
-    
-    # look for directories containing data for part number provided
-    root_subdirs = os.listdir(root_dir)
-    part_subdirs = fnmatch.filter(root_subdirs, part_num_match)
-    
-    # are there any subdirectories?
-    if len(part_subdirs) == 0:
-        raise TDMSUploadError('Could not find any subdirectories for part number matching "' +
-              part_num_match + '".')
-
-    # put subdirectories in order
-    part_subdirs.sort()
-
-    # get list of .tdms file matches
-    tdms_matches = TDMS_MATCHES
-    if arguments.tdms_file_matches is not None:
-        tdms_matches = arguments.tdms_file_matches
-    tdms_matches = [file_match.replace('_', ' ') for file_match in tdms_matches]
-
-    # report on tdms file being used
-    log("Using .tdms file matches in: " + str(tdms_matches))
-
-    # look through each subdirectory for run chart data
-    metadata = []
-    for subdir in part_subdirs:
-
-        # look for test data directory
-        test_data_dir = os.path.join(root_dir, subdir, 'Test Data')
-
-        # skip if run_chart_dir is not an actual directory
-        if not os.path.isdir(test_data_dir):
-            log('Skipping "' + test_data_dir + '" because it''s not a directory.')
-            continue
-
-        # each of the subdirectories of run_chart_dir will be a row in the 
-        # metadata table for the run chart model
-        possible_run_chart_dirs = os.listdir(test_data_dir)
-
-        # sort according to data ids
-        possible_run_chart_dirs.sort()
-
-        # check that we found data directories
-        if len(possible_run_chart_dirs) == 0:
-            raise TDMSUploadError('No data subdirectories found for part number match "' + 
-                  part_num_match + '".')
-
-        # check that data directories conform to expected format
-        for run_chart_dir in possible_run_chart_dirs:
-
-            # check that directory is expected format for a run chart
-            run_chart_ids = parse_run_chart(run_chart_dir)
-
-            # if it's not a run chart then skip it
-            if run_chart_ids is None:
-                log('Skipping run chart subdirectory "' + run_chart_dir + 
-                    '" because it does not conform to "part_lot_batch_serial" string format.')
-                continue
-        
-            # find .tdms files in run chart directory
-            run_chart_files = os.listdir(os.path.join(test_data_dir, run_chart_dir))
-            run_chart_tdms_files = [run_chart_file for run_chart_file in run_chart_files 
-                                    if run_chart_file.endswith('.tdms')]
-        
-            # check that we have .tdms files
-            if len(run_chart_tdms_files) == 0:
-                log ('Skipping subdirectory "' + run_chart_ids[0] + '" -- does not ' +
-                      'contain any TDMS files.')
-                continue
-
-            # screen for .tdms files according to argument parameters
-            run_chart_tdms_matches = []
-            run_chart_tdms_types = []
-            for run_chart_file in run_chart_tdms_files:
-                for match in tdms_matches:
-                    if match in run_chart_file:
-
-                        # check that .tdms file has matching part_lot_batch_sn
-                        if not run_chart_file.startswith(
-                            run_chart_ids[0] + "_" + 
-                            run_chart_ids[1] + "_" + 
-                            run_chart_ids[2] + "_" + 
-                            run_chart_ids[3]):
-                            continue
-                        
-                        # keep track of files and types
-                        run_chart_tdms_types.append(match)
-                        run_chart_tdms_matches.append(run_chart_file)
-
-            # check that we have matching .tdms files
-            if len(run_chart_tdms_matches) == 0:
-                log ('Skipping subdirectory "' + run_chart_ids[0] + '" -- does not ' +
-                      'contain any TDMS files with file matches.')
-                continue
-
-            # store in metadata structure
-            metadata.append({"part": run_chart_ids[0],
-                             "lot": run_chart_ids[1],
-                             "batch": run_chart_ids[2],
-                             "sn": run_chart_ids[3],
-                             "source": os.path.join(os.path.abspath(test_data_dir), 
-                                                    run_chart_dir),
-                             "tdms_files": run_chart_tdms_matches,
-                             "tdms_types": run_chart_tdms_types})
-
-    # check that files were found
-    if metadata == []:
-        raise TDMSUploadError("No TDMS files matching selection criterion were found.")
+    # read all meta data before further run chart specific filtering
+    metadata = dac_tdms_util.catalog_tdms_files(arguments, log, TDMS_MATCHES)
 
     # get common set of tdms types
     common_tdms_types = set(metadata[0]["tdms_types"])
     intersection_flag = False
     for row in range(len(metadata)):
 
         # set intersection
@@ -729,15 +597,15 @@
         help="Delete output .zip file after successful model creation).")
 
     # do not upload to slycat
     parser.add_argument("--do-not-upload", action="store_true",
         help="Do not upload to slycat server.")
 
     # model and project names/descriptions
-    parser.add_argument("--marking", default="ouo3", 
+    parser.add_argument("--marking", default="cui", 
         help="Marking type.  Default: %(default)s")
     parser.add_argument("--model-description", default="", 
         help="New model description.  Default: %(default)s")
     parser.add_argument("--model-name", default="DAC Run Chart Model", 
         help="New model name.  Default: %(default)s")
     parser.add_argument("--project-description", default="", 
         help="New project description.  Default: %(default)s")
```

### Comparing `slycat-web-client-3.4.0/slycat/web/client/dac_tdms.py` & `slycat-web-client-4.0.0/slycat/web/client/dac_tdms.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,28 +13,23 @@
 # 10/21/2020
 
 # connection to Slycat server
 import slycat.web.client
 
 # DAC UI defaults
 from slycat.web.client.dac_defaults import dac_model_defaults
+import slycat.web.client.dac_tdms_util as dac_tdms_util
+from slycat.web.client.dac_tdms_util import TDMSUploadError
 
 # file name manipulation
 import os
 
 # get suffixes from zip file
 import zipfile
 
-# TDMS error handling
-class TDMSUploadError (Exception):
-
-    # exception for TDMS upload problems
-    def __init__(self, message):
-        self.message = message
-
 # check for .TDM, .tdms, or a single .zip file extension
 # returns "not-tdms" for wrong extension, "tdms" for correct extensions,
 # "zip" for a single .zip file
 def check_file_extensions (file_list):
 
     # a single file can end with .zip, .TDM, or .tdms
     if len(file_list) == 1:
@@ -65,65 +60,14 @@
 
     for file in file_list:
         if not os.path.isfile(file):
             files_exist = False
 
     return files_exist
 
-# check the parser parameters
-def check_parser_parms (parms):
-
-    check_parser_msg = []
-
-    # first parameter is minimum number of time points
-    if parms[0] < 2:
-        check_parser_msg.append ("Each channel must have at least two values. " + \
-            "Please use a larger value for min-time-points and try again.")
-    
-    # second parameter is minimum number of channels
-    if parms[1] < 1:
-        check_parser_msg.append ("Each test must have at least one channel. " + \
-            "Please use a larger value for min-channels and try again.")
-    
-    # third parameter is minimum number of shots
-    if parms[2] < 0:
-        check_parser_msg.append("Each channel must occur in at least one channel " + \
-            "(use 0 to indicate every channel).  Please use a non-negative value " + \
-            "for min-num-shots and try again.")
-
-    # fourth parameter is number of landmarks
-    if parms[3] is not None:
-        if not (parms[3] == 0 or parms[3] >= 3):
-            check_parser_msg.append("Number of landmarks must be zero or >= 3.  Please " + \
-                "provide a valid number of landmarks and try again.")
-
-    # fifth parameter is number of PCA components
-    if parms[4] < 2:
-        check_parser_msg.append("Number of PCA components must be >= 2.  Please provide " + \
-            "a valid number of PCA components and try again.")
-
-    # sixth parameter is expected type
-    if parms[5] != "General" and \
-       parms[5] != "Overvoltage" and \
-       parms[5] != "Sprytron":
-        check_parser_msg.append ('Expected data type must be one of "General", ' + \
-            '"Overvoltage" or "Sprytron". Please use one of those options ' + \
-            'and try again.')
-
-    # seventh parameter is union or intersection (combination of time series)
-    if parms[6] != "Union" and \
-       parms[6] != "Intersection":
-        check_parser_msg.append ('Available methods for combining mismatched, ' + \
-            'time points are "Union" and "Intersection". Please use one of those options ' + \
-            'and try again.')
-
-    # seventh and eighth parameters are boolean, so either option is OK 
-
-    return "\n".join(check_parser_msg)
-
 # get file suffixes for .zip file
 def get_suffixes (zip_file):
 
     # save results as a set
     tdms_suffixes = set()
 
     # look through zip file for suffixes
@@ -184,72 +128,50 @@
     # wait until the model is ready
     connection.join_model(mid)
 
     return mid
 
 # check arguments and create model
 def create_model (arguments, log):
-
+    
     # can't have both overvoltage and sprytron
     if arguments.overvoltage and arguments.sprytron:
         raise TDMSUploadError("Can't use both overvoltage and sprytron options " +
               "together. Please select one or the other and try again.")
 
     # check file name extensions
     file_list = arguments.files
     file_type = check_file_extensions (file_list)
     if file_type == "not-tdms":
         log("One or more files had the wrong extension (note that if using .zip " +
               "only one file can be uploaded). Please revise the file list " +
               "and try again.")
-        exit()
+        raise TDMSUploadError("One or more files had the wrong extension " + 
+              "(note that if using .zip only one file can be uploaded). Please " + 
+              "revise the file list and try again.")
 
     # check that files exist
     if not check_files_exist (file_list):
         raise TDMSUploadError("One or more input files did not exist. Please make " +
               "sure the file names are correct and try again.")
 
     # check that zip file is valid
     if file_type == 'zip':
         if not zipfile.is_zipfile(file_list[0]):
             raise TDMSUploadError("Zip file is invalid or corrupt. Please fix the " + 
                   "file and try again.")
 
-    # set shot type
-    shot_type = 'General'
-    if arguments.overvoltage:
-        shot_type = 'Overvoltage'
-    if arguments.sprytron:
-        shot_type = 'Sprytron'
-
-    # set union type
-    union_type = "Union"
-    if arguments.intersection:
-        union_type = "Intersection"
-
-    # populate parameters
-    parser_parms = [arguments.min_time_points, arguments.min_channels, 
-                    arguments.min_num_shots, arguments.num_landmarks,
-                    arguments.num_PCA_comps,
-                    shot_type, union_type, 
-                    not arguments.do_not_infer_channel_units,
-                    not arguments.do_not_infer_time_units]
+    # parser tdms options
+    parser_parms = dac_tdms_util.get_parms (arguments)
 
     # check common parameters
-    check_parser_error = check_parser_parms (parser_parms)
+    parser_parms, check_parser_error = dac_tdms_util.check_parms (arguments, parser_parms)
     if check_parser_error != "":
         raise TDMSUploadError(check_parser_error)
 
-    # landmarks over-rides PCA comps
-    if arguments.num_landmarks is not None:
-        parser_parms[4] = False
-    else:
-        parser_parms[4] = True
-        parser_parms[3] = arguments.num_PCA_comps
-
     # compile suffixes to include if .zip file
     dac_parser = "dac-tdms-file-parser"
     if file_type == "zip":
 
         # get all possible suffixes
         include_suffixes = get_suffixes (file_list[0])
 
@@ -351,44 +273,16 @@
 
     # exclude .tdms files from .zip upload
     parser.add_argument("--exclude", nargs="+",
         help='TDMS file suffixes to exclude within .zip files. ' + 
              'If you want suffixes that include spaces, use quotes, ' +
              'e.g. "suffix with space".')
 
-    # parsing parameters
-    parser.add_argument("--min-time-points", default=10, type=int, 
-        help="Minimum number of time points per channel, integer >= 2. " +
-             "Default: %(default)s.")
-    parser.add_argument("--min-channels", default=2, type=int,
-        help="Minimum number of channels per text, integer >= 1. " +
-             "Default: %(default)s.")
-    parser.add_argument("--min-num-shots", default=1, type=int,
-        help="Channels must occur in at least this many shots, integer >= 0. " +
-             "Use zero to indicate that channel must occur in every shot. " +
-             "Default: %(default)s.")
-    parser.add_argument("--num-landmarks", default=None, type=int,
-        help="Number of landmarks to use, integer >= 3.  Can also use zero " +
-             "to indicate use of full dataset (no landmarks).  Default: %(default)s.")
-    parser.add_argument("--num-PCA-comps", default=10, type=int,
-        help="Number of PCA components to use, integer >= 2.  Note --num-landmarks " + 
-             "over-rides --num-PCA-comps.  Default: %(default)s.")
-    parser.add_argument("--overvoltage", action="store_true",
-        help="Expecting overvoltage data.")
-    parser.add_argument("--sprytron", action="store_true",
-        help="Expecting sprytron data.")
-    parser.add_argument("--intersection", action="store_true", 
-        help="Combine mismatched time steps using intersection. " +
-             "Default is to combine using union.")
-    parser.add_argument("--do-not-infer-channel-units", action="store_true",
-        help="Do not infer channel units. Default is to infer channel units " +
-             "from channel name.")
-    parser.add_argument("--do-not-infer-time-units", action="store_true",
-        help="Do not infer time units. Default is to assume unspecified units " +
-             "are seconds.")
+    # add tmds options
+    parser = dac_tdms_util.add_options (parser)
 
     return parser
 
 # tdms entry point
 def main():
 
     # set up argument parser
```

### Comparing `slycat-web-client-3.4.0/slycat/web/client/dac_tdms_batch.py` & `slycat-web-client-4.0.0/slycat/web/client/dac_tdms_batch_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,16 @@
 
         # log to screen only
         def logger(msg):
             print(msg)
 
     return logger
 
-# tdms batch entry point
-def main():
+# parser
+def parser():
 
     # provide additional command line arguments 
     batch_parser = argparse.ArgumentParser(description=
         "Creates a batch of Dial-A-Cluster models from links to TDMS data " +
         "provided in a file.")
 
     # actual files to upload
@@ -69,16 +69,18 @@
     # optional flag to log results to file
     batch_parser.add_argument('--log_file', default=None,
         help="Optional file to log results of TDMS uploads.  Note that if a model " +
              "fails to upload, the script will not terminate, but will carry on " + 
              "trying to upload the remaaining data.  Log file will be overwritten " +
              "if it already exists.")
 
-    # get command line arguments
-    batch_args = batch_parser.parse_args()
+    return batch_parser
+
+# tdms batch entry point
+def create_batch(batch_args):
 
     # set up logging, always to screen, to file if requested
     log = setup_logging(batch_args.log_file)
 
     # parse batch file
     auth_args = []
     proj_args = []
@@ -119,11 +121,23 @@
             tdms.create_model(arguments, log)
 
         # if there is a problem, skip this model and continue
         except:
             log('Could not upload model with arguments: ' + ' '.join(args))
             log(traceback.format_exc())
 
+# parser command line arguments
+def main():
+
+    # set up argument parser
+    batch_parser = parser()
+
+    # get user arguments
+    arguments = batch_parser.parse_args()
+
+    # check arguments and create model
+    create_batch(arguments)
+
 # command line entry point
 if __name__ == "__main__":
 
     main()
```

### Comparing `slycat-web-client-3.4.0/slycat/web/client/get_model.py` & `slycat-web-client-4.0.0/slycat/web/client/get_model.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/get_project.py` & `slycat-web-client-4.0.0/slycat/web/client/get_project.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/list_markings.py` & `slycat-web-client-4.0.0/slycat/web/client/list_markings.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/list_projects.py` & `slycat-web-client-4.0.0/slycat/web/client/list_projects.py`

 * *Files identical despite different names*

### Comparing `slycat-web-client-3.4.0/slycat/web/client/ps_csv.py` & `slycat-web-client-4.0.0/slycat/web/client/ps_csv.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 
 # This script read and processes a .csv file before pushing it to the Slycat server
 # as a parameter space model.
 
 import os
 import re
 
-import pandas as pd
 import numpy as np
 
 import slycat.web.client
 import urllib.parse as urlparse
 
+# slycat csv parser
+import slycat.pandas_util
+
 # parse command line arguments
 def parser():
 
   parser = slycat.web.client.ArgumentParser(description=
     "Create Slycat Parameter Space model from .csv table.")
 
   # input file
@@ -54,15 +56,19 @@
 # logging is just printing to the screen
 def log (msg):
     print(msg)
 
 # create PS model, show progress by default, arguments 
 # include the command line connection parameters
 # and project/model information
-def upload_model (arguments, parser, df, progress=True):
+def upload_model (arguments, attributes, dimensions, data, progress=True):
+
+  # get column names/types
+  column_names = [attribute["name"] for attribute in attributes]
+  column_types = [attribute["type"] for attribute in attributes]
 
   # setup a connection to the Slycat Web Server.
   connection = slycat.web.client.connect(arguments)
 
   # create a new project to contain our model.
   pid = connection.find_or_create_project(arguments.project_name, arguments.project_description)
 
@@ -70,147 +76,153 @@
   mid = connection.post_project_models(pid, "parameter-image", 
     arguments.model_name, arguments.marking, arguments.model_description)
 
   # Upload our observations as "data-table".
   connection.put_model_arrayset(mid, "data-table")
 
   # Start our single "data-table" array.
-  dimensions = [dict(name="row", end=len(df.index))]
-  attributes = [dict(name=header, type="float64" 
-    if df[header].dtype != "object" else "string") 
-    for header in df.columns]
   connection.put_model_arrayset_array(mid, "data-table", 0, dimensions, attributes)
 
   # Upload each column into the array.
-  for index, header in enumerate(df.columns):
-
-    # make sure type is either float or string
-    if df[header].dtype == "object":
-      values = [df[header].values.astype(str)]
-    else:
-      values = [df[header].values.astype(float)]
+  for index in range(len(column_names)):
+    values = [np.asarray(data[index])]
 
     # push to server
     connection.put_model_arrayset_data(mid, "data-table", "0/%s/..." % index, values)
 
   # Store the remaining parameters.
-  input_col_inds = [index for index, header in enumerate(df.columns) 
-    if header in arguments.input_columns and df[header].dtype != "object"]
+  input_col_inds = [index for index, header in enumerate(column_names) 
+    if header in arguments.input_columns and column_types[index] != "string"]
   connection.put_model_parameter(mid, "input-columns", input_col_inds)
-  output_col_inds = [index for index, header in enumerate(df.columns) 
-    if header in arguments.output_columns and df[header].dtype != "object"]
+  output_col_inds = [index for index, header in enumerate(column_names) 
+    if header in arguments.output_columns and column_types[index] != "string"]
   connection.put_model_parameter(mid, "output-columns", output_col_inds)
-  media_col_inds = [index for index, header in enumerate(df.columns) 
-    if header in arguments.media_columns and df[header].dtype == "object"]
+  media_col_inds = [index for index, header in enumerate(column_names) 
+    if header in arguments.media_columns and column_types[index] == "string"]
   connection.put_model_parameter(mid, "image-columns", media_col_inds)
 
   # Signal that we're done uploading data to the model.  This lets Slycat Web
   # Server know that it can start computation.
   connection.post_model_finish(mid)
 
   # Wait until the model is ready.
   connection.join_model(mid)
 
   return mid
 
-# check arguments and create model
+# check arguments and create model, returns URL to model
 def create_model (arguments, log):
 
   # check that input file exists
   if not os.path.isfile(arguments.file):
     log("Input file " + arguments.file + " does not exist.")
     raise ValueError("Input file " + arguments.file + " does not exist.")
 
   # check that input/output columns are non-intersecting
   if set(arguments.input_columns).intersection(set(arguments.output_columns)):
     log("Input columns and output columns are intersecting.")
     raise ValueError("Input columns and output columns are intersecting.")
 
-  # load input file as pandas dataframe
-  df = pd.read_csv(arguments.file)
+  # parse file using standard slycat csv parser
+  attributes, dimensions, data, csv_read_error = \
+    slycat.pandas_util.parse_file(arguments.file, file_name=True)
+
+  # check for warnings/errors
+  for i in range(len(csv_read_error)):
+    if csv_read_error[i]["type"] == "warning":
+      log("Warning: " + csv_read_error[i]["message"])
+    else:
+      log("Error: " + csv_read_error[i]["message"])
+      raise ValueError(csv_read_error[i]["message"])
+
+  # get column names/types
+  column_names = [attribute["name"] for attribute in attributes]
+  column_types = [attribute["type"] for attribute in attributes]
 
   # check that inputs are in headers
   if arguments.input_columns is not None:
     for input_col in arguments.input_columns:
-      if input_col not in df.columns:
+      if input_col not in column_names:
         log('Input column "' + input_col + '" not found in input file.')
         raise ValueError('Input column "' + input_col + '" not found in input file.')
 
   # check that outputs are in headers
   if arguments.output_columns is not None:
     for output_col in arguments.output_columns:
-      if output_col not in df.columns:
+      if output_col not in column_names:
         log('Output column "' + output_col + '" not found in input file.')
         raise ValueError('Output column "' + output_col + '" not found in input file.')
       
   # check that meda-columns are in headers
   if arguments.media_columns is not None:
     for media_col in arguments.media_columns:
-      if media_col not in df.columns:
+      if media_col not in column_names:
         log('Media column "' + media_col + '" not found in input file.')
         raise ValueError('Media column "' + media_col + '" not found in input file.')
 
   # check that there is at least one numeric columns (to display scatter plot)
-  if not df.select_dtypes(include='float64').columns.to_list():
+  if not 'float64' in column_types:
     log("You must supply at least one numeric column in the input data.")
     raise ValueError("You must supply at least one numeric column in the input data.")
 
   # identify media columns automatically if not provided
   if arguments.media_columns is None:
     arguments.media_columns = []
 
     # search for "file://"
     expression = re.compile("file://")
     search = np.vectorize(lambda x:bool(expression.search(x)))
 
     # go through each column
-    for header in df.columns:
+    for header in range(len(column_names)):
 
       # strings are stored in pandas object type
-      if df[header].dtype == "object":
-        if np.any(search(df[header].values)):
-          arguments.media_columns.append(header)
+      if column_types[header] == "string":
+        if np.any(search(data[header])):
+          arguments.media_columns.append(column_names[header])
 
   # replace media URL hostnames, if requested
   if arguments.media_hostname is not None:
     
     # go through each column
-    for header in df.columns:
+    for header in range(len(column_names)):
 
       # if media column is given and a string
-      if header in arguments.media_columns and df[header].dtype == "object":
+      if column_names[header] in arguments.media_columns and \
+         column_types[header] == "string":
         modified = []
 
         # replace file://cluster with file://hostname
-        for uri in df[header].values:
+        for uri in data[header]:
           uri = urlparse.urlparse(uri)
           path = uri.path
           uri = "file://%s%s" % (arguments.media_hostname, path)
           modified.append(uri)
-        df[header] = modified
+        data[header] = modified
 
   # strip prefix directories, if requested
   if arguments.strip is not None:
 
     # go through each column:
-    for header in df.columns:
+    for header in range(len(column_names)):
 
       # for media columns, strip prefix directories
-      if header in arguments.media_columns and df[header].dtype == "object":
+      if column_names[header] in arguments.media_columns and \
+         column_types[header] == "string":
         modified = []
 
         # strip prefixes
         for uri in df[header].values:
           uri = urlparse.urlparse(uri)
           hostname = uri.netloc
           path = os.path.join(*([os.path.abspath(os.path.dirname(arguments.file))] + 
             uri.path.split(os.sep)[arguments.strip + 1:]))
           uri = "file://%s%s" % (hostname, path)
           modified.append(uri)
-        df[header] = modified
+        data[header] = modified
 
   # echo inputs to user
   log('Input file: ' + arguments.file)
   if arguments.input_columns is not None:
     log('Input columns: ' + str(arguments.input_columns))
   if arguments.output_columns is not None:
     log('Output columns: ' + str(arguments.output_columns))
@@ -218,32 +230,36 @@
     log('Media columns: ' + str(arguments.media_columns))
   if arguments.media_hostname is not None:
     log('Media hostname: ' + str(arguments.media_hostname))
   if arguments.strip is not None:
     log('Stripped ' + str(arguments.strip) + ' prefixes from media columns.')
 
   # upload model
-  mid = upload_model (arguments, parser, df, progress=True)
+  mid = upload_model (arguments, attributes, dimensions, data, progress=True)
 
   # supply direct link to model
   host = arguments.host
   if arguments.port:
       host = host + ":" + arguments.port
-  log("Your new model is located at %s/models/%s" % (host, mid))
+  url = host + "/models/" + mid
+  log("Your new model is located at %s" % url)
   log('***** PS Model Successfully Created *****')
 
+  # return url
+  return url
+
 # main entry point
 def main():
 
     # set up argument parser
     ps_parser = parser()  
 
     # get user arguments
     arguments = ps_parser.parse_args()
 
     # check arguments and create model
-    create_model(arguments, log)
+    url = create_model(arguments, log)
 
 # command line version
 if __name__ == "__main__":
 
     main()
```

### Comparing `slycat-web-client-3.4.0/slycat_web_client.egg-info/PKG-INFO` & `slycat-web-client-4.0.0/slycat_web_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slycat-web-client
-Version: 3.4.0
+Version: 4.0.0
 Summary: Slycat web client utilties for interacting with the Slycat data analysis and visualization server.
 Home-page: https://github.com/sandialabs/slycat
 Author: Shawn Martin
 Author-email: smartin@sandia.gov
 License: Sandia
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -67,24 +67,23 @@
 
 or
 
 ```sh
 $ python -m slycat.web.client.list_markings
 ```
 
-In addition, there are two entry points defined for the Slycat Dial-A-Cluster plugin
+In addition, there are two main entry points defined for the Slycat Dial-A-Cluster plugin
 
 ```sh
 $ dac_tdms
 ```
-
 and
 
 ```sh
-$ dac_tdms_batch
+$ dac_gen
 ```
 
 These are described in greater detail below.
 
 ## User Authentication
 
 The Slycat server requires user authentication.  The slycat.web.client
@@ -208,36 +207,45 @@
 
 This will create a model from a single .TDM file.  You can also use .TDMS
 files and .zip archives containing .tdms files.  The options available
 for the creation of the models are the same as the options available using
 the DAC model creation wizard in the browser.  To see the options use
 the "--help" flag when calling the script.
 
-In addition, a batch script is available for uploading multiple DAC TDMS
-models.  To use this script, you must first create a file containing the
-options for each model.  The file has the following format.
+In addition, there are two methods for uploading batches of multiple DAC
+TDMS models.  The first method uses the dac_tdms_batch script.  This script
+takes as input a part-num match (see also dac_run_chart) and creates
+the corresponding batches.  For example,
+
+```sh
+$ dac_tdms_batch root-data-directory part-num
+```
+
+The second method uses the dac_tdms_batch_file script.  To use this script, 
+you must first create a file containing the options for each model.  The file 
+has the following format.
 
 Line 1 contains the authentication information for the Slycat server that
 you would pass to the dac_tdms script, but separated by commas.
 For example,
 
-    --user,smartin,--kerberos
+    --user,user-name,--kerberos
 
 If authentication information is unnecessary, just leave the line blank.
 
 Line 2 contains the project information for the project that will contain
 the DAC models to be created, e.g.
 
     --project-name,Batch TDMS Models
 
 Line 2 can also be left blank.  It will default to "Batch TDMS Models".
 Lines 3 and beyond contain the model information for each model, such as
 
-    model-data-file-1.tdms,--model-name,Model 1
-    model-data-file-2.tdms,--model-name,Model 2
+    model-data-file-1.tdms,--model-name,Model 1,--project-name,Batch TDMS Models
+    model-data-file-2.tdms,--model-name,Model 2,--project-name,Batch TDMS Models
 
 Note that you must supply a model file (or multiple files) in accordance
 with the dac_tdms script for each model.  Also note that if 
 you want to put models into different projects, you can override the 
 original project given in line 2, by using the "--project-name" flag 
 again, e.g.
```

### Comparing `slycat-web-client-3.4.0/slycat_web_client.egg-info/SOURCES.txt` & `slycat-web-client-4.0.0/slycat_web_client.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 slycat/__init__.py
 slycat/darray.py
+slycat/pandas_util.py
 slycat/web/__init__.py
 slycat/web/client/__init__.py
 slycat/web/client/cca_csv.py
 slycat/web/client/cca_random.py
 slycat/web/client/dac_defaults.py
 slycat/web/client/dac_gen.py
 slycat/web/client/dac_run_chart.py
 slycat/web/client/dac_tdms.py
 slycat/web/client/dac_tdms_batch.py
+slycat/web/client/dac_tdms_batch_file.py
+slycat/web/client/dac_tdms_util.py
 slycat/web/client/get_model.py
 slycat/web/client/get_project.py
 slycat/web/client/list_markings.py
 slycat/web/client/list_projects.py
 slycat/web/client/ps_csv.py
 slycat_web_client.egg-info/PKG-INFO
 slycat_web_client.egg-info/SOURCES.txt
```

