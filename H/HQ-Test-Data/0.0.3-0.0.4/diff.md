# Comparing `tmp/HQ_Test_Data-0.0.3.tar.gz` & `tmp/HQ_Test_Data-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HQ_Test_Data-0.0.3.tar", last modified: Tue Aug  1 08:58:36 2023, max compression
+gzip compressed data, was "HQ_Test_Data-0.0.4.tar", last modified: Tue Aug  1 09:03:32 2023, max compression
```

## Comparing `HQ_Test_Data-0.0.3.tar` & `HQ_Test_Data-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 08:58:36.911250 HQ_Test_Data-0.0.3/
--rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1792 2023-08-01 08:58:36.914255 HQ_Test_Data-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      325 2023-08-01 08:42:54.000000 HQ_Test_Data-0.0.3/README.md
--rw-rw-rw-   0        0        0      373 2023-08-01 08:58:13.000000 HQ_Test_Data-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 08:58:36.976266 HQ_Test_Data-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 08:58:33.970251 HQ_Test_Data-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 08:58:35.244254 HQ_Test_Data-0.0.3/src/HQ_Test_Data/
--rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-08-01 08:57:51.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data/main.py
-drwxrwxrwx   0        0        0        0 2023-08-01 08:58:36.631251 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/
--rw-rw-rw-   0        0        0     1792 2023-08-01 08:58:33.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-08-01 08:58:33.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 08:58:33.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 08:58:33.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-01 08:58:33.000000 HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 09:03:33.158597 HQ_Test_Data-0.0.4/
+-rw-rw-rw-   0        0        0     1079 2023-08-01 08:06:48.000000 HQ_Test_Data-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1792 2023-08-01 09:03:33.162601 HQ_Test_Data-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-08-01 08:42:54.000000 HQ_Test_Data-0.0.4/README.md
+-rw-rw-rw-   0        0        0      373 2023-08-01 09:03:07.000000 HQ_Test_Data-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-01 09:03:33.230616 HQ_Test_Data-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 09:03:30.274607 HQ_Test_Data-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-08-01 09:03:31.413592 HQ_Test_Data-0.0.4/src/HQ_Test_Data/
+-rw-rw-rw-   0        0        0       33 2023-08-01 07:59:40.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data/__init__.py
+-rw-rw-rw-   0        0        0     3363 2023-08-01 09:03:00.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data/main.py
+drwxrwxrwx   0        0        0        0 2023-08-01 09:03:32.892598 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/
+-rw-rw-rw-   0        0        0     1792 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-01 09:03:29.000000 HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/top_level.txt
```

### Comparing `HQ_Test_Data-0.0.3/LICENSE` & `HQ_Test_Data-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HQ_Test_Data-0.0.3/PKG-INFO` & `HQ_Test_Data-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HQ_Test_Data
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package to fetch and print data.
 Author-email: Hossam Ibrahim <hossam.ibrahim@hlag.com>
 License: Copyright (c) [2023] [Hossam_Ibrahim]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `HQ_Test_Data-0.0.3/src/HQ_Test_Data/main.py` & `HQ_Test_Data-0.0.4/src/HQ_Test_Data/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,9 @@
         if temp_df is not None:
             df = pd.concat([df, temp_df])
     cnxn.close()
     return df
 
 def fetch_and_print():
     df = main()  # Call 'main' function and get 'df'
+    df
 #    print(df) # or just df in Jupyter notebooks
```

### Comparing `HQ_Test_Data-0.0.3/src/HQ_Test_Data.egg-info/PKG-INFO` & `HQ_Test_Data-0.0.4/src/HQ_Test_Data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HQ-Test-Data
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package to fetch and print data.
 Author-email: Hossam Ibrahim <hossam.ibrahim@hlag.com>
 License: Copyright (c) [2023] [Hossam_Ibrahim]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

