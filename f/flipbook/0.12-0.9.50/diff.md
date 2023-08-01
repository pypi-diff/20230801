# Comparing `tmp/flipbook-0.12.tar.gz` & `tmp/flipbook-0.9.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipbook-0.12.tar", last modified: Tue Aug  1 15:20:34 2023, max compression
+gzip compressed data, was "dist/flipbook-0.9.50.tar", last modified: Tue Aug 24 02:58:29 2021, max compression
```

## Comparing `flipbook-0.12.tar` & `flipbook-0.9.50.tar`

### file list

```diff
@@ -1,45 +1,19 @@
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:34.023836 flipbook-0.12/
--rw-r--r--   0 weisburd   (502) staff       (20)     1060 2021-04-01 18:19:14.000000 flipbook-0.12/LICENSE
--rw-r--r--   0 weisburd   (502) staff       (20)     6580 2023-08-01 15:20:34.023519 flipbook-0.12/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)     5581 2023-01-15 18:39:47.000000 flipbook-0.12/README.md
--rw-r--r--   0 weisburd   (502) staff       (20)     7297 2021-07-02 22:32:26.000000 flipbook-0.12/compare_form_response_tables.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.989187 flipbook-0.12/flipbook/
--rw-r--r--   0 weisburd   (502) staff       (20)    18891 2023-08-01 15:16:53.000000 flipbook-0.12/flipbook/__init__.py
--rw-r--r--   0 weisburd   (502) staff       (20)       64 2021-09-15 14:02:24.000000 flipbook-0.12/flipbook/__main__.py
--rw-r--r--   0 weisburd   (502) staff       (20)     5309 2023-08-01 12:31:01.000000 flipbook-0.12/flipbook/data_page.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2437 2023-08-01 12:31:05.000000 flipbook-0.12/flipbook/main_list.py
--rw-r--r--   0 weisburd   (502) staff       (20)     2859 2021-08-24 02:49:47.000000 flipbook-0.12/flipbook/save.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.982335 flipbook-0.12/flipbook/static/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.994214 flipbook-0.12/flipbook/static/css/
--rw-r--r--   0 weisburd   (502) staff       (20)     6535 2023-01-15 18:16:35.000000 flipbook-0.12/flipbook/static/css/datatables.min.css
--rw-r--r--   0 weisburd   (502) staff       (20)   628536 2023-01-15 18:13:29.000000 flipbook-0.12/flipbook/static/css/semantic.min.css
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.981524 flipbook-0.12/flipbook/static/css/themes/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.981693 flipbook-0.12/flipbook/static/css/themes/default/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.981860 flipbook-0.12/flipbook/static/css/themes/default/assets/
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:34.002221 flipbook-0.12/flipbook/static/css/themes/default/assets/fonts/
--rw-r--r--   0 weisburd   (502) staff       (20)   105784 2023-01-15 18:31:14.000000 flipbook-0.12/flipbook/static/css/themes/default/assets/fonts/icons.ttf
--rw-r--r--   0 weisburd   (502) staff       (20)    50524 2023-01-15 18:31:07.000000 flipbook-0.12/flipbook/static/css/themes/default/assets/fonts/icons.woff
--rw-r--r--   0 weisburd   (502) staff       (20)    40148 2023-01-15 18:30:56.000000 flipbook-0.12/flipbook/static/css/themes/default/assets/fonts/icons.woff2
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:34.003420 flipbook-0.12/flipbook/static/images/
--rw-r--r--   0 weisburd   (502) staff       (20)     5591 2021-09-28 17:09:18.000000 flipbook-0.12/flipbook/static/images/favicon.png
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:34.017414 flipbook-0.12/flipbook/static/js/
--rw-r--r--   0 weisburd   (502) staff       (20)   328879 2023-01-15 18:17:35.000000 flipbook-0.12/flipbook/static/js/datatables.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)    89476 2020-05-08 07:05:03.000000 flipbook-0.12/flipbook/static/js/jquery.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)     1741 2020-05-04 16:11:46.000000 flipbook-0.12/flipbook/static/js/jquery.serialize-object.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   970387 2020-05-04 16:15:03.000000 flipbook-0.12/flipbook/static/js/pdfmake.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)     4754 2020-05-04 16:15:40.000000 flipbook-0.12/flipbook/static/js/purl.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   275730 2023-01-15 18:13:38.000000 flipbook-0.12/flipbook/static/js/semantic.min.js
--rw-r--r--   0 weisburd   (502) staff       (20)   870284 2020-05-04 16:15:03.000000 flipbook-0.12/flipbook/static/js/vfs_fonts.js
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:34.022740 flipbook-0.12/flipbook/templates/
--rw-r--r--   0 weisburd   (502) staff       (20)    15951 2023-01-15 18:18:44.000000 flipbook-0.12/flipbook/templates/data_page.html
--rw-r--r--   0 weisburd   (502) staff       (20)     5556 2023-01-15 18:18:44.000000 flipbook-0.12/flipbook/templates/main_list.html
--rw-r--r--   0 weisburd   (502) staff       (20)     6583 2021-11-01 11:55:01.000000 flipbook-0.12/flipbook/utils.py
-drwxr-xr-x   0 weisburd   (502) staff       (20)        0 2023-08-01 15:20:33.993072 flipbook-0.12/flipbook.egg-info/
--rw-r--r--   0 weisburd   (502) staff       (20)     6580 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/PKG-INFO
--rw-r--r--   0 weisburd   (502) staff       (20)      981 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/SOURCES.txt
--rw-r--r--   0 weisburd   (502) staff       (20)        1 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/dependency_links.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       43 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/entry_points.txt
--rw-r--r--   0 weisburd   (502) staff       (20)      184 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/requires.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-08-01 15:20:33.000000 flipbook-0.12/flipbook.egg-info/top_level.txt
--rw-r--r--   0 weisburd   (502) staff       (20)       38 2023-08-01 15:20:34.023928 flipbook-0.12/setup.cfg
--rw-r--r--   0 weisburd   (502) staff       (20)     2495 2023-08-01 14:51:40.000000 flipbook-0.12/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-08-24 02:58:29.000000 flipbook-0.9.50/
+-rw-r--r--   0 root         (0) staff       (20)     6965 2021-08-24 02:58:29.000000 flipbook-0.9.50/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     5051 2021-08-24 02:43:34.000000 flipbook-0.9.50/README.md
+-rw-r--r--   0 root         (0) staff       (20)     7297 2021-07-02 22:32:26.000000 flipbook-0.9.50/compare_form_response_tables.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook/
+-rw-r--r--   0 root         (0) staff       (20)    13545 2021-08-24 02:52:57.000000 flipbook-0.9.50/flipbook/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1544 2021-08-24 02:49:47.000000 flipbook-0.9.50/flipbook/__main__.py
+-rw-r--r--   0 root         (0) staff       (20)     4404 2021-08-24 02:49:47.000000 flipbook-0.9.50/flipbook/data_page.py
+-rw-r--r--   0 root         (0) staff       (20)     1901 2021-08-24 02:49:47.000000 flipbook-0.9.50/flipbook/main_list.py
+-rw-r--r--   0 root         (0) staff       (20)     2859 2021-08-24 02:49:47.000000 flipbook-0.9.50/flipbook/save.py
+-rw-r--r--   0 root         (0) staff       (20)     6528 2021-08-24 02:52:57.000000 flipbook-0.9.50/flipbook/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     6965 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      330 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       91 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2021-08-24 02:58:29.000000 flipbook-0.9.50/flipbook.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2021-08-24 02:58:29.000000 flipbook-0.9.50/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1830 2021-08-24 02:52:57.000000 flipbook-0.9.50/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `flipbook-0.12/PKG-INFO` & `flipbook-0.9.50/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,134 @@
 Metadata-Version: 2.1
 Name: flipbook
-Version: 0.12
+Version: 0.9.50
 Summary: Starts a simple image server that lets you quickly flip through image files from a local directory using your web browser and optionally answering customizable questions about each one
 Home-page: https://github.com/broadinstitute/flipbook
 License: MIT
+Description: ## FlipBook
+        
+        This tool starts a simple image server that lets you quickly flip through image files from a local directory using your web browser.
+        Also, it optionally shows a customizable form where you can take notes or answer questions about each image or set of images.
+        
+        ### Example uses:
+        - manual curation / review of sequencing data visualization images such as those generated by [REViewer](https://www.illumina.com/science/genomics-research/reviewer-visualizing-alignments-short-reads-long-repeat.html) for short tandem repeat loci
+        - machine learning training set creation
+        - reviewing a pile of photos
+        
+        ### Features:
+        
+        - simple way to flip through many local image files using your web browser
+        - crawls a top-level directory to find .png, .jpeg, or .svg image files
+        - web interface: home page lists all images
+        - web interface: image pages show the image, an optional customizable form where you can take notes or answer questions about the image, next/previous page links, and optional other customizable info for context
+        - use subdirectories to group images. Any images found in the same subdirectory will be shown on the same page  
+        
+        -------
+        
+        [![PyPI version](https://img.shields.io/pypi/v/flipbook.svg?style=flat)](https://pypi.org/project/flipbook/)  [![Supported Python versions](https://img.shields.io/pypi/pyversions/flipbook.svg)](https://shields.io/)
+        
+        
+        ### Install:
+        
+        ```
+        python3 -m pip install flipbook  
+        ```
+        
+        ### Run:
+        
+        ```
+        python3 -m flipbook    # start server for all images in the current directory and subdirectories
+        ```
+        
+        Below are more examples. Run with `--help` to see all available options and their descriptions.
+        
+        ```
+        python3 -m flipbook -x temp -x keyword2  /path/dir-with-images    #  -x are keyword(s) of paths to skip and /path/dir-with-images is the top level dir to search instead of the current dir
+        
+        python3 -m flipbook -t /path/user_responses.xls    #  change where user responses get saved (default: flipbook_form_responses.tsv)
+        
+        python3 -m flipbook -m /path/metadata.tsv          #  provide a metadata table 
+        ```
+        
+        After the server is running, open your web browser to [http://localhost:8080](http://localhost:8080) to start reviewing images.
+        
+        ### Options:
+        
+        - metadata table (`-m`)
+          
+          It's often useful to add extra info to the image pages to help with review - such as image descriptions, quality scores, etc.
+          To enable this, there are several ways to specify arbitrary key-value pairs to add to specific image pages.
+          The 1st way is to put a file called `flipbook_metadata.json` next to the image(s). All keys and values from this file
+          will appear on that image page. The 2nd way is to use `-m` to pass in a metadata table 
+          (`.tsv` or `.xls`) with a `Path` column + arbitrary other columns. If the `Path` value matches the relative directory containing 
+          the image(s), entries from that row will be added to this image page.  
+          
+          Since the keys and values are treated as html, they can be used to add more complex info - such as
+          colors, text formatting, <img ..> tags with images from other web pages, iframes containing entire sections of external pages, etc. 
+        
+        - responses table (`-t`)
+        
+          As you fill in the forms at the top of the image pages, the responses are written to this table. If you later restart flipbook with the same `-t`, it will reload previous responses. You can also optionally use this table to provide additional columns to display - sometimes this can be more convenient than using `-m`. 
+          
+          *Default*: `flipbook_form_responses.tsv`
+        
+        - custom form schema (`--form-schema-json`)  
+           
+          If you'd like to use non-default questions in the image page forms, you can specify the path or url of a .json file containing a custom form schema. For examples of the expected format see [main/form_schema_examples](https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples)
+          
+        - config file (`~/.flipbook_config`)
+        
+          Most settings that can be provided on the command line can also be set via this YAML config file instead. For example:
+        
+          *~/.flipbook_config*
+          ```
+          form-schema-json: /path/to/my-schema.json
+          hide-metadata-on-home-page: true
+          host: 127.0.0.1
+          port: 8080
+          ```
+        
+          
+        For more details, run:   
+        ```
+        python3 -m flipbook --help
+        ```
+        
+        ### Comparing reviews:
+        
+        If 2 or more people review the same images, the reviews can be compared using the `compare_form_response_tables` script.  
+        
+        For example:
+        ```
+        python3 -m compare_form_response_tables egor_flipbook_form_responses.tsv  ben_flipbook_form_responses.tsv -o combined_responses.tsv -s1 egor -s2 ben
+        ```
+        
+        This script will print concordance stats, and output a `combined_responses.tsv` table that contains one image per row as well as each person's review of the image.  
+          
+        To see the full list of args and descriptions, run `python3 -m compare_form_response_tables --help`
+        
+        ### Development:
+        
+        To create a local dev instance, run
+        
+        ```
+        git clone git@github.com:broadinstitute/flipbook.git
+        cd flipbook
+        
+        # start server in dev mode so it reloads code on change
+        python3 -m flipbook /path/dir-with-images --dev-mode
+        ```
+        
 Keywords: curation,NGS,sequencing,STRs,REviewer,read visualization,machine learning
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## FlipBook
-
-This tool provides a simple user interface for quickly flipping through images stored in some directory on your computer.
-It also optionally shows a form where you can take notes or answer questions about each image or set of images.
-
-### Example uses:
-- manual curation / review of sequencing data visualization images such as those generated by [REViewer](https://www.illumina.com/science/genomics-research/reviewer-visualizing-alignments-short-reads-long-repeat.html) for short tandem repeat loci
-- machine learning training set creation
-- reviewing a pile of photos
-
-### Features:
-
-- simple way to flip through many local image files using your web browser
-- crawls a top-level directory to find .png, .jpeg, or .svg image files
-- web interface: home page lists all images
-- web interface: image pages show the image, an optional customizable form where you can take notes or answer questions about the image, next/previous page links, and optional other customizable info for context
-- use subdirectories to group images. Any images found in the same subdirectory will be shown on the same page  
-- optionally generate a static html website to share your images and form responses publicly. Example @ [https://broadinstitute.github.io/StrPileups/index.html](https://broadinstitute.github.io/StrPileups/index.html)
-
-
-
--------
-
-[![PyPI version](https://img.shields.io/pypi/v/flipbook.svg?style=flat)](https://pypi.org/project/flipbook/)  [![Supported Python versions](https://img.shields.io/pypi/pyversions/flipbook.svg)](https://shields.io/)
-
-
-### Install:
-
-```
-python3 -m pip install flipbook  
-```
-
-### Run:
-
-```
-python3 -m flipbook    # start server for all images in the current directory and subdirectories
-```
-
-Below are more example command lines. Run with `--help` to see all available options and their descriptions.
-
-```
-python3 -m flipbook -x temp -x keyword2  /path/dir-with-images    #  -x are keyword(s) of paths to skip and /path/dir-with-images is the top level dir to search instead of the current dir
-
-python3 -m flipbook -t /path/user_responses.xls    #  change where user responses get saved (default: flipbook_form_responses.tsv)
-
-python3 -m flipbook -m /path/metadata.tsv          #  provide a metadata table 
-```
-
-After the server is running, open your web browser to [http://localhost:8080](http://localhost:8080) to start reviewing images.
-
-
-### Screenshots
-
-Image page:
-
-<img width="1781" alt="image" src="https://user-images.githubusercontent.com/6240170/208694093-b5e7c97d-d2a4-46ab-9852-5db7157a2a3d.png">
-
-
-Home page:
-
-<img width="1786" alt="image" src="https://user-images.githubusercontent.com/6240170/208694216-0a550c82-cca2-4212-b22f-134844da95a5.png">
-
-
-### Options:
-
-- metadata table (`-m`)
-  
-  It's often useful to add extra info to the image pages to help with review - such as image descriptions, quality scores, etc.
-  To enable this, there are several ways to specify arbitrary key-value pairs to add to specific image pages.
-  The 1st way is to put a file called `flipbook_metadata.json` next to the image(s). All keys and values from this file
-  will appear on that image page. The 2nd way is to use `-m` to pass in a metadata table 
-  (`.tsv` or `.xls`) with a `Path` column + arbitrary other columns. If the `Path` value matches the relative directory containing 
-  the image(s), entries from that row will be added to this image page.  
-  
-  Since the keys and values are treated as html, they can be used to add more complex info - such as
-  colors, text formatting, <img ..> tags with images from other web pages, iframes containing entire sections of external pages, etc. 
-
-- responses table (`-t`)
-
-  As you fill in the forms at the top of the image pages, the responses are written to this table. If you later restart flipbook with the same `-t`, it will reload previous responses. You can also optionally use this table to provide additional columns to display - sometimes this can be more convenient than using `-m`. 
-  
-  *Default*: `flipbook_form_responses.tsv`
-
-- custom form schema (`--form-schema-json`)  
-   
-  If you'd like to use non-default questions in the image page forms, you can specify the path or url of a .json file containing a custom form schema. For examples of the expected format see [main/form_schema_examples](https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples)
-  
-- config file (`~/.flipbook_config`)
-
-  Most settings that can be provided on the command line can also be set via this YAML config file instead. For example:
-
-  *~/.flipbook_config*
-  ```
-  form-schema-json: /path/to/my-schema.json
-  hide-metadata-on-home-page: true
-  host: 127.0.0.1
-  port: 8080
-  ```
-
-  
-For more details, run:   
-```
-python3 -m flipbook --help
-```
-
-### Comparing reviews:
-
-If 2 or more people review the same images, the reviews can be compared using the `compare_form_response_tables` script.  
-
-For example:
-```
-python3 -m compare_form_response_tables egor_flipbook_form_responses.tsv  ben_flipbook_form_responses.tsv -o combined_responses.tsv -s1 egor -s2 ben
-```
-
-This script will print concordance stats, and output a `combined_responses.tsv` table that contains one image per row as well as each person's review of the image.  
-  
-To see the full list of args and descriptions, run `python3 -m compare_form_response_tables --help`
-
-### Development:
-
-To create a local dev instance, run
-
-```
-git clone git@github.com:broadinstitute/flipbook.git
-cd flipbook
-
-# start server in dev mode so it reloads code on change
-python3 -m flipbook /path/dir-with-images --dev-mode
-```
```

