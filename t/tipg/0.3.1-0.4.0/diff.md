# Comparing `tmp/tipg-0.3.1.tar.gz` & `tmp/tipg-0.4.0.tar.gz`

## Comparing `tipg-0.3.1.tar` & `tipg-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/__init__.py
--rw-r--r--   0        0        0    32496 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/collections.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/database.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/dependencies.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/errors.py
--rw-r--r--   0        0        0    73823 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/factory.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/logger.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/main.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/middleware.py
--rw-r--r--   0        0        0    20718 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/model.py
--rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/settings.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/__init__.py
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/evaluate.py
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/filter/filters.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/__init__.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/enums.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/resources/response.py
--rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/sql/dbcatalog.sql
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/collection.html
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/collections.html
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/conformance.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/debug.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/footer.html
--rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/header.html
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/item.html
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/items.html
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/landing.html
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/map.html
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/queryables.html
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilematrixset.html
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilematrixsets.html
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tileset.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.3.1/tipg/templates/tilesets.html
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.3.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.3.1/LICENSE
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.3.1/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 tipg-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 tipg-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/__init__.py
+-rw-r--r--   0        0        0    32580 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/collections.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/database.py
+-rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/dependencies.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/errors.py
+-rw-r--r--   0        0        0    73853 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/factory.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/logger.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/main.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/middleware.py
+-rw-r--r--   0        0        0    22734 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/model.py
+-rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/settings.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/filter/__init__.py
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/filter/evaluate.py
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/filter/filters.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/resources/__init__.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/resources/enums.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/resources/response.py
+-rw-r--r--   0        0        0     9679 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/sql/dbcatalog.sql
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/collection.html
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/collections.html
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/conformance.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/debug.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/footer.html
+-rw-r--r--   0        0        0    12152 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/header.html
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/item.html
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/items.html
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/landing.html
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/map.html
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/queryables.html
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/tilematrixset.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/tilematrixsets.html
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/tileset.html
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tipg-0.4.0/tipg/templates/tilesets.html
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 tipg-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tipg-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 tipg-0.4.0/README.md
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 tipg-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 tipg-0.4.0/PKG-INFO
```

### Comparing `tipg-0.3.1/tipg/collections.py` & `tipg-0.4.0/tipg/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from buildpg import RawDangerous as raw
 from buildpg import asyncpg, clauses
 from buildpg import funcs as pg_funcs
 from buildpg import logic, render
 from ciso8601 import parse_rfc3339
 from morecantile import Tile, TileMatrixSet
-from pydantic import BaseModel, Field, root_validator
+from pydantic import BaseModel, Field, model_validator
 from pygeofilter.ast import AstType
 
 from tipg.errors import (
     InvalidDatetime,
     InvalidDatetimeColumnName,
     InvalidGeometryColumnName,
     InvalidLimit,
@@ -85,22 +85,22 @@
 
 
 class Column(BaseModel):
     """Model for database Column."""
 
     name: str
     type: str
-    description: Optional[str]
-    geometry_type: Optional[str]
-    srid: Optional[int]
-    bounds: Optional[List[float]]
-    mindt: Optional[str]
-    maxdt: Optional[str]
+    description: Optional[str] = None
+    geometry_type: Optional[str] = None
+    srid: Optional[int] = None
+    bounds: Optional[List[float]] = None
+    mindt: Optional[str] = None
+    maxdt: Optional[str] = None
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
     def sridbounds_default(cls, values):
         """Set default bounds and srid when this is a function."""
         if values.get("geometry_type"):
             values["srid"] = values.get("srid", 4326)
             values["bounds"] = values.get("bounds", [-180, -90, 180, 90])
         return values
 
@@ -156,20 +156,20 @@
 class Collection(BaseModel):
     """Model for DB Table and Function."""
 
     type: str
     id: str
     table: str
     dbschema: str = Field(..., alias="schema")
-    title: Optional[str]
-    description: Optional[str]
+    title: Optional[str] = None
+    description: Optional[str] = None
     properties: List[Column] = []
-    id_column: Optional[str]
-    geometry_column: Optional[Column]
-    datetime_column: Optional[Column]
+    id_column: Optional[str] = None
+    geometry_column: Optional[Column] = None
+    datetime_column: Optional[Column] = None
     parameters: List[Parameter] = []
 
     @property
     def extent(self) -> Optional[Extent]:
         """Return extent."""
         extent: Dict[str, Any] = {}
         if cols := self.geometry_columns:
```

### Comparing `tipg-0.3.1/tipg/database.py` & `tipg-0.4.0/tipg/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     """Connect."""
     if not settings:
         settings = PostgresSettings()
 
     con_init = connection_factory(schemas, user_sql_files)
 
     app.state.pool = await asyncpg.create_pool_b(
-        settings.database_url,
+        str(settings.database_url),
         min_size=settings.db_min_conn_size,
         max_size=settings.db_max_conn_size,
         max_queries=settings.db_max_queries,
         max_inactive_connection_lifetime=settings.db_max_inactive_conn_lifetime,
         init=con_init,
         **kwargs,
     )
```

### Comparing `tipg-0.3.1/tipg/dependencies.py` & `tipg-0.4.0/tipg/dependencies.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """tipg dependencies."""
 
 import re
-import sys
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Literal, Optional, Tuple, get_args
 
 from morecantile import Tile
 from morecantile import tms as default_tms
 from pygeofilter.ast import AstType
 from pygeofilter.parsers.cql2_json import parse as cql2_json_parser
 from pygeofilter.parsers.cql2_text import parse as cql2_text_parser
+from typing_extensions import Annotated
 
 from tipg.collections import Catalog, Collection
 from tipg.errors import InvalidBBox, MissingCollectionCatalog, MissingFunctionParameter
-from tipg.resources import enums
+from tipg.resources.enums import MediaType
 from tipg.settings import TMSSettings
 
 from fastapi import Depends, HTTPException, Path, Query
 
 from starlette.requests import Request
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated  # pylint: disable=no-name-in-module
-else:
-    from typing_extensions import Annotated
-
-
 tms_settings = TMSSettings()
 
+ResponseType = Literal["json", "html"]
+QueryablesResponseType = Literal["schemajson", "html"]
+ItemsResponseType = Literal["geojson", "html", "json", "csv", "geojsonseq", "ndjson"]
+ItemResponseType = Literal["geojson", "html", "json"]
+VectorResponseType = Literal["geojson", "mvt"]
+VectorType = Literal["pbf", "mvt"]
+FilterLang = Literal["cql2-text", "cql2-json"]
+
 
 def CollectionParams(
     request: Request,
     collectionId: Annotated[str, Path(description="Collection identifier")],
 ) -> Collection:
     """Return Layer Object."""
     collection_pattern = re.match(  # type: ignore
@@ -61,17 +63,15 @@
     collection_catalog: Catalog = getattr(request.app.state, "collection_catalog", None)
     if not collection_catalog:
         raise MissingCollectionCatalog("Could not find collections catalog.")
 
     return collection_catalog
 
 
-def accept_media_type(
-    accept: str, mediatypes: List[enums.MediaType]
-) -> Optional[enums.MediaType]:
+def accept_media_type(accept: str, mediatypes: List[MediaType]) -> Optional[MediaType]:
     """Return MediaType based on accept header and available mediatype.
 
     Links:
     - https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html
     - https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept
 
     """
@@ -113,78 +113,76 @@
 
     return None
 
 
 def OutputType(
     request: Request,
     f: Annotated[
-        Optional[enums.ResponseType],
+        Optional[ResponseType],
         Query(
             description="Response MediaType. Defaults to endpoint's default or value defined in `accept` header."
         ),
     ] = None,
-) -> Optional[enums.MediaType]:
+) -> Optional[MediaType]:
     """Output MediaType: json or html."""
     if f:
-        return enums.MediaType[f.name]
+        return MediaType[f]
 
-    accepted_media = [enums.MediaType[v] for v in enums.ResponseType.__members__]
+    accepted_media = [MediaType[v] for v in get_args(ResponseType)]
     return accept_media_type(request.headers.get("accept", ""), accepted_media)
 
 
 def QueryablesOutputType(
     request: Request,
     f: Annotated[
-        Optional[enums.QueryablesResponseType],
+        Optional[QueryablesResponseType],
         Query(
             description="Response MediaType. Defaults to endpoint's default or value defined in `accept` header."
         ),
     ] = None,
-) -> Optional[enums.MediaType]:
+) -> Optional[MediaType]:
     """Output MediaType: schemajson or html."""
     if f:
-        return enums.MediaType[f.name]
+        return MediaType[f]
 
-    accepted_media = [
-        enums.MediaType[v] for v in enums.QueryablesResponseType.__members__
-    ]
+    accepted_media = [MediaType[v] for v in get_args(QueryablesResponseType)]
     return accept_media_type(request.headers.get("accept", ""), accepted_media)
 
 
 def ItemsOutputType(
     request: Request,
     f: Annotated[
-        Optional[enums.ItemsResponseType],
+        Optional[ItemsResponseType],
         Query(
             description="Response MediaType. Defaults to endpoint's default or value defined in `accept` header."
         ),
     ] = None,
-) -> Optional[enums.MediaType]:
+) -> Optional[MediaType]:
     """Output MediaType: geojson, html, json, csv, geojsonseq, ndjson."""
     if f:
-        return enums.MediaType[f.name]
+        return MediaType[f]
 
-    accepted_media = [enums.MediaType[v] for v in enums.ItemsResponseType.__members__]
+    accepted_media = [MediaType[v] for v in get_args(ItemsResponseType)]
     return accept_media_type(request.headers.get("accept", ""), accepted_media)
 
 
 def ItemOutputType(
     request: Request,
     f: Annotated[
-        Optional[enums.ItemResponseType],
+        Optional[ItemResponseType],
         Query(
             description="Response MediaType. Defaults to endpoint's default or value defined in `accept` header."
         ),
     ] = None,
-) -> Optional[enums.MediaType]:
+) -> Optional[MediaType]:
     """Output MediaType: geojson, json or html."""
     if f:
-        return enums.MediaType[f.name]
+        return MediaType[f]
 
