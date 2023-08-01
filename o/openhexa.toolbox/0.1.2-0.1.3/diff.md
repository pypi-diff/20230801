# Comparing `tmp/openhexa.toolbox-0.1.2.tar.gz` & `tmp/openhexa.toolbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhexa.toolbox-0.1.2.tar", last modified: Thu Jul 13 11:43:25 2023, max compression
+gzip compressed data, was "openhexa.toolbox-0.1.3.tar", last modified: Tue Aug  1 10:50:16 2023, max compression
```

## Comparing `openhexa.toolbox-0.1.2.tar` & `openhexa.toolbox-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/toolbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29915 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/dhis2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/periods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 11:43:25.000000 openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-13 11:43:00.000000 openhexa.toolbox-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 11:43:25.041154 openhexa.toolbox-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/dhis2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/periods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-01 10:50:16.000000 openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:50:16.657501 openhexa.toolbox-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-01 10:49:43.000000 openhexa.toolbox-0.1.3/tests/test_lib.py
```

### Comparing `openhexa.toolbox-0.1.2/LICENSE` & `openhexa.toolbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openhexa.toolbox-0.1.2/PKG-INFO` & `openhexa.toolbox-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/api.py` & `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,15 @@
     @staticmethod
     def raise_if_error(response: requests.Response):
         """Raise DHIS2Error with message provided by API."""
         # raise DHIS2 error if error message is provided
         if response.status_code != 200 and "json" in response.headers["content-type"]:
             msg = response.json()
             if msg.get("status") == "ERROR":
-                raise DHIS2Error(
-                    f"{msg.get('status')} {msg.get('httpStatusCode')}:"
-                    f" {msg.get('message')}"
-                )
+                raise DHIS2Error(f"{msg.get('status')} {msg.get('httpStatusCode')}:" f" {msg.get('message')}")
 
         # raise with requests if no error message provided
         response.raise_for_status()
 
     def authenticate(self, username: str, password: str) -> requests.Session():
         """Authentify using Basic Authentication."""
         s = requests.Session()
@@ -70,17 +67,15 @@
         return s
 
     def get(self, endpoint: str, params: dict = None) -> requests.Response:
         r = self.session.get(f"{self.url}/{endpoint}", params=params)
         self.raise_if_error(r)
         return r
 
-    def get_paged(
-        self, endpoint: str, params: dict = None, page_size: 1000 = None
-    ) -> Iterable[requests.Response]:
+    def get_paged(self, endpoint: str, params: dict = None, page_size: 1000 = None) -> Iterable[requests.Response]:
         """Iterate over all response pages."""
         if params is None:
             params = {}
         params["pageSize"] = page_size
 
         r = self.session.get(f"{self.url}/{endpoint}", params=params)
         self.raise_if_error(r)
```

### Comparing `openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/dhis2.py` & `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/dhis2.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,15 @@
             for ou in page["organisationUnits"]:
                 org_units.append(
                     {
                         "id": ou.get("id"),
                         "name": ou.get("name"),
                         "level": ou.get("level"),
                         "path": ou.get("path"),
-                        "geometry": json.dumps(ou.get("geometry"))
-                        if ou.get("geometry")
-                        else None,
+                        "geometry": json.dumps(ou.get("geometry")) if ou.get("geometry") else None,
                     }
                 )
         return org_units
 
     @staticmethod
     def add_parent_organisation_units(org_unit_id: str) -> pl.DataFrame:
         """Add full org unit hierarchy columns.
@@ -156,17 +154,15 @@
         ):
             groups = []
             for group in page.json().get("organisationUnitGroups"):
                 groups.append(
                     {
                         "id": group.get("id"),
                         "name": group.get("name"),
-                        "organisation_units": [
-                            ou.get("id") for ou in group["organisationUnits"]
-                        ],
+                        "organisation_units": [ou.get("id") for ou in group["organisationUnits"]],
                     }
                 )
             org_unit_groups += groups
         return groups
 
     @use_cache("datasets")
     def datasets(self) -> List[dict]:
@@ -183,17 +179,15 @@
             params={
                 "fields": "id,name,dataSetElements,indicators,organisationUnits",
                 "pageSize": 10,
             },
         ):
             for ds in page.json()["dataSets"]:
                 row = {"id": ds.get("id"), "name": ds.get("name")}
-                row["data_elements"] = [
-                    dx["dataElement"]["id"] for dx in ds["dataSetElements"]
-                ]
+                row["data_elements"] = [dx["dataElement"]["id"] for dx in ds["dataSetElements"]]
                 row["indicators"] = [indicator["id"] for indicator in ds["indicators"]]
                 row["organisation_units"] = [ou["id"] for ou in ds["organisationUnits"]]
                 datasets.append(row)
         return datasets
 
     @use_cache("data_elements")
     def data_elements(self) -> List[dict]:
@@ -246,17 +240,15 @@
 
         Return
         ------
         list of dict
             Id and name of all category option combos.
         """
         combos = []