### Comparing `flipbook-0.12/README.md` & `flipbook-0.9.50/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 ## FlipBook
 
-This tool provides a simple user interface for quickly flipping through images stored in some directory on your computer.
-It also optionally shows a form where you can take notes or answer questions about each image or set of images.
+This tool starts a simple image server that lets you quickly flip through image files from a local directory using your web browser.
+Also, it optionally shows a customizable form where you can take notes or answer questions about each image or set of images.
 
 ### Example uses:
 - manual curation / review of sequencing data visualization images such as those generated by [REViewer](https://www.illumina.com/science/genomics-research/reviewer-visualizing-alignments-short-reads-long-repeat.html) for short tandem repeat loci
 - machine learning training set creation
 - reviewing a pile of photos
 
 ### Features:
 
 - simple way to flip through many local image files using your web browser
 - crawls a top-level directory to find .png, .jpeg, or .svg image files
 - web interface: home page lists all images
 - web interface: image pages show the image, an optional customizable form where you can take notes or answer questions about the image, next/previous page links, and optional other customizable info for context
 - use subdirectories to group images. Any images found in the same subdirectory will be shown on the same page  
-- optionally generate a static html website to share your images and form responses publicly. Example @ [https://broadinstitute.github.io/StrPileups/index.html](https://broadinstitute.github.io/StrPileups/index.html)
-
-
 
 -------
 
 [![PyPI version](https://img.shields.io/pypi/v/flipbook.svg?style=flat)](https://pypi.org/project/flipbook/)  [![Supported Python versions](https://img.shields.io/pypi/pyversions/flipbook.svg)](https://shields.io/)
 
 
 ### Install:
@@ -32,39 +29,26 @@
 
 ### Run:
 
 ```
 python3 -m flipbook    # start server for all images in the current directory and subdirectories
 ```
 
-Below are more example command lines. Run with `--help` to see all available options and their descriptions.
+Below are more examples. Run with `--help` to see all available options and their descriptions.
 
 ```
 python3 -m flipbook -x temp -x keyword2  /path/dir-with-images    #  -x are keyword(s) of paths to skip and /path/dir-with-images is the top level dir to search instead of the current dir
 
 python3 -m flipbook -t /path/user_responses.xls    #  change where user responses get saved (default: flipbook_form_responses.tsv)
 
 python3 -m flipbook -m /path/metadata.tsv          #  provide a metadata table 
 ```
 
 After the server is running, open your web browser to [http://localhost:8080](http://localhost:8080) to start reviewing images.
 
-
-### Screenshots
-
-Image page:
-
-<img width="1781" alt="image" src="https://user-images.githubusercontent.com/6240170/208694093-b5e7c97d-d2a4-46ab-9852-5db7157a2a3d.png">
-
-
-Home page:
-
-<img width="1786" alt="image" src="https://user-images.githubusercontent.com/6240170/208694216-0a550c82-cca2-4212-b22f-134844da95a5.png">
-
-
 ### Options:
 
 - metadata table (`-m`)
   
   It's often useful to add extra info to the image pages to help with review - such as image descriptions, quality scores, etc.
   To enable this, there are several ways to specify arbitrary key-value pairs to add to specific image pages.
   The 1st way is to put a file called `flipbook_metadata.json` next to the image(s). All keys and values from this file
```

### Comparing `flipbook-0.12/compare_form_response_tables.py` & `flipbook-0.9.50/compare_form_response_tables.py`

 * *Files identical despite different names*

### Comparing `flipbook-0.12/flipbook/__init__.py` & `flipbook-0.9.50/flipbook/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,30 @@
 import collections
 import configargparse
-from flask import Flask, Response, send_from_directory
-from flask_cors import CORS
-import jinja2
 import json
 import os
 import pandas as pd
-import pkg_resources
-import pkgutil
 import re
 import requests
-import shutil
-import sys
+from flipbook.utils import get_relative_directory_to_data_files_list, get_relative_directory_to_metadata, is_excel_table
 
-from flipbook.utils import get_relative_directory_to_data_files_list, get_relative_directory_to_metadata, \
-    is_excel_table, get_data_page_url, METADATA_JSON_FILE_TYPE, CONTENT_HTML_FILE_TYPE
 
 PATH_COLUMN = 'Path'
-WEBSITE_DIR = "flipbook_html"
-MAIN_PAGE_HEADER_FILENAME = "flipbook_main_page_header.html"
-DATA_PAGE_HEADER_FILENAME = "flipbook_data_page_header.html"
 
 p = configargparse.ArgumentParser(
     formatter_class=configargparse.DefaultsFormatter,
     add_config_file_help=True,
     add_env_var_help=True,
     config_file_parser_class=configargparse.YAMLConfigFileParser,
     default_config_files=["~/.flipbook_config"],
     args_for_writing_out_config_file=["--save-current-options-to-config-file"],
 )
 p.add_argument("-i", "--include", action="append", help="Only include files whose path contains this keyword")
 p.add_argument("-x", "--exclude", action="append", help="Skip files whose path contains this keyword. If both "
-               " --include and --exclude are specified, --exclude takes precedence over --include", default=[WEBSITE_DIR])
+                    " --include and --exclude are specified, --exclude takes precedence over --include")
 p.add_argument("-t", "--form-responses-table", default="flipbook_form_responses.tsv",
                help="The .tsv or .xls path where form responses are saved. If the file already exists,"
                     "it will be parsed for previous form responses and then updated as the user fills in the form(s)."
                     "If the file doesn't exist, it will be created after the 1st form response.")
 p.add_argument("-m", "--metadata-table", default="flipbook_metadata.tsv",
                help="The .tsv or .xls path containing metadata to show on data pages. There are two optional ways "
                     "to add metadata to the data pages. The 1st way is to put a 'flipbook_metadata.json' file "
@@ -43,28 +32,20 @@
                     "the json file will be shown at the top of the data page that displays those images). "
                     "The other way is to specify this table, which needs to have a 'Path' column with relative "
                     "directory paths that contain images and data files. The data page corresponding to those "
                     "directory paths will then display values from the other columns in this table. If both this table "
                     "and 'flipbook_metadata.json' files are found, the values from this table will override values in "
                     "the 'flipbook_metadata.json' files.")
 p.add_argument("-j", "--form-schema-json", help="Path of .json file containing a custom form schema. For the expected format "
-               "see https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples")
+                    "see https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples")
 p.add_argument("-s", "--sort-by", action="append", help="Order pages by metadata column(s)")
-p.add_argument("-r", "--reverse-sort", action="store_true", help="Reverses the sort order")
 p.add_argument("--hide-metadata-on-home-page", action="store_true", help="Don't show metadata columns in the "
                "home page table")
 p.add_argument("--add-metadata-to-form-responses-table", action="store_true", help="Also write metadata columns to the "
-               "form responses table when saving users' form responses")
-
-p.add_argument("--generate-static-website", action="store_true", help="Instead of starting a web server, this option "
-               "causes FlipBook to write out a set of static html pages for all the images it finds and then exit. "
-               "The generated pages can then be viewed in a browser, uploaded to some other web server (such as "
-               "GitHub Pages, embedded in another existing website, etc. The generated web pages are identical to "
-               "the standard FlipBook user interface except they don't contain the forms for entering responses about "
-               "each image - and so just allow flipping through the images.")
+                "form responses table when saving users' form responses")
 
 #p.add_argument("-c", "--config-file", help="Path of yaml config file", env_var="FLIPBOOK_CONFIG_FILE")
 p.add_argument("-v", "--verbose", action='count', default=0, help="Print more info")
 p.add_argument("--host", default="127.0.0.1", env_var="HOST", help="Listen for connections on this hostname or IP")
 p.add_argument("-p", "--port", default="8080", env_var="PORT", type=int, help="Listen for connections on this port")
 p.add_argument("--dev-mode", action="store_true", env_var="DEV", help="Run server in developer mode so it reloads "
                "html templates and source code if they're changed")
@@ -169,17 +150,14 @@
     {
         "type": "text",
         "columnName": "Notes",
         "size": 60
     }
 ]
 
-if args.generate_static_website:
-    FORM_SCHEMA = {}
-
 if args.form_schema_json:
     print(f"Loading form schema from {args.form_schema_json}")
     try:
         if os.path.isfile(args.form_schema_json):
             with open(args.form_schema_json, "rt") as f:
                 FORM_SCHEMA = json.load(f)
         elif args.form_schema_json.startswith("http"):
@@ -297,104 +275,8 @@
                 continue
             metadata_value = RELATIVE_DIRECTORY_TO_METADATA.get(relative_dir, {}).get(s)
             if metadata_value is not None:
                 sort_key.append(str(metadata_value))
                 continue
         return tuple(sort_key)
 
-    RELATIVE_DIRECTORY_TO_DATA_FILES_LIST = sorted(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST, key=get_sort_key, reverse=args.reverse_sort)
-
-
-def send_file(path):
-    print(f"Sending {args.directory} {path}")
-    if path.startswith("/static/"):
-        mimetype = None
-        if path.endswith(".png"):
-            mimetype="image/png"
-        return Response(pkg_resources.resource_stream('flipbook', path), mimetype=mimetype)
-
-    return send_from_directory(args.directory, path, as_attachment=True)
-
-
-def get_static_data_page_url(page_number, last):
-    i = page_number - 1
-    if i < 0 or i >= len(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST):
-        raise ValueError(f"page_number arg is out of bounds. It must be between 1 and {len(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST)}")
-
-    relative_dir, _ = RELATIVE_DIRECTORY_TO_DATA_FILES_LIST[i]
-    name = relative_dir.replace("/", "__")
-    return f"page_{name}.html"
-
-
-def main():
-    # add a ctime(..) function to allow the last-changed-time of a path to be computed within a jinja template
-    jinja2.environment.DEFAULT_FILTERS['ctime'] = lambda path: int(os.path.getctime(path)) if os.path.isfile(path) else 0
-
-    from flipbook.main_list import main_list_handler
-    from flipbook.data_page import data_page_handler
-    from flipbook.save import save_form_handler
-
-    app = Flask(__name__)
-
-    if args.generate_static_website:
-        os.chdir(args.directory)
-        os.makedirs(WEBSITE_DIR, exist_ok=True)
-
-        with open(os.path.join(WEBSITE_DIR, "index.html"), "wt") as f:
-            f.write(main_list_handler(is_static_website=True).get_data(as_text=True))
-        with open(os.path.join(WEBSITE_DIR, "favicon.png"), "wb") as f:
-            f.write(pkgutil.get_data('flipbook', 'static/images/favicon.png'))
-
-        flipbook_package_dir = sys.modules['flipbook'].__path__[0]
-        static_dir = os.path.join(flipbook_package_dir, "static")
-        print("Copying", static_dir)
-        shutil.copytree(static_dir, os.path.join(WEBSITE_DIR, "static"))
-
-        last_page_number = len(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST)
-        for i, (relative_directory, data_file_types_and_paths) in enumerate(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST):
-            page_number = i + 1
-            with app.test_request_context(get_data_page_url(page_number, last_page_number)):
-                page_dir = os.path.join(WEBSITE_DIR, relative_directory)
-                os.makedirs(page_dir, exist_ok=True)
-                for data_file_type, data_file in data_file_types_and_paths:
-                    if data_file_type in (METADATA_JSON_FILE_TYPE, CONTENT_HTML_FILE_TYPE):
-                        continue
-                    print("Copying", data_file_type, data_file, "to", page_dir)
-                    shutil.copy(data_file, page_dir)
-
-                with open(os.path.join(WEBSITE_DIR, get_static_data_page_url(page_number, last_page_number)), "wt") as f:
-                    f.write(data_page_handler(is_static_website=True).get_data(as_text=True))
-        print("Done")
-        print(f"Generated static website in the {os.path.realpath(WEBSITE_DIR)} directory")
-        sys.exit(0)
-
-    # start web server
-    CORS(app)
-
-    app.url_map.strict_slashes = False
-
-    app.add_url_rule('/', view_func=main_list_handler, methods=['GET'])
-    app.add_url_rule('/page', view_func=data_page_handler, methods=['POST', 'GET'])
-    app.add_url_rule('/save', view_func=save_form_handler, methods=['POST'])
-    app.add_url_rule('/<path:path>', view_func=send_file, methods=['GET'])
-
-    host = os.environ.get('HOST', args.host)
-    port = int(os.environ.get('PORT', args.port))
-    if args.verbose:
-        print(f"Connecting to {host}:{port}")
-
-    #if args.production_server:
-    #    from whitenoise import WhiteNoise
-    #    app.wsgi_app = WhiteNoise(app.wsgi_app, root="static/")
-    #    waitress.serve(app, host=host, port=port)
-    #else:
-    try:
-        os.environ["WERKZEUG_RUN_MAIN"] = "true"
-        app.run(
-            debug=args.dev_mode,
-            host=host,
-            port=port)
-    except OSError as e:
-        if "already in use" in str(e):
-            p.error(f"Port {port} is already in use by another process. Use -p to specify a different port.")
-        else:
-            raise e
+    RELATIVE_DIRECTORY_TO_DATA_FILES_LIST = sorted(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST, key=get_sort_key)
```

### Comparing `flipbook-0.12/flipbook/data_page.py` & `flipbook-0.9.50/flipbook/data_page.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
 from flask import request, Response
 from pprint import pprint, pformat
 from flipbook import args, RELATIVE_DIRECTORY_TO_DATA_FILES_LIST, FORM_SCHEMA, FORM_RESPONSES, \
-    RELATIVE_DIRECTORY_TO_METADATA, FORM_RADIO_BUTTON_KEYBOARD_SHORTCUTS, EXTRA_DATA_IN_FORM_RESPONSES_TABLE, \
-    get_static_data_page_url, DATA_PAGE_HEADER_FILENAME
-from flipbook.utils import load_jinja_template, get_data_page_url, CONTENT_HTML_FILE_TYPE, \
-    IMAGE_FILE_TYPE
+    RELATIVE_DIRECTORY_TO_METADATA, FORM_RADIO_BUTTON_KEYBOARD_SHORTCUTS, EXTRA_DATA_IN_FORM_RESPONSES_TABLE
+from flipbook.utils import load_jinja_template, get_data_page_url, CONTENT_HTML_FILE_TYPE, IMAGE_FILE_TYPE
 
 DATA_PAGE_TEMPLATE = None
 
 
-def data_page_handler(is_static_website=False):
+def data_page_handler():
     global DATA_PAGE_TEMPLATE
     if DATA_PAGE_TEMPLATE is None or args.dev_mode:
         DATA_PAGE_TEMPLATE = load_jinja_template("data_page")
 
     if args.verbose:
         print(f"data_page_handler received {request.url}")
 
@@ -33,28 +31,15 @@
         print(f"data_page_handler request.form: {bool(request.form)} {pformat(request.form)}")
         print(f"data_page_handler request.args: {bool(request.args)} {pformat(request.args)}")
         print(f"data_page_handler request.values: {bool(request.values)} {pformat(request.values)}")
         print(f"data_page_handler request.get_json(..): {bool(json_args)} {pformat(json_args)}")
         print(f"data_page_handler request.__dict__: {pformat(request.__dict__)}")
         print(f"data_page_handler params: {params}")
 
-    i = None
-    relative_dir = params.get("path")
-    if relative_dir:
-        # override i
-        for idx, (known_relative_dir, _) in enumerate(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST):
-            if relative_dir == known_relative_dir:
-                i = idx + 1
-                break
-        else:
-            print(f"ERROR: path param '{relative_dir}' not recognized. Falling back on using i param.")
-
-    if i is None:
-        i = params.get("i")
-
+    i = params.get("i")
     try:
         if isinstance(i, list):
             i = int(i[0])
         else:
             i = int(i)
     except (ValueError, TypeError) as e:
         print(f"ERROR: unable to parse parameter i: '{i}': {type(e).__name__} {e}. Setting i = 1.")
@@ -103,29 +88,22 @@
             content_html_strings.append((data_file_path, content_string))
 
     if args.verbose:
         print(f"data_page_handler returning i={i}, last={last}, relative_directory={relative_dir}, "
               f"{len(image_file_paths)} image_file_paths, {len(metadata_json_dict)} records in metadata_json_dict, "
               f"{len(content_html_strings)} content_html_strings")
 
-    data_page_header_html = ""
-    if os.path.isfile(os.path.join(args.directory, DATA_PAGE_HEADER_FILENAME)):
-        with open(os.path.join(args.directory, DATA_PAGE_HEADER_FILENAME), "rt") as f:
-            data_page_header_html = f.read()
-
     html = DATA_PAGE_TEMPLATE.render(
         i=i,
         last=last,
-        header_html=data_page_header_html,
         relative_directory=relative_dir,
         image_file_paths=image_file_paths,
         metadata_json_dict=metadata_json_dict,
         content_html_strings=content_html_strings,
-        get_data_page_url=get_data_page_url if not is_static_website else get_static_data_page_url,
+        get_data_page_url=get_data_page_url,
         form_schema=FORM_SCHEMA,
         form_radio_button_keyboard_shortcuts=FORM_RADIO_BUTTON_KEYBOARD_SHORTCUTS,
         form_responses=FORM_RESPONSES.get(relative_dir, {}),
-        is_static_website=is_static_website,
     )
 
     return Response(html, mimetype='text/html')
```

### Comparing `flipbook-0.12/flipbook/main_list.py` & `flipbook-0.9.50/flipbook/main_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-import os
-
 from flask import request, Response
+
 from flipbook import args, RELATIVE_DIRECTORY_TO_DATA_FILES_LIST, FORM_RESPONSES, FORM_SCHEMA_COLUMNS, \
     RELATIVE_DIRECTORY_TO_METADATA, METADATA_COLUMNS, EXTRA_DATA_IN_FORM_RESPONSES_TABLE, \
-    EXTRA_COLUMNS_IN_FORM_RESPONSES_TABLE, get_static_data_page_url, MAIN_PAGE_HEADER_FILENAME
+    EXTRA_COLUMNS_IN_FORM_RESPONSES_TABLE
 from flipbook.utils import load_jinja_template, get_data_page_url
 
 MAIN_LIST_TEMPLATE = None
 
 
-def main_list_handler(is_static_website=False):
+def main_list_handler():
     global MAIN_LIST_TEMPLATE
     if MAIN_LIST_TEMPLATE is None or args.dev_mode:
         MAIN_LIST_TEMPLATE = load_jinja_template("main_list")
 
     if args.verbose:
-        print(f"main_list_handler received {request.url}")
+        print(f"main_list_handler recieved {request.url}")
 
     data_files_list = [
         (page_number + 1, relative_directory, data_file_types_and_paths)
         for page_number, (relative_directory, data_file_types_and_paths) in enumerate(RELATIVE_DIRECTORY_TO_DATA_FILES_LIST)
     ]
 
     # combine metadata from 2 potential sources: RELATIVE_DIRECTORY_TO_METADATA and EXTRA_DATA_IN_FORM_RESPONSES_TABLE
     metadata_columns = []
     metadata_dict = {}
     if not args.hide_metadata_on_home_page:
-        metadata_columns = METADATA_COLUMNS
-        if not is_static_website:
-            metadata_columns += EXTRA_COLUMNS_IN_FORM_RESPONSES_TABLE
+        metadata_columns = METADATA_COLUMNS + EXTRA_COLUMNS_IN_FORM_RESPONSES_TABLE
         for relative_dir in list(RELATIVE_DIRECTORY_TO_METADATA.keys()) + list(EXTRA_DATA_IN_FORM_RESPONSES_TABLE.keys()):
             metadata_dict[relative_dir] = dict(RELATIVE_DIRECTORY_TO_METADATA.get(relative_dir, {}))
             metadata_dict[relative_dir].update(dict(EXTRA_DATA_IN_FORM_RESPONSES_TABLE.get(relative_dir, {})))
 
-    main_page_header_html = ""
-    if os.path.isfile(os.path.join(args.directory, MAIN_PAGE_HEADER_FILENAME)):
-        with open(os.path.join(args.directory, MAIN_PAGE_HEADER_FILENAME), "rt") as f:
-            main_page_header_html = f.read()
-
     html = MAIN_LIST_TEMPLATE.render(
-        header_html=main_page_header_html,
         data_files_list=data_files_list,
-        get_data_page_url=get_data_page_url if not is_static_website else get_static_data_page_url,
+        get_data_page_url=get_data_page_url,
         form_column_names=FORM_SCHEMA_COLUMNS,
         form_responses_dict=FORM_RESPONSES,
         metadata_column_names=metadata_columns,
         metadata_dict=metadata_dict,
         form_responses_table_path=args.form_responses_table,
-        is_static_website=is_static_website,
     )
 
     return Response(html, mimetype='text/html')
 
+
```

### Comparing `flipbook-0.12/flipbook/save.py` & `flipbook-0.9.50/flipbook/save.py`

 * *Files identical despite different names*

### Comparing `flipbook-0.12/flipbook/utils.py` & `flipbook-0.9.50/flipbook/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 CONTENT_HTML_FILE_TYPE = "content_html"
 
 METADATA_JSON_FILE_SUFFIX = "flipbook_metadata.json"
 CONTENT_HTML_FILE_SUFFIX = "flipbook_content.html"
 
 
 def get_relative_directory_to_data_files_list(
-        top_level_dir,
-        keywords_to_include,
-        keywords_to_exclude,
-        suffixes=("svg", "png", "jpeg", "jpg", "gif", "webp", CONTENT_HTML_FILE_SUFFIX, METADATA_JSON_FILE_SUFFIX),
-        verbose=False):
+    top_level_dir,
+    keywords_to_include,
+    keywords_to_exclude,
+    suffixes=("svg", "png", "jpeg", "jpg", "gif", "webp", CONTENT_HTML_FILE_SUFFIX, METADATA_JSON_FILE_SUFFIX),
+    verbose=False):
     data_file_paths = []
 
     print(f"Looking for " + ", ".join(suffixes[:-1]) + f", and {suffixes[-1]} files in {top_level_dir}")
     if keywords_to_include or keywords_to_exclude:
         sys.stdout.write("Keeping only file paths that ")
         if keywords_to_include:
