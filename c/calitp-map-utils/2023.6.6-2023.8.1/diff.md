# Comparing `tmp/calitp_map_utils-2023.6.6.tar.gz` & `tmp/calitp_map_utils-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.6.6.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.8.1.tar", max compression
```

## Comparing `calitp_map_utils-2023.6.6.tar` & `calitp_map_utils-2023.8.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2387 2023-06-05 15:29:19.429177 calitp_map_utils-2023.6.6/README.md
--rw-r--r--   0        0        0     5047 2023-06-05 18:36:05.513720 calitp_map_utils-2023.6.6/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-06-05 15:00:29.259950 calitp_map_utils-2023.6.6/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1441 2023-06-05 15:00:29.260623 calitp_map_utils-2023.6.6/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      645 2023-06-06 14:00:47.375690 calitp_map_utils-2023.6.6/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 calitp_map_utils-2023.6.6/PKG-INFO
+-rw-r--r--   0        0        0     3674 2023-07-24 19:16:34.269930 calitp_map_utils-2023.8.1/README.md
+-rw-r--r--   0        0        0     5113 2023-07-31 15:40:25.453826 calitp_map_utils-2023.8.1/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-26 17:16:54.925708 calitp_map_utils-2023.8.1/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2023-06-26 17:16:54.926512 calitp_map_utils-2023.8.1/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      637 2023-08-01 21:43:12.769889 calitp_map_utils-2023.8.1/pyproject.toml
+-rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 calitp_map_utils-2023.8.1/PKG-INFO
```

### Comparing `calitp_map_utils-2023.6.6/README.md` & `calitp_map_utils-2023.8.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -4,28 +4,47 @@
 in Jupyter notebooks, especially those built into static websites using JupyterBook. By using `IFrame` widgets to
 call the deployed application with a specific URL containing the desired state, a Jupyter user can render geospatial
 data that has been stored in GCS. This avoids the problem of `ipyleaflet` and other Jupyter visualization widgets
 that store their data in the static HTML of a rendered JupyterBook webpage. The Python code in `calitp_map_utils`
 defines the contract between data producers (i.e. notebooks) and the data consumer (i.e. the Svelte app) as well
 as provides some utilities for validating the GeoJSON of specific analysis types.
 
-## Developing
+## calitp_map_utils
+
+As mentioned above, `calitp_map_utils` is a small utility library that defines Pydantic types that can be used for
+data validation as well as Typescript types for type-hinting in the Svelte app. Also, the library contains
+a few CLI commands to facilitate validating pre-existing data with those types and/or generate a quick URL
+with state for testing.
+
+TODO: a GitHub Action workflow exists to build the package, but it does not currently publish to pypi; right now
+that is done manually with `poetry publish`.
+
+## Developing the maps app
 
 You can run a development server locally; use the calitp-map-utils CLI to generate a valid state URL for testing.
 
 ```bash
 npm run dev
 echo '{ "legend_url": "https://storage.googleapis.com/calitp-map-tiles/legend_test.svg", "layers": [ {"name": "D7 State Highway Network", "url": "https://storage.googleapis.com/calitp-map-tiles/d7_shn.geojson.gz", "type": "state_highway_network"}, {"name": "California High Quality Transit Areas - Stops", "url": "https://storage.googleapis.com/calitp-map-tiles/ca_hq_transit_stops.geojson.gz"}, {"name": "LA Metro Bus Speed Maps AM Peak", "url": "https://storage.googleapis.com/calitp-map-tiles/metro_am.geojson.gz", "type": "speedmap"} ] }' | gzip | basenc --base64url | poetry run python -m calitp_map_utils validate-state --base64url --compressed --data --verbose --host=http://localhost:5173
 ...
 URL: localhost:5173?state=H4sIAO38fWQC_6WSMU_DMBCF_8opM03GSt0KDAwUgcqGkHVNr47B8RnfhZJW_e8kbVE6FAY6WSef3_fek7dZwJqyCYTG-yvIPLaUpJtftj832e0Y5opKcOdstcYWHkjXnN6zbr9Jvl-pVKNMikKUE1rKLbP1hNFJXnJdlOidxlGNcaTOkxTLsZEq5Jb4Tbg7N72WtnHPkx5mqgPMhAEWE0dK6kiOhndXMNi86SArTsHh3ig8NT21heeEQZzCNBEKjLosHOUC7yWa6sPoQdVIr3Y-yLHSv13fT2FGmhiuG4F5JFrCDKPAdAaPhJd0XPeyBuvfWu5Z3fb5Yl_3f0GN5zAk2TDXw7RY8NfJhEKdmik5rJw9-VBkKSzNPzMcXyuJ5vJps9039EE5DrACAAA%3D
 ```
 