-        for page in self.client.api.get_paged(
-            "categoryOptionCombos", params={"fields": "id,name"}, page_size=1000
-        ):
+        for page in self.client.api.get_paged("categoryOptionCombos", params={"fields": "id,name"}, page_size=1000):
             combos += page.json().get("categoryOptionCombos")
         return combos
 
     @use_cache("indicators")
     def indicators(self) -> List[dict]:
         """Get indicators metadata.
 
@@ -457,34 +449,30 @@
             df = dataframe
 
         levels = pl.DataFrame(self.organisation_unit_levels())
         org_units = pl.DataFrame(self.organisation_units())
 
         for lvl in range(1, len(levels)):
             org_units = org_units.with_columns(
-                pl.col("path")
-                .apply(lambda path: self._get_uid_from_level(path, lvl))
-                .alias(f"parent_level_{lvl}_id")
+                pl.col("path").apply(lambda path: self._get_uid_from_level(path, lvl)).alias(f"parent_level_{lvl}_id")
             )
 
             org_units = org_units.join(
                 other=org_units.filter(pl.col("level") == lvl).select(
                     [
                         pl.col("id").alias(f"parent_level_{lvl}_id"),
                         pl.col("name").alias(f"parent_level_{lvl}_name"),
                     ]
                 ),
                 on=f"parent_level_{lvl}_id",
                 how="left",
             )
 
         df = df.join(
-            other=org_units.select(
-                ["id"] + [col for col in org_units.columns if col.startswith("parent_")]
-            ),
+            other=org_units.select(["id"] + [col for col in org_units.columns if col.startswith("parent_")]),
             how="left",
             left_on=org_unit_id_column,
             right_on="id",
         )
 
         if src_format == "pandas":
             df = df.to_pandas()
@@ -520,18 +508,15 @@
                 params_to_chunk.append((param, max_length))
 
         if not params_to_chunk:
             return [params]
 
         chunks = []
         for chunk in itertools.product(
-            *[
-                _split_list(params.get(param), max_length)
-                for param, max_length in params_to_chunk
-            ]
+            *[_split_list(params.get(param), max_length) for param, max_length in params_to_chunk]
         ):
             p = params.copy()
             for i, (param, _) in enumerate(params_to_chunk):
                 p[param] = chunk[i]
             chunks.append(p)
 
         return chunks
@@ -594,17 +579,15 @@
             raise DHIS2Error("No data dimension provided")
         if not where:
             raise DHIS2Error("No spatial dimension provided")
         if not when:
             raise DHIS2Error("No temporal dimension provided")
 
         if data_elements and not self.client.version >= 2.39:
-            raise DHIS2Error(
-                "Data elements parameter not supported for DHIS2 versions < 2.39"
-            )
+            raise DHIS2Error("Data elements parameter not supported for DHIS2 versions < 2.39")
 
         params = {
             "dataElement": data_elements,
             "dataSet": datasets,
             "dataElementGroup": data_element_groups,
             "period": periods,
             "startDate": start_date,
@@ -692,21 +675,16 @@
 
         dimension = params["dimension"]
 
         dim_chunks = []
         for dim in dimension:
             dim_id, dim_items = self.split_dimension_param(dim)
             if dim_id in MAX_DIM_ITEMS:
-                dim_item_chunks = [
-                    item
-                    for item in _split_list(dim_items, MAX_DIM_ITEMS.get(dim_id, 50))
-                ]
-                dim_item_chunks = [
-                    f"{dim_id}:{';'.join(dim_items)}" for dim_items in dim_item_chunks
-                ]
+                dim_item_chunks = [item for item in _split_list(dim_items, MAX_DIM_ITEMS.get(dim_id, 50))]
+                dim_item_chunks = [f"{dim_id}:{';'.join(dim_items)}" for dim_items in dim_item_chunks]
                 dim_chunks.append(dim_item_chunks)
             else:
                 dim_chunks.append([dim])
 
         param_chunks = []
         for chunk in itertools.product(*dim_chunks):
             param_chunk = params.copy()
```

### Comparing `openhexa.toolbox-0.1.2/openhexa/toolbox/dhis2/periods.py` & `openhexa.toolbox-0.1.3/openhexa/toolbox/dhis2/periods.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,19 +72,15 @@
 
     def __init__(self, period: Union[str, datetime]):
         super().__init__(period)
         self._delta = relativedelta(weeks=1)
 
     @staticmethod
     def check_period(period: str):
-        if (
-            (len(period) != 6 and len(period) != 7)
-            or period[4] != "W"
-            or period[5] == "0"
-        ):
+        if (len(period) != 6 and len(period) != 7) or period[4] != "W" or period[5] == "0":
             raise ValueError(f'"{period}" is not valid DHIS2 week')
 
     @staticmethod
     def to_datetime(period: str) -> datetime:
         return datetime.strptime(period, "%YW%W")
 
     @staticmethod
```

### Comparing `openhexa.toolbox-0.1.2/openhexa.toolbox.egg-info/PKG-INFO` & `openhexa.toolbox-0.1.3/openhexa.toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhexa.toolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of tools to acquire & process data from various sources
 Author-email: Bluesquare <dev@bluesquarehub.com>
 Maintainer-email: Bluesquare <dev@bluesquarehub.com>
 License: MIT License
         
         Copyright (c) 2023 Bluesquare
```

### Comparing `openhexa.toolbox-0.1.2/pyproject.toml` & `openhexa.toolbox-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openhexa.toolbox"
-version = "0.1.2"
+version = "0.1.3"
 description = "A set of tools to acquire & process data from various sources"
 authors = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com"}
 ]
 maintainers = [
     { name = "Bluesquare", email = "dev@bluesquarehub.com" }
 ]
@@ -25,22 +25,25 @@
     "python-dateutil",
     "pandas",
     "polars",
     "diskcache"
 ]
 
 [project.optional-dependencies]
-dev = ["pytest", "build"]
+dev = ["ruff~=0.0.278", "pytest~=7.3.0", "build~=0.10.0", "pytest-cov~=4.0.0" , "black~=23.7.0", "pre-commit"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = true
 
 [project.urls]
 "Homepage" = "https://github.com/blsq/openhexa-toolbox"
 "Bug Tracker" = "https://github.com/blsq/openhexa-toolbox/issues"
 
 [tool.black]
-line-length = 88
+line-length = 120
 
 [tool.ruff]
-line-length = 88
+line-length = 120
+
+[tool.ruff.pycodestyle]
+max-doc-length = 120
```

