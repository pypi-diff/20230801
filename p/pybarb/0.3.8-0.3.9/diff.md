# Comparing `tmp/pybarb-0.3.8.tar.gz` & `tmp/pybarb-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.8.tar", last modified: Tue Jul 25 11:07:06 2023, max compression
+gzip compressed data, was "pybarb-0.3.9.tar", last modified: Tue Aug  1 14:03:26 2023, max compression
```

## Comparing `pybarb-0.3.8.tar` & `pybarb-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 11:07:06.039852 pybarb-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-07-25 11:06:56.000000 pybarb-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/pybarb/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 11:06:56.000000 pybarb-0.3.8/pybarb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-07-25 11:06:56.000000 pybarb-0.3.8/pybarb/pybarb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:07:06.039852 pybarb-0.3.8/pybarb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 11:07:06.000000 pybarb-0.3.8/pybarb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:07:06.039852 pybarb-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-25 11:06:56.000000 pybarb-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 14:03:26.198536 pybarb-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-01 14:03:18.000000 pybarb-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:03:18.000000 pybarb-0.3.9/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33050 2023-08-01 14:03:18.000000 pybarb-0.3.9/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:03:26.198536 pybarb-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 14:03:18.000000 pybarb-0.3.9/setup.py
```

### Comparing `pybarb-0.3.8/README.md` & `pybarb-0.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 
 ## What's in this repository?
 
 ### pybarb
 
 pybarb is a python package for interacting with the Barb API. It allows you to connect to an API endpoint, query it, and convert the results into a number of formats including pandas dataframes and csv, excel and json files. It also allows you to write the results to a database using SQLAlchemy. 
 
-- [The package code](https://github.com/coppeliaMLA/barb_api/tree/pyBARB_dev/python/pybarb)
+- [The package code](https://github.com/coppeliaMLA/pybarb/tree/main/pybarb)
 - [The getting started guide](http://www.coppelia.io/pybarb/pybarb/getting_started.html)
+- [The getting started guide - jupyter notebook version](https://github.com/coppeliaMLA/pybarb/blob/main/pybarb/getting_started.ipynb)
 
 ### Jupyter notebooks
 
 Examples of how to use the Barb API for various usecases. *Note these were written before the development of pybarb. It's much easier now!*
 
 - [A broadcaster example](jupyter_notebooks/a_broadcaster_example.ipynb)
 - [A media agency example](jupyter_notebooks/a_media_agency_example.ipynb)
```

### Comparing `pybarb-0.3.8/pybarb/pybarb.py` & `pybarb-0.3.9/pybarb/pybarb.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,34 @@
         if regex_filter is not None:
 
             regex = re.compile(regex_filter)
             list_of_buyers = list(filter(regex.search, list_of_buyers))
 
         return list_of_buyers
     
+    def list_advertisers(self, regex_filter=None):
+        """
+        Lists the advertisers available in the API.
+
+            Returns:
+                list: The advertisers result set.
+        """
+
+        api_url = f"{self.api_root}advertiers"
+        api_response_data = requests.get(url=api_url, headers=self.headers)
+
+        list_of_advertisers = api_response_data.json()
+
+        if regex_filter is not None:
+
+            regex = re.compile(regex_filter)
+            list_of_buyers = list(filter(regex.search, list_of_advertisers))
+
+        return list_of_advertisers
+
     def query_asynch_endpoint(self, endpoint, parameters):
         """
         Queries the asynch endpoint.
 
             Args:
                 endpoint (str): The endpoint to query.
                 parameters (dict): The query parameters.
```

