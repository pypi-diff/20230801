# Comparing `tmp/earthaccess-0.5.2.tar.gz` & `tmp/earthaccess-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthaccess-0.5.2.tar", max compression
+gzip compressed data, was "earthaccess-0.5.3.tar", max compression
```

## Comparing `earthaccess-0.5.2.tar` & `earthaccess-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2023-04-21 00:03:02.080972 earthaccess-0.5.2/LICENSE.txt
--rw-r--r--   0        0        0     7873 2023-04-21 00:03:02.080972 earthaccess-0.5.2/README.md
--rw-r--r--   0        0        0      810 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/__init__.py
--rw-r--r--   0        0        0     9745 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/api.py
--rw-r--r--   0        0        0    14106 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/auth.py
--rw-r--r--   0        0        0   207752 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/css/iso_bootstrap4.0.0min.css
--rw-r--r--   0        0        0      199 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/css/styles.css
--rw-r--r--   0        0        0     5495 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/daac.py
--rw-r--r--   0        0        0     1780 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/formatters.py
--rw-r--r--   0        0        0    10661 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/results.py
--rw-r--r--   0        0        0    24980 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/search.py
--rw-r--r--   0        0        0    21685 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/store.py
--rw-r--r--   0        0        0      140 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/utils/_validation.py
--rw-r--r--   0        0        0        0 2023-04-21 00:03:02.084972 earthaccess-0.5.2/earthaccess/widgets.py
--rw-r--r--   0        0        0     1918 2023-04-21 00:03:02.088971 earthaccess-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     9348 1970-01-01 00:00:00.000000 earthaccess-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-01 15:44:48.412541 earthaccess-0.5.3/LICENSE.txt
+-rw-r--r--   0        0        0     8101 2023-08-01 15:44:48.412541 earthaccess-0.5.3/README.md
+-rw-r--r--   0        0        0      810 2023-08-01 15:44:48.412541 earthaccess-0.5.3/earthaccess/__init__.py
+-rw-r--r--   0        0        0     9908 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/api.py
+-rw-r--r--   0        0        0    14106 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/auth.py
+-rw-r--r--   0        0        0   207752 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/css/iso_bootstrap4.0.0min.css
+-rw-r--r--   0        0        0      199 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/css/styles.css
+-rw-r--r--   0        0        0     5495 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/daac.py
+-rw-r--r--   0        0        0     1774 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/formatters.py
+-rw-r--r--   0        0        0    10661 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/results.py
+-rw-r--r--   0        0        0    26405 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/search.py
+-rw-r--r--   0        0        0    24144 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/store.py
+-rw-r--r--   0        0        0      140 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/utils/_validation.py
+-rw-r--r--   0        0        0        0 2023-08-01 15:44:48.416541 earthaccess-0.5.3/earthaccess/widgets.py
+-rw-r--r--   0        0        0     2027 2023-08-01 15:44:48.420541 earthaccess-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     9374 1970-01-01 00:00:00.000000 earthaccess-0.5.3/PKG-INFO
```

### Comparing `earthaccess-0.5.2/LICENSE.txt` & `earthaccess-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.2/README.md` & `earthaccess-0.5.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 
 <p align="center">
 
 <a href="https://twitter.com/allison_horst" target="_blank">
     <img src="https://img.shields.io/badge/Art%20By-Allison%20Horst-blue" alt="Art Designer: Allison Horst">
 </a>
 
-<a href="https://pypi.org/project/earthdata" target="_blank">
+<a href="https://pypi.org/project/earthaccess" target="_blank">
     <img src="https://img.shields.io/pypi/v/earthaccess?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
-<a href="https://pypi.org/project/earthdata/" target="_blank">
+<a href="https://anaconda.org/conda-forge/earthaccess" target="_blank">
+    <img src="https://img.shields.io/conda/vn/conda-forge/earthaccess.svg" alt="Conda Versions">
+</a>
+
+<a href="https://pypi.org/project/earthaccess/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/earthaccess.svg" alt="Python Versions">
 </a>
 
 <a href='https://earthdata.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/earthdata/badge/?version=latest' alt='Documentation Status' />
 </a>
 
@@ -90,20 +94,19 @@
 
 Once we have selected our dataset we can search for the data granules using *doi*, *short_name* or *concept_id*.
 If we are not sure or we don't know how to search for a particular dataset, we can start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the [NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a complete list of search parameters we can use visit the extended [API documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
 
 ```python
 
 results = earthaccess.search_data(
-    short_name='ATL06',
-    version="005",
+    short_name='SEA_SURFACE_HEIGHT_ALT_GRIDS_L4_2SATS_5DAY_6THDEG_V_JPL2205',
     cloud_hosted=True,
     bounding_box=(-10, 20, 10, 50),
-    temporal=("2020-02", "2020-03"),
-    count=100
+    temporal=("1999-02", "2019-03"),
+    count=10
 )
 
 
 ```
 
 Now that we have our results we can do multiple things: We can iterate over them to get HTTP (or S3) links, we can download the files to a local folder, or we can open these files and stream their content directly to other libraries e.g. xarray.
 
