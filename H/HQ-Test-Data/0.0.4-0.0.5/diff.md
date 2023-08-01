# Comparing `tmp/HQ_Test_Data-0.0.4.tar.gz` & `tmp/HQ_Test_Data-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HQ_Test_Data-0.0.4.tar", last modified: Tue Aug  1 09:03:32 2023, max compression
+gzip compressed data, was "HQ_Test_Data-0.0.5.tar", last modified: Tue Aug  1 09:06:39 2023, max compression
```

## Comparing `HQ_Test_Data-0.0.4.tar` & `HQ_Test_Data-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:03:33.158597 HQ_Test_Data-0.0.4/
--rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1792 2023-08-01 09:03:33.162601 HQ_Test_Data-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-08-01 08:42:54.000000 HQ_Test_Data-0.0.4/README.md
--rw-rw-rw-   0        0        0      373 2023-08-01 09:03:07.000000 HQ_Test_Data-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 09:03:33.230616 HQ_Test_Data-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 09:03:30.274607 HQ_Test_Data-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 09:03:31.413592 HQ_Test_Data-0.0.4/src/HQ_Test_Data/
--rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data/__init__.py
--rw-rw-rw-   0        0        0     3363 2023-08-01 09:03:00.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data/main.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:03:32.892598 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/
--rw-rw-rw-   0        0        0     1792 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:06:39.945309 HQ_Test_Data-0.0.5/
+-rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1792 2023-08-01 09:06:39.874313 HQ_Test_Data-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-08-01 08:42:54.000000 HQ_Test_Data-0.0.5/README.md
+-rw-rw-rw-   0        0        0      373 2023-08-01 09:06:18.000000 HQ_Test_Data-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:06:39.949313 HQ_Test_Data-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 09:06:37.033310 HQ_Test_Data-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 09:06:38.213311 HQ_Test_Data-0.0.5/src/HQ_Test_Data/
+-rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data/__init__.py
+-rw-rw-rw-   0        0        0     3370 2023-08-01 09:06:12.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:06:39.593307 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/
+-rw-rw-rw-   0        0        0     1792 2023-08-01 09:06:36.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-08-01 09:06:36.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:06:36.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 09:06:36.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 09:06:36.000000 HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/top_level.txt
```

### Comparing `HQ_Test_Data-0.0.4/LICENSE` & `HQ_Test_Data-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HQ_Test_Data-0.0.4/PKG-INFO` & `HQ_Test_Data-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HQ_Test_Data
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package to fetch and print data.
 Author-email: Hossam Ibrahim <hossam.ibrahim@hlag.com>
 License: Copyright (c) [2023] [Hossam_Ibrahim]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `HQ_Test_Data-0.0.4/src/HQ_Test_Data/main.py` & `HQ_Test_Data-0.0.5/src/HQ_Test_Data/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,9 +66,9 @@
         if temp_df is not None:
             df = pd.concat([df, temp_df])
     cnxn.close()
     return df
 
 def fetch_and_print():
     df = main()  # Call 'main' function and get 'df'
-    df
+    return df
 #    print(df) # or just df in Jupyter notebooks
```

### Comparing `HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/PKG-INFO` & `HQ_Test_Data-0.0.5/src/HQ_Test_Data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HQ-Test-Data
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python package to fetch and print data.
 Author-email: Hossam Ibrahim <hossam.ibrahim@hlag.com>
 License: Copyright (c) [2023] [Hossam_Ibrahim]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

