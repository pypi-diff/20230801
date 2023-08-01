# Comparing `tmp/discuit-0.2.1.tar.gz` & `tmp/discuit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discuit-0.2.1.tar", last modified: Tue Apr 18 07:59:13 2023, max compression
+gzip compressed data, was "discuit-0.3.0.tar", last modified: Tue Aug  1 11:21:38 2023, max compression
```

## Comparing `discuit-0.2.1.tar` & `discuit-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.367019 discuit-0.2.1/
--rw-r--r--   0 doerte     (501) staff       (20)      454 2023-04-18 07:52:44.000000 discuit-0.2.1/CITATION.cff
--rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.2.1/LICENSE
--rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.2.1/MANIFEST.in
--rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.2.1/NOTICE
--rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:59:13.367077 discuit-0.2.1/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)     6801 2023-04-18 07:21:17.000000 discuit-0.2.1/README.md
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.365679 discuit-0.2.1/discuit/
--rw-r--r--   0 doerte     (501) staff       (20)      192 2023-02-24 12:59:01.000000 discuit-0.2.1/discuit/__init__.py
--rw-r--r--   0 doerte     (501) staff       (20)    16136 2023-04-18 07:50:10.000000 discuit-0.2.1/discuit/run_discuit.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.366666 discuit-0.2.1/discuit.egg-info/
--rw-r--r--   0 doerte     (501) staff       (20)     7883 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/PKG-INFO
--rw-r--r--   0 doerte     (501) staff       (20)      334 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/SOURCES.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/dependency_links.txt
--rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.2.1/discuit.egg-info/not-zip-safe
--rw-r--r--   0 doerte     (501) staff       (20)      276 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/requires.txt
--rw-r--r--   0 doerte     (501) staff       (20)        8 2023-04-18 07:59:13.000000 discuit-0.2.1/discuit.egg-info/top_level.txt
--rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.2.1/pyproject.toml
--rw-r--r--   0 doerte     (501) staff       (20)     1897 2023-04-18 07:59:13.367458 discuit-0.2.1/setup.cfg
--rw-r--r--   0 doerte     (501) staff       (20)       87 2023-02-15 15:09:44.000000 discuit-0.2.1/setup.py
-drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-04-18 07:59:13.366782 discuit-0.2.1/tests/
--rw-r--r--   0 doerte     (501) staff       (20)      343 2023-02-24 12:59:25.000000 discuit-0.2.1/tests/test_my_module.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742740 discuit-0.3.0/
+-rw-r--r--   0 doerte     (501) staff       (20)      454 2023-08-01 07:36:22.000000 discuit-0.3.0/CITATION.cff
+-rw-r--r--   0 doerte     (501) staff       (20)    11359 2023-02-15 15:09:44.000000 discuit-0.3.0/LICENSE
+-rw-r--r--   0 doerte     (501) staff       (20)       70 2023-02-15 15:09:44.000000 discuit-0.3.0/MANIFEST.in
+-rw-r--r--   0 doerte     (501) staff       (20)       68 2023-02-25 18:49:41.000000 discuit-0.3.0/NOTICE
+-rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-01 11:21:38.742824 discuit-0.3.0/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)     6624 2023-07-31 18:59:36.000000 discuit-0.3.0/README.md
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.741088 discuit-0.3.0/discuit/
+-rw-r--r--   0 doerte     (501) staff       (20)      206 2023-07-31 18:15:19.000000 discuit-0.3.0/discuit/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)     1909 2023-08-01 07:39:44.000000 discuit-0.3.0/discuit/calculations.py
+-rw-r--r--   0 doerte     (501) staff       (20)     4681 2023-08-01 07:28:02.000000 discuit-0.3.0/discuit/clustering.py
+-rw-r--r--   0 doerte     (501) staff       (20)     6125 2023-08-01 07:39:44.000000 discuit-0.3.0/discuit/command_line.py
+-rw-r--r--   0 doerte     (501) staff       (20)     2494 2023-08-01 07:45:08.000000 discuit-0.3.0/discuit/run.py
+-rw-r--r--   0 doerte     (501) staff       (20)     2991 2023-08-01 07:34:05.000000 discuit-0.3.0/discuit/write.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742213 discuit-0.3.0/discuit.egg-info/
+-rw-r--r--   0 doerte     (501) staff       (20)     7706 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/PKG-INFO
+-rw-r--r--   0 doerte     (501) staff       (20)      465 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/SOURCES.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/dependency_links.txt
+-rw-r--r--   0 doerte     (501) staff       (20)       54 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/entry_points.txt
+-rw-r--r--   0 doerte     (501) staff       (20)        1 2023-02-25 18:42:43.000000 discuit-0.3.0/discuit.egg-info/not-zip-safe
+-rw-r--r--   0 doerte     (501) staff       (20)      276 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/requires.txt
+-rw-r--r--   0 doerte     (501) staff       (20)       14 2023-08-01 11:21:38.000000 discuit-0.3.0/discuit.egg-info/top_level.txt
+-rw-r--r--   0 doerte     (501) staff       (20)      376 2023-02-25 18:49:41.000000 discuit-0.3.0/pyproject.toml
+-rw-r--r--   0 doerte     (501) staff       (20)     1977 2023-08-01 11:21:38.743246 discuit-0.3.0/setup.cfg
+-rw-r--r--   0 doerte     (501) staff       (20)      206 2023-08-01 11:21:30.000000 discuit-0.3.0/setup.py
+drwxr-xr-x   0 doerte     (501) staff       (20)        0 2023-08-01 11:21:38.742457 discuit-0.3.0/tests/
+-rw-r--r--   0 doerte     (501) staff       (20)        0 2023-02-15 15:09:44.000000 discuit-0.3.0/tests/__init__.py
+-rw-r--r--   0 doerte     (501) staff       (20)      343 2023-08-01 07:45:59.000000 discuit-0.3.0/tests/test_my_module.py
```

### Comparing `discuit-0.2.1/LICENSE` & `discuit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discuit-0.2.1/PKG-INFO` & `discuit-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.2.1
+Version: 0.3.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
@@ -22,16 +22,14 @@
 Provides-Extra: dev
 Provides-Extra: publishing
 License-File: LICENSE
 License-File: NOTICE
 
 ## Badges
 
