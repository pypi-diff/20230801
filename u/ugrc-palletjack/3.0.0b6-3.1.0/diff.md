# Comparing `tmp/ugrc-palletjack-3.0.0b6.tar.gz` & `tmp/ugrc-palletjack-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugrc-palletjack-3.0.0b6.tar", last modified: Tue Feb 28 23:41:56 2023, max compression
+gzip compressed data, was "ugrc-palletjack-3.1.0.tar", last modified: Mon Jul 31 23:24:39 2023, max compression
```

## Comparing `ugrc-palletjack-3.0.0b6.tar` & `ugrc-palletjack-3.1.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:41:56.453523 ugrc-palletjack-3.0.0b6/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-02-28 23:41:56.453523 ugrc-palletjack-3.0.0b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-02-28 23:41:56.457523 ugrc-palletjack-3.0.0b6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:41:56.453523 ugrc-palletjack-3.0.0b6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:41:56.453523 ugrc-palletjack-3.0.0b6/src/palletjack/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)    44653 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    37139 2023-02-28 23:41:52.000000 ugrc-palletjack-3.0.0b6/src/palletjack/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-28 23:41:53.000000 ugrc-palletjack-3.0.0b6/src/palletjack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 23:41:56.453523 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 23:41:56.000000 ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:24:39.745536 ugrc-palletjack-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-31 23:24:39.745536 ugrc-palletjack-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-31 23:24:39.745536 ugrc-palletjack-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:24:39.741536 ugrc-palletjack-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:24:39.745536 ugrc-palletjack-3.1.0/src/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24687 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39616 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38035 2023-07-31 23:24:35.000000 ugrc-palletjack-3.1.0/src/palletjack/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-31 23:24:36.000000 ugrc-palletjack-3.1.0/src/palletjack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 23:24:39.745536 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 23:24:39.000000 ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/zip-safe
```

### Comparing `ugrc-palletjack-3.0.0b6/LICENSE` & `ugrc-palletjack-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-3.0.0b6/PKG-INFO` & `ugrc-palletjack-3.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugrc-palletjack
-Version: 3.0.0b6
+Version: 3.1.0
 Summary: Updating AGOL feature services with data from SFTP shares.
 Home-page: https://github.com/agrc/palletjack
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 License: UNKNOWN
 Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
 Keywords: gis