+You can point the `--host` parameter at a Netlify URL to provide an easy way to test against an already-published version of the app. As of 2023-07-21
+the production URL is [https://embeddable-maps.calitp.org](https://embeddable-maps.calitp.org) but you can also use preview
+Netlify sites deployed via `netlify deploy ...` with `--alias=some-alias` and/or without the `--prod` flag (see below).
+
 ## Build and deploy to Netlify
 
-To create a production version of your app:
+The site is deployed to production on merges to main, as defined in [../../.github/workflows/deploy-apps-maps.yml](../../.github/workflows/deploy-apps-maps.yml).
 
+You may also deploy manually with the following:
 ```bash
+(from the apps/maps folder)
 npm run build
-netlify deploy --site=cal-itp-data-analyses --dir=build --alias=leaflet-speedmaps
+netlify deploy --site=embeddable-maps-calitp-org --dir=build
 ```
 
+By default, this deploys a preview site with a generated alias prefix. You may pass an explicit alias with `--alias=<some-alias>`
+or deploy to production with `--prod`.
+
 We could look into using the [Netlify adapter](https://kit.svelte.dev/docs/adapter-netlify) at some point.
```

### Comparing `calitp_map_utils-2023.6.6/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.8.1/calitp_map_utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import base64
 import gzip
 import json
 import os
 from enum import Enum
 from typing import Any, Dict, Optional, Tuple, Union
 
+import gcsfs
 import requests
 import typer
-from calitp_data.storage import get_fs  # type: ignore
 from furl import furl
 from geojson_pydantic import Feature, FeatureCollection, MultiPolygon, Point, Polygon
 from geojson_pydantic.geometries import Geometry
 from geojson_pydantic.types import Position
 from pydantic import BaseModel, Field, HttpUrl, ValidationError, conlist, root_validator
 from tqdm import tqdm
 
 MAP_APP_URL_ENV_VAR = "CALITP_MAP_APP_URL"
 MAP_APP_URL = os.getenv(MAP_APP_URL_ENV_VAR)
 
 
 class LayerType(str, Enum):  # name?
     speedmaps = "speedmap"
+    speed_variation = "speed_variation"
     hqta_areas = "hqta_areas"
     hqta_stops = "hqta_stops"
     state_highway_network = "state_highway_network"
 
 
 class Tooltip(BaseModel):
     html: str
@@ -53,14 +54,15 @@
     agency_name_primary: str
     agency_name_secondary: Optional[str]
 
 
 # Dict Props just mean properties are an arbitrary dictionary
 LAYER_FEATURE_TYPES = {
     LayerType.speedmaps: Feature[Polygon, Speedmap],
+    LayerType.speed_variation: Feature[Polygon, Dict],
     LayerType.hqta_areas: Feature[Union[Polygon, MultiPolygon], HQTA],
     LayerType.hqta_stops: Feature[Point, HQTA],
     LayerType.state_highway_network: Feature[Union[Polygon, MultiPolygon], Dict],
 }
 
 
 def validate_geojson(
@@ -74,15 +76,15 @@
     if path.startswith("https://"):
         resp = requests.get(path)
         resp.raise_for_status()
         d = json.loads(
             gzip.decompress(resp.content).decode() if is_compressed else resp.text
         )
     else:
-        openf = get_fs().open if path.startswith("gs://") else open
+        openf = gcsfs.GCSFileSystem().open if path.startswith("gs://") else open
 
         with openf(path, "rb" if is_compressed else "r") as f:
             if is_compressed:
                 f = gzip.GzipFile(fileobj=f)
             d = json.load(f)
 
     collection = FeatureCollection(**d)
```

### Comparing `calitp_map_utils-2023.6.6/calitp_map_utils/cli.py` & `calitp_map_utils-2023.8.1/calitp_map_utils/cli.py`

 * *Files identical despite different names*