@@ -136,15 +139,17 @@
 **Option 3: Direct S3 Access - Stream data directly to xarray**
 
 This method works best if you are in the same Amazon Web Services (AWS) region as the data (us-west-2) and you are working with gridded datasets (processing level 3 and above).
 
 ```python
 import xarray as xr
 
-ds = xr.open_mfdataset(earthaccess.open(results))
+files = earthaccess.open(results)
+
+ds = xr.open_mfdataset(files)
 
 ```
 
 And that's it! Just one line of code, and this same piece of code will also work for data that are not hosted in the cloud, i.e. located at NASA storage centers.
 
 
 > More examples coming soon!
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 [earthaccess, a python library to search, download or stream NASA Earth science
                       data with just a few lines of code]
-      [Art_Designer:_Allison_Horst] [Package_version] [Python_Versions]
-                            [Documentation_Status]
+   [Art_Designer:_Allison_Horst] [Package_version] [Conda_Versions] [Python
+                       Versions] [Documentation_Status]
 ## **Overview** *earthaccess* is a **python library to search, download or
 stream NASA Earth science data** with just a few lines of code. In the age of
 cloud computing, the power of open science only reaches its full potential if
 we have easy-to-use workflows that facilitate research in an inclusive,
 efficient and reproducible way. Unfortunately âas it stands todayâ
 scientists and students alike face a steep learning curve adapting to systems
 that have grown too complex and end up spending more time on the technicalities
@@ -47,45 +47,46 @@
 search for the data granules using *doi*, *short_name* or *concept_id*. If we
 are not sure or we don't know how to search for a particular dataset, we can
 start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/
 earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the
 [NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a
 complete list of search parameters we can use visit the extended [API
 documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
-```python results = earthaccess.search_data( short_name='ATL06', version="005",
-cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("2020-02", "2020-
-03"), count=100 ) ``` Now that we have our results we can do multiple things:
-We can iterate over them to get HTTP (or S3) links, we can download the files
-to a local folder, or we can open these files and stream their content directly
-to other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using
-the data links** If we already have a workflow in place for downloading our
-data, we can use *earthaccess* as a search-only library and get HTTP links from
-our query results. This could be the case if our current workflow uses a
-different language and we only need the links as input. ```python # if the data
-set is cloud hosted there will be S3 links available. The access parameter
-accepts "direct" or "external", direct access is only possible if you are in
-the us-west-2 region in the cloud. data_links = [granule.data_links
-(access="direct") for granule in results] # or if the data is an on-prem
-dataset data_links = [granule.data_links(access="external") for granule in
-results] ``` > Note: *earthaccess* can get S3 credentials for us, or
-auhenticated HTTP sessions in case we want to use them with a different
-library. **Option 2: Download data to a local folder** This option is practical
-if you have the necessary space available on disk. The *earthaccess* library
-will print out the approximate size of the download and its progress. ```python
-files = earthaccess.download(results, "./local_folder") ``` **Option 3: Direct
-S3 Access - Stream data directly to xarray** This method works best if you are
-in the same Amazon Web Services (AWS) region as the data (us-west-2) and you
-are working with gridded datasets (processing level 3 and above). ```python
-import xarray as xr ds = xr.open_mfdataset(earthaccess.open(results)) ``` And
-that's it! Just one line of code, and this same piece of code will also work
-for data that are not hosted in the cloud, i.e. located at NASA storage
-centers. > More examples coming soon! ### Compatibility Only **Python 3.8+** is
-supported. ## Contributors [![Contributors](https://contrib.rocks/
-image?repo=nsidc/earthaccess)](https://github.com/nsidc/earthaccess/graphs/
-contributors) ## Contributing Guide Welcome! ðð > Please see the
-[Contributing Guide](CONTRIBUTING.md). ### [Project Board](https://github.com/
-nsidc/earthdata/discussions). ### Glossary NASA_Earth_Science_Glossary ##
-License earthaccess is licensed under the MIT license. See [LICENSE]
-(LICENSE.txt). ## Level of Support
+```python results = earthaccess.search_data
+( short_name='SEA_SURFACE_HEIGHT_ALT_GRIDS_L4_2SATS_5DAY_6THDEG_V_JPL2205',
+cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("1999-02", "2019-
+03"), count=10 ) ``` Now that we have our results we can do multiple things: We
+can iterate over them to get HTTP (or S3) links, we can download the files to a
+local folder, or we can open these files and stream their content directly to
+other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using the
+data links** If we already have a workflow in place for downloading our data,
+we can use *earthaccess* as a search-only library and get HTTP links from our
+query results. This could be the case if our current workflow uses a different
+language and we only need the links as input. ```python # if the data set is
+cloud hosted there will be S3 links available. The access parameter accepts
+"direct" or "external", direct access is only possible if you are in the us-
+west-2 region in the cloud. data_links = [granule.data_links(access="direct")
+for granule in results] # or if the data is an on-prem dataset data_links =
+[granule.data_links(access="external") for granule in results] ``` > Note:
+*earthaccess* can get S3 credentials for us, or auhenticated HTTP sessions in
+case we want to use them with a different library. **Option 2: Download data to
+a local folder** This option is practical if you have the necessary space
+available on disk. The *earthaccess* library will print out the approximate
+size of the download and its progress. ```python files = earthaccess.download
+(results, "./local_folder") ``` **Option 3: Direct S3 Access - Stream data
+directly to xarray** This method works best if you are in the same Amazon Web
+Services (AWS) region as the data (us-west-2) and you are working with gridded
+datasets (processing level 3 and above). ```python import xarray as xr files =
+earthaccess.open(results) ds = xr.open_mfdataset(files) ``` And that's it! Just
+one line of code, and this same piece of code will also work for data that are
+not hosted in the cloud, i.e. located at NASA storage centers. > More examples
+coming soon! ### Compatibility Only **Python 3.8+** is supported. ##
+Contributors [![Contributors](https://contrib.rocks/image?repo=nsidc/
+earthaccess)](https://github.com/nsidc/earthaccess/graphs/contributors) ##
+Contributing Guide Welcome! ðð > Please see the [Contributing Guide]
+(CONTRIBUTING.md). ### [Project Board](https://github.com/nsidc/earthdata/
+discussions). ### Glossary NASA_Earth_Science_Glossary ## License earthaccess
+is licensed under the MIT license. See [LICENSE](LICENSE.txt). ## Level of
+Support
 [https://raw.githubusercontent.com/nsidc/earthdata/main/docs/nsidc-logo.png]
 This repository is not actively supported by NSIDC but we welcome issue
 submissions and pull requests in order to foster community contribution.
```

### Comparing `earthaccess-0.5.2/earthaccess/__init__.py` & `earthaccess-0.5.3/earthaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.2/earthaccess/api.py` & `earthaccess-0.5.3/earthaccess/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                                upper_right_lon, upper_right_lat)
     Returns:
         an list of DataCollection results that can be used to get
         information such as concept_id, doi, etc. about a dataset.
     Examples:
         ```python
         datasets = earthaccess.search_datasets(
-            keywords="sea surface anomaly",
+            keyword="sea surface anomaly",
             cloud_hosted=True
         )
         ```
     """
     if not validate.valid_dataset_parameters(**kwargs):
         print(
             "Warning: a valid set of parameters is needed to search for datasets on CMR"
@@ -160,15 +160,20 @@
         local_path: local directory to store the remote data granules
         provider: if we download a list of URLs we need to specify the provider.
         threads: parallel number of threads to use to download the files, adjust as necessary, default = 8
 
     Returns:
         List of downloaded files
     """
