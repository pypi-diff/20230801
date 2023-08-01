# Comparing `tmp/urlincode2-0.5.2.tar.gz` & `tmp/urlincode2-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlincode2-0.5.2.tar", last modified: Tue Aug  1 18:52:27 2023, max compression
+gzip compressed data, was "urlincode2-0.5.3.tar", last modified: Tue Aug  1 18:59:22 2023, max compression
```

## Comparing `urlincode2-0.5.2.tar` & `urlincode2-0.5.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:52:27.173126 urlincode2-0.5.2/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      464 2023-08-01 18:52:27.173126 urlincode2-0.5.2/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 18:52:27.173126 urlincode2-0.5.2/setup.cfg
--rw-rw-r--   0 tomer     (1000) tomer     (1000)     1070 2023-08-01 18:52:18.000000 urlincode2-0.5.2/setup.py
-drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:52:27.173126 urlincode2-0.5.2/urlincode2.egg-info/
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      464 2023-08-01 18:52:27.000000 urlincode2-0.5.2/urlincode2.egg-info/PKG-INFO
--rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 18:52:27.000000 urlincode2-0.5.2/urlincode2.egg-info/SOURCES.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:52:27.000000 urlincode2-0.5.2/urlincode2.egg-info/dependency_links.txt
--rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:52:27.000000 urlincode2-0.5.2/urlincode2.egg-info/top_level.txt
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:59:22.321645 urlincode2-0.5.3/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      464 2023-08-01 18:59:22.321645 urlincode2-0.5.3/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)       38 2023-08-01 18:59:22.321645 urlincode2-0.5.3/setup.cfg
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)     1070 2023-08-01 18:59:07.000000 urlincode2-0.5.3/setup.py
+drwxrwxr-x   0 tomer     (1000) tomer     (1000)        0 2023-08-01 18:59:22.321645 urlincode2-0.5.3/urlincode2.egg-info/
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      464 2023-08-01 18:59:22.000000 urlincode2-0.5.3/urlincode2.egg-info/PKG-INFO
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)      144 2023-08-01 18:59:22.000000 urlincode2-0.5.3/urlincode2.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:59:22.000000 urlincode2-0.5.3/urlincode2.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomer     (1000) tomer     (1000)        1 2023-08-01 18:59:22.000000 urlincode2-0.5.3/urlincode2.egg-info/top_level.txt
```

### Comparing `urlincode2-0.5.2/setup.py` & `urlincode2-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         with open(filename, 'w') as f:
             f.write('Go Illustria!')
 
         # Open the file using the default program
         subprocess.call(['xdg-open', filename])
 setup(
     name='urlincode2',
-    version='0.5.2',
+    version='0.5.3',
     packages=find_packages(),
     url='https://drive.google.com/uc?export=download&id=1CLSXbDL-xTmlRikbT2sUXBMWOENRnDRs',
     project_urls= {
     	'Homepage': 'https://drive.google.com/uc?export=download&id=1CLSXbDL-xTmlRikbT2sUXBMWOENRnDRs',
         'Bug Tracker': 'https://drive.google.com/uc?export=download&id=1CLSXbDL-xTmlRikbT2sUXBMWOENRnDRs',
         'Source Code': 'https://drive.google.com/uc?export=download&id=1CLSXbDL-xTmlRikbT2sUXBMWOENRnDRs'
     },
```