-            sys.stdout.write("contain " + " and ".join([f'"{k}"' for k in keywords_to_include]))
+            sys.stdout.write("contain " + " or ".join([f'"{k}"' for k in keywords_to_include]))
         if keywords_to_include and keywords_to_exclude:
             sys.stdout.write(" and ")
         if keywords_to_exclude:
             sys.stdout.write("don't contain " + " or ".join([f'"{k}"' for k in keywords_to_exclude]))
         sys.stdout.write("\n")
 
     glob_string = "|".join([f"{top_level_dir}/**/*{suffix}" for suffix in suffixes]).replace("\\", "/")
@@ -51,18 +51,18 @@
         else:
             raise Exception(f"Unexpected file suffix: {data_file_path}")
 
         data_file_counter_by_suffix[data_file_suffix] += 1
         relative_data_file_path = os.path.relpath(data_file_path, top_level_dir)
 
         if keywords_to_include:
-            included_keyword_misses = [k for k in keywords_to_include if k not in relative_data_file_path] if keywords_to_include else []
-            if included_keyword_misses:
+            included_keyword_matches = [k for k in keywords_to_include if k in relative_data_file_path] if keywords_to_include else []
+            if not included_keyword_matches:
                 if verbose:
-                    print(f"Skipping {data_file_suffix} file: {relative_data_file_path} - it doesn't contain --include keyword(s): ", ", ".join(included_keyword_misses))
+                    print(f"Skipping {data_file_suffix} file: {relative_data_file_path} - it doesn't contain any --include keyword.")
                 continue
 
         excluded_keyword_matches = [k for k in keywords_to_exclude if k in relative_data_file_path] if keywords_to_exclude else []
         if excluded_keyword_matches:
             excluded_keyword_to_matching_paths[excluded_keyword_matches[0]].append(relative_data_file_path)
             if verbose:
                 print(f"Skipping {data_file_suffix} file: {relative_data_file_path} - it contains excluded keyword: '{excluded_keyword_matches[0]}'")