-(Customize these badges with your own links, and check https://shields.io/ or https://badgen.net/ to see which other badges are available.)
-
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/doerte/discuit-project) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/doerte/discuit-project)](https://github.com/doerte/discuit-project) |
 | (3/5) community registry           | <!-- [![RSD](https://img.shields.io/badge/rsd-discuit-00a3e3.svg)](https://www.research-software.nl/software/<replace-with-name>) [![workflow pypi badge](https://img.shields.io/pypi/v/<replace-with-name>.svg?colorB=blue)](https://pypi.python.org/project/<replace-with-name>/) -->|
 | (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7671856.svg)](https://doi.org/10.5281/zenodo.7671856) |
 | (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
@@ -78,19 +76,21 @@
 
 <!-- ## Documentation
 
 Include a link to your project's full documentation here. --> 
 
 ## Using Discuit
 In the terminal, run Discuit with the following command:
-python3 run_discuit.py "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
+discuit "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
 
-Example: python3 discuit/run_discuit.py example/input.csv 2 --columns l a n c n d --runs 3
+Example: discuit example/input.csv 2 --columns l a n c n d --runs 3
 
-This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" and "disregard" (in that order). The program will run 3 times (and create 3 output files).
+This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. 
+The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" 
+and "disregard" (in that order). The program will run 3 times (and create 3 output files).
 
 ### Required input
 The input file needs to be a .csv file with a first line containing headings followed by rows that represent the different items. Each column specifies one variable. 
 
 When launching the script, please specify per column what kind a data the script should expect: 
 - (l)abel: just a label, will not be taken into consideration, could be the itemname or itemnumber. This can only be assigned once. 
 - (n)umerical: a numerical variable, such as frequency or AoA,
```

### Comparing `discuit-0.2.1/README.md` & `discuit-0.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 ## Badges
 
-(Customize these badges with your own links, and check https://shields.io/ or https://badgen.net/ to see which other badges are available.)
-
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/doerte/discuit-project) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/doerte/discuit-project)](https://github.com/doerte/discuit-project) |
 | (3/5) community registry           | <!-- [![RSD](https://img.shields.io/badge/rsd-discuit-00a3e3.svg)](https://www.research-software.nl/software/<replace-with-name>) [![workflow pypi badge](https://img.shields.io/pypi/v/<replace-with-name>.svg?colorB=blue)](https://pypi.python.org/project/<replace-with-name>/) -->|
 | (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7671856.svg)](https://doi.org/10.5281/zenodo.7671856) |
 | (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
@@ -52,19 +50,21 @@
 
 <!-- ## Documentation
 
 Include a link to your project's full documentation here. --> 
 
 ## Using Discuit
 In the terminal, run Discuit with the following command:
-python3 run_discuit.py "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
+discuit "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
 
-Example: python3 discuit/run_discuit.py example/input.csv 2 --columns l a n c n d --runs 3
+Example: discuit example/input.csv 2 --columns l a n c n d --runs 3
 
-This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" and "disregard" (in that order). The program will run 3 times (and create 3 output files).
+This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. 
+The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" 
+and "disregard" (in that order). The program will run 3 times (and create 3 output files).
 
 ### Required input
 The input file needs to be a .csv file with a first line containing headings followed by rows that represent the different items. Each column specifies one variable. 
 
 When launching the script, please specify per column what kind a data the script should expect: 
 - (l)abel: just a label, will not be taken into consideration, could be the itemname or itemnumber. This can only be assigned once. 
 - (n)umerical: a numerical variable, such as frequency or AoA,
```

### Comparing `discuit-0.2.1/discuit.egg-info/PKG-INFO` & `discuit-0.3.0/discuit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discuit
-Version: 0.2.1
+Version: 0.3.0
 Summary: Dynamic item set clustering UI tool: The goal of this package is to split datasets (e.g. words defined by several variables) into subsets that are as comparable as possible.
 Home-page: https://github.com/doerte/discuit-project
 Author: Dörte de Kok
 Author-email: me@doerte.eu
 Project-URL: Bug Tracker, https://github.com/doerte/discuit-project/issues
 Keywords: clustering
 Classifier: Development Status :: 4 - Beta
@@ -22,16 +22,14 @@
 Provides-Extra: dev
 Provides-Extra: publishing
 License-File: LICENSE
 License-File: NOTICE
 
 ## Badges
 
-(Customize these badges with your own links, and check https://shields.io/ or https://badgen.net/ to see which other badges are available.)
-
 | fair-software.eu recommendations | |
 | :-- | :--  |
 | (1/5) code repository              | [![github repo badge](https://img.shields.io/badge/github-repo-000.svg?logo=github&labelColor=gray&color=blue)](https://github.com/doerte/discuit-project) |
 | (2/5) license                      | [![github license badge](https://img.shields.io/github/license/doerte/discuit-project)](https://github.com/doerte/discuit-project) |
 | (3/5) community registry           | <!-- [![RSD](https://img.shields.io/badge/rsd-discuit-00a3e3.svg)](https://www.research-software.nl/software/<replace-with-name>) [![workflow pypi badge](https://img.shields.io/pypi/v/<replace-with-name>.svg?colorB=blue)](https://pypi.python.org/project/<replace-with-name>/) -->|
 | (4/5) citation                     | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7671856.svg)](https://doi.org/10.5281/zenodo.7671856) |
 | (5/5) checklist                    | [![workflow cii badge](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>/badge)](https://bestpractices.coreinfrastructure.org/projects/<replace-with-created-project-identifier>) |
@@ -78,19 +76,21 @@
 
 <!-- ## Documentation
 
 Include a link to your project's full documentation here. --> 
 
 ## Using Discuit
 In the terminal, run Discuit with the following command:
-python3 run_discuit.py "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
+discuit "name of input file" [number of desired sets] --columns l/c/n/a/d --runs [desired number of runs]
 
-Example: python3 discuit/run_discuit.py example/input.csv 2 --columns l a n c n d --runs 3
+Example: discuit example/input.csv 2 --columns l a n c n d --runs 3
 
-This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" and "disregard" (in that order). The program will run 3 times (and create 3 output files).
+This will run Discuit with the [provided testfile](example/input.csv) and create 2 subsets. 
+The columns in the file are identified as "label", "categorical", "numerical", "absolute", "numerical" 
+and "disregard" (in that order). The program will run 3 times (and create 3 output files).
 
 ### Required input
 The input file needs to be a .csv file with a first line containing headings followed by rows that represent the different items. Each column specifies one variable. 
 
 When launching the script, please specify per column what kind a data the script should expect: 
 - (l)abel: just a label, will not be taken into consideration, could be the itemname or itemnumber. This can only be assigned once. 
 - (n)umerical: a numerical variable, such as frequency or AoA,
```

### Comparing `discuit-0.2.1/setup.cfg` & `discuit-0.3.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 keywords = clustering
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = discuit
 project_urls = 
 	Bug Tracker = https://github.com/doerte/discuit-project/issues
 url = https://github.com/doerte/discuit-project
-version = 0.2.1
+version = 0.3.0
 
 [options]
 zip_safe = False
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
@@ -55,14 +55,18 @@
 publishing = 
 	twine
 	wheel
 
 [options.packages.find]
 include = discuit, discuit.*
 
+[options.entry_points]
+console_scripts = 
+	discuit = discuit.command_line:main
+
 [isort]
 lines_after_imports = 2
 force_single_line = 1
 no_lines_before = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 known_first_party = discuit
 src_paths = discuit,tests
 line_length = 120
```