-    results = earthaccess.__store__.get(granules, local_path, provider, threads)
+    try:
+        results = earthaccess.__store__.get(granules, local_path, provider, threads)
+    except AttributeError as err:
+        print(err)
+        print("You must call earthaccess.login() before you can download data")
+        return []
     return results
 
 
 def open(
     granules: Union[List[str], List[earthaccess.results.DataGranule]],
     provider: Optional[str] = None,
 ) -> List[AbstractFileSystem]:
```

### Comparing `earthaccess-0.5.2/earthaccess/auth.py` & `earthaccess-0.5.3/earthaccess/auth.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.2/earthaccess/css/iso_bootstrap4.0.0min.css` & `earthaccess-0.5.3/earthaccess/css/iso_bootstrap4.0.0min.css`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.2/earthaccess/daac.py` & `earthaccess-0.5.3/earthaccess/daac.py`

 * *Files identical despite different names*

### Comparing `earthaccess-0.5.2/earthaccess/formatters.py` & `earthaccess-0.5.3/earthaccess/formatters.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def _repr_granule_html(granule: Any) -> str:
     css_styles = _load_static_files()
     css_inline = f"""<div id="{uuid4()}" style="height: 0px; display: none">
             {''.join([f"<style>{style}</style>" for style in css_styles])}
             </div>"""
-    style = "max-height: 140px;"
+    style = "max-height: 120px;"
     dataviz_img = "".join(
         [
             f'<a href="{link}"><img style="{style}" src="{link}" alt="Data Preview"/></a>'
             for link in granule.dataviz_links()[0:2]
             if link.startswith("http")
         ]
     )
@@ -43,15 +43,15 @@
     {css_inline}
     <div class="bootstrap">
       <div class="container-fluid border">
         <div class="row border">
           <div class="col-6">
             <p><b>Data</b>: {data_links}<p/>
             <p><b>Size</b>: {granule_size} MB</p>