-    accepted_media = [enums.MediaType[v] for v in enums.ItemResponseType.__members__]
+    accepted_media = [MediaType[v] for v in get_args(ItemResponseType)]
     return accept_media_type(request.headers.get("accept", ""), accepted_media)
 
 
 def bbox_query(
     bbox: Annotated[
         Optional[str],
         Query(description="Spatial Filter."),
@@ -279,24 +277,24 @@
 
 
 def filter_query(
     query: Annotated[
         Optional[str], Query(description="CQL2 Filter", alias="filter")
     ] = None,
     filter_lang: Annotated[
-        Optional[enums.FilterLang],
+        Optional[FilterLang],
         Query(
             description="CQL2 Language (cql2-text, cql2-json). Defaults to cql2-text.",
             alias="filter-lang",
         ),
     ] = None,
 ) -> Optional[AstType]:
     """Parse Filter Query."""
     if query is not None:
-        if filter_lang == enums.FilterLang.cql2_json:
+        if filter_lang == "cql2-json":
             return cql2_json_parser(query)
 
         # default to cql2-text
         return cql2_text_parser(query)
 
     return None
```

### Comparing `tipg-0.3.1/tipg/errors.py` & `tipg-0.4.0/tipg/errors.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/factory.py` & `tipg-0.4.0/tipg/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """tipg.factory: router factories."""
 
 import abc
 import csv
 import json
-import sys
 from dataclasses import dataclass, field
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
@@ -21,14 +20,15 @@
 import jinja2
 import orjson
 from ciso8601 import parse_rfc3339
 from morecantile import Tile, TileMatrixSet
 from morecantile import tms as default_tms
 from morecantile.defaults import TileMatrixSets
 from pygeofilter.ast import AstType
+from typing_extensions import Annotated
 
 from tipg import model
 from tipg.collections import Catalog, Collection
 from tipg.dependencies import (
     CatalogParams,
     CollectionParams,
     ItemsOutputType,
@@ -53,30 +53,50 @@
 from fastapi.responses import ORJSONResponse
 
 from starlette.datastructures import QueryParams
 from starlette.requests import Request
 from starlette.responses import HTMLResponse, Response, StreamingResponse
 from starlette.templating import Jinja2Templates, _TemplateResponse
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated  # pylint: disable=no-name-in-module
-else:
-    from typing_extensions import Annotated
-
-
 tms_settings = TMSSettings()
 mvt_settings = MVTSettings()
 features_settings = FeaturesSettings()
 
 DEFAULT_TEMPLATES = Jinja2Templates(
     directory="",
     loader=jinja2.ChoiceLoader([jinja2.PackageLoader(__package__, "templates")]),
 )  # type:ignore
 
 
+COMMON_CONFORMS = [
+    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/core",
+    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/landingPage",
+    "http://www.opengis.net/spec/ogcapi-common-2/1.0/conf/collections",
+    "http://www.opengis.net/spec/ogcapi-common-2/1.0/conf/simple-query",
+    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/json",
+    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/html",
+    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/oas30",
+]
+FEATURES_CONFORMS = [
+    "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core",
+    "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/html",
+    "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30",
+    "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson",
+    "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/filter",
+    "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/features-filter",
+]
+TILES_CONFORMS = [
+    "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/core",
+    "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/oas30",
+    "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/mvt",
+    "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/tileset",
+    "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/tilesets-list",
+]
+
+
 def create_csv_rows(data: Iterable[Dict]) -> Generator[str, None, None]:
     """Creates an iterator that returns lines of csv from an iterable of dicts."""
 
     class DummyWriter:
         """Dummy writer that implements write for use with csv.writer."""
 
         def write(self, line: str):
@@ -269,31 +289,20 @@
             tags=["OGC Common"],
         )
         def conformance(
             request: Request,
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
         ):
             """Get conformance."""
-            data = model.Conformance(
-                conformsTo=[
-                    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/core",
-                    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/landingPage",
-                    "http://www.opengis.net/spec/ogcapi-common-2/1.0/conf/collections",
-                    "http://www.opengis.net/spec/ogcapi-common-2/1.0/conf/simple-query",
-                    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/json",
-                    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/html",
-                    "http://www.opengis.net/spec/ogcapi-common-1/1.0/conf/oas30",
-                    *self.conforms_to,
-                ]
-            )
+            data = model.Conformance(conformsTo=[*COMMON_CONFORMS, *self.conforms_to])
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="conformance",
                 )
 
             return data
 
         @self.router.get(
             "/",
@@ -345,36 +354,29 @@
                     *self.links(request),
                 ],
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="landing",
                 )
 
             return data
 
 
 @dataclass
 class OGCFeaturesFactory(EndpointsFactory):
     """OGC Features Endpoints Factory."""
 
     @property
     def conforms_to(self) -> List[str]:
         """Factory conformances."""