```

### Comparing `flipbook-0.12/flipbook.egg-info/PKG-INFO` & `flipbook-0.9.50/flipbook.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,134 @@
 Metadata-Version: 2.1
 Name: flipbook
-Version: 0.12
+Version: 0.9.50
 Summary: Starts a simple image server that lets you quickly flip through image files from a local directory using your web browser and optionally answering customizable questions about each one
 Home-page: https://github.com/broadinstitute/flipbook
 License: MIT
+Description: ## FlipBook
+        
+        This tool starts a simple image server that lets you quickly flip through image files from a local directory using your web browser.
+        Also, it optionally shows a customizable form where you can take notes or answer questions about each image or set of images.
+        
+        ### Example uses:
+        - manual curation / review of sequencing data visualization images such as those generated by [REViewer](https://www.illumina.com/science/genomics-research/reviewer-visualizing-alignments-short-reads-long-repeat.html) for short tandem repeat loci
+        - machine learning training set creation
+        - reviewing a pile of photos
+        
+        ### Features:
+        
+        - simple way to flip through many local image files using your web browser
+        - crawls a top-level directory to find .png, .jpeg, or .svg image files
+        - web interface: home page lists all images
+        - web interface: image pages show the image, an optional customizable form where you can take notes or answer questions about the image, next/previous page links, and optional other customizable info for context
+        - use subdirectories to group images. Any images found in the same subdirectory will be shown on the same page  
+        
+        -------
+        
+        [![PyPI version](https://img.shields.io/pypi/v/flipbook.svg?style=flat)](https://pypi.org/project/flipbook/)  [![Supported Python versions](https://img.shields.io/pypi/pyversions/flipbook.svg)](https://shields.io/)
+        
+        
+        ### Install:
+        
+        ```
+        python3 -m pip install flipbook  
+        ```
+        
+        ### Run:
+        
+        ```
+        python3 -m flipbook    # start server for all images in the current directory and subdirectories
+        ```
+        
+        Below are more examples. Run with `--help` to see all available options and their descriptions.
+        
+        ```
+        python3 -m flipbook -x temp -x keyword2  /path/dir-with-images    #  -x are keyword(s) of paths to skip and /path/dir-with-images is the top level dir to search instead of the current dir
+        
+        python3 -m flipbook -t /path/user_responses.xls    #  change where user responses get saved (default: flipbook_form_responses.tsv)
+        
+        python3 -m flipbook -m /path/metadata.tsv          #  provide a metadata table 
+        ```
+        
+        After the server is running, open your web browser to [http://localhost:8080](http://localhost:8080) to start reviewing images.
+        
+        ### Options:
+        
+        - metadata table (`-m`)
+          
+          It's often useful to add extra info to the image pages to help with review - such as image descriptions, quality scores, etc.
+          To enable this, there are several ways to specify arbitrary key-value pairs to add to specific image pages.
+          The 1st way is to put a file called `flipbook_metadata.json` next to the image(s). All keys and values from this file
+          will appear on that image page. The 2nd way is to use `-m` to pass in a metadata table 
+          (`.tsv` or `.xls`) with a `Path` column + arbitrary other columns. If the `Path` value matches the relative directory containing 
+          the image(s), entries from that row will be added to this image page.  
+          
+          Since the keys and values are treated as html, they can be used to add more complex info - such as
+          colors, text formatting, <img ..> tags with images from other web pages, iframes containing entire sections of external pages, etc. 
+        
+        - responses table (`-t`)
+        
+          As you fill in the forms at the top of the image pages, the responses are written to this table. If you later restart flipbook with the same `-t`, it will reload previous responses. You can also optionally use this table to provide additional columns to display - sometimes this can be more convenient than using `-m`. 
+          
+          *Default*: `flipbook_form_responses.tsv`
+        
+        - custom form schema (`--form-schema-json`)  
+           
+          If you'd like to use non-default questions in the image page forms, you can specify the path or url of a .json file containing a custom form schema. For examples of the expected format see [main/form_schema_examples](https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples)
+          
+        - config file (`~/.flipbook_config`)
+        
+          Most settings that can be provided on the command line can also be set via this YAML config file instead. For example:
+        
+          *~/.flipbook_config*
+          ```
+          form-schema-json: /path/to/my-schema.json
+          hide-metadata-on-home-page: true
+          host: 127.0.0.1
+          port: 8080
+          ```
+        
+          
+        For more details, run:   
+        ```
+        python3 -m flipbook --help
+        ```
+        
+        ### Comparing reviews:
+        
+        If 2 or more people review the same images, the reviews can be compared using the `compare_form_response_tables` script.  
+        
+        For example:
+        ```
+        python3 -m compare_form_response_tables egor_flipbook_form_responses.tsv  ben_flipbook_form_responses.tsv -o combined_responses.tsv -s1 egor -s2 ben
+        ```
+        
+        This script will print concordance stats, and output a `combined_responses.tsv` table that contains one image per row as well as each person's review of the image.  
+          
+        To see the full list of args and descriptions, run `python3 -m compare_form_response_tables --help`
+        
+        ### Development:
+        
+        To create a local dev instance, run
+        
+        ```
+        git clone git@github.com:broadinstitute/flipbook.git
+        cd flipbook
+        
+        # start server in dev mode so it reloads code on change
+        python3 -m flipbook /path/dir-with-images --dev-mode
+        ```
+        
 Keywords: curation,NGS,sequencing,STRs,REviewer,read visualization,machine learning
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## FlipBook
-
-This tool provides a simple user interface for quickly flipping through images stored in some directory on your computer.
-It also optionally shows a form where you can take notes or answer questions about each image or set of images.
-
-### Example uses:
-- manual curation / review of sequencing data visualization images such as those generated by [REViewer](https://www.illumina.com/science/genomics-research/reviewer-visualizing-alignments-short-reads-long-repeat.html) for short tandem repeat loci
-- machine learning training set creation
-- reviewing a pile of photos
-
-### Features:
-
-- simple way to flip through many local image files using your web browser
-- crawls a top-level directory to find .png, .jpeg, or .svg image files
-- web interface: home page lists all images
-- web interface: image pages show the image, an optional customizable form where you can take notes or answer questions about the image, next/previous page links, and optional other customizable info for context
-- use subdirectories to group images. Any images found in the same subdirectory will be shown on the same page  
-- optionally generate a static html website to share your images and form responses publicly. Example @ [https://broadinstitute.github.io/StrPileups/index.html](https://broadinstitute.github.io/StrPileups/index.html)
-
-
-
--------
-
-[![PyPI version](https://img.shields.io/pypi/v/flipbook.svg?style=flat)](https://pypi.org/project/flipbook/)  [![Supported Python versions](https://img.shields.io/pypi/pyversions/flipbook.svg)](https://shields.io/)
-
-
-### Install:
-
-```
-python3 -m pip install flipbook  
-```
-
-### Run:
-
-```
-python3 -m flipbook    # start server for all images in the current directory and subdirectories
-```
-
-Below are more example command lines. Run with `--help` to see all available options and their descriptions.
-
-```
-python3 -m flipbook -x temp -x keyword2  /path/dir-with-images    #  -x are keyword(s) of paths to skip and /path/dir-with-images is the top level dir to search instead of the current dir
-
-python3 -m flipbook -t /path/user_responses.xls    #  change where user responses get saved (default: flipbook_form_responses.tsv)
-
-python3 -m flipbook -m /path/metadata.tsv          #  provide a metadata table 
-```
-
-After the server is running, open your web browser to [http://localhost:8080](http://localhost:8080) to start reviewing images.
-
-
-### Screenshots
-
-Image page:
-
-<img width="1781" alt="image" src="https://user-images.githubusercontent.com/6240170/208694093-b5e7c97d-d2a4-46ab-9852-5db7157a2a3d.png">
-
-
-Home page:
-
-<img width="1786" alt="image" src="https://user-images.githubusercontent.com/6240170/208694216-0a550c82-cca2-4212-b22f-134844da95a5.png">
-
-
-### Options:
-
-- metadata table (`-m`)
-  
-  It's often useful to add extra info to the image pages to help with review - such as image descriptions, quality scores, etc.
-  To enable this, there are several ways to specify arbitrary key-value pairs to add to specific image pages.
-  The 1st way is to put a file called `flipbook_metadata.json` next to the image(s). All keys and values from this file
-  will appear on that image page. The 2nd way is to use `-m` to pass in a metadata table 
-  (`.tsv` or `.xls`) with a `Path` column + arbitrary other columns. If the `Path` value matches the relative directory containing 
-  the image(s), entries from that row will be added to this image page.  
-  
-  Since the keys and values are treated as html, they can be used to add more complex info - such as
-  colors, text formatting, <img ..> tags with images from other web pages, iframes containing entire sections of external pages, etc. 
-
-- responses table (`-t`)
-
-  As you fill in the forms at the top of the image pages, the responses are written to this table. If you later restart flipbook with the same `-t`, it will reload previous responses. You can also optionally use this table to provide additional columns to display - sometimes this can be more convenient than using `-m`. 
-  
-  *Default*: `flipbook_form_responses.tsv`
-
-- custom form schema (`--form-schema-json`)  
-   
-  If you'd like to use non-default questions in the image page forms, you can specify the path or url of a .json file containing a custom form schema. For examples of the expected format see [main/form_schema_examples](https://github.com/broadinstitute/flipbook/tree/main/form_schema_examples)
-  
-- config file (`~/.flipbook_config`)
-
-  Most settings that can be provided on the command line can also be set via this YAML config file instead. For example:
-
-  *~/.flipbook_config*
-  ```
-  form-schema-json: /path/to/my-schema.json
-  hide-metadata-on-home-page: true
-  host: 127.0.0.1
-  port: 8080
-  ```
-
-  
-For more details, run:   
-```
-python3 -m flipbook --help
-```
-
-### Comparing reviews:
-
-If 2 or more people review the same images, the reviews can be compared using the `compare_form_response_tables` script.  
-
-For example:
-```
-python3 -m compare_form_response_tables egor_flipbook_form_responses.tsv  ben_flipbook_form_responses.tsv -o combined_responses.tsv -s1 egor -s2 ben
-```
-
-This script will print concordance stats, and output a `combined_responses.tsv` table that contains one image per row as well as each person's review of the image.  
-  
-To see the full list of args and descriptions, run `python3 -m compare_form_response_tables --help`
-
-### Development:
-
-To create a local dev instance, run
-
-```
-git clone git@github.com:broadinstitute/flipbook.git
-cd flipbook
-
-# start server in dev mode so it reloads code on change
-python3 -m flipbook /path/dir-with-images --dev-mode
-```
```

### Comparing `flipbook-0.12/setup.py` & `flipbook-0.9.50/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,66 +1,48 @@
 import os
 import sys
 from setuptools import setup
 
-# NOTE: This package must be installed with pip, and not with python3 setup.py install
-# in order for static files to work on the webpage
 command = sys.argv[-1]
 if command == 'publish':
     os.system('rm -rf dist')
     os.system('python3 setup.py sdist')
     os.system('python3 setup.py bdist_wheel')
     os.system('twine upload dist/*whl dist/*gz')
     sys.exit()
 
 with open("README.md", "rt") as fh:
     long_description = fh.read()
 
 install_requires = [
-    "configargparse>=1.5.5",
-    "flask-cors>=4.0.0",
-    "gunicorn>=21.2.0",
-    "jinja2>=3.1.2",
-    "openpyxl>=3.1.1",
-    "pandas>=2.0.3",
-    "requests>=2.31.0",
-    "wcmatch>=8.4.1",
-    "xlrd>=2.0.1",
-    "xlwt>=1.3.0",
-
-    # NOTE: there is a "KeyError: 'WERKZEUG_SERVER_FD'" in the latest versions of Werkzeug
-    # when starting the server, so use a previous version of flask and Werkzeug
-    "flask==2.1",
-    "Werkzeug==2.0.0",
+    "configargparse",
+    "flask",
+    "flask-cors",
+    "gunicorn",
+    "jinja2",
+    "openpyxl",
+    "pandas",
+    "requests",
+    "wcmatch",
+    "xlrd",
+    "xlwt",
 ]
 
 setup(
     name='flipbook',
-    version="0.12",
+    version="0.9.50",
     description="Starts a simple image server that lets you quickly flip through image files from a local directory "
                 "using your web browser and optionally answering customizable questions about each one",
     install_requires=install_requires,
-    entry_points = {
-        'console_scripts': [
-            'flipbook = flipbook:main',
-        ],
-    },
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=["flipbook"],
     py_modules=["compare_form_response_tables"],
     include_package_data=True,
-    package_data={'': [
-        'static/*/*.*',
-        'static/*/*/*.*',
-        'static/*/*/*/*.*',
-        'static/*/*/*/*/*.*',
-        'static/*/*/*/*/*/*.*',
-        'templates/*.*',
-    ]},
+    package_data={'': ['*/*.png', '*/*.html']},
     python_requires=">=3.7",
     license="MIT",
     keywords='curation, NGS, sequencing, STRs, REviewer, read visualization, machine learning',
     url='https://github.com/broadinstitute/flipbook',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