-            <p><b>Spatial</b>: <span>{granule["umm"]["SpatialExtent"]}</span></p>
+            <p><b>Cloud Hosted</b>: <span>{granule.cloud_hosted}</span></p>
           </div>
           <div class="col-2 offset-sm-3 pull-right">
             {dataviz_img}
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -3,17 +3,17 @@
 _load_static_files() -> List[str]: """Load styles""" return
 [ pkg_resources.resource_string("earthaccess", fname).decode("utf8") for fname
 in STATIC_FILES ] def _repr_collection_html() -> str: return "
 " def _repr_granule_html(granule: Any) -> str: css_styles = _load_static_files
 () css_inline = f"""
 {''.join([f"
 " for style in css_styles])}
-""" style = "max-height: 140px;" dataviz_img = "".join( [ f'[Data_Preview]' for
+""" style = "max-height: 120px;" dataviz_img = "".join( [ f'[Data_Preview]' for
 link in granule.dataviz_links()[0:2] if link.startswith("http") ] ) data_links
 = "".join( [ f'{link.split("/")[-1]}' for link in granule.data_links() ] )
 granule_size = round(granule.size(), 2) # TODO: probably this needs to be
 integrated on a list data structure granule_str = f""" {css_inline}
 Data: {data_links}
 Size: {granule_size} MB
-Spatial: {granule["umm"]["SpatialExtent"]}
+Cloud Hosted: {granule.cloud_hosted}
 {dataviz_img}
 """ return granule_str
```

### Comparing `earthaccess-0.5.2/earthaccess/results.py` & `earthaccess-0.5.3/earthaccess/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,25 +243,25 @@
 
     def size(self) -> float:
         """
         Returns:
             Returns the total size for the granule in MB
         """
         try:
-            data_granule = self["mmm"]["DataGranule"]
+            data_granule = self["umm"]["DataGranule"]
             total_size = sum(
                 [
                     float(s["Size"])
                     for s in data_granule["ArchiveAndDistributionInformation"]
                     if "ArchiveAndDistributionInformation" in data_granule
                 ]
             )
         except Exception:
             try:
-                data_granule = self["mmm"]["DataGranule"]
+                data_granule = self["umm"]["DataGranule"]
                 total_size = sum(
                     [
                         float(s["SizeInBytes"])
                         for s in data_granule["ArchiveAndDistributionInformation"]
                         if "ArchiveAndDistributionInformation" in data_granule
                     ]
                 ) / (1024 * 1024)
```

### Comparing `earthaccess-0.5.2/earthaccess/search.py` & `earthaccess-0.5.3/earthaccess/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -408,14 +408,32 @@
             provider = find_provider_by_shortname(
                 self.params["short_name"], cloud_hosted
             )
             if provider is not None:
                 self.params["provider"] = provider
         return self
 
+    def granule_name(self, granule_name: str) -> Type[CollectionQuery]:
+        """Find granules matching either granule ur or producer granule id,
+        queries using the readable_granule_name metadata field.
+
+        ???+ Tip
+            We can use wirldcards on a granule name to further refine our search
+            i.e. MODGRNLD.*.daily.*
+
+        Parameters:
+            granule_name (String): granule name (accepts wildcards)
+        """
+        if not isinstance(granule_name, str):
+            raise TypeError("granule_name must be of type string")
+
+        self.params["readable_granule_name"] = granule_name
+        self.params["options[readable_granule_name][pattern]"] = True
+        return self
+
     def online_only(self, online_only: bool = True) -> Type[GranuleQuery]:
         """Only match granules that are listed online and not available for download.
         The opposite of this method is downloadable().
         Parameters:
             online_only (Boolean): True to require granules only be online
         """
         super().online_only(online_only)
@@ -659,7 +677,27 @@
         method is online_only().
 
         Parameters:
             downloadable: True to require granules be downloadable
         """
         super().downloadable(downloadable)
         return self
+
+    def doi(self, doi: str) -> Type[GranuleQuery]:
+        """Searh data granules by DOI
+
+        ???+ Tip
+            Not all datasets have an associated DOI, internally if a DOI is found
+            earthaccess will grab the concept_id for the query to CMR.
+
+        Parameters:
+            doi (String): DOI of a datasets, e.g. 10.5067/AQR50-3Q7CS
+        """
+        collection = DataCollections().doi(doi).get()
+        if len(collection) > 0:
+            concept_id = collection[0].concept_id()
+            self.params["concept_id"] = concept_id
+        else:
+            print(
+                f"earthaccess couldn't find any associated collections with the DOI: {doi}"
+            )
+        return self
```

### Comparing `earthaccess-0.5.2/earthaccess/store.py` & `earthaccess-0.5.3/earthaccess/store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,83 @@
 import datetime
 import os
 import shutil
 import traceback
 from copy import deepcopy
+from functools import lru_cache
 from itertools import chain
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 from uuid import uuid4
 
 import fsspec
 import requests
 import s3fs
 from multimethod import multimethod as singledispatchmethod
 from pqdm.threads import pqdm
 
+import earthaccess
+
 from .daac import DAAC_TEST_URLS, find_provider
 from .results import DataGranule
 from .search import DataCollections
 
 
+class EarthAccessFile(fsspec.spec.AbstractBufferedFile):
+    def __init__(self, f: fsspec.AbstractFileSystem, granule: DataGranule) -> None:
+        self.f = f
+        self.granule = granule
+
+    def __getattr__(self, method: str) -> Any:
+        return getattr(self.f, method)
+
+    def __reduce__(self) -> Any:
+        return make_instance, (
+            type(self.f),
+            self.f,
+            self.f.__reduce__(),
+        )
+
+    def __repr__(self) -> str:
+        return str(self.f)
+
+
+def _open_files(
+    data_links: List[str],
+    granules: Union[List[str], List[DataGranule]],
+    fs: fsspec.AbstractFileSystem,
+    threads: Optional[int] = 8,
+) -> List[fsspec.AbstractFileSystem]:
+    def multi_thread_open(data: tuple) -> EarthAccessFile:
+        urls, granule = data
+        if type(granule) is not str:
+            if len(granule.data_links()) > 1:
+                print(
+                    "Warning: This collection contains more than one file per granule. "
+                    "earthaccess will only open the first data link, "
+                    "try filtering the links before opening them."
+                )
+        return EarthAccessFile(fs.open(urls), granule)
+
+    fileset = pqdm(zip(data_links, granules), multi_thread_open, n_jobs=threads)
+    return fileset
+
+
+def make_instance(cls: Any, granule: DataGranule, _reduce: Any) -> EarthAccessFile:
+    if earthaccess.__store__.running_in_aws and cls is not s3fs.S3File:
+        # On AWS but not using a S3File. Reopen the file in this case for direct S3 access.
+        # NOTE: This uses the first data_link listed in the granule. That's not
+        #       guaranteed to be the right one.
+        return EarthAccessFile(earthaccess.open([granule])[0], granule)
+    else:
+        func = _reduce[0]
+        args = _reduce[1]
+        return func(*args)
+
+
 class Store(object):
     """
     Store class to access granules on-prem or in the cloud.
     """
 
     def __init__(self, auth: Any, pre_authorize: bool = False) -> None:
         """Store is the class to access data
@@ -107,14 +162,15 @@
             else:
                 self._requests_cookies.update(new_session.cookies.get_dict())
         elif resp.status_code >= 200 and resp.status_code <= 300:
             self._requests_cookies = self._http_session.cookies.get_dict()
         elif resp.status_code >= 500:
             resp.raise_for_status()
 
+    @lru_cache
     def get_s3fs_session(
         self,
         daac: Optional[str] = None,
         concept_id: Optional[str] = None,
         provider: Optional[str] = None,
     ) -> s3fs.S3FileSystem:
         """
@@ -122,14 +178,19 @@
 
         Parameters:
             daac: any of the DAACs e.g. NSIDC, PODAAC
         Returns:
             a s3fs file instance
         """
         if self.auth is not None:
+            if not any([concept_id, daac, provider]):
+                raise ValueError(
+                    "At least one of the concept_id, daac, or provider "
+                    "parameters must be specified. "
+                )
             if concept_id is not None:
                 provider = self._derive_concept_provider(concept_id)
                 s3_credentials = self.auth.get_s3_credentials(provider=provider)
             elif daac is not None:
                 s3_credentials = self.auth.get_s3_credentials(daac=daac)
             elif provider is not None:
                 s3_credentials = self.auth.get_s3_credentials(provider=provider)
@@ -149,25 +210,28 @@
             return deepcopy(self.s3_fs)
         else:
             print(
                 "A valid Earthdata login instance is required to retrieve S3 credentials"
             )
             return None
 
+    @lru_cache
     def get_fsspec_session(self) -> fsspec.AbstractFileSystem:
         """Returns a fsspec HTTPS session with bearer tokens that are used by CMR.
         This HTTPS session can be used to download granules if we want to use a direct, lower level API
 
         Returns:
             fsspec HTTPFileSystem (aiohttp client session)
         """
         token = self.auth.token["access_token"]
         client_kwargs = {
             "headers": {"Authorization": f"Bearer {token}"},
-            "trust_env": True,
+            # This is important! if we trust the env end send a bearer token
+            # auth will fail!
+            "trust_env": False,
         }
         session = fsspec.filesystem("https", client_kwargs=client_kwargs)
         return session
 
     def get_requests_session(self, bearer_token: bool = True) -> requests.Session:
         """Returns a requests HTTPS session with bearer tokens that are used by CMR.
         This HTTPS session can be used to download granules if we want to use a direct, lower level API
@@ -215,14 +279,15 @@
         raise NotImplementedError("granules should be a list of DataGranule or URLs")
 
     @_open.register
     def _open_granules(
         self,
         granules: List[DataGranule],
         provider: Optional[str] = None,
+        threads: Optional[int] = 8,
     ) -> Union[List[Any], None]:
         fileset: List = []
         data_links: List = []
         total_size = round(sum([granule.size() for granule in granules]) / 1024, 2)
         print(f" Opening {len(granules)} granules, approx size: {total_size} GB")
 
         if self.auth is None:
@@ -244,45 +309,46 @@
                 chain.from_iterable(
                     granule.data_links(access=access_method) for granule in granules
                 )
             )
 
             if s3_fs is not None:
                 try:
-
-                    def multi_thread_open(url: str) -> Any:
-                        return s3_fs.open(url)
-
-                    fileset = pqdm(data_links, multi_thread_open, n_jobs=8)
-
+                    fileset = _open_files(
+                        data_links=data_links,
+                        granules=granules,
+                        fs=s3_fs,
+                        threads=threads,
+                    )
                 except Exception:
                     print(
                         "An exception occurred while trying to access remote files on S3: "
                         "This may be caused by trying to access the data outside the us-west-2 region"
                         f"Exception: {traceback.format_exc()}"
                     )
                     return None
             else:
-                fileset = self._open_urls_https(data_links, n_jobs=8)
+                fileset = self._open_urls_https(data_links, granules, threads=threads)
             return fileset
         else:
             access_method = "on_prem"
             data_links = list(
                 chain.from_iterable(
                     granule.data_links(access=access_method) for granule in granules
                 )
             )
-            fileset = self._open_urls_https(data_links, n_jobs=8)
+            fileset = self._open_urls_https(data_links, granules, threads=threads)
             return fileset
 
     @_open.register
     def _open_urls(
         self,
         granules: List[str],
         provider: Optional[str] = None,
+        threads: Optional[int] = 8,
     ) -> Union[List[Any], None]:
         fileset: List = []
         data_links: List = []
 
         if isinstance(granules[0], str) and (
             granules[0].startswith("s3") or granules[0].startswith("http")
         ):
@@ -301,19 +367,20 @@
             return None
 
         if self.running_in_aws and granules[0].startswith("s3"):
             if provider is not None:
                 s3_fs = self.get_s3fs_session(provider=provider)
                 if s3_fs is not None:
                     try:
-
-                        def multi_thread_open(url: str) -> Any:
-                            return s3_fs.open(url)
-
-                        fileset = pqdm(data_links, multi_thread_open, n_jobs=8)
+                        fileset = _open_files(
+                            data_links=data_links,
+                            granules=granules,
+                            fs=s3_fs,
+                            threads=threads,
+                        )
                     except Exception:
                         print(
                             "An exception occurred while trying to access remote files on S3: "
                             "This may be caused by trying to access the data outside the us-west-2 region"
                             f"Exception: {traceback.format_exc()}"
                         )
                         return None
@@ -327,15 +394,15 @@
                 return None
         else:
             if granules[0].startswith("s3"):
                 print(
                     "We cannot open S3 links when we are not in-region, try using HTTPS links"
                 )
                 return None
-            fileset = self._open_urls_https(data_links, 8)
+            fileset = self._open_urls_https(data_links, granules, 8)
             return fileset
 
     def get(
         self,
         granules: Union[List[DataGranule], List[str]],
         local_path: Optional[str] = None,
         provider: Optional[str] = None,
@@ -529,24 +596,22 @@
             self._download_file,
             n_jobs=threads,
             argument_type="args",
         )
         return results
 
     def _open_urls_https(
-        self, urls: List[str] = [], n_jobs: int = 8
+        self,
+        urls: List[str],
+        granules: Union[List[str], List[DataGranule]],
+        threads: Optional[int] = 8,
     ) -> List[fsspec.AbstractFileSystem]:
         https_fs = self.get_fsspec_session()
         if https_fs is not None:
             try:
-
-                def multi_thread_open(url: str) -> Any:
-                    return https_fs.open(url)
-
-                fileset = pqdm(urls, multi_thread_open, n_jobs=8)
-
+                fileset = _open_files(urls, granules, https_fs, threads)
             except Exception:
                 print(
                     "An exception occurred while trying to access remote files via HTTPS: "
                     f"Exception: {traceback.format_exc()}"
                 )
         return fileset
```

### Comparing `earthaccess-0.5.2/pyproject.toml` & `earthaccess-0.5.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [tool.poetry]
 name = "earthaccess"
-version = "0.5.2"
+version = "0.5.3"
 homepage = "https://github.com/nsidc/earthaccess"
 description = "Client library for NASA Earthdata APIs"
 authors = ["earthaccess contributors"]
 maintainers = [
-    "Luis Lopez <betolin@gmail.com>"
+    "Luis Lopez <betolin@gmail.com>",
+    "Joseph H. Kennedy <jhkennedy@alaska.edu>",
+    "Matt Fisher <mfisher87@gmail.com>"
 ]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Framework :: IPython",
     "Development Status :: 4 - Beta",
@@ -49,25 +51,26 @@
 pytest = ">=6.0"
 pytest-cov = ">=2.8"
 pytest-watch = ">=4.2"
 mkdocs = ">=1.2"
 mkdocs-material = ">=7.1,<9.0"
 markdown-callouts = ">=0.2.0"
 markdown-include = ">=0.6"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocstrings = {extras = ["python"], version = ">=0.19.0"}
 mkdocs-jupyter = ">=0.19.0"
 pymdown-extensions = ">=9.2"
 pygments = ">=2.11.1"
 responses = ">=0.14"
 types-requests = ">=0.1"
 types-setuptools = ">=0.1"
 ipywidgets = ">=7.7.0"
 widgetsnbextension = ">=3.6.0"
 # for notebook integrations and documentation examples
 xarray = ">=2023.01"
 matplotlib = ">=3.3"
 h5netcdf = ">=0.11"
 dask = ">=2022.1"
+pyproj = ">=3.5.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `earthaccess-0.5.2/PKG-INFO` & `earthaccess-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthaccess
-Version: 0.5.2
+Version: 0.5.3
 Summary: Client library for NASA Earthdata APIs
 Home-page: https://github.com/nsidc/earthaccess
 License: MIT
 Author: earthaccess contributors
 Maintainer: Luis Lopez
 Maintainer-email: betolin@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -17,18 +17,14 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: fsspec (>=2022.1)
 Requires-Dist: multimethod (>=1.8)
 Requires-Dist: pqdm (>=0.1)
 Requires-Dist: python-cmr (>=0.7)
 Requires-Dist: requests (>=2.26,<3.0.0)
@@ -42,19 +38,23 @@
 
 <p align="center">
 
 <a href="https://twitter.com/allison_horst" target="_blank">
     <img src="https://img.shields.io/badge/Art%20By-Allison%20Horst-blue" alt="Art Designer: Allison Horst">
 </a>
 
-<a href="https://pypi.org/project/earthdata" target="_blank">
+<a href="https://pypi.org/project/earthaccess" target="_blank">
     <img src="https://img.shields.io/pypi/v/earthaccess?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 
-<a href="https://pypi.org/project/earthdata/" target="_blank">
+<a href="https://anaconda.org/conda-forge/earthaccess" target="_blank">
+    <img src="https://img.shields.io/conda/vn/conda-forge/earthaccess.svg" alt="Conda Versions">
+</a>
+
+<a href="https://pypi.org/project/earthaccess/" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/earthaccess.svg" alt="Python Versions">
 </a>
 
 <a href='https://earthdata.readthedocs.io/en/latest/?badge=latest'>
     <img src='https://readthedocs.org/projects/earthdata/badge/?version=latest' alt='Documentation Status' />
 </a>
 
@@ -128,20 +128,19 @@
 
 Once we have selected our dataset we can search for the data granules using *doi*, *short_name* or *concept_id*.
 If we are not sure or we don't know how to search for a particular dataset, we can start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the [NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a complete list of search parameters we can use visit the extended [API documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
 
 ```python
 
 results = earthaccess.search_data(
-    short_name='ATL06',
-    version="005",
+    short_name='SEA_SURFACE_HEIGHT_ALT_GRIDS_L4_2SATS_5DAY_6THDEG_V_JPL2205',
     cloud_hosted=True,
     bounding_box=(-10, 20, 10, 50),
-    temporal=("2020-02", "2020-03"),
-    count=100
+    temporal=("1999-02", "2019-03"),
+    count=10
 )
 
 
 ```
 
 Now that we have our results we can do multiple things: We can iterate over them to get HTTP (or S3) links, we can download the files to a local folder, or we can open these files and stream their content directly to other libraries e.g. xarray.
 
@@ -174,15 +173,17 @@
 **Option 3: Direct S3 Access - Stream data directly to xarray**
 
 This method works best if you are in the same Amazon Web Services (AWS) region as the data (us-west-2) and you are working with gridded datasets (processing level 3 and above).
 
 ```python
 import xarray as xr
 
-ds = xr.open_mfdataset(earthaccess.open(results))
+files = earthaccess.open(results)
+
+ds = xr.open_mfdataset(files)
 
 ```
 
 And that's it! Just one line of code, and this same piece of code will also work for data that are not hosted in the cloud, i.e. located at NASA storage centers.
 
 
 > More examples coming soon!
```

#### html2text {}

```diff
@@ -1,31 +1,28 @@
-Metadata-Version: 2.1 Name: earthaccess Version: 0.5.2 Summary: Client library
+Metadata-Version: 2.1 Name: earthaccess Version: 0.5.3 Summary: Client library
 for NASA Earthdata APIs Home-page: https://github.com/nsidc/earthaccess
 License: MIT Author: earthaccess contributors Maintainer: Luis Lopez
 Maintainer-email: betolin@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Framework :: IPython Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: MacOS Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Topic :: Software Development Classifier:
-Topic :: Software Development :: Libraries Requires-Dist: fsspec (>=2022.1)
-Requires-Dist: multimethod (>=1.8) Requires-Dist: pqdm (>=0.1) Requires-Dist:
-python-cmr (>=0.7) Requires-Dist: requests (>=2.26,<3.0.0) Requires-Dist: s3fs
-(>=2021.11,<2024) Requires-Dist: tinynetrc (>=1.3.1,<2.0.0) Description-
-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: fsspec (>=2022.1) Requires-Dist: multimethod (>=1.8) Requires-
+Dist: pqdm (>=0.1) Requires-Dist: python-cmr (>=0.7) Requires-Dist: requests
+(>=2.26,<3.0.0) Requires-Dist: s3fs (>=2021.11,<2024) Requires-Dist: tinynetrc
+(>=1.3.1,<2.0.0) Description-Content-Type: text/markdown
 [earthaccess, a python library to search, download or stream NASA Earth science
                       data with just a few lines of code]
-      [Art_Designer:_Allison_Horst] [Package_version] [Python_Versions]
-                            [Documentation_Status]
+   [Art_Designer:_Allison_Horst] [Package_version] [Conda_Versions] [Python
+                       Versions] [Documentation_Status]
 ## **Overview** *earthaccess* is a **python library to search, download or
 stream NASA Earth science data** with just a few lines of code. In the age of
 cloud computing, the power of open science only reaches its full potential if
 we have easy-to-use workflows that facilitate research in an inclusive,
 efficient and reproducible way. Unfortunately âas it stands todayâ
 scientists and students alike face a steep learning curve adapting to systems
 that have grown too complex and end up spending more time on the technicalities
@@ -67,45 +64,46 @@
 search for the data granules using *doi*, *short_name* or *concept_id*. If we
 are not sure or we don't know how to search for a particular dataset, we can
 start with the ["Introducing NASA earthaccess"](https://nsidc.github.io/
 earthaccess/tutorials/demo/#querying-for-datasets) tutorial or through the
 [NASA Earthdata Search portal](https://search.earthdata.nasa.gov/). For a
 complete list of search parameters we can use visit the extended [API
 documentation](https://nsidc.github.io/earthaccess/user-reference/api/api/).
-```python results = earthaccess.search_data( short_name='ATL06', version="005",
-cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("2020-02", "2020-
-03"), count=100 ) ``` Now that we have our results we can do multiple things:
-We can iterate over them to get HTTP (or S3) links, we can download the files
-to a local folder, or we can open these files and stream their content directly
-to other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using
-the data links** If we already have a workflow in place for downloading our
-data, we can use *earthaccess* as a search-only library and get HTTP links from
-our query results. This could be the case if our current workflow uses a
-different language and we only need the links as input. ```python # if the data
-set is cloud hosted there will be S3 links available. The access parameter
-accepts "direct" or "external", direct access is only possible if you are in
-the us-west-2 region in the cloud. data_links = [granule.data_links
-(access="direct") for granule in results] # or if the data is an on-prem
-dataset data_links = [granule.data_links(access="external") for granule in
-results] ``` > Note: *earthaccess* can get S3 credentials for us, or
-auhenticated HTTP sessions in case we want to use them with a different
-library. **Option 2: Download data to a local folder** This option is practical
-if you have the necessary space available on disk. The *earthaccess* library
-will print out the approximate size of the download and its progress. ```python
-files = earthaccess.download(results, "./local_folder") ``` **Option 3: Direct
-S3 Access - Stream data directly to xarray** This method works best if you are
-in the same Amazon Web Services (AWS) region as the data (us-west-2) and you
-are working with gridded datasets (processing level 3 and above). ```python
-import xarray as xr ds = xr.open_mfdataset(earthaccess.open(results)) ``` And
-that's it! Just one line of code, and this same piece of code will also work
-for data that are not hosted in the cloud, i.e. located at NASA storage
-centers. > More examples coming soon! ### Compatibility Only **Python 3.8+** is
-supported. ## Contributors [![Contributors](https://contrib.rocks/
-image?repo=nsidc/earthaccess)](https://github.com/nsidc/earthaccess/graphs/
-contributors) ## Contributing Guide Welcome! ðð > Please see the
-[Contributing Guide](CONTRIBUTING.md). ### [Project Board](https://github.com/
-nsidc/earthdata/discussions). ### Glossary NASA_Earth_Science_Glossary ##
-License earthaccess is licensed under the MIT license. See [LICENSE]
-(LICENSE.txt). ## Level of Support
+```python results = earthaccess.search_data
+( short_name='SEA_SURFACE_HEIGHT_ALT_GRIDS_L4_2SATS_5DAY_6THDEG_V_JPL2205',
+cloud_hosted=True, bounding_box=(-10, 20, 10, 50), temporal=("1999-02", "2019-
+03"), count=10 ) ``` Now that we have our results we can do multiple things: We
+can iterate over them to get HTTP (or S3) links, we can download the files to a
+local folder, or we can open these files and stream their content directly to
+other libraries e.g. xarray. ### **Accessing the data** **Option 1: Using the
+data links** If we already have a workflow in place for downloading our data,
+we can use *earthaccess* as a search-only library and get HTTP links from our
+query results. This could be the case if our current workflow uses a different
+language and we only need the links as input. ```python # if the data set is
+cloud hosted there will be S3 links available. The access parameter accepts
+"direct" or "external", direct access is only possible if you are in the us-
+west-2 region in the cloud. data_links = [granule.data_links(access="direct")
+for granule in results] # or if the data is an on-prem dataset data_links =
+[granule.data_links(access="external") for granule in results] ``` > Note:
+*earthaccess* can get S3 credentials for us, or auhenticated HTTP sessions in
+case we want to use them with a different library. **Option 2: Download data to
+a local folder** This option is practical if you have the necessary space
+available on disk. The *earthaccess* library will print out the approximate
+size of the download and its progress. ```python files = earthaccess.download
+(results, "./local_folder") ``` **Option 3: Direct S3 Access - Stream data
+directly to xarray** This method works best if you are in the same Amazon Web
+Services (AWS) region as the data (us-west-2) and you are working with gridded
+datasets (processing level 3 and above). ```python import xarray as xr files =
+earthaccess.open(results) ds = xr.open_mfdataset(files) ``` And that's it! Just
+one line of code, and this same piece of code will also work for data that are
+not hosted in the cloud, i.e. located at NASA storage centers. > More examples
+coming soon! ### Compatibility Only **Python 3.8+** is supported. ##
+Contributors [![Contributors](https://contrib.rocks/image?repo=nsidc/
+earthaccess)](https://github.com/nsidc/earthaccess/graphs/contributors) ##
+Contributing Guide Welcome! ðð > Please see the [Contributing Guide]
+(CONTRIBUTING.md). ### [Project Board](https://github.com/nsidc/earthdata/
+discussions). ### Glossary NASA_Earth_Science_Glossary ## License earthaccess
+is licensed under the MIT license. See [LICENSE](LICENSE.txt). ## Level of
+Support
 [https://raw.githubusercontent.com/nsidc/earthdata/main/docs/nsidc-logo.png]
 This repository is not actively supported by NSIDC but we welcome issue
 submissions and pull requests in order to foster community contribution.
```