@@ -18,58 +18,66 @@
 License-File: LICENSE
 
 # agrc/palletjack
 
 ![Build Status](https://github.com/agrc/palletjack/workflows/Build%20and%20Test/badge.svg)
 [![codecov](https://codecov.io/gh/agrc/palletjack/branch/main/graph/badge.svg)](https://codecov.io/gh/agrc/palletjack)
 
-A library of classes for automatically updating AGOL feature services with data from external sources. Client apps (often called 'skids') can reuse these classes for common use cases. These classes handle different parts of the Extract and Load steps in the ETL process.
+A library of classes and methods for automatically updating AGOL feature services with data from several different types of external sources. Client apps (sometimes called 'skids') can reuse these classes for common use cases. The code modules are oriented around each step in the extract, transform, and load process.
 
-`palletjack` works with pandas DataFrames (either regular for tabular data or Esri's spatially-enabled dataframes for spatial data). Most methods either return a dataframe or use a dataframe for their source data.
+`palletjack` works with pandas DataFrames (either regular for tabular data or Esri's spatially-enabled dataframes for spatial data). The extract and transform methods return dataframes and the load methods consume dataframes as their source data.
 
-See `docs/api.md` for documentation on the available classes and methods, logging, and errors.
-
-See `docs/examples.py` for (bare-bones) example code implementing the various classes/methods. You can also search our GitHub organization for "skid" repositories that use palletjack.
+The [documentation](https://agrc.github.io/palletjack/palletjack) includes a user guide along with an API description of the available classes and methods.
 
 Pallet jack: [forklift's](https://www.github.com/agrc/forklift) little brother.
 
+## Dependencies
+
+`palletjack` relies on the dependencies listed in `setup.py`. These are all available on PyPI and can be installed in most environments, including Google Cloud Functions.
+
+The `arcgis` library does all the heavy lifting for spatial data. If the `arcpy` library is not available (such as in a cloud function), it relies on `shapely` for its geometry engine.
+
 ## Installation
 
 1. Activate your application's environment
 1. `pip install ugrc-palletjack`
 
-## Dependencies
-
-`palletjack` relies on `setup.py` to install `pandas`, `numpy`, `pysftp`, and `arcgis`. `FeatureServiceInlineUpdater.update_existing_features_in_feature_service_with_arcpy()` also relies on having arcpy installed through either ArcGIS Pro or ArcGIS Enterprise.
+## Quick start
 
-## Usage
-
-1. `import palletjack`
-1. Instantiate one or more of the classes as needed.
-1. Call the methods on your instantiated objects to perform the specific action desired.
+1. Import the desired modules
+1. Use a class in `extract` to load a dataframe from an external source
+1. Transform your dataframe as desired with helper methods from `transform`
+1. Use the dataframe to update a hosted feature service using the methods in `load`
 
    ```python
-   loader = palletjack.SFTPLoader(secrets, download_dir)
-   files_downloaded = loader.download_sftp_files(sftp_folder=secrets.SFTP_FOLDER)
-   dataframe = loader.read_csv_into_dataframe('data.csv', secrets.DATA_TYPES)
-
-   updater = FeatureServiceInlineUpdater(gis, dataframe, secrets.KEY_COLUMN)
-   rows_updated = updater.update_existing_features_in_hosted_feature_layer(
-      secrets.FEATURE_LAYER_ITEMID, list(secrets.DATA_TYPES.keys())
-    )
+   from palletjack import extract, transform, load
+
+   #: Load the data from a Google Sheet
+   gsheet_extractor = extract.GSheetLoader(path_to_service_account_json)
+   sheet_df = gsheet_extractor.load_specific_worksheet_into_dataframe(sheet_id, 'title of desired sheet', by_title=True)
+
+   #: Convert the data to points using lat/long fields, clean for uploading
+   spatial_df = pd.DataFrame.spatial.from_xy(input_df, x_column='longitude', y_column='latitude')
+   renamed_df = transform.DataCleaning.rename_dataframe_columns_for_agol(spatial_df)
+   cleaned_df = transform.DataCleaning.switch_to_nullable_int(renamed_df, ['an_int_field_with_null_values'])
+
+   #: Truncate the existing feature service data and load the new data
+   gis = arcgis.gis.GIS('my_agol_org_url', 'username', 'super-duper-secure-password')
+   updates = palletjack.load.FeatureServiceUpdater.truncate_and_load_features(
+      gis, 'feature_service_item_id', cleaned_df, r'c:\directory\to\save\truncated\data\in\case\of\error'
+   )
    ```
 
 ## Development
 
-1. Create a conda environment with arcpy, arcgis
-   - `conda create -n palletjack`
+1. Create a conda environment with Python 3.9
+   - `conda create -n palletjack python=3.9`
    - `activate palletjack`
-   - `conda install arcgis arcpy -c esri`
 1. Clone the repo
-1. Install in dev mode
+1. Install in dev mode with development dependencies
    - `pip install -e .[tests]`
 
 ### Troubleshooting Weird Append Errors
 
 If a `FeatureLayer.append()` call (within a load.FeatureServiceUpdater method) fails with an "Unknown Error: 500" error or something like that, you can query the results to get more info. The debug log will include the HTTP GET call, something like the following:
 `https://services1.arcgis.com:443 POST /<unique string>/arcgis/rest/services/<feature layer name>/FeatureServer/<layer id>/append/jobs/<job guid>?f=json token=<crazy long token string>`
```

### Comparing `ugrc-palletjack-3.0.0b6/README.md` & `ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,91 @@
+Metadata-Version: 2.1
+Name: ugrc-palletjack
+Version: 3.1.0
+Summary: Updating AGOL feature services with data from SFTP shares.
+Home-page: https://github.com/agrc/palletjack
+Author: Jake Adams, UGRC
+Author-email: jdadams@utah.gov
+License: UNKNOWN
+Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
+Keywords: gis
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Utilities
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+License-File: LICENSE
+
 # agrc/palletjack
 
 ![Build Status](https://github.com/agrc/palletjack/workflows/Build%20and%20Test/badge.svg)
 [![codecov](https://codecov.io/gh/agrc/palletjack/branch/main/graph/badge.svg)](https://codecov.io/gh/agrc/palletjack)
 
-A library of classes for automatically updating AGOL feature services with data from external sources. Client apps (often called 'skids') can reuse these classes for common use cases. These classes handle different parts of the Extract and Load steps in the ETL process.
-
-`palletjack` works with pandas DataFrames (either regular for tabular data or Esri's spatially-enabled dataframes for spatial data). Most methods either return a dataframe or use a dataframe for their source data.
+A library of classes and methods for automatically updating AGOL feature services with data from several different types of external sources. Client apps (sometimes called 'skids') can reuse these classes for common use cases. The code modules are oriented around each step in the extract, transform, and load process.
 
-See `docs/api.md` for documentation on the available classes and methods, logging, and errors.
+`palletjack` works with pandas DataFrames (either regular for tabular data or Esri's spatially-enabled dataframes for spatial data). The extract and transform methods return dataframes and the load methods consume dataframes as their source data.
 
-See `docs/examples.py` for (bare-bones) example code implementing the various classes/methods. You can also search our GitHub organization for "skid" repositories that use palletjack.
+The [documentation](https://agrc.github.io/palletjack/palletjack) includes a user guide along with an API description of the available classes and methods.
 
 Pallet jack: [forklift's](https://www.github.com/agrc/forklift) little brother.
 
+## Dependencies
+
+`palletjack` relies on the dependencies listed in `setup.py`. These are all available on PyPI and can be installed in most environments, including Google Cloud Functions.
+
+The `arcgis` library does all the heavy lifting for spatial data. If the `arcpy` library is not available (such as in a cloud function), it relies on `shapely` for its geometry engine.
+
 ## Installation
 
 1. Activate your application's environment
 1. `pip install ugrc-palletjack`
 
-## Dependencies
-
-`palletjack` relies on `setup.py` to install `pandas`, `numpy`, `pysftp`, and `arcgis`. `FeatureServiceInlineUpdater.update_existing_features_in_feature_service_with_arcpy()` also relies on having arcpy installed through either ArcGIS Pro or ArcGIS Enterprise.
-
-## Usage
+## Quick start
 
-1. `import palletjack`
-1. Instantiate one or more of the classes as needed.
-1. Call the methods on your instantiated objects to perform the specific action desired.
+1. Import the desired modules
+1. Use a class in `extract` to load a dataframe from an external source
+1. Transform your dataframe as desired with helper methods from `transform`
+1. Use the dataframe to update a hosted feature service using the methods in `load`
 
    ```python
-   loader = palletjack.SFTPLoader(secrets, download_dir)
-   files_downloaded = loader.download_sftp_files(sftp_folder=secrets.SFTP_FOLDER)
-   dataframe = loader.read_csv_into_dataframe('data.csv', secrets.DATA_TYPES)
-
-   updater = FeatureServiceInlineUpdater(gis, dataframe, secrets.KEY_COLUMN)
-   rows_updated = updater.update_existing_features_in_hosted_feature_layer(
-      secrets.FEATURE_LAYER_ITEMID, list(secrets.DATA_TYPES.keys())
-    )
+   from palletjack import extract, transform, load
+
+   #: Load the data from a Google Sheet
+   gsheet_extractor = extract.GSheetLoader(path_to_service_account_json)
+   sheet_df = gsheet_extractor.load_specific_worksheet_into_dataframe(sheet_id, 'title of desired sheet', by_title=True)
+
+   #: Convert the data to points using lat/long fields, clean for uploading
+   spatial_df = pd.DataFrame.spatial.from_xy(input_df, x_column='longitude', y_column='latitude')
+   renamed_df = transform.DataCleaning.rename_dataframe_columns_for_agol(spatial_df)
+   cleaned_df = transform.DataCleaning.switch_to_nullable_int(renamed_df, ['an_int_field_with_null_values'])
+
+   #: Truncate the existing feature service data and load the new data
+   gis = arcgis.gis.GIS('my_agol_org_url', 'username', 'super-duper-secure-password')
+   updates = palletjack.load.FeatureServiceUpdater.truncate_and_load_features(
+      gis, 'feature_service_item_id', cleaned_df, r'c:\directory\to\save\truncated\data\in\case\of\error'
+   )
    ```
 
 ## Development
 
-1. Create a conda environment with arcpy, arcgis
-   - `conda create -n palletjack`
+1. Create a conda environment with Python 3.9
+   - `conda create -n palletjack python=3.9`
    - `activate palletjack`
-   - `conda install arcgis arcpy -c esri`
 1. Clone the repo
-1. Install in dev mode
+1. Install in dev mode with development dependencies
    - `pip install -e .[tests]`
 
 ### Troubleshooting Weird Append Errors
 
 If a `FeatureLayer.append()` call (within a load.FeatureServiceUpdater method) fails with an "Unknown Error: 500" error or something like that, you can query the results to get more info. The debug log will include the HTTP GET call, something like the following:
 `https://services1.arcgis.com:443 POST /<unique string>/arcgis/rest/services/<feature layer name>/FeatureServer/<layer id>/append/jobs/<job guid>?f=json token=<crazy long token string>`
 
 You can use this and a token from an AGOL tab to build a new job status url. To get the token, log into AGOL in a browser and open a private hosted feature layer item. Click the layer, and then open the developer console. With the Network tab of the console open, click on the "View" link for the service URL. You should see a document in the list whose name includes "?token=<really long token string>". Copy the name and then copy out the token string.
 
 Now that you've got the token string, you can build the status query:
 `https://services1.arcgis.com/<unique string>/arcgis/rest/services/<feature layer name>/FeatureServer/<layer id>/append/jobs/<job guid>?f=json&<token from agol>`
 
 Calling this URL in a browser should return a message that will hopefully give you more info as to why it failed.
+
+
```

### Comparing `ugrc-palletjack-3.0.0b6/setup.cfg` & `ugrc-palletjack-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-3.0.0b6/setup.py` & `ugrc-palletjack-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-3.0.0b6/src/palletjack/extract.py` & `ugrc-palletjack-3.1.0/src/palletjack/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-"""Classes for loading data from various sources into a pandas dataframe
+"""Extract tabular/spatial data from various sources into a pandas dataframe.
+
+Each different type of source has its own class. Each class may have multiple methods available for different loading
+operations or techniques.
 """
 
 import logging
 import mimetypes
 import os
 import re
 from io import BytesIO
@@ -12,23 +15,34 @@
 import geopandas as gpd
 import pandas as pd
 import pysftp
 import requests
 import sqlalchemy
 from googleapiclient.http import MediaIoBaseDownload
 
-from . import utils
+from palletjack import utils
 
 logger = logging.getLogger(__name__)
 
 
 class GSheetLoader:
-    """Loads data from a Google Sheets spreadsheet into a pandas data frame"""
+    """Loads data from a Google Sheets spreadsheet into a pandas data frame
+
+    Requires either the path to a service account .json file that has access to the sheet in question or a
+    `google.auth.credentials.Credentials` object. Calling `google.auth.default()` in a Google Cloud Function will give
+    you a tuple of a `Credentials` object and the project id. You can use this `Credentials` object to authorize
+    pygsheets as the same account the Cloud Function is running under.
+    """
 
     def __init__(self, credentials):
+        """
+        Args:
+            credentials (str or google.auth.credentials.Credentials): Path to the service file OR credentials object
+                obtained from google.auth.default() within a cloud function.
+        """
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         self.gsheets_client = utils.authorize_pygsheets(credentials)
 
     def load_specific_worksheet_into_dataframe(self, sheet_id, worksheet, by_title=False):
         """Load a single worksheet from a spreadsheet into a dataframe by worksheet index or title
 
         Args:
@@ -72,37 +86,46 @@
         identifying the source worksheet.
 
         Args:
             worksheet_dfs (dict): {'worksheet_name': Worksheet as a dataframe}.
 
         Raises:
             ValueError: If all the worksheets in worksheets_dfs don't have the same column index, it raises an error
-            and bombs out.
+                and bombs out.
 
         Returns:
             pd.DataFrame: A single combined data frame with a new 'worksheet' column identifying the worksheet the row
-            came from. The row index is the original row numbers and is probably not unique.
+                came from. The row index is the original row numbers and is probably not unique.
         """
 
         dataframes = list(worksheet_dfs.values())
 
         #: Make sure all the dataframes have the same columns
         if not all([set(dataframes[0].columns) == set(df.columns) for df in dataframes]):
             raise ValueError('Columns do not match; cannot create multi-index dataframe')
 
         self._class_logger.debug('Concatting worksheet dataframes %s into a single dataframe', worksheet_dfs.keys())
         concatted_df = pd.concat(dataframes, keys=worksheet_dfs.keys(), names=['worksheet', 'row'])
         return concatted_df.reset_index(level='worksheet')
 
 
 class GoogleDriveDownloader:
-    """Downloads images from publicly-shared Google Drive links (https://drive.google.com/file/d/big_long_id/etc)
+    """Provides methods to download any non-html file (ie, Content-Type != text/html) Google Drive file from it's
+    sharing link (of the form `https://drive.google.com/file/d/big_long_id/etc`). The files may be publicly shared or shared with a service account.
+
+    This class has two similar sets of methods. The `*_using_api` methods authenticate to the Google API using either a
+    service account file or a `google.auth.credentials.Credentials` object and downloads using the API. The
+    `*_using_api` methods are the most robust and should be used whenever possible.
     """
 
     def __init__(self, out_dir):
+        """
+        Args:
+            out_dir (str or Path): Directory to save downloaded files. Can be reassigned later to change the directory.
+        """
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         self._class_logger.debug('Initializing GoogleDriveDownloader')
         self._class_logger.debug('Output directory: %s', out_dir)
         self.out_dir = Path(out_dir)
         regex_pattern = '(\/|=)([-\w]{25,})'  # pylint:disable=anomalous-backslash-in-string
         self._class_logger.debug('Regex pattern: %s', regex_pattern)
         self.regex = re.compile(regex_pattern)
@@ -124,19 +147,19 @@
 
     def _get_http_response(self, file_id, base_url='https://docs.google.com/uc?export=download'):
         """Performs the HTTP GET request and checks the response
 
         Args:
             file_id (str): The Google-created unique id for the file
             base_url (str, optional): The base URL for the GET call. Defaults to 'https://docs.google.com/uc?
-                                      export=download'.
+                export=download'.
 
         Raises:
             RuntimeError: If Content-Type is text/html, we can't get the file, either because it doesn't exist or isn't
-                          publicly shared.
+                publicly shared.
 
         Returns:
             request.response: The requests response object.
         """
 
         response = requests.get(base_url, params={'id': file_id}, stream=True)
 
@@ -191,14 +214,21 @@
             except IndexError as err:
                 raise IndexError(f'Regex could not extract the file id from sharing link {sharing_link}') from err
         raise RuntimeError(f'Regex could not match sharing link {sharing_link}')
 
     def download_file_from_google_drive(self, sharing_link, join_id, pause=0.):
         """Download a publicly-shared image from Google Drive using it's sharing link
 
+        Uses an anonymous HTTP request with support for sleeping between downloads to try to get around Google's
+        blocking (I haven't found a good value yet).
+
+        Logs a warning if the URL doesn't match the proper pattern or it can't extract the unique id from the sharing
+        URL. Will also log a warning if the header's Content-Type is text/html, which usually indicates the HTTP
+        response was an error message instead of the file.
+
         Args:
             sharing_link (str): The publicly-shared link to the image.
             join_id (str or int): The unique key for the row (used for reporting)
             pause (flt, optional): Pause the specified number of seconds before downloading. Defaults to 0.
 
         Returns:
             Path: Path of downloaded file or None if download fails/is not possible
@@ -263,15 +293,21 @@
         downloader = MediaIoBaseDownload(in_memory, request)
         done = False
         while not done:
             _, done = downloader.next_chunk()
         out_file_path.write_bytes(in_memory.getbuffer())
 
     def download_file_from_google_drive_using_api(self, gsheets_client, sharing_link, join_id):
-        """Download a file from Google Drive using an authenticated client and the Google API via pygsheets
+        """ Download a file using the Google API via pygsheets authentication.
+
+        Requires a pygsheets client object that handles authentication.
+
+        Logs a warning if the URL doesn't match the proper pattern or it can't extract the unique id from the sharing
+        URL. Will also log a warning if the header's Content-Type is text/html, which usually indicates the HTTP
+        response was an error message instead of the file.
 
         Args:
             gsheets_client (pygsheets.Client): The authenticated client object from pygsheets
             sharing_link (str): Sharing link to the file to be downloaded
             join_id (str or int): Unique key for the row (used for reporting)
 
         Returns:
@@ -299,16 +335,16 @@
     def download_attachments_from_dataframe(self, dataframe, sharing_link_column, join_id_column, output_path_column):
         """Download the attachments linked in a dataframe column, creating a new column with the resulting path
 
         Args:
             dataframe (pd.DataFrame): Input dataframe with required columns
             sharing_link_column (str): Column holding the Google sharing link
             join_id_column (str): Column holding a unique key (for reporting purposes)
-            output_path_column (str): Column for the resulting path; will be added if it doesn't existing in the
-            dataframe
+            output_path_column (str): Column for the resulting path; will be added if it doesn't exist in the
+                dataframe
 
         Returns:
             pd.DataFrame: Input dataframe with output path info
         """
 
         dataframe[output_path_column] = dataframe.apply(
             lambda x: self.download_file_from_google_drive(x[sharing_link_column], x[join_id_column], pause=5), axis=1
@@ -324,15 +360,15 @@
         Args:
             credentials (str or google.auth.credentials.Credentials): Path to the service file OR credentials object
                 obtained from google.auth.default() within a cloud function.
             dataframe (pd.DataFrame): Input dataframe with required columns
             sharing_link_column (str): Column holding the Google sharing link
             join_id_column (str): Column holding a unique key (for reporting purposes)
             output_path_column (str): Column for the resulting path; will be added if it doesn't existing in the
-            dataframe
+                dataframe
 
         Returns:
             pd.DataFrame: Input dataframe with output path info
         """
 
         client = utils.authorize_pygsheets(credentials)
 
@@ -344,14 +380,23 @@
 
 
 class SFTPLoader:
     """Loads data from an SFTP share into a pandas DataFrame
     """
 
     def __init__(self, host, username, password, knownhosts_file, download_dir):
+        """
+        Args:
+            host (str): The SFTP host to connect to
+            username (str): SFTP username
+            password (str): SFTP password
+            knownhosts_file (str): Path to a known_hosts file for pysftp.CnOpts. Can be generated via ssh-keyscan.
+            download_dir (str or Path): Directory to save downloaded files
+        """
+
         self.host = host
         self.username = username
         self.password = password
         self.knownhosts_file = knownhosts_file
         self.download_dir = download_dir
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
@@ -434,14 +479,23 @@
         return dataframe
 
 
 class PostgresLoader:
     """Loads data from a Postgres/PostGIS database into a pandas data frame"""
 
     def __init__(self, host, database, username, password, port=5432):
+        """
+        Args:
+            host (str): Postgres server host name
+            database (str): Database to connect to
+            username (str): Database user
+            password (str): Database password
+            port (int, optional): Database port. Defaults to 5432.
+        """
+
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         if os.environ.get('FUNCTION_TARGET') is not None:  #: this is an env var specific to cloud functions
             self._class_logger.info('running in GCF, using unix socket')
             self.engine = sqlalchemy.create_engine(
                 sqlalchemy.engine.url.URL.create(
                     drivername='postgresql+pg8000',
                     username=username,
@@ -461,19 +515,21 @@
                     host=host,
                     port=port,
                 )
             )
 
     def read_table_into_dataframe(self, table_name, index_column, crs, spatial_column):
         """Read a table into a dataframe
+
         Args:
             table_name (str): Name of table or view to read in the following format: schema.table_name
             index_column (str): Name of column to use as the dataframe's index
             crs (str): Coordinate reference system of the table's geometry column
             spatial_column (str): Name of the table's geometry or geography column
+
         Returns:
             pd.DataFrame.spatial: Table as a spatially enabled dataframe
         """
 
         self._class_logger.info('Reading `%s` into dataframe', table_name)
 
         dataframe = gpd.read_postgis(
```

### Comparing `ugrc-palletjack-3.0.0b6/src/palletjack/load.py` & `ugrc-palletjack-3.1.0/src/palletjack/load.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Classes for loading data from spatially-enabled pandas DataFrames into AGOL Feature Services
+"""Modify existing ArcGIS Online content (mostly hosted feature services). Contains classes for updating hosted feature
+service data, modifying the attachments on a hosted feature service, or modifying map symbology.
 """
 
 import json
 import logging
 import sys
 import warnings
 from datetime import datetime
@@ -17,39 +18,47 @@
 
 logger = logging.getLogger(__name__)
 
 
 class FeatureServiceUpdater:
     """Update an AGOL Feature Service with data from a pandas DataFrame.
 
-    Contains four class methods that should be called directly without need to instantiate an instance: add_features,
+    Contains four class methods that can be called directly without needing to instantiate an object: add_features,
     remove_features, update_features, and truncate_and_load_features.
+
+    It is the client's responsibility to separate out the new data into these different steps. If the extract/transform
+    stages result in seperate groups of records that need to be added, deleted, and updated, the client must call the
+    three different methods with dataframes containing only the respective records for each operation.
+
+    Because the update process uploads the data as geojson, all input geometries must be in WGS84 (wkid 4326). Input
+    dataframes can be projected using dataframe.spatial.project(4326). ArcGIS Online will then project the uploaded
+    data to match the hosted feature service's projection.
     """
 
     @classmethod
     def add_features(cls, gis, feature_service_itemid, dataframe, layer_index=0):
         """Adds new features to existing hosted feature layer from new dataframe.
 
-        The new dataframe must have a 'SHAPE' column containing geometries of the same type as the live data. New
-        OBJECTIDs will be automatically generated.
+        The new dataframe must have a 'SHAPE' column containing geometries of the same type as the live data. The
+        dataframe must have a WGS84 (wkid 4326) projection. New OBJECTIDs will be automatically generated.
 
         The new dataframe's columns and data must match the existing data's fields (with the exception of generated
         fields like shape area and length) in name, type, and allowable length. Live fields that are not nullable and
         don't have a default value must have a value in the new data; missing data in these fields will raise an error.
 
         Args:
             gis (arcgis.gis.GIS): GIS item for AGOL org
             features_service_item_id (str): itemid for service to update
             dataframe (pd.DataFrame.spatial): Spatially enabled dataframe of data to be added
             layer_index (int): Index of layer within service to update. Defaults to 0.
 
         Raises:
             ValueError: If the new field and existing fields don't match, the SHAPE field is missing or has an
-                        incompatible type, the new data contains null fields, the new data exceeds the existing field
-                        lengths, or a specified field is missing from either new or live data.
+                incompatible type, the new data contains null fields, the new data exceeds the existing field
+                lengths, or a specified field is missing from either new or live data.
 
         Returns:
             int: Number of features added
         """
         updater = cls(gis, feature_service_itemid, dataframe, fields=list(dataframe.columns), layer_index=layer_index)
         return updater._add_new_data_to_hosted_feature_layer()
 
@@ -80,35 +89,39 @@
         updater = cls(gis, feature_service_itemid, layer_index=layer_index)
         return updater._delete_data_from_hosted_feature_layer(delete_oids)
 
     @classmethod
     def update_features(cls, gis, feature_service_itemid, dataframe, layer_index=0, update_geometry=True):
         """Updates existing features within a hosted feature layer using OBJECTID as the join field.
 
-        The new data can have either attributes and geometries or only attributes based on the update_geometry flag. A
-        combination of updates from a source with both attributes & geometries and a source with attributes-only must
-        be done with two separate calls. The geometries must be provided in a SHAPE column and be the same type as the
-        live data.
-
         The new dataframe's columns and data must match the existing data's fields (with the exception of generated
         fields like shape area and length) in name, type, and allowable length. Live fields that are not nullable and
         don't have a default value must have a value in the new data; missing data in these fields will raise an error.
 
+        Uses the OBJECTID field to determine which features should be updated by the underlying FeatureLayer.append()
+        method. The most robust way to do this is to load the live data as a dataframe, subset it down to the desired
+        rows, make your edits based on a separate join id, and then pass that dataframe to this method.
+
+        The new data can have either attributes and geometries or only attributes based on the update_geometry flag. A
+        combination of updates from a source with both attributes & geometries and a source with attributes-only must
+        be done with two separate calls. The geometries must be provided in a SHAPE column, be the same type as the
+        live data, and have a WGS84 (wkid 4326) projection.
+
         Args:
             gis (arcgis.gis.GIS): GIS item for AGOL org
             features_service_item_id (str): itemid for service to update
             dataframe (pd.DataFrame.spatial): Spatially enabled dataframe of data to be updated
             layer_index (int): Index of layer within service to update. Defaults to 0.
             update_geometry (bool): Whether to update attributes and geometry (True) or just attributes (False).
-            Defaults to False.
+                Defaults to False.
 
         Raises:
             ValueError: If the new field and existing fields don't match, the SHAPE field is missing or has an
-                        incompatible type, the new data contains null fields, the new data exceeds the existing field
-                        lengths, or a specified field is missing from either new or live data.
+                incompatible type, the new data contains null fields, the new data exceeds the existing field
+                lengths, or a specified field is missing from either new or live data.
 
         Returns:
             int: Number of features updated
         """
 
         updater = cls(
             gis,
@@ -123,16 +136,16 @@
     def truncate_and_load_features(cls, gis, feature_service_itemid, dataframe, failsafe_dir='', layer_index=0):
         """Overwrite a hosted feature layer by truncating and loading the new data
 
         When the existing dataset is truncated, a copy is kept in memory as a spatially-enabled dataframe. If the new
         data fail to load, this copy is reloaded. If the reload fails, the copy is written to failsafe_dir with the
         filename {todays_date}.json (2022-12-31.json).
 
-        The new dataframe must have a 'SHAPE' column containing geometries of the same type as the live data. New
-        OBJECTIDs will be automatically generated.
+        The new dataframe must have a 'SHAPE' column containing geometries of the same type as the live data. The
+        dataframe must have a WGS84 (wkid 4326) projection. New OBJECTIDs will be automatically generated.
 
         The new dataframe's columns and data must match the existing data's fields (with the exception of generated
         fields like shape area and length) in name, type, and allowable length. Live fields that are not nullable and
         don't have a default value must have a value in the new data; missing data in these fields will raise an error.
 
         Args:
             gis (arcgis.gis.GIS): GIS item for AGOL org
@@ -165,172 +178,36 @@
             if 'SHAPE' in self.new_dataframe.columns:
                 self.new_dataframe.spatial.set_geometry('SHAPE')
         if fields is not None:
             self.fields = list(set(fields) - {'Shape_Area', 'Shape_Length'})  #: We don't use these auto-gen fields
         self.failsafe_dir = failsafe_dir if failsafe_dir else None
         self.layer_index = layer_index
 
-    #: NOTE: Saving all this for potential reuse in transform.py
-
-    # def __init__(self, gis, dataframe, index_column, field_mapping=None):
-    #     self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
-    #     self.gis = gis
-    #     self.index_column = utils.rename_columns_for_agol([index_column])[index_column]
-
-    #     if field_mapping:
-    #         dataframe = utils.rename_fields(dataframe, field_mapping)
-
-    #     self.new_dataframe = dataframe.rename(columns=utils.rename_columns_for_agol(dataframe.columns))
-    #     try:
-    #         self.new_data_as_dict = self.new_dataframe.set_index(self.index_column).to_dict('index')
-    #     except KeyError as error:
-    #         raise KeyError(f'Index column {index_column} not found in dataframe columns') from error
-
-    # def _get_common_rows(self, live_dataframe) -> pd.DataFrame:
-    #     """Create a dataframe containing only the rows common to both the existing live dataset and the new updates
-
-    #     Args:
-    #         live_dataframe (pd.Dataframe): The existing, live dataframe created from an AGOL hosted feature layer.
-
-    #     Returns:
-    #         pd.DataFrame: A new dataframe containing the common rows created by .merge()ing.
-    #     """
-
-    #     subset_dataframe = live_dataframe[live_dataframe[self.index_column] \
-    #         .isin(self.new_dataframe[self.index_column])] \
-    #         .set_index(self.index_column)
-    #     subset_dataframe.update(self.new_dataframe.set_index(self.index_column))
-
-    #     not_found_dataframe = self.new_dataframe[~self.new_dataframe[self.index_column]
-    #                                              .isin(live_dataframe[self.index_column])]
-    #     if not not_found_dataframe.empty:
-    #         keys_not_found = list(not_found_dataframe[self.index_column])
-    #         self._class_logger.warning(
-    #             'The following keys from the new data were not found in the existing dataset: %s', keys_not_found
-    #         )
-
-    #     return subset_dataframe.reset_index()
-
-    # def _clean_dataframe_columns(self, dataframe, fields) -> pd.DataFrame:
-    #     """Delete superfluous fields from dataframe that will be used for the .edit() operation
-
-    #     Removes or renames the '_x', '_y' fields that are created by dataframe.merge() as appropriate based on the
-    #     fields provided.
-
-    #     Args:
-    #         dataframe (pd.Dataframe): Dataframe to be cleaned
-    #         fields (list[str]): The fields to keep; all others will be deleted
-
-    #     Returns:
-    #         pd.DataFrame: A dataframe with only our desired columns.
-    #     """
-
-    #     #: rename specified fields, delete any other _x/_y fields (in effect, just keep the specified fields...)
-    #     #: TODO: There may be a simpler way to do this- maybe .reindex(fields)?
-    #     rename_dict = {f'{f}_y': f for f in fields}
-    #     renamed_dataframe = dataframe.rename(columns=rename_dict).copy()
-    #     fields_to_delete = [f for f in renamed_dataframe.columns if f.endswith(('_x', '_y'))]
-    #     fields_to_delete.append('_merge')
-    #     self._class_logger.debug('Deleting joined dataframe fields: %s', fields_to_delete)
-    #     return renamed_dataframe.drop(labels=fields_to_delete, axis='columns', errors='ignore').copy()
-
-    # def _get_old_and_new_values(self, live_dict, object_ids):
-    #     """Create a dictionary of the old (existing, live) and new values based on a list of object ids
-
-    #     Args:
-    #         live_dict (dict): The old (existing, live) data, key is an arbitrary index, content is another dict keyed
-    #         by the field names.
-    #         object_ids (list[int]): The object ids to include in the new dictionary
-
-    #     Returns:
-    #         dict: {object_id:
-    #                 {'old_values': {data as dict from live_dict},
-    #                  'new_values': {data as dict from self.new_dataframe}
-    #                 },
-    #               ...,
-    #               }
-    #     """
-    #     oid_and_key_lookup = {
-    #         row['OBJECTID']: row[self.index_column] for _, row in live_dict.items() if row['OBJECTID'] in object_ids
-    #     }
-    #     old_values_by_oid = {row['OBJECTID']: row for _, row in live_dict.items() if row['OBJECTID'] in object_ids}
-    #     new_data_as_dict_preserve_key = self.new_dataframe.set_index(self.index_column, drop=False).to_dict('index')
-    #     new_values_by_oid = {
-    #         object_id: new_data_as_dict_preserve_key[key] for object_id, key in oid_and_key_lookup.items()
-    #     }
-
-    #     combined_values_by_oid = {
-    #         object_id: {
-    #             'old_values': old_values_by_oid[object_id],
-    #             'new_values': new_values_by_oid[object_id]
-    #         } for object_id in oid_and_key_lookup
-    #     }
-
-    #     return combined_values_by_oid
-
-    # def _parse_results(self, results_dict, live_dataframe) -> int:
-    #     """Integrate .edit() results with data for reporting purposes. Relies on _get_old_and_new_values().
-
-    #     Args:
-    #         results_dict (dict): AGOL response as a python dict (raw output from .edit_features(). Defined in
-    #         https://developers.arcgis.com/rest/services-reference/enterprise/apply-edits-feature-service-layer-.htm,
-    #         where `true`/`false` are python True/False.
-    #         live_dataframe (pd.DataFrame): Existing/live dataframe created from hosted feature layer.
-
-    #     Returns:
-    #         int: Number of edits successfully applied. If any failed, rollback will cause this to be set to 0.
-    #     """
-
-    #     live_dataframe_as_dict = live_dataframe.to_dict('index')
-    #     update_results = results_dict['updateResults']
-    #     if not update_results:
-    #         self._class_logger.info('No update results returned; no updates attempted')
-    #         return 0
-    #     update_successes = [result['objectId'] for result in update_results if result['success']]
-    #     update_failures = [result['objectId'] for result in update_results if not result['success']]
-    #     rows_updated = len(update_successes)
-    #     if update_successes:
-    #         self._class_logger.info('%s rows successfully updated:', len(update_successes))
-    #         for _, data in self._get_old_and_new_values(live_dataframe_as_dict, update_successes).items():
-    #             self._class_logger.debug('Existing data: %s', data['old_values'])
-    #             self._class_logger.debug('New data: %s', data['new_values'])
-    #     if update_failures:
-    #         self._class_logger.warning(
-    #             'The following %s updates failed. As a result, all successful updates should have been rolled back.',
-    #             len(update_failures)
-    #         )
-    #         for _, data in self._get_old_and_new_values(live_dataframe_as_dict, update_failures).items():
-    #             self._class_logger.warning('Existing data: %s', data['old_values'])
-    #             self._class_logger.warning('New data: %s', data['new_values'])
-    #         rows_updated = 0
-
-    #     return rows_updated
-
     def _add_new_data_to_hosted_feature_layer(self) -> int:
         """Adds new features to existing hosted feature layer. Uses fields from new dataframe.
 
         Raises:
             ValueError: If the new field and existing fields don't match, the new data contains null fields,
-                        the new data exceeds the existing field lengths, or a specified field is missing from either
-                        new or live data.
+                the new data exceeds the existing field lengths, or a specified field is missing from either
+                new or live data.
 
         Returns:
             int: Number of features added
         """
 
         self._class_logger.info(
             'Adding items to layer `%s` in itemid `%s` in-place', self.layer_index, self.feature_service_itemid
         )
         self._class_logger.debug('Using fields %s', self.fields)
 
         #: Field checks to prevent various AGOL errors
         utils.FieldChecker.check_fields(self.feature_layer.properties, self.new_dataframe, self.fields, add_oid=False)
 
         #: Upsert
-        append_count = self._upsert_data(
+        append_count = self._upload_data(
             self.feature_layer,
             self.new_dataframe,
             upsert=False,
         )
         return append_count
 
     def _delete_data_from_hosted_feature_layer(self, delete_oids) -> int:
@@ -377,16 +254,16 @@
         return actual_delete_count
 
     def _update_hosted_feature_layer(self, update_geometry) -> int:
         """Updates existing features within a hosted feature layer using OBJECTID as the join field
 
         Raises:
             ValueError: If the new field and existing fields don't match, the new data contains null fields,
-                        the new data exceeds the existing field lengths, or a specified field is missing from either
-                        new or live data.
+                the new data exceeds the existing field lengths, or a specified field is missing from either
+                new or live data.
 
         Returns:
             int: Number of features updated
         """
 
         self._class_logger.info(
             'Updating layer `%s` in itemid `%s` in-place', self.layer_index, self.feature_service_itemid
@@ -399,35 +276,34 @@
             self._class_logger.debug('Attribute-only update; inserting null geometries')
             self.new_dataframe['SHAPE'] = utils.get_null_geometries(self.feature_layer.properties)
 
         #: Field checks to prevent various AGOL errors
         utils.FieldChecker.check_fields(self.feature_layer.properties, self.new_dataframe, self.fields, add_oid=True)
 
         #: Upsert
-        append_count = self._upsert_data(
+        append_count = self._upload_data(
             self.feature_layer,
             self.new_dataframe,
             upsert=True,
             upsert_matching_field='OBJECTID',
             append_fields=self.fields,  #: Apparently this works if append_fields is all the fields, but not a subset?
             update_geometry=update_geometry
         )
         return append_count
 
     #: TODO: rename this method? not everything is an upsert
-    #: FIXME: Note: in this docstring
-    def _upsert_data(self, target_featurelayer, dataframe, **append_kwargs):
+    def _upload_data(self, target_featurelayer, dataframe, **append_kwargs):
         """UPdate and inSERT data into live dataset with featurelayer.append()
 
-        Note: The call to to_featureset() in this method will add new OBJECTIDs to the new data if they aren't already present. If
+        Note: The call to to_featureset() in this method will add new OBJECTIDs to the new data if they aren't already present.
 
         Args:
             target_featurelayer (arcgis.features.FeatureLayer): Live dataset
             dataframe (pd.DataFrame): Spatially-enabled dataframe containing new data. Column names must match live
-            data. New data must have a valid shape column
+                data. New data must have a valid shape column
             append_kwargs (keyword arguments): Arguments to be passed to .append()
 
         Raises:
             RuntimeError: If append fails; will attempt to rollback appends that worked.
 
         Returns:
             dict: Messages returned from append operation
@@ -508,15 +384,15 @@
         utils.FieldChecker.check_fields(self.feature_layer.properties, self.new_dataframe, self.fields, add_oid=False)
 
         self._class_logger.info('Truncating existing features...')
         self._truncate_existing_data()
 
         try:
             self._class_logger.info('Loading new data...')
-            append_count = self._upsert_data(self.feature_layer, self.new_dataframe, upsert=False)
+            append_count = self._upload_data(self.feature_layer, self.new_dataframe, upsert=False)
             self._class_logger.debug('Total truncate and load time: %s', datetime.now() - start)
         except Exception:
             if self.failsafe_dir:
                 self._class_logger.error(
                     'Append failed, feature service may be dirty due to append chunking. Data saved to %s',
                     saved_layer_path
                 )
@@ -544,31 +420,43 @@
         if truncate_result['status'] != 'Completed':
             raise RuntimeError(
                 f'Failed to truncate existing data from layer id {self.layer_index} in itemid {self.feature_service_itemid}'
             )
 
 
 class FeatureServiceAttachmentsUpdater:
-    """Add or overwrite attachments in a feature service using a dataframe of the desired "new" attachments. Uses a
-    join field present in both live data and the attachments dataframe to match attachments with live data.
+    """Add or overwrite attachments in a feature service using a dataframe of the desired "new" attachments.
+
+    Updates the attachments based on a dataframe containing two columns: a join key present in the live data (the
+    dataframe column name must match the feature service field name) and the path of the file to attach to the feature.
+    While AGOL supports multiple attachments, this only accepts a single file as input.
+
+    If a matching feature in AGOl doesn't have an attachment, the file referred to by the dataframe will be uploaded.
+    If it does have an attachment, it checks the existing filename with the referenced file. If they are different, the
+    file from the dataframe will be updated. If they are the same, nothing happens.
     """
 
     def __init__(self, gis):
+        """
+        Args:
+            gis (arcgis.gis.GIS): The AGOL organization's gis object
+        """
+
         self.gis = gis
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         self.failed_dict = {}
 
     def _get_live_oid_and_guid_from_join_field_values(self, live_features_as_df, attachment_join_field, attachments_df):
         """Get the live Object ID and guid from the live features for only the features in attachments_df
 
         Args:
             live_features_as_df (pd.DataFrame): Spatial dataframe of all the feature layer's live data from AGOL
             attachment_join_field (str): Column in attachments_df to use as a join key with live data
             attachments_df (pd.DataFrame): New attachment data, including the join key and a path to the "new"
-                                           attachment
+                attachment
 
         Returns:
             pd.DataFrame: Attachments dataframe with corresponding live OIDs and GUIDs.
         """
 
         self._class_logger.debug('Using %s as the join field between live and new data', attachment_join_field)
         subset_df = live_features_as_df.reindex(columns=['OBJECTID', 'GlobalID', attachment_join_field])
@@ -601,15 +489,15 @@
         """Create a dataframe containing the action needed for each feature resulting from the attachment join.
 
         If the live feature doesn't have an attachment, add the attachment. If it does, compare the file names and only
         attach if they are different. Otherwise, leave null.
 
         Args:
             attachment_eval_df (pd.DataFrame): DataFrame of live attachment data, subsetted to features that matched
-                                               the join key in the new attachments
+                the join key in the new attachments
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             pd.DataFrame: attachment_eval_df with 'operation' and 'new_filename' columns added
         """
 
         #: Get the file name from the full path
@@ -635,15 +523,15 @@
         return attachment_eval_df
 
     def _add_attachments_by_oid(self, attachment_action_df, attachment_path_field):
         """Add attachments using the feature's OID based on the 'operation' field of the dataframe
 
         Args:
             attachment_action_df (pd.DataFrame): A dataframe containing 'operation', 'OBJECTID', and
-                                                 attachment_path_field columns
+                attachment_path_field columns
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             int: The number of features that successfully have attachments added.
         """
 
         adds_dict = attachment_action_df[attachment_action_df['operation'] == 'add'].to_dict(orient='index')
@@ -672,15 +560,15 @@
         return adds_count
 
     def _overwrite_attachments_by_oid(self, attachment_action_df, attachment_path_field):
         """Overwrite attachments using the feature's OID based on the 'operation' field of the dataframe
 
         Args:
             attachment_action_df (pd.DataFrame): A dataframe containing 'operation', 'OBJECTID', 'ID', 'NAME', and
-                                                 attachment_path_field columns
+                attachment_path_field columns
             attachment_path_field (str): The column that holds the attachment path
 
         Returns:
             int: The number of features that successfully have their attachments overwritten.
         """
 
         overwrites_dict = attachment_action_df[attachment_action_df['operation'] == 'overwrite'].to_dict(orient='index')
@@ -736,18 +624,18 @@
         attachments. If the name of the "new" attachment is the same as an existing attachment for that feature, it is
         not updated. If it is different or there isn't an existing attachment, the "new" attachment is attached to that
         feature.
 
         Args:
             feature_layer_itemid (str): The AGOL Item ID of the feature layer to update
             attachment_join_field (str): The field containing the join key between the attachments dataframe and the
-                                         live data
+                live data
             attachment_path_field (str): The field containing the desired attachment file path
             attachments_df (pd.DataFrame): A dataframe of desired attachments, including a join key and the local path
-                                           to the attachment
+                to the attachment
             layer_number (int, optional): The layer within the Item ID to update. Defaults to 0.
 
         Returns:
             (int, int): Tuple of counts of successful overwrites and adds.
         """
 
         self._class_logger.info('Updating attachments...')
@@ -796,18 +684,28 @@
         attachments_dataframe['full_file_path'] = attachments_dataframe[attachment_column] \
                                                     .apply(lambda filename: str(Path(out_dir, filename)))
 
         return attachments_dataframe
 
 
 class ColorRampReclassifier:
-    """Updates the interval ranges on a layer's classification renderer based on the layer's current data.
+    """Updates the interval ranges on a webmap's layer's classification renderer based on the layer's current data.
+
+    Manually edits the JSON definition to change a layer's color ramp values based on a simple unclassed scheme similar
+    to AGOL's unclassed ramp. The minimum value is the dataset minimum, the max is the mean value plus one standard
+    deviation.
     """
 
     def __init__(self, webmap_item, gis):
+        """
+        Args:
+            webmap_item (arcgis.mapping.WebMap): The webmap item in the AGOL organization
+            gis (arcgis.gis.GIS): The AGOL organization as a gis object
+        """
+
         self.webmap_item = webmap_item
         self.gis = gis
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
     def _get_layer_dataframe(self, layer_name, feature_layer_number=0):
         """Create a dataframe from layer_name in self.webmap_item
```

### Comparing `ugrc-palletjack-3.0.0b6/src/palletjack/transform.py` & `ugrc-palletjack-3.1.0/src/palletjack/transform.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-"""transform.py: Processes in the Transformation step of ETL
+"""Transform pandas dataframes in preparation for loading to AGOL.
 """
+import locale
 import logging
 import warnings
 from datetime import datetime
 
 import arcgis
 import pandas as pd
 from arcgis import GeoAccessor, GeoSeriesAccessor
 
 from palletjack import utils
 
 module_logger = logging.getLogger(__name__)
 
 
 class APIGeocoder:
-    """Geocode using the UGRC Web API Geocoder.
+    """Geocode a dataframe using the UGRC Web API Geocoder.
 
     Instantiate an APIGeocoder object with an api key from developer.mapserv.utah.gov. It will attempt to validate the
-    API key. If it fails, it will raise one of the following:
-        RuntimeError: If there was a network or other error
-        ValueError: If the API responds with an invalid key message
-        UserWarning: If the API responds with some other abnormal result
+    API key. If validation fails, it will raise one of the following errors:
+
+    - RuntimeError: If there was a network or other error
+    - ValueError: If the key is invalid
+    - UserWarning: If the API responds with some other abnormal result
+
+    The individual geocoding steps are exposed in the `palletjack.utils.Geocoding` class in the utils module for use in
+    other settings.
     """
 
     def __init__(self, api_key):
+        """
+        Args:
+            api_key (str): API key obtained from developer.mapserv.utah.gov
+        """
         self.api_key = api_key
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
         utils.Geocoding.validate_api_key(self.api_key)
 
     def geocode_dataframe(self, dataframe, street_col, zone_col, wkid, rate_limits=(0.015, 0.03), **api_args):
         """Geocode a pandas dataframe into a spatially-enabled dataframe
 
@@ -35,15 +44,15 @@
 
         Args:
             dataframe (pd.DataFrame): Input data with separate columns for street address and zip or city
             street_col (str): The column containing the street address
             zone_col (str): The column containing either the zip code or the city name
             wkid (int): The projection to return the x/y points in
             rate_limits(Tuple <float>): A lower and upper bound in seconds for pausing between API calls. Defaults to
-            (0.015, 0.03)
+                (0.015, 0.03)
             **api_args (dict): Keyword arguments to be passed as parameters in the API GET call.
 
         Returns:
             pd.DataFrame.spatial: Geocoded data as a spatially-enabled DataFrame
         """
 
         start = datetime.now()
@@ -85,17 +94,34 @@
             self._class_logger.debug('Average time per record: %s', (end - start) / len(spatial_dataframe.index))
         except ZeroDivisionError:
             warnings.warn('Empty spatial dataframe after geocoding', RuntimeWarning)
         return spatial_dataframe
 
 
 class FeatureServiceMerging:
+    """Get the live dataframe from a feature service and update it from another dataframe
+    """
 
     @staticmethod
     def update_live_data_with_new_data(live_dataframe, new_dataframe, join_column):
+        """Update a dataframe with data from another
+
+        Args:
+            live_dataframe (pd.DataFrame): The dataframe containing info to be updated
+            new_dataframe (pd.DataFrame): Dataframe containing source info to use in the update
+            join_column (str): The column with unique IDs to be used as a key between the two dataframes
+
+        Raises:
+            ValueError: If the join_column is missing from either live or new data
+            RuntimeWarning: If there are rows in the new data that are not found in the live data; these will not be
+                added to the live dataframe.
+
+        Returns:
+            pd.DataFrame: The updated dataframe, with data types converted via .convert_dtypes()
+        """
 
         try:
             live_dataframe.set_index(join_column, inplace=True)
             new_dataframe.set_index(join_column, inplace=True)
         except KeyError as error:
             raise ValueError('Join column not found in live or new dataframes') from error
 
@@ -109,14 +135,28 @@
             )
 
         live_dataframe.update(new_dataframe)
         return (live_dataframe.reset_index().convert_dtypes())
 
     @staticmethod
     def get_live_dataframe(gis, feature_service_itemid, layer_index=0):
+        """Get a spatially-enabled dataframe representation of a hosted feature layer
+
+        Args:
+            gis (arcgis.gis.GIS): GIS object of the desired organization
+            feature_service_itemid (str): itemid in the gis of the desired hosted feature service
+            layer_index (int, optional): Index of the desired layer within the hosted feature service. Defaults to 0.
+
+        Raises:
+            RuntimeError: If it fails to load the data
+
+        Returns:
+            pd.DataFrame.spatial: Spatially-enabled dataframe representation of the hosted feature layer
+        """
+
         try:
             feature_layer = arcgis.features.FeatureLayer.fromitem(
                 gis.content.get(feature_service_itemid), layer_id=layer_index
             )
             live_dataframe = feature_layer.query(as_df=True)
         except Exception as error:
             raise RuntimeError('Failed to load live dataframe') from error
@@ -134,24 +174,25 @@
 
         Args:
             dataframe (pd.DataFrame): Input dataframe with columns to be converted
             fields_that_should_be_ints (list[str]): List of column names to be converted
 
         Raises:
             TypeError: If any of the conversions fail. Often caused by values that aren't int-castable floats (ie. x.0)
-            or np.nans.
+                or np.nans.
 
         Returns:
             pd.DataFrame: Input dataframe with columns converted to nullable Int64
         """
 
-        int_dict = {field: 'Int64' for field in fields_that_should_be_ints}
+        retyped = dataframe.copy()
         try:
-            retyped = dataframe.astype(int_dict)
-        except TypeError as error:
+            for field in fields_that_should_be_ints:
+                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], 'Int64')
+        except (TypeError, ValueError) as error:
             raise TypeError(
                 'Cannot convert one or more fields to nullable ints. Check for non-int/non-np.nan values.'
             ) from error
         return retyped
 
     @staticmethod
     def switch_to_float(dataframe, fields_that_should_be_floats):
@@ -159,32 +200,51 @@
 
         Args:
             dataframe (pd.DataFrame): Input dataframe with columns to be converted
             fields_that_should_be_floats (list[str]): List of column names to be converted
 
         Raises:
             TypeError: If any of the conversions fail. Often caused by values that aren't castable to floats
-            (non-empty, non-numeric strings, etc)
+                (non-empty, non-numeric strings, etc)
 
         Returns:
             pd.DataFrame: Input dataframe with columns converted to float
         """
 
-        float_dict = {field: 'float' for field in fields_that_should_be_floats}
-        empty_string_dict = {field: {'': None} for field in fields_that_should_be_floats}
+        retyped = dataframe.copy()
         try:
-            no_empty_strings = dataframe.replace(empty_string_dict)
-            retyped = no_empty_strings.astype(float_dict)
-        except TypeError as error:
+            for field in fields_that_should_be_floats:
+                retyped[field] = DataCleaning._switch_series_to_numeric_dtype(retyped[field], 'float')
+        except (TypeError, ValueError) as error:
             raise TypeError(
                 'Cannot convert one or more fields to floats. Check for non-float/non-null values.'
             ) from error
         return retyped
 
     @staticmethod
+    def _switch_series_to_numeric_dtype(series, dtype):
+        """Switch the dtype of a series to the specified dtype
+
+        Series of dtype 'object' (ie, series of strings or mixed strings and numbers) are converted to str so that they
+        can be de-localized to remove comma thousands separators
+
+        Args:
+            series (pd.Series): The series to be converted
+            dtype (str): The dtype to convert to
+
+        Returns:
+            pd.Series: The converted series
+        """
+
+        if series.dtype == 'object':
+            series = series.astype(str).apply(locale.delocalize)
+            series.replace('', None, inplace=True)
+        return series.astype(dtype)
+
+    @staticmethod
     def switch_to_datetime(dataframe, date_fields, **to_datetime_kwargs):
         """Convert specified fields to datetime dtypes to ensure proper date formatting for AGOL
 
         Args:
             dataframe (pd.DataFrame): The source dataframe
             date_fields (List[int]): The fields to convert to datetime
             **to_datetime_kwargs (keyword arguments, optional): Arguments to pass through to pd.to_datetime
```

### Comparing `ugrc-palletjack-3.0.0b6/src/palletjack/utils.py` & `ugrc-palletjack-3.1.0/src/palletjack/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""Utility classes and methods that are used internally throughout palletjack. Many are exposed publicly in case they are useful elsewhere in a client's code.
+"""
+
 import datetime
 import importlib
 import logging
 import random
 import re
 import sys
 import warnings
@@ -26,15 +29,15 @@
     seconds between each retry. Any arguments for worker_method can be passed in as additional parameters to retry()
     following worker_method: retry(foo_method, arg1, arg2, keyword_arg=3)
 
     Args:
         worker_method (callable): The name of the method to be retried (minus the calling parens)
 
     Raises:
-        error: The final error the causes worker_method to fail after 3 retries
+        error: The final error that causes worker_method to fail after 3 retries
 
     Returns:
         various: The value(s) returned by worked_method
     """
     tries = 1
     max_tries = 3
     delay = 2  #: in seconds
@@ -191,31 +194,31 @@
     for field in featurelayer.properties.indexes:
         if field['fields'] == field_name:
             if not field['isUnique']:
                 raise RuntimeError(f'{field_name} does not have a "unique constraint" set within the feature layer')
 
 
 class Geocoding:
-    """Container class for methods to geocode an address
+    """Methods for geocoding an address
     """
 
     @staticmethod
     def geocode_addr(street, zone, api_key, rate_limits, **api_args):
         """Geocode an address through the UGRC Web API geocoder
 
         Invalid results are returned with an x,y of 0,0, a score of 0.0, and a match address of 'No Match'
 
         Args:
             street (str): The street address
             zone (str): The zip code or city
             api_key (str): API key obtained from developer.mapserv.utah.gov
-            rate_limits(Tuple <float>): A lower and upper bound in seconds for pausing between API calls. Defaults to
-            (0.015, 0.03)
-            **api_args (dict): Keyword arguments to be passed as parameters in the API GET call. The API key will be added
-            to this dict.
+            rate_limits (Tuple <float>): A lower and upper bound in seconds for pausing between API calls. Defaults to
+                (0.015, 0.03)
+            **api_args (dict): Keyword arguments to be passed as parameters in the API GET call. The API key will be
+                added to this dict.
 
         Returns:
             tuple[int]: The match's x coordinate, y coordinate, score, and match address
         """
 
         sleep(random.uniform(rate_limits[0], rate_limits[1]))
         url = f'https://api.mapserv.utah.gov/api/v1/geocode/{street}/{zone}'
@@ -234,16 +237,16 @@
             geocode_result_dict['matchAddress'],
         )
 
     @staticmethod
     def _geocode_api_call(url, api_args):
         """Makes a requests.get call to the geocoding API.
 
-        Meant to be called through a retry wrapper so that the RuntimeErrors get tried again a couple times before finally
-        raising the error.
+        Meant to be called through a retry wrapper so that the RuntimeErrors get tried again a couple times before
+            finally raising the error.
 
         Args:
             url (str): Base url for GET request
             api_args (dict): Dictionary of URL parameters
 
         Raises:
             RuntimeError: If the server does not return response and request.get returns a falsy object.
@@ -328,16 +331,20 @@
 
     return floor(n / 20)
 
 
 def authorize_pygsheets(credentials):
     """Authenticate pygsheets using either a service file or google.auth.credentials.Credentials object.
 
-    Tries first to load credentials as a service account file; if this fails with a FileNotFoundError, tries to pass
-    credentials directly as a custom_credential.
+    Requires either the path to a service account .json file that has access to the files in question or  a `google.
+    auth.credentials.Credentials` object. Calling `google.auth.default()` in a Google Cloud Function will give you a
+    tuple of a `Credentials` object and the project id. You can use this `Credentials` object to authorize pygsheets as
+    the same account the Cloud Function is running under.
+
+    Tries first to load credentials from file; if this fails tries credentials directly as a custom_credential.
 
     Args:
         credentials (str or google.auth.credentials.Credentials): Path to the service file OR credentials object
             obtained from google.auth.default() within a cloud function.
 
     Raises:
         RuntimeError: If both authorization method attempts fail
@@ -363,14 +370,15 @@
     Args:
         feature_layer (arcgis.features.FeatureLayer): The FeatureLayer object to save to disk.
         directory (str or Path): The directory to save the data to.
 
     Returns:
         Path: The full path to the output file, named with the layer name and today's date.
     """
+
     module_logger.debug('Downloading existing data...')
     dataframe = feature_layer.query().sdf
 
     if dataframe.empty:
         return f'No data to save in feature layer {feature_layer.properties.name}'
 
     out_path = Path(directory, f'{feature_layer.properties.name}_{datetime.date.today()}.json')
@@ -378,39 +386,46 @@
     out_path.write_text(dataframe.spatial.to_featureset().to_json, encoding='utf-8')
 
     return out_path
 
 
 class FieldChecker:
     """Check the fields of a new dataframe against live data. Each method will raise errors if its checks fail.
+    Provides the check_fields class method to run all the checks in one call with having to create an object.
     """
 
     @classmethod
     def check_fields(cls, live_data_properties, new_dataframe, fields, add_oid):
         """Run all the field checks, raising errors and warnings where they fail.
 
         Check individual method docstrings for details and specific errors raised.
 
         Args:
             live_data_properties (dict): FeatureLayer.properties of live data
             new_dataframe (pd.DataFrame): New data to be checked
             fields (List[str]): Fields to check
             add_oid (bool): Add OBJECTID to fields if its not already present (for operations that are dependent on
-                            OBJECTID, such as upsert)
+                OBJECTID, such as upsert)
         """
 
         field_checker = cls(live_data_properties, new_dataframe)
+        field_checker.check_fields_present(fields, add_oid=add_oid)
         field_checker.check_live_and_new_field_types_match(fields)
         field_checker.check_for_non_null_fields(fields)
         field_checker.check_field_length(fields)
-        field_checker.check_fields_present(fields, add_oid=add_oid)
         field_checker.check_srs_wgs84()
         field_checker.check_nullable_ints_shapely()
 
     def __init__(self, live_data_properties, new_dataframe):
+        """
+        Args:
+            live_data_properties (dict): FeatureLayer.properties of live data
+            new_dataframe (pd.DataFrame): New data to be checked
+        """
+
         self.live_data_properties = live_data_properties
         self.fields_dataframe = pd.DataFrame(live_data_properties.fields)
         self.new_dataframe = new_dataframe
 
     def check_live_and_new_field_types_match(self, fields):
         """Raise an error if the field types of the live and new data don't match.
 
@@ -418,15 +433,15 @@
         _check_geometry_types to verify the spatial types are compatible.
 
         Args:
             fields (List[str]): Fields to be updated
 
         Raises:
             ValueError: If the field types or spatial types are incompatible, the new data has multiple geometry types,
-            or the new data is not a valid spatially-enabled dataframe.
+                or the new data is not a valid spatially-enabled dataframe.
             NotImplementedError: If the live data has a field that has not yet been mapped to a pandas dtype.
         """
 
         #: Converting dtypes to str and comparing seems to be the only way to break out into shorts and longs, singles
         #: and doubles. Otherwise, checking subclass is probably more pythonic.
         short_ints = ['uint8', 'uint16', 'int8', 'int16']
         long_ints = ['int', 'uint32', 'uint64', 'int32', 'int64']
@@ -496,15 +511,15 @@
 
         Args:
             live_data_properties (dict): FeatureLayer.properties of live data
             new_dataframe (pd.DataFrame): New data to be added/updated
 
         Raises:
             ValueError: If the new data is not a valid spatially-enabled dataframe, has multiple geometry types, or has
-            a geometry type that doesn't match the live data.
+                a geometry type that doesn't match the live data.
         """
 
         esri_to_sedf_geometry_mapping = {
             'esriGeometryPoint': 'point',
             'esriGeometryMultipoint': 'multipoint',
             'esriGeometryPolyline': 'polyline',
             'esriGeometryPolygon': 'polygon',
@@ -530,15 +545,15 @@
         appropriate nodata values.
 
         Args:
             fields (List[str]): Fields to check
 
         Raises:
             ValueError: If the new data contains nulls in a field that the live data says is not nullable and doesn't
-            have a default value.
+                have a default value.
         """
 
         columns_with_nulls = self.new_dataframe.columns[self.new_dataframe.isna().any()].tolist()
         # fields_dataframe = pd.DataFrame(self.live_data_properties['fields'])
         non_nullable_live_columns = self.fields_dataframe[
             ~(self.fields_dataframe['nullable']) &
             ~(self.fields_dataframe['defaultValue'].astype(bool))]['name'].tolist()
@@ -563,15 +578,15 @@
         """Raise an error if a new data string value is longer than allowed in the live data.
 
         Args:
             fields (List[str]): Fields to check
 
         Raises:
             ValueError: If the string fields in the new data contain a value longer than the corresponding field in the
-            live data allows.
+                live data allows.
         """
 
         if 'length' not in self.fields_dataframe.columns:
             module_logger.debug('No fields with length property')
             return
 
         length_limited_fields = self.fields_dataframe[
@@ -590,23 +605,24 @@
 
     def check_fields_present(self, fields, add_oid):
         """Raise an error if the fields to be operated on aren't present in either the live or new data.
 
         Args:
             fields (List[str]): The fields to be operated on.
             add_oid (bool): Add OBJECTID to fields if its not already present (for operations that are dependent on
-                            OBJECTID, such as upsert)
+                OBJECTID, such as upsert)
 
         Raises:
             RuntimeError: If any of fields are not in live or new data.
         """
 
         live_fields = set(self.fields_dataframe['name'])
         new_fields = set(self.new_dataframe.columns)
         working_fields = set(fields)
+        working_fields.discard('SHAPE')  #: The fields from the feature layer properties don't include the SHAPE field.
         if add_oid:
             working_fields.add('OBJECTID')
 
         live_dif = working_fields - live_fields
         new_dif = working_fields - new_fields
 
         error_message = []
@@ -645,15 +661,15 @@
     def check_nullable_ints_shapely(self):
         """Raise a warning if null values occur within nullable integer fields of the dataframe
 
         Apparently due to a convention within shapely, any null values in an integer field are converted to 0.
 
         Raises:
             UserWarning: If we're using shapely instead of arcpy, the new dataframe uses nullable int dtypes, and there
-            is one or more pd.NA values within a nullable int column.
+                is one or more pd.NA values within a nullable int column.
         """
 
         #: Only occurs if client is using shapely instead of arcpy
         if importlib.util.find_spec('arcpy'):
             return
 
         nullable_ints = {'Int8', 'Int16', 'Int32', 'Int64', 'UInt8', 'UInt16', 'UInt32', 'UInt64'}
@@ -711,15 +727,15 @@
             }
         }).JSON
 
     raise NotImplementedError(f'Null value generator for live geometry type {live_geometry_type} not yet implemented')
 
 
 class DeleteUtils:
-    """Container class for verifying Object IDs used for delete operations
+    """Verify Object IDs used for delete operations
     """
 
     @staticmethod
     def check_delete_oids_are_ints(oid_list):
         """Raise an error if a list of strings can't be parsed as ints
 
         Args:
@@ -781,15 +797,15 @@
         if oids_not_in_layer:
             warnings.warn(f'OBJECTIDs {oids_not_in_layer} were not found in the live data')
 
         return len(oids_not_in_layer)
 
 
 class Chunking:
-    """Container class for dividing a dataframe into chunks to satisfy size requirements for append operation
+    """Divide a dataframe into chunks to satisfy upload size requirements for append operation.
     """
 
     @staticmethod
     def _ceildiv(num, denom):
         """Perform ceiling division: 5/4 = 2
 
         Args:
@@ -834,15 +850,15 @@
         nullable numeric fields in feature sets created from individual chunks to None prior to converting to geojson to
         ensure the field stays numeric.
 
         Args:
             dataframe (pd.DataFrame.spatial): Spatially-enabled dataframe to be converted to geojson
             feature_layer_fields: All the fields from the feature layer (feature_layer.properties.fields)
             max_bytes (int, optional): Maximum size in bytes any one geojson string can be. Defaults to 100000000 (AGOL
-            text uploads are limited to 100 MB?)
+                text uploads are limited to 100 MB?)
 
         Returns:
             list[str]: A list of the dataframe chunks converted to geojson
         """
 
         geojson_size = sys.getsizeof(dataframe.spatial.to_featureset().to_geojson.encode('utf-16'))
         module_logger.debug('Initial file size: %s', geojson_size)
```

### Comparing `ugrc-palletjack-3.0.0b6/src/ugrc_palletjack.egg-info/SOURCES.txt` & `ugrc-palletjack-3.1.0/src/ugrc_palletjack.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 setup.cfg
 setup.py
 src/palletjack/__init__.py
 src/palletjack/errors.py
 src/palletjack/extract.py
 src/palletjack/load.py
-src/palletjack/testing.py
 src/palletjack/transform.py
 src/palletjack/utils.py
 src/palletjack/version.py
 src/ugrc_palletjack.egg-info/PKG-INFO
 src/ugrc_palletjack.egg-info/SOURCES.txt
 src/ugrc_palletjack.egg-info/dependency_links.txt
 src/ugrc_palletjack.egg-info/entry_points.txt
```

