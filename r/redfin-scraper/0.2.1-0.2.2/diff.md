# Comparing `tmp/redfin-scraper-0.2.1.tar.gz` & `tmp/redfin-scraper-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfin-scraper-0.2.1.tar", last modified: Wed May 24 17:52:42 2023, max compression
+gzip compressed data, was "redfin-scraper-0.2.2.tar", last modified: Tue Aug  1 20:43:21 2023, max compression
```

## Comparing `redfin-scraper-0.2.1.tar` & `redfin-scraper-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.198446 redfin-scraper-0.2.1/
--rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4232 2023-05-24 17:52:42.197442 redfin-scraper-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2366 2023-05-20 17:17:34.000000 redfin-scraper-0.2.1/README.md
--rw-rw-rw-   0        0        0      904 2023-05-24 17:51:29.000000 redfin-scraper-0.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.162021 redfin-scraper-0.2.1/redfin_scraper/
--rw-rw-rw-   0        0        0      120 2023-05-24 17:51:32.000000 redfin-scraper-0.2.1/redfin_scraper/__init__.py
--rw-rw-rw-   0        0        0      381 2023-05-20 17:01:49.000000 redfin-scraper-0.2.1/redfin_scraper/config.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.190448 redfin-scraper-0.2.1/redfin_scraper/core/
--rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.2.1/redfin_scraper/core/__init__.py
--rw-rw-rw-   0        0        0    12424 2023-05-24 17:51:55.000000 redfin-scraper-0.2.1/redfin_scraper/core/redfin_scraper.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.195452 redfin-scraper-0.2.1/redfin_scraper/resources/
--rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.2.1/redfin_scraper/resources/__init__.py
--rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.2.1/redfin_scraper/resources/json_tools.py
--rw-rw-rw-   0        0        0     2445 2023-05-24 17:51:24.000000 redfin-scraper-0.2.1/redfin_scraper/resources/logging.py
-drwxrwxrwx   0        0        0        0 2023-05-24 17:52:42.187450 redfin-scraper-0.2.1/redfin_scraper.egg-info/
--rw-rw-rw-   0        0        0     4232 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-24 17:52:42.000000 redfin-scraper-0.2.1/redfin_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 17:52:42.198446 redfin-scraper-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-01 20:43:21.511551 redfin-scraper-0.2.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-18 00:15:21.000000 redfin-scraper-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4232 2023-08-01 20:43:21.510552 redfin-scraper-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2366 2023-05-20 17:17:34.000000 redfin-scraper-0.2.2/README.md
+-rw-rw-rw-   0        0        0      904 2023-08-01 20:40:45.000000 redfin-scraper-0.2.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-08-01 20:43:21.462376 redfin-scraper-0.2.2/redfin_scraper/
+-rw-rw-rw-   0        0        0      120 2023-08-01 20:39:59.000000 redfin-scraper-0.2.2/redfin_scraper/__init__.py
+-rw-rw-rw-   0        0        0      381 2023-05-20 17:01:49.000000 redfin-scraper-0.2.2/redfin_scraper/config.py
+drwxrwxrwx   0        0        0        0 2023-08-01 20:43:21.502554 redfin-scraper-0.2.2/redfin_scraper/core/
+-rw-rw-rw-   0        0        0        0 2023-03-11 03:00:34.000000 redfin-scraper-0.2.2/redfin_scraper/core/__init__.py
+-rw-rw-rw-   0        0        0    12472 2023-08-01 20:39:54.000000 redfin-scraper-0.2.2/redfin_scraper/core/redfin_scraper.py
+drwxrwxrwx   0        0        0        0 2023-08-01 20:43:21.508557 redfin-scraper-0.2.2/redfin_scraper/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-25 20:03:01.000000 redfin-scraper-0.2.2/redfin_scraper/resources/__init__.py
+-rw-rw-rw-   0        0        0     1116 2023-03-11 03:00:17.000000 redfin-scraper-0.2.2/redfin_scraper/resources/json_tools.py
+-rw-rw-rw-   0        0        0     2445 2023-05-24 17:51:24.000000 redfin-scraper-0.2.2/redfin_scraper/resources/logging.py
+drwxrwxrwx   0        0        0        0 2023-08-01 20:43:21.497554 redfin-scraper-0.2.2/redfin_scraper.egg-info/
+-rw-rw-rw-   0        0        0     4232 2023-08-01 20:43:21.000000 redfin-scraper-0.2.2/redfin_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-08-01 20:43:21.000000 redfin-scraper-0.2.2/redfin_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 20:43:21.000000 redfin-scraper-0.2.2/redfin_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-08-01 20:43:21.000000 redfin-scraper-0.2.2/redfin_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-01 20:43:21.000000 redfin-scraper-0.2.2/redfin_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 20:43:21.511551 redfin-scraper-0.2.2/setup.cfg
```

### Comparing `redfin-scraper-0.2.1/LICENSE.txt` & `redfin-scraper-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.1/PKG-INFO` & `redfin-scraper-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `redfin-scraper-0.2.1/README.md` & `redfin-scraper-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.1/pyproject.toml` & `redfin-scraper-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "redfin-scraper"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python library used to scrape data from Redfin.com using the unofficial Stringray API."
 readme = "README.md"
 authors = [{ name = "Ryan Sherby", email = "ryan.m.sherby@gmail.com" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `redfin-scraper-0.2.1/redfin_scraper/core/redfin_scraper.py` & `redfin-scraper-0.2.2/redfin_scraper/core/redfin_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,25 +154,27 @@
     
         
         for city_state in city_states:
             zip_list += self._select_zip_codes(city_state,lat_tuner,lon_tuner)
 
         zip_list=list(set(zip_list)) #Eliminate duplicates
 
+        df_list=[]
+
         if self._mp:
             df_list=self._multiprocess_func(self._core,zip_list)
         else:
             df_list=self._core(zip_list)
 
         
         self._data_id_ticker+=1
         self.data_id=f"D{self._data_id_ticker:03d}"
 
 
-        if len(df_list)==0:
+        if (len(df_list)==0 or df_list is None):
             self.data[self.data_id]=None
             return None
 
 
         concat_df=pd.concat(df_list,axis=0,ignore_index=True)
         converted_df=concat_df.drop('ZIP OR POSTAL CODE',axis=1).apply(lambda row:pd.to_numeric(row,errors='ignore'))
         converted_df.insert(6,'ZIP OR POSTAL CODE',concat_df['ZIP OR POSTAL CODE'].astype(str))
@@ -197,15 +199,15 @@
 
         df_list=self._set_dataframe(api_responses)
 
         return df_list
 
 
 
-    def _multiprocess_func(self,func,list_obj):
+    def _multiprocess_func(self,func,list_obj:list):
         
         main_list=[]
 
         list_of_lists=list(self._split(list_obj,multiprocessing.cpu_count()))
         # Separate list into cpu_count equal pieces
 
         with concurrent.futures.ProcessPoolExecutor() as exe:
```

### Comparing `redfin-scraper-0.2.1/redfin_scraper/resources/json_tools.py` & `redfin-scraper-0.2.2/redfin_scraper/resources/json_tools.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.1/redfin_scraper/resources/logging.py` & `redfin-scraper-0.2.2/redfin_scraper/resources/logging.py`

 * *Files identical despite different names*

### Comparing `redfin-scraper-0.2.1/redfin_scraper.egg-info/PKG-INFO` & `redfin-scraper-0.2.2/redfin_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfin-scraper
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python library used to scrape data from Redfin.com using the unofficial Stringray API.
 Author-email: Ryan Sherby <ryan.m.sherby@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ryan Sherby
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