-        return [
-            "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core",
-            "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/html",
-            "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30",
-            "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/geojson",
-            "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/filter",
-            "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/features-filter",
-        ]
+        return FEATURES_CONFORMS
 
     def links(self, request: Request) -> List[model.Link]:
         """OGC Features API links."""
         return [
             model.Link(
                 title="List of Collections",
                 href=self.url_for(request, "collections"),
@@ -520,15 +522,15 @@
                 url = self.url_for(request, "collections") + f"?{query_params}"
                 links.append(
                     model.Link(
                         href=url,
                         rel="next",
                         type=MediaType.json,
                         title="Next page",
-                    ).dict(exclude_none=True),
+                    ),
                 )
 
             if offset:
                 qp = dict(request.query_params)
                 qp.pop("offset")
                 prev_offset = max(offset - items_returned, 0)
                 if prev_offset:
@@ -542,67 +544,65 @@
 
                 links.append(
                     model.Link(
                         href=url,
                         rel="prev",
                         type=MediaType.json,
                         title="Previous page",
-                    ).dict(exclude_none=True),
+                    ),
                 )
 
             data = model.Collections(
                 links=links,
                 numberMatched=matched_items,
                 numberReturned=items_returned,
                 collections=[
                     model.Collection(
-                        **{
-                            "id": collection.id,
-                            "title": collection.id,
-                            "description": collection.description,
-                            "extent": collection.extent,
-                            "links": [
-                                model.Link(
-                                    href=self.url_for(
-                                        request,
-                                        "collection",
-                                        collectionId=collection.id,
-                                    ),
-                                    rel="collection",
-                                    type=MediaType.json,
+                        id=collection.id,
+                        title=collection.id,
+                        description=collection.description,
+                        extent=collection.extent,
+                        links=[
+                            model.Link(
+                                href=self.url_for(
+                                    request,
+                                    "collection",
+                                    collectionId=collection.id,
                                 ),
-                                model.Link(
-                                    href=self.url_for(
-                                        request,
-                                        "items",
-                                        collectionId=collection.id,
-                                    ),
-                                    rel="items",
-                                    type=MediaType.geojson,
+                                rel="collection",
+                                type=MediaType.json,
+                            ),
+                            model.Link(
+                                href=self.url_for(
+                                    request,
+                                    "items",
+                                    collectionId=collection.id,
                                 ),
-                                model.Link(
-                                    href=self.url_for(
-                                        request,
-                                        "queryables",
-                                        collectionId=collection.id,
-                                    ),
-                                    rel="queryables",
-                                    type=MediaType.schemajson,
+                                rel="items",
+                                type=MediaType.geojson,
+                            ),
+                            model.Link(
+                                href=self.url_for(
+                                    request,
+                                    "queryables",
+                                    collectionId=collection.id,
                                 ),
-                            ],
-                        }
+                                rel="queryables",
+                                type=MediaType.schemajson,
+                            ),
+                        ],
                     )
                     for collection in collections_list
                 ],
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="collections",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}",
@@ -621,73 +621,73 @@
         def collection(
             request: Request,
             collection: Annotated[Collection, Depends(self.collection_dependency)],
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
         ):
             """Metadata for a feature collection."""
 
-            data = model.Collection(
-                **{
-                    **collection.dict(),
+            data = model.Collection.model_validate(
+                {
+                    **collection.model_dump(),
                     "title": collection.id,
                     "extent": collection.extent,
                     "links": [
-                        model.Link(
-                            href=self.url_for(
+                        {
+                            "href": self.url_for(
                                 request,
                                 "collection",
                                 collectionId=collection.id,
                             ),
-                            rel="self",
-                            type=MediaType.json,
-                        ),
-                        model.Link(
-                            title="Items",
-                            href=self.url_for(
+                            "rel": "self",
+                            "type": "application/json",
+                        },
+                        {
+                            "title": "Items",
+                            "href": self.url_for(
                                 request, "items", collectionId=collection.id
                             ),
-                            rel="items",
-                            type=MediaType.geojson,
-                        ),
-                        model.Link(
-                            title="Items (CSV)",
-                            href=self.url_for(
+                            "rel": "items",
+                            "type": "application/geo+json",
+                        },
+                        {
+                            "title": "Items (CSV)",
+                            "href": self.url_for(
                                 request, "items", collectionId=collection.id
                             )
                             + "?f=csv",
-                            rel="alternate",
-                            type=MediaType.csv,
-                        ),
-                        model.Link(
-                            title="Items (GeoJSONSeq)",
-                            href=self.url_for(
+                            "rel": "alternate",
+                            "type": "text/csv",
+                        },
+                        {
+                            "title": "Items (GeoJSONSeq)",
+                            "href": self.url_for(
                                 request, "items", collectionId=collection.id
                             )
                             + "?f=geojsonseq",
-                            rel="alternate",
-                            type=MediaType.geojsonseq,
-                        ),
-                        model.Link(
-                            title="Queryables",
-                            href=self.url_for(
+                            "rel": "alternate",
+                            "type": "application/geo+json-seq",
+                        },
+                        {
+                            "title": "Queryables",
+                            "href": self.url_for(
                                 request,
                                 "queryables",
                                 collectionId=collection.id,
                             ),
-                            rel="queryables",
-                            type=MediaType.schemajson,
-                        ),
+                            "rel": "queryables",
+                            "type": "application/schema+json",
+                        },
                     ],
                 }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="collection",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/queryables",
@@ -712,30 +712,25 @@
             ] = None,
         ):
             """Queryables for a feature collection.
 
             ref: http://docs.ogc.org/DRAFTS/19-079r1.html#filter-queryables
             """
             qs = "?" + str(request.query_params) if request.query_params else ""
-
+            self_url = self.url_for(request, "queryables", collectionId=collection.id)
             data = model.Queryables(
-                **{
-                    "title": collection.id,
-                    "$id": self.url_for(
-                        request, "queryables", collectionId=collection.id
-                    )
-                    + qs,
-                    "properties": collection.queryables,
-                }
+                title=collection.id,
+                link=self_url + qs,
+                properties=collection.queryables,
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="queryables",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/items",
@@ -894,49 +889,49 @@
                         headers={
                             "Content-Disposition": "attachment;filename=items.ndjson"
                         },
                     )
 
             qs = "?" + str(request.query_params) if request.query_params else ""
             links: List[Dict] = [
-                model.Link(
-                    title="Collection",
-                    href=self.url_for(
+                {
+                    "title": "Collection",
+                    "href": self.url_for(
                         request, "collection", collectionId=collection.id
                     ),
-                    rel="collection",
-                    type=MediaType.json,
-                ).dict(exclude_none=True),
-                model.Link(
-                    title="Items",
-                    href=self.url_for(request, "items", collectionId=collection.id)
+                    "rel": "collection",
+                    "type": "application/json",
+                },
+                {
+                    "title": "Items",
+                    "href": self.url_for(request, "items", collectionId=collection.id)
                     + qs,
-                    rel="self",
-                    type=MediaType.geojson,
-                ).dict(exclude_none=True),
+                    "rel": "self",
+                    "type": "application/geo+json",
+                },
             ]
 
             items_returned = len(items["features"])
 
             if (matched_items - items_returned) > offset:
                 next_offset = offset + items_returned
                 query_params = QueryParams(
                     {**request.query_params, "offset": next_offset}
                 )
                 url = (
                     self.url_for(request, "items", collectionId=collection.id)
                     + f"?{query_params}"
                 )
                 links.append(
-                    model.Link(
-                        href=url,
-                        rel="next",
-                        type=MediaType.geojson,
-                        title="Next page",
-                    ).dict(exclude_none=True),
+                    {
+                        "href": url,
+                        "rel": "next",
+                        "type": "application/geo+json",
+                        "title": "Next page",
+                    },
                 )
 
             if offset:
                 qp = dict(request.query_params)
                 qp.pop("offset")
                 prev_offset = max(offset - items_returned, 0)
                 if prev_offset:
@@ -945,20 +940,20 @@
                     query_params = QueryParams({**qp})
 
                 url = self.url_for(request, "items", collectionId=collection.id)
                 if qp:
                     url += f"?{query_params}"
 
                 links.append(
-                    model.Link(
-                        href=url,
-                        rel="prev",
-                        type=MediaType.geojson,
-                        title="Previous page",
-                    ).dict(exclude_none=True),
+                    {
+                        "href": url,
+                        "rel": "prev",
+                        "type": "application/geo+json",
+                        "title": "Previous page",
+                    },
                 )
 
             data = {
                 "type": "FeatureCollection",
                 "id": collection.id,
                 "title": collection.title or collection.id,
                 "description": collection.description
@@ -967,35 +962,35 @@
                 "numberMatched": matched_items,
                 "numberReturned": items_returned,
                 "links": links,
                 "features": [
                     {
                         **feature,  # type: ignore
                         "links": [
-                            model.Link(
-                                title="Collection",
-                                href=self.url_for(
+                            {
+                                "title": "Collection",
+                                "href": self.url_for(
                                     request,
                                     "collection",
                                     collectionId=collection.id,
                                 ),
-                                rel="collection",
-                                type=MediaType.json,
-                            ).dict(exclude_none=True),
-                            model.Link(
-                                title="Item",
-                                href=self.url_for(
+                                "rel": "collection",
+                                "type": "application/json",
+                            },
+                            {
+                                "title": "Item",
+                                "href": self.url_for(
                                     request,
                                     "item",
                                     collectionId=collection.id,
                                     itemId=feature.get("id"),
                                 ),
-                                rel="item",
-                                type=MediaType.json,
-                            ).dict(exclude_none=True),
+                                "rel": "item",
+                                "type": "application/geo+json",
+                            },
                         ],
                     }
                     for feature in items["features"]
                 ],
             }
 
             # HTML Response
@@ -1152,31 +1147,31 @@
                             "Content-Disposition": "attachment;filename=items.ndjson"
                         },
                     )
 
             data = {
                 **feature,  # type: ignore
                 "links": [
-                    model.Link(
-                        href=self.url_for(
+                    {
+                        "href": self.url_for(
                             request, "collection", collectionId=collection.id
                         ),
-                        rel="collection",
-                        type=MediaType.json,
-                    ).dict(exclude_none=True),
-                    model.Link(
-                        href=self.url_for(
+                        "rel": "collection",
+                        "type": "application/json",
+                    },
+                    {
+                        "href": self.url_for(
                             request,
                             "item",
                             collectionId=collection.id,
                             itemId=itemId,
                         ),
-                        rel="self",
-                        type=MediaType.geojson,
-                    ).dict(exclude_none=True),
+                        "rel": "self",
+                        "type": "application/geo+json",
+                    },
                 ],
             }
 
             # HTML Response
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
@@ -1194,21 +1189,15 @@
 
     supported_tms: TileMatrixSets = default_tms
     with_viewer: bool = True
 
     @property
     def conforms_to(self) -> List[str]:
         """Factory conformances."""
-        return [
-            "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/core",
-            "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/oas30",
-            "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/mvt",
-            "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/tileset",
-            "http://www.opengis.net/spec/ogcapi-tiles-1/1.0/conf/tilesets-list",
-        ]
+        return TILES_CONFORMS
 
     def links(self, request: Request) -> List[model.Link]:
         """OGC Tiles API links."""
         return [
             model.Link(
                 title="Collection Vector Tiles",
                 href=self.url_for(
@@ -1287,37 +1276,37 @@
             output_type: Annotated[Optional[MediaType], Depends(OutputType)] = None,
         ):
             """
             OGC Specification: http://docs.opengeospatial.org/per/19-069.html#_tilematrixsets
             """
             data = model.TileMatrixSetList(
                 tileMatrixSets=[
-                    {
-                        "id": tms_id,
-                        "links": [
-                            {
-                                "href": self.url_for(
+                    model.TileMatrixSetRef(
+                        id=tms_id,
+                        title=f"Definition of {tms_id} tileMatrixSets",
+                        links=[
+                            model.TileMatrixSetLink(
+                                href=self.url_for(
                                     request,
                                     "tilematrixset",
                                     tileMatrixSetId=tms_id,
                                 ),
-                                "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
-                                "type": "application/json",
-                                "title": f"Definition of {tms_id} tileMatrixSets",
-                            }
+                                rel="http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
+                                type=MediaType.json,
+                            )
                         ],
-                    }
+                    )
                     for tms_id in self.supported_tms.list()
                 ]
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="tilematrixsets",
                 )
 
             return data
 
         @self.router.get(
             "/tileMatrixSets/{tileMatrixSetId}",
@@ -1345,18 +1334,23 @@
             """
             OGC Specification: http://docs.opengeospatial.org/per/19-069.html#_tilematrixset
             """
             data = self.supported_tms.get(tileMatrixSetId)
 
             if output_type == MediaType.html:
                 # For visualization purpose we add the tms bbox
-                data = {**data.dict(exclude_none=True), "bbox": data.bbox}
+                data = {
+                    **data.model_dump(exclude_none=True, mode="json"),
+                    "bbox": data.bbox,
+                }
                 return self._create_html_response(
                     request,
-                    json.dumps(data),
+                    json.dumps(
+                        data,
+                    ),
                     template_name="tilematrixset",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/tiles",
@@ -1384,67 +1378,69 @@
             if bounds := collection.bounds:
                 collection_bbox = {
                     "lowerLeft": [bounds[0], bounds[1]],
                     "upperRight": [bounds[2], bounds[3]],
                     "crs": "http://www.opengis.net/def/crs/OGC/1.3/CRS84",
                 }
 
-            data = model.TileSetList(
-                tilesets=[
-                    model.TileSet(
-                        title=f"'{collection.id}' tileset tiled using {tms} TileMatrixSet",
-                        dataType="vector",
-                        crs=self.supported_tms.get(tms).crs,
-                        boundingBox=collection_bbox,
-                        links=[
-                            {
-                                "href": self.url_for(
-                                    request,
-                                    "collection_tileset",
-                                    collectionId=collection.id,
-                                    tileMatrixSetId=tms,
-                                ),
-                                "rel": "self",
-                                "type": MediaType.json,
-                                "title": f"'{collection.id}' tileset tiled using {tms} TileMatrixSet",
-                            },
-                            {
-                                "href": self.url_for(
-                                    request,
-                                    "tilematrixset",
-                                    tileMatrixSetId=tms,
-                                ),
-                                "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
-                                "type": MediaType.json,
-                                "title": f"Definition of '{tms}' tileMatrixSet",
-                            },
-                            {
-                                "href": self.url_for(
-                                    request,
-                                    "collection_get_tile",
-                                    tileMatrixSetId=tms,
-                                    collectionId=collection.id,
-                                    z="{z}",
-                                    x="{x}",
-                                    y="{y}",
-                                ),
-                                "rel": "tile",
-                                "type": MediaType.mvt,
-                                "title": "Templated link for retrieving Vector tiles",
-                            },
-                        ],
-                    )
-                    for tms in self.supported_tms.list()
-                ]
+            data = model.TileSetList.model_validate(
+                {
+                    "tilesets": [
+                        {
+                            "title": f"'{collection.id}' tileset tiled using {tms} TileMatrixSet",
+                            "dataType": "vector",
+                            "crs": self.supported_tms.get(tms).crs,
+                            "boundingBox": collection_bbox,
+                            "links": [
+                                {
+                                    "href": self.url_for(
+                                        request,
+                                        "collection_tileset",
+                                        collectionId=collection.id,
+                                        tileMatrixSetId=tms,
+                                    ),
+                                    "rel": "self",
+                                    "type": "application/json",
+                                    "title": f"'{collection.id}' tileset tiled using {tms} TileMatrixSet",
+                                },
+                                {
+                                    "href": self.url_for(
+                                        request,
+                                        "tilematrixset",
+                                        tileMatrixSetId=tms,
+                                    ),
+                                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
+                                    "type": "application/json",
+                                    "title": f"Definition of '{tms}' tileMatrixSet",
+                                },
+                                {
+                                    "href": self.url_for(
+                                        request,
+                                        "collection_get_tile",
+                                        tileMatrixSetId=tms,
+                                        collectionId=collection.id,
+                                        z="{z}",
+                                        x="{x}",
+                                        y="{y}",
+                                    ),
+                                    "rel": "tile",
+                                    "type": "application/vnd.mapbox-vector-tile",
+                                    "title": "Templated link for retrieving Vector tiles",
+                                },
+                            ],
+                        }
+                        for tms in self.supported_tms.list()
+                    ]
+                }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="tilesets",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/tiles/{tileMatrixSetId}",
@@ -1469,14 +1465,15 @@
 
             if bounds := collection.bounds:
                 collection_bbox = {
                     "lowerLeft": [bounds[0], bounds[1]],
                     "upperRight": [bounds[2], bounds[3]],
                     "crs": "http://www.opengis.net/def/crs/OGC/1.3/CRS84",
                 }
+
                 tilematrix_limit = []
                 for matrix in tms:
                     ulTile = tms.tile(bounds[0], bounds[3], int(matrix.id))
                     lrTile = tms.tile(bounds[2], bounds[1], int(matrix.id))
                     minx, maxx = (min(ulTile.x, lrTile.x), max(ulTile.x, lrTile.x))
                     miny, maxy = (min(ulTile.y, lrTile.y), max(ulTile.y, lrTile.y))
                     tilematrix_limit.append(
@@ -1498,63 +1495,65 @@
                         "maxTileRow": matrix.matrixHeight,
                         "minTileCol": 0,
                         "maxTileCol": matrix.matrixWidth,
                     }
                     for matrix in tms
                 ]
 
-            data = model.TileSet(
-                title=f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
-                dataType="vector",
-                crs=tms.crs,
-                boundingBox=collection_bbox,
-                links=[
-                    {
-                        "href": self.url_for(
-                            request,
-                            "collection_tileset",
-                            collectionId=collection.id,
-                            tileMatrixSetId=tileMatrixSetId,
-                        ),
-                        "rel": "self",
-                        "type": MediaType.json,
-                        "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
-                    },
-                    {
-                        "href": self.url_for(
-                            request,
-                            "tilematrixset",
-                            tileMatrixSetId=tileMatrixSetId,
-                        ),
-                        "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
-                        "type": MediaType.json,
-                        "title": f"Definition of '{tileMatrixSetId}' tileMatrixSet",
-                    },
-                    {
-                        "href": self.url_for(
-                            request,
-                            "collection_get_tile",
-                            tileMatrixSetId=tileMatrixSetId,
-                            collectionId=collection.id,
-                            z="{z}",
-                            x="{x}",
-                            y="{y}",
-                        ),
-                        "rel": "tile",
-                        "type": MediaType.mvt,
-                        "title": "Templated link for retrieving Vector tiles",
-                    },
-                ],
-                tileMatrixSetLimits=tilematrix_limit,
+            data = model.TileSet.model_validate(
+                {
+                    "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
+                    "dataType": "vector",
+                    "crs": tms.crs,
+                    "boundingBox": collection_bbox,
+                    "links": [
+                        {
+                            "href": self.url_for(
+                                request,
+                                "collection_tileset",
+                                collectionId=collection.id,
+                                tileMatrixSetId=tileMatrixSetId,
+                            ),
+                            "rel": "self",
+                            "type": "application/json",
+                            "title": f"'{collection.id}' tileset tiled using {tileMatrixSetId} TileMatrixSet",
+                        },
+                        {
+                            "href": self.url_for(
+                                request,
+                                "tilematrixset",
+                                tileMatrixSetId=tileMatrixSetId,
+                            ),
+                            "rel": "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes",
+                            "type": "application/json",
+                            "title": f"Definition of '{tileMatrixSetId}' tileMatrixSet",
+                        },
+                        {
+                            "href": self.url_for(
+                                request,
+                                "collection_get_tile",
+                                tileMatrixSetId=tileMatrixSetId,
+                                collectionId=collection.id,
+                                z="{z}",
+                                x="{x}",
+                                y="{y}",
+                            ),
+                            "rel": "tile",
+                            "type": "application/vnd.mapbox-vector-tile",
+                            "title": "Templated link for retrieving Vector tiles",
+                        },
+                    ],
+                    "tileMatrixSetLimits": tilematrix_limit,
+                }
             )
 
             if output_type == MediaType.html:
                 return self._create_html_response(
                     request,
-                    data.json(exclude_none=True),
+                    data.model_dump_json(exclude_none=True),
                     template_name="tileset",
                 )
 
             return data
 
         @self.router.get(
             "/collections/{collectionId}/tiles/{tileMatrixSetId}/{z}/{x}/{y}",
```

### Comparing `tipg-0.3.1/tipg/main.py` & `tipg-0.4.0/tipg/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
 app.add_middleware(CacheControlMiddleware, cachecontrol=settings.cachecontrol)
 app.add_middleware(CompressionMiddleware)
 
 if settings.catalog_ttl:
     app.add_middleware(
         CatalogUpdateMiddleware,
+        func=register_collection_catalog,
         ttl=settings.catalog_ttl,
         schemas=db_settings.schemas,
         tables=db_settings.tables,
         exclude_tables=db_settings.exclude_tables,
         exclude_table_schemas=db_settings.exclude_table_schemas,
         functions=db_settings.functions,
         exclude_functions=db_settings.exclude_functions,
```

### Comparing `tipg-0.3.1/tipg/middleware.py` & `tipg-0.4.0/tipg/middleware.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """tipg middlewares."""
 
 import re
 from datetime import datetime, timedelta
-from typing import Any, Optional, Set
+from typing import Any, Optional, Protocol, Set
 
-from tipg.collections import register_collection_catalog
 from tipg.logger import logger
 
 from starlette.background import BackgroundTask
 from starlette.datastructures import MutableHeaders
 from starlette.requests import Request
 from starlette.types import ASGIApp, Message, Receive, Scope, Send
 
@@ -60,25 +59,36 @@
                         response_headers["Cache-Control"] = self.cachecontrol
 
             await send(message)
 
         await self.app(scope, receive, send_wrapper)
 
 
+class CatalogUpdateFunc(Protocol):
+    """Catalog update function protocol."""
+
+    def __call__(self, app: ASGIApp, **kwargs: Any) -> None:
+        """define input/output for the function."""
+        ...
+
+
 class CatalogUpdateMiddleware:
     """Middleware to update the catalog cache."""
 
     def __init__(
         self,
         app: ASGIApp,
+        *,
+        func: CatalogUpdateFunc,
         ttl: int = 300,
         **kwargs: Any,
     ) -> None:
         """Init Middleware."""
         self.app = app
+        self.func = func
         self.ttl = ttl
         self.kwargs = kwargs
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send):
         """Handle call."""
         if scope["type"] != "http":
             await self.app(scope, receive, send)
@@ -92,15 +102,15 @@
         if not last_updated or datetime.now() > (
             last_updated + timedelta(seconds=self.ttl)
         ):
             logger.debug(
                 f"Running catalog refresh in background. Last Updated: {last_updated}"
             )
             background = BackgroundTask(
-                register_collection_catalog,
+                self.func,
                 request.app,
                 **self.kwargs,
             )
 
         await self.app(scope, receive, send)
         if background:
             await background()
```

### Comparing `tipg-0.3.1/tipg/model.py` & `tipg-0.4.0/tipg/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 """tipg models."""
 
 from datetime import datetime
-from enum import Enum
-from typing import Dict, List, Literal, Optional, Tuple, Union
+from typing import Dict, List, Literal, Optional, Set, Tuple, Union
 
 from geojson_pydantic.features import Feature, FeatureCollection
 from morecantile.models import CRSType
-from pydantic import AnyHttpUrl, AnyUrl, BaseModel, Field, conint, root_validator
+from pydantic import AnyUrl, BaseModel, Field, RootModel, model_validator
+from typing_extensions import Annotated
 
 from tipg.resources.enums import MediaType
 
 
 class Link(BaseModel):
     """Link model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/common-core/link.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    href: str = Field(
-        ...,
-        description="Supplies the URI to a remote resource (or resource fragment).",
-        example="http://data.example.com/buildings/123",
-    )
-    rel: str = Field(
-        ..., description="The type or semantics of the relation.", example="alternate"
-    )
-    type: Optional[MediaType] = Field(
-        description="A hint indicating what the media type of the result of dereferencing the link should be.",
-        example="application/geo+json",
-    )
-    templated: Optional[bool] = Field(
-        description="This flag set to true if the link is a URL template."
-    )
-    varBase: Optional[str] = Field(
-        description="A base path to retrieve semantic information about the variables used in URL template.",
-        example="/ogcapi/vars/",
-    )
-    hreflang: Optional[str] = Field(
-        description="A hint indicating what the language of the result of dereferencing the link should be.",
-        example="en",
-    )
-    title: Optional[str] = Field(
-        description="Used to label the destination of a link such that it can be used as a human-readable identifier.",
-        example="Trierer Strasse 70, 53115 Bonn",
-    )
-    length: Optional[int]
+    href: Annotated[
+        str,
+        Field(
+            description="Supplies the URI to a remote resource (or resource fragment).",
+            example="http://data.example.com/buildings/123",
+        ),
+    ]
+    rel: Annotated[
+        str,
+        Field(
+            description="The type or semantics of the relation.", example="alternate"
+        ),
+    ]
+    type: Annotated[
+        Optional[MediaType],
+        Field(
+            description="A hint indicating what the media type of the result of dereferencing the link should be.",
+            example="application/geo+json",
+        ),
+    ] = None
+    templated: Annotated[
+        Optional[bool],
+        Field(description="This flag set to true if the link is a URL template."),
+    ] = None
+    varBase: Annotated[
+        Optional[str],
+        Field(
+            description="A base path to retrieve semantic information about the variables used in URL template.",
+            example="/ogcapi/vars/",
+        ),
+    ] = None
+    hreflang: Annotated[
+        Optional[str],
+        Field(
+            description="A hint indicating what the language of the result of dereferencing the link should be.",
+            example="en",
+        ),
+    ] = None
+    title: Annotated[
+        Optional[str],
+        Field(
+            description="Used to label the destination of a link such that it can be used as a human-readable identifier.",
+            example="Trierer Strasse 70, 53115 Bonn",
+        ),
+    ] = None
+    length: Optional[int] = None
 
-    class Config:
-        """Link model configuration."""
-
-        use_enum_values = True
+    model_config = {"use_enum_values": True}
 
 
 class Spatial(BaseModel):
     """Spatial Extent model.
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/extent.yaml
 
@@ -90,97 +105,85 @@
 class Extent(BaseModel):
     """Extent model.
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/extent.yaml
 
     """
 
-    spatial: Optional[Spatial]
-    temporal: Optional[Temporal]
+    spatial: Optional[Spatial] = None
+    temporal: Optional[Temporal] = None
 
 
 class Collection(BaseModel):
     """Collection model.
 
     Note: `CRS` is the list of CRS supported by the service not the CRS of the collection
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/collection.yaml
 
     """
 
     id: str
-    title: Optional[str]
-    description: Optional[str]
+    title: Optional[str] = None
+    description: Optional[str] = None
     links: List[Link]
-    extent: Optional[Extent]
+    extent: Optional[Extent] = None
     itemType: str = "feature"
     crs: List[str] = ["http://www.opengis.net/def/crs/OGC/1.3/CRS84"]
 
-    class Config:
-        """Collection model configuration."""
-
-        extra = "ignore"
+    model_config = {"extra": "ignore"}
 
 
 class Collections(BaseModel):
     """
     Collections model.
 
     Ref: http://beta.schemas.opengis.net/ogcapi/common/part2/0.1/collections/openapi/schemas/collections.yaml
 
     """
 
     links: List[Link]
-    timeStamp: Optional[str]
-    numberMatched: Optional[int]
-    numberReturned: Optional[int]
+    timeStamp: Optional[str] = None
+    numberMatched: Optional[int] = None
+    numberReturned: Optional[int] = None
     collections: List[Collection]
 
-    class Config:
-        """Collection model configuration."""
-
-        extra = "allow"
+    model_config = {"extra": "allow"}
 
 
 class Item(Feature):
     """Item model
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/featureGeoJSON.yaml
 
     """
 
-    links: Optional[List[Link]]
-
-    class Config:
-        """Link model configuration."""
+    links: Optional[List[Link]] = None
 
-        arbitrary_types_allowed = True
+    model_config = {"arbitrary_types_allowed": True}
 
 
 class Items(FeatureCollection):
     """Items model
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/featureCollectionGeoJSON.yaml
 
     """
 
     id: str
-    title: Optional[str]
-    description: Optional[str]
-    keywords: Optional[List[str]]
-    features: List[Item]  # type: ignore
-    links: Optional[List[Link]]
-    timeStamp: Optional[str]
-    numberMatched: Optional[int]
-    numberReturned: Optional[int]
+    title: Optional[str] = None
+    description: Optional[str] = None
+    keywords: Optional[List[str]] = None
+    features: List[Item]
+    links: Optional[List[Link]] = None
+    timeStamp: Optional[str] = None
+    numberMatched: Optional[int] = None
+    numberReturned: Optional[int] = None
 
-    class Config:
-        """Link model configuration."""
-
-        arbitrary_types_allowed = True
+    model_config = {"arbitrary_types_allowed": True}
 
     def json_seq(self, **kwargs):
         """return a GeoJSON sequence representation."""
         for f in self.features:
             yield f.json(**kwargs) + "\n"
 
 
@@ -197,452 +200,535 @@
 class Landing(BaseModel):
     """Landing page model.
 
     Ref: http://schemas.opengis.net/ogcapi/features/part1/1.0/openapi/schemas/landingPage.yaml
 
     """
 
-    title: Optional[str]
-    description: Optional[str]
+    title: Optional[str] = None
+    description: Optional[str] = None
     links: List[Link]
 
 
 class Queryables(BaseModel):
     """Queryables model.
 
     Ref: https://docs.ogc.org/DRAFTS/19-079r1.html#filter-queryables
 
     """
 
     title: str
     properties: Dict[str, Dict[str, str]]
     type: str = "object"
-    schema_name: str = Field(
-        "https://json-schema.org/draft/2019-09/schema", alias="$schema"
-    )
-    link: str = Field(..., alias="$id")
+    schema_name: Annotated[
+        str, Field(alias="$schema")
+    ] = "https://json-schema.org/draft/2019-09/schema"
+    link: Annotated[str, Field(alias="$id")]
+
+    model_config = {"populate_by_name": True}
 
 
 class TileMatrixSetLink(BaseModel):
     """
     TileMatrixSetLink model.
     Based on http://docs.opengeospatial.org/per/19-069.html#_tilematrixsets
     """
 
-    href: AnyHttpUrl
-    rel: str = "item"
+    href: str
+    rel: str = "http://www.opengis.net/def/rel/ogc/1.0/tiling-schemes"
     type: MediaType = MediaType.json
 
-    class Config:
-        """Config for model."""
-
-        use_enum_values = True
+    model_config = {"use_enum_values": True}
 
 
 class TileMatrixSetRef(BaseModel):
     """
     TileMatrixSetRef model.
     Based on http://docs.opengeospatial.org/per/19-069.html#_tilematrixsets
     """
 
     id: str
-    title: Optional[str]
+    title: Optional[str] = None
     links: List[TileMatrixSetLink]
 
 
 class TileMatrixSetList(BaseModel):
     """
     TileMatrixSetList model.
     Based on http://docs.opengeospatial.org/per/19-069.html#_tilematrixsets
     """
 
     tileMatrixSets: List[TileMatrixSetRef]
 
 
-class SchemeEnum(str, Enum):
-    """TileJSON scheme choice."""
-
-    xyz = "xyz"
-    tms = "tms"
-
-
 class LayerJSON(BaseModel):
     """
     https://github.com/mapbox/tilejson-spec/tree/master/3.0.0#33-vector_layers
     """
 
     id: str
-    fields: Dict = Field(default_factory=dict)
-    description: Optional[str]
-    minzoom: Optional[int]
-    maxzoom: Optional[int]
+    fields: Annotated[Dict, Field(default_factory=dict)]
+    description: Optional[str] = None
+    minzoom: Optional[int] = None
+    maxzoom: Optional[int] = None
 
 
 class TileJSON(BaseModel):
     """
     TileJSON model.
     Based on https://github.com/mapbox/tilejson-spec/tree/master/2.2.0
     """
 
     tilejson: str = "3.0.0"
-    name: Optional[str]
-    description: Optional[str]
+    name: Optional[str] = None
+    description: Optional[str] = None
     version: str = "1.0.0"
-    attribution: Optional[str]
-    template: Optional[str]
-    legend: Optional[str]
-    scheme: SchemeEnum = SchemeEnum.xyz
+    attribution: Optional[str] = None
+    template: Optional[str] = None
+    legend: Optional[str] = None
+    scheme: Literal["xyz", "tms"] = "xyz"
     tiles: List[str]
-    vector_layers: Optional[List[LayerJSON]]
-    grids: Optional[List[str]]
-    data: Optional[List[str]]
+    vector_layers: Optional[List[LayerJSON]] = None
+    grids: Optional[List[str]] = None
+    data: Optional[List[str]] = None
     minzoom: int = Field(0, ge=0, le=30)
     maxzoom: int = Field(30, ge=0, le=30)
-    fillzoom: Optional[int]
+    fillzoom: Optional[int] = None
     bounds: List[float] = [180, -85.05112877980659, 180, 85.0511287798066]
-    center: Optional[Tuple[float, float, int]]
+    center: Optional[Tuple[float, float, int]] = None
 
-    @root_validator
-    def compute_center(cls, values):
+    @model_validator(mode="after")
+    def compute_center(self):
         """Compute center if it does not exist."""
-        bounds = values["bounds"]
-        if not values.get("center"):
-            values["center"] = (
+        bounds = self.bounds
+        if not self.center:
+            self.center = (
                 (bounds[0] + bounds[2]) / 2,
                 (bounds[1] + bounds[3]) / 2,
-                values["minzoom"],
+                self.minzoom,
             )
-        return values
-
-    class Config:
-        """TileJSON model configuration."""
-
-        use_enum_values = True
+        return self
 
 
 class StyleJSON(BaseModel):
     """
     Simple Mapbox/Maplibre Style JSON model.
 
     Based on https://docs.mapbox.com/help/glossary/style/
 
     """
 
     version: int = 8
-    name: Optional[str]
-    metadata: Optional[Dict]
+    name: Optional[str] = None
+    metadata: Optional[Dict] = None
     layers: List[Dict]
     sources: Dict
     center: List[float] = [0, 0]
     zoom: int = 1
 
 
-class TimeStamp(BaseModel):
+class TimeStamp(RootModel):
     """TimeStamp model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/common-geodata/timeStamp.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    __root__: datetime = Field(
-        ...,
-        description="This property indicates the time and date when the response was generated using RFC 3339 notation.",
-        example="2017-08-17T08:05:32Z",
-    )
+    root: Annotated[
+        datetime,
+        Field(
+            description="This property indicates the time and date when the response was generated using RFC 3339 notation.",
+            example="2017-08-17T08:05:32Z",
+        ),
+    ]
 
 
 class BoundingBox(BaseModel):
     """BoundingBox model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/2DBoundingBox.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    lowerLeft: List[float] = Field(
-        ...,
-        max_items=2,
-        min_items=2,
-        description="A 2D Point in the CRS indicated elsewhere",
-    )
-    upperRight: List[float] = Field(
-        ...,
-        max_items=2,
-        min_items=2,
-        description="A 2D Point in the CRS indicated elsewhere",
-    )
-    crs: Optional[CRSType] = Field(name="CRS")
-    orderedAxes: Optional[List[str]] = Field(max_items=2, min_items=2)
-
-
-class Type(Enum):
-    """Type enum.
-
-    Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
-
-    Code generated using https://github.com/koxudaxi/datamodel-code-generator/
-    """
-
-    array = "array"
-    boolean = "boolean"
-    integer = "integer"
-    null = "null"
-    number = "number"
-    object = "object"
-    string = "string"
-
-
-class AccessConstraints(Enum):
-    """AccessConstraints enum.
-
-    Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
-
-    Code generated using https://github.com/koxudaxi/datamodel-code-generator/
-    """
-
-    unclassified = "unclassified"
-    restricted = "restricted"
-    confidential = "confidential"
-    secret = "secret"
-    topSecret = "topSecret"
+    lowerLeft: Annotated[
+        List[float],
+        Field(
+            max_length=2,
+            min_length=2,
+            description="A 2D Point in the CRS indicated elsewhere",
+        ),
+    ]
+    upperRight: Annotated[
+        List[float],
+        Field(
+            max_length=2,
+            min_length=2,
+            description="A 2D Point in the CRS indicated elsewhere",
+        ),
+    ]
+    crs: Annotated[Optional[CRSType], Field(name="CRS")] = None
+    orderedAxes: Annotated[
+        Optional[List[str]], Field(max_length=2, min_length=2)
+    ] = None
+
+
+# Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
+Type = Literal["array", "boolean", "integer", "null", "number", "object", "string"]
+
+# Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
+AccessConstraints = Literal[
+    "unclassified", "restricted", "confidential", "secret", "topSecret"
+]
 
 
 class Properties(BaseModel):
     """Properties model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    title: Optional[str]
-    description: Optional[str] = Field(description="Implements 'description'")
-    type: Optional[Type]
-    enum: Optional[List] = Field(
-        description="Implements 'acceptedValues'", min_items=1, unique_items=True
-    )
-    format: Optional[str] = Field(description="Complements implementation of 'type'")
-    contentMediaType: Optional[str] = Field(description="Implements 'mediaType'")
-    maximum: Optional[float] = Field(description="Implements 'range'")
-    exclusiveMaximum: Optional[float] = Field(description="Implements 'range'")
-    minimum: Optional[float] = Field(description="Implements 'range'")
-    exclusiveMinimum: Optional[float] = Field(description="Implements 'range'")
-    pattern: Optional[str]
-    maxItems: Optional[conint(ge=0)] = Field(  # type: ignore
-        description="Implements 'upperMultiplicity'"
-    )
-    minItems: Optional[conint(ge=0)] = Field(  # type: ignore
-        0, description="Implements 'lowerMultiplicity'"
-    )
-    observedProperty: Optional[str]
-    observedPropertyURI: Optional[AnyUrl]
-    uom: Optional[str]
-    uomURI: Optional[AnyUrl]
+    title: Optional[str] = None
+    description: Annotated[
+        Optional[str], Field(description="Implements 'description'")
+    ] = None
+    type: Optional[Type] = None
+    enum: Annotated[
+        Optional[Set],
+        Field(
+            description="Implements 'acceptedValues'",
+            min_length=1,
+        ),
+    ] = None
+    format: Annotated[
+        Optional[str],
+        Field(description="Complements implementation of 'type'"),
+    ] = None
+    contentMediaType: Annotated[
+        Optional[str], Field(description="Implements 'mediaType'")
+    ] = None
+    maximum: Annotated[Optional[float], Field(description="Implements 'range'")] = None
+    exclusiveMaximum: Annotated[
+        Optional[float], Field(description="Implements 'range'")
+    ] = None
+    minimum: Annotated[Optional[float], Field(description="Implements 'range'")] = None
+    exclusiveMinimum: Annotated[
+        Optional[float], Field(description="Implements 'range'")
+    ] = None
+    pattern: Optional[str] = None
+    maxItems: Annotated[
+        Optional[int],
+        Field(
+            description="Implements 'upperMultiplicity'",
+            ge=0,
+        ),
+    ] = None
+    minItems: Annotated[
+        Optional[int],
+        Field(
+            description="Implements 'lowerMultiplicity'",
+            ge=0,
+        ),
+    ] = 0
+    observedProperty: Optional[str] = None
+    observedPropertyURI: Optional[AnyUrl] = None
+    uom: Optional[str] = None
+    uomURI: Optional[AnyUrl] = None
 
 
 class PropertiesSchema(BaseModel):
     """PropertiesSchema model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/propertiesSchema.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
     type: Literal["object"]
-    required: Optional[List[str]] = Field(
-        description="Implements 'multiplicity' by citing property 'name' defined as 'additionalProperties'",
-        min_items=1,
-    )
+    required: Annotated[
+        Optional[List[str]],
+        Field(
+            description="Implements 'multiplicity' by citing property 'name' defined as 'additionalProperties'",
+            min_length=1,
+        ),
+    ] = None
     properties: Dict[str, Properties]
 
 
 class Style(BaseModel):
     """Style model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/style.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    id: str = Field(
-        ..., description="An identifier for this style. Implementation of 'identifier'"
-    )
-    title: Optional[str] = Field(description="A title for this style")
-    description: Optional[str] = Field(
-        description="Brief narrative description of this style"
-    )
-    keywords: Optional[List[str]] = Field(description="keywords about this style")
-    links: Optional[List[Link]] = Field(
-        description="Links to style related resources. Possible link 'rel' values are: 'style' for a URL pointing to the style description, 'styleSpec' for a URL pointing to the specification or standard used to define the style.",
-        min_items=1,
-    )
+    id: Annotated[
+        str,
+        Field(
+            description="An identifier for this style. Implementation of 'identifier'"
+        ),
+    ]
+    title: Annotated[Optional[str], Field(description="A title for this style")] = None
+    description: Annotated[
+        Optional[str], Field(description="Brief narrative description of this style")
+    ] = None
+    keywords: Annotated[
+        Optional[List[str]], Field(description="keywords about this style")
+    ] = None
+    links: Annotated[
+        Optional[List[Link]],
+        Field(
+            description="Links to style related resources. Possible link 'rel' values are: 'style' for a URL pointing to the style description, 'styleSpec' for a URL pointing to the specification or standard used to define the style.",
+            min_length=1,
+        ),
+    ] = None
 
 
 class GeospatialData(BaseModel):
     """Geospatial model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/geospatialData.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    title: Optional[str] = Field(
-        description="Title of this tile matrix set, normally used for display to a human",
-    )
-    description: Optional[str] = Field(
-        description="Brief narrative description of this tile matrix set, normally available for display to a human",
-    )
-    keywords: Optional[str] = Field(
-        description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this layer",
-    )
-    id: str = Field(
-        ...,
-        description="Unique identifier of the Layer. Implementation of 'identifier'",
-    )
-    dataType: Literal["map", "vector", "coverage"] = Field(
-        ..., description="Type of data represented in the tileset"
-    )
-    geometryDimension: Optional[conint(ge=0, le=3)] = Field(  # type: ignore
-        description="The geometry dimension of the features shown in this layer (0: points, 1: curves, 2: surfaces, 3: solids), unspecified: mixed or unknown",
-    )
-    featureType: Optional[str] = Field(
-        description="Feature type identifier. Only applicable to layers of datatype 'geometries'",
-    )
-    attribution: Optional[str] = Field(
-        description="Short reference to recognize the author or provider"
-    )
-    license: Optional[str] = Field(description="License applicable to the tiles")
-    pointOfContact: Optional[str] = Field(
-        description="Useful information to contact the authors or custodians for the layer (e.g. e-mail address, a physical address,  phone numbers, etc)",
-    )
-    publisher: Optional[str] = Field(
-        description="Organization or individual responsible for making the layer available",
-    )
-    theme: Optional[str] = Field(description="Category where the layer can be grouped")
-    crs: Optional[CRSType] = Field(name="CRS")
-    epoch: Optional[float] = Field(
-        description="Epoch of the Coordinate Reference System (CRS)"
-    )
-    minScaleDenominator: Optional[float] = Field(
-        description="Minimum scale denominator for usage of the layer"
-    )
-    maxScaleDenominator: Optional[float] = Field(
-        description="Maximum scale denominator for usage of the layer"
-    )
-    minCellSize: Optional[float] = Field(
-        description="Minimum cell size for usage of the layer"
-    )
-    maxCellSize: Optional[float] = Field(
-        description="Maximum cell size for usage of the layer"
-    )
-    maxTileMatrix: Optional[str] = Field(
-        description="TileMatrix identifier associated with the minScaleDenominator",
-    )
-    minTileMatrix: Optional[str] = Field(
-        description="TileMatrix identifier associated with the maxScaleDenominator",
-    )
-    boundingBox: Optional[BoundingBox]
-    created: Optional[TimeStamp]
-    updated: Optional[TimeStamp]
-    style: Optional[Style]
-    geoDataClasses: Optional[List[str]] = Field(
-        description="URI identifying a class of data contained in this layer (useful to determine compatibility with styles or processes)",
-    )
-    propertiesSchema: Optional[PropertiesSchema]
-    links: Optional[List[Link]] = Field(
-        description="Links related to this layer. Possible link 'rel' values are: 'geodata' for a URL pointing to the collection of geospatial data.",
-        min_items=1,
-    )
+    title: Annotated[
+        Optional[str],
+        Field(
+            description="Title of this tile matrix set, normally used for display to a human",
+        ),
+    ] = None
+    description: Annotated[
+        Optional[str],
+        Field(
+            description="Brief narrative description of this tile matrix set, normally available for display to a human",
+        ),
+    ] = None
+    keywords: Annotated[
+        Optional[str],
+        Field(
+            description="Unordered list of one or more commonly used or formalized word(s) or phrase(s) used to describe this layer",
+        ),
+    ] = None
+    id: Annotated[
+        str,
+        Field(
+            description="Unique identifier of the Layer. Implementation of 'identifier'"
+        ),
+    ]
+    dataType: Annotated[
+        Literal["map", "vector", "coverage"],
+        Field(description="Type of data represented in the tileset"),
+    ]
+    geometryDimension: Annotated[
+        Optional[int],
+        Field(  # type: ignore
+            description="The geometry dimension of the features shown in this layer (0: points, 1: curves, 2: surfaces, 3: solids), unspecified: mixed or unknown",
+            ge=0,
+            le=3,
+        ),
+    ] = None
+    featureType: Annotated[
+        Optional[str],
+        Field(
+            description="Feature type identifier. Only applicable to layers of datatype 'geometries'",
+        ),
+    ] = None
+    attribution: Annotated[
+        Optional[str],
+        Field(description="Short reference to recognize the author or provider"),
+    ] = None
+    license: Annotated[
+        Optional[str], Field(description="License applicable to the tiles")
+    ] = None
+    pointOfContact: Annotated[
+        Optional[str],
+        Field(
+            description="Useful information to contact the authors or custodians for the layer (e.g. e-mail address, a physical address,  phone numbers, etc)",
+        ),
+    ] = None
+    publisher: Annotated[
+        Optional[str],
+        Field(
+            description="Organization or individual responsible for making the layer available",
+        ),
+    ] = None
+    theme: Annotated[
+        Optional[str], Field(description="Category where the layer can be grouped")
+    ] = None
+    crs: Annotated[Optional[CRSType], Field(name="CRS")] = None
+    epoch: Annotated[
+        Optional[float],
+        Field(description="Epoch of the Coordinate Reference System (CRS)"),
+    ] = None
+    minScaleDenominator: Annotated[
+        Optional[float],
+        Field(description="Minimum scale denominator for usage of the layer"),
+    ] = None
+    maxScaleDenominator: Annotated[
+        Optional[float],
+        Field(description="Maximum scale denominator for usage of the layer"),
+    ] = None
+    minCellSize: Annotated[
+        Optional[float], Field(description="Minimum cell size for usage of the layer")
+    ] = None
+    maxCellSize: Annotated[
+        Optional[float], Field(description="Maximum cell size for usage of the layer")
+    ] = None
+    maxTileMatrix: Annotated[
+        Optional[str],
+        Field(
+            description="TileMatrix identifier associated with the minScaleDenominator",
+        ),
+    ] = None
+    minTileMatrix: Annotated[
+        Optional[str],
+        Field(
+            description="TileMatrix identifier associated with the maxScaleDenominator",
+        ),
+    ] = None
+    boundingBox: Optional[BoundingBox] = None
+    created: Optional[TimeStamp] = None
+    updated: Optional[TimeStamp] = None
+    style: Optional[Style] = None
+    geoDataClasses: Annotated[
+        Optional[List[str]],
+        Field(
+            description="URI identifying a class of data contained in this layer (useful to determine compatibility with styles or processes)",
+        ),
+    ] = None
+    propertiesSchema: Optional[PropertiesSchema] = None
+    links: Annotated[
+        Optional[List[Link]],
+        Field(
+            description="Links related to this layer. Possible link 'rel' values are: 'geodata' for a URL pointing to the collection of geospatial data.",
+            min_length=1,
+        ),
+    ] = None
 
 
 class TilePoint(BaseModel):
     """TilePoint model.
 
     Ref: https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/tilePoint.yaml
 
     Code generated using https://github.com/koxudaxi/datamodel-code-generator/
     """
 
-    coordinates: List[float] = Field(..., max_items=2, min_items=2)
-    crs: Optional[CRSType] = Field(name="CRS")
-    tileMatrix: Optional[str] = Field(
-        description="TileMatrix identifier associated with the scaleDenominator"
-    )
-    scaleDenominator: Optional[float] = Field(
-        description="Scale denominator of the tile matrix selected"
-    )
-    cellSize: Optional[float] = Field(
-        description="Cell size of the tile matrix selected"
-    )
+    coordinates: Annotated[List[float], Field(max_length=2, min_length=2)]
+    crs: Annotated[Optional[CRSType], Field(name="CRS")]
+    tileMatrix: Annotated[
+        Optional[str],
+        Field(description="TileMatrix identifier associated with the scaleDenominator"),
+    ] = None
+    scaleDenominator: Annotated[
+        Optional[float],
+        Field(description="Scale denominator of the tile matrix selected"),
+    ] = None
+    cellSize: Annotated[
+        Optional[float], Field(description="Cell size of the tile matrix selected")
+    ] = None
 
 
 class TileMatrixLimits(BaseModel):
     """
     The limits for an individual tile matrix of a TileSet's TileMatrixSet, as defined in the OGC 2D TileMatrixSet and TileSet Metadata Standard
 
     Based on https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/tileMatrixLimits.yaml
     """
 
     tileMatrix: str
-    minTileRow: int = Field(ge=0)
-    maxTileRow: int = Field(ge=0)
-    minTileCol: int = Field(ge=0)
-    maxTileCol: int = Field(ge=0)
+    minTileRow: Annotated[int, Field(ge=0)]
+    maxTileRow: Annotated[int, Field(ge=0)]
+    minTileCol: Annotated[int, Field(ge=0)]
+    maxTileCol: Annotated[int, Field(ge=0)]
 
 
 class TileSet(BaseModel):
     """
     TileSet model.
 
     Based on https://github.com/opengeospatial/ogcapi-tiles/blob/master/openapi/schemas/tms/tileSet.yaml
     """
 
-    title: Optional[str] = Field(description="A title for this tileset")
-    description: Optional[str] = Field(
-        description="Brief narrative description of this tile set"
-    )
-    dataType: Literal["map", "vector", "coverage"] = Field(
-        ..., description="Type of data represented in the tileset"
-    )
-    crs: CRSType = Field(..., name="CRS")
-    tileMatrixSetURI: Optional[AnyUrl] = Field(
-        description="Reference to a Tile Matrix Set on an official source for Tile Matrix Sets"
-    )
-    links: List[Link] = Field(description="Links to related resources")
-    tileMatrixSetLimits: Optional[List[TileMatrixLimits]] = Field(
-        description="Limits for the TileRow and TileCol values for each TileMatrix in the tileMatrixSet. If missing, there are no limits other that the ones imposed by the TileMatrixSet. If present the TileMatrices listed are limited and the rest not available at all",
-    )
-    epoch: Optional[Union[float, int]] = Field(
-        description="Epoch of the Coordinate Reference System (CRS)"
-    )
-    layers: Optional[List[GeospatialData]] = Field(min_items=1)
-    boundingBox: Optional[BoundingBox]
-    centerPoint: Optional[TilePoint]
-    style: Optional[Style]
-    attribution: Optional[str] = Field(
-        description="Short reference to recognize the author or provider"
-    )
-    license: Optional[str] = Field(description="License applicable to the tiles")
-    accessConstraints: Optional[AccessConstraints] = Field(
-        "unclassified",
-        description="Restrictions on the availability of the Tile Set that the user needs to be aware of before using or redistributing the Tile Set",
-    )
-    keywords: Optional[List[str]] = Field(description="keywords about this tileset")
-    version: Optional[str] = Field(
-        description="Version of the Tile Set. Changes if the data behind the tiles has been changed",
-    )
-    created: Optional[TimeStamp]
-    updated: Optional[TimeStamp]
-    pointOfContact: Optional[str] = Field(
-        description="Useful information to contact the authors or custodians for the Tile Set",
-    )
-    mediaTypes: Optional[List[str]] = Field(
-        description="Media types available for the tiles"
-    )
+    title: Annotated[
+        Optional[str], Field(description="A title for this tileset")
+    ] = None
+    description: Annotated[
+        Optional[str], Field(description="Brief narrative description of this tile set")
+    ] = None
+    dataType: Annotated[
+        Literal["map", "vector", "coverage"],
+        Field(description="Type of data represented in the tileset"),
+    ]
+    crs: Annotated[CRSType, Field(name="CRS")]
+    tileMatrixSetURI: Annotated[
+        Optional[AnyUrl],
+        Field(
+            description="Reference to a Tile Matrix Set on an official source for Tile Matrix Sets"
+        ),
+    ] = None
+    links: Annotated[
+        List[Link],
+        Field(description="Links to related resources"),
+    ]
+    tileMatrixSetLimits: Annotated[
+        Optional[List[TileMatrixLimits]],
+        Field(
+            description="Limits for the TileRow and TileCol values for each TileMatrix in the tileMatrixSet. If missing, there are no limits other that the ones imposed by the TileMatrixSet. If present the TileMatrices listed are limited and the rest not available at all",
+        ),
+    ] = None
+    epoch: Annotated[
+        Optional[Union[float, int]],
+        Field(description="Epoch of the Coordinate Reference System (CRS)"),
+    ] = None
+    layers: Annotated[
+        Optional[List[GeospatialData]],
+        Field(min_length=1),
+    ] = None
+    boundingBox: Optional[BoundingBox] = None
+    centerPoint: Optional[TilePoint] = None
+    style: Optional[Style] = None
+    attribution: Annotated[
+        Optional[str],
+        Field(description="Short reference to recognize the author or provider"),
+    ] = None
+    license: Annotated[
+        Optional[str], Field(description="License applicable to the tiles")
+    ] = None
+    accessConstraints: Annotated[
+        Optional[AccessConstraints],
+        Field(
+            description="Restrictions on the availability of the Tile Set that the user needs to be aware of before using or redistributing the Tile Set",
+        ),
+    ] = "unclassified"
+    keywords: Annotated[
+        Optional[List[str]], Field(description="keywords about this tileset")
+    ] = None
+    version: Annotated[
+        Optional[str],
+        Field(
+            description="Version of the Tile Set. Changes if the data behind the tiles has been changed",
+        ),
+    ] = None
+    created: Optional[TimeStamp] = None
+    updated: Optional[TimeStamp] = None
+    pointOfContact: Annotated[
+        Optional[str],
+        Field(
+            description="Useful information to contact the authors or custodians for the Tile Set",
+        ),
+    ] = None
+    mediaTypes: Annotated[
+        Optional[List[str]], Field(description="Media types available for the tiles")
+    ] = None
 
 
 class TileSetList(BaseModel):
     """
     TileSetList model.
 
     Based on https://docs.ogc.org/is/20-057/20-057.html#toc34
```

### Comparing `tipg-0.3.1/tipg/settings.py` & `tipg-0.4.0/tipg/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,203 +1,177 @@
 """tipg config."""
 
 import pathlib
-import sys
 from typing import Any, Dict, List, Optional
 
-import pydantic
+from pydantic import (
+    DirectoryPath,
+    Field,
+    FieldValidationInfo,
+    PostgresDsn,
+    field_validator,
+    model_validator,
+)
+from pydantic_settings import BaseSettings
+from typing_extensions import TypedDict
 
-# Pydantic does not support older versions of typing.TypedDict
-# https://github.com/pydantic/pydantic/pull/3374
-if sys.version_info < (3, 9, 2):
-    from typing_extensions import TypedDict
-else:
-    from typing import TypedDict
 
-
-class APISettings(pydantic.BaseSettings):
+class APISettings(BaseSettings):
     """API settings"""
 
     name: str = "TiPg: OGC Features and Tiles API"
     debug: bool = False
     cors_origins: str = "*"
     cachecontrol: str = "public, max-age=3600"
     template_directory: Optional[str] = None
 
     add_tiles_viewer: bool = True
 
     catalog_ttl: int = 300
 
-    @pydantic.validator("cors_origins")
+    model_config = {"env_prefix": "TIPG_", "env_file": ".env", "extra": "ignore"}
+
+    @field_validator("cors_origins")
     def parse_cors_origin(cls, v):
         """Parse CORS origins."""
         return [origin.strip() for origin in v.split(",")]
 
-    class Config:
-        """model config"""
-
-        env_prefix = "TIPG_"
-        env_file = ".env"
-
 
 class TableConfig(TypedDict, total=False):
     """Configuration to add table options with env variables."""
 
     geomcol: Optional[str]
     datetimecol: Optional[str]
     pk: Optional[str]
     properties: Optional[List[str]]
 
 
-class TableSettings(pydantic.BaseSettings):
+class TableSettings(BaseSettings):
     """Table configuration settings"""
 
     fallback_key_names: List[str] = ["ogc_fid", "id", "pkey", "gid"]
     table_config: Dict[str, TableConfig] = {}
     datetime_extent: bool = True
 
-    class Config:
-        """model config"""
-
-        env_prefix = "TIPG_"
-        env_file = ".env"
-        env_nested_delimiter = "__"
+    model_config = {
+        "env_prefix": "TIPG_",
+        "env_file": ".env",
+        "env_nested_delimiter": "__",
+        "extra": "ignore",
+    }
 
 
-class TMSSettings(pydantic.BaseSettings):
+class TMSSettings(BaseSettings):
     """TiPG TMS settings"""
 
     default_tms: str = "WebMercatorQuad"
     default_minzoom: int = 0
     default_maxzoom: int = 22
 
-    class Config:
-        """model config"""
-
-        env_prefix = "TIPG_"
-        env_file = ".env"
+    model_config = {"env_prefix": "TIPG_", "env_file": ".env", "extra": "ignore"}
 
 
-class FeaturesSettings(pydantic.BaseSettings):
+class FeaturesSettings(BaseSettings):
     """TiPG Items settings"""
 
-    default_features_limit: int = pydantic.Field(10, ge=0)
-    max_features_per_query: int = pydantic.Field(10000, ge=0)
+    default_features_limit: int = Field(10, ge=0)
+    max_features_per_query: int = Field(10000, ge=0)
 
-    class Config:
-        """model config"""
+    model_config = {"env_prefix": "TIPG_", "env_file": ".env", "extra": "ignore"}
 
-        env_prefix = "TIPG_"
-        env_file = ".env"
-
-    @pydantic.root_validator(pre=False)
-    def max_default(cls, values):
+    @model_validator(mode="after")
+    def max_default(self):
         """Set default bounds and srid when this is a function."""
-        if values.get("default_features_limit") > values.get("max_features_per_query"):
+        if self.default_features_limit > self.max_features_per_query:
             raise ValueError(
-                f"Invalid combination of `limit` ({values.get('default_features_limit')}) and `max features per query` ({values.get('max_features_per_query')}) values"
+                f"Invalid combination of `limit` ({self.default_features_limit}) and `max features per query` ({self.max_features_per_query}) values"
             )
 
-        return values
+        return self
 
 
-class MVTSettings(pydantic.BaseSettings):
+class MVTSettings(BaseSettings):
     """TiPG MVT settings"""
 
     tile_resolution: int = 4096
     tile_buffer: int = 256
     tile_clip: bool = True
     max_features_per_tile: int = 10000
 
-    set_mvt_layername: Optional[bool]
-
-    class Config:
-        """model config"""
+    set_mvt_layername: Optional[bool] = None
 
-        env_prefix = "TIPG_"
-        env_file = ".env"
+    model_config = {"env_prefix": "TIPG_", "env_file": ".env", "extra": "ignore"}
 
 
-class PostgresSettings(pydantic.BaseSettings):
+class PostgresSettings(BaseSettings):
     """Postgres connection settings.
 
     Attributes:
         postgres_user: postgres username.
         postgres_pass: postgres password.
         postgres_host: hostname for the connection.
         postgres_port: database port.
         postgres_dbname: database name.
 
     """
 
-    postgres_user: Optional[str]
-    postgres_pass: Optional[str]
-    postgres_host: Optional[str]
-    postgres_port: Optional[str]
-    postgres_dbname: Optional[str]
+    postgres_user: Optional[str] = None
+    postgres_pass: Optional[str] = None
+    postgres_host: Optional[str] = None
+    postgres_port: Optional[str] = None
+    postgres_dbname: Optional[str] = None
 
-    database_url: Optional[pydantic.PostgresDsn] = None
+    database_url: Optional[PostgresDsn] = None
 
     db_min_conn_size: int = 1
     db_max_conn_size: int = 10
     db_max_queries: int = 50000
     db_max_inactive_conn_lifetime: float = 300
 
-    class Config:
-        """model config"""
-
-        env_file = ".env"
+    model_config = {"env_file": ".env", "extra": "ignore"}
 
     # https://github.com/tiangolo/full-stack-fastapi-postgresql/blob/master/%7B%7Bcookiecutter.project_slug%7D%7D/backend/app/app/core/config.py#L42
-    @pydantic.validator("database_url", pre=True)
-    def assemble_db_connection(cls, v: Optional[str], values: Dict[str, Any]) -> Any:
+    @field_validator("database_url", mode="before")
+    def assemble_db_connection(cls, v: Optional[str], info: FieldValidationInfo) -> Any:
         """Validate db url settings."""
         if isinstance(v, str):
             return v
 
-        return pydantic.PostgresDsn.build(
+        return PostgresDsn.build(
             scheme="postgresql",
-            user=values.get("postgres_user"),
-            password=values.get("postgres_pass"),
-            host=values.get("postgres_host", ""),
-            port=values.get("postgres_port", 5432),
-            path=f"/{values.get('postgres_dbname') or ''}",
+            username=info.data.get("postgres_user"),
+            password=info.data.get("postgres_pass"),
+            host=info.data.get("postgres_host", ""),
+            port=info.data.get("postgres_port", 5432),
+            path=f"/{info.data.get('postgres_dbname') or ''}",
         )
 
 
-class DatabaseSettings(pydantic.BaseSettings):
+class DatabaseSettings(BaseSettings):
     """TiPg Database settings."""
 
     schemas: List[str] = ["public"]
-    tables: Optional[List[str]]
-    exclude_tables: Optional[List[str]]
-    exclude_table_schemas: Optional[List[str]]
-    functions: Optional[List[str]]
-    exclude_functions: Optional[List[str]]
-    exclude_function_schemas: Optional[List[str]]
+    tables: Optional[List[str]] = None
+    exclude_tables: Optional[List[str]] = None
+    exclude_table_schemas: Optional[List[str]] = None
+    functions: Optional[List[str]] = None
+    exclude_functions: Optional[List[str]] = None
+    exclude_function_schemas: Optional[List[str]] = None
 
     only_spatial_tables: bool = True
 
-    class Config:
-        """model config"""
+    model_config = {"env_prefix": "TIPG_DB_", "env_file": ".env", "extra": "ignore"}
 
-        env_prefix = "TIPG_DB_"
-        env_file = ".env"
 
-
-class CustomSQLSettings(pydantic.BaseSettings):
+class CustomSQLSettings(BaseSettings):
     """TiPg Custom SQL settings."""
 
-    custom_sql_directory: Optional[pydantic.DirectoryPath]
-
-    class Config:
-        """model config"""
+    custom_sql_directory: Optional[DirectoryPath]
 
-        env_prefix = "TIPG_"
-        env_file = ".env"
+    model_config = {"env_prefix": "TIPG_", "env_file": ".env", "extra": "ignore"}
 
     @property
     def sql_files(self) -> Optional[List[pathlib.Path]]:
         """return a list of SQL files within the custom sql directory."""
         if self.custom_sql_directory:
             return list(self.custom_sql_directory.glob("*.sql"))
```

### Comparing `tipg-0.3.1/tipg/filter/evaluate.py` & `tipg-0.4.0/tipg/filter/evaluate.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/filter/filters.py` & `tipg-0.4.0/tipg/filter/filters.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/resources/response.py` & `tipg-0.4.0/tipg/resources/response.py`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/sql/dbcatalog.sql` & `tipg-0.4.0/tipg/sql/dbcatalog.sql`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/collection.html` & `tipg-0.4.0/tipg/templates/collection.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/collections.html` & `tipg-0.4.0/tipg/templates/collections.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/conformance.html` & `tipg-0.4.0/tipg/templates/conformance.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/header.html` & `tipg-0.4.0/tipg/templates/header.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/item.html` & `tipg-0.4.0/tipg/templates/item.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/items.html` & `tipg-0.4.0/tipg/templates/items.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/landing.html` & `tipg-0.4.0/tipg/templates/landing.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/map.html` & `tipg-0.4.0/tipg/templates/map.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/queryables.html` & `tipg-0.4.0/tipg/templates/queryables.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/tilematrixset.html` & `tipg-0.4.0/tipg/templates/tilematrixset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/tilematrixsets.html` & `tipg-0.4.0/tipg/templates/tilematrixsets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/tileset.html` & `tipg-0.4.0/tipg/templates/tileset.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/tipg/templates/tilesets.html` & `tipg-0.4.0/tipg/templates/tilesets.html`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/.gitignore` & `tipg-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/LICENSE` & `tipg-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/README.md` & `tipg-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tipg-0.3.1/pyproject.toml` & `tipg-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,20 @@
     "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = ["version"]
 dependencies = [
     "orjson",
     "asyncpg>=0.23.0",
     "buildpg>=0.3",
-    "fastapi>=0.95.1",
+    "fastapi>=0.100.0",
     "jinja2>=2.11.2,<4.0.0",
-    "morecantile>=4.2,<5.0",
-    "pydantic[dotenv]~=1.0",
-    "geojson-pydantic>=0.4.3,<1.0",
+    "morecantile>=5.0,<6.0",
+    "pydantic~=2.0",
+    "pydantic-settings~=2.0",
+    "geojson-pydantic>=1.0,<2.0",
     "pygeofilter>=0.2.0,<0.3.0",
     "ciso8601~=2.3",
     "starlette-cramjam>=0.3,<0.4",
     "importlib_resources>=1.1.0; python_version < '3.9'",
     "typing_extensions; python_version < '3.9'",
 ]
```

### Comparing `tipg-0.3.1/PKG-INFO` & `tipg-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipg
-Version: 0.3.1
+Version: 0.4.0
 Summary: Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
 Project-URL: Homepage, https://developmentseed.org/tipg
 Project-URL: Source, https://github.com/developmentseed/tipg
 Project-URL: Documentation, https://developmentseed.org/tipg/
 Author-email: Vincent Sarago <vincent@developmentseed.org>, David Bitner <david@developmentseed.org>
 License: MIT License
         
@@ -37,21 +37,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Python: >=3.8
 Requires-Dist: asyncpg>=0.23.0
 Requires-Dist: buildpg>=0.3
 Requires-Dist: ciso8601~=2.3
-Requires-Dist: fastapi>=0.95.1
-Requires-Dist: geojson-pydantic<1.0,>=0.4.3
+Requires-Dist: fastapi>=0.100.0
+Requires-Dist: geojson-pydantic<2.0,>=1.0
 Requires-Dist: importlib-resources>=1.1.0; python_version < '3.9'
 Requires-Dist: jinja2<4.0.0,>=2.11.2
-Requires-Dist: morecantile<5.0,>=4.2
+Requires-Dist: morecantile<6.0,>=5.0
 Requires-Dist: orjson
-Requires-Dist: pydantic[dotenv]~=1.0
+Requires-Dist: pydantic-settings~=2.0
+Requires-Dist: pydantic~=2.0
 Requires-Dist: pygeofilter<0.3.0,>=0.2.0
 Requires-Dist: starlette-cramjam<0.4,>=0.3
 Requires-Dist: typing-extensions; python_version < '3.9'
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tipg Version: 0.3.1 Summary: Simple and Fast
+Metadata-Version: 2.1 Name: tipg Version: 0.4.0 Summary: Simple and Fast
 Geospatial OGC Features and Tiles API for PostGIS. Project-URL: Homepage,
 https://developmentseed.org/tipg Project-URL: Source, https://github.com/
 developmentseed/tipg Project-URL: Documentation, https://developmentseed.org/
 tipg/ Author-email: Vincent Sarago
 developmentseed.org>, David Bitner
 developmentseed.org> License: MIT License Copyright (c) 2022 Development Seed
 Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -22,32 +22,33 @@
 Features,OGC Tiles,POSTGIS Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS Requires-
 Python: >=3.8 Requires-Dist: asyncpg>=0.23.0 Requires-Dist: buildpg>=0.3
-Requires-Dist: ciso8601~=2.3 Requires-Dist: fastapi>=0.95.1 Requires-Dist:
-geojson-pydantic<1.0,>=0.4.3 Requires-Dist: importlib-resources>=1.1.0;
+Requires-Dist: ciso8601~=2.3 Requires-Dist: fastapi>=0.100.0 Requires-Dist:
+geojson-pydantic<2.0,>=1.0 Requires-Dist: importlib-resources>=1.1.0;
 python_version < '3.9' Requires-Dist: jinja2<4.0.0,>=2.11.2 Requires-Dist:
-morecantile<5.0,>=4.2 Requires-Dist: orjson Requires-Dist: pydantic
-[dotenv]~=1.0 Requires-Dist: pygeofilter<0.3.0,>=0.2.0 Requires-Dist:
-starlette-cramjam<0.4,>=0.3 Requires-Dist: typing-extensions; python_version <
-'3.9' Provides-Extra: dev Requires-Dist: pre-commit; extra == 'dev' Provides-
-Extra: docs Requires-Dist: mkdocs; extra == 'docs' Requires-Dist: mkdocs-
-material; extra == 'docs' Requires-Dist: pdocs; extra == 'docs' Requires-Dist:
-pygments; extra == 'docs' Provides-Extra: server Requires-Dist: uvicorn
-[standard]<0.19.0,>=0.12.0; extra == 'server' Provides-Extra: test Requires-
-Dist: httpx; extra == 'test' Requires-Dist: mapbox-vector-tile; extra == 'test'
-Requires-Dist: numpy; extra == 'test' Requires-Dist: protobuf<4.0,>=3.0; extra
-== 'test' Requires-Dist: psycopg2; extra == 'test' Requires-Dist: pytest; extra
-== 'test' Requires-Dist: pytest-asyncio; extra == 'test' Requires-Dist: pytest-
-benchmark; extra == 'test' Requires-Dist: pytest-cov; extra == 'test' Requires-
-Dist: pytest-pgsql; extra == 'test' Requires-Dist: sqlalchemy<1.4,>=1.1; extra
-== 'test' Description-Content-Type: text/markdown
+morecantile<6.0,>=5.0 Requires-Dist: orjson Requires-Dist: pydantic-
+settings~=2.0 Requires-Dist: pydantic~=2.0 Requires-Dist:
+pygeofilter<0.3.0,>=0.2.0 Requires-Dist: starlette-cramjam<0.4,>=0.3 Requires-
+Dist: typing-extensions; python_version < '3.9' Provides-Extra: dev Requires-
+Dist: pre-commit; extra == 'dev' Provides-Extra: docs Requires-Dist: mkdocs;
+extra == 'docs' Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist:
+pdocs; extra == 'docs' Requires-Dist: pygments; extra == 'docs' Provides-Extra:
+server Requires-Dist: uvicorn[standard]<0.19.0,>=0.12.0; extra == 'server'
+Provides-Extra: test Requires-Dist: httpx; extra == 'test' Requires-Dist:
+mapbox-vector-tile; extra == 'test' Requires-Dist: numpy; extra == 'test'
+Requires-Dist: protobuf<4.0,>=3.0; extra == 'test' Requires-Dist: psycopg2;
+extra == 'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-
+asyncio; extra == 'test' Requires-Dist: pytest-benchmark; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test' Requires-Dist: pytest-pgsql; extra
+== 'test' Requires-Dist: sqlalchemy<1.4,>=1.1; extra == 'test' Description-
+Content-Type: text/markdown
  [https://user-images.githubusercontent.com/10407788/204477834-2533241a-5927-
                           4f56-959e-4e8494027bc0.png]
       Simple and Fast Geospatial OGC Features and Tiles API for PostGIS.
                  [Test] [Coverage] [Package_version] [License]
 --- **Documentation**: https://developmentseed.org/tipg/ **Source Code**:
 https://github.com/developmentseed/tipg --- `tipg`, pronounced *T[ee]pg*, is a
 **python** package which helps creating lightweight OGC **Features** and
```

