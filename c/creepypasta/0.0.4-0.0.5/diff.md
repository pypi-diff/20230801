# Comparing `tmp/creepypasta-0.0.4.tar.gz` & `tmp/creepypasta-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "creepypasta-0.0.4.tar", last modified: Tue Aug  1 11:41:05 2023, max compression
+gzip compressed data, was "creepypasta-0.0.5.tar", last modified: Tue Aug  1 16:15:46 2023, max compression
```

## Comparing `creepypasta-0.0.4.tar` & `creepypasta-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.328323 creepypasta-0.0.4/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-08-01 11:41:05.328385 creepypasta-0.0.4/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-07-31 03:53:30.000000 creepypasta-0.0.4/README.md
--rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-08-01 10:26:33.000000 creepypasta-0.0.4/pyproject.toml
--rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-08-01 11:41:05.328646 creepypasta-0.0.4/setup.cfg
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.325790 creepypasta-0.0.4/src/
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.327154 creepypasta-0.0.4/src/creepypasta/
--rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-07-31 04:40:38.000000 creepypasta-0.0.4/src/creepypasta/__init__.py
--rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-07-28 13:46:50.000000 creepypasta-0.0.4/src/creepypasta/pasta_listings.py
--rw-r--r--   0 sandrews   (501) staff       (20)    17564 2023-08-01 11:34:15.000000 creepypasta-0.0.4/src/creepypasta/pasta_stories.py
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.327989 creepypasta-0.0.4/src/creepypasta.egg-info/
--rw-r--r--   0 sandrews   (501) staff       (20)      661 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/PKG-INFO
--rw-r--r--   0 sandrews   (501) staff       (20)      342 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/SOURCES.txt
--rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/dependency_links.txt
--rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/requires.txt
--rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-08-01 11:41:05.000000 creepypasta-0.0.4/src/creepypasta.egg-info/top_level.txt
-drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 11:41:05.328106 creepypasta-0.0.4/test/
--rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.4/test/test-units.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 16:15:46.353575 creepypasta-0.0.5/
+-rw-r--r--   0 sandrews   (501) staff       (20)     1066 2023-08-01 11:48:20.000000 creepypasta-0.0.5/LICENSE
+-rw-r--r--   0 sandrews   (501) staff       (20)      683 2023-08-01 16:15:46.353627 creepypasta-0.0.5/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)       66 2023-08-01 11:48:20.000000 creepypasta-0.0.5/README.md
+-rw-r--r--   0 sandrews   (501) staff       (20)      898 2023-08-01 16:14:37.000000 creepypasta-0.0.5/pyproject.toml
+-rw-r--r--   0 sandrews   (501) staff       (20)      918 2023-08-01 16:15:46.353903 creepypasta-0.0.5/setup.cfg
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 16:15:46.350863 creepypasta-0.0.5/src/
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 16:15:46.352289 creepypasta-0.0.5/src/creepypasta/
+-rw-r--r--   0 sandrews   (501) staff       (20)       59 2023-08-01 11:48:20.000000 creepypasta-0.0.5/src/creepypasta/__init__.py
+-rw-r--r--   0 sandrews   (501) staff       (20)     8825 2023-08-01 11:48:20.000000 creepypasta-0.0.5/src/creepypasta/pasta_listings.py
+-rw-r--r--   0 sandrews   (501) staff       (20)    17564 2023-08-01 11:48:20.000000 creepypasta-0.0.5/src/creepypasta/pasta_stories.py
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 16:15:46.353206 creepypasta-0.0.5/src/creepypasta.egg-info/
+-rw-r--r--   0 sandrews   (501) staff       (20)      683 2023-08-01 16:15:46.000000 creepypasta-0.0.5/src/creepypasta.egg-info/PKG-INFO
+-rw-r--r--   0 sandrews   (501) staff       (20)      350 2023-08-01 16:15:46.000000 creepypasta-0.0.5/src/creepypasta.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)        1 2023-08-01 16:15:46.000000 creepypasta-0.0.5/src/creepypasta.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)      181 2023-08-01 16:15:46.000000 creepypasta-0.0.5/src/creepypasta.egg-info/requires.txt
+-rw-r--r--   0 sandrews   (501) staff       (20)       12 2023-08-01 16:15:46.000000 creepypasta-0.0.5/src/creepypasta.egg-info/top_level.txt
+drwxr-xr-x   0 sandrews   (501) staff       (20)        0 2023-08-01 16:15:46.353320 creepypasta-0.0.5/test/
+-rw-r--r--   0 sandrews   (501) staff       (20)     2453 2023-07-28 13:51:00.000000 creepypasta-0.0.5/test/test-units.py
```

### Comparing `creepypasta-0.0.4/PKG-INFO` & `creepypasta-0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # 🕯️ creepypasta
 
 Docs => https://jellomoat.github.io/pasta/
```

### Comparing `creepypasta-0.0.4/pyproject.toml` & `creepypasta-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 requires = [
     "setuptools>=61.0",
     "beautifulsoup4>=4.12.2",
     "lxml>=4.9.3",
     "requests==2.31.0",
     "pandas==2.0.3",
     "pathlib==1.0.1",
-    "chromedriver-binary-auto>=0.2.6",
+    "chromedriver-binary-auto>=0.3.0",
     "selenium==4.10.0",
     "selenium-wire==5.1.0",
     "tqdm==4.65.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "creepypasta"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Stephanie Andrews", email="jellomoat@gmail.com" },
 ]
 description = "A small package to crawl CreepyPasta and parse into structured data."
 
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `creepypasta-0.0.4/setup.cfg` & `creepypasta-0.0.5/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = creepypasta
-version = 0.0.3
+version = 0.0.5
 author = Stephanie Andrews
 author_email = jellomoat@gmail.com
 description = A small package to crawl CreepyPasta and parse into structured data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://jellomoat.github.io/pasta/
 project_urls = 
@@ -22,15 +22,15 @@
 install_requires = 
 	setuptools >= 61.0
 	beautifulsoup4 >= 4.12.2
 	lxml == 4.9.3
 	requests == 2.31.0
 	pandas == 2.0.3
 	pathlib == 1.0.1
-	chromedriver-binary-auto == 0.2.6
+	chromedriver-binary-auto >= 0.3.0
 	selenium == 4.10.0
 	selenium-wire == 5.1.0
 	tqdm == 4.65.0
 
 [options.packages.find]
 where = src
```

### Comparing `creepypasta-0.0.4/src/creepypasta/pasta_listings.py` & `creepypasta-0.0.5/src/creepypasta/pasta_listings.py`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.4/src/creepypasta/pasta_stories.py` & `creepypasta-0.0.5/src/creepypasta/pasta_stories.py`

 * *Files identical despite different names*

### Comparing `creepypasta-0.0.4/src/creepypasta.egg-info/PKG-INFO` & `creepypasta-0.0.5/src/creepypasta.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: creepypasta
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small package to crawl CreepyPasta and parse into structured data.
 Home-page: https://jellomoat.github.io/pasta/
 Author: Stephanie Andrews
 Author-email: Stephanie Andrews <jellomoat@gmail.com>
 Project-URL: Homepage, https://github.com/jellomoat/pasta
 Project-URL: Bug Tracker, https://github.com/jellomoat/pasta/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # 🕯️ creepypasta
 
 Docs => https://jellomoat.github.io/pasta/
```

### Comparing `creepypasta-0.0.4/test/test-units.py` & `creepypasta-0.0.5/test/test-units.py`

 * *Files identical despite different names*

